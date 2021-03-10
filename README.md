# k8s_cluster
Launch a k8s multi-node cluster over aws cloud
In this repository there are two ansible roles:
one for launching the instances- **awslaunch**
Here you have to provide your aws credentials, ami-id , security group, region etc in vars folder of awslaunch role.
second one launch k8s cluster in the instances - **kube_cluster**
During running the playbook kube_cluster/tests/test.yml , it will prompt for the number of slave nodes.
Automatically store the token and transfer to the worker nodes of cluster.
