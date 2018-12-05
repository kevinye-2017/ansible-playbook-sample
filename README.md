```
+-----------+
requirement
ansible 2.4.3+,python2.7,centos7+
+-----------+

```

```
+-----------+
some best practice example for ansible playbook roles
include tomcat,redis-replication,zabbix-agent etc...
+-----------+
```
excute example
```
create hosts files (define ansible inventory)
ansible-playbook -i hosts -e "target=zabbix" deploy_zabbix_agentd.yml
ansible-playbook -i hosts -e "target=tomcat" install_tomcat.yml
```
