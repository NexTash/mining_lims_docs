# 5. Preparing specimens

**Who:** Technician. **Result:** Sample **Prepared** (one specimen) or several **pieces**,
each **Prepared** with its own data sheet.

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

If one delivered core gives several test specimens, click **Split into Pieces**:

1. Enter the **number of pieces** and, optionally, their **specimen codes** (one per line,
   for example UCS-0005, UCS-0006) and the nominal **diameter** and **height**.
2. Confirm. The system creates one child sample per piece with status **Prepared**, its own
   number and code, its own data sheet and its own QR label. The pieces are listed on the
   parent sample; **View > Parent Sample** on a piece goes back.

Print the labels of the pieces (**Print > Sample Label (QR)** on each piece) and attach
them. The parent sample moves on with its pieces: it is approved when every piece has been
approved.

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
