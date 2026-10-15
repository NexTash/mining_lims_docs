# Standard

**Purpose:** the register of the standards the laboratory works to. There are two kinds:

- **Test Method** or **Practice** - the procedure a test follows (ASTM D7012, ASTM D4543,
  MNS ...). The data sheet implements its calculations and validity requirements, and the
  designation and title are printed on the report. Linked from the Test as *Test Method
  Standard*.
- **Specification** - acceptance limits that results are compared with, for example a
  project requirement "UCS ≥ 50 MPa". Linked from the Test under *Specifications* and
  copied to each sample; results outside a limit are marked on the report.

**Who:** Head of Laboratory maintains; everyone reads.

## Fields

| Field | Meaning |
| --- | --- |
| Designation | As printed, with edition: ASTM D7012-23. This is the record's ID. |
| Title | Full title of the standard. |
| Organisation | ASTM, ISO, MNS, BS, AASHTO, ISRM, Project / Client, Other. |
| Type | Test Method, Practice or Specification. |
| Material | Rock, Soil, Aggregate or General. |
| Status | Active, Superseded or Withdrawn. |
| Edition | Year or edition, e.g. 2023 or 2012 (reapproved 2021). |
| Supersedes | The earlier edition this one replaces. |
| In Accreditation Scope | The method is within the laboratory's MNS ISO/IEC 17025 scope. |
| Document | Controlled copy of the standard (kept private). |
| Scope / Remarks | Free text. |
| Acceptance Limits (Specifications only) | One row per parameter: the parameter, the limit as printed (>= 50, <= 2.5, 6-9), unit and note. |
| Printed Notes | Text printed under the results when the specification is applied. |

!!! note "Keep editions current"
    When a new edition is adopted, create the new designation, set *Supersedes*, mark the
    old one *Superseded* and change the Tests to the new one. Old reports keep the
    designation they were issued with.
