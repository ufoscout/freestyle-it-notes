# Docker

## Configuration
By default docker uses /var/lib/docker as folder, to change it modify the file "/etc/default/docker.io" and add "-g desiredFolder" to the line:
DOCKER_OPTS="-dns 8.8.8.8 -dns 8.8.4.4"
eg:
DOCKER_OPTS="-dns 8.8.8.8 -dns 8.8.4.4 -g /mnt"

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


## Work with images

```
docker pull -t latest <imageName>
# or
docker pull <imageName>:<tagname>
```