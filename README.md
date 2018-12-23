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

| Variable       | Description |
| -------------- |-------------|
| git_username   | username of the user which should used for git |
| git_password   | password for the given git_user |
| git_repo       | the path to the git repository the files should be pushed to |
| git_branch     | the branch it should pushed to |

Disclaimer: Output parsing from json to more human readable console output is not possible.

### add_vrf.yml

Adds a new VRF similar to the UC2 from the exercise yang last week.

| Variable       | Description |
| -------------- | ----------- |
| vrf_name       | Name of the new VRF |
| route_target   | Route target. Will be used for export and import |
| route_distinguisher | Route distinguisher of the VRF |