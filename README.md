"# roles-and-permission" 

Sample DB import 
  1. make new db role_based_access_control 
  2. RUN schema-sample.sql to import dummy roles and permissions
  
  USE:
  username: avinash1@company.com , password: 123456
  username: avinash2@company.com , password: 123456
for accessing dummy users, and in index see their role and permissions.

-------------DB STRUCTURE---------------

USER Table 
user_id, username, password, email, created_at

ROLES  (ex: admin, finance, marketing)
role_id, role_name

USER_ROLE (role assigned to user)
user_id, role_id

PERMISSIONS (Permission definition eg: add_accounts_info, add_billing_info, delete_accounts_info)
perm_id, perm_desc

role_perm (Assigning permission to role)
role_id, perm_id
