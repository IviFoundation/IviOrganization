# IVI Credential Summary

This document contains:

- A summary list of the IVI Credentials
- Who the IVI Foundation grants access to the credentials
- IVI Practices regarding using the IVI Password safe
- Circumstances where credential owners should share credentials

## Summary of IVI Credentials

| Credential           |  IVI Owner/Backup    | Protected Actions                   | Restricted |
| ----------           | ----------------     | -----------------                   | ------------- |
| Bank Accounts        | Treasurer/President  | Establishing authorized IVI Signatures, Account owner | yes |
| Azure Dev Ops        | TC Chair/President   | Authorize users, manage account     | yes |
| Github               | TC Chair/President   | Authorize users, manage account     | yes |
| DigiCert             | President/TC Chair   | Purchase IVI certs, insert in vault | yes |
| Code signing Certs   | TC Chair/President   | Access IVI private keys, manage signing tools | yes |
| NuGet Logon          | TC Chair/President   | Identify packages as IviFoundation owned | yes |
| SharePoint admin     | President/TC Chair   | Authorize users, manage account     | yes |
| 1Password admin      | President/TC Chair   | Authorize users, manage account     | yes |
| IVI EIN (employer ID)| President/Treasurer  | Change entry in vault               | no |
| OLD IVI website admin| President/TC Chair   | Act for IVI                         | no |
| VTM Group admin      | President/TC Chair   | Act for IVI                         | no |
| Microsoft Account    | President/TC Chair   | Act for IVI                         | no |
| Gravitar (icons)     | President/TC Chair   | Act for IVI                         | no |
| CPA Secure Portal    | President/Treasurer  | Act for IVI                         | no |
| QuickBooks           | Treasurer/President  | Act for IVI                         | no |
| Network Solutions    | President/TC Chair   | Act for IVI                         | no |

**NOTES:**

- Several items indicate "Act for IVI", the point is that the authority level is intrinsic in the credential.  Typically, IVI is a customer and the credential only serves to identify and authorize IVI.
- Several credentials are listed as not being restricted.  These are less restricted than others and may be made available to trusted people working on IVI Foundation business.  They are not limited to the designated owner and backup, although the owner/backup are responsible for managing them as described below.
- Credentials with a primary owner of the President may be utilized at the discretion of the IVI BoD
- Credentials with a primary owner of the TC Chair may be utilized at the discretion of the IVI Technical Committee
- Credentials with a primary owner of the Treasurer may be utilized at the discretion of the IVI BoD
- Several credentials are used to _authorize_ other users.  For example, the SharePoint credentials are used to specify the privilege level of other users, up to and including authorizing full administrative privileges.  In these cases, the IVI processes (such as the Operating Procedures) dictate how/who/when a user is authorized.  The credentials identified here are those that represent the IVI Foundation and are the ultimate authority to authorize/deauthorize appropriate users based on documented IVI Processes.

## Delegating Authority

All credentials have an identified owner and backup.  In general the backup is authorized to utilize the credential as needed.  If owners will be unavailable for extended period, they may designate someone else to act on their behalf in their absence (and only in their absence).

From time-to-time IVI may hire or appoint a temporarily-authorized-user to perform work on behalf of the foundation that requires one of restricted credentials. In that case at the discretion of the credential owner with approval from the backup, that temporarily-authorized-user can be authorized to use the credential for a fixed period of time.  After the time elapses the credential shall be changed so the temporarily-authorized-user no longer has access (probably requires generating new secrets).

Only those credentials that indicate **_designee_** under owner/backup may be shared with someone other than an IVI officer.  These credentials are necessary for conducting various IVI business and do not require the degree of business controls as the others.

## Credential Details

If possible, the username should be: _IviFoundation_

The following are our preferences for credential type from most preferred to least:

- Use Passkey stored in 1Password vault if possible (this permits sharing between owner and designee) 
- If a personalized second factor is required, sign up 2 users if possible - both should document 2nd factor in 1Password (email, phone, etc.)
- Failing the above, prefer that the single owner be TC Chair, President, Secretary, or Treasurer; also consider VTM as appropriate as the owner.  Document the second factor in 1Password.

## 1Password Vaults

The credentials are placed into 1Password vaults.  The vaults are shared by the appropriate authorized people.

- Executive Vault --- all credentials owned by President or TC Chair
- Fiscal Vault -- all credentials owned by President and Treasurer
- General Vault -- all other credentials.  These are owner by Pres/TC Chair and are released individually by an executive for use by someone.
- Other vaults if none of the above categories work (for example we may need a web vault with DNS registration, website credentials, …?).  Especially useful for things that do not require restricted access.
