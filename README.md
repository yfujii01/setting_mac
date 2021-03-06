# setting_mac

```sh
# brew
/usr/bin/ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"

# 最新のbrewではcaskが自動インストールらしいのでcaskを独自に入れない
# cask
## brew install caskがいるかも？
## brew install ~~は動くが、brew cask listやbrew cask search ~~は失敗した
## brewとか再インストールしたり色々して治った
##brew tap homebrew/cask

# gitは最初から入っているがbash_completion.dがないので入れる
brew install git

# terminal
brew cask install iterm2

brew install peco
brew install ghq
brew install hub

# chrome
brew cask install google-chrome

# コマンド
brew install wget

# ssh setting
mkdir ~/.ssh

# 中身はLastPassから
vi ~/.ssh/id_rsa

chmod 600 ~/.ssh/id_rsa 

# ime
brew cask install google-japanese-ime
## OS再起動
sudo reboot

# PC名変更
# システム環境設定 > 共通 > コンピュータ名

# dotfiles
curl -L https://raw.github.com/yfujii01/dotfiles/master/dotfiles.sh > ~/dotfiles.sh
sh ~/dotfiles.sh
exec $SHELL -l

# vscode
brew cask install visual-studio-code

# anyenv
git clone https://github.com/riywo/anyenv ~/.anyenv
exec $SHELL -l

# キーボード割当変更
brew install Caskroom/cask/karabiner-elements
# fnとcapsを入れ替える


# 言語インストール
anyenv install nodenv
anyenv install rbenv
anyenv install pyenv
anyenv install jenv
exec $SHELL -l

brew tap caskroom/versions
brew cask install java
/usr/libexec/java_home -V
jenv add $(/usr/libexec/java_home -v 10)
jenv global 10.0

nodenv install 10.4.1
nodenv global 10.4.1

pyenv install 3.6.5
pyenv global 3.6.5

rbenv install 2.5.1
rbenv global 2.5.1

# vagrant
brew cask install virtualbox
brew cask install vagrant

# centos
vagrant box add CentOS7_x64 https://github.com/tommy-muehle/puppet-vagrant-boxes/releases/download/1.1.0/centos-7.0-x86_64.box

mkdir -p ~/VM/CentOS7_x64
cd ~/VM/CentOS7_x64

vagrant init CentOS7_x64
vagrant up


# docker
brew cask install docker
open /Applications/Docker.app
## GUIで確認画面が表示される


```
