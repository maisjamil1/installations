# Installations

# Ubuntu Linux
- to enter BIOS (Boot Menu) - ThinkPad
https://support.lenovo.com/jo/en/solutions/ht500222-recommended-ways-to-enter-bios-boot-menu-thinkpad-thinkcentre-thinkstation

- install Linux
https://www.youtube.com/watch?v=G7ffzC4S0A4&t=77s


# Install Terminator 
'''
sudo add-apt-repository ppa:gnome-terminator

sudo apt-get update

sudo apt-get install terminator
'''




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
