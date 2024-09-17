# Data Wrangling and Visualization in Python

## Overview
 The goal of the project is to perform **data wrangling** and **data visualization** using the provided **ECE Board Exam dataset**. The analysis is carried out using Python and the following libraries: `pandas`, `matplotlib`, and `seaborn`.

---

## Table of Contents

- [Overview](#overview)
- [Dataset](#dataset)
- [Intended Learning Outcomes](#intended-learning-outcomes)
- [Installation](#installation)
- [Instructions](#instructions)
  - [Task 1: Data Wrangling](#task-1-data-wrangling)
  - [Task 2: Data Visualization](#task-2-data-visualization)
- [Results](#results)
  - [Instru DataFrame](#instru-dataframe)
  - [Mindy DataFrame](#mindy-dataframe)
- [Visualizations](#visualizations)
- [References](#references)

---

## Dataset

The dataset used for this project contains student records from **ECE Board Exams**. You can download the dataset from the provided link: [ECE Board Exam Dataset](bit.ly/ECEBoardExamDataset).

The dataset includes the following features:
- `Name`: The name of the student
- `Gender`: Gender of the student
- `Track`: The academic track chosen by the student (e.g., Instrumentation, Communication)
- `Math`, `GEAS`, `Electronics`: Scores in respective subjects
- `Hometown`: Region of origin (e.g., Luzon, Visayas, Mindanao)

---

## Intended Learning Outcomes

1. Understand how to use Python libraries for data wrangling (i.e., `pandas`) and data visualization (i.e., `matplotlib`, `seaborn`).
2. Learn to clean, manipulate, and transform datasets into useful information.
3. Create visual representations that tell a story about the dataset.

---

## Instructions

### Task 1: Data Wrangling

In this task, you need to create specific subsets of the dataset based on the following conditions:

1. **Instru DataFrame**: Extract rows where:
   - The `Track` is **Instrumentation**.
   - The `Hometown` is **Luzon**.
   - The `Electronics` score is greater than 70.

   **Example Output:**
   | Name  | GEAS | Electronics |
   |-------|------|-------------|
   | S6    | 90   | 82          |
   | S10   | 70   | 79          |

2. **Mindy DataFrame**: Extract rows where:
   - The `Gender` is **Female**.
   - The `Hometown` is **Mindanao**.
   - The `Average` score is 55 or higher.

   To calculate the `Average`, use the following formula:
   ```python
   data['Average'] = data[['Math', 'GEAS', 'Electronics']].mean(axis=1)
## Data Visualization

In this task, you need to create visualizations to analyze how different features contribute to the average grade:

1. **Track vs. Average Grade**: Create a plot to show how the average grade varies with different academic tracks.
2. **Gender vs. Average Grade**: Create a plot to compare the average grades of male and female students.
3. **Hometown vs. Average Grade**: Create a plot to compare the average grades of students from different hometowns (e.g., Luzon, Visayas, Mindanao).

The visualizations should be created using `matplotlib` and `seaborn` libraries. Save the visualizations as image files (e.g., PNG) and place them in the `images/` directory.

---

## Results

### Instru DataFrame

Filtered results where:
- Track is "Instrumentation"
- Hometown is "Luzon"
- Electronics score > 70

| Name  | GEAS | Electronics |
|-------|------|-------------|
| S6    | 90   | 82          |
| S10   | 70   | 79          |

### Mindy DataFrame

Filtered results where:
- Gender is "Female"
- Hometown is "Mindanao"
- Average score ≥ 55

| Name | Track          | Electronics | Average |
|------|----------------|-------------|---------|
| S5   | Communication  | 69          | 79.33   |
| S7   | Communication  | 73          | 68.67   |

---
## Changelogs
1. Added a readme file
2. Edited readme file
3. Reworked on the phython code
4. Added code for the graph for part 2

---




