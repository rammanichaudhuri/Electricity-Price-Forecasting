# electricity-price-prediction
predicting the price of electricity by using previous data

dataset : https://www.kaggle.com/salilchoubey/electrity-prices
total data rows : 38014

description of the features :

DateTime: String, defines date and time of sample
Holiday: String, gives name of holiday if day is a bank holiday
HolidayFlag: integer, 1 if day is a bank holiday, zero otherwise
DayOfWeek: integer (0-6), 0 monday, day of week
WeekOfYear: integer, running week within year of this date
Day integer: day of the date
Month integer: month of the date
Year: integer year of the date
PeriodOfDay: integer denotes half hour period of day (0-47)
ForecastWindProduction: the forecasted wind production for this period
SystemLoadEA: the national load forecast for this period
SMPEA: the price forecast for this period
ORKTemperature: the actual temperature measured at Cork airport
ORKWindspeed: the actual windspeed measured at Cork airport
CO2Intensity: the actual CO2 intensity in (g/kWh) for the electricity produced
ActualWindProduction: the actual wind energy production for this period
SystemLoadEP2: the actual national system load for this period
SMPEP2: the actual price of this time period, the value to be forecasted.

missing values were filled with median

result :

using ridge regressor ->  mean(actual price/predicted price) = 0.9186573707226419

using random forrest -> mean(actual price/predicted price)=  0.9143769430183479

