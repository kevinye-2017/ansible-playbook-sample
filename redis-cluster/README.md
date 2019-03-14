6 nodes
excute example
```
create hosts files (define ansible inventory)
ansible-playbook -i hosts redis-cluster.yml -e "target=redis" -f 6
```
