# Fresh Install Setup for Ubuntu

## Installation

### Altair

```
sudo snap install altair
```

### Git

```
sudo apt install git
git config --global user.name "Ralph Largo"
git config --global user.email "devlargs@gmail.com"
ssh-keygen -t rsa -C "devlargs@gmail.com"
cat ~/.ssh/id_rsa.pub
```

### Mongo

```
sudo apt remove --autoremove mongodb-org
sudo rm /etc/apt/sources.list.d/mongodb*.list
sudo apt update
sudo apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv 4B7C549A058F8B6B
echo "deb [arch=amd64] http://repo.mongodb.org/apt/ubuntu bionic/mongodb-org/4.2 multiverse" | sudo tee /etc/apt/sources.list.d/mongodb-org-4.2.list
sudo apt update
sudo apt install mongodb-org
systemctl enable mongod.service
systemctl start mongod.service
mongo
```

### Node JS

```
sudo apt-get install curl
curl -sL https://deb.nodesource.com/setup_13.x | sudo -E bash -
sudo apt-get install nodejs
```

### PHP

```
sudo apt install software-properties-common
sudo add-apt-repository ppa:ondrej/php
sudo apt install php7.3 php7.3-common php7.3-opcache php7.3-cli php7.3-gd php7.3-curl php7.3-mysql
php -v
```

### Shutter

#### For v18 below
```
 sudo apt-get install shutter
```

#### For 20.04
```
sudo add-apt-repository -y ppa:linuxuprising/shutter
sudo apt-get update
sudo apt-get install -y shutter
```

### Spotify 
```
snap install spotify
```

### Slack

```
wget https://downloads.slack-edge.com/linux_releases/slack-desktop-4.0.2-amd64.deb
sudo apt install ./slack-desktop-*.deb
```

### Skype
```
wget https://go.skype.com/skypeforlinux-64.deb
sudo apt install ./skypeforlinux-64.deb
```

### Visual Studio Code

```
sudo apt install software-properties-common apt-transport-https wget
wget -q https://packages.microsoft.com/keys/microsoft.asc -O- | sudo apt-key add -
sudo add-apt-repository "deb [arch=amd64] https://packages.microsoft.com/repos/vscode stable main"
sudo apt install code
```

### VLC

```
sudo apt-get update
sudo snap install vlc
```

### Gitkraken
```
sudo snap install gitkraken --classic
```

---

### Other Software to be downloaded via website

I do not recommend these softwares to be downloaded via command line interface because it doesnt show the proper icons when it is being displayed on the taskbar.

- Composer

## Useful NPM Plugins

### Nodemon

```
npm install -g nodemon
```

### React Native

```
npm install -g expo-cli
```

### Typescript

```
npm install -g typescript
```

### Vue

```
npm install -g @vue/cli
```
