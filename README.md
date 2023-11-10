
This playbook enable user to deploy a basic monitoring stack based on:

- [Prometheus](https://prometheus.io)
- [Grafana](https://grafana.com)
- [Node Exporter](https://github.com/prometheus/node_exporter)
- [cAdvisor](https://github.com/google/cadvisor)

With an optional install of [Ceph Exporter](https://github.com/digitalocean/ceph_exporter/tree/luminous)

## Requirments 

- [Install Ansible](http://docs.ansible.com/ansible/intro_installation.html)

## Usage

1. Fill in variables based on deployment enviornment: group_vars/all.yml
2. Fill in hosts IPs or hostname.
3. Run ```ansible-playbook -i hosts site.yml -e "promstack_action=deploy"``` to deploy

## Remove Deployment

To remove deployment, simply run

```ansible-playbook -i hosts destroy.yml```
