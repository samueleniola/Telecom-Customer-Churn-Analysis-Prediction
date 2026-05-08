# 📱 Telecom Customer Churn Analysis & Prediction

[![Python](https://img.shields.io/badge/Python-3.8+-blue.svg)](https://www.python.org/)
[![scikit-learn](https://img.shields.io/badge/scikit--learn-1.0+-orange.svg)](https://scikit-learn.org/)
[![Pandas](https://img.shields.io/badge/Pandas-1.3+-red.svg)](https://pandas.pydata.org/)
[![License](https://img.shields.io/badge/License-MIT-green.svg)](LICENSE)

> **Reduce customer churn by 30%+ using data-driven retention strategies**

## 📊 Project Overview

I analyzes **100,000+ telecom customers** (170,000+ data points) to identify churn patterns and build predictive models. The insights help reduce customer attrition through targeted retention campaigns.

### Key Business Impact
- ✅ **27%** current churn rate → **18%** target (33% reduction)
- ✅ **$5M+** annual revenue at risk identified
- ✅ **80%** of churn risk explained by just 3 factors
- ✅ **3.2x ROI** from highest-impact retention strategies

---

## 🎯 Problem Statement

Telecom companies lose **20-40% of customers annually** due to:
- Month-to-month contracts (5x higher churn than annual)
- Payment method friction (electronic check = 38% churn)
- Poor early customer experience (45% churn in first 6 months)

**Goal:** Predict which customers will churn and deliver actionable retention strategies.

---

## 📁 Dataset

### Source
Telecommunications customer data with 10,000+ customers (after cleaning) and 21 features.

### Key Features
| Feature | Type | Description |
|---------|------|-------------|
| `CustomerID` | ID | Unique identifier (dropped for modeling) |
| `Age` | Numeric | Customer age (18-80 years) |
| `Gender` | Categorical | Female / Male / Other |
| `Tenure` | Numeric | Months with company (1-72) |
| `MonthlyCharges` | Numeric | Monthly bill amount ($10-$150) |
| `TotalCharges` | Numeric | Lifetime charges (cleaned for negatives) |
| `Contract` | Categorical | Month-to-month / One year / Two year |
| `PaymentMethod` | Categorical | Electronic check / Mailed check / Bank transfer / Credit card |
| `Churn` | Target | Yes / No |

### Data Quality Notes
- ⚠️ `TotalCharges` had negative values (converted to `MonthlyCharges * Tenure`)
- ⚠️ Missing values handled via imputation
- ✅ No duplicate records found

---

## 🔍 Exploratory Data Analysis

### Key Findings

#### 1. Contract Type is #1 Predictor
