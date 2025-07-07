# 🏏 ODI Cricket Match Analysis and Prediction

This project presents a detailed data science pipeline applied to **One Day International (ODI) cricket matches**, including exploratory analysis, statistical testing, and machine learning-based predictive modeling. The analysis primarily focuses on India’s ODI performance, identifying patterns, strengths, weaknesses, and key predictors of match outcomes.

---

## 📁 Table of Contents

- [Project Overview](#project-overview)
- [Key Features](#key-features)
- [Dataset](#dataset)
- [Analyses Performed](#analyses-performed)
- [Machine Learning Models](#machine-learning-models)
- [Visualizations](#visualizations)
- [How to Run](#how-to-run)
- [Folder Structure](#folder-structure)
- [Results](#results)
- [Requirements](#requirements)
- [License](#license)

---

## 📌 Project Overview

This repository contains a complete cricket data science project pipeline applied to ODI matches, particularly focused on the Indian cricket team. The goals are:

- To understand performance patterns through data.
- To test statistical differences (e.g., economy rate in wins vs losses).
- To predict outcomes such as match win probability and bowler economy using machine learning.

---

## 🚀 Key Features

- 📊 Descriptive and Correlation Analysis
- 📈 Hypothesis Testing (T-tests, ANOVA)
- 🧠 Machine Learning Models:
  - XGBoost for Win Prediction
  - Random Forest for Economy Prediction
- 📉 Feature Importance Analysis
- 🗺️ Visualizations (Boxplots, Heatmaps, Line Graphs)
- 📅 Date & Opponent-based Slicing

---

## 📂 Dataset

- Source: Combined ODI cricket data scraped and cleaned manually
- File: `Combined final data.xlsx`
- Sheet: `India`
- Size: ~500+ records of India’s ODI matches

### Sample Columns:

| Column            | Description                               |
|-------------------|-------------------------------------------|
| `Winner`          | Match winner                              |
| `India Runs`      | Total runs scored by India                |
| `Ind_Eco_Win`     | Bowler economy rate when India wins       |
| `Ind_Eco_Loss`    | Bowler economy rate when India loses      |
| `India 4`, `India 6` | Number of 4s and 6s hit by India       |
| `Opp_Eco`         | Economy rate of the opponent bowlers      |

---

## 🔍 Analyses Performed

### 1. 🧮 Descriptive Analysis
- Mean, median, std deviation, and other aggregates on team and player performance.

### 2. 📈 Correlation Matrix
- Heatmap to find relationships between features like 4s, 6s, total runs, eco rate.

### 3. 🔬 Statistical Testing
- **T-Test**: Compared `Ind_Eco_Win` vs `Ind_Eco_Loss` to test economy effectiveness.
- **ANOVA**: Compared economy rate across multiple opponents to check significance.

---

## 🤖 Machine Learning Models

### ✅ Win Probability (Classification)
- **Model Used**: XGBoost
- **Input Features**: Toss, Runs, 4s, 6s, Opposition, Venue
- **Output**: Probability of India winning

### ✅ Economy Prediction (Regression)
- **Model Used**: Random Forest Regressor
- **Input Features**: Overs, Wickets, Match Venue, Opposition
- **Output**: Predicted economy rate of Indian bowlers

---

## 📊 Visualizations

- `boxplot`: Economy rate in wins vs losses
- `heatmap`: Correlation matrix of match features
- `barplot`: Wins vs Opponent
- `lineplot`: Economy rate trend over time

---

## ▶️ How to Run

1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/odi-cricket-analysis.git
   cd odi-cricket-analysis
