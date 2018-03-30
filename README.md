# Ansible Conditional Prompt Example

## How To

1. Customize `sample_inventory` to informations of your hosts
2. If you want to set the password for the `foo` user, be sure to set the crypted password as mentioned [here](http://docs.ansible.com/ansible/latest/reference_appendices/faq.html#how-do-i-generate-crypted-passwords-for-the-user-module)
3. Start the play with a command like the following

```bash
ansible-playbook -i inventory site.yml -e configure_user=true
```