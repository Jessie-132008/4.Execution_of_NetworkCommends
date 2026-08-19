# 4.Execution_of_NetworkCommands
## AIM :Use of Network commands in Real Time environment
## Software : Command Prompt And Network Protocol Analyzer
## Procedure: To do this EXPERIMENT- follows these steps:
<BR>
In this EXPERIMENT- students have to understand basic networking commands e.g cpdump, netstat, ifconfig, nslookup ,traceroute and also Capture ping and traceroute PDUs using a network protocol analyzer 
<BR>
All commands related to Network configuration which includes how to switch to privilege mode
<BR>
and normal mode and how to configure router interface and how to save this configuration to
<BR>
flash memory or permanent memory.
<BR>
This commands includes
<BR>
• Configuring the Router commands
<BR>
• General Commands to configure network
<BR>
• Privileged Mode commands of a router 
<BR>
• Router Processes & Statistics
<BR>
• IP Commands
<BR>
• Other IP Commands e.g. show ip route etc.
<BR>
**Program:**

```

Microsoft Windows [Version 10.0.26200.9168]
(c) Microsoft Corporation. All rights reserved.
C:\Users\acer>ping google.com
Pinging google.com [2404:6800:4007:83c::200e] with 32 bytes of data:
Reply from 2404:6800:4007:83c::200e: time=40ms
Reply from 2404:6800:4007:83c::200e: time=20ms
Reply from 2404:6800:4007:83c::200e: time=18ms
Reply from 2404:6800:4007:83c::200e: time=32ms
Ping statistics for 2404:6800:4007:83c::200e:
    Packets: Sent = 4, Received = 4, Lost = 0 (0% loss),
Approximate round trip times in milli-seconds:
    Minimum = 18ms, Maximum = 40ms, Average = 27ms
C:\Users\acer>ipconfig
Windows IP Configuration
Ethernet adapter Ethernet 2:
   Connection-specific DNS Suffix  . :
   Link-local IPv6 Address . . . . . : fe80::f105:cb0f:d91e:5471%8
   IPv4 Address. . . . . . . . . . . : 192.168.56.1
   Subnet Mask . . . . . . . . . . . : 255.255.255.0
   Default Gateway . . . . . . . . . :
Wireless LAN adapter Local Area Connection* 1:
   Media State . . . . . . . . . . . : Media disconnected
   Connection-specific DNS Suffix  . :
Wireless LAN adapter Local Area Connection* 2:
   Media State . . . . . . . . . . . : Media disconnected
   Connection-specific DNS Suffix  . :
Wireless LAN adapter Wi-Fi:
   Connection-specific DNS Suffix  . : saveetha.in
   IPv6 Address. . . . . . . . . . . : 2403:8600:c090:42:0:400:f0:d5b
   Link-local IPv6 Address . . . . . : fe80::cdd0:4780:c94e:5071%3
   Autoconfiguration IPv4 Address. . : 169.254.85.31
   Subnet Mask . . . . . . . . . . . : 255.255.0.0
   Default Gateway . . . . . . . . . : fe80::eedd:24ff:fe3d:ced5%3
Ethernet adapter Ethernet:
   Media State . . . . . . . . . . . : Media disconnected
   Connection-specific DNS Suffix  . :
C:\Users\acer>ping -c 169.254.85.31
Access denied. Option -c requires administrative privileges.
C:\Users\acer>ping 169.254.85.31
Pinging 169.254.85.31 with 32 bytes of data:
Reply from 169.254.85.31: bytes=32 time<1ms TTL=128
Reply from 169.254.85.31: bytes=32 time<1ms TTL=128
Reply from 169.254.85.31: bytes=32 time<1ms TTL=128
Reply from 169.254.85.31: bytes=32 time<1ms TTL=128
Ping statistics for 169.254.85.31:
    Packets: Sent = 4, Received = 4, Lost = 0 (0% loss),
Approximate round trip times in milli-seconds:
    Minimum = 0ms, Maximum = 0ms, Average = 0ms
C:\Users\acer>hostname
TMP215-75-G2
C:\Users\acer>getmac
Physical Address    Transport Name
=================== ==========================================================
FC-6D-77-6C-0F-02   \Device\Tcpip_{05DFA269-CEFB-4295-ADCE-7123750CCF35}
74-D4-DD-CF-7C-97   Media disconnected
0A-00-27-00-00-08   \Device\Tcpip_{34D09AB7-968B-4631-A454-3505BE22D0CC}
C:\Users\acer>nslookup google.com
Server:  UnKnown
Address:  2403:8600:c090:42:a000::200
Non-authoritative answer:
Name:    google.com
Addresses:  2404:6800:4007:83c::200e
          172.217.24.110
C:\Users\acer>netstat -an
Active Connections
  Proto  Local Address          Foreign Address        State
  TCP    0.0.0.0:80             0.0.0.0:0              LISTENING
  TCP    0.0.0.0:135            0.0.0.0:0              LISTENING
  TCP    0.0.0.0:445            0.0.0.0:0              LISTENING
  TCP    0.0.0.0:1309           0.0.0.0:0              LISTENING
  TCP    0.0.0.0:4343           0.0.0.0:0              LISTENING
  TCP    0.0.0.0:4449           0.0.0.0:0              LISTENING
  TCP    0.0.0.0:5040           0.0.0.0:0              LISTENING
  TCP    0.0.0.0:5141           0.0.0.0:0              LISTENING
  TCP    0.0.0.0:7680           0.0.0.0:0              LISTENING
  TCP    0.0.0.0:49664          0.0.0.0:0              LISTENING
  TCP    0.0.0.0:49665          0.0.0.0:0              LISTENING
  TCP    0.0.0.0:49666          0.0.0.0:0              LISTENING
  TCP    0.0.0.0:49667          0.0.0.0:0              LISTENING
  TCP    0.0.0.0:49668          0.0.0.0:0              LISTENING
  TCP    0.0.0.0:49672          0.0.0.0:0              LISTENING
  TCP    0.0.0.0:58995          0.0.0.0:0              LISTENING
  TCP    127.0.0.1:4709         0.0.0.0:0              LISTENING
  TCP    127.0.0.1:5141         127.0.0.1:62435        ESTABLISHED
  TCP    127.0.0.1:9993         0.0.0.0:0              LISTENING
  TCP    127.0.0.1:15152        0.0.0.0:0              LISTENING
  TCP    127.0.0.1:19443        0.0.0.0:0              LISTENING
  TCP    127.0.0.1:46753        0.0.0.0:0              LISTENING
  TCP    127.0.0.1:46760        0.0.0.0:0              LISTENING
  TCP    127.0.0.1:46934        0.0.0.0:0              LISTENING
  TCP    127.0.0.1:46935        0.0.0.0:0              LISTENING
  TCP    127.0.0.1:46935        127.0.0.1:54138        ESTABLISHED
  TCP    127.0.0.1:46936        0.0.0.0:0              LISTENING
  TCP    127.0.0.1:46936        127.0.0.1:49683        ESTABLISHED
  TCP    127.0.0.1:46937        0.0.0.0:0              LISTENING
  TCP    127.0.0.1:46937        127.0.0.1:49684        ESTABLISHED
  TCP    127.0.0.1:49669        127.0.0.1:49670        ESTABLISHED
  TCP    127.0.0.1:49670        127.0.0.1:49669        ESTABLISHED
  TCP    127.0.0.1:49675        127.0.0.1:49676        ESTABLISHED
  TCP    127.0.0.1:49676        127.0.0.1:49675        ESTABLISHED
  TCP    127.0.0.1:49677        127.0.0.1:49678        ESTABLISHED
  TCP    127.0.0.1:49678        127.0.0.1:49677        ESTABLISHED
  TCP    127.0.0.1:49679        127.0.0.1:49680        ESTABLISHED
  TCP    127.0.0.1:49680        127.0.0.1:49679        ESTABLISHED
  TCP    127.0.0.1:49681        127.0.0.1:49682        ESTABLISHED
  TCP    127.0.0.1:49682        127.0.0.1:49681        ESTABLISHED
  TCP    127.0.0.1:49683        127.0.0.1:46936        ESTABLISHED
  TCP    127.0.0.1:49684        127.0.0.1:46937        ESTABLISHED
  TCP    127.0.0.1:49685        127.0.0.1:49686        ESTABLISHED
  TCP    127.0.0.1:49686        127.0.0.1:49685        ESTABLISHED
  TCP    127.0.0.1:50494        0.0.0.0:0              LISTENING
  TCP    127.0.0.1:50636        127.0.0.1:58995        ESTABLISHED
  TCP    127.0.0.1:51779        0.0.0.0:0              LISTENING
  TCP    127.0.0.1:51780        0.0.0.0:0              LISTENING
  TCP    127.0.0.1:51781        0.0.0.0:0              LISTENING
  TCP    127.0.0.1:51782        0.0.0.0:0              LISTENING
  TCP    127.0.0.1:52669        127.0.0.1:58995        ESTABLISHED
  TCP    127.0.0.1:54136        127.0.0.1:54137        ESTABLISHED
  TCP    127.0.0.1:54137        127.0.0.1:54136        ESTABLISHED
  TCP    127.0.0.1:54138        127.0.0.1:46935        ESTABLISHED
  TCP    127.0.0.1:54139        127.0.0.1:54140        ESTABLISHED
  TCP    127.0.0.1:54140        127.0.0.1:54139        ESTABLISHED
  TCP    127.0.0.1:54141        127.0.0.1:54142        ESTABLISHED
  TCP    127.0.0.1:54142        127.0.0.1:54141        ESTABLISHED
  TCP    127.0.0.1:58995        127.0.0.1:50636        ESTABLISHED
  TCP    127.0.0.1:58995        127.0.0.1:52669        ESTABLISHED
  TCP    127.0.0.1:58995        127.0.0.1:60870        ESTABLISHED
  TCP    127.0.0.1:60870        127.0.0.1:58995        ESTABLISHED
  TCP    127.0.0.1:62435        127.0.0.1:5141         ESTABLISHED
  TCP    169.254.85.31:139      0.0.0.0:0              LISTENING
  TCP    169.254.85.31:7680     169.254.139.215:55313  ESTABLISHED
  TCP    169.254.85.31:7680     169.254.229.252:61246  TIME_WAIT
  TCP    169.254.85.31:55691    169.254.131.247:7680   SYN_SENT
  TCP    169.254.85.31:55692    169.254.214.26:7680    SYN_SENT
  TCP    169.254.85.31:55693    169.254.70.61:7680     SYN_SENT
  TCP    192.168.56.1:139       0.0.0.0:0              LISTENING
  TCP    [::]:80                [::]:0                 LISTENING
  TCP    [::]:135               [::]:0                 LISTENING
  TCP    [::]:445               [::]:0                 LISTENING
  TCP    [::]:4343              [::]:0                 LISTENING
  TCP    [::]:4449              [::]:0                 LISTENING
  TCP    [::]:5141              [::]:0                 LISTENING
  TCP    [::]:7680              [::]:0                 LISTENING
  TCP    [::]:49664             [::]:0                 LISTENING
  TCP    [::]:49665             [::]:0                 LISTENING
  TCP    [::]:49666             [::]:0                 LISTENING
  TCP    [::]:49667             [::]:0                 LISTENING
  TCP    [::]:49668             [::]:0                 LISTENING
  TCP    [::]:49672             [::]:0                 LISTENING
  TCP    [::]:58995             [::]:0                 LISTENING
  TCP    [::1]:15161            [::]:0                 LISTENING
  TCP    [::1]:15161            [::1]:56287            ESTABLISHED
  TCP    [::1]:15161            [::1]:59566            ESTABLISHED
  TCP    [::1]:15161            [::1]:59567            ESTABLISHED
  TCP    [::1]:56287            [::1]:15161            ESTABLISHED
  TCP    [::1]:59566            [::1]:15161            ESTABLISHED
  TCP    [::1]:59567            [::1]:15161            ESTABLISHED
  TCP    [2403:8600:c090:42:0:400:f0:d5b]:49410  [2603:1040:a06:6::1]:443  
ESTABLISHED
  TCP    [2403:8600:c090:42:0:400:f0:d5b]:49822  [64:ff9b::acbc:9b19]:443  
ESTABLISHED
  TCP    [2403:8600:c090:42:0:400:f0:d5b]:50975  [64:ff9b::8c52:7219]:443  
ESTABLISHED
  TCP    [2403:8600:c090:42:0:400:f0:d5b]:51620  [64:ff9b::a66c:c8af]:443  
TIME_WAIT
  TCP    [2403:8600:c090:42:0:400:f0:d5b]:51772  
[2403:8600:c090:42:a000::300]:443  ESTABLISHED
  TCP    [2403:8600:c090:42:0:400:f0:d5b]:52335  [2606:50c0:8002::154]:443  
ESTABLISHED
  TCP    [2403:8600:c090:42:0:400:f0:d5b]:53176  [2606:50c0:8000::215]:443  
ESTABLISHED
  TCP    [2403:8600:c090:42:0:400:f0:d5b]:53480  [2603:1040:603:c::d6]:443  
ESTABLISHED
  TCP    [2403:8600:c090:42:0:400:f0:d5b]:54109  [2404:6800:4003:c06::bc]:443  
ESTABLISHED
  TCP    [2403:8600:c090:42:0:400:f0:d5b]:54174  [2404:6800:4000:1025::54]:443  
ESTABLISHED
  TCP    [2403:8600:c090:42:0:400:f0:d5b]:54746  [64:ff9b::be5c:c7b2]:443  
CLOSE_WAIT
  TCP    [2403:8600:c090:42:0:400:f0:d5b]:55666  [2404:6800:4000:1025::54]:443  
ESTABLISHED
  TCP    [2403:8600:c090:42:0:400:f0:d5b]:55675  [64:ff9b::a66c:c8af]:443  
ESTABLISHED
  TCP    [2403:8600:c090:42:0:400:f0:d5b]:55676  [64:ff9b::9ce3:e21]:443  
CLOSE_WAIT
  TCP    [2403:8600:c090:42:0:400:f0:d5b]:55677  [2404:6800:4007:804::200e]:443 
ESTABLISHED
  TCP    [2403:8600:c090:42:0:400:f0:d5b]:55678  [2404:6800:4007:804::200e]:443 
ESTABLISHED
  TCP    [2403:8600:c090:42:0:400:f0:d5b]:55686  [64:ff9b::3468:811b]:443  
ESTABLISHED
  TCP    [2403:8600:c090:42:0:400:f0:d5b]:56878  
[2a03:2880:f36a:120:face:b00c:0:167]:443  ESTABLISHED
  TCP    [2403:8600:c090:42:0:400:f0:d5b]:57226  [64:ff9b::a66c:c8af]:443  
CLOSE_WAIT
  TCP    [2403:8600:c090:42:0:400:f0:d5b]:57310  [2603:1047:1:98::80]:443  
ESTABLISHED
  TCP    [2403:8600:c090:42:0:400:f0:d5b]:57351  
[2a03:2880:f36a:120:face:b00c:0:167]:443  ESTABLISHED
  TCP    [2403:8600:c090:42:0:400:f0:d5b]:57762  [64:ff9b::3468:811b]:443  
TIME_WAIT
  TCP    [2403:8600:c090:42:0:400:f0:d5b]:58710  [2a04:4e42:25::347]:443  
ESTABLISHED
  TCP    [2403:8600:c090:42:0:400:f0:d5b]:59066  
[2603:1063:2001:1904::365:ff1]:443  ESTABLISHED
  TCP    [2403:8600:c090:42:0:400:f0:d5b]:59118  [64:ff9b::be5c:c7b2]:443  
CLOSE_WAIT
  TCP    [2403:8600:c090:42:0:400:f0:d5b]:59174  [2606:50c0:8000::215]:443  
ESTABLISHED
  TCP    [2403:8600:c090:42:0:400:f0:d5b]:59571  [2603:1040:a06:6::1]:443  
ESTABLISHED
  TCP    [2403:8600:c090:42:0:400:f0:d5b]:60738  [2606:4700::6812:17de]:443  
ESTABLISHED
  TCP    [2403:8600:c090:42:0:400:f0:d5b]:61356  [2606:4700::6812:1b30]:443  
ESTABLISHED
  TCP    [2403:8600:c090:42:0:400:f0:d5b]:61719  [2606:4700::6812:17de]:443  
ESTABLISHED
  TCP    [2403:8600:c090:42:0:400:f0:d5b]:62802  [2606:4700:20::681a:d25]:443  
ESTABLISHED
  TCP    [2403:8600:c090:42:0:400:f0:d5b]:64095  [64:ff9b::acbc:9b19]:443  
ESTABLISHED
  TCP    [2403:8600:c090:42:0:400:f0:d5b]:64412  [64:ff9b::8c52:7119]:443  
ESTABLISHED
  TCP    [2403:8600:c090:42:0:400:f0:d5b]:64616  [64:ff9b::b9c7:6c85]:443  
ESTABLISHED
  TCP    [2403:8600:c090:42:0:400:f0:d5b]:64797  [2606:50c0:8003::154]:443  
ESTABLISHED
  UDP    0.0.0.0:68             *:*
  UDP    0.0.0.0:5050           *:*
  UDP    0.0.0.0:5353           *:*
  UDP    0.0.0.0:5353           *:*
  UDP    0.0.0.0:5353           *:*
  UDP    0.0.0.0:5353           *:*
  UDP    0.0.0.0:5353           *:*
  UDP    0.0.0.0:5353           *:*
  UDP    0.0.0.0:5353           *:*
  UDP    0.0.0.0:5353           *:*
  UDP    0.0.0.0:5353           *:*
  UDP    0.0.0.0:5353           *:*
  UDP    0.0.0.0:5353           *:*
  UDP    0.0.0.0:5353           *:*
  UDP    0.0.0.0:5353           *:*
  UDP    0.0.0.0:5353           *:*
  UDP    0.0.0.0:5353           *:*
  UDP    0.0.0.0:5353           *:*
  UDP    0.0.0.0:5353           *:*
  UDP    0.0.0.0:5353           *:*
  UDP    0.0.0.0:5353           *:*
  UDP    0.0.0.0:5353           *:*
  UDP    0.0.0.0:5353           *:*
  UDP    0.0.0.0:5355           *:*
  UDP    0.0.0.0:55533          *:*
  UDP    0.0.0.0:58259          *:*
  UDP    0.0.0.0:60865          *:*
  UDP    127.0.0.1:1900         *:*
  UDP    127.0.0.1:58258        *:*
  UDP    127.0.0.1:58666        127.0.0.1:58666
  UDP    127.0.0.1:63691        *:*
  UDP    169.254.85.31:137      *:*
  UDP    169.254.85.31:138      *:*
  UDP    169.254.85.31:1900     *:*
  UDP    169.254.85.31:63690    *:*
  UDP    192.168.56.1:137       *:*
  UDP    192.168.56.1:138       *:*
  UDP    192.168.56.1:1900      *:*
  UDP    192.168.56.1:63689     *:*
  UDP    [::]:5353              *:*
  UDP    [::]:5353              *:*
  UDP    [::]:5353              *:*
  UDP    [::]:5353              *:*
  UDP    [::]:5353              *:*
  UDP    [::]:5353              *:*
  UDP    [::]:5353              *:*
  UDP    [::]:5353              *:*
  UDP    [::]:5353              *:*
  UDP    [::]:5353              *:*
  UDP    [::]:5353              *:*
  UDP    [::]:5355              *:*
  UDP    [::]:55533             *:*
  UDP    [::]:60865             *:*
  UDP    [::1]:1900             *:*
  UDP    [::1]:63688            *:*
  UDP    [fe80::cdd0:4780:c94e:5071%3]:1900  *:*
  UDP    [fe80::cdd0:4780:c94e:5071%3]:63687  *:*
  UDP    [fe80::f105:cb0f:d91e:5471%8]:1900  *:*
  UDP    [fe80::f105:cb0f:d91e:5471%8]:63686  *:*
C:\Users\acer>tracert google.com
Tracing route to google.com [2404:6800:4007:83c::200e]
over a maximum of 30 hops:
  1     1 ms     1 ms     2 ms  2403:8600:c090:42::1
  2     *        *        *     Request timed out.
  3     *        *        *     Request timed out.
  4    34 ms    13 ms    14 ms  lcmaaa-ap-in-x0e.1e100.net 
[2404:6800:4007:83c::200e]
Trace complete.
C:\Users\acer>vnstat -d
'vnstat' is not recognized as an internal or external command,
operable program or batch file.
C:\Users\acer>users
'users' is not recognized as an internal or external command,
operable program or batch file.
C:\Users\acer>nbtstat
Displays protocol statistics and current TCP/IP connections using NBT
(NetBIOS over TCP/IP).
NBTSTAT [ [-a RemoteName] [-A IP address] [-c] [-n]
        [-r] [-R] [-RR] [-s] [-S] [interval] ]
  -a   (adapter status) Lists the remote machine's name table given its name
  -A   (Adapter status) Lists the remote machine's name table given its
                        IP address.
  -c   (cache)          Lists NBT's cache of remote [machine] names and their IP 
addresses
  -n   (names)          Lists local NetBIOS names.
  -r   (resolved)       Lists names resolved by broadcast and via WINS
  -R   (Reload)         Purges and reloads the remote cache name table
  -S   (Sessions)       Lists sessions table with the destination IP addresses
  -s   (sessions)       Lists sessions table converting destination IP
                        addresses to computer NETBIOS names.
  -RR  (ReleaseRefresh) Sends Name Release packets to WINS and then, starts 
Refresh
  RemoteName   Remote host machine name.
  IP address   Dotted decimal representation of the IP address.
  interval     Redisplays selected statistics, pausing interval seconds
               between each display. Press Ctrl+C to stop redisplaying
               statistics.
C:\Users\acer>systeminfo
Host Name:                     TMP215-75-G2
OS Name:                       Microsoft Windows 11 Home Single Language
OS Version:                    10.0.26200 N/A Build 26200
OS Manufacturer:               Microsoft Corporation
OS Configuration:              Standalone Workstation
OS Build Type:                 Multiprocessor Free
Registered Owner:              acer
Registered Organization:       N/A
Product ID:                    00342-42784-66138-AAOEM
Original Install Date:         01-09-2025, 15:21:05
System Boot Time:              18-08-2026, 13:01:41
System Manufacturer:           Acer
System Model:                  TravelMate P215-75-G2-TCO
System Type:                   x64-based PC
Processor(s):                  1 Processor(s) Installed.
                               [01]: Intel64 Family 6 Model 170 Stepping 4 
GenuineIntel ~1200 Mhz
BIOS Version:                  INSYDE Corp. V1.05tt01a, 01-09-2025
Windows Directory:             C:\Windows
System Directory:              C:\Windows\system32
Boot Device:                   \Device\HarddiskVolume1
System Locale:                 en-us;English (United States)
Input Locale:                  00004009
Time Zone:                     (UTC+05:30) Chennai, Kolkata, Mumbai, New Delhi
Total Physical Memory:         15,869 MB
Available Physical Memory:     2,676 MB
Virtual Memory: Max Size:      28,157 MB
Virtual Memory: Available:     11,398 MB
Virtual Memory: In Use:        16,759 MB
Page File Location(s):         C:\pagefile.sys
Domain:                        WORKGROUP
Logon Server:                  \\TMP215-75-G2
Hotfix(s):                     5 Hotfix(s) Installed.
                               [01]: KB5120708
                               [02]: KB5054156
                               [03]: KB5121003
                               [04]: KB5120102
                               [05]: KB5123304
Network Card(s):               3 NIC(s) Installed.
                               [01]: Intel(R) Wi-Fi 6E AX211 160MHz
                                     Connection Name: Wi-Fi
                                     DHCP Enabled:    Yes
                                     DHCP Server:     255.255.255.255
                                     IP address(es)
                                     [01]: 169.254.85.31
                                     [02]: fe80::cdd0:4780:c94e:5071
                                     [03]: 2403:8600:c090:42:0:400:f0:d5b
                               [02]: Realtek PCIe GbE Family Controller
                                     Connection Name: Ethernet
                                     Status:          Media disconnected
                               [03]: VirtualBox Host-Only Ethernet Adapter
                                     Connection Name: Ethernet 2
                                     DHCP Enabled:    No
                                     IP address(es)
                                     [01]: 192.168.56.1
                                     [02]: fe80::f105:cb0f:d91e:5471
Virtualization-based security: Status: Running
                               Required Security Properties:
                                     Base Virtualization Support
                               Available Security Properties:
                                     Base Virtualization Support
                                     Secure Boot
                                     DMA Protection
                                     UEFI Code Readonly
                                     SMM Security Mitigations 1.0
                                     Mode Based Execution Control
                                     APIC Virtualization
                               Services Configured:
                                     Hypervisor enforced Code Integrity
                               Services Running:
                                     Hypervisor enforced Code Integrity
                               App Control for Business policy: Enforced
                               App Control for Business user mode policy: 
Enforced
                               Security Features Enabled:
Hyper-V Requirements:          A hypervisor has been detected. Features required 
for Hyper-V will not be displayed.

```



## Output

## Result
Thus Execution of Network commands Performed 
