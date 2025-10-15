# Instructions and Materials for Quiz 1

Complete information will appear here by 3 PM on Thursday 2025-10-16.

In the meantime, here is what is currently available for your review.

1. The complete Quiz instructions and questions document (pdf) will be posted later.
    - You can read the [current draft of instructions for students](431-2025-quiz1_instructions_only.pdf) now.
    - *Note that we'll delete this draft when it is replaced by the full document.*
2. Four data sets will be posted here later.
    - All of these files can be found in our **Shared Drive**, in the Quiz 1 folder's data subfolder.
    - Also, they can each be found [on our 431-data webpage](https://github.com/THOMASELOVE/431-data).
    - The data sets are:
        - [`q05.Rds`](https://github.com/THOMASELOVE/431-quizzes-2025/raw/refs/heads/main/quiz1/data/q05.Rds),
        - [`q09.csv`](https://raw.githubusercontent.com/THOMASELOVE/431-quizzes-2025/refs/heads/main/quiz1/data/q09.csv),
        - [`q13.xlsx`](https://github.com/THOMASELOVE/431-quizzes-2025/raw/refs/heads/main/quiz1/data/q13.xlsx) and
        - [`q18.csv`](https://raw.githubusercontent.com/THOMASELOVE/431-quizzes-2025/refs/heads/main/quiz1/data/q18.csv).
        - Another data set you might need is [`survey15_2014_to_2025.csv`](https://raw.githubusercontent.com/THOMASELOVE/431-quizzes-2025/refs/heads/main/quiz1/data/survey15_2014_to_2025.csv), which has been on [our 431-data page](https://github.com/THOMASELOVE/431-data) for a while now.
    - Here's a copy of the [Love-431.R](https://raw.githubusercontent.com/THOMASELOVE/431-quizzes-2025/refs/heads/main/quiz1/data/Love-431.R) script, too, just in case.
3. The Google Form Answer Sheet, where you will provide your responses, is found at <https://bit.ly/431-quiz-1-answer-sheet-2025>. This will open on 2025-10-16.
4. Below is a digital copy (so that you can copy and paste it into RStudio) of the list of R packages described in the instructions.

```
library(car)
library(DescTools)
library(Epi)
library(ggdist)
library(ggpubr)
library(glue)
library(infer)
library(janitor)
library(knitr)
library(MKinfer)
library(mosaic)
library(naniar)
library(patchwork)
library(readxl)
library(rstanarm)
library(easystats)
library(tidyverse)

source("data/Love-431.R")

theme_set(theme_bw())
knitr::opts_chunk$set(comment = NA)
```
