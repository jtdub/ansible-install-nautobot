# Ansible: Install Nautobot
This repository is a set of playbooks that installs everything that is needed for [Nautobot](https://github.com/nautobot/nautobot) on a Redhat-based Linux Distribution.

## Installing

 1. Clone this repository to the system that you want to install Nautobot on.
	 1a. `git clone https://github.com/jtdub/ansible-install-nautobot.git`
 2. Enter the repository directory.
	 2a. `cd ansible-install-nautobot`
 3. Execute `./scripts/run.sh`. This ensures that the necessary packages are installed to run the ansible playbooks.
 4. Modify `./playbooks/group_vars/all` to suite your needs.
 5. Execute ansible.
	 5a. `ansible-playbook -b playbooks/nautobot.yaml`
 6. Profit.
