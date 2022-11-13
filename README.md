# selfhosted-pi

my self hosted stuff
![Logo](pics/main.jpg)
in this project i have created a self hosted pi that can be used to host many services and applications.
This is a list of services and web applications can be hosted on your own server(s) too .
dont forget to give this project a star⭐ to support me.

## First Steps

- install the raspbian os on your sd card.
  you can follow this tutorial from [2:25](https://www.youtube.com/watch?v=gyMpI8csWis&t=1304s) ⏩ prep the Raspberry Pi.
- connect the raspberry pi to your wifi network.
- ssh into the raspberry pi using the ssh command.

```
ssh pi@ipaddress
```

- update and upgrade the system using the command below.

```
sudo apt update && sudo apt upgrade
```

- and reboot the system.

```
sudo reboot
```

congratulations you have now installed the raspberry pi.

- now you can install the following software.

```
sudo apt install git
sudo apt install neovim
    ...
        ...
            ...
```

### installing docker

to install docker, clone this repo and run the install script.

```
git clone https://github.com/Ayman-s-Lab/selfhosted-pi.git
cd selfhosted-pi/installation-scripts
chmod +rx docker.sh
./docker.sh
```
Remember to logout/reboot for the changes to take effect.
```
logout
```
ssh into the raspberry pi again
### installing portainer
portainer is a web application that can be used to manage and easily deploy your docker containers .

to install portainer, open th installation-scripts folder and run the install script.

```
cd installation-scripts
chmod +rx portainer.sh
./portainer.sh
```
yeah, now you can access portainer at http://ipaddress:9000 .

you created a new administrator user and chose docker as a container env aaand you are ready to go🎆.

Click Settings, in the bottom-left corner, and paste the Portainer v2 json file link from below into the "App Templates" box.
this is the one i use for my portainer.
i will create my own soon.

```
https://raw.githubusercontent.com/ntv-one/portainer/main/template.json
```
You're done! Now just click App Templates and deploy applications!


## Contributing :

- Open issue  .
- Fork and clone repository.
- Make Changes .
- Review changes .
- Send pull request .

Thank you for your interest in contributing to this project.
