"# roles-and-permission" 

Sample DB import 
  1.make new db role_based_access_control 
  2. execute 

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
