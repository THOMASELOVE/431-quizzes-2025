# Instructions and Materials for Quiz 1

## Changes since Class 14 ended

- 2025-10-17 I had somehow provided the (slightly) wrong **q05.rds**. The originally posted one had two variables, named `subject` and `result`. The correct one contains two variables, named `subject` and `score`. Now, the new version of [q05.rds is here](https://github.com/THOMASELOVE/431-quizzes-2025/raw/refs/heads/main/quiz1/data/q05.Rds), and on [our 431-data page](https://github.com/THOMASELOVE/431-data), and in our [Shared Drive](https://thomaselove.github.io/431-2025/google.html). Changing to this corrected version of the **q05.rds** should not change your answer to Question 5 at all, but it will work with the published code properly without you having to edit the variable name. Editing the name of the variable from `result` to `score` is **not** one of the two necessary changes we want you to list in your response to Question 5.

## What is posted?

Everything is now available.

1. The complete [Quiz instructions and questions document](https://github.com/THOMASELOVE/431-quizzes-2025/blob/main/quiz1/431-2025-quiz1.pdf) (pdf, 33 pages) is now available.
    - The instructions section is slightly different than what was posted previously, but only slightly.
2. All provided data sets are now available.
    - All of the files listed here can also be found in our **Shared Drive**, in the Quiz 1 folder's data subfolder, and on [on our 431-data webpage](https://github.com/THOMASELOVE/431-data).
    - The Quiz 1 data sets are:
        - [`q05.Rds`](https://github.com/THOMASELOVE/431-quizzes-2025/raw/refs/heads/main/quiz1/data/q05.Rds),
        - [`q09.csv`](https://raw.githubusercontent.com/THOMASELOVE/431-quizzes-2025/refs/heads/main/quiz1/data/q09.csv),
        - [`q13.xlsx`](https://github.com/THOMASELOVE/431-quizzes-2025/raw/refs/heads/main/quiz1/data/q13.xlsx) and
        - [`q18.csv`](https://raw.githubusercontent.com/THOMASELOVE/431-quizzes-2025/refs/heads/main/quiz1/data/q18.csv).
        - Another data set (for Question 27) that you might need is [`survey15_2014_to_2025.csv`](https://raw.githubusercontent.com/THOMASELOVE/431-quizzes-2025/refs/heads/main/quiz1/data/survey15_2014_to_2025.csv), which has been on [our 431-data page](https://github.com/THOMASELOVE/431-data) for a while now.
    - Here's a copy of the [Love-431.R](https://raw.githubusercontent.com/THOMASELOVE/431-quizzes-2025/refs/heads/main/quiz1/data/Love-431.R) script, too, just in case.
3. The Google Form Answer Sheet, where you will provide your responses, is found at <https://bit.ly/431-quiz-1-answer-sheet-2025>. It is now open.
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
