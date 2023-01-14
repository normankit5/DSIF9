**Problem Statement**

Mean sea level in Singapore rises by 3mm to 4mm per year. It is projected that by the Year 2100, the mean sea level in Singapore would rise by 1000mm compared to a baseline levels between 1995 to 2014. While the rise of mean sea levels could be mitigated with measures such as coastal protection (external defence), it is suspected that rise of mean sea levels may also put strain on the internal defences such as water catchment facilities, storm runoff drains, etc in the form of increased precipitation/erratic weather patterns that results in potential floods. Floods in Singapore between 2000-2015 resulted in flood damage costing 32M$.

The project aims to examine the relationship between Singapore’s mean sea level and its weather conditions to mitigate floods effectively

**Data Dictionary**

|Feature|Type|Dataset|Description|Source|
|---|---|---|---|---|
|date|datetime64[ns]|combined_df|Date of the data|Various Source|
|year|int64|combined_df|Extracted year of the data|Various Source|
|monthly_wet_bulb_temperature|float64|wet-bulb-temperature-hourly|Originally hourly wet bulb temperature (temperature at 100% humidity), it was converted to monthly mean|Data from Project 1 source|
|temp_mean_daily_min|float64|surface-air-temperature-monthly-mean-daily-minimum|Mean of the daily minimum temperature over a given month|Data from Project 1 source|
|maximum_rainfall_in_a_day|float64|rainfall-monthly-maximum-daily-total|The maximum rainfall recorded in a day over a given month|Data from Project 1 source|
|no_of_rainy_days|float64|rainfall-montyly-number-of-rain-days|The number of recorded rainy days over a given month, a rainy day is defined as more than 0.2mm of rainfall|Data from Project 1 source|
|total_rainfall|float64|rainfall-monthly-total|Total rainfall in mm|Data from Project 1 source|
|mean_sunshine_hrs|float64|sunshine-duration-monthly-mean-daily-duration|The mean sunshine hours over a given month|Data from Project 1 source|
|mean_relative_humidity|float64|relative-humidity-monthly-mean|The mean relative humidity over a given month|
|mean_sea_level_RLR|float64|mean-sea-level|The mean sea level in relation to the RLR datum|https://psmsl.org/data/obtaining/stations/1351.php|

**Summary of Analysis**
The analysis shows that the rise of mean sea level has a correlation with the features (humidity, temperature, number of rainy days) which encourages higher amount of rainfall


**Takeaways, Recommendations, and Conclusions**

It seems that a rising mean sea level poses both external (in the form of sea water submerging low lands) and internal problems (in the form of inability of water catchment and storm runoff to discharge the rain in time). While we could construct seawalls to ward of the effects of rising sea levels, we would not be able to control the amount of rain on our island. As seen from the EDAs, it seems that higher number of rainy days with higher amount of rainfall can be expected, this would in turn cause flooding on our island should our water catchment and storm water runoff are unable to handle it.

We would recommend that the current capacity of the water catchments and storm water runoff systems to be review so that we are adequately prepared for this inevitability. We would also suggest on embarking an actual weather simulation with a complementary data science predictive model to complement the forecasting of future mean sea levels, and forecasting of rainfall on the island