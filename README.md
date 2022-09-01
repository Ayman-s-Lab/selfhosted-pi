# selfhosted-pi

my self hosted stuff
![Logo](images/main.jpg)
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
sudo apt install nvim
    ...
        ...
            ...
```

### installing docker

to install docker, clone this repo and run the install script.

```
git clone https://github.com/Ayman-s-Lab/selfhosted-pi.git
cd selfhosted-pi/installation-scripts
./docker.sh
```
