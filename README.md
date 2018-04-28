## Predicting MLB Free Agent Values

Welcome to my second Metis project, created in April 2018. In this project, we were tasked with using web-scraping tools to grab data and then create effective and accurate linear regression models to explore/predict continuous dependent variables. This project is known in Metis as "Project Luther"

I am a big baseball fan - go Mets! - so I decided to use this as an opportunity to explore free agent valuations in MLB. You'll see 8 Jupyter notebooks here, organized by task

### Section 1 - Scraping ESPN
* **Final 1 - ESPN Web Scrape.ipynb** - here I use Selenium to scrape ESPN for historical MLB free agent data

### Section 2 - Scraping Fangraphs
* **Final 2 - Fangraphs Scrape 1.ipynb**
* **Final 2.1 - Fangraphs Scrape 2.ipynb**
* **Final 2.2 - Fangraphs Scrape 3.ipynb**  
For these notebooks, I also used Selenium. I went through 3 of Fangraphs' major hitting statistical sections and grabbed every qualifying season by a hitter (and his respective statistics) for each page. It was substantially easier to keep these scrapes separate and combine data afterwards, which is why there are 3 notebooks doing almost the same thing here.

### Section 3 - Data Cleaning and Merging
* **Final 3 - Data Cleaning and Combining.ipynb**
* * **Final 3.1 - Non_FA Data Clean and Merge.ipynb**   
Here I used Pandas to combine the above datasets into 2 main dataframes. One would join free agent data with hitting data. This would be the engine to then model off of. The second notebook is for cleaning the hitting stats of the rest of the MLB. I ultimately used this as test data for my model to see if its predictions aligned with common sense Values

### Section 4 - Exploratory Data Analysis
* **Final 4 - Exploratory Data Analysis.ipynb**  
This was my space to explore bivariate relationships within the data, as well as to aggregate statistics across different groupings

### Section 5 - Modeling
* **Final 5 - Regression Analysis**  
Using my cleaned datasets, I present here the most effective model I could design across numerous features. Attempts had been made using regularization, polynomial processing and other tactics, but ultimately none approached the test/train $r^2$ of the model presented here. I then use this model to predict free agent values for young players Michael Conforto (OF, NY Mets) and Joe Panik (2B, SF Giants)  

As always, please let me know if you have any questions or comments!

-Brian
