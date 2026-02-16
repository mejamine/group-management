# Group Management for linux

This repository includes multiple playbooks that manages groups in linux.

---

## tasks: 

- Create Group
- Modify Group Name
- Delete Group
- Add Member to Group
- Remove Member from Group

---

## Using in AAP

### General Config :
1. **Inventory:** create from file or manually  
2. **Credential:** SSH username/password + sudo

### Create Group
Before running the playbook add a survey to define these variables :
1. create_group_names (list of groups to create , example : dev,devops ) comma seperated

### Modify Group :
Before running the template add a survey to define these variables :
1. modify_group_old_name : old name of the group
2. modify_group_new_name : new name of the group


### Delete Group
Before running the template add a survey to define these variables :
1. delete_groupe_name : name of the group to delete
2. delete_refactor_group_name : name of the group to move the members to before the delete

### Add Member to Group
Before running the template add a survey to define these variables :
1. add_member_group_name : group name 
2. add_member_member_name : user username to add

### Remove Member from Group
Before running the template add a survey to define these variables :
1. remove_member_group_name : group name
2. remove_member_member_name : user username to remove from group


---

## Variables
### hosts variables : (in hosts.ini or create manuaaly in AAP)(inventory related)
- `ansible_host` – ip address of the host
- `ansible_user` – username of the host user
