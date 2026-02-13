# Configuration Management Using Ansible
# Use Ansible to automatically configure a remote Linux server (instead of installing software manually).

# Tools and Technology Used
- Ansible installed on Control Node/Master Node
- Two or More VM required for this Management using Ansible Linux (Ubuntu, CentOS)
- Git
- Python2/3 dependencies
- Linux Editor (Vi, Vim, Nano)


# Command to Install Ansible on Control Node 
$ sudo apt install ansible -y

$ ansible --version   ->  To check version whether it's installed Correctly or not.


# To run Ansible Inventory file is required, it consist of all dependencies like hostname of target VM, varaibales like username, auth key, etc ..

$ ansible <hostname> -i inventory -m ping     ->    this will ping the target host and confirm whether connection is success or not.


# We can install packages using this inventory but playbook yml file is more effiecient and reliable.

$ ansible-playbook <hostname/all> -i inventory <playbook-file.yml>

# For more details you can view the attched file for output whilw running the ansible command.
