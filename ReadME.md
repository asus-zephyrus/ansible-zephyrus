# Zephyrus Setup - 

## install ansible collection for flatpak
```
ansible-galaxy collection install community.general
ansible-galaxy install ansible.install-gcloud
ansible-galaxy install deekayen.awscli2
```

## Run the playbook ( opensuse ) 
```
This -K is for user password not root. by default we run this as root ( not a good practice )

ansible-playbook opensuse-playbook.yml -e "@group_vars/opensuse.yml" -K
```

## Run Playbook ( debian )
```
This -K is for user password not root. by default we run this as root ( not a good practice )

ansible-playbook debian-install.yml -e "@group_vars/debian-install.yml" -K
```