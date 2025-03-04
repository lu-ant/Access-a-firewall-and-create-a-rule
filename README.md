# Access-a-firewall-and-create-a-rule
Overview
This project demonstrates how to access and configure firewall rules within Google Cloud's Virtual Private Cloud (VPC). Proper firewall management is essential for securing cloud resources by controlling incoming and outgoing traffic based on specified rules.

Prerequisites
Before proceeding, ensure you have:

Google Cloud Project: An active project with billing enabled.
Permissions: Roles such as roles/compute.securityAdmin or roles/compute.networkAdmin assigned to your user account.
Google Cloud SDK: Installed and configured on your local machine.
Steps to Access and Create a Firewall Rule
Access the Firewall Rules:

Navigate to the Google Cloud Console.
Select your project from the project selector.
In the left-hand navigation menu, go to VPC network > Firewall rules.
Create a New Firewall Rule:

Click on Create firewall rule.
Fill in the following details:
Name: A unique identifier for the firewall rule.
Network: Select the VPC network where the rule will be applied.
Priority: Assign a priority value (lower numbers indicate higher priority).
Direction of Traffic: Choose Ingress for incoming traffic or Egress for outgoing traffic.
Action on Match: Select Allow or Deny based on the desired outcome.
Targets: Specify the instances to which this rule applies, either by All instances in the network or Specified target tags.
Source Filter: Define the source of the traffic:
IP ranges: Specify IP ranges in CIDR format (e.g., 0.0.0.0/0 for all IPs).
Protocols and Ports: Select the protocols (e.g., TCP, UDP, ICMP) and specify the ports (e.g., tcp:80 for HTTP).
Finalize and Create the Rule:

Review all configurations to ensure accuracy.
Click Create to apply the firewall rule.
