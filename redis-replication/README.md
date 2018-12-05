```
+-----------+
requirement
ansible 2.7+,python2.7,centos7+
+-----------+

```

```
```
excute example
```
create hosts files (define ansible inventory)
ansible-playbook -i hosts redis-replication.yml -e "target=rediscluster"
```
