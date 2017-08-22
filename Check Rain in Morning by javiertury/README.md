# Check Rain Tasks
Customizable rain notifications for tasker. Get rain notifications in the morning if it is going to rain during the day. 
This project is based on the work from javiertury tasker-check-rain https://github.com/javiertury/tasker-check-rain
Even this description is based on his work :) so be sure to check his githun out. He has a lot more options, i have only improved the morning option to my own needs.

Requirements
  * These tasks are for the android app [Tasker](http://tasker.dinglisch.net/)
  * You need an API key from [openweathermap.org](http://openweathermap.org/appid)


# Installation
The folder `Check Rain in Morning by javiertury` in this repo contains 2 files. Copy those 2 files to your android device, preferably to `/sdcard/Tasker`.
  1. Open tasker and then touch and hold on `PROFILES` tab until a menu pops up.
  2. Select `import`.
  3. Browse the directory in which you put your `Profiles` directory and open it.
  4. Import each profile one by one

Finally open tasker, go to `VARS` tab and create a variable named `%W_ow_key` with you openweathermap.org API key. 

# Configuration

## Location source

These tasks automatically use your last know location using either gps or network location. If you want to specify a fixed location, you have to specify a city and enable fixed city location for the notification type you want.

The specified city is common to all notification types. It's stored in the global variable `%W_loc_city` and follows the format `<city name>,<country ISO 3166 code>`, for example, `Boston,us`. For each type of notification you can set the location source to `city` to use the city specified in `%W_loc_city` or to `auto`(default).
  * For Morning notifications it is `%W_mor_lsrc`
  
## Notification titles and text

You can customize the notification title using global variables. The title of the notifications must be stored in global variables so that these notifications can be automatically removed and the profiles `Check Rain <NOTIFICATION TYPE> Touch` can open an app when those notifications are touched.
  * For Morning notifications it is `%W_mor_title`
  
The text of those notifications can be set modifying the the action `Notifiy Sound` inside each notification type task.

## Change launched app on notification touch

By default when a notification is touched Forecastie is launched. If you want to change the app go to `TASKS`, open the task `Clear Notify And Open Weather` and edit `Launch App`. If you already had Forecastie installed but it was not being launch by touching the notification, you can fix it by setting it again using the previous steps.

