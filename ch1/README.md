## ✅ 1. Install Ansible

Install **Ansible** on your control node (the machine from which you will run Ansible commands).

- Use a package manager suitable for your OS:
  - On RHEL/CentOS: `yum install ansible`
  - On Debian/Ubuntu: `apt install ansible`
  - Or use `pip3 install ansible` for Python-based environments

---

## ✅ 2. Create Ansible Configuration File

- Inside the directory: `playbooks/`
- Create a file named: `ansible.cfg`
- In this file:
  - Disable SSH host key checking to allow automatic SSH connections without manual confirmation.

> 📌 Hint: Use the `[defaults]` section and set `host_key_checking = False`.

---

## ✅ 3. Create Inventory File

- File Name: `inventory.ini`
- Location: `playbooks/` directory
- Add the following two hosts:

### 🔹 Host Details

#### node01
- Hostname: `target machine IP`
- User: `admin` *(update as needed)*
- Password: `admin123` *(update as needed)*

#### node02
- Hostname: `target machine IP`
- User: `admin` *(update as needed)*
- Password: `admin123` *(update as needed)*

> ⚠️ Make sure to use Ansible variables like `ansible_host`, `ansible_user`, and `ansible_password` for proper SSH authentication.

---

## ✅ 4. Define Group `web_nodes`

In the same `inventory.ini` file:

- Create a group called `[web_nodes]`
- Add both `node01` and `node02` as members of this group.

> You will then be able to target them in playbooks using:
```yaml
hosts: web_nodes
```