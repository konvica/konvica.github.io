---
layout: page
title: About
permalink: /about/
---

**Machine Learning Developer, Data Scientist, Data Engineer, Data Analyst**

[comment]: <> (I develop End-to-End Machine Learning solutions, perform statistical analysis and econometric modelling. I engage in every step of the Machine Learning lifecycle, e.g. business understanding, data wrangling, model training, deployment, etc. I am able to work without close supervision and collaborate with a team. I have a Master’s degree in Applied Mathematics.)

I develop End-to-End Machine Learning solutions, perform statistical analysis and econometric modelling. I have worked on many projects in various domains such as healthcare, fintech, telco, IoT and more. I have engaged in every step of the Machine Learning Lifecycle from Business Understanding and Customer needs at the start to product Deployment or Visualization at the finish. As an Applied Mathematics graduate with a Master’s degree, I have a strong background in statistics, optimization, quantitative finance, econometrics and computer science.

Please look at my CV [here]({{ site.baseurl }}/resume.pdf) or github profile for examples of my work or contact me for more details on my experience.

## Summary of projects
Here is a brief summary of all projects I have worked on. The results vary from dockerized applications to presentations of results. They are ordered from the most recent. In addition, there are several smaller projects on my github repository or in the blog section of this page that are not listed here.

###### Detection of cut document
Specific personal identification documents are invalidated by cutting corners. We trained CNN segmentation model to localize document on image and employed computer vision techniques to validate all corners of the document. We had to account for various quality of photos and any kind of perspective rotation. We implemented a python microservice using `gRPC` and dockerized it.  

###### Air-quality and road meteorology IoT sensors
I worked on numerous data analyses and hypothesis tests of sensor accuracy. I designed a process to calibrate sensors of air quality using regression models and evaluated metrics in several environments (`stats-models`). I implemented a method to spatially interpolate road temperature from several static stations (`geopandas`,`pykrige`,`rasterio`,...). I created and managed TimescaleDB database to store measurements and results and visualized them in Grafana deployed on an in-house cloud (`docker`,`jenkins`,`DCOS`). 

###### Spatial estimation of traffic density
Some roads are manually monitored every 5 years. To estimate the rest I extracted publicly available map data features (population density, proximity to buildings, schools, factories, ...). I used regression kriging to spatially estimate traffic density for every unaccounted road.  (`pykrige`, `xgboost`, `geopandas`, `geospark`, `scipy.spatial` for spatial indexing). 

###### Uplift modelling - TELCO
Created a demo for estimating uplift - effect of giving an offer to a specific customer. In the end, we can choose the offer with the highest uplift for a customer. To estimate uplift we used causal modelling techniques - propensity score matching/weighting and causal trees. 

###### Cancer incidence rates prediction
National Cancer Registry periodically publishes reports on cancer statistics. Cancer incidence is one of the important statistics describing the number of new cases and is often used to describe historical trends. Predicting incidence rates for future years can help plan countermeasures for a specific population. We used the Age-Period-Cohort model framework with dropping insignificant factors to predict long-term incidence rates. Since cancer incidence is several years behind, we used external data for better short-term prediction.

###### Spoof detection
Spoof detection in face biometrics is the ability to detect if a face is real or fake (face printed on paper, displayed on screen). It was required to detect on static photo. Using `OpenCV` and `dlib` I extracted normalized face images without distorting texture or artifacts, that are present when the photo is fake. I trained 3 different computer vision models for spoof detection. First uses SVM to classify fakes based on texture, reflection, color and sharpness features. Second model is CNN classifier with random patch region extraction to prevent overfitting, due to limited training data. Last model was a fully convolutional network, that is trained to estimate 3D face depth. Both convolutional models performed reasonable well considering the input is just static photo. 

###### Classify fraud benefit claims
Due to the sensitive topic and data, I provide only a basic description. We trained `xgboost` classifier on highly categorical big data. The categories have a hierarchical structure, which is important to account for similarities between different categories. `Pyspark` was used for feature engineering. 

###### Banking Process Mining
Each application for a bank product undergoes an approval process. We used `pyspark` to extract features for each stage of the process and trained LSTM neural network (`tensorflow`) to predict the next steps of the process. 

###### Predict the demand for mortgages
Mortgage applications create load on the bank's back-office - risk approval, real estate check, ... Predicting demand for mortgages or the number of submitted applications several weeks ahead would help with back-office resource management and planning. 

###### Customer Relation Management data in TELCO
We looked for valuable insights from the Customer Relation Management (CRM) data of a telecommunication company. Using `nltk` and NLP techniques (tokenization, lemmatization and word embeddings), we extracted features from a free-text commentary of customer interaction with the company's employees. Using TSNE dimensionality reduction, we visualized customers in clusters.

###### Effectivity of healthcare providers based on economic data
We calculated the economic effectivity of healthcare using Data Envelopment Analysis (DEA). DEA models estimate an effectivity frontier by optimizing input and output matrices for each subject in analysis. DEA was done using `numpy` and `scipy.optimize`, data manipulation with `pyspark`. 

###### Bill of Materials (BOM) checking
Learning patterns from correct examples to find mistakes in new designs. [Read more]({{ site.baseurl }}/BOMvalidator)

###### Geospatial analytics of Industry machinery and vehicles
Company developing IoT devices to collect data from Industry machines including GPS coordinates looks to expand the analytics of the data. Clustering the location points to classify if the vehicle is working or detect construction sites and more. [Read more]({{ site.baseurl }}/GeoAnalytics)





















[comment]: <> ([kosik.matus@gmail.com]&#40;mailto:kosik.matus@gmail.com&#41;)