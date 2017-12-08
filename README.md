PCGRIP: Personal Cancer Gene Reporter StackStorm Integration Pack
=================================================================

WARNING: Work in Progress, incubation stage

This pack is meant to be used to control cancer reporting software such as the [PCGR](https://github.com/sigven/pcgr).

It depends on the [StackStorm-ansible pack](https://github.com/StackStorm-Exchange/stackstorm-ansible) for instantiating and building
a fully functional PCGR instance. The deployment details and dependencies to tilt up such an instance are coded as ansible roles (and playbooks) in
[pcgr-deploy](https://github.com/umccr/pcgr-deploy).

In order to submit data samples to the running instance, a barebones Flask webservice, [pcgr-webservice](https://github.com/umccr/pcgr-webservice),
is used to send and execute the processing on uploaded VCF files.

This pack is following the StackStorm-ansible blueprint throughly described in the [Ansible-ChatOps StackStorm blogpost](https://stackstorm.com/2015/06/24/ansible-chatops-get-started-%F0%9F%9A%80/).
