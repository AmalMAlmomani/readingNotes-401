- `<Login />` and `<Auth />`


- `<Auth />` component

  - Based on your permissions and login status, it either gives you access to a component or jsx or hides it.
  - Must not use Redux
    - Why? We don’t want to force implementors into a specific state management system.

# DEFINITION OF ROLE-BASED ACCESS CONTROL (RBAC)
  - restricts network access based on a person's role within an organization and has become one of the main methods for advanced access control. 

  - **Some of the designations in an RBAC tool can include:**

   - 1. Management role scope – it limits what objects the role group is allowed to manage.
   - 2. Management role group – you can add and remove members.
   - 3. Management role – these are the types of tasks that can be performed by a specific role group.
   - 4. Management role assignment – this links a role to a role group.

  - **Other options for user access may include:**
    - `Primary` – the primary contact for a specific account or role.
    - `Billing` – access for one end-user to the billing account.
    - `Technical` – assigned to users that perform technical tasks.
    - `Administrative` – access for users that perform administrative tasks.


  - **BENEFITS OF RBAC:**
    - 1. Reducing administrative work and IT support. 
    - 2. Maximizing operational efficiency.
    - 3. Improving compliance.

  
  - **BEST PRACTICES FOR IMPLEMENTING RBAC:**
    - `Current Status:` Create a list of every software, hardware and app that has some sort of security.
    - `Current Roles:` Even if you do not have a formal roster and list of roles, determining what each individual team member does may only take a little discussion. 
    - `Write a Policy:` Any changes made need to be written for all current and future employees to see.
    - `Make Changes:` Once the current security status and roles are understood (not to mention a policy is written), it’s time to make the changes.
    - `Continually Adapt:` It’s likely that the first iteration of RBAC will require some tweaking. 
