## Active Directory:
a data base which stores information like your user information, computer information and other network object info. It has capabilities to manage and administrate the complete Network which connect with AD.

## Group Policy:
primarily a security tool and can be used to apply security settings to users and computers within active directory.

## organizational unit (OU) 
 a subdivision within an Active Directory into which you can place users, groups, computers, and other organizational units.

LDAP- Lightweight Directory Access Protocol. A lightweight client-server protocol for accessing directory services.

Domain- A domain is a set of network resources (applications, printers, and so forth)

Tree-An Active Directory tree is a collection of domains within a Microsoft Active Directory network.

Forest-is a group of ad trees

domain controller- is the main or the centerpiece of the Windows Active Directory.

Promoting a server to domain controller:

Install AD DS Role:

**Server manager--> manage--> add roles or features--> select “Role-based or feature-based and select next****à Select server from server pool and press Next****à Check Active Directory Domain services and press Add features then press Next and Next -****à Confirm installation.**

 Promote server:

_Set a static IP_

**Server manager****à Click on flag symbol and click promote this server to domain controller****à Add to existing domain or add new Forrest and press next -****àInput Directory service restore mode password-****àSelect DNS options and press next****à Verify NetBIOS name and press next** **àVerify system folder paths****à Review Options and press next** **à Run perquisite checks****àComplete promotion.**

**Power shell method:**

**Open Powershell**

**Install-WindowsFeature -name AD-Domain-Services -IncludeManagementTools**

**Test-ADDSForestInstallation -DomainName _DOMAINNAME.com_ -InstallDns**

**SafeModeAdministratorPassword**     _enter and confirm password_

**Install-ADDSForest -DomainName _DOMAINNAME.com_ -InstallDNS**

**SafeModeAdministratorPassword**     _enter and confirm password_

Type “A” for “Yes to All” and hit enter

After instillation is completed and server restarts verify success in PowerShell with:

**Get-ADDomainController**

gpupdate/force -forces group policy to update.

gpupdate/result – shows result of group policy update

cached credentials- In an Active Directory domain, a form of the logon information is **cached** locally on users’ machines to allow users to log on to their windows machines when they have no way of reaching the domain controller for authentication.

Apipa address -is automatic private ip addressing typically with a 169.xxx address.

PowerShell- a cross-platform task automation and configuration management framework, consisting of a command-line shell and scripting language. Unlike most shells, which accept and return text, **PowerShell** is built on top of the. NET Common Language Runtime (CLR) and accepts and returns

Host file – an operating system **file** that maps hostnames to IP addresses

Robocopy- Robust File Copy, is a command-line directory and/or file replication command for Microsoft Windows.

Shadow copy- technology included in Microsoft Windows that can create backup **copies** or snapshots of computer files or volumes, even when they are in use.

 print spooler - a software service that manages the printing process

Diskpart - a manual utility with a command-line structure that allows users to alter a disk, drive, partition, or volume.

## Commands:

Ipconfig :

-   Current IPv4 Address
-   Subnet Mask
-   Default Gateway IP
-   Current domain

Ipconfig/all :

-   Physical address:
-   DHCP enabled:
-   Autoconfiguration enabled:
-   IPV6 address:
-   IPV4 address:
-   Subnet mask:
-   Lease obtained/expires:
-   Default gateway:
-   DHCP Server:
-   DNS server:
-   Netbios tcpip:

TRACERT: Trace Route - Number of hops (intermediate servers) before getting to the destination

Time it takes to get to each hop

Ping – sends icmp echo request packets to ip (ttl is time to live value of packets sent)

Ping –t continuous ping

Net stop – stops windows service ie print spooler

Net start – starts service

Net stat – shows active connections

REGEDIT: Edit keys in the Windows registry (use with caution).

Sfc /scannow -scan and fix windows files

Chkdsk – scan entire drive

nslookup- Query the nameserver for the IP address of the given HOST

## File systems:

NTFS (New Technology File system)

·       Supports long file names and larger values then FAT

·       Maximum volume size of 8 petabytes

·       Maximum file size of 16 exabytes

·       Provides ability to authorize user access to files and folders using DACLs(Discretionary Access Control Lists)

·       Provides journaling or protection against accidental deletion.

FAT32 (File Allocation Table)

·       Lacks the file security NTFS provides

·       Max partition size of 32gb

·       Max file size of 4GB

exFAT (Extended File Allocation Table)

·       Optimized for flash drives

·       Designed to be lightweight like FAT32 without the 4gb FAT32 limitation

·       Compatible with Windows, Mac OS X, and Linux (with additional software)