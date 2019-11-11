# general

This is a ansible role to install and upgrade your [cups](https://www.cups.org/) printserver to the latest version. It does the installation itself, existing installations get upgraded. The `printserver` group_vars configuration contains the `apt_packages` variable, where driver packages for all common printer manufacturers are prepared. Just uncomment the matching ones.

The role was developed on [Raspbian](https://raspbian.org/), but should run on every Debian based system. 

# how to use

1. change the variables in the inventory/group_vars/{printserver,all} files.
2. change the inventory/hosts file

After that you can run it with the command `ansible-playbook playbooks/printserver.yml`


