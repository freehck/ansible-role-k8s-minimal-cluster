freehck.k8s_minimal_cluster
=========

Install kubernetes cluster (minimal working)

Description
-----------

This role installs kubernetes cluster. Full automation: installs all the binaries, initializes cluster, join nodes to cluster, installs CNI.

This role is a dummy one, and it uses other simple roles from Galaxy.

This purpose of this role is to be a minimal testing variant of `freehck.k8s`, that I use for testing application roles, so it uses the same variable prefix `k8s_`, not `k8s_minimal_cluster_`. Consider this role as a tasting approach, not something more. If you need to deploy kubernetes, please use `freehck.k8s` instead of this one.

Due to reasons above I don't provide any variables and playbook examples in this readme.

Tests
-----

This role provides you with a Vagrant-based test suite under `tests/` directory.

To get a fully operational Kubernetes cluster, type following command in terminal:

    cd tests && make

Install
-------

This role can be installed from [Ansible Galaxy](https://galaxy.ansible.com/):

`ansible-galaxy install freehck.k8s_minimal_cluster`

License
-------

MIT

Author Information
------------------

Dmitrii Kashin, <freehck@freehck.ru>
