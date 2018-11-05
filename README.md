# Erlang_ansible_kerl
Install Erlang and required deps by using Ansible and Kerl

# Getting Started

Install required Ansible roles ( If you are not installing all the erlang
dependancies yourself.
```
ansible-galaxy install geerlingguy.homebrew
```

=======
!NB!
most ansible playbooks are "Hosts: all"
So be careful to only add localhost to /ets/ansible/hosts
if you intend to install stuff on 1 machine, or multiple hosts etc


## Java 
( install the JDK yourself ) horrible ansbile and oracle licenses experience

# OpenSSL
Install openssl.yml with ansible, ( WIP ) passing in params to openssl.yml
```
ansible-playbook --ask-become-pass 
```
OR
install openssl with ( homebrew ): 
```
ansible-playbook --ask-become-pass erlang_homebrow_deps_packages.yml
```

if installing openssl with homebrew, then configure Erlang to use:
```
./configure --with-ssl=/usr/local/opt/openssl
```

## Kerl
```
ansible-playbook --ask-become-pass kerl.yml
```