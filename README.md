# Dell-Customer-Ansible
This is a customer ansible playbook for onboarding new poweredge servers utilizing OME and iDRAC.
This is to provide customers with a good place to learn and utilize our systemen management tools with OME.

Dell OpenManage Ansible Modules allows data center and IT administrators to use RedHat Ansible to automate and orchestrate the configuration, deployment, and update of Dell EMC PowerEdge Servers and modular infrastructure by leveraging the management automation capabilities in-built into the Integrated Dell Remote Access Controller (iDRAC), OpenManage Enterprise (OME) and OpenManage Enterprise Modular (OMEM).

OpenManage Ansible Modules simplifies and automates provisioning, deployment, and updates of PowerEdge servers and modular infrastructure. It allows system administrators and software developers to introduce the physical infrastructure provisioning into their software provisioning stack, integrate with existing DevOps pipelines and manage their infrastructure using version-controlled playbooks, server configuration profiles, and templates in line with the Infrastructure-as-Code (IaC) principles.

## Supported Platforms
  * iDRAC7 based Dell PowerEdge Servers with firmware versions 2.63.60.62 and above.
  * iDRAC8 based Dell PowerEdge Servers with firmware versions 2.82.82.82 and above.
  * iDRAC9 based Dell PowerEdge Servers with firmware versions 5.10.10.00 and above.
  * Dell OpenManage Enterprise versions 3.8.3 and above.
  * Dell OpenManage Enterprise Modular versions 1.40.10 and above.

## Prerequisites
  * [Ansible >= 2.13.2](https://github.com/ansible/ansible)
  * Python >= 3.9.6
  * To run the iDRAC modules, install OpenManage Python Software Development Kit (OMSDK) 
  using either ```pip install omsdk --upgrade``` or ```pip install -r requirements.txt```. 
  OMSDK can also be installed from [Dell EMC OpenManage Python SDK](https://github.com/dell/omsdk)
  * Operating System
    * Red Hat Enterprise Linux (RHEL) 8.6 and 9.0
    * SUSE Linux Enterprise Server (SLES) 15 SP3 and 15 SP4
    * Ubuntu 22.04 and 20.04.04

## Installation

* From [galaxy](https://galaxy.ansible.com/dellemc/openmanage):  
```ansible-galaxy collection install dellemc.openmanage```

    - For offline installation on the Ansible control machine, download the required tar archive version of the collection from [Dell OpenManage collection](https://galaxy.ansible.com/dellemc/openmanage) and run the command given below:  
      ```ansible-galaxy collection install dellemc-openmanage-<version>.tar.gz```

* From [github](https://github.com/dell/dellemc-openmanage-ansible-modules/tree/collections):  
Install the collection from the github repository using the latest commit on the branch 'collections'  
```ansible-galaxy collection install git+https://github.com/dell/dellemc-openmanage-ansible-modules.git,collections```

## About
Dell OpenManage Ansible Modules is 100% open source and community-driven. All components are available under [GPL-3.0 license](https://www.gnu.org/licenses/gpl-3.0.html) on GitHub.

## Sources
https://github.com/dell/dellemc-openmanage-ansible-modules
