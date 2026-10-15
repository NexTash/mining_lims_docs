# Test

**Purpose:** a service the laboratory sells, for example *Uniaxial compressive strength of
rock*. A Test ties together the standard it follows, the data sheet (Test Method), the
parameters it reports, the price and the report templates. Requests are made of Tests and
every sample belongs to one Test.

**Who:** Head of Laboratory creates and edits. Everyone else reads; the **Service Price** is
visible to the Head of Laboratory and the Director only.

## Fields

| Field | Meaning |
| --- | --- |
| Test Name, Abbreviation | Name as shown to staff and customers; short code used in specimen codes (UCS, PL). |
| Status | Active tests can be chosen on requests. |
| Material | Rock, Soil or Aggregate. |
| Test Method Standard | The standard (ASTM D7012-23 ...) the data sheet follows; printed on the report. From the [Standards register](standard.md). |
| Category | Rock, Soil, Aggregate or Preparation (for preparation records such as ASTM D4543). |
| Description | Free text. |
| Retention Days | How long material of this test is kept after receipt. |
| Typical Duration Days | Planning information. |
| Storage Instructions | How to store samples of this test. |
| Worksheet Method | The Test Method that defines the data sheet. |
| Requires passed preparation record, Preparation Test | Shows a reminder when a specimen has no approved preparation record of the given test. |
| Specifications | Specifications whose acceptance limits are compared with the results by default; copied to each sample as *Standards Applied*. Leave empty when the customer has no limits. |
| Report Terms / Notes | Printed under the results of every report of this test. |
| Parameters | One line per reported quantity: Parameter, Unit, Method (data sheet that produces it), Decimal Places, Uncertainty (printed), Accredited Range (printed). |
| Service Price per Sample, Currency | The list price proposed on requests. |
| Report Title | Heading of the reports (TEST REPORT - ... by default). |
| Internal / Detailed / Brief Report Format | The print formats used for the three reports. The standard ones cover all tests; a laboratory can copy and adjust a print format per test. |

## Buttons

- **View > Test Method (data sheet)** - opens the data sheet designer of the test.
- **View > Samples** - all samples of this test.

## Adding a new test

1. Make sure the [Standard](standard.md) and the [Parameters](parameter.md) exist.
2. Create the [Test Method](test-method.md) (data sheet) or ask NexTash to.
3. Create the Test, link the standard and the method, add the parameters with units,
   decimals and uncertainty, set the price, save.
