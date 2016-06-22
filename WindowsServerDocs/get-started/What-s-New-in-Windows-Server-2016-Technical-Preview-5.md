---
title: What&#39;s New in Windows Server 2016 Technical Preview 5
ms.custom: na
ms.prod: windows-server-threshold
ms.reviewer: na
ms.suite: na
ms.technology: 
  - server-general
ms.tgt_pltfrm: na
ms.topic: article
ms.assetid: 2827f332-44d4-4785-8b13-98429087dcc7
author: jaimeo
---
# What&#39;s New in Windows Server 2016 Technical Preview 5
The content in this section describes what's new and changed in Windows Server® 2016 Technical Preview. The new features and changes listed here are the ones most likely to have the greatest impact as you work with this release. There are several new additions in each of these areas: [Compute](What-s-New-in-Windows-Server-2016-Technical-Preview-5.md#BKMK_Compute), [Identity](What-s-New-in-Windows-Server-2016-Technical-Preview-5.md#BKMK_Identity), [Management and Automation](What-s-New-in-Windows-Server-2016-Technical-Preview-5.md#BKMK_ManagAuto), [Networking](What-s-New-in-Windows-Server-2016-Technical-Preview-5.md#BKMK_Networking), [Security](What-s-New-in-Windows-Server-2016-Technical-Preview-5.md#BKMK_Security), and [Storage](What-s-New-in-Windows-Server-2016-Technical-Preview-5.md#BKMK_Storage).  
  
> [!IMPORTANT]  
> This preview release should not be used in production environments.  
  
## <a name="BKMK_Compute"></a>Compute  
The Compute area includes virtualization products and features for the IT professional to design, deploy, and maintain Windows Server.  
  
### General  
**New for Technical Preview 5**: Physical and virtual machines benefit from greater time accuracy due to improvements in the Win32 Time and Hyper-V Time Synchronization Services. Windows Server can now host services that are compliant with upcoming regulations which require a 1ms accuracy with regards to UTC.  
  
### Hyper-V  
-   [What's new in Hyper-V on Windows Server 2016 Technical Preview](../compute/hyper-v/What-s-new-in-Hyper-V-on-Windows-Server-2016-Technical-Preview.md). This topic explains the new and changed functionality of the Hyper\-V role in Windows Server 2016 Technical Preview, Client Hyper\-V running on Windows 10, and Microsoft Hyper\-V Server Technical Preview.  
  
-   [Windows Containers](https://msdn.microsoft.com/virtualization/windowscontainers/containers_welcome):  **new for Technical Preview 5**, Windows Server 2016 Technical Preview container support adds performance improvements, simplified network management, and support for Windows containers on Windows 10. For some additional information on containers, see [Containers: Docker, Windows and Trends](http://azure.microsoft.com/blog/2015/08/17/containers-docker-windows-and-trends/).  
  
### Nano Server  
What's New in [Nano Server](https://technet.microsoft.com/library/mt126167.aspx). **Starting in Technical Preview 5**, Nano Server now has an updated module for building Nano Server images, including more separation of physical host and guest virtual machine functionality as well as support for different Windows Server editions.   
There are also improvements to the Recovery Console, including separation of inbound and outbound firewall rules as well as the ability to repair configuration of WinRM.  
  
### Remote Desktop Services  
[Use Azure SQL DB for your Remote Desktop Connection Broker high availability environment](../compute/remote-desktop-services/Use-an-Azure-SQL-database-to-enable-high-availability-for-your-Connection-Broker.md). With the release of **Technical Preview 5**, deploying a highly available RDS deployment lets you leverage Azure SQL Database for your RD Connection Brokers in high availability mode.  
  
## <a name="BKMK_Identity"></a>Identity and Access  
New features in Identity improve the ability for organizations to secure Active Directory environments and help them migrate to cloud-only deployments and hybrid deployments, where some applications and services are hosted in the cloud and others are hosted on premises.  
  
### Active Directory Certificate Services  
What’s New in Active Directory Certificate Services. Active Directory Certificate Services \(AD CS\) in Windows Server 2016 Technical Preview increases support for TPM key attestation: You can now use Smart Card KSP for key attestation, and devices that are not joined to the domain can now use NDES enrollment to get certificates that can be attested for keys being in a TPM.  
  
### Active Directory Domain Services  
Active Directory Domain Services includes improvements to help organizations secure Active Directory environments and provide better identity management experiences for both corporate and personal devices. For more information, see [What's new in Active Directory Domain Services (AD DS) in Windows Server Technical Preview](https://technet.microsoft.com/library/mt163897.aspx).   
  
### Active Directory Federation Services  
What’s New in Active Directory Federation Services. Active Directory Federation Services \(AD FS\) in Windows Server 2016 Technical Preview includes new features that enable you to configure AD FS to authenticate users stored in Lightweight Directory Access Protocol \(LDAP\) directories. For more information, see   [What's New in AD FS for Windows Server 2016](../identity/ad-fs/overview/What-s-new-in-Active-Directory-Federation-Services-for-Windows-Server-2016-Technical-Preview.md).  
  
### Web Application Proxy  
The latest version of Web Application Proxyfocuses on new features that enable publishing and preauthentication for more applications and improved user experience. Check out the full list of new features that includes preauthentication for rich client apps such as Exchange ActiveSync and wildcard domains for easier publishing of SharePoint apps. For more information, see [What's New in Web Application Proxy in Windows Server Technical Preview](https://technet.microsoft.com/library/dn765473.aspx).  
  
##  <a name="BKMK_ManagAuto"></a>Management and Automation  
The Management and Automation area focuses on tool and reference information for IT pros who want to run and manage Windows Server Technical Preview, including Windows PowerShell.  
  
Windows PowerShell 5.0 includes significant new features—including support for developing with classes, and new security features—that extend its use, improve its usability, and allow you to control and manage Windows\-based environments more easily and comprehensively. See [Windows Management Framework (WMF) 5.0 RTM Release Notes Overview](https://msdn.microsoft.com/powershell/wmf/releasenotes) for details. **Starting in Technical Preview 5**, new additions include:  
the ability to run PowerShell.exe locally on Nano Server (no longer remote only), new Local Users & Groups cmdlets to replace the GUI, added PowerShell debugging support, and added support in Nano Server for security logging & transcription and JEA.   
  
## <a name="BKMK_Networking"></a>Networking  
This area addresses networking products and features for the IT professional to design, deploy, and maintain Windows Server Technical Preview.  
  
**Technical Preview 5** adds improvements in three main areas. You can now both mirror and route traffic to new or existing virtual appliances. Together with a distributed firewall and Network security groups, this enables you to dynamically segment and secure workloads in a manner similar to Azure. Second, you can deploy and manage the entire Software-defined networking (SDN) stack using System Center Virtual Machine Manager. Finally, you can use Docker to manage Windows Server container networking, and associate SDN policies not only with virtual machines but containers as well. For more information, see [Plan Software Defined Networking Deployment](https://technet.microsoft.com/library/mt605207.aspx).  
  
## <a name="BKMK_Security"></a>Security  
Includes ecurity solutions and features for the IT professional to deploy in your datacenter and cloud environment. For information about security in Windows Server 2016 Technical Preview generally, see [Security and Assurance](https://technet.microsoft.com/library/mt130644.aspx).  
  
### Just Enough Administration  
Just Enough Administration in Windows Server Technical Preview is security technology that enables delegated administration for anything that can be managed with Windows PowerShell. **In Technical Preview 5**, we added support for running under a network identity, connecting over PowerShell Direct, securely copying files to/from JEA endpoints, and configuring the PowerShell console to launch in a JEA context by default. For more details, see [JEA on GitHub](http://aka.ms/JEA).  
  
### Shielded Virtual Machines  
**Starting in Windows Server 2016 Technical Preview 5**, a number of new features are available for shielded virtual machines:  
  
- New "Encryption Supported" mode that offers more protections than for an ordinary virtual machine, but less than "Shielded" mode, while still supporting vTPM, disk encryption, Live Migration traffic encryption, and other features, including direct fabric administration conveniences such as virtual machine console connections and Powershell Direct.  
  
- Full support for converting existing non-shielded Generation 2 virtual machines to shielded virtual machines, including automated disk encryption.  
  
- Hyper-V Virtual Machine Manager can now view the fabrics upon which a shielded virtual is authorized to run, providing a way for the fabric administrator to open a shielded virtual machine's key protector (KP) and view the fabrics it is permitted to run on.  
  
- You can switch Attestation modes on a running Host Guardian Service. Now you can switch on the fly between the less secure but simpler Active Directory-based attestation and TPM-based attestation.  
  
- End-to-end diagnostics tooling based on Windows PowerShell that is able to detect misconfigurations or errors in both guarded Hyper-V hosts and the Host Guardian Service.  
  
- A recovery environment that offers a means to securely troubleshoot and repair shielded virtual machines within the fabric in which they normally run while offering the same level of protection as the shielded virtual machine itself.  
  
For more details and instructions for working with shielded virtual machines, see [Shielded VMs and Guarded Fabric Validation Guide for Windows Server 2016 (TPM)](http://aka.ms/shieldedvms).  
  
### Windows Defender  
[Windows Defender Overview for Windows Server Technical Preview](../security/windows-defender/Windows-Defender-Overview-for-Windows-Server-Technical-Preview.md). Windows Server Antimalware is installed and enabled by default in Windows Server 2016 Technical Preview, but the user interface for Windows Server Antimalware is not installed. However, Windows Server Antimalware will update antimalware definitions and protect the computer without the user interface. If you need the user interface for Windows Server Antimalware, you can install it after the operating system installation by using the Add Roles and Features Wizard.  
  
  
## <a name="BKMK_Storage"></a>Storage  
This area covers storage products and features for the IT professional to design, deploy, and maintain Windows Server Technical Preview.  
  
-   [What's New in File and Storage Services in Windows Server 2016 Technical Preview](../storage/What-s-New-in-File-and-Storage-Services-in-Windows-Server-2016-Technical-Preview.md). **For Technical Preview 5**, enhancements include simplification, manageability, and smaller scale Storage Spaces Direct. The new Health Service continues to improve the day-to-day monitoring, operations, and maintenance experience of Storage Spaces Direct. Storage Replica brings flexibility by expanding stretch clusters to asynchronous support, delegation of administration, and improved efficiency with support for thinly provisioned storage.   
  
-   [What's New in Failover Clustering in Windows Server Technical Preview](../compute/failover-clustering/What-s-New-in-Failover-Clustering-in-Windows-Server-Technical-Preview.md). **For Technical Preview 5** new additions include VM Node Fairness to seamless load balancing of Virtual Machines (VMs) across the nodes in a cluster, VM Start Order introduces start order orchestration for virtual machines (and all groups) in a cluster, and Simplified SMB Multi-channel and Multi-NIC Cluster Networks to make it easier to set up high speed networks on Scale-out File Servers.  
  
## See Also  
  
-   [Release Notes: Important Issues in Windows Server 2016 Technical Preview](Release-Notes--Important-Issues-in-Windows-Server-2016-Technical-Preview.md)  
  
