# Access Control (ACL)

## Access Controls 
  - are the selective restriction of resources, implemented everywhere in computer systems.


## Back End (API Layer)
  - Manage the login cycle with the front-end application
  - Maintain the User’s database
  - Maintain roles for each user
  - Authenticate users (basic and bearer)
  - Create, manage, and apply Role Based Access Controls
  - Maintain and reference their capabilities, based on their role
  - Restrict access to features (like routes) based on capabilities
  - Express Middleware could be used to restrict access to routes
  - Mongoose Middleware/Hooks could be use to restrict access to business logic


## Front End (Client Layer)
  - Initiate the login process
  - Store login tokens as cookies
  - Manage login state, capabilities
  - Control physical & visual access (hide/show/alter) to components based on RBAC rules
  - Alter behaviors based on RBAC rules


## What is RBAC?
    -  is nothing more than the idea of assigning system access to users based on their role within an organization.

  - **RBAC implementation**
    - 1. Inventory your systems
    - 2. Analyze your workforce and create roles
    - 3. Assign people to roles
    - 4. Never make one-off changes
    - 5. Audit
    