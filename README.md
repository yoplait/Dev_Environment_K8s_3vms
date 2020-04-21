# Introduction

This is a first approach to help in the Docker and Kubernetes joourney 

##  Requirements:

## Setup:

## Steps:



1. Install Vagrant
2. Install Ansible
3. Install VirtualBox
4. Do some tests



## Usage:

Clone the directory and then run to validate:

```
vagrant validate
```
We can check what items are going to be spin and created:
```
vagrant status
```
Then we can start the platform:
```
vagrant up
```


## Accessing master
```
$ vagrant ssh k8s-master

vagrant@k8s-master:~$ kubectl get nodes
NAME         STATUS   ROLES    AGE     VERSION
k8s-master   Ready    master   18m     v1.13.3
node-1       Ready    <none>   12m     v1.13.3
node-2       Ready    <none>   6m22s   v1.13.3
```
## Accessing nodes
```
$ vagrant ssh node-1
$ vagrant ssh node-2
```

## Destroying scenario
```
$ vagrant destroy --force --parallel
```


Thanks

[Email me](perezpardojc@gmail.com)

[Tweet me](https://twitter.com/perezpardojc)

[Browse other interesting tutorials](https://github.com/yoplait)



This has been tested with vagrant 1.9.1 and VirtualBox 5.0.32. 

