```
+-----------+
requirement
ansible 2.4.3+,python2.7,centos7+
+-----------+

```
改变master数量，需修改redis-replication/redis-replication/tasks/main.yml
if loop.index0 == 0，默认ip第一个为master，例如我想做10台redis集群,其中6台用作读写，其余4台用作只读  if loop.index0 <= 5
```
+-----------+
some best practice example for ansible playbook roles
include tomcat,redis-replication,zabbix-agent etc...

all roles are configurable (in ansible roles default directory)
+-----------+
```
excute example
```
create hosts files (define ansible inventory)
ansible-playbook -i hosts -e "target=zabbix" deploy_zabbix_agentd.yml
ansible-playbook -i hosts -e "target=tomcat" install_tomcat.yml
```
