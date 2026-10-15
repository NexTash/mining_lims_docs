# Sample

**Purpose:** one sample or specimen through its whole life in the laboratory: expected,
received, prepared, tested, reviewed, approved, stored and disposed of. Samples are created
automatically when a request is paid; pieces are created by splitting a received sample.

**Statuses:** Waiting, Sample Rejected, Received, Preparation Failed, Prepared, Tested, Test
Rejected, Reviewed, Review Rejected, Approved. See the process pages
[4](../process/04-sample-receipt.md), [5](../process/05-sample-preparation.md),
[6](../process/06-testing.md), [7](../process/07-review-and-approval.md) and
[9](../process/09-storage-and-disposal.md).

**Who:** Technician receives and prepares; Engineer tests; Head of Laboratory reviews;
Director approves. The Customer sees only the status of their samples in the portal.

## Header and Scope

| Field | Meaning |
| --- | --- |
| Specimen Code | The laboratory's specimen number printed on the report (UCS-0005). The record ID (S26-00012) is separate. |
| Status | Current step; changed through the Actions menu. |
| Child Sample, Parent Sample, Piece No. | Set automatically for pieces cut from a parent sample. |
| Customer, Request, Customer Email, Customer Address | From the request. |
| Test | The test this sample is for. Fixed when the sample is created. |
| Material | Rock, Soil or Aggregate, from the test. |
| Engineer | The engineer working on the data sheet. Any engineer may start a Prepared sample; the field is filled when the sheet is completed. |
| Borehole ID, Depth From / To, Lithology | Where the sample comes from; printed on the report. |
| Parameters | The results, one line per reported parameter: value, unit, method, status (Pending until the data sheet is completed) and a link to the sheet. Read-only. |

## Receiving tab

| Field | Meaning |
| --- | --- |
| Received On, Received By | Set when the sample is accepted. |
| Delivered By | The customer's person who brought the sample; printed on the receipt form. |
| Condition on Receipt | Intact, Fractured, Weathered, Disturbed or Damaged Packaging. |
| Core Length, Weight, Photo on Receipt, Receipt Remarks | Inspection record. |
| Rejection Note, Rejection Photo | Mandatory to use *Reject Sample*; the note is e-mailed to the customer. |

## Processing tab

| Field | Meaning |
| --- | --- |
| Prepared On, Prepared By | Set when the sample is marked prepared or split. |
| Preparation Method | Sawing, End Facing, Lapping / Grinding, Coring, Trimming, Wet Preparation. |
| Nominal Diameter, Nominal Height | Target dimensions of the specimen; pre-filled on the data sheet. |
| Preparation Notes | Free text. |
| Equipment Used | Equipment, purpose, who used it and for how long. The calibration status is shown; expired equipment is refused when the setting *Block On Expired Calibration* is on. Usage is logged on the equipment record. |
| Room Temperature, Room Humidity | Conditions during preparation and testing. |
| Failure Note, Failure Photo | Mandatory to use *Preparation Failed*. |

## Testing & Review tab

| Field | Meaning |
| --- | --- |
| Tested On | Set when the data sheet is completed. |
| Photo Before / After Testing, Failure Mode / Observation, Laboratory Comments | Printed on the Detailed and Internal reports. |
| Report for Customer | Brief or Detailed; chosen by the Head of Laboratory before approving. Brief by default (see Settings). |
| Review Note, Reviewed By, Reviewed On | The Head of Laboratory's review. The note is mandatory for a rejection and is e-mailed to the engineer. |
| Director Note, Approved By, Approved On | The Director's approval. The note is mandatory for a rejection. |
| Standards Applied | Specifications (acceptance limits) copied from the Test; untick **Print** to leave one off this report. |
| Report Terms / Notes | Text printed under the results, from the Test; can be edited per sample. |

## Storage & Custody tab

| Field | Meaning |
| --- | --- |
| Storage Location, Stored On | Where the material is kept. |
| Retention Days, Discard Due | Retention period (from the Test or Settings) and the resulting due date. |
| Discard Method, Discard Remarks, Discarded On, Discarded By | What was done with the material when the retention ended. |
| Custody Log | Every hand-over with time, people and condition. |

## Buttons

- **Split into Pieces** (Received or Prepared, not on a piece).
- **Print**: Sample Label (QR), Sample Receipt Form, Chain of Custody.
- **Reports** (from Tested): Internal, Detailed, Brief.
- **View**: Request, Observation Data Sheets, Parent Sample.
