# Group Policy Basics lab

Domain: corp.adtraining.com. Evidence supplied October 25, 2026.

- GPO: Disable Control Panel for End Users.
- Linked to: CorpAdTraining/EndUsers OU.
- Link enabled: Yes. GPO status: Enabled. Enforced: No.
- User Configuration > Policies > Administrative Templates > Control Panel > Prohibit access to Control Panel and PC settings: Enabled selected in the editor.

## Evidence
- 01-GPO-linked-to-EndUsers.png: link location and status.
- 02-Control-Panel-policy-enabled.png: GPO identity, setting path, and Enabled selection. Apply was available; saved setting has not yet been independently verified.

## Pending verification
Save the setting with Apply/OK. Test with an intended domain user in EndUsers on a suitable domain-joined machine, then capture the Control Panel restriction and evidence identifying the applied GPO (for example, a user-scope Group Policy Results report). Do not grant an ordinary test user domain-controller interactive logon merely to test this policy.

This is a user policy. OU location and policy filtering determine scope; a configured and linked GPO alone is not proof that a user's session received it.
