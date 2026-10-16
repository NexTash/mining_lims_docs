# Roles and permissions

Each user has one role. The table shows what each role can do; "workflow" means the role
can take the actions of its step and edit the fields that step needs.

| | Customer | Technician | Engineer | Head of Laboratory | Director of Centre |
| --- | --- | --- | --- | --- | --- |
| Request | Own, read-only (portal) | Create, workflow | Read | Workflow (price, payment), read all | Read |
| Sample | Own status only (portal) | Workflow (receive, prepare, split), read all | Workflow (test), read all | Workflow (review), read all | Workflow (approve), read all |
| Test report | Own approved report (chosen format) | Read all | Read all | Read all | Read all |
| Invoice and service price | Own invoices (portal and e-mail) | No access | No access | Edit, read all | Read all |
| Customer, Contract | - | Read customers (to pick on a request) | No access | Edit all | Read all |
| Equipment, Calibration, Maintenance | - | Read | Edit all | Read | Read |
| Audit trail, KPI reports | - | No access | No access | Yes | Yes |
| Test, Parameter, Standard, Test Method | - | Read | Read | Edit all | Read |
| Observation Data Sheet | - | Read | Workflow (edit, complete) | Read | Read |
| Settings, users, notifications, print formats | - | No access | No access | Settings; the rest with System Manager | Read |

Rules enforced by the system in addition to the table:

- Only the Technician receives, prepares and splits samples; only the Head of Laboratory
  can approve or reject a Tested sample; only the Director can approve or reject a Reviewed
  sample.
- A split sample has no actions of its own; it follows its pieces.
- The custody log is written by the system and cannot be edited.
- A rejection at receipt, a preparation failure, a test rejection and a review rejection
  each require a note (and a photo for the first two).
- A data sheet cannot be changed once its sample has been reviewed.
- Customers never see other customers' data and have no access to the desk.

The workflows themselves (statuses, actions and the roles allowed to take them) are
standard Frappe Workflows (Setup > Workflows) and can be viewed there.
