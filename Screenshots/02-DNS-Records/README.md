# DNS records lab evidence

Completed October 21, 2026 on DC01 in corp.adtraining.com.

- A record: router.corp.adtraining.com -> 192.168.60.2 (VMware NAT gateway).
- CNAME: gateway.corp.adtraining.com -> router.corp.adtraining.com.
- Reverse zone: 60.168.192.in-addr.arpa, covering 192.168.60.0/24.
- PTR: 192.168.60.2 -> router.corp.adtraining.com.

Screenshots 01-03 document the configured records. Screenshot 04 verifies all three with nslookup against DC01's local DNS service (127.0.0.1). Forward name queries use a trailing dot to avoid suffix searching.

Validation: router returned 192.168.60.2; gateway returned router and the expected address with gateway listed as an alias; the reverse lookup returned router.corp.adtraining.com.

These records label the existing VMware gateway; creating them did not create a new router or change routing.

## DC01 reverse lookup extension

Added PTR 192.168.60.10 -> dc01.corp.adtraining.com. Corrected a typo in the target hostname and verified with `nslookup 192.168.60.10`, which returned DC01.corp.adtraining.com and 192.168.60.10. Screenshot 05 shows both router and DC01 PTR records; screenshot 06 shows the successful DC01 reverse lookup. Hostname capitalization does not change DNS identity.
