# Privileged Identity Management (PIM) Simulation

## Objective
Simulate Privileged Identity Management (PIM) in Microsoft Entra ID to demonstrate how organizations secure administrative access using just-in-time (JIT) role activation.

---

## Scenario — Admin Access Should Not Be Permanent

In a traditional Role-Based Access Control (RBAC) setup, administrative roles are assigned permanently.

This creates security risks such as:
- Unauthorized access if an account is compromised  
- Excessive permissions beyond job requirements  
- Increased attack surface for privileged accounts  

---

## Current State (RBAC Implementation)

In previous labs, administrative access was assigned using RBAC.

Example:
- User assigned **User Administrator** role  
- Role remains active at all times  

---

## Problem Identified

- User has continuous administrative access  
- No approval required for elevated privileges  
- No expiration or time restriction on access  

---

## Security Risk

Permanent admin roles violate the principle of least privilege.

If compromised:
- Attacker gains full administrative control  
- No time limits reduce detection opportunities  
- Increased risk of system compromise  

---

## Solution — Privileged Identity Management (PIM)

PIM introduces controlled, temporary access to privileged roles.

---

## Simulated PIM Workflow

### Step 1 — Assign Eligible Role
- User is assigned as **eligible**, not active  
- No admin access by default  

---

### Step 2 — Request Activation
- User must request access when needed  
- Justification may be required  

---

### Step 3 — Temporary Access Granted
- Role becomes active for a limited time (example: 1 hour)  

---

### Step 4 — Automatic Expiration
- Access is removed after time expires  
- User returns to standard permissions  

---

## RBAC vs PIM Comparison

| Feature | RBAC | PIM |
|--------|------|-----|
| Access Type | Always Active | Temporary |
| Security Level | Lower | Higher |
| Risk Exposure | High | Reduced |
| Access Control | Static | Dynamic |

---

## Key Takeaway

PIM enforces:
- Just-in-time access  
- Least privilege  
- Time-based permissions  

This significantly reduces risk from privileged accounts.

---

## Real-World Application

Organizations use PIM to:
- Protect admin accounts  
- Reduce insider threats  
- Improve compliance  
- Control access to critical systems  

---

## Lab Limitation

PIM features were not available due to licensing restrictions in the lab environment.

This simulation demonstrates how privileged access would be securely implemented in a real-world environment.

---

## Skills Demonstrated

- Identity and Access Management (IAM)  
- RBAC vs PIM understanding  
- Security risk analysis  
- Privileged access concepts  
