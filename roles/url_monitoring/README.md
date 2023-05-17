# Ansible-URL-Monitor

URL monitoring Bot is basically fetching the staus of  multiple URLs i.e if it is Active/Inactive.

* Ansible Automation Bot solution implemented, Bot will Monitors all the URLs and as output send two email notification to user groups:

 	    	1. Consolidated reports of all Urls stating Active and Inactive state 
 	    	2. Explicit notification to users of all Urls in Inactive state. 

* This activity which was performed once a day will now can performed multiple time, as per desired frequency through Ansible Automation Bot.

### Requirements
* OS Supported: Windows(WSL)/Linux
* Ansible Engine or Ansible Tower/AAP

### Role Variables
* Update the required variables:

![image](https://media.github.ibm.com/user/334631/files/9e3b2700-18d9-11ed-98c5-224e844cbd18)

### Dependencies
* Ansible core modules required which is present while installing ansible engine.
* Also this role needs to be ran with "become: yes" option. Sudo privileges are required

### Run instruction

* Update the URLs to be monitored in **.csv** format and place it under the the directory structure
 **Example**
![image](https://media.github.ibm.com/user/334631/files/fa06af80-18db-11ed-8e4a-bbe227677424)

* Update the required variables as mentioned under Roles Variable
* Run role [main.yml](https://github.ibm.com/ECA-Ansible-Assets/Ansible-URL-Monitor/blob/2a8eecd1e65e78a53337a6e54fd4643d23a3ced7/main.yml) 
* Run the below command if using Ansible Engine:
                  `ansible-playbook main.yml`

### Author Information
samparna_sona@in.ibm.com
