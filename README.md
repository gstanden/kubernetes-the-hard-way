# Kubernetes The Hard Way

This is my fork "Kubernetes the hard way" by Kelsey Hightower. I forked this guide because what I want to do is to build an LXD-containerized automatically-deployed containerized-Kubernetes option scripted and integrated into the Orabuntu-LXC project. I realize that basically goes against Kelsey's principles that this is supposed to be for learning.  However, the goal of Orabuntu-LXC, which is a 100% shell script project, is to make container ops and related networking, namespace, and cgroup veritically-integrated systems more accessible so that the build is easy but the reverse-engineering is not, by which I mean that one of the goals of Orabuntu-LXC is to automate the building of a total container environment, but using the common denominator of readily-accessible shell script so that the user can then study the as-built system and the shell script to gain an understanding of how things actually work.  So in that sense, the containerization of Kelsey's "Kubernetes the hard way" carries on Kelsey's project mission and spirit.

Kubernetes The Hard Way is optimized for learning, which means taking the long route to ensure you understand each task required to bootstrap a Kubernetes cluster.

> The results of this tutorial should not be viewed as production ready, and may receive limited support from the community, but don't let that stop you from learning!

## Copyright

<a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/"><img alt="Creative Commons License" style="border-width:0" src="https://i.creativecommons.org/l/by-nc-sa/4.0/88x31.png" /></a><br />This work is licensed under a <a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/">Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International License</a>.


## Target Audience

The target audience for this tutorial is someone planning to support a production Kubernetes cluster and wants to understand how everything fits together.

## Cluster Details

Kubernetes The Hard Way guides you through bootstrapping a highly available Kubernetes cluster with end-to-end encryption between components and RBAC authentication.

* [kubernetes](https://github.com/kubernetes/kubernetes) v1.21.0
* [containerd](https://github.com/containerd/containerd) v1.4.4
* [coredns](https://github.com/coredns/coredns) v1.8.3
* [cni](https://github.com/containernetworking/cni) v0.9.1  (hoping to try out Project Antrea alternative to cni successfully with this)
* [etcd](https://github.com/etcd-io/etcd) v3.4.15

## Labs

This tutorial makes no assumption about your platform for running Kubernetes, because this will be an LXD-containerized Kubernetes.  It does require adequate memory, CPU, and network resources.  More about that as I work through my rendition of "Kubernetes the hard way."

* [Prerequisites](docs/01-prerequisites.md)
* [Installing the Client Tools](docs/02-client-tools.md)
* [Provisioning Compute Resources](docs/03-compute-resources.md)
* [Provisioning the CA and Generating TLS Certificates](docs/04-certificate-authority.md)
* [Generating Kubernetes Configuration Files for Authentication](docs/05-kubernetes-configuration-files.md)
* [Generating the Data Encryption Config and Key](docs/06-data-encryption-keys.md)
* [Bootstrapping the etcd Cluster](docs/07-bootstrapping-etcd.md)
* [Bootstrapping the Kubernetes Control Plane](docs/08-bootstrapping-kubernetes-controllers.md)
* [Bootstrapping the Kubernetes Worker Nodes](docs/09-bootstrapping-kubernetes-workers.md)
* [Configuring kubectl for Remote Access](docs/10-configuring-kubectl.md)
* [Provisioning Pod Network Routes](docs/11-pod-network-routes.md)
* [Deploying the DNS Cluster Add-on](docs/12-dns-addon.md)
* [Smoke Test](docs/13-smoke-test.md)
* [Cleaning Up](docs/14-cleanup.md)
