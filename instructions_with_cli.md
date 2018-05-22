# Installation with CLI

You do not need to download and install Sam Hewitt's Suru Icon, because it already comes installed under Lubuntu 18.04, Ubuntu 18.04 and above.

Firstly, you must have `git` and `svn` installed. 

```shell
sudo apt install curl git subversion wget
```

Choose one of two options — Git or SVN. We recommend strongly SVN, which is quicker like a MIllenium Falcon than Git. 

### Git

```shell
# If the folder icons doesn't exist
mkdir ~/.local/share/icons
# You need to enter in the icons folder to download the icons pack
cd ~/.local/share/icons
# Download the icon packs...
git clone https://github.com/Magog64/SURU-PLUS.git
git clone https://github.com/gusbemacbe/SURU-PLUS-DARK.git
git clone https://github.com/gusbemacbe/suru-plus-dark-lubuntu.git
# To update the next latest changes
git pull origin master 
# You need to rename these folders
mv SURU-PLUS Suru++
mv SURU-PLUS-DARK 'Suru++ Dark'
mv suru-plus-dark-lubuntu 'Suru++ Dark Lubuntu'
```

### SVN

```shell
# If the folder icons doesn't exist
mkdir ~/.local/share/icons
# Download quickly like a Millennium Falcon
svn export https://github.com/Magog64/SURU-PLUS/trunk/ ~/.local/share/icons/Suru++
svn export https://github.com/gusbemacbe/SURU-PLUS-DARK/trunk/ ~/.local/share/icons/Suru++\ Dark
svn export https://github.com/gusbemacbe/suru-plus-dark-lubuntu/trunk/ ~/.local/share/icons/Suru++\ Dark\ Lubuntu
# When we will update the icons, and if you want to update the icons, just overwrite
svn export --force https://github.com/Magog64/SURU-PLUS/trunk/ ~/.local/share/icons/Suru++
svn export --force https://github.com/gusbemacbe/SURU-PLUS-DARK/trunk/ ~/.local/share/icons/Suru++\ Dark
svn export --force https://github.com/gusbemacbe/suru-plus-dark-lubuntu/trunk/ ~/.local/share/icons/Suru++\ Dark\ Lubuntu
```
