# E-mail notifications

Mining LIMS sends an e-mail at every hand-over of the process. The texts are standard
Frappe **Notifications** (sidebar: Setup > Email Notifications); the Head of Laboratory
can adjust the wording or recipients there.

| When | Who receives it | Content |
| --- | --- | --- |
| Request priced (Set Final Price) | Customer contact e-mail | Invoice as PDF, request to pay and bring the samples. |
| Request priced | Technician | The request has been priced and the invoice sent. |
| Request paid (samples created) | Technician | The sample is expected; please receive it when it arrives. |
| Sample rejected at receipt | Customer contact e-mail, Head of Laboratory | Reason from the rejection note; please send a replacement. |
| Preparation failed | Head of Laboratory | Failure note; contact the customer for a replacement. |
| Data sheet completed (sample Tested) | Head of Laboratory | The sample is ready for review. |
| Test rejected by the Head of Laboratory | The engineer of the sample | Review note; correct and complete again. |
| Sample reviewed | Director of Centre | Waiting for approval; which report was chosen. |
| Review rejected by the Director | Head of Laboratory | Director's note. |
| Sample approved | Customer contact e-mail | The chosen report (Brief or Detailed) as PDF; also available in the portal. |
| Calibration due within the reminder period | Engineers, Head of Laboratory | Equipment and due date. |
| Calibration overdue | Engineers, Head of Laboratory | Equipment is blocked until recalibrated. |
| Retention period over | Technician | The sample can be returned or discarded. |

Sent e-mails are listed in the timeline of the record they concern.

!!! note
    E-mails need an outgoing e-mail account on the server (Setup > Email Account). Without
    one the notifications are queued but not delivered.
