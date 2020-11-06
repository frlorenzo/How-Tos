# Make Ubuntu Look Like macOS


## Prerequisites: GNOME Tweaks and GNOME Extensions

```
sudo apt update
sudo apt upgrade
sudo apt install gnome-tweaks -y
sudo apt install gnome-shell-extensions -y
```
 
Make sure the **"user themes"** extension is installed.



## Step 1: Install a macOS inspired GTK theme

- [McMojave](https://www.pling.com/p/1275087)
- [Cataline](https://www.pling.com/p/1226871)

Extract the downloaded theme and copy this extracted theme folder to `.local/share/themes` folder. Open GNOME Tweak tool and change the Application and Shell theme.



## Step 2: Install macOS like icons

- [McMojave-circle ](www://https.gnome-look.org/p/1305429/)
- [Mojave CT icons](https://www.gnome-look.org/p/1210856/)

Extarct the download folder and copy it to `.icons` folder in your home directory. 



## Step 3: Add macOS like dock

- [Dash to Dock](https://micheleg.github.io/dash-to-dock/) GNOME Shell Extension

Follow instruction in section [manual installation](https://micheleg.github.io/dash-to-dock/download.html). You also need to install `dconf-editor`

```
sudo apt install dconf-editor
```



## Step 4: Use macOS wallpaper

- [Mac OS wallpaper](https://oswallpapers.com/category/mac-os/)

Download [package here](https://drive.google.com/open?id=1iOL89QxMs9zHWT7M2d26OrZcmJj2IIDI). 
Next, extract `.zip` file to `~/.local/share/backgrounds`


#### Change the lock screen Wallpaper
[PENDING]



## Step 5: Change system fonts

- [Roboto](https://fonts.google.com/specimen/Roboto?query=robot&selection.family=Roboto:ital,wght@0,100;0,300;0,400;0,500;0,700;0,900;1,100;1,300;1,400;1,500;1,700;1,900&sidebar.open=true) font by Google.

Download and extract '.zip' file to `~/.fonts` directory 
- Restart `Alt+F2` + `r` 
- Change the system wide font using GNOME Tweaks tool


## Bonus Tip: Spotlight like app launcher 
[PENDING]



## Reference
[How to Make Ubuntu Look Like macOS in 5 Easy Steps](https://itsfoss.com/make-ubuntu-look-like-macos/)
