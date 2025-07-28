قبل ما تبدأ عدل ال inventory

### 1. Create a playbook callled perm.yml under /playbooks directory, an inventory file called inventory is already present under /home/bob/playbooks directory itself. Using this playbook perform below mentioned tasks:
*frist create user called sam , group called sam*
1. Create an empty file called blog.txt under /opt/news/ directory on node01. Change its group owner to sam .
2. Create an empty file called story.txt under /opt/news/ directory on node02. Change its user owner to sam .
---
### 2. Create a playbook called file.yml under playbooks/ directory and use this playbook to create a file called /opt/file.txt on node01 host. The contents of the file must be This file is created by Ansible!

### 3. Create a playbook called copy.yml under playbooks/ directory to copy /opt/file.txt file to node01 location /home/file.txt.
ملحوظه :هو نفس الفايل اللي انت انشأته ف السؤال اللي قبل دا , يعني التاسك بيقولك في فايل ف node01 عايز اعمله كوبي ف مكان تاني
يعني انت مش هتعمل كوبي من ال control to target 
انت بتعمل كوبي من مكان فالتارجت لمكان تاني برده فالتارجت
---
### 4. Write a playbook called replace.yml under playbooks/ directory 
1. We have a file called /opt/file.txt on node01. Using Ansible replace module replace string "Ansible" with "Ansible Automation"  in that file.
---
