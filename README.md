# Первоначальная настройка рабочего окружения

```bash
sudo apt-get update
sudo apt-get -y full-upgrade

sudo add-apt-repository ppa:graphics-drivers/ppa
sudo ubuntu-drivers autoinstall

sudo apt-get install -y mc build-essential git screenfetch curl gcc g++ make apt-transport-https ca-certificates gnupg-agent software-properties-common fonts-powerline

sudo add-apt-repository ppa:ondrej/php
sudo apt-get install -y php7.3-cli php7.3-mysql php7.3-mbstring php7.3-mbstring php7.3-sqlite3 php7.3-gd php7.3-sybase php7.3-bz2 php7.3-curl php7.3-xml


curl -sS https://getcomposer.org/installer | sudo php -- --install-dir=/usr/local/bin --filename=composer


curl -sL https://deb.nodesource.com/setup_10.x | sudo -E bash -
sudo apt-get install -y nodejs
```

#### Установка ZSH
```bash
sudo apt-get install -y zsh
sh -c "$(curl -fsSL https://raw.github.com/robbyrussell/oh-my-zsh/master/tools/install.sh)"


git clone https://github.com/zsh-users/zsh-syntax-highlighting ${ZSH_CUSTOM:-~/.oh-my-zsh/custom}/plugins/zsh-syntax-highlighting
git clone https://github.com/zsh-users/zsh-autosuggestions ${ZSH_CUSTOM:-~/.oh-my-zsh/custom}/plugins/zsh-autosuggestions
git clone https://github.com/zsh-users/zsh-completions ${ZSH_CUSTOM:=~/.oh-my-zsh/custom}/plugins/zsh-completions
git clone https://github.com/rulweb/zsh-rulweb ${ZSH_CUSTOM:=~/.oh-my-zsh/custom}/plugins/zsh-rulweb
```

#### Отредактировать файл
```bash
nano ~/.zshrc
```

#### Найти
```text
plugins=(git)
```

#### Заменить на
```text
plugins=(
	git
	zsh-syntax-highlighting
	zsh-autosuggestions
	zsh-completions
	zsh-rulweb
)
```

## Установка софта из Snap пакетов
```bash
sudo snap install vlc
sudo snap install sublime-text --classic
sudo snap install telegram-desktop

sudo snap install phpstorm --classic
sudo snap install goland --classic
sudo snap install intellij-idea-ultimate --classic
sudo snap install webstorm --classic
```
