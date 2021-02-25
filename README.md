# anomaly-detection-by-deep-learning-wavelet-transform

# Project Goal:
Georgia Department of Transportation (GDOT) quantifies traveler data such as; speed, volume, count and vehicle class with two sperate systems.

*	continuous count station (CCS)
* video detection station (VDS) 

These two systems feature diverse approaches to collecting traveler data. VDS uses a deep learning algorithm applied to a live video feed while, CCS uses scales buried in the pavement to collect information. Each model possesses its differing inadequacy. Subsequentially, applied anomaly detection can be used to developed a more precise and resilient data source from the model sum.

# Methods:
This project featured extensive data collection, including web scraping more than 200 GB of data from a culmination of VDS, CCS and weather data. See my [previous repo]( https://github.com/clint-kristopher-morris/synthetic-parallel-selenium/edit/main/README.md) for information on techniques I developed to ameliorate web-scraping speed. 

After data collection VDS-CCS stations were geospatially matched with a k-nearest approach. Additionally, a weighted meshgrid of nearest weather stations was constructed for bilinear weather interpolation. 

Below shows a map of VDS (blue) and CCS (red) mapped. 

![](https://i.ibb.co/NsDXrGp/VDS-CCS2s.png)

Analysis: 

Continuous wavelets were constructed for each day for both the CCS and VDS locations. To located errors Z-score values of the errors were also constructed. The image below shows;

* VDS wavelet for one station, on one day.
* CCS wavelet for a matched station.
* The errors among the stations

There is an obvious error in the VDS data, this error was due to inclement weather preventing the VDS station from correctly collecting traffic information. Due to errors like this weather data was also added as a third data source to explain other data variations.


![](https://i.ibb.co/JnDVyDK/waveletS.png)

# Results:
This project is currently underway...

# Tools:
* [Dask](https://docs.dask.org/en/latest/install.html)
* [Google Cloud Platform](https://cloud.google.com/) or alternatively you can use [Coiled](https://cloud.coiled.io/)
* Python 3.6
