Ansible stuff

To test the ansible playbook before running

'''
ansible-playbook --syntax-check webservers.yml
ansible-lint webservers.yml
yamllint webservers.yml
ansible-inventory --host testserver -i inventory/vagrant.ini
'''

If you want to validate vagrant file

'''
vagrant validate
'''
