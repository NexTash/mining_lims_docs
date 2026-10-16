# 5. Preparing specimens

**Who:** Technician. **Result:** Sample **Prepared** (one specimen), or several **pieces**
that are each received, prepared and tested on their own.

Preparation turns the delivered material into test specimens: sawing and end-grinding a
core, trimming a soil sample, coring. Record it on the **Processing** tab of the Received
sample:

1. **Preparation Method**, **Nominal Diameter** and **Nominal Height** of the specimen,
   **Preparation Notes**.
2. **Equipment Used** - add the saw, grinder, caliper and so on. The calibration status of
   each item is shown; equipment with an expired calibration cannot be used while the
   *Block On Expired Calibration* rule is on (see [Settings](../modules/settings.md)).
3. **Room Temperature** and **Room Humidity**.
4. **Save**.

## One specimen

If the whole sample is tested as one specimen, use **Actions > Mark Prepared**. The sample
becomes **Prepared**, an **Observation Data Sheet** is created for it, and the Engineer can
start.

## Several specimens: Split into Pieces

If one delivered core gives several test specimens, click **Split into Pieces** on the
Received sample (Technician only):

1. Enter the **number of pieces** and, optionally, their **specimen codes** (one per line,
   for example UCS-0005, UCS-0006) and the nominal **diameter** and **height**.
2. Confirm. The system creates one child sample per piece with status **Received**, its own
   number and code and its own QR label. The pieces are listed on the parent sample;
   **View > Parent Sample** on a piece goes back.
3. Open each piece, record its preparation on the **Processing** tab and use
   **Actions > Mark Prepared**. The piece becomes **Prepared** and its data sheet is created.
   If a piece breaks, use **Preparation Failed** on that piece only.

Print the labels of the pieces (**Print > Sample Label (QR)** on each piece) and attach
them.

Each piece has its own workflow from here on: it is prepared, tested, reviewed and approved
on its own. The parent sample has no actions of its own any more; it follows its pieces and
always shows the least advanced stage among them. It becomes **Prepared** when every piece is
prepared, **Tested** when every piece is tested, and **Approved** when every piece has been
approved. If one piece is sent back, the parent steps back with it.

## When preparation fails

If the specimen breaks or cannot be made to the required dimensions:

1. On the **Processing** tab fill in **Failure Note** and attach a **Failure Photo**. Both
   are mandatory.
2. **Actions > Preparation Failed.** The Head of Laboratory is notified and contacts the
   customer for a replacement.
3. When the replacement arrives use **Actions > Receive Replacement**; the sample is
   **Received** again and preparation starts over.

!!! tip "Preparation record (ASTM D4543)"
    Tests that require a preparation record (for example UCS after D4543) show a reminder
    when no approved preparation record exists for the specimen. Run the preparation test
    on the specimen first if your procedure requires it.

Next: [Testing and the data sheet](06-testing.md).
