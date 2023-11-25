## <span style="color:green">Project Description</span>
This project was created to fulfill the Capstone requirement for the May 2023 session of ***Data Analytics with Python*** 
through [CodeLouisville](https://codekentucky.org/ "CodeKY"), now known as Code:You.

The purpose of this project is to take an inital look at what, if any, relationship exists between temperature and air quality index (AQI) in Louisville, Kentucky from January 1st, 1980 to December 31st, 2020.

There are two data files in this analysis. Both are from publically accessible sources. The first is the weather data from https://www.ncei.noaa.gov/access/search/data-search/daily-summaries?pageNum=1&bbox=38.417,-85.886,37.955,-85.424, and second is the AQI data from https://www.kaggle.com/datasets/threnjen/40-years-of-air-quality-index-from-the-epa-daily. The files included in the project have been trimmed down to make their sizes more managable, but the data cleaning process is performed within the air_quality.ipynb file.

## <span style="color:green">Project Features</span>
The following features are included in order to meet the requirements of the course:

1. Reading data from two CSV files.
2. The data is cleaned, merged, and used to calculate new values that further serve the analysis.
3. Visualization are included using matplotlib.
4. A requirements.txt file is included, as well as instructions for using a virtual environment while running the project.
5. This readme.md file, as well as comments and markdown cells throughout the project.
### Instructions
1. Clone the repo to your machine.
2. Create and activate a virtual environment and install the packages listed in the requirements.txt file. (instructions below)
3. Run the Jupyter Notebook 


### Virtual Environment Instructions
1. After you have cloned the repo to your machine, navigate to the project folder in GitBash/Terminal.
2. Create a virtual environment in the project folder.
3. Activate the virtual environment.
4. Install the required packages.
5. When you are done working on your repo, deactivate the virtual environment.

### Virtual Environment Commands

| Command    | Linux/Mac                       | GitBash                         |
|------------|---------------------------------|---------------------------------|
| Create     | python3 -m venv venv            | python -m venv venv             |
| Activate   | source venv/bin/activate        | source venv/Scripts/activate    |
| Install    | pip install -r requirements.txt | pip install -r requirements.txt |
| Deactivate | deactivate                      | deactivate      

## <span style="color:green">Interpretation and Analysis</span>
### Hyposthesis
My hypothesis for this project was that there would be a positive correlation between increasing temperature and increasing AQI. I believed that this would present itself as higher AQI's during summer months, and lower AQI's in winter months, generally, with some deviations. 
### Interpretation
The analysis showed that there is a positive correlation between AQI and temperature, but not a perfect one. There is a generally observable trend, but also instances where the two variables are less positively correlated. The general trend is observable by looking at the scatter plot comparing maximum, minimum, and average temperatures with the AQI for each day available in the dataset. 
This general trend was also observable in the bar charts, the first showing the average AQI per month for all years, and the second showing the average temperature per month for all years. The peaks of the two charts matched perfectly, with the highest AQI's appearing in the hottest months, June, July, and August. However, the relationship was not linear across all months. 
Another observation was how AQI fluctuates throughout the week. The idea was that perhaps car communting (more common during the weekdays) would have a noticable effect on AQI. The data showed a slight uptick in AQI from Monday - Friday, a drop on Saturday and a further drop on Sunday. Without further data on car use it is not possible to identify a cause and effect relationship here, but we do acknowledge the correlation. 
### Conclusion
In conclusion, there is a clear correlation between the hottest temperatures and the highest AQI's, but it appears that there are more weather variables that need to be considered in further analyses. As an inital exploratory analysis, I believe this project successfully identifies that there is a correlation worthy of further analysis between AQI and temperature. 
