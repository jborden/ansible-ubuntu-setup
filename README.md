# Ansible for setting up Ubuntu Desktop

This is my personal Ansible Desktop. It tries to replicate the feel
of macOS.

# Prerequistes

1. install ansible
```
sudo apt install ansible
```

2. enable passwordless sudo
```
sudo visudo
```

change the line
%sudo  ALL=(ALL:ALL) ALL
%sudo  ALL=(ALL:ALL) NOPASSWD: ALL
# Run Playbook

```
ansible-playbook playbook.yml
```
