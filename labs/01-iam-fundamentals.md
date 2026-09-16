# IAM Fundamentals Lab

## 1. Objective

The objective of this lab is to develop a foundational understanding of Identity and Access Management (IAM) and demonstrate how organizations control access to systems and information.

## 2. IAM Concepts

This lab focuses on the following core IAM concepts:

- Authentication
- Authorization
- Users and groups
- Roles
- Role-Based Access Control (RBAC)
- Least privilege
- Multi-Factor Authentication (MFA)

## 3. Authentication vs. Authorization

**Authentication** verifies who a user is.

Examples:
- Username and password
- Security key
- Biometric authentication
- Multi-Factor Authentication (MFA)

**Authorization** determines what an authenticated user is allowed to access.

For example, an employee may be authorized to access a payroll application but not the organization's administrator console.

## 4. Role-Based Access Control

RBAC assigns permissions based on a user's job role rather than assigning permissions individually to every user.

Example:

| Role | Example Permissions |
|---|---|
| Help Desk | Reset user passwords |
| Analyst | Access security dashboards |
| Manager | Approve access requests |
| Administrator | Manage security configurations |

## 5. Least Privilege

The principle of least privilege means users should receive only the access necessary to perform their assigned responsibilities.

Example:

A security analyst who investigates alerts may need access to SIEM dashboards and security logs, but does not necessarily need permission to modify firewall configurations.

## 6. Security Scenario

### Scenario

A healthcare organization has three employees:

- Alice — Help Desk Analyst
- Bob — Security Analyst
- Carol — IT Administrator

### Access Requirements

Alice needs to reset passwords and assist users.

Bob needs to investigate security alerts and review logs.

Carol needs administrative access to manage security infrastructure.

### Proposed Access Model

| User | Role | Access |
|---|---|---|
| Alice | Help Desk | User support and password resets |
| Bob | Security Analyst | SIEM and security logs |
| Carol | Administrator | Security infrastructure |

This approach reduces unnecessary privileges and follows the principle of least privilege.

## 7. Security Considerations

Poor IAM practices can create significant security risks, including:

- Excessive user privileges
- Unauthorized access
- Privilege escalation
- Orphaned accounts
- Credential compromise
- Insider threats

Organizations should regularly review user access, remove unnecessary privileges, enforce MFA, and monitor privileged accounts.

## 8. Key Takeaways

This lab demonstrated the relationship between:

**Authentication → Authorization → Roles → Permissions → Least Privilege**

IAM is a fundamental component of enterprise and cloud security because it determines who can access systems, what they can access, and what actions they are permitted to perform.

## 9. Future Lab Extensions

Future work will expand this lab into hands-on implementations involving:

- Active Directory
- Microsoft Entra ID
- RBAC
- MFA
- Privileged Access Management
- Access reviews
- Cloud IAM
