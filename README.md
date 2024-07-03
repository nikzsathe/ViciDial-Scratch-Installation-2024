# VICIDIAL INSTALLATION SCRIPTS (Default is Eastern Time Zone US)
# Centos7 and AlmaLinux8 Vicidial Install pre_requisites
# Avoid on CentOS7 since its dead and no updates are available so it'll not work for CentOS7. Go for Alma Linux 8 

```

hostnamectl set-hostname xxxxxx.xxxxx.xxx
### Use YOUR SubDomain

vi /etc/hosts
##Change domain name for actual server ip (xxx.xxx.xxx.xxx   complete domain name    subdomain only)

timedatectl set-timezone America/New_York

yum check-update
yum update -y
yum -y install epel-release
yum update -y
yum install git -y
yum install -y kernel*

sed -i 's/SELINUX=enforcing/SELINUX=disabled/g' /etc/selinux/config    

reboot

````
  Reboot Before running this script

# Install VICIDIAL scripts

```
git clone https://github.com/nikzsathe/ViciDial-Scratch-Installation-2024.git
cd ViciDial-Scratch-Installation-2024
```

# Execute Centos7 Vicidial Install
```
chmod +x vicidial-install-c7.sh
./vicidial-install-c7.sh
```

# Execute AlmaLinux8 Vicidial Install
```
chmod +x vicidial-install-almalinux8.sh
./vicidial-install-almalinux8.sh
```
# Execute AlmaLinux9 Vicidial Install
```
chmod +x vicidial-install-almalinux9.sh
./vicidial-install-almalinux9.sh
```

# Install WEBRTC for VICIDIAL Now
# DO THIS IF YOU HAVE PUBLIC DOMAIN WITH PUBLIC IP ONLY

```
chmod +x vicidial-enable-webrtc.sh
./vicidial-enable-webrtc.sh
```#   V i c i D i a l - S c r a t c h - I n s t a l l a t i o n - 2 0 2 4  
 