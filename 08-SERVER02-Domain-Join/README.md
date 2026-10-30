# SERVER02 network preparation and domain join

Evidence supplied October 29, 2026.

- IPv4 dialog shows 192.168.60.20, mask 255.255.255.0, gateway 192.168.60.2, preferred DNS 192.168.60.10, alternate DNS blank.
- nslookup dc01.corp.adtraining.com. used DNS server DC01.corp.adtraining.com at 192.168.60.10 and returned the expected DC01 hostname/address.
- The dialog captures configured values; ipconfig confirmation of the applied local IP has not yet been supplied. The query verifies DNS reachability and host resolution, not domain membership or full AD service discovery.
- Windows rename to SERVER02 and domain join to corp.adtraining.com remain unverified in these screenshots.

Next evidence: post-restart Local Server showing SERVER02, domain corp.adtraining.com, and its local IP; optionally the AD computer object on DC01.

Screenshot 03 confirms "Welcome to the corp.adtraining.com domain." Background Local Server shows Windows computer name SERVER02 and IPv4 192.168.60.20. The background Workgroup label is pre-refresh/pre-restart state. Domain join succeeded; restart and post-restart membership verification remain pending. Earlier RDS Quick Start was blocked because the server was still in a workgroup; typing into the Domain field instead of the Workgroup field completed the join.
