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
 [ *A shellscript is coming in next release to automatically install it, check if conky is installed and another to launch the script with some arguments [set.sh, lcinit.sh] (retarded starting time, network card)* ]

# *Getting the script* #

*Don't use with kde...*

CLI means "Command Line Interface"
- It is simple using Git CLI: "git clone https://github.com/StefanoBelli/LightConky"
- Getting latest version - from LightConky directory: "git pull"
- Ubuntu font is needed: Arch Linux User can get it by package communtiy/ttf-ubuntu-font-family
- hddtemp is needed to show Disk temperature (Celsius)
What else? Ah...
You need to launch hddtemp daemon to see Disk temperature, else Conky says that hddtemp is not reachable, this because server is not launched and running.
To launch hddtemp daemon:

- $ su -c "hddtemp -d /dev/device"  - or -
- $ sudo hddtemp -d /dev/device - or -
- # hddtemp -d /dev/device

Where $ is any user except root, and # is root, you don't need to include # or $ ; device is a device such as sda, sdb, sdc, sdd, and more... this should be your hard drive (dev device)

# *Developer* #
I remind you that I am NOT original developer, this was an old script 
(http://crunchbang.org/forums/viewtopic.php?pid=45168#p45168), I improved this. This is my first Conky script :)

Contact me: [Stefano Belli]
- Google+ : plus.google.com/+StefanoBelli
- EMail: stefano9913@gmail.com
- GitHub: https://github.com/StefanoBelli

Don't forget to visit my(I am not the owner)blog: http://www.inthebit.it/ 

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

**Version 0.2**

- Removed Name, Time, Date
- Removed CPUs bars
- Added Operating System
- Added Architecture
- Added Desktop Environment
- Added RAM, SWAP, Filesystem Usage Percentage
- Added RAM, SWAP, Filesystem Bars
- Added CPU Graph
- Moved Section names to center (align to center)
- Added ESSID, AP MAC Address, Bitrate, Signal Quality percentage & bar, Wireless card mode and External IP (requires Curl) 
- Now refreshes every 0.25 ms (milliseconds)
- Some changes to window specs 
- Changed Network section color to 'green'
- Added some if-else statement for Operating System / Network Cards (eth0, enp9s0, wlan0, wlp7s0), so you don't need to change anything if your network card is identified as 'wlp7s0'
- See commits to show more...

**Version 0.3**
- If-else statement removed from 'NETWORK' section as it is not working well, so you need to type your network card... a shell script is coming
- Added lconky-scripts folder
- Moved all except this file (README.md) to lconky-scripts/ 
- Added another script: lightconkyrc2 

  *lightconkyrc2*
   - Added User, Day, Time informations
   - Added various battery informations 
   - Added Rhythmbox Support
 
  *lightconkyrc1*
   - As previously said removed if-else statement
   - Fixed some syntax errors
 
