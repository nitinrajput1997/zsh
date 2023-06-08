# zsh

### Install zsh and ohmyzsh:
```
sudo apt install zsh git -y
sh -c "$(curl -fsSL https://raw.github.com/ohmyzsh/ohmyzsh/master/tools/install.sh)"
```

### Move to plugins directory:
```
cd ~/.oh-my-zsh/plugins
```

###  Clone plugins:
```
git clone https://github.com/zsh-users/zsh-autosuggestions.git
git clone https://github.com/zsh-users/zsh-syntax-highlighting.git
```
### Open config file:
```
vim ~/.zshrc
```
add the following lines in ~/.zshrc file:
```
# zsh plugins
plugins=(git
zsh-autosuggestions
zsh-syntax-highlighting
docker docker-compose
kubectl kubectx kube-ps1
)
```
### In the end add  this to bashrc file and after that exit from terminal
```
vim ~/.bashrc
exec zsh #adding this line
```
