# Weight-Training-Workouts

## Overview
This project performs comprehensive data mining and analysis on a weightlifting dataset containing 721 workout sessions. The analysis explores patterns, relationships, and insights within workout data through multiple analytical approaches.

## Dataset
The dataset (`DataSet/weightlifting_721_workouts.csv`) contains:
- 9,932 records across 9,932 workout sets
- Dates and times of workouts
- Exercise names and categories
- Set details (weight, repetitions, duration, distance)

## Analysis Approaches

### 1. Association Rules Analysis
Identifies frequently co-occurring exercises and meaningful relationships between workout elements using the Apriori algorithm.

**Key findings:**
- "Chin Up" is the most frequent exercise (~34%), followed by "Squat (Barbell)" (~32%)
- Most frequent itemsets are single exercises, with few frequent exercise pairs
- Top association rules show relationships between specific exercise combinations

### 2. Clustering Analysis
Groups similar workout sessions to identify distinct training patterns using K-means, DBSCAN, and hierarchical clustering.

**Key findings:**
- Three distinct workout profiles identified:
  - Strength-focused workouts (higher weights, lower reps)
  - Endurance-focused workouts (more reps, lighter weights)
  - Balanced medium-intensity workouts
- DBSCAN identified outlier workout sessions that don't fit standard patterns

### 3. Decision Tree Analysis
Classifies and predicts workout characteristics based on input features.

**Key findings:**
- Repetition count is the strongest indicator for predicting heavy vs. regular sets
- For sets with low rep counts (≤5), weights tend to be significantly heavier
- Secondary factors (duration, distance) play a role in weight prediction for higher-rep sets

### 4. Regression Analysis
Models relationships between workout variables, particularly focusing on weight-repetition relationships.

**Key findings:**
- Negative correlation between repetitions and weight (R² ~0.14)
- Multiple regression with reps, seconds, and distance explains weight variation better than reps alone
- The relationship confirms the strength-endurance continuum in weightlifting

### 5. Statistical Analysis
Applies descriptive and inferential statistics to understand distributions and relationships in the dataset.

**Key findings:**
- Significant differences in weight used between exercise types (Deadlift > Squat > Bench Press)
- Weight typically increases from first to last set in a workout session
- High weights and high repetitions rarely occur together (confirmed by contingency tables)

## Conclusions
The analysis reveals meaningful patterns in workout behaviors:

1. Clear evidence of the strength-endurance tradeoff (higher weights correlate with lower reps)
2. Distinct workout styles identified through clustering correspond to different training objectives
3. Exercise selection shows preferences for core compound movements (Chin Up, Squat, etc.)
4. Weight progression within workouts follows expected patterns (typically increasing through sets)

## Copyright
Copyright La Vericii