# DHCP lab on DC01

Authorization verified October 26, 2026.

The post-install wizard initially reported error 20070 (could not contact Active Directory). Subsequent SRV lookup and nltest domain discovery succeeded. Get-DhcpServerInDC under the earlier account/session returned PermissionDenied, WIN32 5. After signing in as CORP\Administrator and using elevated PowerShell, the query returned no entries. This does not independently establish the cause of the initial wizard error.

User ran:
```powershell
Add-DhcpServerInDC -DnsName "dc01.corp.adtraining.com" -IPAddress 192.168.60.10
Get-DhcpServerInDC
```

The final query listed dc01.corp.adtraining.com at 192.168.60.10, confirming registration in the AD authorized DHCP server list. Screenshot 01 captures this result.

Scope creation, activation, service status, and client lease delivery are not yet verified. VMware NAT DHCP was previously configured with pool 192.168.60.128-192.168.60.254; coordinate it before activating the Windows DHCP scope. Lab subnet is 192.168.60.0/24, gateway 192.168.60.2, domain DNS server DC01 at 192.168.60.10.

Screenshot 02 shows the scope wizard configured with start 192.168.60.100, end 192.168.60.120, prefix /24, mask 255.255.255.0 (21 addresses). Proposed scope name from preceding wizard page: LAN_Network. Wizard completion and activation are still unverified.

Screenshot 03 shows 192.168.60.2 entered on the Router (Default Gateway) page before appearing in the list. User subsequently confirmed clicking Add. Record intended scope router option (003) as 192.168.60.2; final saved scope options are not yet visually verified.
