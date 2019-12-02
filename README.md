# ansible-examples

[![Build Status](https://dev.azure.com/IBM-Blockchain/ansible-examples/_apis/build/status/IBM-Blockchain.ansible-examples?branchName=master)](https://dev.azure.com/IBM-Blockchain/ansible-examples/_build/latest?definitionId=2&branchName=master)

This repository contains a set of example Ansible playbooks for building Hyperledger Fabric networks using the IBM Blockchain Platform. All of the example Ansible playbooks make use of the Ansible role `ibm.blockchain_platform_manager`, available from [Ansible Galaxy](https://galaxy.ansible.com/ibm/blockchain_platform_manager).

two-org-network
-------

The [two-org-network](two-org-network/README.md) directory contains an Ansible playbook for building a Hyperledger Fabric network with two organizations, `Org1` and `Org2`. Each organization has two peers. The two peers are configured with a single channel, `channel1`. The FabCar sample contract is instantiated on this channel, with an endorsement policy stating that both organizations must endorse any transactions.

License
-------

Apache-2.0