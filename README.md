# Erlang_ansible_kerl
Install Erlang and required deps by using Ansible and Kerl

!NB!
most ansible playbooks are "Hosts: all"
So be careful to only add localhost to /ets/ansible/hosts
if you intend to install stuff on 1 machine, or multiple hosts etc

# Deps

## Java 
( install the JDK yourself ) horrible ansbile and oracle licenses experience

# SSL


## Kerl
ansible-playbook --ask-become-pass kerl.yml