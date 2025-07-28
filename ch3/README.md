قبل ما تبدأ عدل ال inventory

### ✅ 1. `perm.yml` – File Ownership and Permissions

**Location**: `/playbooks/perm.yml`

**Instructions**:
- Create a **user** named `sam` and a **group** named `sam`.
- On `node01`:
  - Create an empty file named `blog.txt` in `/opt/news/`.
  - Set the **group owner** of the file to `sam`.
- On `node02`:
  - Create an empty file named `story.txt` in `/opt/news/`.
  - Set the **user owner** of the file to `sam`.

---

### ✅ 2. `file.yml` – Create File with Content

**Location**: `/playbooks/file.yml`

**Instructions**:
- On `node01`, create a file at `/opt/file.txt`.
- The content of the file must be: This file is created by Ansible!
---

### ✅ 3. `copy.yml` – Local Copy on Target Node

**Location**: `/playbooks/copy.yml`

**Instructions**:
- Copy the file `/opt/file.txt` to `/home/file.txt` **on the same host (`node01`)**.
- This is a local copy operation happening **on the target**, not between control and target nodes.
ملحوظه :هو نفس الفايل اللي انت انشأته ف السؤال اللي قبل دا , يعني التاسك بيقولك في فايل ف node01 عايز اعمله كوبي ف مكان تاني
يعني انت مش هتعمل كوبي من ال control to target 
انت بتعمل كوبي من مكان فالتارجت لمكان تاني برده فالتارجت
---

### ✅ 4. `replace.yml` – Replace Text in a File

**Location**: `/playbooks/replace.yml`

**Instructions**:
- On `node01`, locate the file `/opt/file.txt`.
- Use the Ansible `replace` module to replace string "Ansible" with "Ansible Automation"  in that file.
---
