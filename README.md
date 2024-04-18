
# Notification Crash

* Built on VS2022 17.9 on x64 host, targeting x64
* Works on x64 machine
* Crashes on ARM64 machine


```csharp
    AppNotificationManager notificationManager = AppNotificationManager.Default;
    
    AppNotificationBuilder builder = new AppNotificationBuilder();
    builder.AddText("hello");
    
    notificationManager.Show(builder.BuildNotification());
```


```
Microsoft Windows [Version 10.0.22631.3447]
(c) Microsoft Corporation. All rights reserved.

C:\Users\ste>systeminfo

Host Name:                 WIN11-ARM
OS Name:                   Microsoft Windows 11 Pro
OS Version:                10.0.22631 N/A Build 22631
OS Manufacturer:           Microsoft Corporation
OS Configuration:          Standalone Workstation
OS Build Type:             Multiprocessor Free
Registered Owner:          ste
Registered Organization:   N/A
Product ID:                00330-66899-16971-AAOEM
Original Install Date:     06/09/2022, 08:58:08
System Boot Time:          13/04/2024, 20:11:17
System Manufacturer:       Microsoft Corporation
System Model:              Windows Dev Kit 2023
System Type:               ARM64-based PC
Processor(s):              1 Processor(s) Installed.
                           [01]: ARMv8 (64-bit) Family 8 Model D4B Revision   0 Qualcomm Technologies Inc ~2995 Mhz
BIOS Version:              Microsoft Corporation 12.6.235, 29/01/2024
Windows Directory:         C:\Windows
System Directory:          C:\Windows\system32
Boot Device:               \Device\HarddiskVolume1
System Locale:             en-gb;English (United Kingdom)
Input Locale:              en-gb;English (United Kingdom)
Time Zone:                 (UTC+00:00) Dublin, Edinburgh, Lisbon, London
Total Physical Memory:     32,165 MB
Available Physical Memory: 26,388 MB
Virtual Memory: Max Size:  34,213 MB
Virtual Memory: Available: 28,810 MB
Virtual Memory: In Use:    5,403 MB
Page File Location(s):     C:\pagefile.sys
Domain:                    WORKGROUP
Logon Server:              \\WIN11-ARM
Hotfix(s):                 7 Hotfix(s) Installed.
                           [01]: KB5036620
                           [02]: KB5026039
                           [03]: KB5027397
                           [04]: KB5033055
                           [05]: KB5036893
                           [06]: KB5032393
                           [07]: KB5037020
Network Card(s):           2 NIC(s) Installed.
                           [01]: Surface Ethernet Adapter
                                 Connection Name: Ethernet
                                 DHCP Enabled:    Yes
                                 DHCP Server:     10.0.0.1
                                 IP address(es)
                                 [01]: 10.0.0.123
                                 [02]: fe80::b3aa:a56d:ed0c:f0ef
                           [02]: Bluetooth Device (Personal Area Network)
                                 Connection Name: Bluetooth Network Connection
                                 Status:          Media disconnected
Hyper-V Requirements:      A hypervisor has been detected. Features required for Hyper-V will not be displayed.

```