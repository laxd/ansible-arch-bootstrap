# Ansible bootstrap - Arch
Ansible playbook to install ansible dependencies on a arch remote not yet managed by ansible

The requirements that need to be made before running this role:

* A user present on the host with sudo access
* If the host is remote, sshd must be running and allow the user to log in

To run:

    ansible-playbook bootstrap.yml
