# Ansible
## Usage
Run the scripts with the following parameters:
```
ansible-playbook ./[script-name].yml -u [username] -k
```

## Scripts
### wr_and_list.yml
Saves the running-config to the startup-config, then lists all vlans on the device, lists all routes and saves them in the *out* folder.
Also, it commits the folder to the given git repository.

Disclaimer: Output parsing from json to more human readable console output is not possible.

### add_vrf.yml

Adds a new VRF similar to the UC2 from the exercise yang last week.
