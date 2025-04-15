# IVI Credential Summary

This document contains a summary list of the IVI Credentials and who should have access to them.

## Summary of IVI Credentials

| Credential           |  IVI Owner/Backup    | Protected Actions                   | Process Notes |
| ----------           | ----------------     | -----------------                   | ------------- |
| Bank Accounts        | Treasurer/President  | Establishing authorized IVI Signatures, Account owner |  |
| Azure Dev Ops        | TC Chair/President   | Authorize users, manage account     |  |
| Github               | TC Chair/President   | Authorize users, manage account     |  |
| DigiCert             | President/TC Chair   | Purchase IVI certs, insert in vault |  |
| Code signing Certs   | TC Chair/President   | Access IVI private keys, manage signing tools |  |
| NuGet Logon          | TC Chair/President   | Identify packages as IviFoundation owned |  |
| SharePoint admin     | President/TC Chair   | Authorize users, manage account     |  |
| 1Password admin      | President/TC Chair   | Authorize users, manage account     |  |
| IVI EIN (employer ID)| President/TC Chair   | Change entry in vault               |  |
| OLD IVI website admin| President/TC Chair   | Act for IVI                         |  |
| VTM Group admin      | President/TC Chair/designee   | Act for IVI                |  |
| Microsoft Account    | President/TC Chair/designee   | Act for IVI                |  |
| Gravitar (icons)     | President/TC Chair/designee   | Act for IVI                |  |
| CPA Secure Portal    | President/TC Chair/designee   | Act for IVI                |  |
| QuickBooks           | President/TC Chair/designee   | Act for IVI                |  |
| Network Solutions    | President/TC Chair/designee   | Act for IVI                |  |

**NOTES:**

- Several items indicate "Act for IVI", the point is that the authority level is intrinsic in the credential.  Typically, IVI is a customer and the credential only serves to identify and authorize IVI.
- Several credentials include "designee" as possible backup.  These are less restricted than others and may be made available to trusted people working on IVI Foundation business.
- Credentials with a primary owner of the President may be utilized at the discretion of the IVI BoD
- Credentials with a primary owner of the TC Chair may be utilized at the discretion of the IVI Technical Committee
- Credentials with a primary owner of the Treasurer may be utilized at the discretion of the IVI BoD
- Several credentials are used to _authorize_ other users.  For example, the SharePoint credentials are used to specify the privilege level of other users, up to and including authorizing full administrative privileges.  In these cases, the IVI processes (such as the Operating Procedures) dictate how/who/when a user is authorized.  The credentials identified here are those that represent the IVI Foundation and are the ultimate authority to authorize/deauthorize appropriate users based on documented IVI Processes.

## Delegating Authority

All credentials have an identified owner and backup.  In general the backup is authorized to utilize the credential when the owner is not available.  If owners will be unavailable for more than 1 week, they should notify the backup, and possibly designate an additional backup.

Only those credentials that indicate ***designee*** under owner/backup may be shared with someone other than an IVI officer.  These credentials are necessary for conducting various IVI business and do not require the degree of business controls as the others.

## Credential Details

If possible, the username should be: IviFoundation.

The following are our preferences for credential from best to worst:

- Use Passkey stored in 1Password vault if possible (anyone with 1Password access can use it) 
- If 2FA required, sign up 2 users if possible - both should document 2nd factor in 1Password (email, phone, etc)
- If cannot sign-up two user and no Passkey and 2FA required: prefer that the owner be TC Chair, President, or Treasurer; also consider VTM as appropriate as the owner.  Second factor documented.

## 1Password Vaults

The credentials are placed into 1Password vaults.  The vaults are shared by the appropriate authorized people.

- Executive Vault --- all credentials owned by President or TC Chair
- Fiscal Vault -- all credentials owned by President and Treasurer
- General Vault -- all other credentials.  These are owner by Pres/TC Chair and are released individually by an executive for use by someone.
- Perhaps other vaults as needed (maybe we have a web vault with DNS registration, website, …?).  Especially for things that require less security.
