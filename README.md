ansible-playbook -i inventory web-db.yaml 

### Out put
ansible-playbook -i inventory web-db.yaml -v

### $ log file at /var/log/ansible.log is not writeable and we cannot create it, aborting
sudo touch /var/log/ansible.log
ubuntu@ip-172-31-32-78:~/profile/ex7$ sudo chown ubuntu /var/log/ansible.log

### Group and Host name
Host name
mkdir host_vars
vim [name host as web02]
USER: user form file web02

Grop
mkdir group_vars
vim [name Group as webservers]
USER: user form file webservers
├── README.md
├── ansible.cfg
├── clientkey.pem
├── group_vars
│   ├── all
│   └── webservers
├── host_vars
│   └── web02
├── inventory
└── vars_precedence.yaml
https://docs.ansible.com/ansible/latest/playbook_guide/playbooks_variables.html
