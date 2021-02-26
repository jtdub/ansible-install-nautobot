# Ansible: Install Nautobot
This repository is a set of playbooks that installs everything that is needed for [Nautobot](https://github.com/nautobot/nautobot) on a Redhat-based Linux Distribution.

## Installing

 1. Install `git`.
	 - [ ] `yum -y install git`
 2. Clone this repository to the system that you want to install Nautobot on.
	 - [ ] `git clone https://github.com/jtdub/ansible-install-nautobot.git`
 3. Enter the repository directory.
	 - [ ] `cd ansible-install-nautobot`
 4. Execute the shell scripts to setup the prerequisites
	 - [ ] `./scripts/run.sh`
 5. Modify `./playbooks/group_vars/all` to suit your needs.
 6. Execute ansible.
	 - [ ] `ansible-playbook -b playbooks/nautobot.yaml`
 7. Create admin account in Nautobot.
	 - [ ] `sudo su - nautobot /opt/nautobot/venv/bin/nautobot-server --config /opt/nautobot/nautobot_config.py createsuperuser`
 8. Profit.
