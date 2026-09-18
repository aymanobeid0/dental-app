# Permissions

“Unresolved” means no permission was agreed. It must not be treated as an automatic grant.

## Access matrix

| Action | Owner | Doctor | Staff |
|---|---|---|---|
| Register patients | Unresolved | Unresolved | Allowed |
| Read clinical history | All patients, read-only | Authorized patients | No |
| Read plans and procedures | Yes | Authorized patients | For coordination and billing |
| Create plans and procedures | No through owner role | Yes, own work | No |
| Edit clinical notes | No | Own notes before locking | No |
| Add dated amendments | No | Own notes | No |
| Read allergies and conditions | Yes | Authorized patients | No |
| Update shared medical information | No | Authorized treating doctors | No |
| View patient financial information | Yes | Own activity only | Yes |
| View clinic financial reports | Yes | No | No |
| Record patient payments | Unresolved | Yes | Yes |
| Issue refunds | Yes, with reason/history | Yes, within own financial scope | Yes, with reason/history |
| Correct or void payments | Linked-doctor approval | Own entries with reason; other cases unresolved | Linked-doctor approval |
| Approve payment corrections | No owner override agreed | Linked doctor | No |
| Allocate excess to credit or another procedure | Unresolved | Within own financial scope | Yes |
| Change procedure prices and discounts | Yes | Own procedures | No |
| Record lab/material costs | Yes | Own procedures | Yes |
| Configure compensation | Yes | No | No |
| View individual doctor compensation | All doctors | Own only | No agreed access |
| View own staff compensation | Through owner reporting | Not applicable | Unresolved |
| Record compensation payouts | Unresolved | Unresolved | Unresolved |
| Configure consultation fees | Yes | No | No |
| Apply/waive returning consultation fee | Unresolved | Gives decision to staff | After speaking to doctor |
| Manage mobile money app list | Yes | No | No |
| Set currency label | Yes | No | No |
| Book appointments and choose duration | Unresolved | Yes | Yes |
| Manage doctor availability | All doctors | Own | No |
| Mark arrival | Unresolved | Assigned doctor | Yes |
| Upload clinical attachments | Unresolved | Yes | X-rays; other types unresolved |
| View X-rays | Yes | Authorized patients | Single upload preview only |
| Create prescriptions | No through owner role | Yes | No |
| Save a new medicine to shared list | Unresolved | Yes | Unresolved |
| Enter/correct opening debt | Unresolved | Unresolved | Unresolved |
| Manage accounts and roles | Unresolved | Unresolved | Unresolved |

## Doctor access lifecycle

1. Assignment or booking identifies the doctor but does not grant initial clinical access.
2. Staff or the assigned doctor marks the patient arrived.
3. The doctor can access the clinical record.
4. After consultation or established treatment planning, access continues.
5. Shared clinical history remains visible, but other doctors' financial information does not.
6. Only the author edits their own clinical entries, except shared medical essentials.
7. After the visit, clinical note changes require dated amendments.

## Boundaries requiring later definition

- Combined owner/doctor roles.
- Access revocation when a doctor leaves.
- Separation of shared procedure descriptions from private financial fields.
- Permission to correct actual visit times.
- Procedure catalog maintenance.
- Staff printing of clinical documents.
- Administrative patient-record edits.
- Opening debt and compensation payout administration.
