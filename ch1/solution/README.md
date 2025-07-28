## 1.Install ansible
`using yum`
```bash 
sudo yum install ansible -y
```
`using apt`
```bash 
sudo apt install ansible
```
---
## 2.Create an Ansible configuration file under playbooks directory and disable the SSH host key checking for Ansible.

Run below command:

```bash 
vi playbooks/ansible.cfg
```
Add below lines in it and save:

```yaml
[defaults]
host_key_checking = False
```
---
## 3. Create an Ansible inventory file called inventory for host node01 under playbooks directory.
```bash
vi playbooks/inventory.ini
```
Add below content in this file:
```yaml
node01 ansible_host=13.23.44.9 ansible_ssh_pass=admin123 ansible_user=admin
node02 ansible_host=13.23.44.10 ansible_ssh_pass=admin123 ansible_user=admin
```
You can test it out using Ansible ping:
```bash
cd /playbooks
ansible -i inventory node01 -m ping -v
```
---
## 4.Create a group called web_nodes in playbooks/inventory.ini inventory file, further add node01 and node02 as a member of this group.
```yaml
[web_nodes]
node01
node02
```
---
