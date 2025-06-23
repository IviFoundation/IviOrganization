# IVI Credential Summary

This document contains:

- A summary list of the IVI Credentials
- Who the IVI Foundation grants access to the credentials
- IVI Practices regarding using the IVI Password safe
- Circumstances where credential owners should share credentials

## Summary of IVI Credentials

| Credential           |  IVI Owner/Backup   | Administrator  | Protected Actions                   | Restricted |
| ----------           | ----------------    | -------------  | -----------------                   | ------------- |
| Bank Accounts        | Treasurer/President |     VTM        | Establishing authorized IVI Signatures, Account owner | yes |
| Azure Dev Ops        | TC Chair/President  |                | Authorize users, manage account     | yes |
| Github               | TC Chair/President  |                | Authorize users, manage account     | yes |
| DigiCert             | President/TC Chair  |                | Purchase IVI certs, insert in vault | yes |
| Code signing Certs   | TC Chair/President  |                | Access IVI private keys, manage signing tools | yes |
| NuGet Logon          | TC Chair/President  |                | Identify packages as IviFoundation owned | yes |
| SharePoint admin     | President/TC Chair  |                | Authorize users, manage account     | yes |
| 1Password admin      | President/TC Chair  |                | Authorize users, manage account     | yes |
| IVI EIN (employer ID)| President/Treasurer |     <none>     | Change entry in vault               | no |
| OLD IVI website admin| President/TC Chair  |                | Act for IVI                         | no |
| VTM Group admin      | President/TC Chair  |                | Act for IVI                         | no |
| Microsoft Account    | President/TC Chair  |                | Act for IVI                         | no |
| Gravitar (icons)     | President/TC Chair  |                | Act for IVI                         | no |
| CPA Secure Portal    | President/Treasurer |                | Act for IVI                         | no |
| QuickBooks           | Treasurer/President |                | Act for IVI                         | no |
| Network Solutions    | President/TC Chair  |                | Act for IVI                         | no |

**NOTES:**

- Several items indicate "Act for IVI", the point is that the authority level is intrinsic in the credential.  Typically, IVI is a customer and the credential only serves to identify and authorize IVI.
- Several credentials are listed as not being restricted.  These are less restricted than others and may be made available to trusted people working on IVI Foundation business.  They are not limited to the designated owner and backup, although the owner/backup are responsible for managing them as described below.
- Credentials with a primary owner of the President may be utilized at the discretion of the IVI BoD
- Credentials with a primary owner of the TC Chair may be utilized at the discretion of the IVI Technical Committee
- Credentials with a primary owner of the Treasurer may be utilized at the discretion of the IVI BoD
- Several credentials are used to _authorize_ other users.  For example, the SharePoint credentials are used to specify the privilege level of other users, up to and including authorizing full administrative privileges.  In these cases, the IVI processes (such as the Operating Procedures) dictate how/who/when a user is authorized.  The credentials identified here are those that represent the IVI Foundation and are the ultimate authority to authorize/deauthorize appropriate users based on documented IVI Processes.
- The administrator (if listed) has access to the credentials and acts on behalf of the owner for IVI.  They are not permitted to share credentials with others.

## Delegating Authority

All credentials have an identified owner and backup.  In general the backup is authorized to utilize the credential as needed.  If owners will be unavailable for extended period, they may designate someone from an IVI member company or the IVI management company to act on their behalf in their absence (and only in their absence)

From time-to-time IVI may hire or appoint a temporarily-authorized-user to perform work on behalf of the foundation that requires one of restricted credentials. In that case at the discretion of the credential owner with approval from the backup, that temporarily-authorized-user can be authorized to use the credential for a fixed period of time.  After the time elapses the credential shall be changed so the temporarily-authorized-user no longer has access (probably requires generating new secrets).

## Credential Details

If possible, the username should be: _IviFoundation_

The following are our preferences for credential type from most preferred to least:

- A Passkey stored in a 1Password vault (with username _IviFoundation_)
- A username/password combination.  If possible, the username should be _IviFoundation_ and the password should be randomly generated by 1Password (with high obscurity, long passwords, enabling non-alphabetic characters et cetera where permitted).
- If a personalized factor is required (such as a phone contact), sign up 2 users if possible - both should document 2nd factor in 1Password (email, phone, etc.)
- Failing the above, prefer that the single owner be TC Chair, President, Secretary, or Treasurer; also consider VTM as appropriate as the owner.  Document the second factor in 1Password.

Most services require two factors, and the first two preferred credential types should be used, and no other users configured.  In this way, the authorized 1Password users get access just through the 1Password authorization.

## 1Password Vaults

The credentials are placed into 1Password vaults.  The vaults are shared by the appropriate authorized people.

- Executive Vault --- all credentials owned by President or TC Chair
- Fiscal Vault -- all credentials owned by President and Treasurer
- General Vault -- all other credentials.  These are owner by Pres/TC Chair and are released individually by an executive for use by someone.
- Other vaults if none of the above categories work (for example we may need a web vault with DNS registration, website credentials, …?).  Especially useful for things that do not require restricted access.

## Updating Credentials

Credentials should be updated annually or when a new person is added with access to sensitive credentials.
