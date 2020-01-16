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

### Slack

```
wget https://downloads.slack-edge.com/linux_releases/slack-desktop-4.0.2-amd64.deb
sudo apt install ./slack-desktop-*.deb
```

### Visual Studio Code

```
sudo apt install software-properties-common apt-transport-https wget
wget -q https://packages.microsoft.com/keys/microsoft.asc -O- | sudo apt-key add -
sudo add-apt-repository "deb [arch=amd64] https://packages.microsoft.com/repos/vscode stable main"
sudo apt install code
```

---

### Other Software to be downloaded via website

I do not recommend these softwares to be downloaded via command line interface because it doesnt show the proper icons when it is being displayed on the taskbar.

- Gitkraken
