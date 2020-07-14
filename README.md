# ansible-examples

[![Build Status](https://dev.azure.com/IBM-Blockchain/ansible-examples/_apis/build/status/IBM-Blockchain.ansible-examples?branchName=master)](https://dev.azure.com/IBM-Blockchain/ansible-examples/_build/latest?definitionId=2&branchName=master)

⚠️ ⚠️ ⚠️

The IBM Blockchain Platform 2.5 release includes a new Ansible collection that can be used to build, operate & govern and grow blockchain networks.

The Ansible collection can be found here:

- Ansible collection documentation (https://ibm-blockchain.github.io/ansible-collection/)
- IBM Blockchain Platform documentation (https://cloud.ibm.com/docs/blockchain?topic=blockchain-ansible)
- Ansible Galaxy (https://galaxy.ansible.com/ibm/blockchain_platform)
- GitHub (https://github.com/IBM-Blockchain/ansible-collection/)

Support for the Ansible collection is included as part of the IBM Blockchain Platform.

It is strongly recommended that you use the Ansible collection instead of the Ansible role used by these examples.

You should only use these examples if you are building development networks and you wish to build a local network using Docker.

⚠️ ⚠️ ⚠️

This repository contains a set of example Ansible playbooks for building Hyperledger Fabric networks using the IBM Blockchain Platform. All of the example Ansible playbooks make use of the Ansible role `ibm.blockchain_platform_manager`, available from [Ansible Galaxy](https://galaxy.ansible.com/ibm/blockchain_platform_manager).

one-org-network
-------

The [one-org-network](one-org-network/README.md) directory contains an Ansible playbook for building a Hyperledger Fabric network with one organization, `Org1`. The organization has two peers. The two peers are configured with a single channel, `channel1`. The FabCar sample contract is instantiated on this channel.

two-org-network
-------

The [two-org-network](two-org-network/README.md) directory contains an Ansible playbook for building a Hyperledger Fabric network with two organizations, `Org1` and `Org2`. Each organization has two peers. The two peers are configured with a single channel, `channel1`. The FabCar sample contract is instantiated on this channel, with an endorsement policy stating that both organizations must endorse any transactions.

License
-------

Apache-2.0