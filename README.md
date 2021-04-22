# Ansible roles boilerplate

![ci badge](https://github.com/syskin/expressjs-boilerplate/workflows/CI/badge.svg)
[![GitHub version](https://img.shields.io/badge/version-v1.0.0-blue.svg)](https://github.com/syskin/expressjs-boilerplate)
[![Sync Vulnerabilities Status](https://app.snyk.io/test/github/syskin/expressjs-boilerplate/badge.svg)](https://snyk.io/test/github/syskin/expressjs-boilerplate)

An easy Ansible boilerplate to manage your VPS/Server set up through Ansible roles.

## Install Vagrant locally for test purpose

- Set up a test VM `vagrant up`

- Destroy your VM `vagrant destroy`

All docs about Vagrant could be found on the doc : https://www.vagrantup.com/docs/cli

## Execute Ansible playbook example

Examples :

- Execute entire production script to the production environnement  `ansible-playbook projects/test/3_production.yml -i ./inventories/prod.yaml`

- Execute only the `cronjobs` steps of the install script in the dev environnement `ansible-playbook projects/test/2_install.yml -i ./inventories/test.yaml --tags="cronjobs"`


## Ansible galaxy roles

Only from geerlingguy

- nginx (https://galaxy.ansible.com/geerlingguy/nginx)
- ntp (https://galaxy.ansible.com/geerlingguy/ntp)
- certbot (https://galaxy.ansible.com/geerlingguy/certbot)
