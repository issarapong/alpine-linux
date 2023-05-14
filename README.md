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
#### Enviroment after use Docker

```
/home/alpine # df -h
Filesystem      Size  Used Avail Use% Mounted on
devtmpfs         10M     0   10M   0% /dev
shm             218M     0  218M   0% /dev/shm
/dev/nvme0n1p2  989M  525M  398M  57% /
tmpfs            88M  324K   87M   1% /run
/dev/nvme0n1p1  486K  294K  192K  61% /boot/efi
cgroup_root      10M     0   10M   0% /sys/fs/cgroup
overlay         989M  525M  398M  57% /var/lib/docker/overlay2/cdaa18bf421e1d588899937d18844ae3f9f0feaddb0bac096a472df33fefd0f6/merged
```
