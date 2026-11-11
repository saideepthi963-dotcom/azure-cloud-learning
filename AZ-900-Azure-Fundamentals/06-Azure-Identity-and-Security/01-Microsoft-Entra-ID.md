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

## Microsoft Entra Domain Services

**Microsoft Entra Domain Services** provides traditional Windows domain services in Azure without requiring you to manage domain controllers.

Imagine your company has an old application that relies on Windows Active Directory authentication.

You want to move that application to Azure, but it doesn't support modern cloud sign-in methods.

**Microsoft Entra Domain Services allows the application to continue using traditional authentication while Microsoft manages the domain infrastructure.**

### What Does It Provide?

**Domain Join:** Allows Windows computers and servers to join a managed domain.

**Group Policy:** Centrally manages Windows computer and user settings.

**LDAP:** Allows applications to look up users and directory information.

**Kerberos and NTLM:** Traditional Windows authentication protocols.

Microsoft manages the domain controllers, including maintenance, patching, and backups.

### How Does It Work with Microsoft Entra ID?

Microsoft Entra Domain Services synchronizes identities from Microsoft Entra ID into a managed domain.

```text
Microsoft Entra ID
       │
       │ One-way synchronization
       ▼
Microsoft Entra Domain Services
       │
       ▼
Older Windows Applications
```

In hybrid environments, users can also originate from an on-premises Active Directory environment synchronized with Microsoft Entra ID.

The managed domain provides traditional authentication without requiring organizations to deploy their own domain controllers.

### Other Important Features

**High Availability:** Microsoft deploys multiple managed domain controllers for reliability.

**Managed Infrastructure:** Microsoft handles the underlying domain controller infrastructure.

**One-Way Synchronization:** Identity information flows from Microsoft Entra ID into the managed domain, not back to Entra ID.

**Legacy Application Support:** Helps migrate applications requiring LDAP, Kerberos, NTLM, or Group Policy.

### Microsoft Entra ID vs. Entra Domain Services

| Microsoft Entra ID | Microsoft Entra Domain Services |
|---|---|
| Modern cloud identity management | Traditional Windows domain services |
| Supports cloud application authentication and SSO | Supports LDAP, Kerberos, and NTLM |
| Used for Microsoft 365 and Azure access | Used for legacy applications and domain-joined VMs |
| Cloud identity platform | Microsoft-managed domain infrastructure |

**Main takeaway:** Microsoft Entra Domain Services helps older applications use traditional Windows authentication in Azure without requiring you to manage domain controllers.

## Microsoft Entra ID Authentication

**Authentication means verifying that a person is who they claim to be.**

Microsoft Entra ID provides several ways to make sign-ins more secure and convenient.

### 1. Self-Service Password Reset (SSPR)

Imagine an employee forgets their Microsoft 365 password.

Instead of contacting IT support, they can verify their identity and reset the password themselves.

**SSPR → Reset forgotten passwords without IT assistance.**

Users can access the password reset portal at https://aka.ms/sspr.

### 2. Multifactor Authentication (MFA)

Imagine someone steals your password.

Normally, they might be able to sign in using it. But with MFA, they must also pass another identity check.

For example, you enter your password and approve a notification in Microsoft Authenticator.

MFA uses different types of authentication factors:

| Factor | Example |
|---|---|
| **Something you know** | Password or PIN |
| **Something you have** | Phone or security key |
| **Something you are** | Fingerprint or facial recognition |

**MFA → Requires two or more different authentication factors to verify your identity.**

### 3. Password Protection

Microsoft Entra ID helps prevent users from choosing weak or easily guessed passwords.

For example, it can block common passwords such as `password123` or passwords containing the company's name.

It uses a global banned-password list and supports custom password restrictions.

**Password Protection → Prevents weak or commonly used passwords.**

### 4. Passwordless Authentication

**Passwordless authentication allows users to sign in without entering a traditional password.**

Imagine unlocking your Windows laptop using your fingerprint instead of typing a password.

Microsoft Entra ID supports several passwordless methods:

**Windows Hello for Business:** Uses fingerprint, facial recognition, or a device PIN.

**FIDO2 Security Keys:** Physical security keys used for secure sign-in.

**Microsoft Authenticator:** Supports passwordless sign-in using a mobile device.

**Passwordless → Sign in securely without entering a traditional password.**

---

## Understanding the Differences

| Feature | Main Purpose |
|---|---|
| **SSPR** | Reset your own forgotten password |
| **MFA** | Add extra verification during sign-in |
| **Password Protection** | Block weak passwords |
| **Passwordless** | Sign in without a traditional password |

### Main Takeaway

Microsoft Entra ID improves authentication by making sign-ins more secure, reducing password-related risks, and allowing users to manage common authentication tasks themselves.