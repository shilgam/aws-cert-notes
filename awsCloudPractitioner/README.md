# Code snippets

- Link with code snippets: https://courses.datacumulus.com/downloads/certified-cloud-practitioner-zb2/
- version: code_v2022-12-16


## Section 6 - EC2 Instance Storage

### EBS Volume (Elastic Block Store Volume)

- **EBS volume** is network attached drive which results in slow performance but data is persistent meaning even if you reboot the instance data will be there.

Pros:
- data is persistent (even if you reboot the instance data will be there)
- Can use EBS Snapshots for backups or transfering volume across Availability Zones

Cons:
- Can be mounted to only 1 EC2 instance at a time
- Mapped to specific Availability Zone

### AMI (Amazon Machine Image)

Why? To customise EC2 instance + faster boot

Types:
- Public AMI (AWS provided)
- your own AMI
- from AWS Marketplace AMI

### EC2 Image Builder

Allows to build, test and test AMIs

### EC2 Instance Store (Ephemeral storage)

- **EC2 Instance Store**

This storage is located on disks that are physically attached to the host computer.

Pros:
- high I/O performance

Cons:
- lost if our instance is stoped or terminated

### EFS (Elastic File System) - network file system

Pros:
- can be mounted to 100s of EC2 instances simultaneously
- can be mounted to EC2 instances in multiple availability zones


Cons:
- works only for Linux EC2 instances
- highly expensive
    - but **EFS-IA** (EFS Infrequent Access) can be used for cost optimisation



### Amazon FSx

Why?
- To launch 3rd party high-performance file systems on AWS

Offerings:

1. FSx for Windows File Server

1. FSx for Lustre
    - storage fo High Performance Computing
    - the name "Lustre" = "Linux" + "cluster"

1. FSx for NetApp ONTAP
