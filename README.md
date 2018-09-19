```
+--------------+
initailize maven tomcat jdk running environment
using ansible 2.6
create hosts file as ansible inventory
+--------------+
```
```
+--------------+
command sample:
ansible-playbook -i hosts -e "target=jdk" install_tomcat.yml
+--------------+
```
