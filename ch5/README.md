# Ansible Challenge – Task Overview
### ✅ 1. `lineinfile.yaml`

Create a playbook called **`lineinfile.yaml`** with the following requirements:

- Ensure the file `/var/www/html/index.html` exists.
- If the file does not exist, create it (use `create: yes`).
- Add the line below to the **top** of the file while preserving existing content:


---

### ✅ 2. `archive.yml`

Create a playbook called **`archive.yml`** with the following requirements:

- Create a compressed archive of the directory `/usr/src/ecommerce/`.
- The archive should be named `demo.tar.gz`.
- Save the archive under the directory `/opt/ecommerce/` on all hosts.
- Make sure the archive format is `tar.gz`.

---

### ✅ 3. Install Node.js Role Using Ansible Galaxy

Using **Ansible Galaxy**, install a role named `geerlingguy.nodejs` and place it inside the directory:


---

### ✅ 4. Custom Role: `package`

Create an Ansible role named **`package`** under:


The role must:

- Install the **nginx** package.
- Start the **nginx** service and ensure it's enabled at boot.

Then, create a playbook named **`playbooks/role.yml`** to consume this role and apply it on the target hosts.

---

### 📎 Notes

- All playbooks should be executable using `ansible-playbook`.
- Make sure `become: true` is used when needed.
- Use proper directory structures for roles and tasks.
- Target hosts can be defined in your inventory file or use `localhost` for testing.

