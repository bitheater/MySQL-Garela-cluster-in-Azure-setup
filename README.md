# MySQL-Garela-cluster-in-Azure-setup
How to configure a MySQL Galera cluster to work with Azure.
This document asumes that a MytSQL cluster is being installed already in 3 instances of an Azure's cloud service, for more information about how to install a Galera custer please got to:
http://galeracluster.com/documentation-webpages/installmariadb.html

## Microsoft Azure Xplat-CLI
  
    Ref: https://github.com/Azure/azure-xplat-cli
    cross-platform command line interface for developers and IT administrators to develop, deploy and manage Microsoft Azure applications.
    - Install Azure Xplat-CLI
    ## Installation

### Install from npm

You can install the azure-cli npm package directly.
```bash
npm install -g azure-cli
```

### Install on Ubuntu
The Xplat-CLI requires Node.js. Installation varies slightly by Ubuntu version.

**Ubuntu 14.04 Trusty Tahr**

On Ubuntu 14, the Node.js package is called nodejs-legacy. The npm package is installed first to get the Node Package Manager used to install the CLI.

```bash
sudo apt-get install nodejs-legacy
sudo apt-get install npm
sudo npm install -g azure-cli
```
**Ubuntu 12.04 Precise Pangolin**

On Ubuntu 12, the version of Node.js available in the default package manager is too old. You can use the Personal Package Archive feature to install the current binary distribution. First, install the curl package to easily retrieve the install script.

```bash
sudo apt-get install curl
curl -sL https://deb.nodesource.com/setup | sudo bash -
sudo apt-get install -y nodejs
sudo npm install -g azure-cli
```

## MySQL Galera Notification Command

    Ref: http://galeracluster.com/documentation-webpages/notificationcmd.html
    

