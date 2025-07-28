
# Ansible Challenge – Conditional Logic, Loops, and File Management

This repository includes four Ansible tasks focusing on conditionals, loops, file management, and package installation.

---

### ✅ 1. Conditional Output – `playbooks/banana.yml`

**Objective**: Modify the playbook to conditionally display a message based on the value of the variable `fruit`.

- If `fruit == "banana"`, print: I am a Banana
- Otherwise, print: I am not a Banana


> Use the `when` condition in each task to handle the logic.

---

### ✅ 2. Loop Over Fruit List – `playbooks/fruits.yml`

**Objective**: Enhance the playbook to loop over multiple fruits.

- A variable called `fruits` contains a list of fruit names.
- Modify the task to print each fruit using a loop.
- Use either `loop:` or `with_items:` to iterate through the list.

---

### ✅ 3. Install a Package on Localhost – `playbooks/package.yml`

**Objective**: Create a playbook to install the `vim-enhanced` package locally.

```bash
ansible-playbook -i localhost, playbooks/package.yml
```
---
### ✅ 4. There is a playbook playbooks/copy_file.yml on student-node. It is supposed to perform below tasks but needs some modification, modify this playbook to add some conditions so that below tasks can be performed:



- Copy blog.txt file present under /usr/src/condition directory on student-node to node01 under /opt/condition directory. Its user and group owner must be bob and its permissions must be 0640.


- Copy story.txt file present under /usr/src/condition directory on student-node to node02 under /opt/condition directory. Its user and group owner must be sam and its permissions must be 0400.
---