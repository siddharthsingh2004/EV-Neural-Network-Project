# EV_charging_neural_network

For this project, I used PyTorch to train a neural network to predict residential electric vehicle charging loads using real-world data from apartment buildings in Norway.
I compared the Mean Squared Error to the MSE achieved by Linear Regression from sklearn to prove that the activation functions and non-linearity helped reduce the error of predictions.
Real-Data Link: https://data.mendeley.com/datasets/jbks2rcwyj/1


Description of Columns: 
* session_ID - the unique id for each EV charging session
* Garage_ID - the unique id for the garage of the apartment
* User_ID - the unique id for each user
* User_private - 1.0 indicates private charge point spaces and 0.0 indicates shared charge point spaces
* Shared_ID - the unique id if shared charge point spaces are used
* Start_plugin - the plug-in date and time in the format (day.month.year hour:minute)
* Start_plugin_hour - the plug-in date and time rounded to the start of the hour
* End_plugout - the plug-out date and time in the format (day.month.year hour:minute)
* End_plugout_hour - the start of the hour of the End_plugout hour
* El_kWh - the charged energy in kWh (charging loads)
* Duration_hours - the duration of the EV connection time per session
* Plugin_category - the plug-in time categorized by early/late night, morning, afternoon, and evening
* Duration_category - the plug-in duration categorized by 3 hour groups
* month_plugin_{month} - the month of the plug-in session
* weekdays_plugin_{day} - the day of the week of the plug-in session
* Date_from - the starting time in the format (day.month.year hour:minute)
* Date_to - the ending time in the format (day.month.year hour:minute)
* Location 1 to 5 - contains the number of vehicles each hour at a specified traffic location.
