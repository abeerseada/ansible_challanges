### 1.The playbook /home/bob/playbooks/banana.yml has a variable defined called fruit. There are two tasks written in this playbook to print a text.
Use the when conditional to print I am a Banana if the value of fruit is banana otherwise it should print I am not a Banana.
---
### 2. The playbook playbooks/fruits.yml currently runs an echo command to print a fruit name. Add a loop directive (i.e with_items) in the task to print all fruits defined under the fruits variable.
---
### 3. Create a playbook called package.yml under playbooks/ directory to install vim-enhanced package on localhost.
```bash
ansible-playbook -i localhost, package.yml
```
---
### 4. There is a playbook playbooks/copy_file.yml on student-node. It is supposed to perform below tasks but needs some modification, modify this playbook to add some conditions so that below tasks can be performed:



1. Copy blog.txt file present under /usr/src/condition directory on student-node to node01 under /opt/condition directory. Its user and group owner must be bob and its permissions must be 0640.


2. Copy story.txt file present under /usr/src/condition directory on student-node to node02 under /opt/condition directory. Its user and group owner must be sam and its permissions must be 0400.
---
