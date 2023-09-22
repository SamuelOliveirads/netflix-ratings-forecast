# Planning

## Criteria

- **Why is predicting ratings important?**
    Predicting ratings can be crucial in various scenarios. Typically, there are two types of ratings: consumer ratings and critic ratings. To provide more depth to our problem, we can base it on the following premise:
    > Netflix aims to enhance its quality and relationship with its customers. For this, a predictive rating model is crucial. Once a rating is predicted, Netflix desires to take actionable insights. Let's assume Netflix has a series of projects in their early stages (script drafting) and wants to evaluate them. The ones with the highest predicted ratings would then be prioritized for further development like filming, marketing, etc. The goal is to maximize the number of movies on the platform that are well-received by the audience.

- **Defining a threshold for ratings:**
    Typically, ratings are in the range of 0 to 100. We need to define a threshold for what rating deems a movie worthy of making it to the catalog. While one could use external review sites, this process involves data collection, cleaning, and analysis. Thus, for simplicity, let's set a premise:
    > Movies with ratings above 50 are considered good enough to be added to the catalog.

- **Scope:**
    The focus here is solely on movies. Thus, we'll exclude other media types like TV shows.

## Output:
- Evaluation of model or models' performance, preferably using visual aids. There should be a rationale behind the metrics used and a comprehensive explanation of the results.
- An analysis of how your model adds value to Netflix's business.

## Input:
- Netflix database containing its catalog with the following attributes:
    'show_id', 'type', 'title', 'director', 'cast', 'country', 'date_added', 'release_year', 'rating', 'duration', 'listed_in', 'description'

## Process:
1. **Data Description:**
    - Perform a descriptive analysis and initial data cleaning.

2. **Row & Column Cleaning:**
    - Remove rows or columns that aren't relevant to the project's context.

3. **Feature Engineering:**
    - Creation and transformation of features to better suit the modeling phase.

4. **Exploratory Data Analysis (EDA):**
    - Univariate, bivariate, and multivariate analyses to understand data distributions, relationships, and anomalies.

5. **Data Preparation:**
    - Split the dataset into training and testing subsets.
    - Implement encodings for categorical variables and scale numerical attributes.

6. **Machine Learning:**
    - Test various models to determine which has the best predictive power for this specific task.

7. **Fine-Tuning:**
    - Refine the chosen model's hyperparameters to enhance its predictive capabilities.

8. **Business Performance Evaluation:**
    - Evaluate the model from a business perspective, considering its impact on Netflix's objectives and goals.
