Creating AWS EC2 instance using ansible roles and ansible-vault.
  
Here we are creating a new EC2 instance in AWS platform. The ansible playbooks are orchestrated in ansible role. 'aws-role' is the role name which I used here. Apart from the ansible role, I have used ansible-vault to store my aws credentilas in a better way. Ansible has a nice tool named ansible-galaxy which is used to perform various role related operations. One of these operations named ansible-galaxy init is to setup the predefined Ansible role directory structure for your Ansible projects.

* Role Structure
``` bash
.
├── ansible-aws.yml
└── aws-role
    ├── defaults
    │   └── main.yml
    ├── files
    ├── handlers
    │   └── main.yml
    ├── meta
    │   └── main.yml
    ├── README.md
    ├── tasks
    │   ├── ec2.yml
    │   └── main.yml
    ├── templates
    ├── tests
    │   ├── inventory
    │   └── test.yml
    └── vars
        ├── creds.yml
        └── main.yml

```
* ansible-aws.yml is the main playbook to execute the role called aws-role.
* tasks/main.yml is the tasks file for aws_role.
* tasks/ec2.yml is the task file for ec2.yml
* vars/creds.yml is the encrypted vault file which includes the credenmtials 
* vars/main.yml includes other variables

