# Initial setup checklist

A new laboratory sets Mining LIMS up once, in this order. NexTash normally does steps 3 to 5
together with the laboratory during onboarding; the Head of Laboratory can review and
adjust them afterwards.

| # | What | Who | Where |
| --- | --- | --- | --- |
| 1 | Laboratory name, address, accreditation line, logo, report disclaimer and process rules | Head of Laboratory | [Settings](../modules/settings.md) |
| 2 | User accounts for every staff member, with the right role; each person uploads a signature and position | System Manager, then every user | [Users and signatures](../modules/users-and-signatures.md) |
| 3 | The standards the laboratory works to (ASTM, MNS ...), with edition and accreditation scope | Head of Laboratory | [Standard](../modules/standard.md) |
| 4 | Parameters (the quantities that are reported: compressive strength, moisture content ...) | Head of Laboratory | [Parameter](../modules/parameter.md) |
| 5 | Test Methods: the electronic data sheet for each test, with its formulas, validity checks and charts | NexTash with the Head of Laboratory | [Test Method](../modules/test-method.md) |
| 6 | Tests: the services the laboratory sells, each linking a standard, a data sheet, its parameters, the price and the report templates | Head of Laboratory | [Test](../modules/test.md) |
| 7 | Equipment with calibration intervals, and the current calibration certificates | Engineer | [Equipment](../modules/equipment.md) |
| 8 | Storage locations (racks, shelves, rooms) where samples are kept | Technician or Head of Laboratory | [Storage Location](../modules/storage-location.md) |
| 9 | Customers, with a contact e-mail and, where wanted, a portal login | Head of Laboratory | [Customer](../modules/customer.md) |
| 10 | Contracts, if a customer has agreed prices or quantities (optional) | Head of Laboratory | [Contract](../modules/contract.md) |

!!! note "A ready-made test library"
    Mining LIMS ships with a library of common ASTM rock, soil and aggregate tests (UCS,
    point load, Brazilian tensile, slake durability, Atterberg limits, Proctor, CBR, direct
    shear, consolidation, permeability ...), each with its data sheet, standard and
    parameters. During onboarding this library is loaded and then adjusted to the
    laboratory's own procedures, prices and accreditation scope. Check the standard
    editions against your controlled copies before the first customer report.

After the setup, the daily work starts with [Creating a request](../process/01-request.md).
