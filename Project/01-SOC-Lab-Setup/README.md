Minimum requirements
CPU: 4 Cores minimum
RAM: 8 GB minimum (16 GB recommended)
Storage: 15 GB+ of free space. 

This is my experience in installing  wazuh inside a virtual machine in ubuntu.

Good practice is to ensure all system repositories and packages are fully upgrade
Open terminal type
bash: sudo apt update && sudo apt upgrade -y

img:

Download Wazuh
Use curl to fetch the newest automated script deployment package directly from the official Wazuh Packages Repository
curl -sO https://packages.wazuh.com/4.14/wazuh-install.sh

img:

Make it executable
chmod +x wazuh-install.sh

Install Wazuh
sudo ./wazuh-install.sh -a
 img:


After installation you will have a User name (admin) and password(generated password)
copy the password and save it!
You can now run wazuh
Launch a browser and navigate to https://<YOUR_SERVER_IP>
login using your username and password.
ip host

