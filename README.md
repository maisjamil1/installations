# Installations

# Ubuntu Linux
- to enter BIOS (Boot Menu) - ThinkPad
https://support.lenovo.com/jo/en/solutions/ht500222-recommended-ways-to-enter-bios-boot-menu-thinkpad-thinkcentre-thinkstation

- install Linux
https://www.youtube.com/watch?v=G7ffzC4S0A4&t=77s


# Install Terminator 
```
sudo add-apt-repository ppa:gnome-terminator

sudo apt-get update

sudo apt-get install terminator
```

# Installing ZSH
- `sudo apt install zsh`
- `zsh --version`
- Make it your default shell:`chsh -s $(which zsh)`
https://askubuntu.com/questions/131823/how-to-make-zsh-the-default-shell
# Installing OH MY ZSH
- `sudo apt install curl wget git `
- `sh -c "$(curl -fsSL https://raw.githubusercontent.com/ohmyzsh/ohmyzsh/master/tools/install.sh)"`
- https://www.youtube.com/watch?v=ANxLmiLXtFM
- https://qirolab.com/posts/install-and-setup-oh-my-zsh-on-ubuntu-system



# Docker
-  `sudo apt-get update`
```
sudo apt-get install \
    apt-transport-https \
    ca-certificates \
    curl \
    gnupg \
    lsb-release
```
- `curl -fsSL https://download.docker.com/linux/ubuntu/gpg | sudo gpg --dearmor -o /usr/share/keyrings/docker-archive-keyring.gpg`
```
echo \
  "deb [arch=amd64 signed-by=/usr/share/keyrings/docker-archive-keyring.gpg] https://download.docker.com/linux/ubuntu \
  $(lsb_release -cs) stable" | sudo tee /etc/apt/sources.list.d/docker.list > /dev/null
```
- `sudo apt-get update`
- `sudo apt-get install docker-ce docker-ce-cli containerd.io`
- `docker -v`
- Verify that Docker Engine is installed correctly by running the hello-world image.: `sudo docker run hello-world`
- P.S install docker extension on vscode
