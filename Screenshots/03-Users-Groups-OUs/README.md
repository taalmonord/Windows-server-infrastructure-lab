# Users, groups, and OUs lab

Domain: corp.adtraining.com, managed on DC01. Evidence supplied October 21, 2026.

## Observed configuration
- CorpAdTraining OU contains EndUsers and Security Groups OUs.
- EndUsers contains Alberto Meronta, Brad Coop, Clifford Morehouse, James Dunn, Mike Frank, and Rodger Phillips.
- Security Groups contains HR-Staff and IT-Admins, shown as security groups.
- IT-Admins Members tab shows Clifford Morehouse as a member.
- Clifford's Organization tab shows job title IT Admin, department IT, company CorpAdTraining, and manager James Dunn. That screenshot has an enabled Apply button; persistence of those pending property edits has not been independently verified.

## Evidence limits and next captures
- Group scope and effective permissions are not established by these screenshots. A group named IT-Admins does not automatically grant administrator rights.
- Obtain the sample user's Account tab and each group's General tab if documenting logon settings and scope.
- HR-Staff membership and user sign-in have not yet been demonstrated.
- At the user's request, Clifford replaces Brad as the documented sample account. Screenshot 05 shows Clifford's General tab. Screenshot 06 shows Clifford.Morehouse@corp.adtraining.com (CORP\Clifford.Morehouse), User must change password at next logon selected, and account expiration set to July 30, 2027. Apply is disabled in these captures. The email field shown in General lacks an @ sign and should be corrected or left blank before presenting this as a finished directory profile.
- General/address-tab screenshots were omitted from the selected evidence set because they add little to the OU/group objectives and contain contact/address fields.
