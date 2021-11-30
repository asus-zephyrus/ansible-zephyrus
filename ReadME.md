# Zephyrus Setup - 

## install ansible collection for flatpak
```
ansible-galaxy collection install community.general
```

## Run the playbook 
```
This -K is for user password not root. by default we run this as root ( not a good practice )

ansible-playbook opensuse-playbook.yml -e "@group_vars/opensuse.yml" -K
```