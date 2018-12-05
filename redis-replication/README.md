```
+-----------+
requirement
ansible 2.7+,python2.7,centos7+
stable version  redis-5.0.2 (source code compilation)
use sentinel for auto switch master role
+-----------+

```

```
atleast 2 ip for redis-relication!!!
the first ip is used as the default redis-master
use systemd to manage redis-server and sentinel-server
```

excute example
```
create hosts files (define ansible inventory)
ansible-playbook -i hosts redis-replication.yml -e "target=rediscluster"
```
