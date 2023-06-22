# Access Control (ACL)

### 5 steps to RBAC

1. What is Role Based Access Control (RBAC) and why do we care?
Role-Based Access Control (RBAC) is a security model that provides access control based on predefined roles assigned to users. In RBAC, permissions are associated with roles, and users are assigned specific roles based on their responsibilities and job functions. RBAC simplifies access management by centralizing permissions and reducing administrative overhead. it enhances security, streamlines access management, reduces errors, and improves efficiency in organizations of all sizes. It promotes the principle of least privilege and helps maintain a secure and well-controlled access environment.

2. Describe a Role/Permission heirarchy that you might implement using RBAC.
* Administrator: Manages access and permissions for different functional areas or departments within the organization.
* Manager: Oversees specific teams or projects, with the ability to assign tasks, view relevant reports, and access resources within their assigned area.
* Employee: Has access to resources and permissions necessary for their job role, such as creating and editing documents, accessing certain databases, and participating in specific workflows.
* Guest: Limited access to public information or specific areas of the system, allowing them to view certain content or attend meetings without the ability to make changes or access sensitive data. 

3. What approach might you take to implement RBAC?
* Inventory your systems
* Analyze your workforce and create roles
* Assign people to roles
* Never make one-off changes
* Audit





### wiki - RBAC

1. If Authentication is “you are who you say you are,” what is Authorization?
Authorization is the process of determining what actions or resources a user is allowed to access or perform after successful authentication. It is the process of granting or denying permissions to authenticated users based on their identity, roles, or other attributes

2. Name three primary rules defined for RBAC.
Role assignment: A subject can exercise a permission only if the subject has selected or been assigned a role.
Role authorization: A subject's active role must be authorized for the subject. With rule 1 above, this rule ensures that users can take on only roles for which they are authorized.
Permission authorization: A subject can exercise a permission only if the permission is authorized for the subject's active role. With rules 1 and 2, this rule ensures that users can exercise only permissions for which they are authorized.


3. Describe RBAC to a non-technical friend.
Role-Based Access Control, is a method used to control who can access certain information or perform specific actions within a system. It's like having different levels of access privileges based on the role someone has in an organization.



### RBAC tutorial

1. What Are access rights Associated with? The User? or The Role? Explain.
Access rights in RBAC are associated with roles, not individual users. Roles are predefined sets of permissions that determine what actions can be performed and what resources can be accessed within a system. Each role represents a specific job function or responsibility within an organization.
When a user is assigned a role, they inherit the access rights associated with that role. This means that all users who are assigned the same role will have the same access permissions. It simplifies the management of access control because permissions are defined at the role level, rather than individually for each user.


2. Access Rights, or Authorization, is activated after a user successfully does what?
Access rights, or authorization, is activated after a user successfully authenticates themselves. Authentication is the process of verifying the identity of a user, typically through the use of credentials such as a username and password. Once the user's identity is confirmed and they are deemed to be who they claim to be, the authorization process comes into play. After successful authentication, the authorization process determines what actions and resources the user is allowed to access based on their assigned roles and permissions. The user's identity and associated roles are checked against an access control system or policy to determine the level of access they are granted.

3. Explain how RBAC might benefit a business.
* Enhancing security: RBAC ensures that users have only the necessary access privileges, reducing the risk of unauthorized access or data breaches.
* Streamlining access management: RBAC simplifies user provisioning, role assignments, and permission changes, improving operational efficiency and reducing administrative overhead.
* Ensuring compliance: RBAC helps businesses meet regulatory requirements by enforcing access controls, tracking user activities, and maintaining audit trails for accountability and compliance purposes.