awesome-container-security [![Awesome](https://cdn.rawgit.com/sindresorhus/awesome/d7305f38d29fed78fa85652e3a63e154dd8e8829/media/badge.svg)](https://github.com/sindresorhus/awesome)[![Travis](https://api.travis-ci.org/kai5263499/awesome-container-security.svg?branch=master)](https://travis-ci.org/kai5263499/awesome-container-security)

------------------------------------------------------------------------------------------

A collection of container related security resources

* [**Image**](#image)

* [**Build Management**](#build-management)

* [**Networking/Runtime**](#networking/runtime)

* [**Security profiles**](#security-profiles)

* [**Exploits**](#exploits)

* [**Honeypots**](#honeypots)

* [**Presentations/Posts**](#presentations/posts)

------------------------------------------------------------------------------------------

## Image

------------------------------------------------------------------------------------------
### [Deepfence Runtime Threat Mapper](https://github.com/deepfence/ThreatMapper)
* Identify vulnerabilities in running containers, images, hosts and repositories

### [Dagda](https://github.com/eliasgranderubio/dagda/)
* Static image analysis tool

### [Port Authority Open Source Security Scanner for Docker](https://www.linkedin.com/pulse/port-authority-open-source-security-scanner-docker-srinivasan/)
* [Getting started guide](https://tech.target.com/open%20source/2018/06/07/port-authority-open-source-buzz.html)
* [Source](https://github.com/target/portauthority)
### [Understanding and Hardening Linux Containers](https://www.nccgroup.trust/us/about-us/newsroom-and-events/blog/2016/april/understanding-and-hardening-linux-containers/)
* The "War and Peace" of container security

### [Security Assurance Requirements for Linux Application Container Deployments](https://nvlpubs.nist.gov/nistpubs/ir/2017/NIST.IR.8176.pdf)
* Department of commerce guidance on container security

### [Dramatically Reducing Software Vulnerabilities](https://nvlpubs.nist.gov/nistpubs/ir/2016/NIST.IR.8151.pdf)
* NIST guidance on reducing software vulnerabilities
* [NIST security content automation protocol](https://csrc.nist.gov/projects/security-content-automation-protocol)
* [Extensible Configuration Checklist Description Format (XCCDF)](https://csrc.nist.gov/projects/security-content-automation-protocol/specifications/xccdf/) - Goes along with the SCAP link above for specifying a security template that containers should conform to

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

### [Buildah](https://github.com/containers/buildah)
* [Introduction](http://www.projectatomic.io/blog/2017/06/introducing-buildah/)
* Docker image building framework

### [Packer](https://www.packer.io/docs/builders/docker.html)
* Packer builds Docker containers without the use of Dockerfiles. By not using Dockerfiles, Packer is able to provision containers with portable scripts or configuration management systems that are not tied to Docker in any way. It also has a simple mental model: you provision containers much the same way you provision a normal virtualized or dedicated server.

### [LinuxKit](https://github.com/linuxkit/linuxkit)
* A toolkit for building custom minimal, immutable Linux distributions

### [Grafeas](https://github.com/Grafeas/Grafeas)
* An open-source API to audit and govern your software supply chain

### [Atomic Reactor](https://github.com/containerbuildsystem/atomic-reactor)
* Python library that extends docker build. It's part of the RedHat Atomic project so its rather opinionated

### [Containers Internals Lab](https://github.com/fatherlinux/container-internals-lab)
* A series of exercises that provide a deep dive into the internals of containers. Also has a good SELinux training component

### [Anchore](https://anchore.com/enterprise/)
* Free image scanning service with a commercial offering similar to Docker Cloud
* [anchore-cli](https://github.com/anchore/anchore-cli)

### [Alpine CVE Check](https://github.com/tomwillfixit/alpine-cvecheck)
* Specialized CVE scanner

### [Banyan Collector: A framework to peek inside containers](https://github.com/banyanops/collector)
* Framework for peering inside docker images. Useful for rolling your own image scanning system

### Commercial solutions
* [Black Duck Software](https://www.blackducksoftware.com/)
* [Tenable](https://www.tenable.com/products/tenable-io/container-security) - Includes [FlawCheck](https://www.theregister.co.uk/2016/10/26/tenable_ate_flawcheck_for_devops_enhancement/)
* [GrSecurity](https://grsecurity.net/features) - A collection of image hardening tools
* [Aqua](https://www.aquasec.com/) - Full lifecycle container security management platform

------------------------------------------------------------------------------------------

## Build Management

------------------------------------------------------------------------------------------

### [Habitat.sh](https://www.habitat.sh/)
* Source to deployment framework. An alternative to Kubernetes and Spinnaker. I include it here because it implements a concept of trusted images and dependency management

### Commercial solutions
* [Project Atomic](https://www.projectatomic.io/) - RedHat's complete container solution with strong built-in security
* [Docker Cloud](https://hub.docker.com) - Continuous scanning of images along with a trust mechanism

------------------------------------------------------------------------------------------

## Networking/Runtime

------------------------------------------------------------------------------------------
### [kubeadm](https://github.com/kubernetes/kubeadm)
* Associating Amazon IAM roles to pods

### [kiam](https://github.com/uswitch/kiam)
* Also for associating Amazon IAM roles to pods

### [Secure Container Isolation: Problem Statement & Solution Space](https://docs.google.com/document/d/1QQ5u1RBDLXWvC8K3pscTtTRThsOeBSts_imYEoRyw8A/edit#heading=h.ypyhxoaw8f95)
* Comprehensive guide from Google engineers on securing and isolating containers

### [gVisor](https://github.com/google/gvisor)
* User-space kernel designed to provide better isolation/sandboxing of containers

### [Cilium](https://github.com/cilium/cilium)
* Network policy enforcement based on eBPF
* [Cilium - Container Security and Networking Using BPF and XDP - Thomas Graf, Covalent](https://www.youtube.com/watch?v=CcGtDMm1SJA) - Presentation of Cilium by its creator

### [Linux Monitoring at Scale with eBPF (Brendan Gregg & Alex Maestretti)](https://www.youtube.com/watch?v=44nV6Mj11uw)
* bSides SF 2017 talk about container monitoring at Netflix using eBPF

### [Calico](https://www.projectcalico.org/)
* Security enforcement for [Flannel](https://github.com/coreos/flannel) SDN

### [Kube2IAM](https://github.com/jtblin/kube2iam)
* Apply Amazon Identity Management roles to Kubernetes Pods

### [Envoy](https://www.envoyproxy.io/)
* Sidecar and security enforcement system used at Lyft

### [Romana](https://romana.io/)
* Network policy enforcement
* [Project](https://github.com/romana/romana)

### [Scope](https://github.com/weaveworks/scope)
* Realtime metrics gathering across the cluster

### [Whispers in the Hyper-space: High-speed Covert Channel Attacks in the Cloud](https://www.youtube.com/watch?v=d2TU_Q4U9DA)
* An exploration of covert channels

### [Setting the Record Straight: containers vs. Zones vs. Jails vs. VMs](https://blog.jessfraz.com/post/containers-zones-jails-vms/)
* Contains an interesting point about how contains that share network namespaces can snoop on eachother's traffic

### [Docker Layer 2 ICC Bug](https://github.com/brthor/docker-layer2-icc)
* Containers are able to send raw ethernet frames to other containers with inter-container communication disabled

### Commercial solutions
* [StakRox](https://www.stackrox.com/) - Container security solution with adaptive threat protection
* [NeuVector](https://neuvector.com/) - Continuous network security
* [TwistLock](https://www.twistlock.com/) - Network activity profiling

------------------------------------------------------------------------------------------

## Security profiles

------------------------------------------------------------------------------------------

### [bane](https://github.com/genuinetools/bane)
* AppArmor profile generator for Docker containers

### [Container security as explained by the three pigs](https://www.youtube.com/watch?v=giFKMsIH4b0)
* [Bringing new security features to Docker](https://opensource.com/business/14/9/security-for-docker)
* [The Container Coloring Book](https://github.com/fedoradesign/coloringbook-containers/blob/master/Print-Ready/Web.pdf)

### [SELinux for Mere Mortals](https://www.youtube.com/watch?v=cNoVgDqqJmM)
* A gentle introduction to Security Enhanced Linux

### [SELinux is no Longer an Option](https://www.youtube.com/watch?v=dtclmj3H7ZU)

### [Firejail](https://github.com/netblue30/firejail)
* Linux namespaces and seccomp-bpf sandbox. Also works with GUI apps

### [Docker SELinux Capabilities reference](https://docs.docker.com/engine/reference/run/#runtime-privilege-and-linux-capabilities)
* A handy list of capabilities that are enabled by default in Docker

### [Detailed post about SELinux Capabilities](https://forums.grsecurity.net/viewtopic.php?f=7&t=2522)
* An SELinux deep dive

### [What capabilities do I really need in my container?](https://danwalsh.livejournal.com/76358.html)
* Blog post about figuring out what capabilities a container needs

### [Secure Your Containers with this One Weird Trick](https://www.redhat.com/en/blog/secure-your-containers-one-weird-trick)
* Spoiler, its using SELinux

### [Falco](https://sysdig.com/opensource/falco/)
* Open source container security monitoring
* [Technical discussion](https://sysdig.com/blog/selinux-seccomp-falco-technical-discussion/)
* [WTF, My Container Just Spawned a Shell - Jorge Salamero Sanz, Sysdig](https://www.youtube.com/watch?v=LPgjLzFcFVU)

### [Getting towards real sandbox containers](https://blog.jessfraz.com/post/getting-towards-real-sandbox-containers/)

### [Bubblewrap](https://github.com/containers/bubblewrap)

### [Subgraph](https://subgraph.com/)
* Bills itself as an adversary resistant computing platform. Under the hood the idea is to run containers in user space

### [Linux Containers in 500 Lines of Code](https://blog.lizzie.io/linux-containers-in-500-loc.html)
* An exercise that also takes you through the nitty gritty details of capabilities management

------------------------------------------------------------------------------------------

## Exploits

------------------------------------------------------------------------------------------

### [harpoon](https://github.com/ProfessionallyEvil/harpoon)
* Post exploitation framework

### [waitid](https://www.twistlock.com/labs-blog/escaping-docker-container-using-waitid-cve-2017-5123/)
* CVE-2017-5123
* Privledge escalation using the waitid syscall

### [nsenter](https://coderwall.com/p/xwbraq/attach-to-your-docker-containers-with-ease-using-nsenter)
* This isn't an exploit but it allows user to access the host VM if run in privileged mode

### [Dirty COW](https://dirtycow.ninja/)
* CVE-2016-5195
* Privilege escalation vulnerability in Linux kernel
* [Proof of concept](https://github.com/scotty-c/dirty-cow-poc)
* [Proof of concept collection](https://github.com/dirtycow/dirtycow.github.io/wiki/PoCs)
* [Dirty COW and why lying is bad even if you are the Linux kernel](https://chao-tic.github.io/blog/2017/05/24/dirty-cow)

### [Docker CVE List](https://www.cvedetails.com/vulnerability-list/vendor_id-13534/product_id-28125/Docker-Docker.html)
* List of known security vulnerabilities for Docker

### [Three Overlooked Lessons about Container Security](https://thenewstack.io/three-overlooked-lessons-container-security/)
* Outlines an interesting spear-phishing attack on image maintainers

### [Docker Scan](https://github.com/cr0hn/dockerscan)
* Image scanning system with a red-team focus of exploitation

### [Twitter Vine Source Code Dump](https://avicoder.me/2016/07/22/Twitter-Vine-Source-code-dump/)
* A case study of a vulnerable private registry

------------------------------------------------------------------------------------------

## Honeypots

------------------------------------------------------------------------------------------

### [How I capture and monitor Wordpress attacks](https://medium.com/@SecurityBender/how-i-capture-and-monitor-wordpress-attacks-ceda512b07)
* Capturing exploit attempts by emulating a Wordpress box

### [DShield](https://github.com/xme/dshield-docker)
* Docker container running cowrie with DShield output enabled

### [Dockerpot](https://www.itinsight.hu/blog/posts/2015-05-04-creating-honeypots-using-docker.html)
* Fairly old but a great idea for platform to build honeypots

------------------------------------------------------------------------------------------

## Presentations/Posts

------------------------------------------------------------------------------------------
### [Pets, cattle and insects](https://hub.packtpub.com/pets-cattle-analogy-demonstrates-how-serverless-fits-software-infrastructure-landscape/)
* An extension of the helpful cattle and pets analogy
### [Capability based sandboxing](https://archive.fosdem.org/2016/schedule/event/capsicum/)
* The author presents the intreaging notion of applying the microservices approach to containers where you divide an application apart by capabilities
* [Awesome Object Capabilities](https://github.com/dckc/awesome-ocap) - A language-level implementation of the capability based sandboxing methodology
* [Linux port of Capsicum](https://github.com/google/capsicum-linux) related to this [LWN post](https://lwn.net/Articles/604287/)
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
* [Evolution of Container Usage at Netflix](https://netflixtechblog.com/the-evolution-of-container-usage-at-netflix-3abfc096781b) - Also provides insight into container monitoring, logging, and security at Netflix.
### [Docker Networking in Production at Visa](https://www.youtube.com/watch?v=k3SeQPt0f0o)
* Chief Systems Architect Sasi Kannappan describes how Docker is used at Visa
### [The Golden Ticket- Docker and High Security Microservices - Black Belt Track](https://www.youtube.com/watch?v=346WmxQ5xtk)
### [Docker Engine Security Cheatsheet](https://github.com/konstruktoid/Docker/blob/master/Security/CheatSheet.adoc)
* Collection of resources on hardening your Docker daemon
### [Dance Madly on the Lip of a Volcano](https://www.youtube.com/watch?v=sNjylW8FV9A)
* Balancing moving fast and breaking things with securing against vulnerabilities
### [Making Security Invisible - Jessica Frazelle - JOTB17](https://www.youtube.com/watch?v=BuFTHOgsgAY)
* Great presentation on sandboxing containers
### [Vulnerability Exploitation In Docker Container Environments](https://www.youtube.com/watch?v=77-jaeUKH7c)
### [Docker Security Best Practices](https://dev.to/petermbenjamin/docker-security-best-practices-45ih)
### [Kubernetes Security Best Practices](https://dev.to/petermbenjamin/kubernetes-security-best-practices-hlk)
