# Ansible roles boilerplate

An easy Ansible boilerplate to manage your VPS set up through ansible roles.

## Install vagrant for test purpose

- Set up a test VM `vagrant up`

- Destroy your VM `vagrant destroy`

All docs about Vagrant could be found on the doc : https://www.vagrantup.com/docs/cli

## Execute ansible playbook example

Examples :

- Execute entire production script to the production environnement  `ansible-playbook projects/test/3_production.yml -i ./inventories/prod.yaml`

- Execute only the `cronjobs` steps of the install script in the dev environnement `ansible-playbook projects/test/2_install.yml -i ./inventories/test.yaml --tags="cronjobs"`


**Ansible galaxy roles**

Only from geerlingguy

- nginx (https://galaxy.ansible.com/geerlingguy/nginx)
- ntp (https://galaxy.ansible.com/geerlingguy/ntp)
- certbot (https://galaxy.ansible.com/geerlingguy/certbot)
