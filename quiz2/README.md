# Instructions and Materials for Quiz 2

## Changes and Comments after Class 23

**Note**: If I need to make changes or provide comments on the Quiz after class 23 on 2025-11-20, that information will be posted here **and** emailed to all students.

## Everything you need will be available at 3 PM on 2025-11-20.

1. The complete[^1] [Quiz 2 instructions and questions document (pdf, 43 pages)] will be available by 3 PM.
2. The Google Form Answer Sheet, where you will provide your responses, is found at <https://bit.ly/431-2025-quiz2-answer-form>.
    - It is open now, and will remain open until 12:30 PM on Wednesday 2025-12-03.
3. The data sets relevant to the Quiz are now available.
    - All five Quiz 2 data sets (along with the `Love-431.R` script) are posted to the Quiz 2 folder on our Shared Drive in the data subfolder.
    - The data files are also available on our [431-data page](https://github.com/THOMASELOVE/431-data).
    - The data sets used in Quiz 2 are:
        - `hosp650.csv`
        - `kid_scr.Rds`
        - `rheuma.xlsx`
        - `wtchg1.xpt`
        - `wtchg2.Rds`
        - We'll also use the `survey15_2014_to_2025.csv` file which is found [at this link](https://raw.githubusercontent.com/THOMASELOVE/431-data/refs/heads/main/data/survey15_2014_to_2025.csv). A PDF of the survey itself is [found on our Class 2 README](https://github.com/THOMASELOVE/431-classes-2025/blob/main/class02/431_surveyhandout_1perstudent_2025-09-04.pdf).
4. There are two chunks of code that you should copy and paste into RStudio as you are preparing your responses.

- The first code chunk loads the R packages for the Quiz. 
    - It assumes that you have the `431-Love.R` script in a data subdirectory below your R Project for this Quiz.

```
#| message: false

library(broom)
library(car)
library(DescTools)
library(Epi)
library(GGally)
library(glue)
library(gt)
library(haven)
library(here)
library(infer)
library(janitor)
library(knitr)
library(mice)
library(MKinfer)
library(mosaic)
library(naniar)
library(olsrr)
library(patchwork)
library(readxl)
library(rstanarm)
library(easystats)
library(tidyverse)

source(here("data/Love-431.R"))

theme_set(theme_bw())
knitr::opts_chunk$set(comment = NA)
```

- The second bit of code you'll want is described in the Setup for Questions 3-16. Here it is.

```
url1 <- "https://raw.githubusercontent.com/THOMASELOVE/431-data/refs/heads/main/data/survey15_2014_to_2025.csv"

surv15 <- read_csv(url1, show_col_types = FALSE) |>
  janitor::clean_names() |>
  select(student, height_in, statfuture, english, haircut,
         smoke, hand_span, lecture, alone, lastsleep, 
         pulse, year) |>
  mutate(across(where(is.character), as_factor)) |>
  mutate(student = as.character(student),
         year = as_factor(year),
         smoke = fct_recode(factor(smoke), "Never" = "1",
                            "Former" = "2", "Current" = "3"))
```

Thanks, and good luck!
 
[^1]: It's a good idea to read the entire document, especially the footnotes, and including page 40.
