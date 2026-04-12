## Day 5 — Access Denied (RBAC Troubleshooting)

### Objective
Simulate real-world access issues where a user has group membership but lacks proper role-based permissions in Microsoft Entra ID.

---

### Scenario — User Has Access but Cannot Access Resource

**Ticket:** User reports access denied despite being added to the correct group

---

### Investigation Steps

- Verified user group membership
- Confirmed user is part of IT-Team
- Checked assigned roles for user

**Findings:**

- User had correct group membership  
- No roles were assigned to the user  
- Group membership alone did not grant required permissions  

![User Group Membership](../../screenshots/user-group-membership.png)

![User Assigned Roles](../../screenshots/user-assigned-roles.png)

---

### Resolution

- Assigned **User Administrator** role to the user  
- Refreshed and verified role assignment  

---

**Outcome:**

Access issue resolved by applying appropriate RBAC role

![Role Assigned](../../screenshots/role-assigned-fix.png)

![Role Confirmation](../../screenshots/role-confirmation.png)

---

### Key Takeaway

This lab demonstrates that group membership alone does not grant permissions in Microsoft Entra ID. Role-Based Access Control (RBAC) must be properly configured to provide access.

Understanding the relationship between groups and roles is critical for resolving access-related issues.

---

### Skills Demonstrated

- Role-Based Access Control (RBAC)
- Access troubleshooting
- Permission validation
- Microsoft Entra ID administration
- Problem-solving and root cause analysis
