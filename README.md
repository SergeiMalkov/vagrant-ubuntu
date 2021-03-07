# Vagrant playground for ansible - Ubuntu LTS Flavor

This is a basic playground to test simple ansible roles and playbooks.
For virtualization we will utilize Virtualbox virtualization platform under Vagrant control.
This machine uses the most recent `Ubuntu 20.04.2` release.


* Initial provisioning is being performed by `initial_provision.yaml` playbook
* `notes` contain different markdown files that could be handy to have when exploring different features of ansible.

## How to use this code?

1. Clone this repo, optionally adjust Vagrantfile and user-related staff
2. Create VMs with `vagrant up` and initial_provision.yaml will run. <br>
Optionally, you could run `vagrant provision $vm_name`
3. Run `ansible-playbook align_infra.yaml`, assuming that ansible.cfg fits the environment. <br>
in 10-20 minutes you will have a playground with two fully-configured Centos 7 machines.

## What next?

Create your own roles for ansible, test them in this small, but neat playground.