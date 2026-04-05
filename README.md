# Configuring Inbound Firewall Rules in AWS EC2 Security Groups

## Objective

Configured inbound firewall rules on an AWS EC2 security group to allow specific types of network traffic to reach the instance. The project focused on understanding port-based access control, protocol types, and how AWS security groups act as virtual firewalls. This is a core cloud networking skill for securing and exposing services appropriately.

### Skills Learned

- Configuring AWS EC2 security group inbound rules
- Understanding TCP ports and their common service associations
- Differentiating between HTTP, HTTPS, SSH, and custom traffic types
- Managing source IP ranges (0.0.0.0/0 for open access)
- Cloud network security fundamentals

### Tools Used

- AWS EC2 Console
- AWS Security Groups
- AWS VPC

## Steps
1. Navigated to EC2 in the AWS Console and selected Security Groups
2. Opened the launch-wizard-2 security group
3. Selected the Inbound rules tab and clicked Edit inbound rules
4. Added the following four rules:
   1. HTTPS (TCP, port 443) from 0.0.0.0/0
   2. HTTP (TCP, port 80) from 0.0.0.0/0
   3. SSH (TCP, port 22) from 0.0.0.0/0
   4. Custom TCP (port 8080) from 0.0.0.0/0
5. Saved the rules, bringing the total inbound rule count to 4
