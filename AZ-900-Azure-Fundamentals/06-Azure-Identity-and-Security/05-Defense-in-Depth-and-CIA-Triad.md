# Defense in Depth and CIA Triad

## 1. Defense in Depth

**Defense in Depth** is a security strategy that uses multiple layers of protection instead of relying on a single security measure.

Imagine a company protecting its customer database.

Even if an attacker gets past the firewall, they still need to bypass network restrictions, server security, application security, and data encryption.

**The idea:** If one security layer fails, other layers continue protecting the data.

### Seven Layers of Defense in Depth

| Layer | Purpose |
|---|---|
| **Physical Security** | Prevent unauthorized access to datacenters |
| **Identity & Access** | Verify users and control permissions |
| **Perimeter** | Protect against external threats, including DDoS attacks |
| **Network** | Restrict communication between network resources |
| **Compute** | Protect virtual machines and servers |
| **Application** | Protect applications from security vulnerabilities |
| **Data** | Protect sensitive information through access controls and encryption |

Each layer provides additional protection, making it harder for an attacker to reach valuable data.

## 2. CIA Triad

The **CIA Triad** represents three fundamental goals of information security:

### Confidentiality — Keep Data Private

Only authorized people should be able to access sensitive information.

**Example:** Encrypting customer passwords and financial information to prevent unauthorized access.

### Integrity — Keep Data Accurate

Data should remain correct and should not be changed without authorization.

**Example:** Ensuring a database record hasn't been secretly modified.

### Availability — Keep Data Accessible

Authorized users should be able to access applications and data when needed.

**Example:** Maintaining backup systems to keep a website available during a server failure.

### CIA Triad Summary

| Principle | Meaning |
|---|---|
| **Confidentiality** | Protect data from unauthorized access |
| **Integrity** | Prevent unauthorized changes to data |
| **Availability** | Ensure data and services remain accessible |

Security decisions often involve balancing these three goals.

## Key Takeaway

**Defense in Depth → Multiple security layers protect resources even if one layer fails.**

**CIA Triad → Confidentiality, Integrity, and Availability.**

Both concepts help organizations design stronger security strategies for cloud and on-premises environments.