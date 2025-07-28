## 1.Install ansible
## 2. Create an Ansible configuration file under playbooks directory and disable the SSH host key checking for Ansible.
## 3. Create an Ansible inventory file called inventory for host node01 under playbooks directory.
Below are the details of `node01`:
Hostname: `target machine ip`
User: `admin` #change user by your user
Password: `admin123` #change user by your password
Below are the details of`node02`:
Hostname: `target machine ip`
User: `admin` #change user by your user
Password: `admin123` #change user by your password
## 4.Create a group called web_nodes in playbooks/inventory.ini inventory file, further add node01 and node02 as a member of this group.

