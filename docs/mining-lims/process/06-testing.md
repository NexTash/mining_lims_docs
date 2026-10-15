# 6. Testing and the data sheet

**Who:** Engineer (any engineer can start a Prepared sample). **Result:** Sample **Tested**.

Every prepared specimen has an **Observation Data Sheet**: the electronic worksheet of the
test. It replaces the paper sheet and the Excel file. You type the readings, the sheet
calculates the results according to the test method, checks the validity requirements of
the standard and draws the charts.

## Opening the sheet

Open the sample (workspace counter *Samples - Prepared*) and click
**View > Observation Data Sheets**, or open **Observation Data Sheets** from the sidebar and
filter by status *Draft*. The sheet shows the sample, the test, the method and the
engineer; set **Test Date** if it differs from today.

## Entering readings

The sheet is laid out as the method defines it: a block of specimen data, grids of
readings (three diameter readings, three height readings, load steps, sieve masses ...)
and the summary rows underneath (averages, concordant values). Calculated columns and the
**result** of every parameter update as you type. Blank inputs simply give blank results,
so you can fill the sheet in several sittings; **Save** keeps what you have.

Typical inputs include the specimen mass and moisture condition, dimensions, peak load,
duration, failure mode, and the method variant (for example D7012 Method C or D).

## Data-logger files

For machine tests (compression, triaxial, consolidation) the laboratory exports a data
file from the testing machine. Instead of typing the curve:

1. **Data Logger > Import Data File** - attach the export (csv, tsv, txt or xlsx). The file
   is stored unchanged with the sheet as the raw record.
2. The columns are matched to the method's **channels** (time, load, axial sensors, lateral
   sensor, load step ...) by their headers. Check the **Channel Mapping** shown on the
   sheet; use **Data Logger > Map Channels** to correct it.
3. The sheet reduces the series: peak load, stress-strain curves, moduli, Poisson's ratio,
   consolidation t50 / t90 and so on, according to the method. The curves appear in the
   **Charts** section and are printed on the Detailed and Internal reports.

**Data Logger > Clear Imported Data** removes the file and goes back to typed values;
**Open Raw File** shows the original export.

## Validity checks

The **Checks** panel lists the requirements of the standard that the sheet verifies, for
example the length-to-diameter ratio, the agreement of duplicate readings, the loading
rate, or that the mass balance closes.

| Severity | Meaning |
| --- | --- |
| **block** | The sheet cannot be completed until the reading is corrected (or the Head of Laboratory decides how to proceed). |
| **flag** | Allowed, but shown on the sheet and the Internal report for the reviewer to judge. |
| **note** | Information only. |

When a blocking check fails the sheet shows **Validity: Invalid** and a red banner.

## Completing

When every reading is in and the checks pass, use **Actions > Complete**. The system:

- stores the results on the sample (one line per parameter) and marks the sample **Tested**;
- records the test date and the engineer, who signs the report;
- makes the three reports (Internal, Detailed, Brief) available on the sample;
- tells the Head of Laboratory that the sample is ready for review.

A completed sheet can be **Reopened** by the engineer as long as the sample has not been
reviewed. Once the Head of Laboratory has approved it, the sheet is locked; only a
rejection by the Head reopens it.

!!! tip "Print the sheet"
    **Print Sheet** gives the paper copy of the data sheet with every reading, the checks
    and the charts, for the laboratory's records.

Field by field: [Observation Data Sheet reference](../modules/observation-data-sheet.md).
Next: [Review and approval](07-review-and-approval.md).
