# hashtopolis-docker

Ansible playbook to provision a hashtoplis setup in 3 docker containers with docker-compose. The application and database files are stored in volumes for persistence. The application is cloned from github.

## Quickstart
1. Create an inventory file
2. Customize `mysql_userpass` or any other variables
3. ansible-playbook setup-hashtopolis.yml
4. Follow initial setup instructions in hashtopolis UI using `db` as the hostname
