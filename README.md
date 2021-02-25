# anomaly-detection-by-deep-learning-wavelet-transform

# Project Goal:
Georgia Department of Transportation (GDOT) quantifies traveler data such as; speed, volume, count and vehicle class with two sperate systems.

*	continuous count station (CCS)
* video detection station (VDS) 

These two systems feature diverse approaches to collecting traveler data. VDS uses a deep learning algorithm applied to a live video feed while, CCS uses scales buried in the pavement to collect information. Each model possesses its differing inadequacy. Subsequentially, applied anomaly detection can be used to developed a more precise and resilient data source from the model sum.

# Methods:
This project featured extensive data collection, including web scraping more than 200 GB of data from a culmination of VDS, CCS and weather data. See my [previous repo]( https://github.com/clint-kristopher-morris/synthetic-parallel-selenium/edit/main/README.md) for information on techniques I developed to ameliorate web-scraping speed. 

After data collection VDS-CCS stations were geospatially matched with a k-nearest approach. Additionally, a weighted meshgrid of nearest weather stations was constructed for bilinear weather interpolation. Below shows a map of VDS (blue) and CCS (red) mapped. 

![](https://i.ibb.co/NsDXrGp/VDS-CCS2s.png)

![](https://i.ibb.co/JnDVyDK/waveletS.png)
