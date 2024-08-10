https://ap-southeast-2.console.aws.amazon.com/ec2/home?region=ap-southeast-2#Home:
https://github.com/icolistvn/bungeecord-SETUP
## SERVER PROXY ##
sudo apt update
sudo apt upgrade
sudo apt install openjdk-17-jdk -y
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
sudo wget https://github.com/icolistvn/bungeecord-SETUP/raw/main/config.yml

#CHINH LAI CAU HINH >>  sudo nano config.yml
#CHINH LAI CAU HINH PORT 19132 PE >>sudo nano plugins/Geyser-BungeeCord/config.yml
>> Thay toan bo 19132 thanh port mong muon

-------- BungeeCord AutoStart ----------------
sudo corntab -e 
>> Nhan 1
cuoi dong >> @reboot sudo java -jar BungeeCord.jar
ctr+x >> y >> enter
sudo reboot
-------------------------------
>>>>> loi not foud corntad
git clone https://github.com/cronie-crond/cronie.git
cd cronie
autoreconf -i
./configure
make
sudo make install
---------------------------------------------

## SERVER MINERCRAFT ##
>>> spigot.yml >>  bungeecord: true

>>Vao SERVER PROXY 
sudo nano plugins/BungeeGuard/token.yml
Copi token pass vao server minercraft >>> \plugins\BungeeGuard\config.yml

J3mnN1dHgeqyrGAcRBH7BrzDwGXnZJMdK37LPjoXx3TUs2orYo685vLVotXYlmaT

