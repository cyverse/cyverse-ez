# cyverse-ez

This repo contains the ansible for CyVerse's ez command line facility. To use, follow these steps:

1. install ansible on the system (e.g. apt-get, yum, from source)
2. use ansible-pull: ansible-pull -v -U https://github.com/cyverse-org/cyverse-ez.git -d /opt/cyverse-ez -i locahost -o 
3. logout and login to your system (to re-read the system-level profile environment)
4. type "ez" for the help

Other notes:
* Ansible v2.0+ is supported
* Requires access to Ansible Galaxy and the ansible-galaxy command
* Modifications to the ez_setup role found in this repo should only be for system profile changes only 
* All other roles (e.g. software installation) should be added through Ansible Galaxy or a git repo, external to this repo
* The variable CYVERSE_INSTALL_ROOT, if defined, will change the install directory for software. Defaults to /opt
