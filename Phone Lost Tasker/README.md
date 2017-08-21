# Phone Lost Tasker Project

## Description

This Project was made to have the highest chances of getting your phone back after you lost it or it was stolen with the power of Tasker.


## How-to-use

How to use this project?
1. Get Tasker (https://play.google.com/store/apps/details?id=net.dinglisch.android.taskerm)
2. Copy all files in TaskerProfiles/Phone Lost Tasker/ (https://github.com/FaserF/TaskerProfiles/archive/master.zip) to your phone on /Tasker/profiles
3. Now open Tasker and long press on Profiles -> Import
4. Go to Tasks -> "Lost" and edit everything thats needed (f.e. Add a phone number, enter your adress and more!)

Now once you have lost your phone just write an SMS from any phone to your phone number with "Lost Phone" if you have really lost it or if it's stolen. The default 2nd Lockscreen Code Tasker will create is 0011.
If you have only left it somewhere in your house and you can't find it, it is better to text your phone with "Find Phone"

For Users who want more security:
5. now create a wallpaper which will contain as much informations as you can (Name, picture, email, adress and so on) and copy it to your phone to /Pictures/Wallpaper/Tasker (or change the location in the Lost Task!)
6. Some things will only work when Tasker Secure Settings Plugin is installed. So go and get it from the Play Store!
7. Download a Sound you want to hear when you send "Find Phone" to your phone. Then copy it to your phone and change the location to your song in the Find Task

## What does it do?

Phone Lost:
- Send an SMS to the last sender (you) with the following informations: Location of the phone, battery status, WIFI Network connected to/nearby, Nearest Cell Network
- Push the same informations via Pushbullet to all of your devices
- Change Wallpaper to one whith informations about you
- Create second lockscreen with another PIN Code and with informations about you
- Take a photo with the front camera
- increase volume of media, alarm, ringer
- auto call a number you have deposited in the app and lower the in call volume
- create a persistant notification with lost phone informations

On Device Boot:
- Check if the device status is "lost"
- If yes auto start the Phone Lost task (to protect killing the Lost Phone tasker project with a reboot)

Phone Find:
- Higher the ringer and media volume
- Play a very high and loud "Beep"
- Say "I am here"
- Wait a minute if it has been found, if not play your music track on the absolute maximum volume and send a sms with the current location


## Issues / Q&A

If you have any issues be sure to create a new issue on github (https://github.com/FaserF/TaskerProfiles/issues)

## More

Languages of the project: English
