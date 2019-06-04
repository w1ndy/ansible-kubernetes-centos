# ansible-kubernetes-centos
Setting up a single-master Kubernetes cluster with Ansible on CentOS [experimental]

Create the ansible host file before running these playbooks.
``/etc/ansible/hosts`` example:

```
[masters]
master.k8s.dev ansible_host=172.17.165.220

[workers]
worker1.k8s.dev ansible_host=172.17.165.221
worker2.k8s.dev ansible_host=172.17.165.222
```

These playbooks can be run with the following command:

```bash
ansible-playbook xxx.yml -bK   # becoming root is required
```
