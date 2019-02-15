
```
+-----------+
requirement
ansible 2.7+,python2.7,centos7+
rabbitmq 3.7+, erlang 21.2+
+-----------+

```

excute example
```
create hosts files (define ansible inventory)
ansible-playbook -i hosts rabbitmq-cluster.yml -e "target=worker"
