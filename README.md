To use any playbook from this repo you need [Ansible](https://docs.ansible.com/ansible/latest/installation_guide/intro_installation.html#installation-guide) to be installed on your control machine.  
To automatically install Consul agent on multiple nodes through Ansible run command:
`ansible-playbook -i inventory.ini -v playbooks/consul/play.yml`.  
If you have permissions error add extra argument to run command
`ansible-playbook -e  "ansible_sudo_pass=put_pass_here" -i inventory.ini -v playbooks/consul/play.yml`.  
By default this command will install Consul on your local machine, you can specify any machines via Ansible inventory file.
