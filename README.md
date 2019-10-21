# ansible-examples

This repository contains a set of example Ansible playbooks for managing blockchain networks using the IBM Blockchain Platform. All of the example Ansible playbooks make use of the Ansible role `ibm.blockchain_platform_manager`, available from [Ansible Galaxy](https://galaxy.ansible.com/ibm/blockchain_platform_manager).

two-org-network
-------

The [two-org-network](two-org-network/README.md) directory contains an Ansible playbook for standing up a IBM Blockchain Platform network with two organizations, `Org1` and `Org2`. Each organization has two peers. The two peers are configured with a single channel, `channel1`. The FabCar sample contract is instantiated on this channel, with an endorsement policy stating that both organizations must endorse any transactions.

License
-------

Apache-2.0