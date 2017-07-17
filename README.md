# joke-programs

## Introduction

This program installs joke program on CentOS7.  

Program list

* asciiquarium
* beer-mug
* cmatrix
* cowsay
* figlet
* fortune-mod
* lolcat
* pong
* sl

## How To install programs

1. install ansible 

```
    sudo yum -y install epel-release
    sudo yum -y install ansible
```

2. excute playbook as root

`ansible-playbook -i localhost all.yml`

3. reload shell profile as root

`source /etc/profile.d/go.sh`
