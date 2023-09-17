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

To generate the keys required for TLS, run in project root.
'''
openssl req -x509 -nodes -days 365 -newkey rsa:2048 \
-subj /CN=localhost \
-keyout files/nginx.key -out files/nginx.crt
'''
