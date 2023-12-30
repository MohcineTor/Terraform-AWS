# Terraform-AWS

## Setting Up a Simple AWS Infrastructure with Terraform

### Objectives:

The main objectives of this tutorial are to:

1. **Configure the AWS Provider:**
   - Set up the AWS provider with a specified region (us-east-1 in this case).

2. **Create a VPC:**
   - Establish a Virtual Private Cloud (VPC) with a defined CIDR block and a name tag.

3. **Create an Internet Gateway:**
   - Generate an internet gateway associated with the VPC created in step 2.

4. **Create a Custom Route Table:**
   - Set up a route table with routes for both IPv4 and IPv6 traffic, associating it with the VPC.

5. **Create a Subnet:**
   - Establish a subnet within the VPC with a specified CIDR block and availability zone.

6. **Associate Subnet with Route Table:**
   - Link the subnet created in step 5 with the custom route table.

7. **Create a Security Group:**
   - Define a security group allowing inbound traffic on ports 22 (SSH), 80 (HTTP), and 443 (HTTPS), and all outbound traffic.

8. **Create a Network Interface:**
   - Generate a network interface within the subnet, assigning a private IP and associating it with the security group.

9. **Assign an Elastic IP:**
   - Allocate an Elastic IP to the network interface created in step 7.

10. **Create Ubuntu Web Server:**
    - Launch an AWS instance with Ubuntu, using the specified AMI, instance type, key name, and user data to install and enable Apache2.
