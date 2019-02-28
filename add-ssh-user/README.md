# Ansible playbook to add an SSH user
#
To run this playbook use the following command

```
# ansible-playbook -i inventory.ini playbook-add-ssh-user.yml --extra-vars "ssh_user=your_ssh_user remote_password=your_hashed_password" --ask-pass
```
