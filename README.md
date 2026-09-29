# AD-Security-Lab-Full Notes(Phase 2:Lab 2.1-2.11)
"These are personal lab notes from a structured Active Directory offensive security curriculum. All work performed in an authorized, self-built home lab environment. No real organizations, real users, or production systems involved".

AD-Security-Lab

A structured Active Directory offensive security lab, built and operated in a personal home lab environment. This repository documents every phase of the lab from initial AD setup through domain persistence techniques.

Lab Environment
Attacker: Kali Linux
Domain Controller: Windows Server 2022 (WIN-56JEHJD0RI3, domain: redteamlab.local)
Domain Client: Windows 10 (domain-joined)
Additional Target: Ubuntu (standalone, Samba, non-domain-joined)
Virtualization: Oracle VirtualBox, Host-Only network (192.168.56.0/24)
Domain Accounts Used
Account	Type	Notes
Administrator	Domain Admin	Primary escalation target
jdoe	Normal domain user	Sole HR-Team member, AdminCount:True
svc_backup	Service account	Kerberoastable, SPN set, Unconstrained Delegation enabled
asrep	Normal user	AS-REP Roastable (pre-auth disabled)
krbtgt	Built-in KDC account	Target for Golden Ticket (Lab 2.10)
Lab Index
Lab	Topic	Status
2.1	Build AD Lab	✅ Complete
2.2	Windows Internals	✅ Complete
2.3	AD Enumeration	✅ Complete
2.4	Kerberoasting	✅ Complete
2.5	AS-REP Roasting	✅ Complete
2.6	NTLM Attacks (LLMNR/NBT-NS Poisoning)	✅ Complete
2.7	NTLM Relay	✅ Complete
2.8	Lateral Movement	✅ Complete
2.9	Domain Escalation (Unconstrained Delegation + ACL Abuse)	✅ Complete
2.10	Golden Ticket	✅ Complete
2.11	Domain Persistence (AdminSDHolder ACL Abuse)	✅ Complete
Skills Demonstrated
Active Directory enumeration (LDAP, BloodHound, netexec)
Kerberos attack chain (Kerberoasting, AS-REP Roasting, Golden Ticket forgery)
NTLM attack chain (poisoning, capture, relay)
Lateral movement techniques
Domain escalation via delegation and ACL abuse
Domain persistence via AdminSDHolder
Post-exploitation (credential dumping, DCSync)
Packet-level verification of attacks (Wireshark/tcpdump)
