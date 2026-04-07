# ad-hoc commands intro

## ping

### without ansible.cfg
```sh
ansible all --key-file ~/.ssh/ansible1 -i inventory -m ping
```
### with config file
```cfg
[defaults]
inventory=inventory
private_key_file=~/.ssh/ansible1
```

ansible all -m ping

## gather_facts
```sh
ansible all -m gather_facts
ansible all -m gather_facts --limit IP ADDRESS //limit against specific server
```

## apt
```sh
ansible all -m apt -a update_cache=true --become --ask-become-pass
ansible all -m apt -a name=vim --become --ask-become-pass

```