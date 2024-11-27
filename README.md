# VeloCityX Data Science Analysis

## Project Overview

This project focuses on analyzing user engagement data for **VeloCityX** to identify behavioral patterns and predict users' likelihood to purchase virtual merchandise. Using advanced data science techniques, we cleaned, processed, and analyzed the dataset to extract actionable insights. The findings were leveraged to propose a new fan challenge aimed at boosting user engagement and monetization.

---

## Objectives

1. Clean and process VeloCityX user engagement data.
2. Analyze correlations between user activities and virtual merchandise purchases.
3. Segment users using K-means clustering to identify behavior patterns.
4. Implement a Random Forest Classifier to predict merchandise purchase likelihood.
5. Propose a new fan challenge based on insights to increase engagement and revenue.

---

## Steps Involved

### 1. Understanding the Data
The dataset contains **7 features** across **100 records**:
- **User ID**: Categorical, unique identifier for each user.
- **Fan Challenges Completed**: Number of challenges users participated in.
- **Predictive Accuracy in Challenges**: User performance in challenges.
- **Virtual Merchandise Purchases**: Count of purchases.
- **Sponsorship Interactions**: Includes ad views and click-through rates.
- **Time Spent on "Live 360" Coverage**: Engagement with live streams.
- **Real-Time Chat Activity**: Interactions in the chat feature.

The dataset is clean with no missing or duplicate values. Preprocessing was minimal as features are mostly numeric.

---

### 2. Correlation Analysis
Correlation analysis was conducted to identify relationships between features. 

#### Key Findings:
- **Fan Challenges Completed**: Moderately correlated with virtual merchandise purchases, suggesting active participants are likely buyers.
- **Sponsorship Interactions**: Correlated with merchandise purchases, indicating engaged users are more likely to buy.
- **Real-Time Chat Activity**: Correlated with sponsorship interactions, highlighting user engagement trends.

---

### 3. K-means Clustering
**K-means clustering** was applied to segment users into groups based on behavior.

#### Clusters Formed:
1. **Cluster 1**: Users active in fan challenges and sponsorship interactions but with low accuracy.
2. **Cluster 2**: Users spending more time on "Live 360" and engaging in real-time chat.
3. **Cluster 3**: Users with high merchandise purchases and challenge accuracy.

#### Cluster Profiling:
- Cluster 2 users exhibit the highest interaction across all metrics and should be prioritized for marketing efforts.
- Merchandise purchase contribution:
  - Cluster 0: 41 purchases.
  - Cluster 1: 104 purchases.
  - Cluster 2: 122 purchases.

---

### 4. Predictive Modeling with Random Forest
A **Random Forest Classifier (RFC)** was implemented to predict whether a user will purchase merchandise. This model is highly effective for both classification and regression tasks.

#### Key Benefits of RFC:
- Handles missing data efficiently.
- Reduces overfitting and underfitting risks.
- Robust performance for imbalanced datasets.

#### Methodology:
- Dataset split into training and testing sets using **stratified sampling** to ensure equal representation of buyers and non-buyers.
- The model's performance was evaluated using metrics like accuracy and feature importance.

#### Key Insights:
- Users engaging in fan challenges, "Live 360" coverage, and sponsorship interactions are more likely to purchase merchandise.
- **Top Influential Features**:
  1. Predictive accuracy in fan challenges.
  2. Time spent on "Live 360".
  3. Sponsorship ad clicks.

---

### 5. Proposed Fan Base Challenge
To leverage insights from the analysis, a new interactive feature called **"Live 360 Fan Quest"** is proposed.

#### Challenge Description:
A game integrated with "Live 360" coverage to enhance engagement:
- **Real-Time Quizzes**:
  - Questions related to races, drivers, and teams.
  - Points awarded for correct answers with a live leaderboard.
- **Interactive Polls**:
  - Polls on ongoing race scenarios (e.g., predicting pit stops).
  - Instant results to foster community interaction.

#### Benefits:
- Increased user engagement through gamified experiences.
- Higher likelihood of virtual merchandise purchases.
- Boosted ad views and sponsorship interactions.

---

## Model Performance

The Random Forest Classifier performed exceptionally well, given the small dataset size. However, the limited dataset introduces a risk of overfitting, and results might vary with a larger dataset.

---

## Key Findings

1. **Engagement Insights**:
   - Users engaging in fan challenges and "Live 360" coverage are primary merchandise buyers.
   - Sponsorship interactions and chatbot usage are strong predictors of purchase likelihood.

2. **Proposed Solution**:
   - Focus on promoting fan challenges to boost user participation and predictive accuracy.
   - Enhance "Live 360" features with interactive elements to increase engagement.

3. **Caveat**:
   - Due to the small dataset, insights should be validated with a larger sample to ensure reliability.

---

## Tools and Technologies Used

- **Python Libraries**:
  - `pandas` for data manipulation.
  - `matplotlib` and `seaborn` for visualization.
  - `sklearn` for clustering and predictive modeling.
- **Algorithms**:
  - K-means clustering for segmentation.
  - Random Forest Classifier for prediction.

---

## Future Recommendations

1. **Scalability**:
   - Expand the dataset to include more user interactions for improved model accuracy.
   - Incorporate additional features like user demographics and regional data.

2. **Advanced Modeling**:
   - Test ensemble methods like Gradient Boosting or XGBoost for better predictions.
   - Use deep learning techniques for user behavior analysis on larger datasets.

3. **Enhanced Engagement**:
   - Introduce gamified elements in other app features.
   - Utilize user feedback to refine fan challenges and interactive polls.

---

## Conclusion

The **VeloCityX Data Science Analysis** provided valuable insights into user behavior, highlighting factors that influence virtual merchandise purchases. By segmenting users and leveraging predictive models, the proposed solutions aim to increase engagement and monetization, paving the way for enhanced user experiences and business outcomes.
