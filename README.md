# Ansible kuberntes deploy scripts
Command to run scripts:
```
ansible-playbook -i hosts main.yml
```

Example of `hosts` file:
```
[masters]
master ansible_host=1.1.1.1 ansible_user=root

[workers]
worker1 ansible_host=1.1.1.2 ansible_user=root
worker2 ansible_host=1.1.1.3 ansible_user=root

[all:vars]
ansible_python_interpreter=/usr/bin/python3

```