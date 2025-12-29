# 3Tier-Architecture-On-Azure

📘 3-Tier Architecture on Azure:
This project demonstrates the design and implementation of a 3-tier architecture using Microsoft Azure Cloud Platform, aimed at building a secure, scalable, and enterprise-grade web application environment. The architecture is structured into three distinct layers — Web Server (Presentation), Application Server (Logic), and Database Server (Data) — each deployed on separate Azure Virtual Machines to ensure isolation, security, and clarity of purpose. 


🧱 Architecture Overview:
The 3-tier model separates the application into logical and physical layers:
Web Server Tier (Frontend):
Acts as the entry point for user requests.
Hosted on an Azure Virtual Machine running Nginx to serve the front-end.
Forwards incoming traffic to the application tier. 

Application Server Tier (Business Logic):
Handles core application logic and processes requests.
Runs Apache Tomcat on an Azure VM listening on port 8080.
Communicates with the database server to fetch and update data. 

Database Tier (Data):
Stores and manages persistent application data using MySQL on an Azure VM.
Placed in a private network for enhanced security and only accessible from the application tier. 

The architecture uses Azure Virtual Networks (VNets) with subnets and Network Security Groups (NSGs) to enforce secure communication between tiers and restrict unauthorized access. 


🚀 Key Features:
Separation of Concerns: Each tier operates independently, allowing easier maintenance and scalability. 
Security Best Practices: Deployment uses private subnets and security rules to protect internal components. 
Scalable Design: Architecture follows modern cloud design patterns suitable for enterprise applications. 


📋 Prerequisites:
Before deploying this design, ensure you have:
An Azure subscription (Free or Paid).
Resource Group to organize related resources.
Virtual Networks (VNets) and Subnets for network segmentation.
Appropriate access permissions to create VMs, NSGs, and VNets in Azure. 


🛠 Deployment Steps:
Create Resource Group – Define a group to contain all project resources. 
Set Up Virtual Networks and Subnets – Configure VNets and subnets for Web, App, and DB tiers. 
Provision Virtual Machines – Deploy VMs for Web, App, and Database tiers. 
Configure NSGs – Apply rules to allow/deny access between tiers.
Install Required Software – Install Nginx on Web server, Apache Tomcat on App server, and MySQL on DB server. 
Establish Connectivity – Use network peering and security rules to ensure communication. 


🎯 Outcome:
By the end of this project, you will have a functioning 3-tier application deployed on Azure with clear separation between front-end, business logic, and data storage layers. This setup exemplifies best practices for cloud architecture including security, isolation, and maintainability.
