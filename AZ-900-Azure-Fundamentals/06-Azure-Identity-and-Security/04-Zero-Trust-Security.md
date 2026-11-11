# Zero Trust Security Model

## What Is Zero Trust?

**Zero Trust** is a security model that assumes no user, device, or network should be automatically trusted, even if they are inside the company's network.

Imagine an employee working from the company office.

Traditionally, being connected to the office network might be considered enough to trust them.

With **Zero Trust**, the company still verifies the employee's identity, checks their device, and limits access to only the resources they need.

**Zero Trust = Never trust automatically, always verify.**

## Three Principles of Zero Trust

### 1. Verify Explicitly

Always verify users and devices before granting access.

Security decisions can consider identity, location, device health, and unusual sign-in activity.

**Example:** An employee may need MFA before accessing company data.

### 2. Use Least-Privilege Access

Give users **only the permissions they need**, for only as long as necessary.

- **Just-in-Time (JIT):** Provides access only when needed, for a limited time.
- **Just-Enough Access (JEA):** Provides only the permissions required for a task.

**Example:** An employee who only needs to read reports should not have permission to delete them.

### 3. Assume Breach

Always assume an attacker might already have access to part of your environment.

Organizations should limit the damage by separating resources, encrypting data, and monitoring suspicious activity.

**Example:** If an attacker compromises one computer, security controls should prevent easy access to other systems.

## Six Pillars of Zero Trust

| Pillar | What It Protects |
|---|---|
| **Identities** | Verify users and services using strong authentication |
| **Devices** | Check device health, security, and compliance |
| **Applications** | Secure applications and control permissions |
| **Data** | Classify, label, and encrypt sensitive information |
| **Infrastructure** | Secure servers, cloud resources, and configurations |
| **Networks** | Segment networks, encrypt traffic, and monitor threats |

All six pillars work together to protect an organization's resources.

## Key Takeaway

The **three principles of Zero Trust** are:

1. **Verify explicitly** — Always verify identity and access requests.
2. **Use least privilege** — Give only necessary permissions.
3. **Assume breach** — Prepare for attacks and limit potential damage.

Zero Trust applies to both **on-premises and cloud environments**.