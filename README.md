# Ansible Code to deploy a HashiCorp Nomad Cluster

This playbook will deploy a Nomad and Consul cluster

## Software Deployed

[HashiCorp Nomad](https://www.nomadproject.io/) 1.0.0-beta3
[HashiCorp Consul](https://www.consul.io/) 1.9.0

## Hosts

You need between 3 and 5 server nodes
This has been tested on Ubuntu 18.04 ARM64 and AMD64 architectures.

If you are running the enterprise version of Nomad make sure you add the license files in the files directory

* consul.hclic
* nomad.hclic

and uncomment the `License Nomad and Consul` section before running the playbook.

## General Notes

This is not a secure deployment.
There are no ACL's enabled
There is no Gossip encryption.

You can get to the Nomad UI by opening

* http://SERVERURL:4646

You can get to the Consul UI by opening

* http://SERVERURL:8500