# Ansible roles to prepare Arm/Raspbian based k3s cluster 

## Prerequests

1. Write Armbian image to an sdcard
2. Insert it to a Pi
3. Boot it
4. Do First login, set a new password
5. copy your ssh key under root user

## Variables

- `network['address', 'dns', 'gateway']` fixed IP Address 
    Default: actual config

## Usage

`ansible-playbook -i path/to/inventory/ armbian-k3s.yml`

After preparation, you need to create the cluster and join the nodes manually