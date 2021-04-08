### yum으로 HPE DL서버군 패키지 설치

## 1. repository 생성
```C
cat > /etc/yum.repos.d/hpe.repo
[HPE-Repository]
name=HPE-Red Hat Linux $releasever - $basearch
baseurl=http://downloads.linux.hpe.com/SDR/downloads/ServicePackforProLiant/RedHat/$releasever/$basearch/current/
enabled=1
gpgcheck=1
gpgkey=http://downloads.linux.hpe.com/SDR/downloads/ServicePackforProLiant/GPG-KEY-ServicePackforProLiant/GPG-KEY-ServicePackf


Ctrl+D
```

## 2. yum update

	yum update


## 3. Install

	yum install ssacli