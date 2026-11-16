# Microsoft 365 Security & Identity Management Lab

<img src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/azure/azure-original.svg" alt="Microsoft identity and cloud platform" height="64">

> Practical Microsoft 365 security lab covering user management, Microsoft Entra ID, MFA, Conditional Access, password protection and organizational security policies.

## Project Overview

This project documents a security configuration exercise for a fictional organization with approximately 50 employees using Microsoft 365. I developed IT security, password and AI usage policies and configured selected controls in a Microsoft 365 Business Premium evaluation environment.

## Technology Stack

Microsoft 365 · Microsoft Entra ID · Microsoft Authenticator · FIDO2 · Conditional Access · Microsoft Entra Password Protection · Microsoft 365 Admin Center

## Implementation

### Identity and user management

Created three test accounts, including one Global Administrator and two standard users. Assigned Microsoft 365 Business Premium licenses and verified account roles in the administration interface.

### Multi-factor authentication

Enabled Microsoft Authenticator and FIDO2 as authentication methods. Configured Conditional Access requirements for administrators, internal users and guest/external users. Tested an interactive sign-in with a standard account and successfully approved it using Microsoft Authenticator.

### Conditional Access

Configured policies requiring MFA and blocking legacy authentication methods. Advanced risk-based protection was not available in the evaluation environment without Microsoft Entra ID P2.

### Password protection

Enabled password protection, configured a custom banned-password list and a threshold of 10 failed sign-in attempts. Tested a password containing a banned word and found that it could still be accepted; the test illustrated that the custom list does not necessarily reject every password containing a listed term. The failed-sign-in threshold was reviewed in configuration, not verified through ten consecutive failed sign-ins.

### Security policy documentation

Developed an IT security policy covering accounts, permissions and information handling; a password policy for standard and administrator accounts; and an AI usage policy addressing confidential data and acceptable use.

## Validation Results

| Area | Result |
|---|---|
| Test users and licenses | Created and verified |
| Global Administrator role | Verified |
| MFA authentication methods | Configured |
| Microsoft Authenticator sign-in | Successfully tested |
| Conditional Access | Configured and settings reviewed |
| Legacy authentication blocking | Configured |
| Custom banned-password behavior | Tested; password containing banned term was accepted |
| Entra ID P2 risk detection | Not available with current license |

## Screenshots

Selected screenshots from the lab have been heavily redacted to remove account identifiers and environment details. Original screenshots and the full assignment report are intentionally not included.

### MFA verification

![Redacted Microsoft Authenticator verification screen](screenshots/mfa-verification-redacted.png)

### Authentication configuration

![Redacted MFA configuration screen](screenshots/mfa-configuration-redacted.png)

### Authentication methods

![Redacted authentication methods screen](screenshots/authentication-methods-redacted.png)

## Security Notes and Limitations

This was an educational evaluation tenant, not a production deployment. One administrator account was excluded from an MFA policy during the exercise to avoid accidental lockout; that exception should not be treated as a production security recommendation. Conditional Access settings were reviewed, and MFA sign-in was tested, but not every policy scenario was independently verified. No credentials or tenant identifiers are intentionally published.

## What I Learned

The lab connected written security requirements to practical Microsoft 365 controls. It reinforced the importance of testing identity policies, understanding license restrictions, managing administrator access and documenting unexpected behavior during password validation.

## Project Status

**Completed educational lab.**

---

*Hands-on identity and security configuration project for learning and portfolio purposes.*
