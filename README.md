# FinalProject

# For this final project I have done an analysis of the bee population in the USA that I found on Kaggle. 

Originally I got a data set from 1998 - 2012 but was able to tetrieve a version that included the years 1990 until 2017.
The data set includes information on the number of colonies per state, yield per colony, total yield per state and the price at which it is sold per lb. 
This data is organised per state per year. 

For the ananlysis I have certain goal I would like to achieve. 

- I want to analyse the increase or decrease in bee populations/total production/efficiency of the bees and determine what can be concluded from this. 
- Second I want to do an prediction on the future of honey production and prices in the USA through linear regression. 

- As a second step in the analysis proces I will be comparing the data set to a data set on pesticides and pollution to determine what the main factors are that are influcencing the change in this essential industry. 

- Finally I would like to give a recommendation to future beekeepers to afvice them where they should locate themselves based on their aspirations.

![que-pasaria-si-se-extinguieran-las-abejas](https://user-images.githubusercontent.com/104360125/187383202-18b3ad29-ed8a-4d08-8e5f-0d40d6467e7a.jpeg)


For the analysis I will be looking both on regional and state level. Below there is an image with the map of how the states are devided into regions North, South, West and Midwest.

![USA split by region](https://user-images.githubusercontent.com/104360125/187384190-faf7bb68-a82d-4602-ba2b-380a9261449f.png)

To start off, here is an image with development of honey production from 1990 until 2017

![Bees prodction vs price per lb (2)](https://user-images.githubusercontent.com/104360125/187385881-b90395ea-a196-4579-8ede-f9967e744e53.png)

We can see that the average number of colonies is quite steady over the year but that in the graph that displays the average yield per colony the yield is slowly decreasing. As a result of this decrease in production the price per lb is rising which occurs when products become more scarse. What suprised me of this graph is how little decrease there is in bee polulations as this is something that is in the news quite frequently. 

** (add % decrease per region)


In this image we can see a similar graph but this one displays the decrease in avarage production and the increased price per lb while the increased production value is displayed below. 

![Bees prodction vs price per lb](https://user-images.githubusercontent.com/104360125/187389607-9bbccb2d-5308-4128-bd11-0142b4bcb91a.png)



In the following image we can see the efficiency, price of honey per lb and the total production value of the state. If you were a honey producer during these years and care most about total production value you should have located yourself in North Dakota if you cared most about efficiency to reduce workload you should have located yourself in Louisiana and if you care most about the price of your product because you want to be an high quality producer you should locate yourself in Virginia. 

Later on we will take a look where it is best to locate yourself in 10 years time and see if this is still the best place to locate your self as a beekeeper. 

![All states compared (1)](https://user-images.githubusercontent.com/104360125/187442881-1d4fc5a0-8188-42c7-b13c-b2e82ee6e578.png)





Following this analysis I did a comparision between this data set and the two data sets that I had mentioned before.

First we will be looking at the use of pesticides in the USA


![States stop using pesticide due to new laws (1)](https://user-images.githubusercontent.com/104360125/187408234-5a6db1ac-9827-466d-ad8c-9e673b8dc443.png) Use of NEONIC pesticides in the USA. 


When plotting the use of NEONIC pesticides in tableau we can see that the use of these pesticides really took off between 2002 - 2004. The only state that was using it before these years was California. Looking at 2015 we can see that almost all states but again besides California stopped the use of these pesticides. I did some quick reseach and found out that this was due to a new bill that would ban the use of these pestices, the use of them increased again after this date since the bill never passed. 



To see the influence of these pesticides on the honey prduction I created a correlation heatmap just like this one. 

![Screenshot 2022-08-30 at 12 08 45](https://user-images.githubusercontent.com/104360125/187410503-e885074c-3ca0-4b59-afbc-e56f07a632e4.png)

The top 5 most influencial values on this heatmap are the relation between:
- nIMIDACLOPRID and the number of colonies. The correlational valus is 0.41
- nIMIDACLOPRID and production value with a collolational value of 0.36
- nACETAMIPRID and the number of colonies. The correlational value is 0.32
- nIMIDACLOPRID and and the total prodcution with a corrolational value of 0.27
- nCLOTHIANIDIN	and the price per lb with a collolational value of 0.26

Over all we can see that ll NEONIC pesticides combined effect the size of colonies with 0.19, the price per lb with 0.28 and the productionvalue with 0.24.

Suprising is however is that the use of these pesticides seems to be positively influencing the total production, the total stock and the number of colonies. This can however be explained by human efforts of re polulaton bee colonies and "cultivating" more bees to counter the effects and therfore changing the data.
The negative effects of pesticides can however be seen in the average yield per colony which mainly shows negative correlation (very small though) 

NEONIC pesticedes although not the main culprit in effecting bee populations and honey production are defenitly an influencial factor but are countered by human influence. 

This is also visible on the following graphs: 
![All states stop using pesticide due to new laws (1)](https://user-images.githubusercontent.com/104360125/187459606-3a5a9c75-ad1a-4a62-9775-b05f7414f503.png)

The yellow line displays the average yield per colony which as been going through a downward trend during the entire period and doesnt seem to be affected by use or stopping to use pesticides, the same counts for the average number of colonies which is compared to pesticide use in the graph underneath. 

The second dataset against which the bees datset was compared is the dataset on pollution in the USA. The pollution dataset has a range of 13 years, going from 2000 until 2012. When mergin the dataset the bees dataset was reduced to the same number of years to avoid null values. 


Just as for the pesticide dataset I did correlation heatmap to determine what pollution factors play a role in the bee population and honey production. 

![Screenshot 2022-08-30 at 12 50 10](https://user-images.githubusercontent.com/104360125/187418250-065cf918-d155-4374-86f7-ec1125078770.png)


The influnecial values in this matrix are mainly nagative corelational values as is expected. We can see that the CO mean, SO2 mean and NO2 mean are developping over the years. 
When plotting this in Tablea we can see the following increase.

The columns most effected by pollution are the price per lb, production value and the stock that is held by the USA with the price per lb being the most heavy hit by pollution with 3 negative values over -0.25

The main pollution culprits are NO2 mean (nitrogen dioxide) S02 (sulfur) and CO (carbon monoxide)


Now it is time to do some linear regression to see where bee colonies could be in 5 years time based on the data we have. 

For 2027 I am able to give the following recommendations..




Over all conclusions. 

Due to big efforts by beekeepers the datasets that I have used are a bit confusing and contradicting the news that we get about the status of bees. 

- We can conclude that humans are doing great work in countering the negative factors that are influenceing bee populations and the efficiency of these bees.

- To get a better insight into bee populations and make better predictions we need more data on repopulation through human intervention, more information on colony loss and more specific data on local and migratory bees. Bees by themselves migrate throughout the states and also get moved around the country to facilitate pollination on agricultural crops. 



