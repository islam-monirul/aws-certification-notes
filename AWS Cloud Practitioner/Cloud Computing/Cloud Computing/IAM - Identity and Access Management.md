IAM = control access to AWS  
Who can access + what they can do

---

## IAM Basics

-    Global service (no region)
-    Used for authentication + authorization

---

## Root vs IAM Users

### Root User

-    Full access
-    Use only for:
     -    Account setup
     -    Billing / critical actions
-    Never use daily

### IAM Users

-    One user = one person
-    Used for daily access

---

## IAM Groups

-    Group = collection of users
-    Used to assign permissions

Rules:

-    Groups contain only users
-    No nested groups
-    User can be in multiple groups
-    User can exist without group (not recommended)

---

## IAM Policies

-    Define permissions
-    Written in JSON
-    Attached to users or groups

### Key Elements

-    Effect: Allow / Deny
-    Action: What (e.g., s3:GetObject)
-    Resource: Which resource
-    Principal: Who

---

## Least Privilege Principle

-    Give only required permissions
-    No extra access

---

## Policy Types

-    AWS Managed → pre-built
-    Custom → user-created
-    Inline → attached to one user only

---

## Password Policy

-    Minimum length
-    Uppercase / lowercase
-    Numbers / symbols
-    Expiration (e.g., 90 days)
-    Prevent reuse

---

## MFA (Multi-Factor Authentication)

Adds extra security

Requires:

-    Password (something you know)
-    Device (something you have)

### Types

-    Virtual (Authy, Google Authenticator)
-    Hardware (security key)

---

## Access Methods

### 1. Console

-    Web login
-    Uses password (+ MFA)

### 2. CLI

-    Command line access
-    Uses access keys

### 3. SDK

-    Used in code (apps)
-    Uses access keys

---

## Access Keys

-    Access Key ID + Secret Key
-    Used for CLI / SDK

Rules:

-    Keep secret
-    Never share
-    One user → own keys

---

## Important Behaviors

-    IAM is global
-    Permissions inherited from groups
-    Removing from group removes permissions
-    Read-only = cannot create/delete
