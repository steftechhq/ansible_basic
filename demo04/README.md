# ad-hoc commands intro

## ping

### without ansible.cfg
```sh
ansible-playbook --list-tags site.yml

ansible-playbook --tags centos --ask-become-pass site.yml
```
