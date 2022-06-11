# termux-send-location

Simple script to send gps (or network retrieved) position to someone through SMS.

## Dependencies
Android apps needed:
- [Termux](https://f-droid.org/packages/com.termux/)
- [Termux:API](https://f-droid.org/packages/com.termux.api/)

In Termux system some packages are required:
- termux-api (for sms sending features)
- termux-location (for retrieving gps or network location)
- jq (for parsing json formatted data from gps)

Those can be installed with: `pkg update && pkg install termux-api termux-location jq`

## Permission
To work properly some permissions need to be activated:
- SMS access
- Position Access 
Those must be granted to "Termux:API" app

## Optional
If you plan to use frequently this features I highly recommend to use it in combination with [Termux:Widget](https://f-droid.org/packages/com.termux.widget/). This app will allow to one-tap-launch of the script, this will make the script usefull in real situations.

Next to installing Termux:Widget app you only need to `mv` the script inside .shortcut folder in the Termux home folder.
The result should be like that:

![immagine](https://user-images.githubusercontent.com/79154297/173182031-ab1b91e9-cd16-4c0a-8af6-57a0ef0bb714.png)
