# 4. Receiving samples

**Who:** Technician. **Result:** Sample **Received** (or **Sample Rejected**).

When the customer brings the material to the laboratory:

1. Open **Samples** filtered to **Waiting** (the counter on the workspace) and open the
   sample for this request and test. If several samples look the same, the **Request** and
   **Test** fields tell them apart.
2. In **Scope**, enter what the sample is: **Borehole ID**, **Depth From / To** and
   **Lithology**. Enter a **Specimen Code** if the laboratory numbers specimens itself
   (for example UCS-0005); it is printed on the report.
3. Open the **Receiving** tab and record the inspection: **Delivered By** (the customer's
   person), **Condition on Receipt** (Intact, Fractured, Weathered, Disturbed, Damaged
   Packaging), **Core Length**, **Weight**, a **Photo on Receipt** and any **Receipt
   Remarks**.
4. **Save**.

## Accepting

**Actions > Accept.** The sample becomes **Received**; the receipt date and your name are
recorded and a *Received* line is added to the custody log. Now print:

- **Print > Sample Label (QR)** - stick it on the sample. The QR code opens the sample in
  the system when scanned by a logged-in user.
- **Print > Sample Receipt Form** - the hand-over document. The laboratory and the customer
  both sign it; file the signed copy.
- **Print > Chain of Custody** if the customer requires it.

## Rejecting

If the sample cannot be tested (wrong material, broken core, insufficient quantity):

1. On the **Receiving** tab fill in **Rejection Note** and attach a **Rejection Photo**,
   then **Save**. Both are mandatory; **Reject Sample** is always offered in the Actions
   menu, but the system refuses the rejection and tells you what is missing until both are
   there.
2. **Actions > Reject Sample.** The sample becomes **Sample Rejected**. The customer
   receives an e-mail with the reason and is asked to send another sample; the Head of
   Laboratory receives a copy.
3. When the replacement arrives, open the same sample and use **Actions > Re-deliver**. It
   goes back to **Waiting** and you receive it as above.

Next: [Preparing specimens](05-sample-preparation.md).
