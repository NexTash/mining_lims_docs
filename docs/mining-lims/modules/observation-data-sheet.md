# Observation Data Sheet

**Purpose:** the electronic worksheet of one test on one specimen. Readings go in, results,
checks and charts come out. Created automatically when a sample is prepared (one sheet per
sample, or one per parameter, depending on the Test Method's layout).

**Statuses:** Draft → Completed (Engineer, *Complete* / *Reopen*). Completing the sheet
marks the sample Tested. See [Testing and the data sheet](../process/06-testing.md).

**Who:** Engineer edits. Head of Laboratory, Technician and Director read.

## Fields

| Field | Meaning |
| --- | --- |
| Sample, Customer, Test | The specimen the sheet belongs to. |
| Method | The Test Method whose data sheet definition is used. |
| Parameter | Filled for per-parameter sheets only. |
| Engineer, Test Date | Who tested and when; filled on completion if left blank. The engineer signs the report. |
| Status | Draft or Completed. |
| Result | The computed results in one line, as shown in lists. |
| Results | One line per parameter with value and status. |
| Raw Data File | The data-logger export attached by **Import Data File**; kept unchanged as the raw record. |
| Imported Rows, Columns in File, Channel Mapping | What was read from the file and how its columns were matched to the method's channels. |
| Validity | Valid or Invalid: Invalid when a blocking check fails. |

The sheet itself (the tables of readings), the **Charts** and the **Checks** are shown
between the header and the footer of the form.

## Buttons

- **Actions > Complete / Reopen**.
- **Data Logger**: Import Data File, Map Channels, Clear Imported Data, Open Raw File.
- **Sheet**: Reload Sheet, Reset Sheet (clears every reading).
- **Print Sheet**, **View > Sample**.

## Rules

- Readings can be entered only while the sample is Prepared or Test Rejected.
- Once the sample is Tested the sheet is locked until the Head of Laboratory rejects it.
- A sheet with no result, a failing blocking check, or a missing data-logger file (where the
  method requires one) cannot be completed.
