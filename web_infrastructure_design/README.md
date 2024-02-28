Web Infrastructure Design Project
Overview
This project focuses on designing web infrastructures, covering various concepts such as network basics, servers, web servers, DNS, load balancers, and monitoring. The project is structured into tasks, each requiring the design of a specific web infrastructure.

Concepts
Before starting the tasks, make sure to familiarize yourself with the following concepts:

Network basics
Server
Web Server
DNS
Load balancer
Monitoring
What is a database
What’s the difference between a web server and an app server?
DNS record types
Single point of failure
How to avoid downtime when deploying new code
High availability cluster (active-active/active-passive)
What is HTTPS
What is a firewall
Learning Objectives
By the end of this project, you should be able to:

Draw a diagram covering the web stack built in sysadmin/devops track projects.
Explain the role of each component in the infrastructure.
Understand system redundancy.
Know acronyms such as LAMP, SPOF, QPS.
Requirements
General
A README.md file at the root of the project folder is mandatory.
For each task, take a picture/screenshot of your diagram after whiteboarding.
Manual QA review must be done for the project.
Upload screenshots to an image hosting service and insert links in the answer file.
Whiteboard each task in front of a mentor, staff, or student without computer or notes during the session.
Tasks
Task 0: Simple Web Stack
Design a one-server web infrastructure for the website reachable via www.foobar.com. The infrastructure should include:

1 server
1 web server (Nginx)
1 application server
1 application files (your code base)
1 database (MySQL)
1 domain name foobar.com configured with a www record pointing to your server IP (8.8.8.8).
Issues:

Single point of failure (SPOF)
Downtime during maintenance
Limited scalability
Task 1: Distributed Web Infrastructure
Design a three-server web infrastructure for www.foobar.com. Additional components include:

2 servers
1 load balancer (HAproxy)
Explain distribution algorithm in the load balancer
Explain Active-Active or Active-Passive setup for load balancer
1 Primary-Replica (Master-Slave) cluster for the database
Issues:

Single points of failure
Security issues (no firewall, no HTTPS)
Lack of monitoring
Task 2: Secured and Monitored Web Infrastructure
Design a three-server web infrastructure for www.foobar.com, ensuring security, encrypted traffic, and monitoring. Add:

3 firewalls
1 SSL certificate for HTTPS
3 monitoring clients
Explain the purpose of each additional element
Issues:

SSL termination at the load balancer level
Single MySQL server accepting writes
Uniformity in server components may lead to problems
Task 3: Scale Up
Add components to scale up the infrastructure. Include:

1 server
1 load balancer (HAproxy) configured as a cluster with the existing one
Separate components (web server, application server, database) onto their own servers
Issues:

Explain the purpose of each additional element
Repository Information
GitHub Repository: holbertonschool-system_engineering-devops
Directory: web_infrastructure_design
Files:
0-simple_web_stack
1-distributed_web_infrastructure
2-secured_and_monitored_web_infrastructure
3-scale_up
Note: Replace "#" with actual links and details.