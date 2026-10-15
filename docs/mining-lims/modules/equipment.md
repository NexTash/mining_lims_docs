# Equipment, calibration and maintenance

**Purpose:** the register of testing machines, measuring instruments and preparation
equipment, with their calibration status, maintenance history and usage.

**Who:** Engineer creates and maintains; everyone else reads. Equipment is added to samples
on the Processing tab, which logs its use.

## Equipment

| Field | Meaning |
| --- | --- |
| Equipment Code, Equipment Name | Laboratory asset number (the record ID) and name. |
| Category | Compression Machine, Point Load Tester, Direct Shear Machine, Triaxial System, Oedometer, Balance, Oven, Caliper, Rock Saw ... |
| Status | Active, Under Maintenance, Out of Service, Retired. Only Active equipment can be used on samples. |
| Manufacturer, Model, Serial No, Location, Responsible, Image | Asset details. |
| Manufactured / Purchased Date, Life-time, End Of Life Date | Lifecycle; the end-of-life date is calculated. |
| Times Used, Usage Hours, Last Used On | Updated automatically from the samples it was used on. |
| Calibration Required, Calibration Interval Days | Whether and how often it must be calibrated. |
| Calibration Status | Not Required, Valid, Due Soon, Expired or Never Calibrated; calculated from the last calibration and the interval. Refreshed daily. |
| Last Calibration Date, Calibration Due Date, Last Calibration | From the latest calibration record. |

**Buttons:** Record Calibration, Record Maintenance, Usage Report.

## Equipment Calibration

One record per calibration event: Calibration Date, Next Due Date (defaults to date plus
interval), Calibrated By (organisation), Certificate No, Result (Pass, Pass with
Adjustment, Fail), Performed By, Certificate file, Uncertainty Note, Remarks. Saving a
passed calibration updates the equipment's status and due date.

## Equipment Maintenance

One record per maintenance job: Type (Preventive, Corrective Repair, Inspection, Upgrade),
Status (Planned, In Progress, Completed), Date, Completed On, Performed By, Next
Maintenance Date, Description, Cost, Downtime Hours, Attachment.

## Reminders and blocking

- Engineers and the Head of Laboratory receive an e-mail when a calibration is due within
  the reminder period set in [Settings](settings.md), and again when it is overdue.
- With *Block On Expired Calibration* switched on, equipment whose calibration has expired
  or was never done cannot be added to a sample being prepared or tested.
