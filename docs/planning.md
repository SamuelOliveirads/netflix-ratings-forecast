# Planning

## Criteria

- **Why is predicting ratings important?**
    Predicting ratings is crucial for decision-making at various stages of content production and release. While there are typically two types of ratings: consumer ratings and critic ratings, the following premise will enhance our understanding of this project's importance:
    > Netflix aims to improve its content quality and strengthen its relationship with viewers. A predictive rating model becomes an instrumental tool in this journey. Netflix has multiple projects at various stages:
    1. **Script Drafting**: Projects in this phase will be evaluated based on predicted ratings. Those with the highest predicted scores will be prioritized for further development, including filming and marketing.
    2. **Development**: Projects currently under development will also undergo rating predictions. Depending on the scores, decisions can be made, for instance, to accelerate or potentially pause certain projects to ensure optimal resource allocation.
    3. **Released Projects**: For projects that have already been launched, they won't be subjected to this prediction process as they've presumably been rated already. However, their actual ratings can serve as valuable data for refining the prediction model.

- **Defining a threshold for ratings:**
    Typically, ratings are in the range of 0 to 100. We need to define a threshold for what rating deems a movie worthy of making it to the catalog. While one could use external review sites, this process involves data collection, cleaning, and analysis. Thus, for simplicity, let's set a premise:
    > Movies with ratings above 50 are considered good enough to be added to the catalog.

- **Scope:**
    The focus here is solely on movies. Thus, we'll exclude other media types like TV shows.

## Output:
- A spreadsheet with the ranking of the films in their different stages
- Scenario simulations with resource allocation
- Evaluation of the model's performance and errors

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

6. **Feature Selection:**
    - Selection of the most relevant features for the model.

7. **Machine Learning:**
    - Test various models to determine which has the best predictive power for this specific task.

8. **Fine-Tuning:**
    - Refine the chosen model's hyperparameters to enhance its predictive capabilities.

9. **Business Performance Evaluation:**
    - Evaluate the model from a business perspective, considering its impact on Netflix's objectives and goals.
