UbuntuServer-24.04-x64
https://ap-southeast-2.console.aws.amazon.com/ec2/home?region=ap-southeast-2#Home:
https://github.com/icolistvn/bungeecord-SETUP
## SERVER PROXY ##
sudo apt update
sudo apt upgrade
sudo apt install openjdk-17-jdk -y
sudo apt-get install cron
sudo apt-get install htop
sudo ufw allow 25565
sudo ufw allow 19132
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
sudo nano config.yml
ctr+x >> y >> enter
sudo nano plugins/BungeeGuard/token.yml
>> Coppi token SERVER PINK   >>> \plugins\BungeeGuard\config.yml

# CHINH NAME MOBLIE "." thanh "§e" >>> sudo nano plugins/floodgate/config.yml
ctr+x >> y >> enter

-------- BungeeCord AutoStart ----------------
cd ..
crontab -e  (Khong chon sudo nha >>>DM NO)
>> Nhan 1
chen cuoi dong >> 
-----------------------
@reboot sudo java -Xms512M -Xmx512M -jar BungeeCord.jar
----------------------
ctr+x >> y >> enter
sudo reboot


##XAC DINH VI TRI FILE BungeeCord.jar Khi bi loi khong tu chay 
sudo apt install plocate
locate BungeeCord.jar

## SERVER MINERCRAFT ##
>>> spigot.yml >>  bungeecord: true


---- TOI UU VPS UBUNTU -----
sudo apt-get autoremove
sudo apt-get clean
sudo sysctl vm.swappiness=10
