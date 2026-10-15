# Customer

**Purpose:** the companies and people the laboratory works for. Every request and sample
belongs to a customer; the customer's contact e-mail receives invoices and reports.

**Created by:** Head of Laboratory, directly with status **Approved** (no approval step).
Technicians, Engineers and the Director can read customers.

## Fields

| Field | Meaning |
| --- | --- |
| Customer Name | Legal or trading name; also the record's ID, printed on reports and invoices. |
| Type | Company, Individual, Government or Research Institute. |
| Status | Approved (can be used on requests) or Disabled. |
| Tax ID, Website, Registration No. | Reference details for invoices. |
| Primary Contact | The contact person. Create contacts from the **Contacts** panel on the left; the first one becomes the primary contact. Its **e-mail** is used for all customer e-mails. |
| Primary Address | The address printed on reports and invoices. Create it from the **Addresses** panel. |
| Portal User | The login that lets this customer use the portal (see below). |
| Portal Login Sent On | When the portal welcome e-mail was sent. |

## Buttons

- **New Request** - starts a request for this customer.
- **View > Requests** - all requests of the customer.
- **Create Portal Login** - creates a website user from the primary contact's e-mail
  address, gives it the *Customer* role, links it here and e-mails the person a link to set
  a password. Later the same button reads **Reset Portal Password**.

!!! warning
    The customer must have an e-mail address on its primary contact before a portal login
    can be created, and before invoices and reports can be e-mailed.
