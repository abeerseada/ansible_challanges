### 1. create a playbook called lineinfile.yaml
a file called /var/www/html/index.html is available (if not, create it using **create: yes**). Using Ansible lineinfile module add the below given content in it:
Welcome to My_Labs!
Also make sure to preserve the existing content and this new line must be added at the top of the file.
---
### 2. Create a playbook called archive.yml
Create an archive of /usr/src/ecommerce/ directory. The archive name must be demo.tar.gz (make sure that archive format is tar.gz) and save it under /opt/ecommerce/ directory on all hosts.
---
### 3. Using Ansible galaxy, install an Ansible role called geerlingguy.nodejs under playbooks/roles directory.
**solution**
```bash
ansible-galaxy install geerlingguy.nodejs -p playbooks/roles
```
---
Create an Ansible role called package under playbooks/roles directory . It should install a package called nginx and should start its service as well.
Further consume this role in playbooks/role.yml playbook