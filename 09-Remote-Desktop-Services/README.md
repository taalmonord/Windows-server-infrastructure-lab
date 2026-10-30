# RDS Quick Start on SERVER02

Evidence supplied October 29, 2026.

- Target SERVER02.corp.adtraining.com at 192.168.60.20, using CORP\Administrator credentials.
- Quick Start configuration lists RD Connection Broker, RD Web Access, and RD Session Host on the same member server.
- Completion screen reports Succeeded for role services, session collection, and RemoteApp programs.
- RD Web URL shown: https://SERVER02.corp.adtraining.com/rdweb. Browser access and applications have not yet been tested.
- An RDP attempt returned a first-logon password-change requirement. A successful user session is not yet demonstrated.
- The submitted connection-settings image showed incomplete target SERVER and username Cop\James.Dunn; excluded from selected evidence. Use SERVER02.corp.adtraining.com and CORP\James.Dunn (verify the actual account logon name in AD).

Next: complete the test user's required password change through a supported password-change flow without disabling NLA, then retry and capture a successful session with hostname and user identity. Do not capture passwords.

## Subsequent validation

Screenshots 05-07 supersede the earlier pending-session status:
- Connections view lists CORP\James.Dunn as Active on SERVER02.corp.adtraining.com, alongside CORP\Administrator.
- Administrator composed a test message to the user session.
- The matching message appears in the remote desktop with SERVER02 shown in the RDP connection bar, verifying delivery.

The first-logon password issue no longer prevented this session; the exact password-change procedure was not evidenced. The message about working hours was manually composed for practice: no automatic after-hours detection, access restriction, or working-hours policy is demonstrated.

RD Web access, individual RemoteApp launches, licensing configuration, and GPO enforcement remain untested by these images.
