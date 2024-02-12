# Server Setup

## SSH
``` ssh <username>@<ip> ```

as root:  
Add user: ```adduser <username>```  
Delete user: ```userdel <username>```  
confirm user created: ```cat /etc/passwd | grep <username>```  
                        ```id <username>```

add user to sudo group:  
show groups of user: ``groups <username> show ``  
``usermod -aG sudo <username>``  
switch to sudo user: ``su - <username> ``

### UFW
``ufw status``  
``ufw status verbose``  
``ufw allow <port>``  
### Delete stuff

``rm -rf <directory-name> ``  

## Docker

``docker compose build ``  
``docker compose up ``
``docker compose up --detach`` ``docker compose up -d``

## Hi
1) Clone repo  
 ``sudo git clone https://github.com/Nizwe/construction.git  ``
 ``cd construction ``
 2) Build container  
 ``docker compose compose build ``
3) Rights to letsencrypt init  
 `` sudo chmod +x ./init-letsencrypt.sh ``  
 4) Run init  
``sudo ./init-letsencrypt.sh``  
