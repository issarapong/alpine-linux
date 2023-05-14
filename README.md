# alpine-linux
alpine-linux

#### Change to root privileges 
```
doas -s
```
#### Install Docker
```
apk add docker
```
#### Start Docker on boot
```
rc-update add docker default
service docker start
```
