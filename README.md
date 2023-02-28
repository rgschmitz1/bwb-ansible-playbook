# Purpose

Document infrastructure as code (IaC) used to automate VM setup to run Bwb

# Dependencies

* Ansible CLI

# VM configuration

The Ansible playbook included in this repository can be used to configure remote servers quickly.  This assumes that ansible is installed on the workspace used for provisioning the server.

> NOTE: `install-ansible.sh` is included in this repository for installing Ansible.

```
# Install required roles
ansible-galaxy install -r requirements.yml
# Run the playbook to setup the remote server
ansible-playbook -i <remote IP>, -u ubuntu main.yml
```
