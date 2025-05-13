For Ubuntu 22.04*

sudo systemctl mask power-profiles-daemon.service
sudo systemctl stop power-profiles-daemon.service

cp ./etc/* /etc/

sudo chmod +x /etc/systemd/set-mygovernor
sudo chmod +x /etc/systemd/system/mygovernor.service

sudo systemctl enable mygovernor.service
sudo systemctl start mygovernor.service

#It also works on Ubuntu 20.04 but you have to 
#replace "power-profiles-daemon.service" with 
#"ondemand.service". The rest is the same.


#Credits: https://askubuntu.com/questions/1419396/how-to-force-enable-performance-mode-in-ubuntu-22-04
#storestyggeulv
