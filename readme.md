----------------------------------------------------------------------------------------------
Linux Valet setup and mysql , phpmyadmin ,php , mysql , dependency
----------------------------------------------------------------------------------------------

Vs code plugin for phpstorm
Install php
Install composer
Install valet
Add valet path
Github ssh key for linux
Valet command
Php extension install
Phpmyadmin for valet
Install mysql client and server
Create root user and password

Php Setup (Linux)
=====================

vs code plugin 
--------------------------------
IntelliJ IDEA Keybindings – vs code plugin for phpstorm keybinding


=================
Valet setup
=================
Install composer
------------------- 
1.sudo apt update
2.sudo apt install php-cli unzip

sudo apt install curl

php composer.phar global require friendsofphp/php-cs-fixer
sudo apt install composer


-------------------------------------------------
//install valet 
-------------------------------------------------
composer global require cpriego/valet-linux -W




//Add valet path dynamically
---------------------------
echo "export PATH=$PATH:$HOME/.config/composer/vendor/bin" >> ~/.zshrc
source ~/.zshrc



//valet dependency
sudo apt-get install network-manager libnss3-tools jq xsel

3.Install php extension
sudo apt install openssl php-bcmath php-curl php-json php-mbstring php-mysql php-tokenizer php-xml php-zip


//valet command
Valet install
Valet park
Valet run
Valet restart
Valet stop
Valet start



https://cpriego.github.io/valet-linux/



https://cpriego.github.io/valet-linux/
https://www.digitalocean.com/community/tutorials/how-to-install-and-use-composer-on-ubuntu-20-04


====================
Generate ssh key linux
====================
ssh-keygen -t rsa
Go to -> home/ahmed/.ssh/id_rsa
Copy code-> and set in github

Copy the SSH public key to your clipboard. ...
In the upper-right corner of any page on GitHub, click your profile photo, then click Settings.
In the "Access" section of the sidebar, click SSH and GPG keys.
Click New SSH key or Add SSH key.
====================
Phpmyadmin for valet
====================
Download phpmyadmin (https://www.phpmyadmin.net/donate/)
Extract and copy to project directory

Install mysql client and server
---------------------------------------
sudo apt-get install mysql-client
sudo apt-get install mysql-server

Create root user and password
And set previledge
---------------------------------------
sudo mysql -u root -p
//create user and password
CREATE USER 'username'@'localhost' IDENTIFIED BY 'password';
//Give previleges
GRANT ALL PRIVILEGES ON *.* TO 'username'@'localhost';

//flush previleges
FLUSH PRIVILEGES;







	



