# Fresh Install Setup for Ubuntu

## Installation

### Node JS
```
sudo apt-get install curl
```

```
curl -sL https://deb.nodesource.com/setup_13.x | sudo -E bash -
```

```
sudo apt-get install nodejs
```

### Git 
```
sudo apt install git
```

### Slack
```
wget https://downloads.slack-edge.com/linux_releases/slack-desktop-4.0.2-amd64.deb
```

```
sudo apt install ./slack-desktop-*.deb
```

### Visual Studio Code
```
sudo apt install software-properties-common apt-transport-https wget
```

```
wget -q https://packages.microsoft.com/keys/microsoft.asc -O- | sudo apt-key add -
```

```
sudo add-apt-repository "deb [arch=amd64] https://packages.microsoft.com/repos/vscode stable main"
```

```
sudo apt install code
```

### Altair
```
sudo snap install altair
```

## Git connection 
```
git config --global user.name "Ralph Largo"
```

```
git config --global user.email "devlargs@gmail.com"
```

```
ssh-keygen -t rsa -C "devlargs@gmail.com"
```

```
cat ~/.ssh/id_rsa.pub
```














