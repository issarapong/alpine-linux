# alpine-linux
alpine-linux,Cheap and fast build service <a href="https://af-south-1.console.aws.amazon.com/ec2/home#launchAmi=ami-02e81fa7058a761d2">Click</a>

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

#### Example run nginx images

```
 docker run --name mynginx1 -p 80:80 -d nginx
```
