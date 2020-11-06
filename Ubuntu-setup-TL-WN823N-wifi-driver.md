# Building and installing using DKMS


## Setup up Driver
```
sudo apt-get install git linux-headers-generic build-essential dkms;
git clone https://github.com/Mange/rtl8192eu-linux-driver;
cd rtl8192eu-linux-driver;
sudo dkms add .;
sudo dkms install rtl8192eu/1.0;
echo "blacklist rtl8xxxu" | sudo tee /etc/modprobe.d/rtl8xxxu.conf;
echo -e "8192eu\n\nloop" | sudo tee /etc/modules;
echo "options 8192eu rtw_power_mgnt=0 rtw_enusbss=0" | sudo tee /etc/modprobe.d/8192eu.conf;
sudo update-grub; sudo update-initramfs -u;
systemctl reboot -i;
```


## Check if its Working
```
sudo lshw -c network;
```
You should see the line driver=8192eu


## Uninstall the Driver
```
sudo dkms uninstall rtl8192eu/1.0 --all
```


## Reference
- https://github.com/Mange/rtl8192eu-linux-driver
- https://www.tp-link.com/ph/home-networking/adapter/tl-wn823n/
