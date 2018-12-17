# Ansible
## Usage
Run the scripts with the following parameters:
```
ansible-playbook ./[script-name].yml -u [username] -k
```

## Scripts
### wr_and_list.yml
Saves the running-config to the startup-config, then lists all vlans on the device, lists all routes and saves them in the *out* folder.

### add_vrf.yml