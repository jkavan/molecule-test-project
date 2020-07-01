# Molecule test project

This is an example project for testing Ansible using Molecule.

Molecule creates 6 Virtualbox machines and installs/configures Apache, Fail2ban and SSH. Finally, it runs a few tests to verify that the environments are configured properly.

It depends on the Oefenweb.fail2ban role, which can be installed from Ansible Galaxy.

## Steps

* Install ansible and molecule.
* Run `ansible-galaxy install -r requirements.yml` in this directory to download the required Ansible roles.
* Run `molecule test` to run the full test cycle.
