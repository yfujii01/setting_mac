# setting_mac

```sh
# brew
/usr/bin/ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"

# cask
brew tap homebrew/cask

# chrome
brew cask install google-chrome

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
```
