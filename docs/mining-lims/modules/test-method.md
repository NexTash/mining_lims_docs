# Test Method (data sheet designer)

**Purpose:** the definition of an electronic data sheet: which readings are entered, how
the results are calculated, which validity checks apply and which charts are drawn. One
Test Method serves one or more Tests.

**Who:** Head of Laboratory can edit. NexTash configures the methods with the laboratory
during onboarding; changes to formulas should be made with care, as they affect how results
are calculated from that moment on (completed sheets keep their stored values).

## Fields

| Field | Meaning |
| --- | --- |
| Method Name, Method Code | Name and short code (usually the standard designation). |
| Status | Active or Inactive. |
| ODS Scope | **Per Sample**: one data sheet covers all parameters of the test (the usual case for rock and soil tests). **Per Parameter**: one sheet per parameter. |
| Data Entry Sheet Designer | The visual designer below the fields. |

## The designer

- **Sections** - blocks of the sheet. A **Form** section is one record laid out as a form
  (specimen data, test conditions); a **Grid** section is a table of readings (fixed
  number of rows, or rows the engineer can add). Each has **fields** with a type (number,
  text, selection, checkbox, date), a unit, decimals, a default and, for calculated
  fields, a **formula** written with the other fields (`(m_wet - m_dry) / (m_dry - m_container) * 100`).
- **Summary rows** under a grid: average, minimum, maximum, sum, count, concordant value.
- **Result per parameter** - the formula that gives the reported value of each parameter,
  using the sheet (`mean(dia.reading)`, `peak_load * 1000 / area`). Functions include mean,
  median, sum, min, max, slope, intercept, interpolation, logarithms and trigonometry.
- **Validity checks** - an expression that is true when the requirement of the standard is
  met, a label and a severity: **block**, **flag** or **note**.
- **Charts** - x and y columns of a table (compaction curve, gradation, flow curve) or
  curves of the data-logger series (stress-strain), with axis labels and an optional
  logarithmic x axis.
- **Data-logger series** - the handler that reduces a machine export (UCS stress-strain,
  peak load, soil unconfined compression, consolidation time curves) and the channels the
  file must provide.
- **Preview Sheet** shows exactly what the engineer will see; **Check Formulas** validates
  the definition before saving.
