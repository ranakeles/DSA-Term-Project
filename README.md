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

6. **Conclusion & General Interpretation**
   
   This project aimed to investigate the potential relationship between global inflation rates and movie industry trends, focusing 	specifically on revenues and popular genres. By integrating data from the TMDB Movies dataset and the Global Inflation dataset, I conducted a detailed exploratory data analysis, statistical testing, and machine learning modeling.

	My analysis revealed that global inflation shows a weak to moderate negative correlation with average movie revenues, particularly during years of economic instability. However, the correlation is not strong enough to make conclusive causal claims.

	In terms of genre trends, inflation did not appear to have a direct or consistent influence on genre popularity. While minor fluctuations were observed in genre frequency over time, they are more likely to be driven by other cultural or economic factors.

	Through machine learning models, especially regression-based approaches, I was able to reasonably predict movie revenues based on features such as budget, runtime, and release year. Adding inflation as a feature showed only a small impact on prediction accuracy, reinforcing the idea that other variables have a stronger influence on box office outcomes.

	Overall, this project demonstrated the value of cross-domain data integration and the importance of combining statistical insight with machine learning to explore real-world trends.
	
