---
layout: single
title: EECinsights - CROP 2.0 nears completion
last_modified_at: 2022-02-17
author: "Rebecca"
author_profile: true
read_time: true
comments: true
share: true
related: true
excerpt: "A digital twin for the Growing Underground farm is unveiled with new functionality including temperature forecasting"
---
We have been developing a [Digital Twin](https://eeci.github.io/home/docs/projects/urbanag/digitaltwin/) for a unique hydroponic underground farm, [Growing Underground](https://growing-underground.com/) located in Clapham, South London.  

Initial development of the digital twin saw an enhanced visualisation platform created, [CROP - Crop Research Observation Platform](https://github.com/alan-turing-institute/CROP), in conjunction with the [Research Engineering Team](https://www.turing.ac.uk/research-engineering) from the [Alan Turing Institute](https://www.turing.ac.uk/).  CROP 2.0 is now nearing completion. This evolution includes further enhancements to the visualisation as well as incorporation of two embedded forecasting models.  

Previously, CROP showed instantaneous environmental conditions in the farm.  In CROP 2.0, the environmental conditions in the farm are also interpreted to show the number of hours over the previous day and week that the conditions have been within certain ranges. This is important for farm operation as it is the time that the crops spend in optimal temperatures that governs crop growth. As you hover over the sections of the graphic the bands are revealed - the figure showing that at the back of the farm the temperature has been between below 20 <sup>o</sup>C for 94 hours of the week.   

{% include figure image_path="/Images/CROP2Vis.jpg" alt="The CROP 2.0 dashboard with instantaneous and historic (daily and weekly) monitored environmental conditions in the farm" %}

The main developments though are the inclusion of two forecasting models.  The first is a temperature forecasting model that predicts temperatures through the farm based on historic temperatures and energy consumption data. 

{% include figure image_path="/Images/EECinsights/EECi_February_Arima.jpg" alt="Forecast and monitored temperatures in the farm" %}

The second forecasting model enables 'what-if' scenarios to be assessed. This is based on the physics-based [GES](https://eeci.github.io/home/docs/projects/urbanag/ges/) model.  The embedded model is calibrated using recent monitored data and then the calibrated model can be used to explore different operational conditions.  Here the scenario modelled is a reduction in ventilation rate to a constant 1ACH with a shift in the time at which the grow lights are switched on back by 3 hours, with a clear impact on the farm temperatures.  

{% include figure image_path="/Images/EECinsights/EECi_February_GESForecast.jpg" alt="Evaluation of operational scenario with a reduction in ventilation rate and earlier switching on of the grow lights" %}

The next stage of development will see crop growth and yield data being integrated within the digital twin.  This will allow us to combine data sources to explore optimal crop growth conditions for the different plants grown in the farm. 
