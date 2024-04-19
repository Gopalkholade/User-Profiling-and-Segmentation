# User Profile Analysis and Segmentation

This Jupyter Notebook provides an exploratory data analysis (EDA) and user segmentation of a dataset containing user profiles for targeted advertising purposes.

## Dataset Exploration

* The script reads the `user_profiles_for_ads.csv` file assumed to be located in the `./Resources` directory.
* It provides an overview of the columns and identifies key user demographics, online behavior, and ad interaction metrics.

## Exploratory Data Analysis (EDA)

* Visualizations using `seaborn` showcase distributions of demographic variables (age, gender, device usage, education level, income), online behavior (time spent online, likes, click-through rates, conversion rates, ad interaction time), and top user interests.
* Key findings are highlighted in comments throughout the code.

## User Segmentation

* The code performs K-means clustering to segment users into distinct groups based on relevant features:
  * Age
  * Gender
  * Income Level
  * Time Spent Online (Weekdays and Weekends)
  * Likes and Reactions
  * Click-Through Rates (CTR)
* The script defines a preprocessing pipeline using `sklearn` to standardize numerical features and one-hot encode categorical features for effective clustering.
* Five user clusters are identified, and their characteristics are analyzed.

## Visualization

* A radar chart using `plotly` visually represents the average profiles of each user segment across key metrics, providing a clear comparison between segments.

## Further Insights and Recommendations

* The user profiles and segmentation results can be used to:
  * Develop targeted ad campaigns that resonate with specific user segments.
  * Optimize ad content and placement based on user demographics, interests, and online behavior.
  * Improve ad targeting strategies for better reach and conversion rates.

## Requirements

* Python 3.x
* pandas
* matplotlib
* seaborn
* warnings
* sklearn
* plotly.graph_objects

## How to Run

1. Ensure you have the required libraries installed (`pip install <library_name>`)
2. Save the code as a Jupyter Notebook (e.g., `user_profile_analysis.ipynb`)
3. Open the notebook in a Jupyter Notebook environment.
4. Run the cells sequentially to execute the code.

Note

* This is a sample analysis. Modify the code to explore additional features or create different visualizations based on your specific needs.
