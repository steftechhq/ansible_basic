# intro

## ping

### without ansible.cfg
ansible all --key-file ~/.ssh/ansible1 -i inventory -m ping

### with config file
```cfg
[defaults]
inventory=inventory
private_key_file=~/.ssh/ansible1
```

ansible all -m ping

## gather_facts
ansible all -m gather_facts
ansible all -m gather_facts --limit IP ADDRESS //limit against specific server


