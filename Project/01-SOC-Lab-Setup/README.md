Minimum requirements
CPU: 4 Cores minimum
RAM: 8 GB minimum (16 GB recommended)
Storage: 15 GB+ of free space. 

This project documents the installation of the Wazuh all-in-one platform on an Ubuntu Server 24.04 virtual machine. 
The goal is to prepare a Security Information and Event Management (SIEM) solution for my SOC home lab.

Good practice is to ensure all system repositories and packages are fully upgrade
Open terminal type
```bash
sudo apt update && sudo apt upgrade -y
```


Download Wazuh
Use curl to fetch the newest automated script deployment package directly from the official Wazuh Packages Repository
```bash
curl -sO https://packages.wazuh.com/4.14/wazuh-install.sh
```

img:

Make it executable
```bash
chmod +x wazuh-install.sh
```

Install Wazuh
```bash
sudo ./wazuh-install.sh -a
```


After installation you will have a User name (admin) and password(generated password)
copy the password and save it!
You can now run wazuh
Launch a browser and navigate to https://<YOUR_SERVER_IP>
login using your username and password.

ip host ussualy 127.0.0.1 (localhost)
Port 443/TCP: Wazuh web dashboard interface.
Port 1514/TCP: Wazuh agent connection for security events.
Port 1515/TCP: Wazuh agent enrollment/registration.
Port 9200/TCP: Wazuh indexer REST API


## Skills Demonstrated

- Ubuntu Linux Administration
- Package Management
- SIEM Deployment
- Wazuh Installation
- Virtual Machine Management
- SOC Lab Configuration
