Cacti server setup wizard

this script requires git and unzip

#Debian To use the script
git clone https://github.com/abr1server/cacti-auto-install.git
cd cacti-auto-install
chmod +x cacti-setup-wizard-debian-Ubuntu.sh
./cacti-setup-wizard-debian-Ubuntu.sh
RUN THE SCRIPT AS ROOT!!

The script also works on RHEL however you MUST enable EPEL prior to running the script and ensure its working to enable RHEL EPEL reports you can use the following command

yum install https://dl.fedoraproject.org/pub/epel/epel-release-latest-7.noarch.rpm
features are
-download either chosen or latest version of cacti
-autoconfigure database either with defaults or chose credentials
-auto tunes MariaDB using cacti recommended settings
-auto-populates cacti database
-downloads all needed packages for cacti install
-asks if you want to install spine if so it will automatically compile it
-adds system user and assigns permissions to folders
-downloads and installs plugins




Debug Add more plugins to download option
add option to select specific plugins from list
Document script

BUGS

June 24th 2024 - Script is not working on Centos 8 will have a fix soon !
![spring](https://github.com/abr1server/cacti-auto-install/assets/119709998/bbd0dd4b-5699-4079-a65c-7f2df5d436d4)

www.Abr1Server.com

