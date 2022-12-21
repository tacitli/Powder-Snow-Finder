# Powder Snow Days in Northeastern US
## Intro
This is a recreational project on finding the powder occurrence in following 13 resorts around New York City in the last snow season.

<img src="https://user-images.githubusercontent.com/86301631/208796393-11fc1a12-21a9-46ae-bcf4-171bde948c2c.png" width="300">

## Data
Due to the Openweather API restriction, we can only query history data for the past one year for education or research use. (Still trying to contact another weather API website). 
The formation of powder snow is conditioned on **temperature** and **wind speed**, so the data queried is the hourly temperature and wind speed data for all 13 ski resorts **from 2021-12-19 to 2022-04-02** (the snow season period). Day temperature and wind speed are calculated by averaging the original hourly data. 

<img src="https://user-images.githubusercontent.com/86301631/208803795-f6177ac0-fe94-46d9-935a-7da6120c063e.png" width="380">

## Data Visualization

https://user-images.githubusercontent.com/86301631/208796962-4bee37dd-13ca-46bd-bae5-62e98686ca12.mp4

https://user-images.githubusercontent.com/86301631/208796964-89c7a5c6-d401-4d4b-a1cd-8e9976151e20.mp4

From the bar chart iteration plots, we can see that the temperature and wind speed are quite fluctuant over the snow season, and possibly subject to yearly temporary conditions. Thus, the data from one year may not be precise enough to do a fine granularity powder snow prediction. But in the following chapter, we can still summarize which period and which resorts are ideal for catching powder snow by analyzing the occurrence number.

# Define the weather condition for perfect powder

Since major resorts all have snowmaking setups, the weather elements we need to consider are temperature and wind speed.
## Temp
Ideal temperatures for light and fluffy snow tend to fall between *0°F and 10°F* near or above the **summit of the mountain**.
## Wind
Along with cold temperatures, we are looking for winds slower than about 15 miles per hour near the **summit of the mountain**. Winds stronger than 15 miles per hour will tend to pick up the snow and pack it more closely together as it blows around during and after it falls.

Credit: 
Collentine. (2019, August). *Perfect powder - explained*. OpenSnow. Retrieved December 11, 2022, from https://opensnow.com/news/post/perfect-powder-explained

## Powder day list visualization 

One dark blue square means a powder day in a given resort calculated by the desired temperature and wind speed condition.

In split view:

![Splited Powder Snow Dates by Resorts in Season 21-22 cropped](https://user-images.githubusercontent.com/86301631/208815779-2173d91f-5e42-47fa-bf5a-e980d4d73369.png)

Continuous timeline:

![Powder Snow Dates by Resorts in Season 21-22](https://user-images.githubusercontent.com/86301631/208797267-2cf23552-4c6d-43a0-b6cb-b671fdce7774.png)


## The resorts that observed the most powder days over the last snow season

![Powder Days Count by Resorts](https://user-images.githubusercontent.com/86301631/208798738-2b521f6e-2067-4428-ade2-41e56905a2b1.png)


From this plot, we can see that the resorts located in Vermont are our go-to place for powder snow since they take over the top of our list over the last snow season. And the occurrence of powder days calculated by our data in VT resorts are significantly higher than in other states. 

Among the resorts in Vermont, **Stowe, Mt Snow, and Stratton** are the **best places** for a powder snow trip.

![Powder Days Count by Dates](https://user-images.githubusercontent.com/86301631/208798587-37a30ac0-8b54-4f86-97b0-445ca68b57d9.png)


According to the plot, from mid-January to early February is an ideal period for a ski trip if you want crush some powder. 
