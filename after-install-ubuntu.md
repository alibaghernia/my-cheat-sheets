# After install ubuntu

### Install cli tools

```bash
sudo apt update
sudo apt upgrade
sudo apt install git curl wget npm nodejs zsh tree 
```

### Install drivers

```bash
sudo ubuntu-drivers autoinstall
```

### Install ohmyzsh

```bash
sh -c "$(curl -fsSL https://raw.github.com/ohmyzsh/ohmyzsh/master/tools/install.sh)"
```

### Install vscode

```bahs
sudo snap install code --classic
```

### Install corepack

```bash
npm i -g corepack
corepack enable
```

### Genrate ssh key github

```bash
ssh-keygen -t ed25519 -C "your@email.com"
```

### Install download manager

```bash
sudo add-apt-repository ppa:persepolis/ppa
sudo apt update
sudo apt install persepolis
```

### Install telegram desktop

```bash
sudo snap install telegram-desktop
```
