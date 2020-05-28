#!/bin/bash
#Silahkan di recode :)
#Jangan Lupa Subscribe Ekid Root

#Variables
clear
b="\033[1m"
u="\033[4m"
bl="\033[30m"
r="\033[31m"
g="\033[32m"
bu="\033[34m"
m="\033[35m"
c="\033[36m"
w="\033[37m"
endc="\033[0m"
enda="\033[0m"
blue="\033[1;34m"
cyan="\033[1;36m"
red="\033[1;31m"

figlet EKID | lolcat
figlet ROOT | lolcat
echo "ADMIN : EBECK KANSAS" | lolcat
echo "YOUTUBE : Ekid Root" | lolcat


###################################################
# CTRL + C
###################################################
trap ctrl_c INT
ctrl_c() {
clear
echo $red"[#]> (Ctrl + C ) Detected, Trying To Exit ... "
echo $cyan"[#]> Thanks"
sleep 1
echo ""
echo $white"[#]> see you gayn :)"
sleep 1
exit
}

lagi=1
while [ $lagi -lt 6 ];
do
echo ""
echo $b "1.  ohmyzsh${enda}";
echo $r "2.  ebeckkansas${endc}";
echo $g "3.  terkey${endc}";
echo $c "4   Lazymux${endc}";
echo $r "5.  Tools-X${endc}";
echo $r "6. Exit${endc}";
echo ""
echo "ebeck kansas" |lolcat
read -p "ekid root :" pil;

# Nmap

case $pil in
1) ohmyzsh
apt update && apt upgrade
apt install git
git clone https://github.com/Cabbagec/termux-ohmyzsh
ls
cd termux-ohmyzsh
ls
./install.sh

;;

# ebeckkansas

2) apt update && apt upgrade
apt install git
apt install python
apt install python2
pip2 install requests
pip2 install mechanize
git clone https://github.com/ekidroot/ebeckhackfb.py
la
cd ebeckhackfb.py
python2 ebeckhackfb.py

;;

#RED_HAWK

3) git clone https://github.com/Tuhinshubhra/RED_HAWK
echo -e "${y} Installer RED_HAWK..."
echo -e "${y} cd RED_HAWK"
echo -e "${y} php RED_HAWK.php"
cd /data/data/com.termux/files/home/RED_HAWK/
php /data/data/com.termux/files/home/RED_HAWK/ RED_HAWK.php

;;

#Lazymux

4) git clone https://github.com/Gameye98/Lazymux
echo "${y} Installer Lazymux..."
echo "${y} cd Lazymux"
echo "${y} python lazymux.py"
cd /data/data/com.termux/files/home/Lazymux/
python2 /data/data/com.termux/files/home/Lazymux/ lazymux.py

;;

#Tools-X

5) git clone https://github.com/Rajkumrdusad/Tool-X
echo "${y} Installer Tool-X..."
echo "${y} cd Tool-X"
echo "${y} sh install.aex"
cd /data/data/com.termux/files/home/Tool-X
bash /data/data/com.termux/files/home/Tool-X/sh install.aex

;;


6) echo "by ebeck kansas" | lolcat
exit
;;

*) echo "sorry, pilihan yang kamu cari tidak tersedia"
esac
done
done
