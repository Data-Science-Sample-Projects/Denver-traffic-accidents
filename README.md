# Denver-traffic-accidents
Description: This is the project folder that accompanies the dataset and notebook I put on kaggle.
Contents: 
 - `notebooks` folder with `EDA` and `Munging the data` notebooks
 - `images` folder with images for both kaggle and github
 -  `src` folder with the contents of the munging notebook modified for production

Note: The data file is too large to put on Github but it resides [here](https://www.kaggle.com/datasets/hrokrin/denver-traffic-accidents)

Status: The dataset and notebook haven't gained much traction on kaggle so I don't think I'm going to put a lot more work into this.

# Discussion
[According to the CDC](https://www.cdc.gov/transportationsafety/pdf/statecosts/2020/CDC-Cost-of-Crash-Deaths-Fact-Sheets_Colorado.pdf), traffic accidents cost Colorado 943M$ in 2018 alone and that number doesn't seem to include the property loss. In 2022 an article in [Denverite](https://denverite.com/2022/01/14/so-how-many-traffic-accidents-occured-on-denvers-neighborhood-streets-in-2021-this-many/) noted there were just over 3100 wrecks on streets with a speedlimit of 25 mph. Of those 3100+ accidents, 84 resulted in a fatality. As a result the city approved the "20 is plenty" ordinance, cutting the speed limit to 20mph. Both of these articles are good and might those interested a start on additional visualizations.
<br><br>

# Takeaways from the Sample EDA notebook 
Kaggle wants an EDA notebook included with submissions for the dataset to get perfect rating. I find this annoying as what gets passed off as EDA is just the output of script (df.head, df.shape, df.describe, etc). I try to put a bit more thought into it but I don't live in Denver (and my area doesn't either collect or make this sort of data available).

So I go with questions I want the answers that are admittedly surface level due to the additional data needed and time available. I'd rather put a little more time into playing with a library 


1. While there are some common accident sites (shown here with a heatmap) essentially the entire city is fair game.

![all Denver accidents over the last 10 years](images/GreaterDenver.png "All Denver accidents over the last 10 years")

<br>

2. Covid had a major positive impact on accidents.

![all Denver accidents over the last 10 years](images/AccidentsByMonth.png "All Denver accidents Accidents by month")

<br>

3. Ruling out non-causes such at "No Apparent", "Other" and "Pending Investigation and/or Court Hearing" we can see aggressive and distracted driving are major issues. Notably, distracted cellphone is smaller that what one might expect.

![Accidents by Factor](images/AccidentsByFactor.png "Accidents by Factor")

<br>

4. DUI/DWAI/DUID related accidents match our intuition of happening more at in the evening hours

![all Denver accidents over the last 10 years](images/CauseTime.png "Accident by Cause of the Hours of the Day")

<br>

 5. There is a slight degree of seasonality. This is also seen the monthly chart above, however this aggregates the 10 years.

![Slight seasonality present](images/Seasonality.png "Slight seasonality present")

<br>

 5. There is a slight degree of seasonality. This is also seen the monthly chart above, however this aggregates the 10 years.

![Slight seasonality present](images/Seasonality.png "Slight seasonality present")
