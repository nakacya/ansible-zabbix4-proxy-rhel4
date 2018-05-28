
# Installation for Zabbix4 

clone repository
```
git clone https://github.com/nakacya/ansible-zabbix4-proxy-rhel7.git
```

configuration
```
vim ./ansible-zabbix-rhel7/group_vars/zabbix4-proxy-server-mysql
```

place of installation
```
vim ./ansible-zabbix4-proxy-rhel7/hosts
```

execute
```
cd ansible-zabbix4-rhel7
ansible-playbook -u <userName> ./zabbix4-proxyr-mysql.yml

# public key authentication
ansible-playbook --private-key=<pathToPrivatekey> -u <userName> ./zabbix4-proxy-mysql.yml
```

mysql security setting
```
mysql_secure_installation
```

First time login
```
http://<ipAddress or DNS>/zabbix/
user: Admin
pass: zabbix
```
#ansible-zabbix4-rhel7
