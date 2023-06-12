# Recap from quiz
## Resources and Access in the Cloud
### Hierarchy
- Level 1
  - Resources
- Level 2
  - Project
- Level 3
  - File
- Level 4
  - Organization node
### Policies
- Policies can be defined at each resource level
- Policies are also inherited downward
### Project
- Basis for enabling and using Google Cloud services
  - Managing APIs
  - Enabling Billing
  - Adding and removing collaborators
  - Enabling other Google services
- Each project is a separate entity under the organization node, and each resource belongs to exactly one project
- Projects can have different owners and users because they’re billed and managed separately
- Has three identifying attributes
  - project id: unique and immutable
  - project name: not unique and mutable
  - project number: for internal use of Google
### Folder
- Folders can contain **projects** and other **folders**
- Can use folders to group projects under an organization in a hierarchy
  - For example, grouping resources per-department in a folder like Legal, Finance, HR, etc
### Organization node
- Can designate an organization policy administrator so that only people with privilege can change policies
- Can assign a project creator role, which is a great way to control who can create projects and, therefore, who can spend money
### IAM
- Identity and Access Management
- With IAM, administrators can apply policies that define who can do what and on which resources
- The **who** part of an IAM policy can be a Google account, a Google group, a service account, or a Cloud Identity domain
- A “who” is also called a **principal** and each principle has its own identifier, usually an email address
- The **can do what** part of an IAM policy is defined by a role
### IAM Role
- An IAM role is a collection of permissions
- When you grant a role to a principal, you grant all the permissions that the role contains, for example, to manage virtual machine instances in a project, you must be able to create, delete, start, stop and change virtual machines
- When a principal is given a role on a specific element of the resource hierarchy, the resulting policy applies to both the chosen element and all the elements below it in the hierarchy
- Can define deny rules that prevent certain principals from using certain permissions, regardless of the roles they're granted
- Deny policies, like allow policies, are inherited through the resource hierarchy
- There are three kinds of roles in IAM: **basic**, **predefined**, and **custom**
### Basic Role
- When applied to a Google Cloud project, they affect all resources in that project
- Basic roles include **owner**, **editor**, **viewer**, and **billing administrator**
### Predefined Role
- When basic roles are too broad
- Specific Google Cloud services offer sets of predefined roles, and they even define where those roles can be applied
### Custom Role
- When even more specific permission is in need
- Can only be applied to either the project level or organization level but not folder level
