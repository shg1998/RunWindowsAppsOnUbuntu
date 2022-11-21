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

**Run .exe Files :**

After installation , for running .exe Apps , Go to their directory , Open Terminal and write this command : 
  - sudo wine ./Your_Program_Name.exe
 
 ![Screenshot (27)](https://user-images.githubusercontent.com/52446257/202989220-c3e2ae3a-a21e-4883-a139-683d1fd53713.png)

**🚫 Also for Uninstall Wine :**

sudo apt remove --auto-remove winehq-stable

**🔔Also You Can Install Lutris Or Bottle Apps instead of Wine for running Windows Apps .** 





**⁉️Now Question is how to Install SqlServer2019 on ubuntu for using that in WPf Or Winform Development 😊**

for Install SqlServer2019 , You Can Use this Link : 

https://computingforgeeks.com/how-to-install-ms-sql-on-ubuntu/

👍 Let's Start : 

**a- update ubuntu system :** 
  - sudo apt update
  - sudo apt -y upgrade
  - sudo reboot (optional :))

**b- Import the public repository GPG keys:**
  - sudo wget -qO- https://packages.microsoft.com/keys/microsoft.asc | sudo apt-key add -

**c- Add Microsoft SQL Server 2019 Ubuntu repository:**
  - sudo add-apt-repository "$(wget -qO- https://packages.microsoft.com/config/ubuntu/20.04/mssql-server-2019.list)"

**d- Install MS SQL Server 2019 on Ubuntu:**
  - sudo apt update
  - sudo apt install mssql-server

**e- Initialize MS SQL Server 2019 on Ubuntu:**
  - sudo /opt/mssql/bin/mssql-conf setup (choose 2 -> Developer)

**f- Install MS SQL tools and unixODBC plugin:**
  - curl https://packages.microsoft.com/keys/microsoft.asc | sudo apt-key add -
  - curl https://packages.microsoft.com/config/ubuntu/20.04/prod.list | sudo tee /etc/apt/sources.list.d/msprod.list
  - sudo apt update 
  - sudo apt install libodbc1
  - sudo apt install unixodbc
  - sudo apt install msodbcsql17
  - sudo ACCEPT_EULA=Y apt install mssql-tools unixodbc-dev

**g- Configure PATH for MS SQL binaries:**
  - echo 'export PATH="$PATH:/opt/mssql-tools/bin"' >> ~/.bash_profile
  - source ~/.bash_profile
  - echo 'export PATH="$PATH:/opt/mssql-tools/bin"' >> ~/.bashrc
  - source ~/.bashrc

**h- Connect to MS SQL console :** 
  - sqlcmd -S 127.0.0.1 -U SA 
  - Enter Your Password

**i- Test Console :** 
  - create database UbuntuDatabase;
  - select name from sys.databases;
  - go

**😍Enjoy from Using Sql Server :)**















