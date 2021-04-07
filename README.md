# ansible-aws-kubernetes

In this repo there are two Ansible roles:
###1. K8sMaster(for configuring K8s Master on the AWS)
###2. K8sSlaves(for configuring K8s SLaves on the AWS)

There are files:
###daemon.json
###k8s.conf
daemon.json file is used to set the driver of Docker Engine as systemd
k8s.conf file set the iptables for the configuration of the K8s Cluster

There's a playbook ###ec2.yml which is used to launch EC2 instances over the AWS
###secure.yml has the access key and secret key of the AWS IAM user which is used in the launching of EC2 instances

###K8sCluster.yml file is used for executing both the roles
