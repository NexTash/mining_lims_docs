# Request

**Purpose:** the customer's order: which tests, how many samples, for which project. It
drives the price, the invoice and the creation of the samples.

**Statuses:** New → Pending → Ready. See [Creating a request](../process/01-request.md),
[Price and invoice](../process/02-pricing-and-invoice.md) and [Payment](../process/03-payment.md).

**Who:** Technician creates; Head of Laboratory prices and confirms payment; Engineer and
Director read; the Customer sees their own requests in the portal.

## Fields

| Field | Meaning |
| --- | --- |
| Series | Numbering, REQ-YYYY-#####. |
| Customer | Mandatory. The customer the work is for. |
| Customer Address | Defaults to the customer's primary address; any address linked to the customer can be chosen. Printed on invoice and reports. |
| Status | New, Pending, Ready or Cancelled. Changed through the Actions menu. |
| Request Date | Date the request was taken. |
| Required By | Date the customer needs the results. |
| Project / Location | Mine, site or borehole programme; printed on the reports. |
| Contact Email | Address that receives the invoice, rejection notices and approved reports. Filled from the customer; can be changed per request. |
| Items | One line per test: **Test**, **Samples** (how many will come), **Test name on invoice** (wording on the invoice), **Price per sample** and **Amount** (Head of Laboratory and Director only), **Created** (samples created so far). |
| Total Samples | Sum of the sample counts. |
| Total Amount, Price Set By, Price Set On, Invoice | Pricing details; visible to the Head of Laboratory and the Director only. |
| Paid On, Payment Reference | Filled through the **Payment Details** button. |
| Notes, Material Summary | Free text; what will be delivered (cores, boxes, bags). |

## Buttons and actions

- **Actions > Set Final Price** (Head of Laboratory, status New) - creates and e-mails the invoice.
- **Payment Details** and **Actions > Paid** (Head of Laboratory, status Pending) - records the payment and creates the samples.
- **View > Samples**, **View > Invoice**.

A request with samples cannot be cancelled until those samples are cancelled.
