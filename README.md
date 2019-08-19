# Bike Sharing Prediction
This project built a neural network using [Numpy](https://www.numpy.org/) to predict daily bike rental ridership with given features.

## Install
The project requires **Python** and the following libraries installed:
* [Numpy](https://www.numpy.org/)
* [Pandas](https://pandas.pydata.org/)
* [Matplotlib](https://matplotlib.org/)

It will also require a software installed to run and execute a [Jupyter Notebook](http://ipython.org/notebook.html)

If you do not have Python installed yet, it is highly recommended that you install the [Anaconda](https://www.anaconda.com/distribution/) distribution of Python, which already has the above packages and more included.

## Code
* Template code is provided in the `Predicting_bike_sharing_data.ipynb` notebook file.
* `Neural_Network.py`, `nn_testing.py` python file, dataset file in Bike-Sharing-Dataset folder are mandatory to complete the project. 

Note that the code included in `nn_testing.py` is meant to test the network architecture in `Neural_Netwrok.py`. 

## Run

Run `Neural_Network.py` before run `Predicting_bike_sharing_data.ipynb`


## Bike Sharing Dataset

Hadi Fanaee-T

Laboratory of Artificial Intelligence and Decision Support (LIAAD), University of Porto
INESC Porto, Campus da FEUP Rua Dr. Roberto Frias, 378 - 4200 - 465 Porto, Portugal

#### Data Set

Bike-sharing rental process is highly correlated to the environmental and seasonal settings. For instance, weather conditions, precipitation, day of week, season, hour of the day, etc. can affect the rental behaviors. The core data set is related to the two-year historical log corresponding to years 2011 and 2012 from Capital Bikeshare system, Washington D.C., USA which is publicly available in http://capitalbikeshare.com/system-data. We aggregated the data on two hourly and daily basis and then extracted and added the corresponding weather and seasonal information. Weather information are extracted from http://www.freemeteo.com. 



#### Files

 `Readme.txt`
`hour.csv` : bike sharing counts aggregated on hourly basis. Records: 17379 hours
`day.csv` : bike sharing counts aggregated on daily basis. Records: 731 days

	
#### Dataset characteristics
Both `hour.csv` and `day.csv` have the following fields, except hr which is not available in day.csv
	
* **instant**: record index
* **dteday **: date
* **season** : season (1:springer, 2:summer, 3:fall, 4:winter)
* **yr** : year (0: 2011, 1:2012)
* **mnth** : month ( 1 to 12)
* **hr** : hour (0 to 23)
* **holiday** : weather day is holiday or not (extracted from http://dchr.dc.gov/page/holiday-schedule)
* **weekday **: day of the week
* **workingday** : if day is neither weekend nor holiday is 1, otherwise is 0.
* **weathersit** : 
	* 1: Clear, Few clouds, Partly cloudy, Partly cloudy
	* 2: Mist + Cloudy, Mist + Broken clouds, Mist + Few clouds, Mist
	* 3: Light Snow, Light Rain + Thunderstorm + Scattered clouds, Light Rain + Scattered clouds
	* 4: Heavy Rain + Ice Pallets + Thunderstorm + Mist, Snow + Fog
* **temp** : Normalized temperature in Celsius. The values are divided to 41 (max)
* **atemp**: Normalized feeling temperature in Celsius. The values are divided to 50 (max)
* **hum**: Normalized humidity. The values are divided to 100 (max)
* **windspeed**: Normalized wind speed. The values are divided to 67 (max)
* **casual**: count of casual users
* **registered**: count of registered users
* **cnt**: count of total rental bikes including both casual and registered


#### License

Use of this dataset in publications must be cited to the following publication:

[1] Fanaee-T, Hadi, and Gama, Joao, "Event labeling combining ensemble detectors and background knowledge", Progress in Artificial Intelligence (2013): pp. 1-15, Springer Berlin Heidelberg, doi:10.1007/s13748-013-0040-3.



#### Contact

For further information about this dataset please contact Hadi Fanaee-T (hadi.fanaee@fe.up.pt)
