# DSA-Term-Project

## Project Overview
In this project, I will analyze data from the TMDB Movies dataset and the Global Inflation dataset to see how global inflation rates affect movie revenues and popular genres. 

## Data Sources
1. **TMDB Movies Dataset:** [Movies.csv on data.world](https://data.world/patriciag/tmdb-data/workspace/file?filename=Movies.csv)
   - **Description:** This dataset contains information about movies, including budget, revenue, genres, and release dates.
   - **Use in Project:** Analyzing movie revenues and which genres are popular over time.

2. **Global Inflation Dataset:** [Global Inflation Data on Kaggle](https://www.kaggle.com/datasets/sazidthe1/global-inflation-data)
   - **Description:** It includes inflation rates from different countries over the years.
   - **Use in Project:** Comparing inflation rates with movie industry performance.

## Data Collection Plan

1. **Data Collection**
	-	**Sources:** TMDB Movies dataset and Global Inflation dataset were used from public platforms like data.world and Kaggle.
	-	The project focuses on the years 2000 to 2010 to align both datasets by year.


2. **Data Cleaning**
	-	**Merging:** Datasets were merged by matching each movie’s release year with the corresponding year in the inflation data.
	-	**Handling Missing Data:** Rows with missing or zero revenue were dropped, genre data was cleaned, and date formats were corrected.


3. **Exploratory Data Analysis (EDA)**
	-	**Visualization:** Bar charts, boxplots, scatter plots, and heatmaps were used to explore trends in revenue, genre, inflation, and production counts.
	-	**Statistics:** Summary statistics were calculated to better understand the distributions of revenue and inflation values.


4. **Hypothesis Testing**
	-	**Revenue Test:** A t-test was used to check if there’s a significant difference in average revenue between low and high-inflation years.
	-	**Genre Test:** A chi-square test was performed to examine if inflation level affects genre distribution.

5. **Machine Learning Methods**

	- 	**Regression:** A Linear Regression model was trained using inflation and movie-related features (vote count, rating, release year) to predict movie revenues. The model achieved an R² score of 0.73.

	-	 **Classification:** Multiple classification models (Logistic Regression, Decision Tree, Random Forest, KNN, XGBoost) were applied to classify movies as high or low revenue. Random Forest performed best with an accuracy of 80.3%.

	-	**Genre as a Feature:** Adding genre information improved classification accuracy to 81.8%, showing that genre helps predict revenue, even though it is not directly influenced by inflation.

	- 	**Genre as Target:** A separate model attempted to predict a movie’s genre based on inflation and numeric features, achieving only 24.9% accuracy. This supports the hypothesis that inflation does not determine genre popularity.

6. **Conclusion**
	
