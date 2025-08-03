# Windows Server + Client AD Lab Setup

Simulates a small enterprise network.

I built a Windows Server 2019 machine.  
I installed Active Directory Domain Services.  
I configured DNS.  
I connected a Windows 10 client to the domain.  
I tested connectivity and name resolution.

No internet. No external network. Fully internal.

## Lab Goals

- Set up an internal-only network in VirtualBox  
- Promote the server to a domain controller  
- Configure the DNS role  
- Join the client to the domain  
- Test ping and nslookup from the client

## Tools Used

- Windows Server 2019  
- Windows 10  
- VirtualBox  
- Internal network adapter  
- Command Prompt and GUI tools

## Problems Faced

- Ping failed at first  
- DNS didn’t resolve  
- Client couldn’t reach the server  

I fixed this by:

- Assigning static IPs  
- Verifying internal network config  
- Reconnecting virtual adapter  
- Restarting the VM after changes  
- Testing again until success

## Key Commands

- `ping 192.168.56.10`  
- `nslookup lab.local 192.168.56.10`  
- `ipconfig /all`  
- `djoin /requestODJ` (if used)

## Results

- Ping success: 0% packet loss  
- Domain name resolved to IP  
- Client joined the domain  
- DNS and AD services running

## Screenshots

All screenshots are in the `/screenshots` folder.  
They show the full lab setup and troubleshooting process.

## Why This Matters


This lab shows I can **build, fix, and manage** Windows-based networks like a pro. I don’t just follow instructions, I troubleshoot live problems, document my work, and bring value like someone already in the field.
I don’t guess. I test.


##  Contact

Let’s build something real.

**GitHub:** [@gudcyber](https://github.com/gudcyber)  
**LinkedIn:** (https://www.linkedin.com/in/goodness-onyemenam/)
