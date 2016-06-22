---
title: The Hyper-V Virtual Machine Management service must be running
description: " "
ms.prod: windows-server-threshold
ms.service: na
manager: timlt
ms.technology: 
  - hyper-v
  - techgroup-compute
ms.tgt_pltfrm: na
ms.topic: article
ms.assetid: f44d6887-6458-4438-9d93-574587e3f7d1
author: KBDAzure
---
# The Hyper-V Virtual Machine Management service must be running
*\[This information is preliminary and subject to change.\]*  
  
*For more information about best practices and scans, see* [Best Practices Analyzer](http://go.microsoft.com/fwlink/?LinkId=122786).  
  
|||  
|-|-|  
|**Operating System**|Windows Server 2016 Technical Preview|  
|**Product\/Feature**|Hyper\-V|  
|**Severity**|Error|  
|**Category**|Prerequisites|  
  
## Issue  
  
*The service required to manage virtual machines is not running.*  
  
## Impact  
  
*No virtual machine management operations can be performed.*  
  
Virtual machines that are running will continue to run. However, you won't be able to manage virtual machines, or create or delete them until the service is running.  
  
## Resolution  
  
*Use the Services snap\-in or Sc config command\-line tool to reconfigure the service to start automatically.*  
  
> [!TIP]  
> If you can't find the service in the desktop app or the command\-line tool reports that the service doesn't exist, the Hyper\-V Management tools probably aren't installed. To install them:  
>   
> - On Windows Server, open Server Manager and use the Add Roles and Features wizard. For more details, see [Install the Hyper-V role on Windows Server Technical Preview](../get-started/Install-the-Hyper-V-role-on-Windows-Server-Technical-Preview.md).  
> - On Windows, from the Desktop, begin typing **programs**, click **Programs and Features** \(Control panel\) > **Turn Windows features on or off** > **Hyper\-V** > **Hyper\-V Management Tools**. Then, click **OK**.  
  
### To reconfigure the service to start automatically using the Services desktop app  
  
1.  Open the Services desktop app. \(Click **Start**, click in the **Start Search** box, type **services.msc**, and then press ENTER.\)  
  
2.  In the details pane, right\-click **Hyper\-V Virtual Machine Management**, and then click **Properties**.  
  
3.  On the **General** tab, in **Startup** type, click **Automatic**.  
  
4.  To start the service, click **Start**.  
  
### To reconfigure the service to start automatically using SC Config  
  
1.  Open Windows PowerShell. \(From the desktop, click **Start** and start typing **Windows PowerShell**.\)  
  
2.  Right\-click **Windows PowerShell** and click **Run as administrator**.  
  
3.  To reconfigure the service, type:  
  
    ```  
    sc config vmms start=auto  
    ```  
  
4.  To start the service, type:  
  
    ```  
    sc start vmms  
    ```  
  
If the service is already configured to start automatically and you just need to restart the service, you can do that from Hyper\-V Manager, or from the "sc start vmms" command shown above.  
  
#### To restart the service from Hyper\-V Manager  
  
1.  Open Hyper\-V Manager. Click **Start**, point to **Administrative Tools**, and then click **Hyper\-V Manager**.  
  
2.  In the navigation pane, click the name of the server if it's not already selected.  
  
3.  In the **Actions** pane, click **Start Service**.  
  
