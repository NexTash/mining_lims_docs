# Invoice

**Purpose:** the bill for a request. Created automatically when the Head of Laboratory sets
the final price; never typed by hand.

**Who:** Head of Laboratory and Director of Centre only. Invoices have their own list under
**Operations > Invoices**.

**Statuses:** Pending (sent, awaiting payment) → Paid (set when the request is marked
Paid) or Cancelled.

## Fields

| Field | Meaning |
| --- | --- |
| Request, Customer, Customer E-mail | Copied from the request. |
| Invoice Date, Due Date | Issue date and payment term. |
| Items | One line per test on the request: Description (the test name as worded on the request), Samples, Rate, Amount. |
| Total, Currency | Invoice total. |
| Paid On, Payment Reference | Copied from the request when it is marked Paid. |
| Emailed On, Emailed To | When and where the invoice was e-mailed. |
| Notes | Free text. |

## Buttons

- **E-mail to Customer** - sends (or re-sends) the invoice PDF to the customer e-mail.
- **Print Invoice** - opens the invoice print format.
- **View > Request** - the request it belongs to.

!!! note
    Payment is confirmed on the **Request** (Payment Details, then Actions > Paid); the
    invoice follows. Later versions will connect to the QPay payment gateway.
