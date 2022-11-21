# RunWindowsAppsOnUbuntu
how to run Windows Apps on Ubuntu?😍✌️🤪

💻first you can see this Link : 

https://ubuntuhandbook.org/index.php/2022/01/wine-stable-7-0-released/

🥲if that link did not exist,come with us : 

**a - Enable 32 bit architecture :** 
  - sudo dpkg --add-architecture i386
 
**b- Install The Key :**
  - wget -O - https://dl.winehq.org/wine-builds/winehq.key | sudo apt-key add -

**c- Add Wine Repo :** 
  - sudo add-apt-repository 'deb https://dl.winehq.org/wine-builds/ubuntu/ focal main'

**d- Install Wine ->** 
  - sudo apt update
  - sudo apt install --install-recommends winehq-stable

**🚫 Also for Uninstall Wine :**

sudo apt remove --auto-remove winehq-stable

**🔔Also You Can Install Lutris Or Bottle Apps instead of Wine for running Windows Apps .** 

**⁉️Now Question is how to Install SqlServer2019 on ubuntu for using that in WPf Or Winform Development 😊**
