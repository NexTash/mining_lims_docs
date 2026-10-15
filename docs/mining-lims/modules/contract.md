# Contract

**Purpose:** optional record of a framework agreement with a customer: which tests, how many
samples and at what price. It is for contract management only; requests do not depend on
it.

**Who:** Head of Laboratory creates and activates; Director of Centre reads. Nobody else
sees contracts.

## Fields

| Field | Meaning |
| --- | --- |
| Customer | The customer the contract is with. |
| Status | Draft, Active, Expired (valid-upto date passed), Closed, Cancelled. |
| Contract Date, Valid From, Valid Upto | Agreement and validity dates. Contracts expire automatically the day after Valid Upto. |
| Agreed Tests | One line per test: Test, Sample Count, Rate per sample; Amount is calculated. |
| Total Samples Agreed, Total Amount | Totals of the lines. |
| Total Samples Collected | Samples received so far under this contract. |

## Actions

**Actions > Activate** moves a Draft contract to Active; **Actions > Close** closes it.
**View > Requests** lists the customer's requests.
