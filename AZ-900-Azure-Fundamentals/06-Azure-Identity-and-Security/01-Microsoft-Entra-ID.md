# Microsoft Entra ID

## 1. What Is Microsoft Entra ID?

**Microsoft Entra ID (formerly Azure Active Directory)** is Microsoft's cloud-based identity and access management service.

Imagine your company has 100 employees who use Microsoft 365, Azure, and other applications.

The company needs to know **who is signing in and what they are allowed to access**.

That's what Microsoft Entra ID helps manage.

### Authentication vs. Authorization

**Authentication → Who are you?**

Example: Signing in using your company email and password.

**Authorization → What are you allowed to access?**

Example: An employee can access their department's applications but not restricted company resources.

## 2. Who Uses Microsoft Entra ID?

**IT Administrators** use it to manage employee accounts, control access, and enforce security policies.

**Developers** use it to add secure sign-in features to applications.

**Employees** use it to sign in to Microsoft 365, Azure, and other connected applications.

## 3. Important Features

### Single Sign-On (SSO)

**SSO allows users to sign in once and access multiple connected applications without signing in separately each time.**

Example: Sign in to your company account and access Outlook, Teams, and other connected applications.

### Multifactor Authentication (MFA)

**MFA requires additional verification beyond a password.**

Example: Enter your password and approve a notification on your phone.

This helps protect accounts even when passwords are compromised.

### Self-Service Password Reset (SSPR)

Allows users to reset their passwords without contacting IT support, when enabled and configured.

### Hybrid Identity

Connects an organization's on-premises Active Directory environment with Microsoft Entra ID.

This helps organizations manage identities across local infrastructure and cloud services.

### Conditional Access

Controls access based on conditions such as the user's location, device, or sign-in risk.

Example: Require MFA when an employee signs in from an unfamiliar location.

### Privileged Identity Management (PIM)

Helps organizations manage powerful administrator permissions.

For example, an administrator can receive elevated access only when needed, instead of having permanent access.

## 4. Microsoft Entra ID Licensing

| Edition | Main Purpose |
|---|---|
| **Free** | Basic identity management, users, groups, and SSO |
| **Premium P1** | Advanced identity management and Conditional Access |
| **Premium P2** | Adds identity protection and Privileged Identity Management |
| **Microsoft 365 Apps edition** | Basic identity features associated with eligible Microsoft 365 subscriptions |

The exact features depend on the license and subscription.

## 5. Security and Monitoring

Microsoft Entra ID also provides tools for managing applications, monitoring sign-ins, reviewing security risks, and controlling authentication.

Features such as smart lockout and banned password lists help protect accounts against password-based attacks.

---

## Key Concepts to Remember

| Concept | Meaning |
|---|---|
| **Microsoft Entra ID** | Manages identities and access |
| **Authentication** | Verifies who you are |
| **Authorization** | Determines what you can access |
| **SSO** | Sign in once to access multiple applications |
| **MFA** | Additional sign-in verification |
| **SSPR** | Reset your own password |
| **Conditional Access** | Controls access based on conditions |
| **PIM** | Controls privileged administrator access |

**Main takeaway:** Microsoft Entra ID helps organizations ensure that the right people can securely access the right resources.