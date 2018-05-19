# promstack-ansible

## Status

This playbook enable user to deploy a basic monitoring stack based on:

- [Prometheus](https://prometheus.io)
- [Grafana](https://grafana.com)
- [Node Exporter](https://github.com/prometheus/node_exporter)
- [cAdvisor](https://github.com/google/cadvisor)

With an optional install of [Ceph Exporter](https://github.com/digitalocean/ceph_exporter/tree/luminous)

## Requirments 

- [Install Ansible](http://docs.ansible.com/ansible/intro_installation.html)

## Usage

1. Copy group_vars/all.yml.sample to group_vars/all.yml

2. Fill in variables based on deployment enviornment.

3. Copy hosts.example and fill in hosts IPs or hostname.

4. Run ```ansible-playbook -i hosts site.yml``` to deploy
