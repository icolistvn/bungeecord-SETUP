UbuntuServer-24.04-x64
https://ap-southeast-2.console.aws.amazon.com/ec2/home?region=ap-southeast-2#Home:
https://github.com/icolistvn/bungeecord-SETUP
## SERVER PROXY ##
sudo apt update
sudo apt upgrade
sudo apt install openjdk-17-jdk -y
sudo apt-get install cron
sudo ufw allow 25565
sudo ufw allow 19132
sudo ufw allow 100
sudo ufw allow 101
------ SERVER YELLOW ------
mkdir -p yellow
cd yellow
sudo wget https://github.com/icolistvn/bungeecord-SETUP/raw/main/BungeeCord.jar
mkdir -p plugins
cd plugins
sudo wget https://github.com/icolistvn/bungeecord-SETUP/raw/main/Geyser-BungeeCord.jar
sudo wget https://github.com/icolistvn/bungeecord-SETUP/raw/main/BungeeGuard.jar
sudo wget https://github.com/icolistvn/bungeecord-SETUP/raw/main/ViaVersion-5.0.3.jar
sudo wget https://github.com/icolistvn/bungeecord-SETUP/raw/main/floodgate-bungee.jar
cd ..
sudo java -jar BungeeCord.jar
doi chay 0.0.0.0:25577 >>> ctr+c

sudo rm config.yml
sudo wget https://github.com/icolistvn/bungeecord-SETUP/raw/main/YELLOW/config.yml
Thay doi ip server >>  sudo nano config.yml
ctr+x >> y >> enter
sudo nano plugins/BungeeGuard/token.yml
>> Coppi token SERVER YELLOW   >>> \plugins\BungeeGuard\config.yml

------ SERVER PINK ------
cd ..
mkdir -p pink
cd pink
sudo wget https://github.com/icolistvn/bungeecord-SETUP/raw/main/BungeeCord.jar
mkdir -p plugins
cd plugins
sudo wget https://github.com/icolistvn/bungeecord-SETUP/raw/main/Geyser-BungeeCord.jar
sudo wget https://github.com/icolistvn/bungeecord-SETUP/raw/main/BungeeGuard.jar
sudo wget https://github.com/icolistvn/bungeecord-SETUP/raw/main/ViaVersion-5.0.3.jar
sudo wget https://github.com/icolistvn/bungeecord-SETUP/raw/main/floodgate-bungee.jar
cd ..
sudo java -jar BungeeCord.jar
doi chay 0.0.0.0:25577 >>> ctr+c

sudo rm config.yml
sudo wget https://github.com/icolistvn/bungeecord-SETUP/raw/main/PINK/config.yml
Thay doi ip server >>  sudo nano config.yml
ctr+x >> y >> enter
sudo nano plugins/BungeeGuard/token.yml
>> Coppi token SERVER PINK   >>> \plugins\BungeeGuard\config.yml

#CHINH LAI CAU HINH PORT PE (Tranh trung IP SERVER PORT YELLOW)>>sudo nano plugins/Geyser-BungeeCord/config.yml
>> Thay toan bo 19132 thanh port mong muon ex:100
>> Thay toan bo 25565 thanh port mong muon ex:101

-------- BungeeCord AutoStart ----------------
cd ..
sudo nano pink.sh
>>> chen vo
---------------
cd pink
sudo java -Xms512M -Xmx512M -jar BungeeCord.jar
---------------
ctr+x >> y >> enter

sudo nano yellow.sh
>>> chen vo
---------------
cd yellow
sudo java -Xms512M -Xmx512M -jar BungeeCord.jar
---------------
ctr+x >> y >> enter

chmod +x pink.sh
chmod +x yellow.sh
crontab -e
>> Nhan 1
chen cuoi dong >> 
-----------------------
@reboot sh pink.sh
@reboot sh yellow.sh
----------------------
ctr+x >> y >> enter
sudo reboot

-------------neu crontab not foud-----------------
sudo apt install make 
git clone https://github.com/cronie-crond/cronie.git
cd cronie
autoreconf -i
./configure
make
sudo make install

## SERVER MINERCRAFT ##
>>> spigot.yml >>  bungeecord: true



---- TOI UU VPS UBUNTU -----
sudo apt-get autoremove
sudo apt-get clean
sudo apt-get clean
