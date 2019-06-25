# ansible-Django

Ansible Playbook for Installing  a Django Application. It Will Install Mysql With Nginx In Order To Distribute The Traffic Across The Web Server .

Please follow the below Steps :

1- Clone the template repository

git clone https://github.com/kimoaliali/ansible-playbook.git

2- Configure The Hosts File as below, But You Have To Replace The IP To Your Webserver And Database Serve . 

[webserver]

192.168.8.101
192.168.8.102
192.168.8.103

[database]

192.168.8.104

3- Install Nginx Loadbalancer .

ansible-playbook loadbalancer.yml

4- Install Mysql database .

ansible-playbook database.yml

5- Install Django Application .

ansible-playbook django.yml

6- Restart the server .

ansible-playbook restart_services.yml



