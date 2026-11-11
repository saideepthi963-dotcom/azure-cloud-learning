# Microsoft Entra Conditional Access

**Conditional Access** is a Microsoft Entra ID security feature that controls access to applications and data based on specific conditions.

### How Does It Work?

Imagine an employee accessing company applications:

- **Trusted device and location:** Access may be allowed.
- **Unfamiliar location:** MFA may be required.
- **Suspicious sign-in:** Access may be blocked.

Conditional Access follows:

**Signals → Policy Evaluation → Access Decision**

### Signals Used

| Signal | What It Checks |
|---|---|
| User or Group | Who is signing in? |
| Location | Where are they signing in from? |
| Device | Is the device trusted or compliant? |
| Application | Which application is being accessed? |
| Sign-in Risk | Is the login attempt suspicious? |
| User Risk | Is the account potentially compromised? |

### Access Controls

Based on the conditions, a policy can:

- **Grant access** when requirements are satisfied.
- **Require MFA** or other security requirements.
- **Block access** when necessary.

### Conditional Access vs. MFA

**MFA:** Verifies identity using multiple authentication factors.

**Conditional Access:** Decides when MFA or other access requirements should be enforced.

### Licensing

Conditional Access generally requires **Microsoft Entra ID P1 or P2**. Certain risk-based capabilities require P2.

### Key Takeaway

**Conditional Access = IF certain conditions are met, THEN apply access controls.**