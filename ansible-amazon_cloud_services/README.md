Creating AWS EC2 instance using ansible roles and ansible-vault.
  
Here we are creating a new EC2 instance in AWS platform.The ansible playbooks are orchestrated in ansible role.'aws-role' is the role name which I used here. Apart from the ansible role, I have used ansible-vault to store my aws credentilas in a better way.

* Structre of the role

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






