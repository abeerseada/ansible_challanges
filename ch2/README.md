## 1.Represent the below given data in Ansible Inventory format in playbooks/inventory_table file

| Server Alias | Server Name   | OS    | User          | Password  |
| ------------ | ------------- | ----- | ------------- | --------- |
| sql\_db1     | sql01.xyz.com | Linux | root          | Lin\$Pass |
| sql\_db2     | sql02.xyz.com | Linux | root          | Lin\$Pass |
| web\_node1   | web01.xyz.com | Win   | administrator | Win\$Pass |
| web\_node2   | web02.xyz.com | Win   | administrator | Win\$Pass |
| web\_node3   | web03.xyz.com | Win   | administrator | Win\$Pass |



| Group Name    | Members                            |
| ------------- | ---------------------------------- |
| db\_nodes     | sql\_db1, sql\_db2                 |
| web\_nodes    | web\_node1, web\_node2, web\_node3 |
| boston\_nodes | sql\_db1, web\_node1               |
| dallas\_nodes | sql\_db2, web\_node2, web\_node3   |
| us\_nodes     | boston\_nodes, dallas\_nodes       |
---
## 2.Create a playbook called playbooks/command.yml which should execute the command to display the contents of file /etc/resolv.conf on localhost. Make sure to use *command module* to complete this task.

