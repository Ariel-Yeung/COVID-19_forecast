# Covid-19 Forecast Project
### Project Author: Man Yi (Ariel) Yeung

### Project Objective:
The project's objective is to analyze past Covid-19 data in the US by county in order to predict on COVID-19 confirmed cases and death counts in the near future.

### Data Source:
The datasets used are obtained from the <a href='https://github.com/CSSEGISandData/COVID-19/tree/master/csse_covid_19_data/csse_covid_19_time_series'>COVID-19 Data Repository by the Center for Systems Science and Engineering (CSSE) at Johns Hopkins University</a> , where COVID-19 data by county are compiled from different state and local department of health websites.

### Datasets:
- `time_series_covid19_confirmed_US.csv`: confirmed case counts in the US by county as of August 28, 2020 <a href='#r2'>[2]</a>
- `time_series_covid19_deaths_US.csv`: death case counts in the US by county as of August 28, 2020 <a href='#r2'>[2]</a>

### Project stages
1. Data Preprocessing
2. Exploratory Data Analysis (EDA)
3. Use of Machine Learning Models<br/>
&emsp; I. &nbsp; Autoregressive Integrated Moving Average (ARIMA) Model<br/>
&emsp;II. &nbsp; Linear Regression Model
4. Results and Discussion<br/>
&emsp; I. &nbsp; Autoregressive Integrated Moving Average (ARIMA) Results<br/>
&emsp;II. &nbsp; Linear Regression Results
5. Conclusion
6. Reference

### Files:
1. <a href='https://nbviewer.jupyter.org/github/Ariel-Yeung/COVID-19_forecast/blob/master/Covid-19_Forecast.ipynb#r1'>Covid-19_Forecast</a> is the <b>main project report</b>. It contains the objective and motivation of the project as well as all results and analysis process. It does not contain any code.
2. <a href='./project_scoping_preprocessing_EDA.ipynb'>project_scoping_preprocessing_EDA</a> contains the project proposal and codes for data pre-processing and exploratory data analysis.
3. <a href='./ARIMA_model.ipynb'>ARIMA_model</a> uses the ARIMA model to train and predict COVID-19 confirmed and death case counts in the US.
4. <a href='./linear_regression_US.ipynb'>linear_regression_US</a> uses the linear regression model to train and predict COVID-19 confirmed and death case counts in the US.
5. <a href='./linear_regression_county.ipynb'>linear_regression_county</a> uses the linear regression model to train and predict COVID-19 confirmed and death case counts in each US county.

### Requirements:
In order to run the project, the following libraries are needed:
- pmdarima: this module can be installed by `'pip install pmdarima'`
- Sklearn
- Pandas
- Matplotlib
- Datetime
- Math
- Numpy
- Collections
- Warnings
