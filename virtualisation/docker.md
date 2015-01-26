# Docker

## Load the docker daemon in ubuntu
```
sudo service docker.io restart
```
To use docker without sudo, add the user to the group docker
```
sudo gpasswd -a ${USER} docker
```


**Note**
It could be needed to install 'apparmor' if not available:
```
sudo apt-get install apparmor
```