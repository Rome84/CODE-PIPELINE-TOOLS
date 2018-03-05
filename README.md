# CODE-PIPELINE-TOOLS
# BUILDING-A-CI/CD-PIPELINE
        VAGRANT=====================================>
        ANSIBLE/CHEF================================> Configuration Management Tools
        TERRAFORM/CLOUDFORMATION===============>  Repplication or instantiation tools.
        CENTOS/REDHAT/UBUNTU=====================>   Operating Systems
        CLOUD-PROVIDER: ============================>AWS and Resources
        GITHUB======================================> Source Version Control
        JENKINS=====================================> CI/CD; Handle Automation and Plugins
        TOMCAT====================================>    Serlvet Container
        MAVEN=======================================>Continous Building
        DOCKER======================================>Containerization
        NEXUS/ARTIFACTORY==========================>  Repositories and Binairies
        SONARQUBE==================================> Code Inspection
        SELENIUM===================================>  Code Testing
        ELASTICSEARCH/SPLUNK=======================> Centralized Log Management Tools
        NAGIOS/NEW-RELIC===========================>  Infrastructure Monitoring Tools
        CDN:========================================>  Akami/Cloud-Front
        SCRIPTING:==================================>  Python, Bash.
        WEB-ARCHITECTURE: =========================>  LAMP Stack, HTTPD, Tomcat.      
        MySQ/MARIADB==============================>   DataBase  
        PROJECT MANAGEMENT TOOL==================> Jira, Confluence,Slack/Hipchat
        NETWORK-SECURITY:==========================> netcat, tcpdump, Wireshark, OSSEC

**********************************************************************************************************************
# Plan and Code
# Build and Test
# Release and Deploy
# Operate and Monitor
**************************************************************************************************************************
# How do all these tools work together?
#                 GIT
1- Developers develop the code and this source code is managed by Version Control System tools like Git etc.
2- Developers send this code to the Git repository and any changes made in the code is committed to this Repository.
#                JENKINS AND MAVEN
3- Jenkins pulls this code from the repository using the Git plugin and build it using tools like Ant or Maven.
#                 ANSIBLE/CHEF/PUPPET
4- Configuration management tools like Ansible/Chef/puppet etc.. deploys & provisions testing environment.
#                 MAVEN AND SELENIUM
5- Jenkins releases this code on the test environment on which testing is done using tools like selenium.
#                 ANSIBLE/CHEF/PUPPET
5- Once the code is tested, Jenkins send it for deployment on the production server (even production server is provisioned & maintained by tools like Ansible/Chef/puppet).
#                 MONITORING
6. After deployment It is continuously monitored by tools like Nagios etc...
#                 DOCKER
7. Docker containers provides testing environment to test the build features.


# WHAT EACH TOOL DOES
# Ansible
Ansible is an automation engine that enables IT admins to automate parts of their daily tasks. Enterprises that use Ansible stand to benefit from increased accountability and compliance in their IT environments as well as innovation and collaboration among their employees. Organizations can also take their Ansible deployment one step further with Tower, which adds control, security and other capabilities that enterprises can monitor with a UI and RESTful API.

# Docker
An infrastructure-neutral platform, Docker integrates into any environment and provides full stack portability for apps. The framework comes with certified containers that enterprises can use to build secure, safer applications. Organizations may choose the Enterprise Edition, which streamlines app development and production across locations running Windows and Linux.


# Chef
Chef is a platform designed to help organizations manage their infrastructure. The Chef Server stores an enterprise’s “cookbooks,” or repositories which houses information about the desired state of a customer’s infrastructure, as well as details pertaining to every “node,” or network machine on which the Chef client runs and obtains configuration information. Chef helps organizations manage all their on-premises and cloud environments as well as accelerates the process of enterprises adopting the cloud.

# GIT
As a version control system (VCS) tool, Git helps developers manage their projects with speed and efficiency. It’s free and open-source, which means anyone can use it. One of its signature features is a branching model that allows developers to create multiple local branches, or pointers to a commit, that are independent of one another. Developers can then merge, create, or delete these branches as their infrastructure evolves.

# Jenkins
Jenkins is another automation server that supports developers as they build, deploy and automate their projects. Users can employ Jenkins as a continuous integration (CI) server or leverage it for continuous delivery (CD). Easy to install and configure, the platform is customizable with nearly every type of CI and CD utility via plugins. Jenkins also allows users to distribute their work across multiple machines.

# JIRA
The focus of JIRA is to streamline the collaborative efforts of software teams. Teams can use the tool to distribute tasks to each and every member. They can then leverage JIRA’s real-time, visual data to track their goals and improve their overall performance. Additionally, JIRA provides software teams with an out-of-the-box solution for shipping out software as well as the opportunity to create their own custom workflows.

# New Relic
More than 15,000 customers use New Relic to innovate with visibility across their infrastructure. A comprehensive tool for data organization, visualization, and evaluation, New Relic enables developers to build apps for any language in any environment. Dashboards track those applications and help deliver insights into how enterprises can optimize their technology.

# Nagios (& Icinga) 
nagios Infrastructure monitoring is a field that has so many solutions… from Zabbix to Nagios to dozens of other open-source tools. Despite the fact that there are now much newer kids on the block, Nagios is a veteran monitoring solution that is highly effective because of the large community of contributors who create plugins for the tool. Nagios does not include all the abilities that we had wanted around the automatic discovery of new instances and services, so we had to work around these issues with the community’s plugins. Fortunately, it wasn’t too hard, and Nagios works great.

