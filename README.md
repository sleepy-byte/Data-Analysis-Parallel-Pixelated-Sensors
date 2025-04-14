# Parallel Pixelated Sensor Analysis in R

This project involves analyzing particle detector data from two 8×8 pixel sensor matrices using R. Each row in the dataset represents a single event and contains the recorded signals for all 128 pixels (64 upstream + 64 downstream).


## Dataset Structure

- The dataset used for this project is available here: https://drive.google.com/file/d/1dYPF5tL3qnBmTVbavyKbPQ0Qooi_CCE1V/view?usp=sharing
- Columns 1–64: Upstream matrix pixel values  
- Columns 65–128: Downstream matrix pixel values  
- Pixel indices are calculated as:

## Objectives

For each event:
1. Detect and handle any missing data
2. Identify the **maximum** and **second maximum** pixel signals for both matrices
3. Extract the corresponding **pixel indices**
4. Visualize index distributions for the top signals
5. Repeat the analysis excluding events with maximum signal < 10
6. Calculate the **ratio** between the top two pixel values (when both > 0)

## Tools Used

- R
- `dplyr`, `tidyverse`
- `ggplot2`

## Outputs

- Histograms of pixel indices (max and second max)
- Heatmap of frequency of pixel maximum
- Filtered signal distribution plots
- Ratio distribution of second-to-first max values

## How to Run

1. Load the dataset (CSV)
2. Open the R script or R Markdown / Notebook (`.Rmd` or `.ipynb`)
3. Run the analysis in RStudio

## Author

Developed for training in scientific data analysis with applications in particle physics.
