# Ansible Openstack Infrastructure and Service Deployment

This Ansible Playbook contains templates to deploy:

- Network infrastructure (networks, subnets, routers and security groups)
- Instances 
- Service Roles

Detailed information:

config.yml: Contains all necessary variables to deploy templates

create_network_infrastructure.yml, that deploys (in this template):

- 2 networks (management and Service)
- 2 Subnets with DHCP pools defined and static routes for instances attached
- 2 routers attached to external networks
- Security Groups and their rules

create_instances.yml, that deploys X instances

inventory.py: Dynamic Inventory to request information about Openstack instances

platform.yml: Contains template structure to deploy services