## 1.Install ansible
`using yum`
```bash 
sudo yum install ansible -y
```
`using apt`
```bash 
sudo apt install ansible
```
## 2.Create an Ansible configuration file under playbooks directory and disable the SSH host key checking for Ansible.

Run below command:

```bash 
vi /home/bob/playbooks/ansible.cfg
```
Add below lines in it and save:

```yaml
[defaults]
host_key_checking = False
```