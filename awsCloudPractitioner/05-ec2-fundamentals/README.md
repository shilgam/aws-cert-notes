# ec2 notes

## EC2 Instance Types Basics

- ec2 instance types: https://aws.amazon.com/ec2/instance-types/
- To compare all ec2 instances together: https://instances.vantage.sh

## Intro to Security Groups

Classic ports to know

- 22 = ssh
- 21 = ftp
- 22 = sftp (using ssh)
- 80 = http
- 443 = https
- 3389 = rdp (remote desctop protocol) - for Windows

## SSH using Mac/Linux:

- To protect private key file: `chmod 0400 path/to/your/ssh-key.pem`
- To SSH to your instance: `ssh -i path/to/your/ssh-key.pem ec2-user@{public_IPv4_address}`

## EC2 Instances Purchasing Options (pdf p.80)

TODO: repeat lecture

Lesson: https://www.udemy.com/course/aws-certified-cloud-practitioner-new/learn/lecture/20055756

1. Dedicated Host
    -
1. Dedicated Instance


1. On-Demand Instances – short workload, predictable pricing, pay by second
1. Reserved (1 & 3 years)
    - Reserved Instances – long workloads
    - Convertible Reserved Instances – long workloads with flexible instances
        - NOTE: "flexible instances" - means you can change instance type, etc.
    - Sch eduled Instances
1. Savings Plans (1 & 3 years) – commitment to an amount of usage, long workload
1. Spot Instances – short workloads, cheap, can lose instances
1. Dedicated Hosts – book an entire physical server
1. Dedicated Instances – no other customers will share your hardware
    - i.e. no other AWS Account will run an instance on the same Host
1. Capacity Reservations – reserve capacity in a specific Availability Zone for any duration
