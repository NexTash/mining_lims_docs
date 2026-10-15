# 3. Payment

**Who:** Head of Laboratory. **Result:** Request **Ready**, Invoice **Paid**, Samples
created with status **Waiting**.

Payment is checked outside the system for now (bank statement, cash receipt). When the
money has arrived:

1. Open the **Pending** request.
2. Click **Payment Details** and enter the date and the bank or receipt reference. This is
   stored on the request and the invoice.
3. **Actions > Paid**.

The system now:

- moves the request to **Ready** and the invoice to **Paid**;
- creates one **Sample** record per sample on the request (two tests with three samples
  each give six samples), all with status **Waiting**, linked to the request, the customer
  and the test;
- tells the Technician that the samples are expected.

From here on the work continues on the samples. **View > Samples** on the request lists
them.

Next: [Receiving samples](04-sample-receipt.md).
