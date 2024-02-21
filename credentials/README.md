# azure vm info
- Ubuntu server(22.04 LTS): 1vcpu, 1gib ram with 60gb storage 
- Server IP address (20.229.177.80)
- Installed: 
    - nginx webserver (v1.18.0)
    - nodejs (v18.2.1)
    - mysql (v8.0.31)
    - certbot SSL for our domain
- add react build file in "/var/www/gdsd1restaurant/html"
- you can review our sites configurations on "/etc/nginx/sites-available"

# domain infos
- Taken a free domain from name.com and linked with our IP address
    - domain name: https://gdsd1restaurant.live
    - domain name from azure: https://gdsd1restaurant.westeurope.cloudapp.azure.com

# connect to azure vm from your local machine
- go to the path where pem file is located or download it in your machine
- to connect to the azure:
    - give permission to use the file
        - chmod 400 <keyname>.pem
    - run the below command
        - ssh -i <private key path>.pem 

# database connection 
- download the mysql workbench
- connect to azure server db
- create a connection and fill the below details
    - connection name: GDSD1Restaurant
    - connection method: Standard TCP/IP over SSH
    - ssh hostname: 20.229.177.80
    - ssh username: 
    - ssh key file: select our <private key>.pem file
    - mysql hostname: 127.0.0.1
    - mysql server port: 3306
    - username: stha24
    - password: Rest@urant123
    - connection image: https://prnt.sc/bl8DOnrniIF0
- create connection
