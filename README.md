# COVID-19_forecast{
 "cells": [
  {
   "cell_type": "markdown",
   "metadata": {},
   "source": [
    "# Covid-19 Forecast Project\n",
    "### Project Author: Man Yi (Ariel) Yeung\n",
    "\n",
    "### Project Objective:\n",
    "The project's objective is to analyze past Covid-19 data in the US by county in order to predict on COVID-19 confirmed cases and death counts in the near future.\n",
    "\n",
    "### Data Source:\n",
    "The datasets used are obtained from the <a href='https://github.com/CSSEGISandData/COVID-19/tree/master/csse_covid_19_data/csse_covid_19_time_series'>COVID-19 Data Repository by the Center for Systems Science and Engineering (CSSE) at Johns Hopkins University</a> , where COVID-19 data by county are compiled from different state and local department of health websites.\n",
    "\n",
    "### Datasets:\n",
    "- `time_series_covid19_confirmed_US.csv`: confirmed case counts in the US by county as of August 28, 2020 <a href='#r2'>[2]</a>\n",
    "- `time_series_covid19_deaths_US.csv`: death case counts in the US by county as of August 28, 2020 <a href='#r2'>[2]</a>\n",
    "\n",
    "### Project stages\n",
    "1. Data Preprocessing\n",
    "2. Exploratory Data Analysis (EDA)\n",
    "3. Use of Machine Learning Models<br/>\n",
    "&emsp; I. &nbsp; Autoregressive Integrated Moving Average (ARIMA) Model<br/>\n",
    "&emsp;II. &nbsp; Linear Regression Model\n",
    "4. Results and Discussion<br/>\n",
    "&emsp; I. &nbsp; Autoregressive Integrated Moving Average (ARIMA) Results<br/>\n",
    "&emsp;II. &nbsp; Linear Regression Results\n",
    "5. Conclusion\n",
    "6. Reference\n",
    "\n",
    "### Files:\n",
    "1. <a href='./Covid-19_Forecast.ipynb'>Covid-19_Forecast</a> is the main project report. It contains the objective and motivation of the project as well as all results and analysis process. It does not contain any code.\n",
    "2. <a href='./project_scoping_preprocessing_EDA.ipynb'>project_scoping_preprocessing_EDA</a> contains the project proposal and codes for data pre-processing and exploratory data analysis.\n",
    "3. <a href='./ARIMA_model.ipynb'>ARIMA_model</a> uses the ARIMA model to train and predict COVID-19 confirmed and death case counts in the US.\n",
    "4. <a href='./linear_regression_US.ipynb'>linear_regression_US</a> uses the linear regression model to train and predict COVID-19 confirmed and death case counts in the US.\n",
    "5. <a href='./linear_regression_county.ipynb'>linear_regression_county</a> uses the linear regression model to train and predict COVID-19 confirmed and death case counts in each US county.\n",
    "\n",
    "### Presentation Recordings:\n",
    "part-1:  https://1513041.mediaspace.kaltura.com/media/t/1_qdn6xuur\n",
    "\n",
    "part-2: https://1513041.mediaspace.kaltura.com/media/t/1_qxzi0ztk\n",
    "\n",
    "### Requirements:\n",
    "In order to run the project, the following libraries are needed:\n",
    "- pmdarima: this module can be installed by `'pip install pmdarima'`\n",
    "- Sklearn\n",
    "- Pandas\n",
    "- Matplotlib\n",
    "- Datetime\n",
    "- Math\n",
    "- Numpy\n",
    "- Collections\n",
    "- Warnings\n",
    "\n",
    "### Improvements, Challenges and Limitations:\n",
    "Improvements can be made to this project. For linear regression model, the forecast length is quite limiting, but increasing the forecasted period would significantly decrease the accuracy of the predictions. ARIMA models show more flexibility and has more capability to be adjust to fit the COVID-19 case counts, but the auto_arima method is limiting. Manual tuning of the parameters might be required to obtain a better fit. Another improvement can be to include factors other than the case count itself. These can include the social distancing rules, quarantine status, healthcare capacity, and so on.\n",
    "\n",
    "The challenge faced in this project lies primarily with fitting and implementing the machine learning models. With the ARIMA model, it is hard to tune the models to obtain an acceptable fitting. With linear regression model, the forecasting period is limited. Increasing the forecasting length would compromise the model accuracy. An important reason for why both models do not provide a highly acceptable predictions is because there are only 220 data points for each case considered, and about 15% of the data being extremely low in the beginning of the outbreak."
   ]
  }
 ],
 "metadata": {
  "kernelspec": {
   "display_name": "Python 3",
   "language": "python",
   "name": "python3"
  },
  "language_info": {
   "codemirror_mode": {
    "name": "ipython",
    "version": 3
   },
   "file_extension": ".py",
   "mimetype": "text/x-python",
   "name": "python",
   "nbconvert_exporter": "python",
   "pygments_lexer": "ipython3",
   "version": "3.7.7"
  }
 },
 "nbformat": 4,
 "nbformat_minor": 4
}
