container-security-awesome [![Awesome](https://cdn.rawgit.com/sindresorhus/awesome/d7305f38d29fed78fa85652e3a63e154dd8e8829/media/badge.svg)](https://github.com/sindresorhus/awesome)[![Travis](https://api.travis-ci.org/kai5263499/container-security-awesome.svg?branch=master)](https://travis-ci.org/kai5263499/container-security-awesome)

------------------------------------------------------------------------------------------

A collection of container related security resources

* [**Image**](#image)

* [**Networking**](#networking)

* [**Security profiles**](#security-profiles)

* [**Exploits**](#exploits)

* [**Presentations**](#presentations)

------------------------------------------------------------------------------------------

## Image

------------------------------------------------------------------------------------------
### [Understanding and Hardening Linux Containers](https://www.nccgroup.trust/us/about-us/newsroom-and-events/blog/2016/april/understanding-and-hardening-linux-containers/)
* The "War and Peace" of container security

### [Security Assurance Requirements for Linux Application Container Deployments](http://nvlpubs.nist.gov/nistpubs/ir/2017/NIST.IR.8176.pdf)
* Department of commerce guidance on container security

### [CoreOS Clair](https://coreos.com/blog/vulnerability-analysis-for-containers.html)
* Utility from CoreOS for automated vulnerability analysis for containers
* [Clair: The Container Image Security Analyzer (by Joey Schorr & Quentin Machu)](https://www.youtube.com/watch?v=Kri67PtPv6s) - Presentation about the Clair platform
* [A more polished presentation of Clair at CoreOS Fest 2016](https://www.youtube.com/watch?v=YDCa51BK2q0)

### [OpenSCAP Container Compliance](https://github.com/OpenSCAP/container-compliance)
* Utility for aiding in compliance checks against a container

### [Actuary](https://github.com/diogomonica/actuary)
* Automated security profiling for Docker image
* [drydock](https://github.com/zuBux/drydock) - Inspired by docker-bench-security with the ability to apply custom security profiles
* [Docker bench security](https://github.com/diogomonica/docker-bench-security) - One of the first security linting utility for Docker

### [Buildah](https://github.com/projectatomic/buildah)
* Docker image building framework

### [Packer](https://www.packer.io/docs/builders/docker.html)
* Packer builds Docker containers without the use of Dockerfiles. By not using Dockerfiles, Packer is able to provision containers with portable scripts or configuration management systems that are not tied to Docker in any way. It also has a simple mental model: you provision containers much the same way you provision a normal virtualized or dedicated server.

### [LinuxKit](https://github.com/linuxkit/linuxkit)
* A toolkit for building custom minimal, immutable Linux distributions

### [Grafeas](https://github.com/Grafeas/Grafeas)
* An open-source API to audit and govern your software supply chain

### Commercial vulnerability scanners
* [Black Duck Software](https://www.blackducksoftware.com/)
* [Docker Cloud](https://cloud.docker.com)
* [Tenable](https://www.tenable.com/products/tenable-io/container-security)
* [GrSecurity](https://grsecurity.net/features.php) - A collection of image hardening tools

------------------------------------------------------------------------------------------

## Networking

------------------------------------------------------------------------------------------
### [Cilium](https://github.com/cilium/cilium)
* Network policy enforcement based on eBPF
* [Cilium - Container Security and Networking Using BPF and XDP - Thomas Graf, Covalent](https://www.youtube.com/watch?v=CcGtDMm1SJA) - Presentation of Cilium by its creator

### [Linux Monitoring at Scale with eBPF (Brendan Gregg & Alex Maestretti)](https://www.youtube.com/watch?v=44nV6Mj11uw)
* bSides SF 2017 talk about container monitoring at Netflix using eBPF

### [Calico](https://www.projectcalico.org/)
* Security enforcement for [Flannel](https://github.com/coreos/flannel) SDN

### [Kube2IAM](https://github.com/jtblin/kube2iam)
* Apply Amazon Identity Management roles to Kubernetes Pods

### [Trieme](https://www.aporeto.com/trireme/)
* SDN application segmentation

### [Envoy](https://envoyproxy.github.io/)
* Sidecar and security enforcement system used at Lyft

### [Scope](https://github.com/weaveworks/scope)
* Realtime metrics gathering across the cluster

### [Segment Routing in Container Networks](http://work.delaat.net/rp/2016-2017/p95/report.pdf)
* Research paper on a practical implementation of segment routing in a container cluster

### Commercial solutions
* [StakRox](https://www.stackrox.com/product/) - Container security solution with adaptive threat protection
* [Netsil](https://netsil.com/) - Operations dashboard for Kubernetes

------------------------------------------------------------------------------------------

## Security profiles

------------------------------------------------------------------------------------------

### [bane](https://github.com/jessfraz/bane)
* AppAromor profile generator for Docker containers

### [SELinux for Mere Mortals](https://www.youtube.com/watch?v=cNoVgDqqJmM)
* A gentle introduction to Security Enhanced Linux

### [SELinux is no Longer an Option](https://www.youtube.com/watch?v=dtclmj3H7ZU)

### [Firejail](https://github.com/netblue30/firejail)
* Linux namespaces and seccomp-bpf sandbox. Also works with GUI apps

### [Docker SELinux Capabilities reference](https://docs.docker.com/engine/reference/run/#runtime-privilege-and-linux-capabilities)
* A handy list of capabilities that are enabled by default in Docker

### [Detailed post about SELinux Capabilities](https://forums.grsecurity.net/viewtopic.php?f=7&t=2522)
* An SELinux deep dive

------------------------------------------------------------------------------------------

## Exploits

------------------------------------------------------------------------------------------

### [nsenter](https://coderwall.com/p/xwbraq/attach-to-your-docker-containers-with-ease-using-nsenter)
* This isn't an exploit but it allows user to access the host VM if run in privileged mode

### [Dirty COW](https://dirtycow.ninja/)
* CVE-2016-5195
* Privilege escalation vulnerability in Linux kernel
* [Proof of concepts](https://github.com/dirtycow/dirtycow.github.io/wiki/PoCs)
* [Dirty COW and why lying is bad even if you are the Linux kernel](https://chao-tic.github.io/blog/2017/05/24/dirty-cow)

### [Docker CVE List](https://www.cvedetails.com/vulnerability-list/vendor_id-13534/product_id-28125/Docker-Docker.html)
* List of known security vulnerabilities for Docker

------------------------------------------------------------------------------------------

## Presentations

------------------------------------------------------------------------------------------
### [Container security as explained by the three pigs](https://www.youtube.com/watch?v=giFKMsIH4b0)
### [Introduction to Container Security](https://www.youtube.com/watch?v=ABFmXCGJlo8)
### [GoDaddy's Production Kubernetes Story & Moving Target Defense in Container Envs](https://www.youtube.com/watch?v=2nisq0stz-s)
### [Container Security Round Table](https://www.youtube.com/watch?v=eY0wIj7lsEw)
### [Secure Substrate: Least Privilege Container Deployment](https://www.youtube.com/watch?v=iHQCVFMBdCA)
### [A Docker Image Walks Into a Notary](https://www.youtube.com/watch?v=JvjdfQC8jxM)
### [How Secure Are Your Docker Images?](https://www.youtube.com/watch?v=dzm-8hp8MQo)
### [Docker Security Deep Dive - Docker Track](https://www.youtube.com/watch?v=tL4IYSKu7ZU)
* Securing the image pipeline from creation to delivery
### [Scaling Application Defense with Intent Based Security - Michael Withrow (Twistlock)](https://www.youtube.com/watch?v=970keZ7VfCg)
* A security model to match the deployment model of many orchestration utilities
### [Container Performance Analysis](https://www.youtube.com/watch?v=bK9A5ODIgac)
* Container performance analysis at Netflix. This contains similar material as the bSides talk listed above with
* [Evolution of Container Usage at Netflix](https://medium.com/netflix-techblog/the-evolution-of-container-usage-at-netflix-3abfc096781b) - Also provides insight into container monitoring, logging, and security at Netflix.
### [Docker Networking in Production at Visa](https://www.youtube.com/watch?v=k3SeQPt0f0o)
* Chief Systems Architect Sasi Kannappan describes how Docker is used at Visa
## [The Golden Ticket- Docker and High Security Microservices - Black Belt Track](https://www.youtube.com/watch?v=346WmxQ5xtk)
