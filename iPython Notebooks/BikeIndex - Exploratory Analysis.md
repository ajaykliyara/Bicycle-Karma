
# Predicting Bicycle Theft : Exploratory Analysis

Bicycle Theft a rising trend, per nationalbikeregistry over 1.5 million bikes are stolen every year. Bicycle theft is not treated as a priority theft by the police. Also only very few number of stolen bikes are recovered. If we considered only bikeindex data (one of the many bike registry) only about 2700 of 30K bikes were recovered, this is a mere 9%.

Bike Theft is serious problem and needs attention and precautionary measures. Our analysis should touch on some of these aspects.

Data sources are as follows,
1. BikeIndex.Org - This data source has information around stolen and non-stolen bikes and will serve as the primary source of data for our data analysis.
2. League of American Bicyclists - This site provides a dataset which has 2011 bicycle commuter rates by state, including percentage and number of bicyclists by gender. 



# Table of Contents

* [Predicting Bicycle Theft : Exploratory Analysis](# Predicting Bicycle Theft : Exploratory Analysis)
* [Bike Theft Trend](### Bike Theft Trend)
* [Georgraphical Exploratory Analysis](## Georgraphical Exploratory Analysis)
    * [Distribution of Stolen Bikes by State](### Distribution of Stolen Bikes by State)
    * [Distribution of Bike Commuters Vs Stolen Bikes by State](### Distribution of Bike Commuters Vs Stolen Bikes by State)
* [Importance of Using a Bike Registry Service](## Importance of Using a Bike Registry Service)
* [The Brand Effect](## The Brand Effect)
    * [Number of Registered Vs Stolen Bike By Manufacturer](### Number of Registered Vs Stolen Bike By Manufacturer)
    * [Number of Years before Theft by Manufacturer](### Number of Years before Theft by Manufacturer)
* [Effect of Bike Locking Mechansim](## Effect of Bike Locking Mechansim)
    * [Locking Mechanism effect](### Locking Mechanism effect)
    * [Locking Mechanism Vs Manufacturer](### Locking Mechanism Vs Manufacturer)
* [Effect of Season, Time of Day on Theft](## Effect of Season, Time of Day on Theft)
* [Reporting Stolen Bikes to Police](## Reporting Stolen Bikes to Police)
* [Tableau Workbooks](### Tableau Workbooks)

### Bike Theft Trend

The chart shows increasing trend in bike theft. There is a steep increase since the year 2004 but that can be attributed to the fact that bike registry was established only in 2004 and as years passed by gained popularity. But that being said the increase trend has been on the rise and is quite steep and is a cause of concern.

<img src="images/0. Bike Theft Trend.jpg" width=885 height=478/>


## Georgraphical Exploratory Analysis

### Distribution of Stolen Bikes by State.
The viz shows the total number of bike stolen that were reported on bike index , what % belonged to each state in the U.S. The color intensity corresponds to percentage, darker the color more the %. One can observe that number of bikes stolen is very high along west coast as ompared to the rest of the country. The 0% you see on the viz implies % less than 1.

But is there a location Bias in the data, which is causing this. The next viz will help answer this question.

<img src="images/1. State Dist.jpg" width=1699 height=873/>

### Distribution of Bike Commuters Vs Stolen Bikes by State
The viz along with the preivously reported % of stolen bikes by state also plots % of bike commuters in the state. The green color intensity corresponds to percentage of bike commuters per state, darker the color more the %. The size of Bike Marker represents % of total bike stolen by state. One can observe on the left of the grey divider line, that number of bike commuters is high that explains the high stolen bikes along west coast as compared to the rest of the country. 

<img src="images/2. Bike Users Vs Stolen Bike.jpg" width=1699 height=873/>

## Importance of Using a Bike Registry Service

There many Bike Registry Services out there, these sites help you store important information about your bike like Serial Number, color , physical features etc. 

But using a registry service does it have an effect on theft or represent a class of Bikers?

Its evident from the viz below that proactively registering you bike does not get it stolen. How we would interpret this is bikers registering their bike represents people are cautious as they took the effort to register their bike on a registry.

But the bulk of the users register after the fact, that is after the bike was stolen.

<img src="images/3. Proactive Reg Dash.jpg" width=1699 height=873/>


As suspected, a simple check of locking mechanism used by Proactive Registers confirms this assumtion that such users are cautious. Primary locking mechanism used by Proactive Registers is 'U-Lock' as compared to the other class which used inferior locking mechanism 'Cable Lock'


<img src="images/4. Reinforce - Proactive Registers.jpg" width=1699 height=873/>



## The Brand Effect

Does the brand(manufacturer) of the bike have an effect on the number of bikes getting stolen? We will run through few viz to determine if there is an relation.

### Number of Registered Vs Stolen Bike By Manufacturer

This viz plots # of Bikes that were registered vs how many of them were stolen by Brand (Manufacturer). A 45 degree line is drawn, this was done to easily identify mostly stolen manufacturer.

Although 'Trek' has most number of registered bikes as well the most stolen brand, but another brand 'Gary Fisher' lies very close to the 45 degree line this implying this brand has a higher chance of getting stolen.

<img src="images/5. Registered Vs Stolen - Manuf.jpg" width=1699 height=873/>

### Number of Years before Theft by Manufacturer

This viz shows the distribution of number of years between stolen year and manufacturer year of stolen bikes by brand.
Majority of the data points (50% box) lie close the 0 axis this means that bulk of the bikes stolen are relatively newer bikes, bikes tend to get stolen after few years of usage possibly because users are careful with newer bikes then may get complacent as years pass by. Once the bikes get quite old they tend to get NOT stolen as much possible because their value may have depreciated and does not warrant the risk of stealing it.

<img src="images/6. Stolen Year Dist by Manu.jpg" width=1699 height=873/>

## Effect of Bike Locking Mechansim

### Locking Mechanism effect

As one would expect locking mechanism plays a keys role in theft. It is only intutive that if one does not secure one's bike well it would result in it getting stolen by making it easier for the thief.

The below viz reinforces this intution. As one can see 'Cable Locks' leads the pack among stolen bikes as these locks are easier to cut through. Cable lock and leaving the bike unlocked constitues over 50% of all theft instances.

The second viz visualizes the locking mechanism vs how the lock was compromised. Again as expected the 'Cable Locks' are mostly cut through.

Two U-Locks seems to be the way to go.

One interesting observation is with the 'U-Lock', if a good lock is not secured to the right support, it completely defeats the purpose.

<img src="images/7. lock dash.jpg" width=1699 height=873/>

### Locking Mechanism Vs Manufacturer

Do expensive bikes use better(epensive) locking mechanism? One would expect bikers to secure expensive bikes with better locks. But that does seem to be the case. Across most bikes most common type of lock during theft is either leaving the bike unlocked or using 'Cable Lock' which cheapest and most insecure among all of the locks.

<img src="images/8. Lock Vs Manufacturer.jpg" width=1699 height=873/>

## Effect of Season, Time of Day on Theft

Season plays a key role in bike theft. From the below viz Summer seems to be prime season for bike theft. This is expected as bike usage is also more during the warmer season. Also with regards time of the day bikes get stolen , this seems to happen later in the day, majority of which is bettween 6-9 PM. This is probably due the fact that in evening bikes are possibly used in the evenings for more casual after work activities like going to restaurant , library etc.

<img src="images/9. Time of Theft Analysis.jpg" width=1699 height=873/>

## Reporting Stolen Bikes to Police

This viz substantiates the fact that bike theft is not always reported to the police. This is possibly one of the very important reasons for this crime to be increasing at an alarming rate.

<img src="images/10. Stolen Bikes Reported.jpg" width=1699 height=873/>

## Point of Interest Near Bike Theft Location

This viz is key in understanding the effect of nearby points of interest to theft location. Google Places API was used through a Python wrapper to find the nearby points of interest with regards to the stolen latitude and longitude. Store, Restaurant , school, lodging , Bar are the primary places near the theft locations as one would expect. These are places where you could potentially spend over an hour allowing the theif enough time to cut through locks. 

<img src="images/11. place word cloud.jpg" width=1699 height=873/>

The next viz splits up lock mechanism Vs Nearby Places. Key observations are the usage of cable locks near lodging type places and leaving bikes unlocked when at schools, restaurants are not good idea.

<img src="images/12. place by locking desc.jpg" width=1699 height=873/>

Finally a plot of stolen location(in red) and the nearby places on the map.


<img src="images/13. place by locking desc.jpg" width=1699 height=873/>


### Tableau Workbooks
All viz done above can be found in the below two tableau workbooks.

1) Stolen Bikes Analysis - https://public.tableau.com/shared/W2KJXWQMW?:display_count=yes

2) Bike Theft Nearby Places Analysis - https://public.tableau.com/shared/8C9KJBXSQ?:display_count=yes
