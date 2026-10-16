# 2. Price and invoice

**Who:** Head of Laboratory. **Result:** Request **Pending**, Invoice created and e-mailed.

1. Open the **New** request (the *Requests - New* counter on the workspace lists them).
2. In **Items**, check the **Price per sample** of each line. It is pre-filled from the
   Test's service price; change it if this customer or project has a different price.
3. If the test name should read differently on the invoice, edit **Test name on invoice**.
   This only changes the wording on the invoice.
4. **Save**, then **Actions > Set Final Price**.

The system now:

- moves the request to **Pending** and records who set the price and when;
- creates an **Invoice** (INV-2026-00007) with status **Pending**, one line per test;
- e-mails the invoice as a PDF to the request's contact e-mail (if the request has none,
  the customer's primary contact or portal login is used), with a short cover letter asking
  the customer to pay and bring the samples;
- tells the Technician that the request has been priced.

The invoice can be opened from the request (**View > Invoice**) or from **Invoices**. It
can be re-sent with **E-mail to Customer** and printed with **Print Invoice**. In the LIMS
only the Head of Laboratory and the Director of Centre can see invoices; the customer sees
its own invoices in the [customer portal](08-reports-and-portal.md#the-customer-portal).

!!! note
    A Pending request can be changed only by the Head of Laboratory. If the price was
    wrong, correct it on the request and re-send the invoice.

Next: [Payment](03-payment.md).
