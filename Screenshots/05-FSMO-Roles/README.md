# FSMO Roles in Action

Baseline captured October 26, 2026 using `netdom query fsmo`.

All five roles are held by DC01.corp.adtraining.com:
- Schema master
- Domain naming master
- PDC emulator (displayed as PDC)
- RID master (displayed as RID pool manager)
- Infrastructure master

The query completed successfully. Screenshot 01 records the before-change state. No transfer, seizure, or second domain controller has been verified in this lab evidence yet.
