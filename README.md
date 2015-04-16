LightConky - A simple and colorful conky script
================================================
Features:
- It says you hello
- Shows you current date and time
- System infos [CPU, RAM, Kernel, Shell, Hostname and Uptime]
- Processes that uses much CPU and RAM resource, PID [Killing-ready]
- Network graphs + IP + Download speed + Upload speed
- Colorful as previously said

This is an improvement of this:  
http://crunchbang.org/forums/viewtopic.php?pid=45168#p45168

# *Instrucions* #
$USER is a bash variable that contains your account's name

- Move lightconkyrc in /home/$USER/.conkyrc directory [mv lightconkyrc ~/.conkyrc ]
- Launch conky from /home/$USER [conky] or [conky .conkyrc]

# *Getting the script* #

CLI means "Command Line Interface"
- It is simple using Git CLI: "git clone https://github.com/StefanoBelli/LightConky"
- Getting latest version - from LightConky directory: "git pull"
- Ubuntu font is needed: Arch Linux User can get it by package communtiy/ttf-ubuntu-font-family
What else? Ah...
If your wireless / ethernet card is not 'wlp7s0' you can change it opening the script with a video text editor, searching 'wlp7s0' string, replacing it with what card are you currently using (eth0, enp9s0, wlan0 etc...)

# *Developer* #
I remind you that I am NOT original developer, this was an old script 
(http://crunchbang.org/forums/viewtopic.php?pid=45168#p45168), I improved this. This is my first Conky script :)

Contact me:
- Google+ : plus.google.com/+StefanoBelli
- EMail: stefano9913@gmail.com

Don't forget to visit my(I am not the owner): http://www.inthebit.it/ 

# *Changelog* #

**Version 0.1**

- Intial release
- Deleted GMail function as it is not working and not needed for now
- Deleted mocp player as it is not working and not needed for now
- Deleted Calendar
- Added colors
- Added Kernel, Shell
- Added User name displaying
- Added Date and time displaying
- Edited something on Processes
- Changed font to Ubuntu (size:9)
 
