## Project: Bicycle Karma: Predicting and tracking bike theft

#### Team: Holmes

#### Course: CS 109

#### Term: Fall 2015

#### [Project URL](https://sites.google.com/a/g.harvard.edu/bicyclekarma/home)

#### [Project screencast](https://sites.google.com/a/g.harvard.edu/bicyclekarma/home/screencast)



------

### Prelude

Bicycle theft has become a glaring problem in many cities, particularly university centric. What is more interesting is the statistics surround this issue. For e.g. as reported by a survey conducted on 2000 riders in Montreal, only 36% of the riders reported the theft and from that only 2.4 percent of the stolen bicycles were recovered. The problem extends well beyond the university scape. FBI statistics from 2014 indicates that 3.6% (184575) of larceny theft is from bicycle thefts that were reported. There could be lots more unreported bicycle thefts. 

Many of the stolen bicycles are sold as parts or as a whole on sites such as e-bay. To enable buyers and victims track the origins of these bikes (parts), ‘Bikeindex’ (a bike registry) is encouraging bicycle owners to register their bicycles as well as report stolen bicycles. They have approximately 60K registered bicycles and have helped in recovering approximately 2650 stolen bicycles

------

### Project Focus:

This project tried to answer the following two questions:

1. What factors influences a bicycle theft? 
2. Can we identify proportion of bikes stolen from home vs public places?

------

### ipython Notebooks & Data:

Please refer to the Index.ipynb file to refer to the individual ipython notebooks. 

- 1 ipython notebooks for Data retrieval 
- 1 ipython notebook for Classification and Modeling
- 1 ipython notebook for Text Analysis
- All files used and created in the python notebooks are stored in the ‘Data’ folder

------

### **Non-standard python libraries used:**

- gensim - topic modelling libraries
- nltk - text processing libraries
- sklearn - libraries and tools for machine learning
- numpy - package for scientific computing
- seaborn - python visualization library built on matplotlib
- matplotlib - 2D plotting library
- pandas - data structures and data analysis tools
- pprint - pretty print for python
- pattern - web mining module
- scipy - scientific tools for python
- pygeocoder - to get attributes like city, state based on lat and long
- googleplaces - python wrapper for google places api, used to get points of interest around the stolen location (lat,long)

