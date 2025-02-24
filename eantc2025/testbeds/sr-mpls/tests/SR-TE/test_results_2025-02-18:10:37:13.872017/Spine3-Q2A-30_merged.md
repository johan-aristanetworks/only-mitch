# Test results for Spine3-Q2A-30

## show version

```text
Arista DCS-7280SR3E-40YC6-F
Hardware version: 11.00
Serial number: SGD22060176
Hardware MAC address: c4ca.2b45.a215
System MAC address: c4ca.2b45.a215

Software image version: 4.33.1.1F
Architecture: x86_64
Internal build version: 4.33.1.1F-40155285.43311F
Internal build ID: 2170da2c-90c5-421e-adc1-86266708cffc
Image format version: 3.0
Image optimization: Default

Uptime: 1 day, 3 hours and 44 minutes
Total memory: 8099700 kB
Free memory: 5113396 kB

```

## show lldp neighbors

```text
Last table change time   : 0:09:20 ago
Number of table inserts  : 91
Number of table deletes  : 77
Number of table drops    : 0
Number of table age-outs : 1

Port      Neighbor Device ID                    Neighbor Port ID            TTL
------- ------------------------------------- ----------------------------- ---
Et2       Arista-PE32-Q2C-32.ns.eantc.de        Ethernet1                   120
Et3       H3C_M1A_120                           Ten-GigabitEthernet0/0/17   121
Et4       Nokia-SR1-217                         1610899524                  121
Et5       Nokia-SXR-214                         ethernet-1/4                120
Et9       Ciena-5134-72                         2                           120
Et12      Ericsson_84_R6678                     5870.7f9f.c403              91 
Et13      Arrcus-53                             swp0                        120
Et15      30c5.0784.3e68                        et-bs/15                    121
Et17      Huawei_124_NetEngine_A816             GigabitEthernet0/2/4        120
Et19      Huawei_128_NetEngine_8000_M14         GigabitEthernet0/5/0        120
Et31      Ciena-8140-66                         2                           120
Et36      Arista-Harness3-JP-39.ns.eantc.de     Ethernet6                   120
Et40      Juniper-179-ACX7024                   523                         120
Ma1       extreme-x460-2                        5                           120

```

## show mac address-table

```text
          Mac Address Table
------------------------------------------------------------------

Vlan    Mac Address       Type        Ports      Moves   Last Move
----    -----------       ----        -----      -----   ---------
Total Mac Addresses for this criterion: 0

          Multicast Mac Address Table
------------------------------------------------------------------

Vlan    Mac Address       Type        Ports
----    -----------       ----        -----
Total Mac Addresses for this criterion: 0
```

## show ip interface brief | exclude una

```text
                                                                        Address
Interface       IP Address          Status     Protocol           MTU   Owner  
--------------- ------------------- ---------- -------------- --------- -------
Ethernet1       20.30.31.30/24      down       down              1500          
Ethernet2       20.30.32.30/24      up         up                1500          
Ethernet3       20.30.120.30/24     up         up                1500          
Ethernet4       20.30.217.30/24     up         up                1500          
Ethernet5       20.30.214.30/24     up         up                1500          
Ethernet7       20.30.184.30/24     up         up                1500          
Ethernet9       20.30.72.30/24      up         up                1500          
Ethernet12      20.30.84.30/24      up         up                1500          
Ethernet13      20.30.53.30/24      up         up                1500          
Ethernet15      20.30.221.30/24     up         up                1500          
Ethernet17      20.30.124.30/24     up         up                1500          
Ethernet19      20.30.128.30/24     up         up                1500          
Ethernet31      20.30.66.30/24      up         up                1500          
Ethernet40      20.30.179.30/24     up         up                1500          
Loopback0       10.0.0.30/32        up         up               65535          
Loopback5001    10.0.0.30/32        up         up               65535          
Management1     192.168.20.30/23    up         up                1500          

```

## show interfaces counters rates | nz

```text
Port      Name                 Intvl  In Mbps      %  In Kpps Out Mbps      %
Et9       Ciena-5134-72 port 2  0:01      0.0   0.0%        0      0.0   0.0%
Et31      Ciena-8140-66 port 2  0:01      0.0   0.0%        0      0.0   0.0%

Port      Out Kpps
```

## show isis neighbors

```text
 
Instance  VRF      System Id        Type Interface          SNPA              State Hold time   Circuit Id          
IGP       default  Arista-PE32-Q2C-32 L2   Ethernet2          P2P               UP    22          44                  
IGP       default  Arrcus-53        L2   Ethernet13         P2P               UP    30          00                  
IGP       default  Ciena-5134-72    L2   Ethernet9          P2P               UP    22          02                  
IGP       default  Ericsson_84_R6678 L2   Ethernet12         P2P               UP    22          02                  
IGP       default  H3C_M1A_120      L2   Ethernet3          P2P               UP    28          01                  
IGP       default  0000.0000.0124   L2   Ethernet17         P2P               UP    27          09                  
IGP       default  0000.0000.0128   L2   Ethernet19         P2P               UP    30          09                  
IGP       default  Juniper-179-ACX7024 L2   Ethernet40         P2P               UP    26          01                  
IGP       default  Nokia-SXR-214    L2   Ethernet5          P2P               UP    24          00                  
IGP       default  Nokia-SR1-217    L2   Ethernet4          P2P               UP    19          00                  
IGP       default  221              L2   Ethernet15         P2P               UP    67          00                  
```

## show isis database detail

```text
Legend:
H - hostname conflict
U - node unreachable

IS-IS Instance: IGP VRF: default
  IS-IS Level 2 Link State Database
    LSPID                   Seq Num  Cksum  Life Length IS  Received LSPID        Flags
    Arista-Spine3-Q2A-30.00-00       341  58231   711   1054 L2  0000.0000.0030.00-00  <>
      LSP generation remaining wait time: 0 ms
      Time remaining until refresh: 411 s
      NLPID: 0xCC(IPv4) 0x8E(IPv6)
      Hostname: Arista-Spine3-Q2A-30
      Area addresses: 49.0001
      Topology: 2 (IPv6)
      Topology: 0 (IPv4)
      Interface address: 20.30.214.30
      Interface address: 20.30.32.30
      Interface address: 20.30.217.30
      Interface address: 20.30.179.30
      Interface address: 20.30.128.30
      Interface address: 20.30.120.30
      Interface address: 20.30.84.30
      Interface address: 20.30.66.30
      Interface address: 20.30.53.30
      Interface address: 20.30.221.30
      Interface address: 20.30.72.30
      Interface address: 20.30.184.30
      Interface address: 20.30.124.30
      Interface address: 10.0.0.30
      Interface address: 2001:0:30:214::30
      Interface address: 2001:0:30:32::30
      Interface address: 2001:0:30:217::30
      Interface address: 2001:0:30:179::30
      Interface address: 2001:0:30:128::30
      Interface address: 2001:0:30:120::30
      Interface address: 2001:0:30:84::30
      Interface address: 2001:0:30:66::30
      Interface address: 2001:0:53:120::30
      Interface address: 2001:0:30:221::30
      Interface address: 2001:0:30:72::30
      Interface address: 2001:0:30:184::30
      Interface address: 2001:0:30:124::30
      IS Neighbor          : 0000.0000.0124.00   Metric: 10
        IPv4 Neighbor Address: 20.30.124.124
        IPv4 Interface Address: 20.30.124.30
        Adj-sid: 362175 flags: [L V] weight: 0x0
      IS Neighbor          : 0000.0000.0128.00   Metric: 10
        IPv4 Neighbor Address: 20.30.128.128
        IPv4 Interface Address: 20.30.128.30
        Adj-sid: 362174 flags: [L V] weight: 0x0
      IS Neighbor          : Ciena-5134-72.00    Metric: 10
        IPv4 Neighbor Address: 20.30.72.72
        IPv4 Interface Address: 20.30.72.30
        Adj-sid: 362161 flags: [L V] weight: 0x0
      IS Neighbor          : 221.00              Metric: 10
        IPv4 Neighbor Address: 20.30.221.221
        IPv4 Interface Address: 20.30.221.30
        Adj-sid: 362160 flags: [L V] weight: 0x0
      IS Neighbor          : Juniper-179-ACX7024.00 Metric: 10
        IPv4 Neighbor Address: 20.30.179.179
        IPv4 Interface Address: 20.30.179.30
        Adj-sid: 362168 flags: [L V] weight: 0x0
      IS Neighbor          : Nokia-SXR-214.00    Metric: 10
        IPv4 Neighbor Address: 20.30.214.214
        IPv4 Interface Address: 20.30.214.30
        Adj-sid: 362166 flags: [L V] weight: 0x0
      IS Neighbor          : Arista-PE32-Q2C-32.00 Metric: 10
        IPv4 Neighbor Address: 20.30.32.32
        IPv4 Interface Address: 20.30.32.30
        Adj-sid: 362159 flags: [L V] weight: 0x0
      IS Neighbor          : H3C_M1A_120.00      Metric: 10
        IPv4 Neighbor Address: 20.30.120.120
        IPv4 Interface Address: 20.30.120.30
        Adj-sid: 362162 flags: [L V] weight: 0x0
      IS Neighbor          : Nokia-SR1-217.00    Metric: 10
        IPv4 Neighbor Address: 20.30.217.217
        IPv4 Interface Address: 20.30.217.30
        Adj-sid: 362171 flags: [L V] weight: 0x0
      IS Neighbor          : Arrcus-53.00        Metric: 10
        IPv4 Neighbor Address: 20.30.53.53
        IPv4 Interface Address: 20.30.53.30
        Adj-sid: 362165 flags: [L V] weight: 0x0
      IS Neighbor          : Ericsson_84_R6678.00 Metric: 10
        IPv4 Neighbor Address: 20.30.84.84
        IPv4 Interface Address: 20.30.84.30
        Adj-sid: 362167 flags: [L V] weight: 0x0
      IS Neighbor (MT-IPv6): Arista-PE32-Q2C-32.00 Metric: 10
        Adj-sid: 362169 flags: [L V F] weight: 0x0
      IS Neighbor (MT-IPv6): H3C_M1A_120.00      Metric: 10
        Adj-sid: 362163 flags: [L V F] weight: 0x0
      Reachability         : 20.30.214.0/24 Metric: 10 Type: 1 Up
      Reachability         : 20.30.32.0/24 Metric: 10 Type: 1 Up
      Reachability         : 20.30.217.0/24 Metric: 10 Type: 1 Up
      Reachability         : 20.30.179.0/24 Metric: 10 Type: 1 Up
      Reachability         : 20.30.128.0/24 Metric: 10 Type: 1 Up
      Reachability         : 20.30.120.0/24 Metric: 10 Type: 1 Up
      Reachability         : 20.30.84.0/24 Metric: 10 Type: 1 Up
      Reachability         : 20.30.66.0/24 Metric: 10 Type: 1 Up
      Reachability         : 20.30.53.0/24 Metric: 10 Type: 1 Up
      Reachability         : 20.30.221.0/24 Metric: 10 Type: 1 Up
      Reachability         : 20.30.72.0/24 Metric: 10 Type: 1 Up
      Reachability         : 20.30.184.0/24 Metric: 10 Type: 1 Up
      Reachability         : 20.30.124.0/24 Metric: 10 Type: 1 Up
      Reachability         : 10.0.0.30/32 Metric: 0 Type: 1 Up
        SR Prefix-SID: 30 Flags: [N] Algorithm: 0
      Reachability (MT-IPv6): 2001:0:30:214::/64 Metric: 10 Type: 1 Up
      Reachability (MT-IPv6): 2001:0:30:32::/64 Metric: 10 Type: 1 Up
      Reachability (MT-IPv6): 2001:0:30:217::/64 Metric: 10 Type: 1 Up
      Reachability (MT-IPv6): 2001:0:30:179::/64 Metric: 10 Type: 1 Up
      Reachability (MT-IPv6): 2001:0:30:128::/64 Metric: 10 Type: 1 Up
      Reachability (MT-IPv6): 2001:0:30:120::/64 Metric: 10 Type: 1 Up
      Reachability (MT-IPv6): 2001:0:30:84::/64 Metric: 10 Type: 1 Up
      Reachability (MT-IPv6): 2001:0:30:66::/64 Metric: 10 Type: 1 Up
      Reachability (MT-IPv6): 2001:0:53:120::/64 Metric: 10 Type: 1 Up
      Reachability (MT-IPv6): 2001:0:30:221::/64 Metric: 10 Type: 1 Up
      Reachability (MT-IPv6): 2001:0:30:72::/64 Metric: 10 Type: 1 Up
      Reachability (MT-IPv6): 2001:0:30:184::/64 Metric: 10 Type: 1 Up
      Reachability (MT-IPv6): 2001:0:30:124::/64 Metric: 10 Type: 1 Up
      Router Capabilities: Router Id: 10.0.0.30 Flags: []
        SR Local Block:
          SRLB Base: 965536 Range: 65536
        Area leader priority: 250 algorithm: 0
        Maximum SID depth:
          Base MPLS imposition (MSD type 1):  12
        SR Capability: Flags: [I V]
          SRGB Base: 20000 Range: 2000
    Arista-PE32-Q2C-32.00-00        20  40455   998    300 L2  0000.0000.0032.00-00  <>
      Remaining lifetime received: 1199 s Modified to: 1200 s
      NLPID: 0xCC(IPv4) 0x8E(IPv6)
      Hostname: Arista-PE32-Q2C-32
      Area addresses: 49.0001
      Topology: 2 (IPv6)
      Topology: 0 (IPv4)
      Interface address: 20.32.175.32
      Interface address: 10.0.0.32
      Interface address: 20.30.32.32
      Interface address: 2001:0:32:175::32
      Interface address: 2001:0:30:32::32
      IS Neighbor          : Juniper-175-ACX7100-48L.00 Metric: 10
        IPv4 Neighbor Address: 20.32.175.175
        IPv4 Interface Address: 20.32.175.32
        Adj-sid: 362151 flags: [L V] weight: 0x0
      IS Neighbor          : Arista-Spine3-Q2A-30.00 Metric: 10
        IPv4 Neighbor Address: 20.30.32.30
        IPv4 Interface Address: 20.30.32.32
        Adj-sid: 362149 flags: [L V] weight: 0x0
      IS Neighbor (MT-IPv6): Arista-Spine3-Q2A-30.00 Metric: 10
        Adj-sid: 362150 flags: [L V F] weight: 0x0
      Reachability         : 20.32.175.0/24 Metric: 10 Type: 1 Up
      Reachability         : 10.0.0.32/32 Metric: 0 Type: 1 Up
        SR Prefix-SID: 32 Flags: [N] Algorithm: 0
      Reachability         : 20.30.32.0/24 Metric: 10 Type: 1 Up
      Reachability (MT-IPv6): 2001:0:32:175::/64 Metric: 10 Type: 1 Up
      Reachability (MT-IPv6): 2001:0:30:32::/64 Metric: 10 Type: 1 Up
      Router Capabilities: Router Id: 10.0.0.32 Flags: []
        SR Local Block:
          SRLB Base: 965536 Range: 65536
        Area leader priority: 250 algorithm: 0
        Maximum SID depth:
          Base MPLS imposition (MSD type 1):  12
        SR Capability: Flags: [I V]
          SRGB Base: 20000 Range: 2000
    Arrcus-53.00-00             172  31376  1031    175 L2  0000.0000.0053.00-00  <>
      Remaining lifetime received: 1199 s Modified to: 1200 s
      NLPID: 0xCC(IPv4)
      Hostname: Arrcus-53
      Area addresses: 49.0001
      Interface address: 10.0.0.53
      IS Neighbor          : Arista-Spine3-Q2A-30.00 Metric: 10
        IPv4 Neighbor Address: 20.30.53.30
        IPv4 Interface Address: 20.30.53.53
      IS Neighbor          : Juniper-175-ACX7100-48L.00 Metric: 10
        IPv4 Neighbor Address: 20.53.175.175
        IPv4 Interface Address: 20.53.175.53
      Reachability         : 20.30.53.0/24 Metric: 10 Type: 1 Up
      Reachability         : 20.53.175.0/24 Metric: 10 Type: 1 Up
      Reachability         : 10.0.0.53/32 Metric: 0 Type: 1 Up
        SR Prefix-SID: 53 Flags: [N P E] Algorithm: 0
      Router Capabilities: Router Id: 10.0.0.53 Flags: []
        SR Capability: Flags: [I V]
          SRGB Base: 20000 Range: 2000
        Algorithms:  0
 U  Ciena-8140-66.00-00           9  61682   187    308 L2  0000.0000.0066.00-00  <>
      Remaining lifetime received: 1199 s Modified to: 1200 s
      NLPID: 0xCC(IPv4)
      Hostname: Ciena-8140-66
      Area addresses: 49.0001
      Topology: 0 (IPv4)
      Interface address: 10.0.0.66
      IS Neighbor          : Juniper-175-ACX7100-48L.00 Metric: 10
        IPv4 Neighbor Address: 20.66.175.175
        IPv4 Interface Address: 20.66.175.66
        Adj-sid: 16003 flags: [L V] weight: 0x0
      IS Neighbor          : Arista-Spine3-Q2A-30.00 Metric: 10
        IPv4 Neighbor Address: 20.30.66.30
        IPv4 Interface Address: 20.30.66.66
        Adj-sid: 16002 flags: [L V] weight: 0x0
      Reachability         : 20.66.175.0/24 Metric: 10 Type: 1 Up
      Reachability         : 20.30.66.0/24 Metric: 10 Type: 1 Up
      Reachability         : 10.0.0.66/32 Metric: 10 Type: 1 Up
        SR Prefix-SID: 66 Flags: [N] Algorithm: 0
      Router Capabilities: Router Id: 10.0.0.66 Flags: []
        SR Capability: Flags: [I]
          SRGB Base: 20000 Range: 2000
        Algorithms:  0
    Ciena-5134-72.00-00          11   9847  1092    308 L2  0000.0000.0072.00-00  <>
      Remaining lifetime received: 1199 s Modified to: 1200 s
      NLPID: 0xCC(IPv4)
      Hostname: Ciena-5134-72
      Area addresses: 49.0001
      Topology: 0 (IPv4)
      Interface address: 10.0.0.72
      IS Neighbor          : Juniper-175-ACX7100-48L.00 Metric: 10
        IPv4 Neighbor Address: 20.72.175.175
        IPv4 Interface Address: 20.72.175.72
        Adj-sid: 16002 flags: [L V] weight: 0x0
      IS Neighbor          : Arista-Spine3-Q2A-30.00 Metric: 10
        IPv4 Neighbor Address: 20.30.72.30
        IPv4 Interface Address: 20.30.72.72
        Adj-sid: 16003 flags: [L V] weight: 0x0
      Reachability         : 20.72.175.0/24 Metric: 10 Type: 1 Up
      Reachability         : 20.30.72.0/24 Metric: 10 Type: 1 Up
      Reachability         : 10.0.0.72/32 Metric: 10 Type: 1 Up
        SR Prefix-SID: 72 Flags: [N] Algorithm: 0
      Router Capabilities: Router Id: 10.0.0.72 Flags: []
        SR Capability: Flags: [I]
          SRGB Base: 20000 Range: 2000
        Algorithms:  0
    Ericsson_84_R6678.00-00       138  20225   385    204 L2  0000.0000.0084.00-00  <>
      Remaining lifetime received: 1199 s Modified to: 1200 s
      NLPID: 0xCC(IPv4) 0x8E(IPv6)
      Hostname: Ericsson_84_R6678
      Area addresses: 49.0001
      Topology: 0 (IPv4)
      Topology: 2 (IPv6)
      Interface address: 10.0.0.84
      Interface address: 2001:0:30:84::175
      IS Neighbor          : Arista-Spine3-Q2A-30.00 Metric: 10
        IPv4 Interface Address: 20.30.84.84
      IS Neighbor          : Juniper-175-ACX7100-48L.00 Metric: 10
        IPv4 Interface Address: 20.84.175.84
      Reachability         : 10.0.0.84/32 Metric: 10 Type: 1 Up
        SR Prefix-SID: 84 Flags: [N P] Algorithm: 0
      Reachability (MT-IPv6): 2001:0:84:175::/64 Metric: 10 Type: 1 Up
      Router Capabilities: Router Id: 10.0.0.84 Flags: []
        Maximum SID depth:
          Base MPLS imposition (MSD type 1):  8
        SR Capability: Flags: [I]
          SRGB Base: 20000 Range: 2000
        Algorithms:  0
    H3C_M1A_120.00-00           203  10995  1187    269 L2  0000.0000.0120.00-00  <>
      Remaining lifetime received: 1199 s Modified to: 1200 s
      NLPID: 0xCC(IPv4) 0x8E(IPv6)
      Hostname: H3C_M1A_120
      Area addresses: 49.0001
      Topology: 0 (IPv4)
      Topology: 2 (IPv6)
      Interface address: 10.0.0.120
      Interface address: 20.30.120.120
      Interface address: 20.120.214.120
      Interface address: 2001:0:30:120::120
      Interface address: 2001:0:120:214::120
      IS Neighbor          : Arista-Spine3-Q2A-30.00 Metric: 10
        IPv4 Neighbor Address: 20.30.120.30
        IPv4 Interface Address: 20.30.120.120
        Adj-sid: 1149 flags: [L V] weight: 0x0
      IS Neighbor (MT-IPv6): Arista-Spine3-Q2A-30.00 Metric: 10
      Reachability         : 10.0.0.120/32 Metric: 0 Type: 1 Up
        SR Prefix-SID: 120 Flags: [N] Algorithm: 0
      Reachability         : 20.30.120.0/24 Metric: 10 Type: 1 Up
      Reachability         : 20.120.214.0/24 Metric: 10 Type: 1 Up
      Reachability (MT-IPv6): 2001:0:30:120::/64 Metric: 10 Type: 1 Up
      Reachability (MT-IPv6): 2001:0:120:214::/64 Metric: 10 Type: 1 Up
      Router Capabilities: Router Id: 10.0.0.120 Flags: []
        Maximum SID depth:
          Base MPLS imposition (MSD type 1):  13
        SR Capability: Flags: [I]
          SRGB Base: 20000 Range: 2000
    0000.0000.0124.00-00         16  37935  1104    268 L2  0000.0000.0124.00-00  <>
      Remaining lifetime received: 1199 s Modified to: 1200 s
      NLPID: 0xCC(IPv4)
      Area addresses: 49.0001
      Interface address: 20.124.175.124
      Interface address: 20.30.124.124
      IS Neighbor          : Juniper-175-ACX7100-48L.00 Metric: 10
        IPv4 Neighbor Address: 20.124.175.175
        IPv4 Interface Address: 20.124.175.124
        Adj-sid: 394 flags: [L V] weight: 0x0
      IS Neighbor          : Arista-Spine3-Q2A-30.00 Metric: 10
        IPv4 Neighbor Address: 20.30.124.30
        IPv4 Interface Address: 20.30.124.124
        Adj-sid: 395 flags: [L V] weight: 0x0
      Reachability         : 20.124.175.0/24 Metric: 10 Type: 1 Up
      Reachability         : 20.30.124.0/24 Metric: 10 Type: 1 Up
      Router Capabilities: Router Id: 10.0.0.124 Flags: []
        Maximum SID depth:
          Base MPLS imposition (MSD type 1):  10
        SR Capability: Flags: [I]
          SRGB Base: 2000 Range: 2001
    0000.0000.0128.00-00         20  22209  1124    290 L2  0000.0000.0128.00-00  <>
      Remaining lifetime received: 1199 s Modified to: 1200 s
      NLPID: 0xCC(IPv4)
      Area addresses: 49.0001
      Interface address: 10.0.0.128
      Interface address: 20.30.128.128
      Interface address: 20.128.175.128
      IS Neighbor          : Arista-Spine3-Q2A-30.00 Metric: 10
        IPv4 Neighbor Address: 20.30.128.30
        IPv4 Interface Address: 20.30.128.128
        Adj-sid: 48122 flags: [L V] weight: 0x0
      IS Neighbor          : Juniper-175-ACX7100-48L.00 Metric: 10
        IPv4 Neighbor Address: 20.128.175.175
        IPv4 Interface Address: 20.128.175.128
        Adj-sid: 48123 flags: [L V] weight: 0x0
      Reachability         : 10.0.0.128/32 Metric: 0 Type: 1 Up
        SR Prefix-SID: 128 Flags: [N] Algorithm: 0
      Reachability         : 20.30.128.0/24 Metric: 10 Type: 1 Up
      Reachability         : 20.128.175.0/24 Metric: 10 Type: 1 Up
      Router Capabilities: Router Id: 10.0.0.128 Flags: []
        Maximum SID depth:
          Base MPLS imposition (MSD type 1):  10
        SR Capability: Flags: [I]
          SRGB Base: 20000 Range: 2000
    Juniper-175-ACX7100-48L.00-00        18  15373   987   1180 L2  0000.0000.0175.00-00  <>
      Remaining lifetime received: 1198 s Modified to: 1200 s
      NLPID: 0xCC(IPv4) 0x8E(IPv6)
      Hostname: Juniper-175-ACX7100-48L
      Area addresses: 49.0001
      Interface address: 10.0.0.175
      Interface address: 2001:0:32:175::175
      IS Neighbor          : Nokia-SR1-217.00    Metric: 10
        IPv4 Neighbor Address: 20.175.217.217
        IPv4 Interface Address: 20.175.217.175
        IPv6 Neighbor Address: 2001:0:175:217::217
        Global IPv6 Interface Address: 2001:0:175:217::175
        Adj-sid: 62 flags: [L V F] weight: 0x0
        Adj-sid: 61 flags: [L V] weight: 0x0
      IS Neighbor          : 221.00              Metric: 10
        IPv4 Neighbor Address: 20.175.221.221
        IPv4 Interface Address: 20.175.221.175
        Global IPv6 Interface Address: 2001:0:175:221::175
        Adj-sid: 68 flags: [L V F] weight: 0x0
        Adj-sid: 67 flags: [L V] weight: 0x0
      IS Neighbor          : Ericsson_84_R6678.00 Metric: 10
        IPv4 Neighbor Address: 20.84.175.84
        IPv4 Interface Address: 20.84.175.175
        IPv6 Neighbor Address: 2001:0:84:175::175
        Global IPv6 Interface Address: 2001:0:84:175::175
        Adj-sid: 60 flags: [L V F] weight: 0x0
        Adj-sid: 59 flags: [L V] weight: 0x0
      IS Neighbor          : Nokia-SXR-214.00    Metric: 10
        IPv4 Neighbor Address: 20.175.214.214
        IPv4 Interface Address: 20.175.214.175
        Global IPv6 Interface Address: 2001:0:175:214::175
        Adj-sid: 66 flags: [L V F] weight: 0x0
        Adj-sid: 65 flags: [L V] weight: 0x0
      IS Neighbor          : Juniper-179-ACX7024.00 Metric: 10
        IPv4 Neighbor Address: 20.175.179.179
        IPv4 Interface Address: 20.175.179.175
        IPv6 Neighbor Address: 2001:0:175::179:179
        Global IPv6 Interface Address: 2001:0:175::179:175
        Adj-sid: 64 flags: [L V F] weight: 0x0
        Adj-sid: 63 flags: [L V] weight: 0x0
      IS Neighbor          : Arrcus-53.00        Metric: 10
        IPv4 Neighbor Address: 20.53.175.53
        IPv4 Interface Address: 20.53.175.175
        Global IPv6 Interface Address: 2001:0:53:175::175
        Adj-sid: 58 flags: [L V] weight: 0x0
      IS Neighbor          : Ciena-5134-72.00    Metric: 10
        IPv4 Neighbor Address: 20.72.175.72
        IPv4 Interface Address: 20.72.175.175
        Global IPv6 Interface Address: 2001:0:72:175::175
        Adj-sid: 70 flags: [L V] weight: 0x0
      IS Neighbor          : 0000.0000.0124.00   Metric: 10
        IPv4 Neighbor Address: 20.124.175.124
        IPv4 Interface Address: 20.124.175.175
        Adj-sid: 71 flags: [L V] weight: 0x0
      IS Neighbor          : 0000.0000.0128.00   Metric: 10
        IPv4 Neighbor Address: 20.128.175.128
        IPv4 Interface Address: 20.128.175.175
        Global IPv6 Interface Address: 2001:0:128:175::175
        Adj-sid: 72 flags: [L V] weight: 0x0
      IS Neighbor          : Arista-PE32-Q2C-32.00 Metric: 10
        IPv4 Neighbor Address: 20.32.175.32
        IPv4 Interface Address: 20.32.175.175
        Global IPv6 Interface Address: 2001:0:32:175::175
        Adj-sid: 74 flags: [L V F] weight: 0x0
        Adj-sid: 73 flags: [L V] weight: 0x0
      Reachability         : 20.131.175.0/24 Metric: 10 Type: 1 Up
      Reachability         : 20.175.217.0/24 Metric: 10 Type: 1 Up
      Reachability         : 20.175.221.0/24 Metric: 10 Type: 1 Up
      Reachability         : 20.84.175.0/24 Metric: 10 Type: 1 Up
      Reachability         : 20.128.175.0/24 Metric: 10 Type: 1 Up
      Reachability         : 20.175.184.0/24 Metric: 10 Type: 1 Up
      Reachability         : 20.124.175.0/24 Metric: 10 Type: 1 Up
      Reachability         : 20.175.214.0/24 Metric: 10 Type: 1 Up
      Reachability         : 20.32.175.0/24 Metric: 10 Type: 1 Up
      Reachability         : 20.72.175.0/24 Metric: 10 Type: 1 Up
      Reachability         : 20.66.175.0/24 Metric: 10 Type: 1 Up
      Reachability         : 20.175.179.0/24 Metric: 10 Type: 1 Up
      Reachability         : 20.120.175.0/24 Metric: 10 Type: 1 Up
      Reachability         : 20.53.175.0/24 Metric: 10 Type: 1 Up
      Reachability         : 10.0.0.175/32 Metric: 0 Type: 1 Up
        SR Prefix-SID: 175 Flags: [N] Algorithm: 0
      Reachability          : 2001:0:131:175::/64 Metric: 10 Type: 1 Up
      Reachability          : 2001:0:175:217::/64 Metric: 10 Type: 1 Up
      Reachability          : 2001:0:175:221::/64 Metric: 10 Type: 1 Up
      Reachability          : 2001:0:84:175::/64 Metric: 10 Type: 1 Up
      Reachability          : 2001:0:128:175::/64 Metric: 10 Type: 1 Up
      Reachability          : 2001:0:175:184::/64 Metric: 10 Type: 1 Up
      Reachability          : 2001:0:175:214::/64 Metric: 10 Type: 1 Up
      Reachability          : 2001:0:32:175::/64 Metric: 10 Type: 1 Up
      Reachability          : 2001:0:72:175::/64 Metric: 10 Type: 1 Up
      Reachability          : 2001:0:66:175::/64 Metric: 10 Type: 1 Up
      Reachability          : 2001:0:175::/64 Metric: 10 Type: 1 Up
      Reachability          : 2001:0:120:175::/64 Metric: 10 Type: 1 Up
      Reachability          : 2001:0:53:175::/64 Metric: 10 Type: 1 Up
      Router Capabilities: Router Id: 10.0.0.175 Flags: []
        Maximum SID depth:
          Base MPLS imposition (MSD type 1):  3
        SR Capability: Flags: [I V]
          SRGB Base: 20000 Range: 2000
        Algorithms:  0, 1
      Unsupported TLV: Type: 14 Length: 2
    Juniper-179-ACX7024.00-00         6  55520   696    380 L2  0000.0000.0179.00-00  <>
      Remaining lifetime received: 1198 s Modified to: 1200 s
      NLPID: 0xCC(IPv4) 0x8E(IPv6)
      Hostname: Juniper-179-ACX7024
      Area addresses: 49.0001
      Interface address: 10.0.0.179
      Interface address: 2001:0:30:179::179
      IS Neighbor          : Juniper-175-ACX7100-48L.00 Metric: 10
        IPv4 Neighbor Address: 20.175.179.175
        IPv4 Interface Address: 20.175.179.179
        IPv6 Neighbor Address: 2001:0:175::179:175
        Global IPv6 Interface Address: 2001:0:175::179:179
        Adj-sid: 21 flags: [L V F] weight: 0x0
        Adj-sid: 20 flags: [L V] weight: 0x0
      IS Neighbor          : Arista-Spine3-Q2A-30.00 Metric: 10
        IPv4 Neighbor Address: 20.30.179.30
        IPv4 Interface Address: 20.30.179.179
        Global IPv6 Interface Address: 2001:0:30:179::179
        Adj-sid: 19 flags: [L V F] weight: 0x0
        Adj-sid: 18 flags: [L V] weight: 0x0
      Reachability         : 20.175.179.0/24 Metric: 10 Type: 1 Up
      Reachability         : 20.30.179.0/24 Metric: 10 Type: 1 Up
      Reachability         : 10.0.0.179/32 Metric: 0 Type: 1 Up
        SR Prefix-SID: 179 Flags: [N] Algorithm: 0
      Reachability          : 2001:0:175::/64 Metric: 10 Type: 1 Up
      Reachability          : 2001:0:30:179::/64 Metric: 10 Type: 1 Up
      Router Capabilities: Router Id: 10.0.0.179 Flags: []
        Maximum SID depth:
          Base MPLS imposition (MSD type 1):  4
        SR Capability: Flags: [I V]
          SRGB Base: 20000 Range: 2000
        Algorithms:  0, 1
      Unsupported TLV: Type: 14 Length: 2
    Nokia-SXR-214.00-00        7574  51595  1191    357 L2  0000.0000.0214.00-00  <>
      NLPID: 0xCC(IPv4) 0x8E(IPv6)
      Hostname: Nokia-SXR-214
      Area addresses: 49.0001
      Interface address: 10.0.0.214
      Interface address: 20.30.214.214
      Interface address: 20.175.214.214
      Interface address: 20.214.216.214
      Interface address: 2000::214
      Interface address: 2001:0:175:214::214
      Interface address: 2001:0:214:216::214
      IS Neighbor          : Nokia-IXRe2-216.00  Metric: 10
        IPv4 Neighbor Address: 20.214.216.216
        IPv4 Interface Address: 20.214.216.214
        Adj-sid: 30003 flags: [L V B] weight: 0x0
      IS Neighbor          : Arista-Spine3-Q2A-30.00 Metric: 10
        IPv4 Neighbor Address: 20.30.214.30
        IPv4 Interface Address: 20.30.214.214
        Adj-sid: 30014 flags: [L V B] weight: 0x0
        Adj-sid: 30015 flags: [L V B F] weight: 0x0
      IS Neighbor          : Juniper-175-ACX7100-48L.00 Metric: 10
        IPv4 Neighbor Address: 20.175.214.175
        IPv4 Interface Address: 20.175.214.214
        Adj-sid: 30016 flags: [L V B] weight: 0x0
        Adj-sid: 30017 flags: [L V B F] weight: 0x0
      Reachability         : 20.30.214.0/24 Metric: 10 Type: 1 Up
      Reachability         : 20.175.214.0/24 Metric: 10 Type: 1 Up
      Reachability         : 20.214.216.0/24 Metric: 10 Type: 1 Up
      Reachability         : 10.0.0.214/32 Metric: 0 Type: 1 Up
        SR Prefix-SID: 214 Flags: [N P] Algorithm: 0
      Reachability          : 2000::214/128 Metric: 0 Type: 1 Up
      Reachability          : 2001:0:175:214::/64 Metric: 10 Type: 1 Up
      Reachability          : 2001:0:214:216::/64 Metric: 10 Type: 1 Up
      Router Capabilities: Router Id: 0.0.0.0 Flags: []
        Maximum SID depth:
          Base MPLS imposition (MSD type 1):  15
        SR Capability: Flags: [I V]
          SRGB Base: 20000 Range: 2000
        Algorithms:  0
    Nokia-IXRe2-216.00-00       135  28535  1083    120 L2  0100.0000.0216.00-00  <>
      NLPID: 0xCC(IPv4)
      Hostname: Nokia-IXRe2-216
      Area addresses: 49.0001.0000.0000.0216.00
      Interface address: 10.0.0.216
      Interface address: 20.214.216.216
      IS Neighbor          : Nokia-SXR-214.00    Metric: 10
        IPv4 Neighbor Address: 20.214.216.214
        IPv4 Interface Address: 20.214.216.216
      Reachability         : 20.214.216.0/24 Metric: 10 Type: 1 Up
      Reachability         : 10.0.0.216/32 Metric: 0 Type: 1 Up
    Nokia-SR1-217.00-00         139  55170   700    371 L2  0100.0000.0217.00-00  <>
      NLPID: 0xCC(IPv4) 0x8E(IPv6)
      Hostname: Nokia-SR1-217
      Area addresses: 49.0001.0000.0000.0216.00
      Interface address: 10.0.0.217
      Interface address: 20.30.217.217
      Interface address: 20.175.217.217
      Interface address: 2001:0:175:217::217
      Interface address: 2002::217
      IS Neighbor          : Arista-Spine3-Q2A-30.00 Metric: 10
        IPv4 Neighbor Address: 20.30.217.30
        IPv4 Interface Address: 20.30.217.217
        Adj-sid: 524286 flags: [L V B] weight: 0x0
        Adj-sid: 524284 flags: [L V B F] weight: 0x0
      IS Neighbor          : Juniper-175-ACX7100-48L.00 Metric: 10
        IPv4 Neighbor Address: 20.175.217.175
        IPv4 Interface Address: 20.175.217.217
        IPv6 Neighbor Address: 2001:0:175:217::175
        Global IPv6 Interface Address: 2001:0:175:217::217
        Adj-sid: 524285 flags: [L V B] weight: 0x0
        Adj-sid: 524283 flags: [L V B F] weight: 0x0
      Reachability         : 10.0.0.217/32 Metric: 0 Type: 1 Up
        SR Prefix-SID: 217 Flags: [N P] Algorithm: 0
      Reachability         : 20.30.217.0/24 Metric: 10 Type: 1 Up
      Reachability         : 20.175.217.0/24 Metric: 10 Type: 1 Up
      Reachability          : 2001:0:175:217::/64 Metric: 10 Type: 1 Up
      Reachability          : 2002::217/128 Metric: 0 Type: 1 Up
      Router Capabilities: Router Id: 10.0.0.217 Flags: []
        Maximum SID depth:
          Base MPLS imposition (MSD type 1):  12
        SR Capability: Flags: [I V]
          SRGB Base: 20000 Range: 2000
        Algorithms:  0
    221.00-00                     4  61582   638     80 L2  0221.0221.0221.00-00  <>
      NLPID: 0xCC(IPv4) 0x8E(IPv6)
      Area addresses: 49.0001
      Router Capabilities: Router Id: 10.0.0.221 Flags: []
        SR Local Block:
          SRLB Base: 626688 Range: 14336
        Maximum SID depth:
          Base MPLS imposition (MSD type 1):  10
        SR Capability: Flags: [I]
          SRGB Base: 720000 Range: 2000
      Unsupported TLV: Type: 14 Length: 2
    221.00-01                     3  55699   651     32 L2  0221.0221.0221.00-01  <>
      Hostname: 221
    221.00-02                     5  33627   745    273 L2  0221.0221.0221.00-02  <>
      Interface address: 20.175.221.221
      Interface address: 20.30.221.221
      Interface address: 10.0.0.221
      Interface address: 2001:0:175:221::221
      Interface address: 2001:0:30:221::221
      Interface address: 1221::1
      IS Neighbor          : Juniper-175-ACX7100-48L.00 Metric: 10
        IPv4 Neighbor Address: 20.175.221.175
        IPv4 Interface Address: 20.175.221.221
        Adj-sid: 524301 flags: [L V B] weight: 0x0
        Adj-sid: 524300 flags: [L V] weight: 0x0
      IS Neighbor          : Arista-Spine3-Q2A-30.00 Metric: 10
        IPv4 Neighbor Address: 20.30.221.30
        IPv4 Interface Address: 20.30.221.221
        Adj-sid: 524303 flags: [L V B] weight: 0x0
        Adj-sid: 524302 flags: [L V] weight: 0x0
      Reachability         : 20.175.221.0/24 Metric: 10 Type: 1 Up
      Reachability         : 20.30.221.0/24 Metric: 10 Type: 1 Up
      Reachability         : 10.0.0.221/32 Metric: 0 Type: 1 Up
        SR Prefix-SID: 1221 Flags: [N] Algorithm: 0
      Reachability          : 2001:0:175:221::/64 Metric: 10 Type: 1 Up
      Reachability          : 2001:0:30:221::/64 Metric: 10 Type: 1 Up
      Reachability          : 1221::1/128 Metric: 0 Type: 1 Up

```

## show isis flex-algo

```text

IS-IS Instance: IGP VRF: default

```

## show isis flex-algo path detail

```text
```

## show isis segment-routing tunnel

```text
  Index     Endpoint          Next Hop/Tunnel Index     Interface     Labels   
--------- ----------------- ------------------------- --------------- ---------
  1         10.0.0.84/32      TI-LFA (1)                -             [ 20084 ]
  2         10.0.0.72/32      TI-LFA (7)                -             [ 3 ]    
  4         10.0.0.175/32     20.30.32.32               Ethernet2     [ 20175 ]
                              20.30.53.53               Ethernet13    [ 20175 ]
                              20.30.72.72               Ethernet9     [ 20175 ]
                              20.30.84.84               Ethernet12    [ 20175 ]
                              20.30.124.124             Ethernet17    [ 2175 ] 
                              20.30.128.128             Ethernet19    [ 20175 ]
                              20.30.179.179             Ethernet40    [ 20175 ]
                              20.30.214.214             Ethernet5     [ 20175 ]
  5         10.0.0.53/32      TI-LFA (2)                -             [ 3 ]    
  6         10.0.0.179/32     TI-LFA (5)                -             [ 3 ]    
  7         10.0.0.120/32     20.30.120.120             Ethernet3     [ 3 ]    
  9         10.0.0.32/32      TI-LFA (8)                -             [ 3 ]    
  10        10.0.0.214/32     TI-LFA (6)                -             [ 20214 ]
  11        10.0.0.128/32     TI-LFA (4)                -             [ 3 ]    
  13        10.0.0.221/32     TI-LFA (0)                -             [ 3 ]    
  16        10.0.0.217/32     TI-LFA (3)                -             [ 20217 ]

```

## show isis segment-routing prefix-segments

```text

System ID: Arista-Spine3-Q2A-30			Instance: 'IGP'
SR supported Data-plane: MPLS			SR Router ID: 10.0.0.30

Node: 12     Proxy-Node: 0      Prefix: 0       Total Segments: 12

Flag Descriptions: R: Re-advertised, N: Node Segment, P: no-PHP
                   E: Explicit-NULL, V: Value, L: Local
Segment status codes: * - Self originated Prefix, L1 - level 1, L2 - level 2, ! - SR-unreachable,
                      # - Some IS-IS next-hops are SR-unreachable
   Prefix                      SID   Label Type       Flags                        System ID       Level Protection  Algorithm   
   ------------------------- ----- ------- ---------- ---------------------------- --------------- ----- ----------- -------------
*  10.0.0.30/32                 30   20030 Node       R:0 N:1 P:0 E:0 V:0 L:0      Arista-Spine3-Q2A-30 L2    unprotected SPF         
   10.0.0.32/32                 32   20032 Node       R:0 N:1 P:0 E:0 V:0 L:0      Arista-PE32-Q2C-32 L2    node        SPF         
   10.0.0.53/32                 53   20053 Node       R:0 N:1 P:1 E:1 V:0 L:0      Arrcus-53       L2    node        SPF         
   10.0.0.72/32                 72   20072 Node       R:0 N:1 P:0 E:0 V:0 L:0      Ciena-5134-72   L2    node        SPF         
   10.0.0.84/32                 84   20084 Node       R:0 N:1 P:1 E:0 V:0 L:0      Ericsson_84_R6678 L2    node        SPF         
   10.0.0.120/32               120   20120 Node       R:0 N:1 P:0 E:0 V:0 L:0      H3C_M1A_120     L2    node        SPF         
   10.0.0.128/32               128   20128 Node       R:0 N:1 P:0 E:0 V:0 L:0      0000.0000.0128  L2    node        SPF         
   10.0.0.175/32               175   20175 Node       R:0 N:1 P:0 E:0 V:0 L:0      Juniper-175-ACX7100-48L L2    unprotected SPF         
   10.0.0.179/32               179   20179 Node       R:0 N:1 P:0 E:0 V:0 L:0      Juniper-179-ACX7024 L2    node        SPF         
   10.0.0.214/32               214   20214 Node       R:0 N:1 P:1 E:0 V:0 L:0      Nokia-SXR-214   L2    node        SPF         
   10.0.0.217/32               217   20217 Node       R:0 N:1 P:1 E:0 V:0 L:0      Nokia-SR1-217   L2    node        SPF         
   10.0.0.221/32              1221  721221 Node       R:0 N:1 P:0 E:0 V:0 L:0      221             L2    node        SPF         
```

## show traffic-engineering segment-routing policy

```text
```

## show mpls segment-routing bindings detail

```text
10.0.0.30/32
   Local binding:  Label: imp-null
      Uptime: 19:30:49
   Remote binding: Peer ID: Arista-PE32-Q2C-32, Label: 20030
      Uptime: 0:57:32
   Remote binding: Peer ID: Arrcus-53, Label: 20030
      Uptime: 0:57:42
   Remote binding: Peer ID: Ciena-5134-72, Label: 20030
      Uptime: 0:31:48
   Remote binding: Peer ID: Ericsson_84_R6678, Label: 20030
      Uptime: 0:57:42
   Remote binding: Peer ID: H3C_M1A_120, Label: 20030
      Uptime: 0:57:36
   Remote binding: Peer ID: 0000.0000.0124, Label: 2030
      Uptime: 0:08:08
   Remote binding: Peer ID: 0000.0000.0128, Label: 20030
      Uptime: 0:09:35
   Remote binding: Peer ID: Juniper-175-ACX7100-48L, Label: 20030
      Uptime: 0:39:21
   Remote binding: Peer ID: Juniper-179-ACX7024, Label: 20030
      Uptime: 0:40:33
   Remote binding: Peer ID: Nokia-SXR-214, Label: 20030
      Uptime: 0:41:53
   Remote binding: Peer ID: Nokia-SR1-217, Label: 20030
      Uptime: 0:57:42
   Remote binding: Peer ID: 221, Label: 720030
      Uptime: 0:33:40
10.0.0.32/32
   Local binding:  Label: 20032
      Uptime: 0:30:29
   Remote binding: Peer ID: Arista-PE32-Q2C-32, Label: imp-null
      Uptime: 0:30:29
   Remote binding: Peer ID: Arrcus-53, Label: 20032
      Uptime: 0:30:29
   Remote binding: Peer ID: Ciena-5134-72, Label: 20032
      Uptime: 0:30:29
   Remote binding: Peer ID: Ericsson_84_R6678, Label: 20032
      Uptime: 0:30:29
   Remote binding: Peer ID: H3C_M1A_120, Label: 20032
      Uptime: 0:30:29
   Remote binding: Peer ID: 0000.0000.0124, Label: 2032
      Uptime: 0:08:08
   Remote binding: Peer ID: 0000.0000.0128, Label: 20032
      Uptime: 0:09:35
   Remote binding: Peer ID: Juniper-175-ACX7100-48L, Label: 20032
      Uptime: 0:30:29
   Remote binding: Peer ID: Juniper-179-ACX7024, Label: 20032
      Uptime: 0:30:29
   Remote binding: Peer ID: Nokia-SXR-214, Label: 20032
      Uptime: 0:30:29
   Remote binding: Peer ID: Nokia-SR1-217, Label: 20032
      Uptime: 0:30:29
   Remote binding: Peer ID: 221, Label: 720032
      Uptime: 0:30:29
10.0.0.53/32
   Local binding:  Label: 20053
      Uptime: 0:57:42
   Remote binding: Peer ID: Arista-PE32-Q2C-32, Label: 20053
      Uptime: 0:57:32
   Remote binding: Peer ID: Arrcus-53, Label: exp-null
      Uptime: 0:57:42
   Remote binding: Peer ID: Ciena-5134-72, Label: 20053
      Uptime: 0:31:48
   Remote binding: Peer ID: Ericsson_84_R6678, Label: 20053
      Uptime: 0:57:42
   Remote binding: Peer ID: H3C_M1A_120, Label: 20053
      Uptime: 0:57:36
   Remote binding: Peer ID: 0000.0000.0124, Label: 2053
      Uptime: 0:08:08
   Remote binding: Peer ID: 0000.0000.0128, Label: 20053
      Uptime: 0:09:35
   Remote binding: Peer ID: Juniper-175-ACX7100-48L, Label: 20053
      Uptime: 0:39:21
   Remote binding: Peer ID: Juniper-179-ACX7024, Label: 20053
      Uptime: 0:40:33
   Remote binding: Peer ID: Nokia-SXR-214, Label: 20053
      Uptime: 0:41:53
   Remote binding: Peer ID: Nokia-SR1-217, Label: 20053
      Uptime: 0:57:42
   Remote binding: Peer ID: 221, Label: 720053
      Uptime: 0:33:40
10.0.0.72/32
   Local binding:  Label: 20072
      Uptime: 0:31:53
   Remote binding: Peer ID: Arista-PE32-Q2C-32, Label: 20072
      Uptime: 0:31:53
   Remote binding: Peer ID: Arrcus-53, Label: 20072
      Uptime: 0:31:53
   Remote binding: Peer ID: Ciena-5134-72, Label: imp-null
      Uptime: 0:31:48
   Remote binding: Peer ID: Ericsson_84_R6678, Label: 20072
      Uptime: 0:31:53
   Remote binding: Peer ID: H3C_M1A_120, Label: 20072
      Uptime: 0:31:53
   Remote binding: Peer ID: 0000.0000.0124, Label: 2072
      Uptime: 0:08:08
   Remote binding: Peer ID: 0000.0000.0128, Label: 20072
      Uptime: 0:09:35
   Remote binding: Peer ID: Juniper-175-ACX7100-48L, Label: 20072
      Uptime: 0:31:53
   Remote binding: Peer ID: Juniper-179-ACX7024, Label: 20072
      Uptime: 0:31:53
   Remote binding: Peer ID: Nokia-SXR-214, Label: 20072
      Uptime: 0:31:53
   Remote binding: Peer ID: Nokia-SR1-217, Label: 20072
      Uptime: 0:31:53
   Remote binding: Peer ID: 221, Label: 720072
      Uptime: 0:31:53
10.0.0.84/32
   Local binding:  Label: 20084
      Uptime: 0:57:42
   Remote binding: Peer ID: Arista-PE32-Q2C-32, Label: 20084
      Uptime: 0:57:32
   Remote binding: Peer ID: Arrcus-53, Label: 20084
      Uptime: 0:57:42
   Remote binding: Peer ID: Ciena-5134-72, Label: 20084
      Uptime: 0:31:48
   Remote binding: Peer ID: Ericsson_84_R6678, Label: 20084
      Uptime: 0:57:42
   Remote binding: Peer ID: H3C_M1A_120, Label: 20084
      Uptime: 0:57:36
   Remote binding: Peer ID: 0000.0000.0124, Label: 2084
      Uptime: 0:08:08
   Remote binding: Peer ID: 0000.0000.0128, Label: 20084
      Uptime: 0:09:35
   Remote binding: Peer ID: Juniper-175-ACX7100-48L, Label: 20084
      Uptime: 0:39:21
   Remote binding: Peer ID: Juniper-179-ACX7024, Label: 20084
      Uptime: 0:40:33
   Remote binding: Peer ID: Nokia-SXR-214, Label: 20084
      Uptime: 0:41:53
   Remote binding: Peer ID: Nokia-SR1-217, Label: 20084
      Uptime: 0:57:42
   Remote binding: Peer ID: 221, Label: 720084
      Uptime: 0:33:40
10.0.0.120/32
   Local binding:  Label: 20120
      Uptime: 0:57:36
   Remote binding: Peer ID: Arista-PE32-Q2C-32, Label: 20120
      Uptime: 0:57:32
   Remote binding: Peer ID: Arrcus-53, Label: 20120
      Uptime: 0:57:36
   Remote binding: Peer ID: Ciena-5134-72, Label: 20120
      Uptime: 0:31:48
   Remote binding: Peer ID: Ericsson_84_R6678, Label: 20120
      Uptime: 0:57:36
   Remote binding: Peer ID: H3C_M1A_120, Label: imp-null
      Uptime: 0:57:36
   Remote binding: Peer ID: 0000.0000.0124, Label: 2120
      Uptime: 0:08:08
   Remote binding: Peer ID: 0000.0000.0128, Label: 20120
      Uptime: 0:09:35
   Remote binding: Peer ID: Juniper-175-ACX7100-48L, Label: 20120
      Uptime: 0:39:21
   Remote binding: Peer ID: Juniper-179-ACX7024, Label: 20120
      Uptime: 0:40:33
   Remote binding: Peer ID: Nokia-SXR-214, Label: 20120
      Uptime: 0:41:53
   Remote binding: Peer ID: Nokia-SR1-217, Label: 20120
      Uptime: 0:57:36
   Remote binding: Peer ID: 221, Label: 720120
      Uptime: 0:33:40
10.0.0.128/32
   Local binding:  Label: 20128
      Uptime: 0:09:35
   Remote binding: Peer ID: Arista-PE32-Q2C-32, Label: 20128
      Uptime: 0:09:35
   Remote binding: Peer ID: Arrcus-53, Label: 20128
      Uptime: 0:09:35
   Remote binding: Peer ID: Ciena-5134-72, Label: 20128
      Uptime: 0:09:35
   Remote binding: Peer ID: Ericsson_84_R6678, Label: 20128
      Uptime: 0:09:35
   Remote binding: Peer ID: H3C_M1A_120, Label: 20128
      Uptime: 0:09:35
   Remote binding: Peer ID: 0000.0000.0124, Label: 2128
      Uptime: 0:08:08
   Remote binding: Peer ID: 0000.0000.0128, Label: imp-null
      Uptime: 0:09:35
   Remote binding: Peer ID: Juniper-175-ACX7100-48L, Label: 20128
      Uptime: 0:09:35
   Remote binding: Peer ID: Juniper-179-ACX7024, Label: 20128
      Uptime: 0:09:35
   Remote binding: Peer ID: Nokia-SXR-214, Label: 20128
      Uptime: 0:09:35
   Remote binding: Peer ID: Nokia-SR1-217, Label: 20128
      Uptime: 0:09:35
   Remote binding: Peer ID: 221, Label: 720128
      Uptime: 0:09:35
10.0.0.175/32
   Local binding:  Label: 20175
      Uptime: 0:39:21
   Remote binding: Peer ID: Arista-PE32-Q2C-32, Label: 20175
      Uptime: 0:39:21
   Remote binding: Peer ID: Arrcus-53, Label: 20175
      Uptime: 0:39:21
   Remote binding: Peer ID: Ciena-5134-72, Label: 20175
      Uptime: 0:31:48
   Remote binding: Peer ID: Ericsson_84_R6678, Label: 20175
      Uptime: 0:39:21
   Remote binding: Peer ID: H3C_M1A_120, Label: 20175
      Uptime: 0:39:21
   Remote binding: Peer ID: 0000.0000.0124, Label: 2175
      Uptime: 0:08:08
   Remote binding: Peer ID: 0000.0000.0128, Label: 20175
      Uptime: 0:09:35
   Remote binding: Peer ID: Juniper-175-ACX7100-48L, Label: imp-null
      Uptime: 0:39:21
   Remote binding: Peer ID: Juniper-179-ACX7024, Label: 20175
      Uptime: 0:39:21
   Remote binding: Peer ID: Nokia-SXR-214, Label: 20175
      Uptime: 0:39:21
   Remote binding: Peer ID: Nokia-SR1-217, Label: 20175
      Uptime: 0:39:21
   Remote binding: Peer ID: 221, Label: 720175
      Uptime: 0:33:40
10.0.0.179/32
   Local binding:  Label: 20179
      Uptime: 0:40:33
   Remote binding: Peer ID: Arista-PE32-Q2C-32, Label: 20179
      Uptime: 0:40:33
   Remote binding: Peer ID: Arrcus-53, Label: 20179
      Uptime: 0:40:33
   Remote binding: Peer ID: Ciena-5134-72, Label: 20179
      Uptime: 0:31:48
   Remote binding: Peer ID: Ericsson_84_R6678, Label: 20179
      Uptime: 0:40:33
   Remote binding: Peer ID: H3C_M1A_120, Label: 20179
      Uptime: 0:40:33
   Remote binding: Peer ID: 0000.0000.0124, Label: 2179
      Uptime: 0:08:08
   Remote binding: Peer ID: 0000.0000.0128, Label: 20179
      Uptime: 0:09:35
   Remote binding: Peer ID: Juniper-175-ACX7100-48L, Label: 20179
      Uptime: 0:39:21
   Remote binding: Peer ID: Juniper-179-ACX7024, Label: imp-null
      Uptime: 0:40:33
   Remote binding: Peer ID: Nokia-SXR-214, Label: 20179
      Uptime: 0:40:33
   Remote binding: Peer ID: Nokia-SR1-217, Label: 20179
      Uptime: 0:40:33
   Remote binding: Peer ID: 221, Label: 720179
      Uptime: 0:33:40
10.0.0.214/32
   Local binding:  Label: 20214
      Uptime: 0:41:53
   Remote binding: Peer ID: Arista-PE32-Q2C-32, Label: 20214
      Uptime: 0:41:53
   Remote binding: Peer ID: Arrcus-53, Label: 20214
      Uptime: 0:41:53
   Remote binding: Peer ID: Ciena-5134-72, Label: 20214
      Uptime: 0:31:48
   Remote binding: Peer ID: Ericsson_84_R6678, Label: 20214
      Uptime: 0:41:53
   Remote binding: Peer ID: H3C_M1A_120, Label: 20214
      Uptime: 0:41:53
   Remote binding: Peer ID: 0000.0000.0124, Label: 2214
      Uptime: 0:08:08
   Remote binding: Peer ID: 0000.0000.0128, Label: 20214
      Uptime: 0:09:35
   Remote binding: Peer ID: Juniper-175-ACX7100-48L, Label: 20214
      Uptime: 0:39:21
   Remote binding: Peer ID: Juniper-179-ACX7024, Label: 20214
      Uptime: 0:40:33
   Remote binding: Peer ID: Nokia-SXR-214, Label: 20214
      Uptime: 0:41:53
   Remote binding: Peer ID: Nokia-SR1-217, Label: 20214
      Uptime: 0:41:53
   Remote binding: Peer ID: 221, Label: 720214
      Uptime: 0:33:40
10.0.0.217/32
   Local binding:  Label: 20217
      Uptime: 0:57:42
   Remote binding: Peer ID: Arista-PE32-Q2C-32, Label: 20217
      Uptime: 0:57:32
   Remote binding: Peer ID: Arrcus-53, Label: 20217
      Uptime: 0:57:42
   Remote binding: Peer ID: Ciena-5134-72, Label: 20217
      Uptime: 0:31:48
   Remote binding: Peer ID: Ericsson_84_R6678, Label: 20217
      Uptime: 0:57:42
   Remote binding: Peer ID: H3C_M1A_120, Label: 20217
      Uptime: 0:57:36
   Remote binding: Peer ID: 0000.0000.0124, Label: 2217
      Uptime: 0:08:08
   Remote binding: Peer ID: 0000.0000.0128, Label: 20217
      Uptime: 0:09:35
   Remote binding: Peer ID: Juniper-175-ACX7100-48L, Label: 20217
      Uptime: 0:39:21
   Remote binding: Peer ID: Juniper-179-ACX7024, Label: 20217
      Uptime: 0:40:33
   Remote binding: Peer ID: Nokia-SXR-214, Label: 20217
      Uptime: 0:41:53
   Remote binding: Peer ID: Nokia-SR1-217, Label: 20217
      Uptime: 0:57:42
   Remote binding: Peer ID: 221, Label: 720217
      Uptime: 0:33:40
10.0.0.221/32
   Local binding:  Label: 21221
      Uptime: 0:33:41
   Remote binding: Peer ID: Arista-PE32-Q2C-32, Label: 21221
      Uptime: 0:33:41
   Remote binding: Peer ID: Arrcus-53, Label: 21221
      Uptime: 0:33:41
   Remote binding: Peer ID: Ciena-5134-72, Label: 21221
      Uptime: 0:31:48
   Remote binding: Peer ID: Ericsson_84_R6678, Label: 21221
      Uptime: 0:33:41
   Remote binding: Peer ID: H3C_M1A_120, Label: 21221
      Uptime: 0:33:41
   Remote binding: Peer ID: 0000.0000.0124, Label: 3221
      Uptime: 0:08:08
   Remote binding: Peer ID: 0000.0000.0128, Label: 21221
      Uptime: 0:09:35
   Remote binding: Peer ID: Juniper-175-ACX7100-48L, Label: 21221
      Uptime: 0:33:41
   Remote binding: Peer ID: Juniper-179-ACX7024, Label: 21221
      Uptime: 0:33:41
   Remote binding: Peer ID: Nokia-SXR-214, Label: 21221
      Uptime: 0:33:41
   Remote binding: Peer ID: Nokia-SR1-217, Label: 21221
      Uptime: 0:33:41
   Remote binding: Peer ID: 221, Label: imp-null
      Uptime: 0:33:40
```

## show ip route

```text

VRF: default
Source Codes:
       C - connected, S - static, K - kernel,
       O - OSPF, IA - OSPF inter area, E1 - OSPF external type 1,
       E2 - OSPF external type 2, N1 - OSPF NSSA external type 1,
       N2 - OSPF NSSA external type2, B - Other BGP Routes,
       B I - iBGP, B E - eBGP, R - RIP, I L1 - IS-IS level 1,
       I L2 - IS-IS level 2, O3 - OSPFv3, A B - BGP Aggregate,
       A O - OSPF Summary, NG - Nexthop Group Static Route,
       V - VXLAN Control Service, M - Martian,
       DH - DHCP client installed default route,
       DP - Dynamic Policy Route, L - VRF Leaked,
       G  - gRIBI, RC - Route Cache Route,
       CL - CBF Leaked Route

Gateway of last resort is not set

 C        10.0.0.30/32
           directly connected, Loopback0
 I L2     10.0.0.32/32 [115/10]
           via 20.30.32.32, Ethernet2
 I L2     10.0.0.53/32 [115/10]
           via 20.30.53.53, Ethernet13
 I L2     10.0.0.72/32 [115/20]
           via 20.30.72.72, Ethernet9
 I L2     10.0.0.84/32 [115/20]
           via 20.30.84.84, Ethernet12
 I L2     10.0.0.120/32 [115/10]
           via 20.30.120.120, Ethernet3
 I L2     10.0.0.128/32 [115/10]
           via 20.30.128.128, Ethernet19
 I L2     10.0.0.175/32 [115/20]
           via 20.30.32.32, Ethernet2
           via 20.30.214.214, Ethernet5
           via 20.30.72.72, Ethernet9
           via 20.30.84.84, Ethernet12
           via 20.30.53.53, Ethernet13
           via 20.30.124.124, Ethernet17
           via 20.30.128.128, Ethernet19
           via 20.30.179.179, Ethernet40
 I L2     10.0.0.179/32 [115/10]
           via 20.30.179.179, Ethernet40
 I L2     10.0.0.214/32 [115/10]
           via 20.30.214.214, Ethernet5
 I L2     10.0.0.216/32 [115/20]
           via 20.30.214.214, Ethernet5
 I L2     10.0.0.217/32 [115/10]
           via 20.30.217.217, Ethernet4
 I L2     10.0.0.221/32 [115/10]
           via 20.30.221.221, Ethernet15
 C        20.30.32.0/24
           directly connected, Ethernet2
 C        20.30.53.0/24
           directly connected, Ethernet13
 C        20.30.66.0/24
           directly connected, Ethernet31
 C        20.30.72.0/24
           directly connected, Ethernet9
 C        20.30.84.0/24
           directly connected, Ethernet12
 C        20.30.120.0/24
           directly connected, Ethernet3
 C        20.30.124.0/24
           directly connected, Ethernet17
 C        20.30.128.0/24
           directly connected, Ethernet19
 C        20.30.179.0/24
           directly connected, Ethernet40
 C        20.30.184.0/24
           directly connected, Ethernet7
 C        20.30.214.0/24
           directly connected, Ethernet5
 C        20.30.217.0/24
           directly connected, Ethernet4
 C        20.30.221.0/24
           directly connected, Ethernet15
 I L2     20.32.175.0/24 [115/20]
           via 20.30.32.32, Ethernet2
 I L2     20.53.175.0/24 [115/20]
           via 20.30.53.53, Ethernet13
 I L2     20.66.175.0/24 [115/30]
           via 20.30.32.32, Ethernet2
           via 20.30.214.214, Ethernet5
           via 20.30.72.72, Ethernet9
           via 20.30.84.84, Ethernet12
           via 20.30.53.53, Ethernet13
           via 20.30.124.124, Ethernet17
           via 20.30.128.128, Ethernet19
           via 20.30.179.179, Ethernet40
 I L2     20.72.175.0/24 [115/20]
           via 20.30.72.72, Ethernet9
 I L2     20.84.175.0/24 [115/30]
           via 20.30.32.32, Ethernet2
           via 20.30.214.214, Ethernet5
           via 20.30.72.72, Ethernet9
           via 20.30.84.84, Ethernet12
           via 20.30.53.53, Ethernet13
           via 20.30.124.124, Ethernet17
           via 20.30.128.128, Ethernet19
           via 20.30.179.179, Ethernet40
 I L2     20.120.175.0/24 [115/30]
           via 20.30.32.32, Ethernet2
           via 20.30.214.214, Ethernet5
           via 20.30.72.72, Ethernet9
           via 20.30.84.84, Ethernet12
           via 20.30.53.53, Ethernet13
           via 20.30.124.124, Ethernet17
           via 20.30.128.128, Ethernet19
           via 20.30.179.179, Ethernet40
 I L2     20.120.214.0/24 [115/20]
           via 20.30.120.120, Ethernet3
 I L2     20.124.175.0/24 [115/20]
           via 20.30.124.124, Ethernet17
 I L2     20.128.175.0/24 [115/20]
           via 20.30.128.128, Ethernet19
 I L2     20.131.175.0/24 [115/30]
           via 20.30.32.32, Ethernet2
           via 20.30.214.214, Ethernet5
           via 20.30.72.72, Ethernet9
           via 20.30.84.84, Ethernet12
           via 20.30.53.53, Ethernet13
           via 20.30.124.124, Ethernet17
           via 20.30.128.128, Ethernet19
           via 20.30.179.179, Ethernet40
 I L2     20.175.179.0/24 [115/20]
           via 20.30.179.179, Ethernet40
 I L2     20.175.184.0/24 [115/30]
           via 20.30.32.32, Ethernet2
           via 20.30.214.214, Ethernet5
           via 20.30.72.72, Ethernet9
           via 20.30.84.84, Ethernet12
           via 20.30.53.53, Ethernet13
           via 20.30.124.124, Ethernet17
           via 20.30.128.128, Ethernet19
           via 20.30.179.179, Ethernet40
 I L2     20.175.214.0/24 [115/20]
           via 20.30.214.214, Ethernet5
 I L2     20.175.217.0/24 [115/20]
           via 20.30.217.217, Ethernet4
 I L2     20.175.221.0/24 [115/20]
           via 20.30.221.221, Ethernet15
 I L2     20.214.216.0/24 [115/20]
           via 20.30.214.214, Ethernet5

```

## show ip route vrf RED

```text

VRF: RED
Source Codes:
       C - connected, S - static, K - kernel,
       O - OSPF, IA - OSPF inter area, E1 - OSPF external type 1,
       E2 - OSPF external type 2, N1 - OSPF NSSA external type 1,
       N2 - OSPF NSSA external type2, B - Other BGP Routes,
       B I - iBGP, B E - eBGP, R - RIP, I L1 - IS-IS level 1,
       I L2 - IS-IS level 2, O3 - OSPFv3, A B - BGP Aggregate,
       A O - OSPF Summary, NG - Nexthop Group Static Route,
       V - VXLAN Control Service, M - Martian,
       DH - DHCP client installed default route,
       DP - Dynamic Policy Route, L - VRF Leaked,
       G  - gRIBI, RC - Route Cache Route,
       CL - CBF Leaked Route

Gateway of last resort is not set

 C        10.0.0.30/32
           directly connected, Loopback5001
 B I      50.10.32.0/24 [200/0]
           via 10.0.0.32/32, IS-IS SR tunnel index 9, label 378528
              via TI-LFA tunnel index 8, label imp-null(3)
                 via 20.30.32.32, Ethernet2, label imp-null(3)
                 backup via 20.30.124.124, Ethernet17, label 2175 20032
 B I      50.10.72.0/24 [200/0]
           via 10.0.0.72/32, IS-IS SR tunnel index 2, label 62002
              via TI-LFA tunnel index 7, label imp-null(3)
                 via 20.30.72.72, Ethernet9, label imp-null(3)
                 backup via 20.30.214.214, Ethernet5, label 20175 20072
 B I      50.10.84.0/24 [200/0]
           via 10.0.0.84/32, IS-IS SR tunnel index 1, label 720896
              via TI-LFA tunnel index 1, label 20084
                 via 20.30.84.84, Ethernet12, label imp-null(3)
                 backup via 20.30.53.53, Ethernet13, label 20175
 B I      50.10.120.0/24 [200/0]
           via 10.0.0.120/32, IS-IS SR tunnel index 7, label 1277
              via 20.30.120.120, Ethernet3, label imp-null(3)
 B I      50.10.179.0/24 [200/0]
           via 10.0.0.179/32, IS-IS SR tunnel index 6, label 16
              via TI-LFA tunnel index 5, label imp-null(3)
                 via 20.30.179.179, Ethernet40, label imp-null(3)
                 backup via 20.30.217.217, Ethernet4, label 20175 20179
 B I      50.10.214.0/24 [200/0]
           via 10.0.0.214/32, IS-IS SR tunnel index 10, label 500000
              via TI-LFA tunnel index 6, label 20214
                 via 20.30.214.214, Ethernet5, label imp-null(3)
                 backup via 20.30.84.84, Ethernet12, label 20175
 B I      50.10.217.0/24 [200/0]
           via 10.0.0.217/32, IS-IS SR tunnel index 16, label 524287
              via TI-LFA tunnel index 3, label 20217
                 via 20.30.217.217, Ethernet4, label imp-null(3)
                 backup via 20.30.53.53, Ethernet13, label 20175
 B I      50.10.221.0/24 [200/0]
           via 10.0.0.221/32, IS-IS SR tunnel index 13, label 524289
              via TI-LFA tunnel index 0, label imp-null(3)
                 via 20.30.221.221, Ethernet15, label imp-null(3)
                 backup via 20.30.53.53, Ethernet13, label 20175 21221
 B I      51.10.120.0/24 [200/0]
           via 10.0.0.120/32, IS-IS SR tunnel index 7, label 1277
              via 20.30.120.120, Ethernet3, label imp-null(3)

```

## show ipv6 route

```text

VRF: default
Displaying 15 of 31 IPv6 routing table entries
Source Codes:
       C - connected, S - static, K - kernel, O3 - OSPFv3,
       B - Other BGP Routes, A B - BGP Aggregate, R - RIP,
       I L1 - IS-IS level 1, I L2 - IS-IS level 2, DH - DHCP,
       NG - Nexthop Group Static Route, M - Martian,
       DP - Dynamic Policy Route, L - VRF Leaked,
       G  - gRIBI, RC - Route Cache Route,
       CL - CBF Leaked Route

 C        2001:0:30:32::/64 [0/0]
           via Ethernet2, directly connected
 C        2001:0:30:66::/64 [0/0]
           via Ethernet31, directly connected
 C        2001:0:30:72::/64 [0/0]
           via Ethernet9, directly connected
 C        2001:0:30:84::/64 [0/0]
           via Ethernet12, directly connected
 C        2001:0:30:120::/64 [0/0]
           via Ethernet3, directly connected
 C        2001:0:30:124::/64 [0/0]
           via Ethernet17, directly connected
 C        2001:0:30:128::/64 [0/0]
           via Ethernet19, directly connected
 C        2001:0:30:179::/64 [0/0]
           via Ethernet40, directly connected
 C        2001:0:30:184::/64 [0/0]
           via Ethernet7, directly connected
 C        2001:0:30:214::/64 [0/0]
           via Ethernet5, directly connected
 C        2001:0:30:217::/64 [0/0]
           via Ethernet4, directly connected
 C        2001:0:30:221::/64 [0/0]
           via Ethernet15, directly connected
 I L2     2001:0:32:175::/64 [115/20]
           via fe80::d6af:f7ff:fe2f:1396, Ethernet2
 C        2001:0:53:120::/64 [0/0]
           via Ethernet13, directly connected
 I L2     2001:0:120:214::/64 [115/20]
           via fe80::be31:e2ff:fee1:ec2c, Ethernet3

```

## show ipv6 route vrf RED

```text

VRF: RED
Displaying 9 of 12 IPv6 routing table entries
Source Codes:
       C - connected, S - static, K - kernel, O3 - OSPFv3,
       B - Other BGP Routes, A B - BGP Aggregate, R - RIP,
       I L1 - IS-IS level 1, I L2 - IS-IS level 2, DH - DHCP,
       NG - Nexthop Group Static Route, M - Martian,
       DP - Dynamic Policy Route, L - VRF Leaked,
       G  - gRIBI, RC - Route Cache Route,
       CL - CBF Leaked Route

 B I      2600:50:10:32::/64 [200/0]
           via 10.0.0.32/32, IS-IS SR tunnel index 9, label 378529
              via TI-LFA tunnel index 8, label imp-null(3)
                 via 20.30.32.32, Ethernet2, label imp-null(3)
                 backup via 20.30.124.124, Ethernet17, label 2175 20032
 B I      2600:50:10:72::/64 [200/0]
           via 10.0.0.72/32, IS-IS SR tunnel index 2, label 62003
              via TI-LFA tunnel index 7, label imp-null(3)
                 via 20.30.72.72, Ethernet9, label imp-null(3)
                 backup via 20.30.214.214, Ethernet5, label 20175 20072
 B I      2600:50:10:84::/64 [200/0]
           via 10.0.0.84/32, IS-IS SR tunnel index 1, label 720897
              via TI-LFA tunnel index 1, label 20084
                 via 20.30.84.84, Ethernet12, label imp-null(3)
                 backup via 20.30.53.53, Ethernet13, label 20175
 B I      2600:50:10:120::/64 [200/0]
           via 10.0.0.120/32, IS-IS SR tunnel index 7, label 1276
              via 20.30.120.120, Ethernet3, label imp-null(3)
 B I      2600:50:10:179::/64 [200/0]
           via 10.0.0.179/32, IS-IS SR tunnel index 6, label 16
              via TI-LFA tunnel index 5, label imp-null(3)
                 via 20.30.179.179, Ethernet40, label imp-null(3)
                 backup via 20.30.217.217, Ethernet4, label 20175 20179
 B I      2600:50:10:214::/64 [200/0]
           via 10.0.0.214/32, IS-IS SR tunnel index 10, label 500000
              via TI-LFA tunnel index 6, label 20214
                 via 20.30.214.214, Ethernet5, label imp-null(3)
                 backup via 20.30.84.84, Ethernet12, label 20175
 B I      2600:50:10:217::/64 [200/0]
           via 10.0.0.217/32, IS-IS SR tunnel index 16, label 524287
              via TI-LFA tunnel index 3, label 20217
                 via 20.30.217.217, Ethernet4, label imp-null(3)
                 backup via 20.30.53.53, Ethernet13, label 20175
 B I      2600:50:10:221::/64 [200/0]
           via 10.0.0.221/32, IS-IS SR tunnel index 13, label 524289
              via TI-LFA tunnel index 0, label imp-null(3)
                 via 20.30.221.221, Ethernet15, label imp-null(3)
                 backup via 20.30.53.53, Ethernet13, label 20175 21221
 B I      2600:51:10:120::/64 [200/0]
           via 10.0.0.120/32, IS-IS SR tunnel index 7, label 1276
              via 20.30.120.120, Ethernet3, label imp-null(3)

! IPv6 routing not enabled
```

## show mpls route

```text
MPLS forwarding table (Label [metric] Vias) - 25 routes 
MPLS next-hop resolution allow default route: False
Metric Codes:
          A - Active metric
Via Type Codes:
          M - MPLS via, LP - LDP pseudowire via,
          I - IP lookup via, V - VLAN via,
          VA - EVPN VLAN aware via, ES - EVPN ethernet segment via,
          VF - EVPN VLAN flood via, AF - EVPN VLAN aware flood via,
          NG - Nexthop group via, BP - BGP pseudowire via,
          VP - VPWS pseudowire via, MSP - Static pseudowire via

 20032   A[1]
                via M, ::, pop
                    EgressACL: apply
                  via TI-LFA tunnel index 8
                    via 20.30.32.32, Ethernet2, label imp-null(3)
                    backup via 20.30.124.124, Ethernet17, label 2175 20032
 20053   A[1]
                via M, ::, pop
                    EgressACL: apply
                  via TI-LFA tunnel index 2
                    via 20.30.53.53, Ethernet13, label exp-null-v4(0)
                    backup via 20.30.84.84, Ethernet12, label 20175 20053
 20072   A[1]
                via M, ::, pop
                    EgressACL: apply
                  via TI-LFA tunnel index 7
                    via 20.30.72.72, Ethernet9, label imp-null(3)
                    backup via 20.30.214.214, Ethernet5, label 20175 20072
 20084   A[1]
                via M, ::, forward
                    EgressACL: apply
                  via TI-LFA tunnel index 1
                    via 20.30.84.84, Ethernet12, label imp-null(3)
                    backup via 20.30.53.53, Ethernet13, label 20175
 20120   A[1]
                via M, pop
                    EgressACL: apply
                    20.30.120.120 Ethernet3
 20128   A[1]
                via M, ::, pop
                    EgressACL: apply
                  via TI-LFA tunnel index 4
                    via 20.30.128.128, Ethernet19, label imp-null(3)
                    backup via 20.30.84.84, Ethernet12, label 20175 20128
 20175   A[1]
                via M, 20.30.32.32, swap 20175
                    EgressACL: apply
                    directly connected, Ethernet2
                    d4:af:f7:2f:13:96, vlan 1007
                via M, 20.30.53.53, swap 20175
                    EgressACL: apply
                    directly connected, Ethernet13
                    5c:07:58:a3:0a:aa, vlan 1014
                via M, 20.30.72.72, swap 20175
                    EgressACL: apply
                    directly connected, Ethernet9
                    e0:9b:27:c4:c5:84, vlan 1012
                via M, 20.30.84.84, swap 20175
                    EgressACL: apply
                    directly connected, Ethernet12
                    58:70:7f:9f:c4:03, vlan 1013
                via M, 20.30.124.124, swap 2175
                    EgressACL: apply
                    directly connected, Ethernet17
                    64:6d:4e:32:e1:22, vlan 1016
                via M, 20.30.128.128, swap 20175
                    EgressACL: apply
                    directly connected, Ethernet19
                    60:53:75:13:ba:d8, vlan 1018
                via M, 20.30.179.179, swap 20175
                    EgressACL: apply
                    directly connected, Ethernet40
                    e8:24:a6:96:05:48, vlan 1020
                via M, 20.30.214.214, swap 20175
                    EgressACL: apply
                    directly connected, Ethernet5
                    18:5b:00:61:ac:6f, vlan 1010
 20179   A[1]
                via M, ::, pop
                    EgressACL: apply
                  via TI-LFA tunnel index 5
                    via 20.30.179.179, Ethernet40, label imp-null(3)
                    backup via 20.30.217.217, Ethernet4, label 20175 20179
 20214   A[1]
                via M, ::, forward
                    EgressACL: apply
                  via TI-LFA tunnel index 6
                    via 20.30.214.214, Ethernet5, label imp-null(3)
                    backup via 20.30.84.84, Ethernet12, label 20175
 20217   A[1]
                via M, ::, forward
                    EgressACL: apply
                  via TI-LFA tunnel index 3
                    via 20.30.217.217, Ethernet4, label imp-null(3)
                    backup via 20.30.53.53, Ethernet13, label 20175
 21221   A[1]
                via M, ::, pop
                    EgressACL: apply
                  via TI-LFA tunnel index 0
                    via 20.30.221.221, Ethernet15, label imp-null(3)
                    backup via 20.30.53.53, Ethernet13, label 20175 21221
 362159  A[1]
                via M, 20.30.32.32, pop
                    EgressACL: apply
                    directly connected, Ethernet2
                    d4:af:f7:2f:13:96, vlan 1007
 362160  A[1]
                via M, 20.30.221.221, pop
                    EgressACL: apply
                    directly connected, Ethernet15
                    30:c5:07:84:3e:79, vlan 1015
 362161  A[1]
                via M, 20.30.72.72, pop
                    EgressACL: apply
                    directly connected, Ethernet9
                    e0:9b:27:c4:c5:84, vlan 1012
 362162  A[1]
                via M, 20.30.120.120, pop
                    EgressACL: apply
                    directly connected, Ethernet3
                    bc:31:e2:e1:ec:2c, vlan 1008
 362163  A[1]
                via M, fe80::be31:e2ff:fee1:ec2c, pop
                    EgressACL: apply
                    directly connected, Ethernet3
                    bc:31:e2:e1:ec:2c, vlan 1008
 362165  A[1]
                via M, 20.30.53.53, pop
                    EgressACL: apply
                    directly connected, Ethernet13
                    5c:07:58:a3:0a:aa, vlan 1014
 362166  A[1]
                via M, 20.30.214.214, pop
                    EgressACL: apply
                    directly connected, Ethernet5
                    18:5b:00:61:ac:6f, vlan 1010
 362167  A[1]
                via M, 20.30.84.84, pop
                    EgressACL: apply
                    directly connected, Ethernet12
                    58:70:7f:9f:c4:03, vlan 1013
 362168  A[1]
                via M, 20.30.179.179, pop
                    EgressACL: apply
                    directly connected, Ethernet40
                    e8:24:a6:96:05:48, vlan 1020
 362169  A[1]
                via M, fe80::d6af:f7ff:fe2f:1396, pop
                    EgressACL: apply
                    directly connected, Ethernet2
                    d4:af:f7:2f:13:96, vlan 1007
 362171  A[1]
                via M, 20.30.217.217, pop
                    EgressACL: apply
                    directly connected, Ethernet4
                    c0:14:b8:21:97:90, vlan 1009
 362174  A[1]
                via M, 20.30.128.128, pop
                    EgressACL: apply
                    directly connected, Ethernet19
                    60:53:75:13:ba:d8, vlan 1018
 362175  A[1]
                via M, 20.30.124.124, pop
                    EgressACL: apply
                    directly connected, Ethernet17
                    64:6d:4e:32:e1:22, vlan 1016
 378528   [0]
                via I, ipv4, vrf RED
```

## show mpls lfib route

```text
MPLS forwarding table (Label [metric] Vias) - 25 routes 
MPLS next-hop resolution allow default route: False
Via Type Codes:
          M - MPLS via, LP - LDP pseudowire via,
          I - IP lookup via, V - VLAN via,
          VA - EVPN VLAN aware via, ES - EVPN ethernet segment via,
          VF - EVPN VLAN flood via, AF - EVPN VLAN aware flood via,
          NG - Nexthop group via, BP - BGP pseudowire via,
          VP - VPWS pseudowire via, MSP - Static pseudowire via
Source Codes:
          G - gRIBI, S - Static MPLS route,
          B2 - BGP L2 EVPN, B3 - BGP L3 VPN,
          R - RSVP, P - Pseudowire,
          L - LDP, M - MLDP,
          I>BL - IS-IS SR to BGP LU, IP - IS-IS SR prefix segment,
          IA - IS-IS SR adjacency segment, I>L - IS-IS SR to LDP,
          L>I - LDP to IS-IS SR, OP - Ospf SR prefix segment,
          OA - Ospf SR adjacency segment, OL - Ospf SR segment to LDP,
          L0 - LDP to Ospf SR segment, BL - BGP LU,
          BL>L - BGP LU to LDP, L>BL - LDP to BGP LU,
          ST - SR TE policy, SMP - SR P2MP,
          BL>I - BGP LU to IS-IS SR, BLS - BGP Link State,
          DE - Debug LFIB

 IP    20032    [1], 10.0.0.32/32
                via TI-LFA tunnel index 8, pop
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                    via 20.30.32.32, Ethernet2, label imp-null(3)
                    backup via 20.30.124.124, Ethernet17, label 2175 20032
 IP    20053    [1], 10.0.0.53/32
                via TI-LFA tunnel index 2, pop
                 payload autoDecide, ttlMode uniform, apply egress-acl
                    via 20.30.53.53, Ethernet13, label exp-null-v4(0)
                    backup via 20.30.84.84, Ethernet12, label 20175 20053
 IP    20072    [1], 10.0.0.72/32
                via TI-LFA tunnel index 7, pop
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                    via 20.30.72.72, Ethernet9, label imp-null(3)
                    backup via 20.30.214.214, Ethernet5, label 20175 20072
 IP    20084    [1], 10.0.0.84/32
                via TI-LFA tunnel index 1, forward
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                    via 20.30.84.84, Ethernet12, label imp-null(3)
                    backup via 20.30.53.53, Ethernet13, label 20175
 IP    20120    [1], 10.0.0.120/32
                via M, 20.30.120.120, pop
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                 interface Ethernet3
 IP    20128    [1], 10.0.0.128/32
                via TI-LFA tunnel index 4, pop
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                    via 20.30.128.128, Ethernet19, label imp-null(3)
                    backup via 20.30.84.84, Ethernet12, label 20175 20128
 IP    20175    [1], 10.0.0.175/32
                via M, 20.30.32.32, swap 20175
                 payload autoDecide, ttlMode uniform, apply egress-acl
                 interface Ethernet2
                via M, 20.30.53.53, swap 20175
                 payload autoDecide, ttlMode uniform, apply egress-acl
                 interface Ethernet13
                via M, 20.30.72.72, swap 20175
                 payload autoDecide, ttlMode uniform, apply egress-acl
                 interface Ethernet9
                via M, 20.30.84.84, swap 20175
                 payload autoDecide, ttlMode uniform, apply egress-acl
                 interface Ethernet12
                via M, 20.30.124.124, swap 2175
                 payload autoDecide, ttlMode uniform, apply egress-acl
                 interface Ethernet17
                via M, 20.30.128.128, swap 20175
                 payload autoDecide, ttlMode uniform, apply egress-acl
                 interface Ethernet19
                via M, 20.30.179.179, swap 20175
                 payload autoDecide, ttlMode uniform, apply egress-acl
                 interface Ethernet40
                via M, 20.30.214.214, swap 20175
                 payload autoDecide, ttlMode uniform, apply egress-acl
                 interface Ethernet5
 IP    20179    [1], 10.0.0.179/32
                via TI-LFA tunnel index 5, pop
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                    via 20.30.179.179, Ethernet40, label imp-null(3)
                    backup via 20.30.217.217, Ethernet4, label 20175 20179
 IP    20214    [1], 10.0.0.214/32
                via TI-LFA tunnel index 6, forward
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                    via 20.30.214.214, Ethernet5, label imp-null(3)
                    backup via 20.30.84.84, Ethernet12, label 20175
 IP    20217    [1], 10.0.0.217/32
                via TI-LFA tunnel index 3, forward
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                    via 20.30.217.217, Ethernet4, label imp-null(3)
                    backup via 20.30.53.53, Ethernet13, label 20175
 IP    21221    [1], 10.0.0.221/32
                via TI-LFA tunnel index 0, pop
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                    via 20.30.221.221, Ethernet15, label imp-null(3)
                    backup via 20.30.53.53, Ethernet13, label 20175 21221
 IA    362159   [1]
                via M, 20.30.32.32, pop
                 payload autoDecide, ttlMode uniform, apply egress-acl
                 interface Ethernet2
 IA    362160   [1]
                via M, 20.30.221.221, pop
                 payload autoDecide, ttlMode uniform, apply egress-acl
                 interface Ethernet15
 IA    362161   [1]
                via M, 20.30.72.72, pop
                 payload autoDecide, ttlMode uniform, apply egress-acl
                 interface Ethernet9
 IA    362162   [1]
                via M, 20.30.120.120, pop
                 payload autoDecide, ttlMode uniform, apply egress-acl
                 interface Ethernet3
 IA    362163   [1]
                via M, fe80::be31:e2ff:fee1:ec2c, pop
                 payload autoDecide, ttlMode uniform, apply egress-acl
                 interface Ethernet3
 IA    362165   [1]
                via M, 20.30.53.53, pop
                 payload autoDecide, ttlMode uniform, apply egress-acl
                 interface Ethernet13
 IA    362166   [1]
                via M, 20.30.214.214, pop
                 payload autoDecide, ttlMode uniform, apply egress-acl
                 interface Ethernet5
 IA    362167   [1]
                via M, 20.30.84.84, pop
                 payload autoDecide, ttlMode uniform, apply egress-acl
                 interface Ethernet12
 IA    362168   [1]
                via M, 20.30.179.179, pop
                 payload autoDecide, ttlMode uniform, apply egress-acl
                 interface Ethernet40
 IA    362169   [1]
                via M, fe80::d6af:f7ff:fe2f:1396, pop
                 payload autoDecide, ttlMode uniform, apply egress-acl
                 interface Ethernet2
 IA    362171   [1]
                via M, 20.30.217.217, pop
                 payload autoDecide, ttlMode uniform, apply egress-acl
                 interface Ethernet4
 IA    362174   [1]
                via M, 20.30.128.128, pop
                 payload autoDecide, ttlMode uniform, apply egress-acl
                 interface Ethernet19
 IA    362175   [1]
                via M, 20.30.124.124, pop
                 payload autoDecide, ttlMode uniform, apply egress-acl
                 interface Ethernet17
 B3    378528   [0]
                via I, ipv4, vrf RED
```

## show bgp evpn

```text
BGP routing table information for VRF default
Router identifier 10.0.0.30, local AS number 64512
Route status codes: * - valid, > - active, S - Stale, E - ECMP head, e - ECMP
                    c - Contributing to ECMP, % - Pending best path selection
Origin codes: i - IGP, e - EGP, ? - incomplete
AS Path Attributes: Or-ID - Originator ID, C-LST - Cluster List, LL Nexthop - Link Local Nexthop

          Network                Next Hop              Metric  LocPref Weight  Path
```

## show bgp vpn-ipv4

```text
BGP routing table information for VRF default
Router identifier 10.0.0.30, local AS number 64512
Route status codes: s - suppressed contributor, * - valid, > - active, E - ECMP head, e - ECMP
                    S - Stale, c - Contributing to ECMP, b - backup, L - labeled-unicast
                    % - Pending best path selection
Origin codes: i - IGP, e - EGP, ? - incomplete
AS Path Attributes: Or-ID - Originator ID, C-LST - Cluster List, LL Nexthop - Link Local Nexthop

          Network                Next Hop              Metric  LocPref Weight  Path
 * >      RD: 10.0.0.32:5001 IPv4 prefix 50.10.32.0/24
                                 10.0.0.32             -       100     0       i
 * >      RD: 72:5001 IPv4 prefix 50.10.72.0/24
                                 10.0.0.72             -       100     0       ?
 * >      RD: 84:5001 IPv4 prefix 50.10.84.0/24
                                 10.0.0.84             0       100     0       ?
 * >      RD: 120:5001 IPv4 prefix 50.10.120.0/24
                                 10.0.0.120            0       100     0       ?
 * >      RD: 179:5001 IPv4 prefix 50.10.179.0/24
                                 10.0.0.179            -       100     0       i
 * >      RD: 214:5001 IPv4 prefix 50.10.214.0/24
                                 10.0.0.214            -       100     0       i
 * >      RD: 217:5001 IPv4 prefix 50.10.217.0/24
                                 10.0.0.217            -       100     0       i
 * >      RD: 210:5001 IPv4 prefix 50.10.221.0/24
                                 10.0.0.221            -       100     0       i
 * >      RD: 120:5001 IPv4 prefix 51.10.120.0/24
                                 10.0.0.120            0       100     0       ?
```

## show bgp vpn-ipv6

```text
BGP routing table information for VRF default
Router identifier 10.0.0.30, local AS number 64512
Route status codes: s - suppressed contributor, * - valid, > - active, E - ECMP head, e - ECMP
                    S - Stale, c - Contributing to ECMP, b - backup, L - labeled-unicast
                    % - Pending best path selection
Origin codes: i - IGP, e - EGP, ? - incomplete
AS Path Attributes: Or-ID - Originator ID, C-LST - Cluster List, LL Nexthop - Link Local Nexthop

          Network                Next Hop              Metric  LocPref Weight  Path
 * >      RD: 10.0.0.32:5001 IPv6 prefix 2600:50:10:32::/64
                                 ::ffff:10.0.0.32      -       100     0       i
 * >      RD: 72:5001 IPv6 prefix 2600:50:10:72::/64
                                 ::ffff:10.0.0.72      -       100     0       ?
 * >      RD: 84:5001 IPv6 prefix 2600:50:10:84::/64
                                 ::ffff:10.0.0.84      0       100     0       ?
 * >      RD: 120:5001 IPv6 prefix 2600:50:10:120::/64
                                 ::ffff:10.0.0.120     0       100     0       ?
 * >      RD: 179:5001 IPv6 prefix 2600:50:10:179::/64
                                 ::ffff:10.0.0.179     -       100     0       i
 * >      RD: 214:5001 IPv6 prefix 2600:50:10:214::/64
                                 ::ffff:10.0.0.214     -       100     0       i
 * >      RD: 217:5001 IPv6 prefix 2600:50:10:217::/64
                                 ::ffff:10.0.0.217     -       100     0       i
 * >      RD: 210:5001 IPv6 prefix 2600:50:10:221::/64
                                 ::ffff:10.0.0.221     -       100     0       i
 * >      RD: 120:5001 IPv6 prefix 2600:51:10:120::/64
                                 ::ffff:10.0.0.120     0       100     0       ?
```

## show bgp ipv4 labeled-unicast

```text
BGP routing table information for VRF default
Router identifier 10.0.0.30, local AS number 64512
Route status codes: s - suppressed contributor, * - valid, > - active, E - ECMP head, e - ECMP
                    S - Stale, c - Contributing to ECMP, b - backup, L - labeled-unicast
                    % - Pending best path selection
Origin codes: i - IGP, e - EGP, ? - incomplete
AS Path Attributes: Or-ID - Originator ID, C-LST - Cluster List, LL Nexthop - Link Local Nexthop

          Network                Next Hop              Metric  AIGP       LocPref Weight  Path
```

## show bgp neighbors

```text
BGP neighbor is 10.0.0.31, remote AS 64512, internal link
 Description: Arista-PE31-Q2C
  BGP version 4, remote router ID 0.0.0.0, VRF default
  Inherits configuration from and member of peer-group IBGP_CLIENT_PEER
  Last read never, last write never
  Hold time is 0, keepalive interval is 0 seconds
  Configured hold time is 180, keepalive interval is 60 seconds
  Effective minimum hold time is 3 seconds
  Send failure hold time is 0 seconds
  Hold timer is inactive
  Keepalive timer is inactive
  Connect timer is active, time left: 00:00:24
  Connection interval is 148 seconds
  Failed connection attempts is 21
  Idle-restart timer is inactive
  BGP state is Active
  Number of transitions to established: 0
  Last state was Connect
  Last event was TransportError
  Last sent socket-error:Connect (Network is unreachable), Last time 00:02:44, First time 00:41:17, Repeats 20
  Types of communities advertised: standard extended large
  Neighbor is a route reflector client
  Neighbor is using global cluster ID 10.0.0.30
  Neighbor Capabilities:
  Restart timer is inactive
  End of rib timer is inactive
  IPv4 Unicast AS_SET/AS_CONFED_SET processing: accept
  IPv6 Unicast AS_SET/AS_CONFED_SET processing: accept
  AIGP attribute send and receive for IPv4 Unicast are enabled
  AIGP attribute send and receive for IPv4 with MPLS Labels are enabled
  AIGP attribute send and receive for IPv6 Unicast are enabled
  AIGP attribute send and receive for IPv6 with MPLS Labels are enabled
  BGP session driven failover for IPv4 Unicast is disabled
  BGP session driven failover for IPv6 Unicast is disabled
  Message Statistics:
                         Sent      Rcvd
    Opens:                  0         0
    Notifications:          0         0
    Updates:                0         0
    Keepalives:             0         0
    Route Refresh:          0         0
    Total messages:         0         0
  Prefix Statistics:
                                   Sent      Rcvd     Best Paths     Best ECMP Paths
    IPv4 Unicast:                     0         0              0                   0
    IPv6 Unicast:                     0         0              0                   0
  Configured maximum total number of routes is 0
  Inbound updates dropped by reason:
    AS path loop detection: 0
    Cluster ID loop detection: 0
    Enforced First AS: 0
    Malformed MPBGP routes: 0
    Originator ID matches local router ID: 0
    Nexthop matches local IP address: 0
    Unexpected IPv6 nexthop for IPv4 routes: 0
    AS_SET/AS_CONFED_SET in AS_PATH for IPv4 Unicast: 0
    AS_SET/AS_CONFED_SET in AS_PATH for IPv6 Unicast: 0
  Inbound updates with attribute errors:
    Resulting in removal of all paths in update (treat as withdraw): 0
    Resulting in AFI/SAFI disable: 0
    Resulting in attribute ignore: 0
    Disabled AFI/SAFIs: None
  Inbound paths dropped by reason:
    IPv4 unicast NLRIs dropped due to martian prefix: 0
    IPv6 unicast NLRIs dropped due to martian prefix: 0
    IPv4 labeled-unicast NLRIs dropped due to excessive labels: 0
    IPv4 labeled-unicast NLRIs dropped due to martian prefix: 0
    IPv6 labeled-unicast NLRIs dropped due to excessive labels: 0
    IPv6 labeled-unicast NLRIs dropped due to martian prefix: 0
    VPN-IPv4 NLRIs dropped due to route import match failure: 0
    VPN-IPv6 NLRIs dropped due to route import match failure: 0
    L2VPN EVPN NLRIs dropped due to route import match failure: 0
    L2VPN EVPN NLRIs dropped due to unsupported route type: 0
    Link-state NLRIs dropped because reception is unsupported: 0
    RT Membership NLRIs dropped due to local origin ASN received from external peer: 0
  Outbound paths dropped by reason:
    IPv4 local address not available: 0
    IPv6 local address not available: 0
Local AS is 64512, local router ID 10.0.0.30
TTL is 255
Local TCP address is 10.0.0.30
Remote TCP address is 10.0.0.31, remote port is 179

BGP neighbor is 10.0.0.32, remote AS 64512, internal link
 Description: Arista-PE32-Q2C
  BGP version 4, remote router ID 10.0.0.32, VRF default
  Inherits configuration from and member of peer-group IBGP_CLIENT_PEER
  Last read 00:00:13, last write 00:00:08
  Hold time is 180, keepalive interval is 60 seconds
  Configured hold time is 180, keepalive interval is 60 seconds
  Effective minimum hold time is 3 seconds
  Send failure hold time is 0 seconds
  Hold timer is active, time left: 00:02:47
  Keepalive timer is active, time left: 00:00:50
  Connect timer is inactive
  Idle-restart timer is inactive
  BGP state is Established, up for 00:30:30
  Number of transitions to established: 1
  Last state was OpenConfirm
  Last event was RecvUpdate
  Last sent socket-error:Connect (Network is unreachable), Last time 00:31:55, First time 00:41:17, Repeats 10
  Types of communities advertised: standard extended large
  Enhanced route refresh stale path removal disabled
  Outbound enhanced route refresh enabled
  Neighbor is a route reflector client
  Neighbor is using global cluster ID 10.0.0.30
  Neighbor Capabilities:
    Multiprotocol VPN-IPv4: advertised and received and negotiated
    Multiprotocol VPN-IPv6: advertised and received and negotiated
    Four Octet ASN: advertised and received and negotiated
    Route Refresh: advertised and received and negotiated
    Enhanced route refresh: advertised and received and negotiated
    Send End-of-RIB messages: advertised and received and negotiated
    Additional-paths recv capability:
      VPN-IPv4: advertised
      VPN-IPv6: advertised
    Additional-paths send capability:
      VPN-IPv4: received
      VPN-IPv6: received
    Graceful Restart advertised:
      Restart-time is 120
      Restart-State bit: no
      Graceful notification: yes
      VPN-IPv4 is enabled, Forwarding State is not preserved
      VPN-IPv6 is enabled, Forwarding State is not preserved
    Graceful Restart received:
      Restart-time is 120
      Restart-State bit: no
      Graceful notification: yes
      VPN-IPv4 is enabled, Forwarding State is not preserved
      VPN-IPv6 is enabled, Forwarding State is not preserved
  Restart timer is inactive
  End of rib timer is inactive
    VPN-IPv4 End-of-RIB received: Yes
      Received 00:30:30
      Number of stale paths removed after graceful restart: 0
      Number of paths received before End-of-RIB: 1
    VPN-IPv6 End-of-RIB received: Yes
      Received 00:30:30
      Number of stale paths removed after graceful restart: 0
      Number of paths received before End-of-RIB: 1
  IPv4 Unicast AS_SET/AS_CONFED_SET processing: accept
  IPv6 Unicast AS_SET/AS_CONFED_SET processing: accept
  AIGP attribute send and receive for IPv4 Unicast are enabled
  AIGP attribute send and receive for IPv4 with MPLS Labels are enabled
  AIGP attribute send and receive for IPv6 Unicast are enabled
  AIGP attribute send and receive for IPv6 with MPLS Labels are enabled
  BGP session driven failover for IPv4 Unicast is disabled
  BGP session driven failover for IPv6 Unicast is disabled
  Message Statistics:
                                  Sent      Rcvd
    Opens:                           1         1
    Notifications:                   0         0
    Updates:                        24        12
    Keepalives:                     35        36
    Enhanced Route Refresh:          0         0
    Begin of Route Refresh:          0         0
    End of Route Refresh:            0         0
    Total messages:                 60        49
  Prefix Statistics:
                                   Sent      Rcvd     Best Paths     Best ECMP Paths
    IPv4 Unicast:                     0         0              0                   0
    VPN-IPv4:                         8         1              1                   0
    IPv6 Unicast:                     0         0              0                   0
    VPN-IPv6:                         8         1              1                   0
  Configured maximum total number of routes is 0
  Inbound updates dropped by reason:
    AS path loop detection: 0
    Cluster ID loop detection: 0
    Enforced First AS: 0
    Malformed MPBGP routes: 0
    Originator ID matches local router ID: 0
    Nexthop matches local IP address: 0
    Unexpected IPv6 nexthop for IPv4 routes: 0
    AS_SET/AS_CONFED_SET in AS_PATH for IPv4 Unicast: 0
    AS_SET/AS_CONFED_SET in AS_PATH for IPv6 Unicast: 0
  Inbound updates with attribute errors:
    Resulting in removal of all paths in update (treat as withdraw): 0
    Resulting in AFI/SAFI disable: 0
    Resulting in attribute ignore: 0
    Disabled AFI/SAFIs: None
  Inbound paths dropped by reason:
    IPv4 unicast NLRIs dropped due to martian prefix: 0
    IPv6 unicast NLRIs dropped due to martian prefix: 0
    IPv4 labeled-unicast NLRIs dropped due to excessive labels: 0
    IPv4 labeled-unicast NLRIs dropped due to martian prefix: 0
    IPv6 labeled-unicast NLRIs dropped due to excessive labels: 0
    IPv6 labeled-unicast NLRIs dropped due to martian prefix: 0
    VPN-IPv4 NLRIs dropped due to route import match failure: 0
    VPN-IPv4 NLRIs dropped due to maximum route limit violation: 0
    VPN-IPv6 NLRIs dropped due to route import match failure: 0
    VPN-IPv6 NLRIs dropped due to maximum route limit violation: 0
    L2VPN EVPN NLRIs dropped due to route import match failure: 0
    L2VPN EVPN NLRIs dropped due to unsupported route type: 0
    Link-state NLRIs dropped because reception is unsupported: 0
    RT Membership NLRIs dropped due to local origin ASN received from external peer: 0
  Outbound paths dropped by reason:
    IPv4 local address not available: 0
    IPv6 local address not available: 0
Local AS is 64512, local router ID 10.0.0.30
TTL is 255
Local TCP address is 10.0.0.30, local port is 39565
Remote TCP address is 10.0.0.32, remote port is 179
Local next hop for next hop self:
  VPN-IPv4: 10.0.0.30
  VPN-IPv6: ::ffff:10.0.0.30
TCP Socket Information:
  TCP state is ESTABLISHED
  Recv-Q: 0/32768
  Send-Q: 0/46080
  Outgoing Maximum Segment Size (MSS): 1448
  Total Number of TCP retransmissions: 0
  Options:
    Timestamps enabled: yes
    Selective Acknowledgments enabled: yes
    Window Scale enabled: yes
    Explicit Congestion Notification (ECN) enabled: no
  Socket Statistics:
    Window Scale (wscale): 7,7
    Retransmission Timeout (rto): 204.0ms
    Round-trip Time (rtt/rtvar): 0.3ms/0.1ms
    Delayed Ack Timeout (ato): 40.0ms
    Congestion Window (cwnd): 10
    TCP Throughput: 392.68 Mbps
    Advertised Recv Window (rcv_space): 14480

BGP neighbor is 10.0.0.53, remote AS 64512, internal link
 Description: Arrcus-53
  BGP version 4, remote router ID 0.0.0.0, VRF default
  Inherits configuration from and member of peer-group IBGP_CLIENT_PEER
  Last read 00:00:04, last write 00:00:04
  Hold time is 0, keepalive interval is 0 seconds
  Configured hold time is 180, keepalive interval is 60 seconds
  Effective minimum hold time is 3 seconds
  Send failure hold time is 0 seconds
  Hold timer is inactive
  Keepalive timer is inactive
  Connect timer is active, time left: 00:01:03
  Connection interval is 64 seconds
  Failed connection attempts is 6
  Idle-restart timer is inactive
  BGP state is Active
  Peering failure hint: Open Message Error/bad AS number
  Number of transitions to established: 0
  Last state was Idle
  Last event was Start
  Last sent notification:Open Message Error/bad AS number, Last time 00:00:04, First time 00:41:18, Repeats 495
  Types of communities advertised: standard extended large
  Neighbor is a route reflector client
  Neighbor is using global cluster ID 10.0.0.30
  Neighbor Capabilities:
    Multiprotocol VPN-IPv4: advertised
    Multiprotocol VPN-IPv6: advertised
    Four Octet ASN: advertised
    Route Refresh: advertised
    Enhanced route refresh: advertised
    Send End-of-RIB messages: advertised
    Additional-paths recv capability:
      VPN-IPv4: advertised
      VPN-IPv6: advertised
    Additional-paths send capability:
    Graceful Restart advertised:
      Restart-time is 120
      Restart-State bit: no
      Graceful notification: yes
      VPN-IPv4 is enabled, Forwarding State is not preserved
      VPN-IPv6 is enabled, Forwarding State is not preserved
  Restart timer is inactive
  End of rib timer is inactive
  IPv4 Unicast AS_SET/AS_CONFED_SET processing: accept
  IPv6 Unicast AS_SET/AS_CONFED_SET processing: accept
  AIGP attribute send and receive for IPv4 Unicast are enabled
  AIGP attribute send and receive for IPv4 with MPLS Labels are enabled
  AIGP attribute send and receive for IPv6 Unicast are enabled
  AIGP attribute send and receive for IPv6 with MPLS Labels are enabled
  BGP session driven failover for IPv4 Unicast is disabled
  BGP session driven failover for IPv6 Unicast is disabled
  Message Statistics:
                         Sent      Rcvd
    Opens:                496       496
    Notifications:        496         0
    Updates:                0         0
    Keepalives:             0         0
    Route Refresh:          0         0
    Total messages:       992       496
  Prefix Statistics:
                                   Sent      Rcvd     Best Paths     Best ECMP Paths
    IPv4 Unicast:                     0         0              0                   0
    IPv6 Unicast:                     0         0              0                   0
  Configured maximum total number of routes is 0
  Inbound updates dropped by reason:
    AS path loop detection: 0
    Cluster ID loop detection: 0
    Enforced First AS: 0
    Malformed MPBGP routes: 0
    Originator ID matches local router ID: 0
    Nexthop matches local IP address: 0
    Unexpected IPv6 nexthop for IPv4 routes: 0
    AS_SET/AS_CONFED_SET in AS_PATH for IPv4 Unicast: 0
    AS_SET/AS_CONFED_SET in AS_PATH for IPv6 Unicast: 0
  Inbound updates with attribute errors:
    Resulting in removal of all paths in update (treat as withdraw): 0
    Resulting in AFI/SAFI disable: 0
    Resulting in attribute ignore: 0
    Disabled AFI/SAFIs: None
  Inbound paths dropped by reason:
    IPv4 unicast NLRIs dropped due to martian prefix: 0
    IPv6 unicast NLRIs dropped due to martian prefix: 0
    IPv4 labeled-unicast NLRIs dropped due to excessive labels: 0
    IPv4 labeled-unicast NLRIs dropped due to martian prefix: 0
    IPv6 labeled-unicast NLRIs dropped due to excessive labels: 0
    IPv6 labeled-unicast NLRIs dropped due to martian prefix: 0
    VPN-IPv4 NLRIs dropped due to route import match failure: 0
    VPN-IPv6 NLRIs dropped due to route import match failure: 0
    L2VPN EVPN NLRIs dropped due to route import match failure: 0
    L2VPN EVPN NLRIs dropped due to unsupported route type: 0
    Link-state NLRIs dropped because reception is unsupported: 0
    RT Membership NLRIs dropped due to local origin ASN received from external peer: 0
  Outbound paths dropped by reason:
    IPv4 local address not available: 0
    IPv6 local address not available: 0
Local AS is 64512, local router ID 10.0.0.30
TTL is 255
Local TCP address is 10.0.0.30
Remote TCP address is 10.0.0.53, remote port is 179

BGP neighbor is 10.0.0.66, remote AS 64512, internal link
 Description: Ciena-8140-66
  BGP version 4, remote router ID 10.0.0.66, VRF default
  Inherits configuration from and member of peer-group IBGP_CLIENT_PEER
  Last read 00:16:57, last write 00:13:57
  Hold time is 180, keepalive interval is 60 seconds
  Configured hold time is 180, keepalive interval is 60 seconds
  Effective minimum hold time is 3 seconds
  Send failure hold time is 0 seconds
  Hold timer is inactive
  Keepalive timer is inactive
  Connect timer is active, time left: 00:01:47
  Connection interval is 148 seconds
  Failed connection attempts is 12
  Idle-restart timer is inactive
  BGP state is Active
  Number of transitions to established: 1
  Last state was Connect
  Last event was TransportError
  Last sent notification:Hold Timer Expired Error/None, Last time 00:13:57
  Last sent socket-error:Connect (Network is unreachable), Last time 00:01:09, First time 00:41:18, Repeats 22
  Types of communities advertised: standard extended large
  Neighbor is a route reflector client
  Neighbor is using global cluster ID 10.0.0.30
  Neighbor Capabilities:
    Multiprotocol IPv4 Unicast: received
    Multiprotocol VPN-IPv4: advertised and received
    Multiprotocol VPN-IPv6: advertised and received
    Four Octet ASN: advertised
    Route Refresh: advertised and received
    Enhanced route refresh: advertised
    Send End-of-RIB messages: advertised and received
    Additional-paths recv capability:
      VPN-IPv4: advertised
      VPN-IPv6: advertised
    Additional-paths send capability:
    Graceful Restart advertised:
      Restart-time is 120
      Restart-State bit: no
      Graceful notification: yes
      VPN-IPv4 is enabled, Forwarding State is not preserved
      VPN-IPv6 is enabled, Forwarding State is not preserved
    Graceful Restart received:
      Restart-time is 0
      Restart-State bit: no
      Graceful notification: no
      IPv4 Unicast is enabled, Forwarding State is not preserved
      VPN-IPv4 is enabled, Forwarding State is not preserved
      VPN-IPv6 is enabled, Forwarding State is not preserved
  Restart timer is inactive
  End of rib timer is inactive
  IPv4 Unicast AS_SET/AS_CONFED_SET processing: accept
  IPv6 Unicast AS_SET/AS_CONFED_SET processing: accept
  AIGP attribute send and receive for IPv4 Unicast are enabled
  AIGP attribute send and receive for IPv4 with MPLS Labels are enabled
  AIGP attribute send and receive for IPv6 Unicast are enabled
  AIGP attribute send and receive for IPv6 with MPLS Labels are enabled
  BGP session driven failover for IPv4 Unicast is disabled
  BGP session driven failover for IPv6 Unicast is disabled
  Message Statistics:
                         Sent      Rcvd
    Opens:                  1         1
    Notifications:          1         0
    Updates:               18         4
    Keepalives:            22        16
    Route Refresh:          0         0
    Total messages:        42        21
  Prefix Statistics:
                                   Sent      Rcvd     Best Paths     Best ECMP Paths
    IPv4 Unicast:                     0         0              0                   0
    IPv6 Unicast:                     0         0              0                   0
  Configured maximum total number of routes is 0
  Inbound updates dropped by reason:
    AS path loop detection: 0
    Cluster ID loop detection: 0
    Enforced First AS: 0
    Malformed MPBGP routes: 0
    Originator ID matches local router ID: 0
    Nexthop matches local IP address: 0
    Unexpected IPv6 nexthop for IPv4 routes: 0
    AS_SET/AS_CONFED_SET in AS_PATH for IPv4 Unicast: 0
    AS_SET/AS_CONFED_SET in AS_PATH for IPv6 Unicast: 0
  Inbound updates with attribute errors:
    Resulting in removal of all paths in update (treat as withdraw): 0
    Resulting in AFI/SAFI disable: 0
    Resulting in attribute ignore: 0
    Disabled AFI/SAFIs: None
  Inbound paths dropped by reason:
    IPv4 unicast NLRIs dropped due to martian prefix: 0
    IPv6 unicast NLRIs dropped due to martian prefix: 0
    IPv4 labeled-unicast NLRIs dropped due to excessive labels: 0
    IPv4 labeled-unicast NLRIs dropped due to martian prefix: 0
    IPv6 labeled-unicast NLRIs dropped due to excessive labels: 0
    IPv6 labeled-unicast NLRIs dropped due to martian prefix: 0
    VPN-IPv4 NLRIs dropped due to route import match failure: 0
    VPN-IPv6 NLRIs dropped due to route import match failure: 0
    L2VPN EVPN NLRIs dropped due to route import match failure: 0
    L2VPN EVPN NLRIs dropped due to unsupported route type: 0
    Link-state NLRIs dropped because reception is unsupported: 0
    RT Membership NLRIs dropped due to local origin ASN received from external peer: 0
  Outbound paths dropped by reason:
    IPv4 local address not available: 0
    IPv6 local address not available: 0
Local AS is 64512, local router ID 10.0.0.30
TTL is 255
Local TCP address is 10.0.0.30
Remote TCP address is 10.0.0.66, remote port is 179

BGP neighbor is 10.0.0.72, remote AS 64512, internal link
 Description: Ciena-5134-72
  BGP version 4, remote router ID 10.0.0.72, VRF default
  Inherits configuration from and member of peer-group IBGP_CLIENT_PEER
  Last read 00:00:42, last write 00:00:13
  Hold time is 180, keepalive interval is 60 seconds
  Configured hold time is 180, keepalive interval is 60 seconds
  Effective minimum hold time is 3 seconds
  Send failure hold time is 0 seconds
  Hold timer is active, time left: 00:02:18
  Keepalive timer is active, time left: 00:00:32
  Connect timer is inactive
  Idle-restart timer is inactive
  BGP state is Established, up for 00:31:42
  Number of transitions to established: 1
  Last state was OpenConfirm
  Last event was RecvUpdate
  Last sent socket-error:Connect (Network is unreachable), Last time 00:31:54, First time 00:41:18, Repeats 11
  Types of communities advertised: standard extended large
  Neighbor is a route reflector client
  Neighbor is using global cluster ID 10.0.0.30
  Neighbor Capabilities:
    Multiprotocol IPv4 Unicast: received
    Multiprotocol VPN-IPv4: advertised and received and negotiated
    Multiprotocol VPN-IPv6: advertised and received and negotiated
    Four Octet ASN: advertised
    Route Refresh: advertised and received and negotiated
    Enhanced route refresh: advertised
    Send End-of-RIB messages: advertised and received and negotiated
    Additional-paths recv capability:
      VPN-IPv4: advertised
      VPN-IPv6: advertised
    Additional-paths send capability:
    Graceful Restart advertised:
      Restart-time is 120
      Restart-State bit: no
      Graceful notification: yes
      VPN-IPv4 is enabled, Forwarding State is not preserved
      VPN-IPv6 is enabled, Forwarding State is not preserved
    Graceful Restart received:
      Restart-time is 0
      Restart-State bit: no
      Graceful notification: no
      IPv4 Unicast is enabled, Forwarding State is not preserved
      VPN-IPv4 is enabled, Forwarding State is not preserved
      VPN-IPv6 is enabled, Forwarding State is not preserved
  Restart timer is inactive
  End of rib timer is inactive
    VPN-IPv4 End-of-RIB received: Yes
      Received 00:31:32
      Number of stale paths removed after graceful restart: 0
      Number of paths received before End-of-RIB: 1
    VPN-IPv6 End-of-RIB received: Yes
      Received 00:31:32
      Number of stale paths removed after graceful restart: 0
      Number of paths received before End-of-RIB: 1
  IPv4 Unicast AS_SET/AS_CONFED_SET processing: accept
  IPv6 Unicast AS_SET/AS_CONFED_SET processing: accept
  AIGP attribute send and receive for IPv4 Unicast are enabled
  AIGP attribute send and receive for IPv4 with MPLS Labels are enabled
  AIGP attribute send and receive for IPv6 Unicast are enabled
  AIGP attribute send and receive for IPv6 with MPLS Labels are enabled
  BGP session driven failover for IPv4 Unicast is disabled
  BGP session driven failover for IPv6 Unicast is disabled
  Message Statistics:
                         Sent      Rcvd
    Opens:                  1         1
    Notifications:          0         0
    Updates:               28         4
    Keepalives:            35        32
    Route Refresh:          0         0
    Total messages:        64        37
  Prefix Statistics:
                                   Sent      Rcvd     Best Paths     Best ECMP Paths
    IPv4 Unicast:                     0         0              0                   0
    VPN-IPv4:                         8         1              1                   0
    IPv6 Unicast:                     0         0              0                   0
    VPN-IPv6:                         8         1              1                   0
  Configured maximum total number of routes is 0
  Inbound updates dropped by reason:
    AS path loop detection: 0
    Cluster ID loop detection: 0
    Enforced First AS: 0
    Malformed MPBGP routes: 0
    Originator ID matches local router ID: 0
    Nexthop matches local IP address: 0
    Unexpected IPv6 nexthop for IPv4 routes: 0
    AS_SET/AS_CONFED_SET in AS_PATH for IPv4 Unicast: 0
    AS_SET/AS_CONFED_SET in AS_PATH for IPv6 Unicast: 0
  Inbound updates with attribute errors:
    Resulting in removal of all paths in update (treat as withdraw): 0
    Resulting in AFI/SAFI disable: 0
    Resulting in attribute ignore: 0
    Disabled AFI/SAFIs: None
  Inbound paths dropped by reason:
    IPv4 unicast NLRIs dropped due to martian prefix: 0
    IPv6 unicast NLRIs dropped due to martian prefix: 0
    IPv4 labeled-unicast NLRIs dropped due to excessive labels: 0
    IPv4 labeled-unicast NLRIs dropped due to martian prefix: 0
    IPv6 labeled-unicast NLRIs dropped due to excessive labels: 0
    IPv6 labeled-unicast NLRIs dropped due to martian prefix: 0
    VPN-IPv4 NLRIs dropped due to route import match failure: 0
    VPN-IPv4 NLRIs dropped due to maximum route limit violation: 0
    VPN-IPv6 NLRIs dropped due to route import match failure: 0
    VPN-IPv6 NLRIs dropped due to maximum route limit violation: 0
    L2VPN EVPN NLRIs dropped due to route import match failure: 0
    L2VPN EVPN NLRIs dropped due to unsupported route type: 0
    Link-state NLRIs dropped because reception is unsupported: 0
    RT Membership NLRIs dropped due to local origin ASN received from external peer: 0
  Outbound paths dropped by reason:
    IPv4 local address not available: 0
    IPv6 local address not available: 0
Local AS is 64512, local router ID 10.0.0.30
TTL is 255
Local TCP address is 10.0.0.30, local port is 38625
Remote TCP address is 10.0.0.72, remote port is 179
Local next hop for next hop self:
  VPN-IPv4: 10.0.0.30
  VPN-IPv6: ::ffff:10.0.0.30
TCP Socket Information:
  TCP state is ESTABLISHED
  Recv-Q: 0/32768
  Send-Q: 0/46080
  Outgoing Maximum Segment Size (MSS): 1460
  Total Number of TCP retransmissions: 3
  Options:
    Timestamps enabled: no
    Selective Acknowledgments enabled: yes
    Window Scale enabled: yes
    Explicit Congestion Notification (ECN) enabled: no
  Socket Statistics:
    Window Scale (wscale): 7,7
    Retransmission Timeout (rto): 204.0ms
    Round-trip Time (rtt/rtvar): 0.7ms/0.0ms
    Delayed Ack Timeout (ato): 40.0ms
    Congestion Window (cwnd): 2
    TCP Throughput: 35.13 Mbps
    Advertised Recv Window (rcv_space): 14600

BGP neighbor is 10.0.0.84, remote AS 64512, internal link
 Description: Ericsson_84
  BGP version 4, remote router ID 10.0.0.84, VRF default
  Inherits configuration from and member of peer-group IBGP_CLIENT_PEER
  Last read 00:00:28, last write 00:00:42
  Hold time is 180, keepalive interval is 60 seconds
  Configured hold time is 180, keepalive interval is 60 seconds
  Effective minimum hold time is 3 seconds
  Send failure hold time is 0 seconds
  Hold timer is active, time left: 00:02:32
  Keepalive timer is active, time left: 00:00:06
  Connect timer is inactive
  Idle-restart timer is inactive
  BGP state is Established, up for 00:41:18
  Number of transitions to established: 1
  Last state was OpenConfirm
  Last event was RecvUpdate
  Types of communities advertised: standard extended large
  Enhanced route refresh stale path removal disabled
  Outbound enhanced route refresh enabled
  Neighbor is a route reflector client
  Neighbor is using global cluster ID 10.0.0.30
  Neighbor Capabilities:
    Multiprotocol IPv4 Unicast: received
    Multiprotocol VPN-IPv4: advertised and received and negotiated
    Multiprotocol IPv6 Unicast: received
    Multiprotocol VPN-IPv6: advertised and received and negotiated
    Four Octet ASN: advertised and received and negotiated
    Route Refresh: advertised and received and negotiated
    Enhanced route refresh: advertised and received and negotiated
    Send End-of-RIB messages: advertised and received and negotiated
    Additional-paths recv capability:
      VPN-IPv4: advertised
      VPN-IPv6: advertised
    Additional-paths send capability:
    Graceful Restart advertised:
      Restart-time is 120
      Restart-State bit: yes
      Graceful notification: yes
      VPN-IPv4 is enabled, Forwarding State is not preserved
      VPN-IPv6 is enabled, Forwarding State is not preserved
    Graceful Restart received:
      Restart-time is 120
      Restart-State bit: no
      Graceful notification: no
      IPv4 Unicast is enabled, Forwarding State is preserved
      VPN-IPv4 is enabled, Forwarding State is preserved
      IPv6 Unicast is enabled, Forwarding State is preserved
      VPN-IPv6 is enabled, Forwarding State is preserved
  Restart timer is inactive
  End of rib timer is inactive
    VPN-IPv4 End-of-RIB received: Yes
      Received 00:41:18
      Number of stale paths removed after graceful restart: 0
      Number of paths received before End-of-RIB: 1
    VPN-IPv6 End-of-RIB received: Yes
      Received 00:41:18
      Number of stale paths removed after graceful restart: 0
      Number of paths received before End-of-RIB: 1
  IPv4 Unicast AS_SET/AS_CONFED_SET processing: accept
  IPv6 Unicast AS_SET/AS_CONFED_SET processing: accept
  AIGP attribute send and receive for IPv4 Unicast are enabled
  AIGP attribute send and receive for IPv4 with MPLS Labels are enabled
  AIGP attribute send and receive for IPv6 Unicast are enabled
  AIGP attribute send and receive for IPv6 with MPLS Labels are enabled
  BGP session driven failover for IPv4 Unicast is disabled
  BGP session driven failover for IPv6 Unicast is disabled
  Message Statistics:
                                  Sent      Rcvd
    Opens:                           1         1
    Notifications:                   0         0
    Updates:                        28         4
    Keepalives:                     45        42
    Enhanced Route Refresh:          0         0
    Begin of Route Refresh:          0         0
    End of Route Refresh:            0         0
    Total messages:                 74        47
  Prefix Statistics:
                                   Sent      Rcvd     Best Paths     Best ECMP Paths
    IPv4 Unicast:                     0         0              0                   0
    VPN-IPv4:                         8         1              1                   0
    IPv6 Unicast:                     0         0              0                   0
    VPN-IPv6:                         8         1              1                   0
  Configured maximum total number of routes is 0
  Inbound updates dropped by reason:
    AS path loop detection: 0
    Cluster ID loop detection: 0
    Enforced First AS: 0
    Malformed MPBGP routes: 0
    Originator ID matches local router ID: 0
    Nexthop matches local IP address: 0
    Unexpected IPv6 nexthop for IPv4 routes: 0
    AS_SET/AS_CONFED_SET in AS_PATH for IPv4 Unicast: 0
    AS_SET/AS_CONFED_SET in AS_PATH for IPv6 Unicast: 0
  Inbound updates with attribute errors:
    Resulting in removal of all paths in update (treat as withdraw): 0
    Resulting in AFI/SAFI disable: 0
    Resulting in attribute ignore: 0
    Disabled AFI/SAFIs: None
  Inbound paths dropped by reason:
    IPv4 unicast NLRIs dropped due to martian prefix: 0
    IPv6 unicast NLRIs dropped due to martian prefix: 0
    IPv4 labeled-unicast NLRIs dropped due to excessive labels: 0
    IPv4 labeled-unicast NLRIs dropped due to martian prefix: 0
    IPv6 labeled-unicast NLRIs dropped due to excessive labels: 0
    IPv6 labeled-unicast NLRIs dropped due to martian prefix: 0
    VPN-IPv4 NLRIs dropped due to route import match failure: 0
    VPN-IPv4 NLRIs dropped due to maximum route limit violation: 0
    VPN-IPv6 NLRIs dropped due to route import match failure: 0
    VPN-IPv6 NLRIs dropped due to maximum route limit violation: 0
    L2VPN EVPN NLRIs dropped due to route import match failure: 0
    L2VPN EVPN NLRIs dropped due to unsupported route type: 0
    Link-state NLRIs dropped because reception is unsupported: 0
    RT Membership NLRIs dropped due to local origin ASN received from external peer: 0
  Outbound paths dropped by reason:
    IPv4 local address not available: 0
    IPv6 local address not available: 0
Local AS is 64512, local router ID 10.0.0.30
TTL is 255
Local TCP address is 10.0.0.30, local port is 46271
Remote TCP address is 10.0.0.84, remote port is 179
Local next hop for next hop self:
  VPN-IPv4: 10.0.0.30
  VPN-IPv6: ::ffff:10.0.0.30
TCP Socket Information:
  TCP state is ESTABLISHED
  Recv-Q: 0/32768
  Send-Q: 0/46080
  Outgoing Maximum Segment Size (MSS): 1428
  Total Number of TCP retransmissions: 1
  Options:
    Timestamps enabled: yes
    Selective Acknowledgments enabled: yes
    Window Scale enabled: yes
    Explicit Congestion Notification (ECN) enabled: no
  Socket Statistics:
    Window Scale (wscale): 0,7
    Retransmission Timeout (rto): 432.0ms
    Round-trip Time (rtt/rtvar): 231.9ms/0.3ms
    Delayed Ack Timeout (ato): 40.0ms
    Congestion Window (cwnd): 10
    TCP Throughput: 0.49 Mbps
    Advertised Recv Window (rcv_space): 14480

BGP neighbor is 10.0.0.120, remote AS 64512, internal link
 Description: Huawei_120
  BGP version 4, remote router ID 10.0.0.120, VRF default
  Inherits configuration from and member of peer-group IBGP_CLIENT_PEER
  Last read 00:00:06, last write 00:00:26
  Hold time is 180, keepalive interval is 60 seconds
  Configured hold time is 180, keepalive interval is 60 seconds
  Effective minimum hold time is 3 seconds
  Send failure hold time is 0 seconds
  Hold timer is active, time left: 00:02:54
  Keepalive timer is active, time left: 00:00:22
  Connect timer is inactive
  Idle-restart timer is inactive
  BGP state is Established, up for 00:41:07
  Number of transitions to established: 1
  Last state was OpenConfirm
  Last event was RecvKeepAlive
  Last sent socket-error:Connect (Connection refused), Last time 00:41:08, First time 00:41:18, Repeats 2
  Types of communities advertised: standard extended large
  Neighbor is a route reflector client
  Neighbor is using global cluster ID 10.0.0.30
  Neighbor Capabilities:
    Multiprotocol VPN-IPv4: advertised and received and negotiated
    Multiprotocol VPN-IPv6: advertised and received and negotiated
    Four Octet ASN: advertised and received and negotiated
    Route Refresh: advertised and received and negotiated
    Enhanced route refresh: advertised
    Send End-of-RIB messages: advertised
    Additional-paths recv capability:
      VPN-IPv4: advertised
      VPN-IPv6: advertised
    Additional-paths send capability:
    Graceful Restart advertised:
      Restart-time is 120
      Restart-State bit: yes
      Graceful notification: yes
      VPN-IPv4 is enabled, Forwarding State is not preserved
      VPN-IPv6 is enabled, Forwarding State is not preserved
  Restart timer is inactive
  End of rib timer is inactive
    VPN-IPv4 End-of-RIB received: No
      Number of stale paths removed after graceful restart: 0
    VPN-IPv6 End-of-RIB received: No
      Number of stale paths removed after graceful restart: 0
  IPv4 Unicast AS_SET/AS_CONFED_SET processing: accept
  IPv6 Unicast AS_SET/AS_CONFED_SET processing: accept
  AIGP attribute send and receive for IPv4 Unicast are enabled
  AIGP attribute send and receive for IPv4 with MPLS Labels are enabled
  AIGP attribute send and receive for IPv6 Unicast are enabled
  AIGP attribute send and receive for IPv6 with MPLS Labels are enabled
  BGP session driven failover for IPv4 Unicast is disabled
  BGP session driven failover for IPv6 Unicast is disabled
  Message Statistics:
                         Sent      Rcvd
    Opens:                  1         1
    Notifications:          0         0
    Updates:               24        13
    Keepalives:            46        51
    Route Refresh:          0         0
    Total messages:        71        65
  Prefix Statistics:
                                   Sent      Rcvd     Best Paths     Best ECMP Paths
    IPv4 Unicast:                     0         0              0                   0
    VPN-IPv4:                         7         2              2                   0
    IPv6 Unicast:                     0         0              0                   0
    VPN-IPv6:                         7         2              2                   0
  Configured maximum total number of routes is 0
  Inbound updates dropped by reason:
    AS path loop detection: 0
    Cluster ID loop detection: 0
    Enforced First AS: 0
    Malformed MPBGP routes: 0
    Originator ID matches local router ID: 0
    Nexthop matches local IP address: 0
    Unexpected IPv6 nexthop for IPv4 routes: 0
    AS_SET/AS_CONFED_SET in AS_PATH for IPv4 Unicast: 0
    AS_SET/AS_CONFED_SET in AS_PATH for IPv6 Unicast: 0
  Inbound updates with attribute errors:
    Resulting in removal of all paths in update (treat as withdraw): 0
    Resulting in AFI/SAFI disable: 0
    Resulting in attribute ignore: 0
    Disabled AFI/SAFIs: None
  Inbound paths dropped by reason:
    IPv4 unicast NLRIs dropped due to martian prefix: 0
    IPv6 unicast NLRIs dropped due to martian prefix: 0
    IPv4 labeled-unicast NLRIs dropped due to excessive labels: 0
    IPv4 labeled-unicast NLRIs dropped due to martian prefix: 0
    IPv6 labeled-unicast NLRIs dropped due to excessive labels: 0
    IPv6 labeled-unicast NLRIs dropped due to martian prefix: 0
    VPN-IPv4 NLRIs dropped due to route import match failure: 0
    VPN-IPv4 NLRIs dropped due to maximum route limit violation: 0
    VPN-IPv6 NLRIs dropped due to route import match failure: 0
    VPN-IPv6 NLRIs dropped due to maximum route limit violation: 0
    L2VPN EVPN NLRIs dropped due to route import match failure: 0
    L2VPN EVPN NLRIs dropped due to unsupported route type: 0
    Link-state NLRIs dropped because reception is unsupported: 0
    RT Membership NLRIs dropped due to local origin ASN received from external peer: 0
  Outbound paths dropped by reason:
    IPv4 local address not available: 0
    IPv6 local address not available: 0
Local AS is 64512, local router ID 10.0.0.30
TTL is 255
Local TCP address is 10.0.0.30, local port is 179
Remote TCP address is 10.0.0.120, remote port is 32598
Local next hop for next hop self:
  VPN-IPv4: 10.0.0.30
  VPN-IPv6: ::ffff:10.0.0.30
TCP Socket Information:
  TCP state is ESTABLISHED
  Recv-Q: 0/32768
  Send-Q: 0/46080
  Outgoing Maximum Segment Size (MSS): 1384
  Total Number of TCP retransmissions: 0
  Options:
    Timestamps enabled: yes
    Selective Acknowledgments enabled: yes
    Window Scale enabled: yes
    Explicit Congestion Notification (ECN) enabled: no
  Socket Statistics:
    Window Scale (wscale): 3,7
    Retransmission Timeout (rto): 204.0ms
    Round-trip Time (rtt/rtvar): 0.3ms/0.1ms
    Delayed Ack Timeout (ato): 40.0ms
    Congestion Window (cwnd): 10
    TCP Throughput: 331.50 Mbps
    Advertised Recv Window (rcv_space): 14600

BGP neighbor is 10.0.0.124, remote AS 64512, internal link
 Description: Huawei_124
  BGP version 4, remote router ID 0.0.0.0, VRF default
  Inherits configuration from and member of peer-group IBGP_CLIENT_PEER
  Last read never, last write never
  Hold time is 0, keepalive interval is 0 seconds
  Configured hold time is 180, keepalive interval is 60 seconds
  Effective minimum hold time is 3 seconds
  Send failure hold time is 0 seconds
  Hold timer is inactive
  Keepalive timer is inactive
  Connect timer is active, time left: 00:01:51
  Connection interval is 148 seconds
  Failed connection attempts is 22
  Idle-restart timer is inactive
  BGP state is Active
  Number of transitions to established: 0
  Last state was Connect
  Last event was TransportError
  Last sent socket-error:Connect (Network is unreachable), Last time 00:00:56, First time 00:41:18, Repeats 21
  Types of communities advertised: standard extended large
  Neighbor is a route reflector client
  Neighbor is using global cluster ID 10.0.0.30
  Neighbor Capabilities:
  Restart timer is inactive
  End of rib timer is inactive
  IPv4 Unicast AS_SET/AS_CONFED_SET processing: accept
  IPv6 Unicast AS_SET/AS_CONFED_SET processing: accept
  AIGP attribute send and receive for IPv4 Unicast are enabled
  AIGP attribute send and receive for IPv4 with MPLS Labels are enabled
  AIGP attribute send and receive for IPv6 Unicast are enabled
  AIGP attribute send and receive for IPv6 with MPLS Labels are enabled
  BGP session driven failover for IPv4 Unicast is disabled
  BGP session driven failover for IPv6 Unicast is disabled
  Message Statistics:
                         Sent      Rcvd
    Opens:                  0         0
    Notifications:          0         0
    Updates:                0         0
    Keepalives:             0         0
    Route Refresh:          0         0
    Total messages:         0         0
  Prefix Statistics:
                                   Sent      Rcvd     Best Paths     Best ECMP Paths
    IPv4 Unicast:                     0         0              0                   0
    IPv6 Unicast:                     0         0              0                   0
  Configured maximum total number of routes is 0
  Inbound updates dropped by reason:
    AS path loop detection: 0
    Cluster ID loop detection: 0
    Enforced First AS: 0
    Malformed MPBGP routes: 0
    Originator ID matches local router ID: 0
    Nexthop matches local IP address: 0
    Unexpected IPv6 nexthop for IPv4 routes: 0
    AS_SET/AS_CONFED_SET in AS_PATH for IPv4 Unicast: 0
    AS_SET/AS_CONFED_SET in AS_PATH for IPv6 Unicast: 0
  Inbound updates with attribute errors:
    Resulting in removal of all paths in update (treat as withdraw): 0
    Resulting in AFI/SAFI disable: 0
    Resulting in attribute ignore: 0
    Disabled AFI/SAFIs: None
  Inbound paths dropped by reason:
    IPv4 unicast NLRIs dropped due to martian prefix: 0
    IPv6 unicast NLRIs dropped due to martian prefix: 0
    IPv4 labeled-unicast NLRIs dropped due to excessive labels: 0
    IPv4 labeled-unicast NLRIs dropped due to martian prefix: 0
    IPv6 labeled-unicast NLRIs dropped due to excessive labels: 0
    IPv6 labeled-unicast NLRIs dropped due to martian prefix: 0
    VPN-IPv4 NLRIs dropped due to route import match failure: 0
    VPN-IPv6 NLRIs dropped due to route import match failure: 0
    L2VPN EVPN NLRIs dropped due to route import match failure: 0
    L2VPN EVPN NLRIs dropped due to unsupported route type: 0
    Link-state NLRIs dropped because reception is unsupported: 0
    RT Membership NLRIs dropped due to local origin ASN received from external peer: 0
  Outbound paths dropped by reason:
    IPv4 local address not available: 0
    IPv6 local address not available: 0
Local AS is 64512, local router ID 10.0.0.30
TTL is 255
Local TCP address is 10.0.0.30
Remote TCP address is 10.0.0.124, remote port is 179

BGP neighbor is 10.0.0.131, remote AS 64512, internal link
 Description: Juniper-131
  BGP version 4, remote router ID 0.0.0.0, VRF default
  Inherits configuration from and member of peer-group IBGP_CLIENT_PEER
  Last read never, last write never
  Hold time is 0, keepalive interval is 0 seconds
  Configured hold time is 180, keepalive interval is 60 seconds
  Effective minimum hold time is 3 seconds
  Send failure hold time is 0 seconds
  Hold timer is inactive
  Keepalive timer is inactive
  Connect timer is active, time left: 00:02:00
  Connection interval is 148 seconds
  Failed connection attempts is 22
  Idle-restart timer is inactive
  BGP state is Active
  Number of transitions to established: 0
  Last state was Connect
  Last event was TransportError
  Last sent socket-error:Connect (Network is unreachable), Last time 00:00:47, First time 00:41:18, Repeats 21
  Types of communities advertised: standard extended large
  Neighbor is a route reflector client
  Neighbor is using global cluster ID 10.0.0.30
  Neighbor Capabilities:
  Restart timer is inactive
  End of rib timer is inactive
  IPv4 Unicast AS_SET/AS_CONFED_SET processing: accept
  IPv6 Unicast AS_SET/AS_CONFED_SET processing: accept
  AIGP attribute send and receive for IPv4 Unicast are enabled
  AIGP attribute send and receive for IPv4 with MPLS Labels are enabled
  AIGP attribute send and receive for IPv6 Unicast are enabled
  AIGP attribute send and receive for IPv6 with MPLS Labels are enabled
  BGP session driven failover for IPv4 Unicast is disabled
  BGP session driven failover for IPv6 Unicast is disabled
  Message Statistics:
                         Sent      Rcvd
    Opens:                  0         0
    Notifications:          0         0
    Updates:                0         0
    Keepalives:             0         0
    Route Refresh:          0         0
    Total messages:         0         0
  Prefix Statistics:
                                   Sent      Rcvd     Best Paths     Best ECMP Paths
    IPv4 Unicast:                     0         0              0                   0
    IPv6 Unicast:                     0         0              0                   0
  Configured maximum total number of routes is 0
  Inbound updates dropped by reason:
    AS path loop detection: 0
    Cluster ID loop detection: 0
    Enforced First AS: 0
    Malformed MPBGP routes: 0
    Originator ID matches local router ID: 0
    Nexthop matches local IP address: 0
    Unexpected IPv6 nexthop for IPv4 routes: 0
    AS_SET/AS_CONFED_SET in AS_PATH for IPv4 Unicast: 0
    AS_SET/AS_CONFED_SET in AS_PATH for IPv6 Unicast: 0
  Inbound updates with attribute errors:
    Resulting in removal of all paths in update (treat as withdraw): 0
    Resulting in AFI/SAFI disable: 0
    Resulting in attribute ignore: 0
    Disabled AFI/SAFIs: None
  Inbound paths dropped by reason:
    IPv4 unicast NLRIs dropped due to martian prefix: 0
    IPv6 unicast NLRIs dropped due to martian prefix: 0
    IPv4 labeled-unicast NLRIs dropped due to excessive labels: 0
    IPv4 labeled-unicast NLRIs dropped due to martian prefix: 0
    IPv6 labeled-unicast NLRIs dropped due to excessive labels: 0
    IPv6 labeled-unicast NLRIs dropped due to martian prefix: 0
    VPN-IPv4 NLRIs dropped due to route import match failure: 0
    VPN-IPv6 NLRIs dropped due to route import match failure: 0
    L2VPN EVPN NLRIs dropped due to route import match failure: 0
    L2VPN EVPN NLRIs dropped due to unsupported route type: 0
    Link-state NLRIs dropped because reception is unsupported: 0
    RT Membership NLRIs dropped due to local origin ASN received from external peer: 0
  Outbound paths dropped by reason:
    IPv4 local address not available: 0
    IPv6 local address not available: 0
Local AS is 64512, local router ID 10.0.0.30
TTL is 255
Local TCP address is 10.0.0.30
Remote TCP address is 10.0.0.131, remote port is 179

BGP neighbor is 10.0.0.179, remote AS 64512, internal link
 Description: Juniper-179
  BGP version 4, remote router ID 10.0.0.179, VRF default
  Inherits configuration from and member of peer-group IBGP_CLIENT_PEER
  Last read 00:00:21, last write 00:00:25
  Hold time is 90, keepalive interval is 30 seconds
  Configured hold time is 180, keepalive interval is 60 seconds
  Effective minimum hold time is 3 seconds
  Send failure hold time is 0 seconds
  Hold timer is active, time left: 00:01:09
  Keepalive timer is active, time left: 00:00:00
  Connect timer is inactive
  Idle-restart timer is inactive
  BGP state is Established, up for 00:40:09
  Number of transitions to established: 1
  Last state was OpenConfirm
  Last event was RecvUpdate
  Last sent socket-error:Connect (Network is unreachable), Last time 00:40:55, First time 00:41:18, Repeats 5
  Types of communities advertised: standard extended large
  Neighbor is a route reflector client
  Neighbor is using global cluster ID 10.0.0.30
  Neighbor Capabilities:
    Multiprotocol IPv4 Unicast: received
    Multiprotocol VPN-IPv4: advertised and received and negotiated
    Multiprotocol VPN-IPv6: advertised and received and negotiated
    Four Octet ASN: advertised and received and negotiated
    Route Refresh: advertised and received and negotiated
    Enhanced route refresh: advertised
    Send End-of-RIB messages: advertised and received and negotiated
    Additional-paths recv capability:
      VPN-IPv4: advertised
      VPN-IPv6: advertised
    Additional-paths send capability:
    Graceful Restart advertised:
      Restart-time is 120
      Restart-State bit: yes
      Graceful notification: yes
      VPN-IPv4 is enabled, Forwarding State is not preserved
      VPN-IPv6 is enabled, Forwarding State is not preserved
    Graceful Restart received:
      Restart-time is 120
      Restart-State bit: no
      Graceful notification: yes
    Long Lived Graceful Restart received:
      Helper only
  Restart timer is inactive
  End of rib timer is inactive
    VPN-IPv4 End-of-RIB received: Yes
      Received 00:40:08
      Number of stale paths removed after graceful restart: 0
      Number of paths received before End-of-RIB: 1
    VPN-IPv6 End-of-RIB received: Yes
      Received 00:40:08
      Number of stale paths removed after graceful restart: 0
      Number of paths received before End-of-RIB: 1
  IPv4 Unicast AS_SET/AS_CONFED_SET processing: accept
  IPv6 Unicast AS_SET/AS_CONFED_SET processing: accept
  AIGP attribute send and receive for IPv4 Unicast are enabled
  AIGP attribute send and receive for IPv4 with MPLS Labels are enabled
  AIGP attribute send and receive for IPv6 Unicast are enabled
  AIGP attribute send and receive for IPv6 with MPLS Labels are enabled
  BGP session driven failover for IPv4 Unicast is disabled
  BGP session driven failover for IPv6 Unicast is disabled
  Message Statistics:
                         Sent      Rcvd
    Opens:                  1         1
    Notifications:          0         0
    Updates:               26         6
    Keepalives:            89        89
    Route Refresh:          0         0
    Total messages:       116        96
  Prefix Statistics:
                                   Sent      Rcvd     Best Paths     Best ECMP Paths
    IPv4 Unicast:                     0         0              0                   0
    VPN-IPv4:                         8         1              1                   0
    IPv6 Unicast:                     0         0              0                   0
    VPN-IPv6:                         8         1              1                   0
  Configured maximum total number of routes is 0
  Inbound updates dropped by reason:
    AS path loop detection: 0
    Cluster ID loop detection: 0
    Enforced First AS: 0
    Malformed MPBGP routes: 0
    Originator ID matches local router ID: 0
    Nexthop matches local IP address: 0
    Unexpected IPv6 nexthop for IPv4 routes: 0
    AS_SET/AS_CONFED_SET in AS_PATH for IPv4 Unicast: 0
    AS_SET/AS_CONFED_SET in AS_PATH for IPv6 Unicast: 0
  Inbound updates with attribute errors:
    Resulting in removal of all paths in update (treat as withdraw): 0
    Resulting in AFI/SAFI disable: 0
    Resulting in attribute ignore: 0
    Disabled AFI/SAFIs: None
  Inbound paths dropped by reason:
    IPv4 unicast NLRIs dropped due to martian prefix: 0
    IPv6 unicast NLRIs dropped due to martian prefix: 0
    IPv4 labeled-unicast NLRIs dropped due to excessive labels: 0
    IPv4 labeled-unicast NLRIs dropped due to martian prefix: 0
    IPv6 labeled-unicast NLRIs dropped due to excessive labels: 0
    IPv6 labeled-unicast NLRIs dropped due to martian prefix: 0
    VPN-IPv4 NLRIs dropped due to route import match failure: 0
    VPN-IPv4 NLRIs dropped due to maximum route limit violation: 0
    VPN-IPv6 NLRIs dropped due to route import match failure: 0
    VPN-IPv6 NLRIs dropped due to maximum route limit violation: 0
    L2VPN EVPN NLRIs dropped due to route import match failure: 0
    L2VPN EVPN NLRIs dropped due to unsupported route type: 0
    Link-state NLRIs dropped because reception is unsupported: 0
    RT Membership NLRIs dropped due to local origin ASN received from external peer: 0
  Outbound paths dropped by reason:
    IPv4 local address not available: 0
    IPv6 local address not available: 0
Local AS is 64512, local router ID 10.0.0.30
TTL is 255
Local TCP address is 10.0.0.30, local port is 41969
Remote TCP address is 10.0.0.179, remote port is 179
Local next hop for next hop self:
  VPN-IPv4: 10.0.0.30
  VPN-IPv6: ::ffff:10.0.0.30
TCP Socket Information:
  TCP state is ESTABLISHED
  Recv-Q: 0/32768
  Send-Q: 0/46080
  Outgoing Maximum Segment Size (MSS): 1448
  Total Number of TCP retransmissions: 0
  Options:
    Timestamps enabled: yes
    Selective Acknowledgments enabled: yes
    Window Scale enabled: yes
    Explicit Congestion Notification (ECN) enabled: no
  Socket Statistics:
    Window Scale (wscale): 0,7
    Retransmission Timeout (rto): 212.0ms
    Round-trip Time (rtt/rtvar): 8.7ms/13.6ms
    Delayed Ack Timeout (ato): 40.0ms
    Congestion Window (cwnd): 10
    TCP Throughput: 13.27 Mbps
    Advertised Recv Window (rcv_space): 14480

BGP neighbor is 10.0.0.214, remote AS 64512, internal link
 Description: Nokia-SXR-214
  BGP version 4, remote router ID 10.0.0.214, VRF default
  Inherits configuration from and member of peer-group IBGP_CLIENT_PEER
  Last read 00:00:18, last write 00:00:24
  Hold time is 90, keepalive interval is 30 seconds
  Configured hold time is 180, keepalive interval is 60 seconds
  Effective minimum hold time is 3 seconds
  Send failure hold time is 0 seconds
  Hold timer is active, time left: 00:01:12
  Keepalive timer is inactive
  Connect timer is inactive
  Idle-restart timer is inactive
  BGP state is Established, up for 00:41:18
  Number of transitions to established: 1
  Last state was OpenConfirm
  Last event was RecvUpdate
  Types of communities advertised: standard extended large
  Neighbor is a route reflector client
  Neighbor is using global cluster ID 10.0.0.30
  Neighbor Capabilities:
    Multiprotocol VPN-IPv4: advertised and received and negotiated
    Multiprotocol VPN-IPv6: advertised and received and negotiated
    Four Octet ASN: advertised and received and negotiated
    Route Refresh: advertised and received and negotiated
    Enhanced route refresh: advertised
    Send End-of-RIB messages: advertised and received and negotiated
    Additional-paths recv capability:
      VPN-IPv4: advertised
      VPN-IPv6: advertised
    Additional-paths send capability:
    Graceful Restart advertised:
      Restart-time is 120
      Restart-State bit: yes
      Graceful notification: yes
      VPN-IPv4 is enabled, Forwarding State is not preserved
      VPN-IPv6 is enabled, Forwarding State is not preserved
    Graceful Restart received:
      Restart-time is 300
      Restart-State bit: no
      Graceful notification: no
  Restart timer is inactive
  End of rib timer is inactive
    VPN-IPv4 End-of-RIB received: Yes
      Received 00:41:18
      Number of stale paths removed after graceful restart: 0
      Number of paths received before End-of-RIB: 1
    VPN-IPv6 End-of-RIB received: Yes
      Received 00:41:18
      Number of stale paths removed after graceful restart: 0
      Number of paths received before End-of-RIB: 1
  IPv4 Unicast AS_SET/AS_CONFED_SET processing: accept
  IPv6 Unicast AS_SET/AS_CONFED_SET processing: accept
  AIGP attribute send and receive for IPv4 Unicast are enabled
  AIGP attribute send and receive for IPv4 with MPLS Labels are enabled
  AIGP attribute send and receive for IPv6 Unicast are enabled
  AIGP attribute send and receive for IPv6 with MPLS Labels are enabled
  BGP session driven failover for IPv4 Unicast is disabled
  BGP session driven failover for IPv6 Unicast is disabled
  Message Statistics:
                         Sent      Rcvd
    Opens:                  1         1
    Notifications:          0         0
    Updates:               28         4
    Keepalives:            92        84
    Route Refresh:          0         0
    Total messages:       121        89
  Prefix Statistics:
                                   Sent      Rcvd     Best Paths     Best ECMP Paths
    IPv4 Unicast:                     0         0              0                   0
    VPN-IPv4:                         8         1              1                   0
    IPv6 Unicast:                     0         0              0                   0
    VPN-IPv6:                         8         1              1                   0
  Configured maximum total number of routes is 0
  Inbound updates dropped by reason:
    AS path loop detection: 0
    Cluster ID loop detection: 0
    Enforced First AS: 0
    Malformed MPBGP routes: 0
    Originator ID matches local router ID: 0
    Nexthop matches local IP address: 0
    Unexpected IPv6 nexthop for IPv4 routes: 0
    AS_SET/AS_CONFED_SET in AS_PATH for IPv4 Unicast: 0
    AS_SET/AS_CONFED_SET in AS_PATH for IPv6 Unicast: 0
  Inbound updates with attribute errors:
    Resulting in removal of all paths in update (treat as withdraw): 0
    Resulting in AFI/SAFI disable: 0
    Resulting in attribute ignore: 0
    Disabled AFI/SAFIs: None
  Inbound paths dropped by reason:
    IPv4 unicast NLRIs dropped due to martian prefix: 0
    IPv6 unicast NLRIs dropped due to martian prefix: 0
    IPv4 labeled-unicast NLRIs dropped due to excessive labels: 0
    IPv4 labeled-unicast NLRIs dropped due to martian prefix: 0
    IPv6 labeled-unicast NLRIs dropped due to excessive labels: 0
    IPv6 labeled-unicast NLRIs dropped due to martian prefix: 0
    VPN-IPv4 NLRIs dropped due to route import match failure: 0
    VPN-IPv4 NLRIs dropped due to maximum route limit violation: 0
    VPN-IPv6 NLRIs dropped due to route import match failure: 0
    VPN-IPv6 NLRIs dropped due to maximum route limit violation: 0
    L2VPN EVPN NLRIs dropped due to route import match failure: 0
    L2VPN EVPN NLRIs dropped due to unsupported route type: 0
    Link-state NLRIs dropped because reception is unsupported: 0
    RT Membership NLRIs dropped due to local origin ASN received from external peer: 0
  Outbound paths dropped by reason:
    IPv4 local address not available: 0
    IPv6 local address not available: 0
Local AS is 64512, local router ID 10.0.0.30
TTL is 255
Local TCP address is 10.0.0.30, local port is 45009
Remote TCP address is 10.0.0.214, remote port is 179
Local next hop for next hop self:
  VPN-IPv4: 10.0.0.30
  VPN-IPv6: ::ffff:10.0.0.30
TCP Socket Information:
  TCP state is ESTABLISHED
  Recv-Q: 0/32768
  Send-Q: 0/332800
  Outgoing Maximum Segment Size (MSS): 1448
  Total Number of TCP retransmissions: 0
  Options:
    Timestamps enabled: yes
    Selective Acknowledgments enabled: yes
    Window Scale enabled: yes
    Explicit Congestion Notification (ECN) enabled: no
  Socket Statistics:
    Window Scale (wscale): 0,7
    Retransmission Timeout (rto): 204.0ms
    Round-trip Time (rtt/rtvar): 0.4ms/0.0ms
    Delayed Ack Timeout (ato): 40.0ms
    Congestion Window (cwnd): 10
    TCP Throughput: 284.62 Mbps
    Advertised Recv Window (rcv_space): 14480

BGP neighbor is 10.0.0.217, remote AS 64512, internal link
 Description: Nokia
  BGP version 4, remote router ID 10.0.0.217, VRF default
  Inherits configuration from and member of peer-group IBGP_CLIENT_PEER
  Last read 00:00:17, last write 00:00:02
  Hold time is 90, keepalive interval is 30 seconds
  Configured hold time is 180, keepalive interval is 60 seconds
  Effective minimum hold time is 3 seconds
  Send failure hold time is 0 seconds
  Hold timer is active, time left: 00:01:13
  Keepalive timer is active, time left: 00:00:18
  Connect timer is inactive
  Idle-restart timer is inactive
  BGP state is Established, up for 00:41:17
  Number of transitions to established: 1
  Last state was OpenConfirm
  Last event was RecvUpdate
  Types of communities advertised: standard extended large
  Neighbor is a route reflector client
  Neighbor is using global cluster ID 10.0.0.30
  Neighbor Capabilities:
    Multiprotocol VPN-IPv4: advertised and received and negotiated
    Multiprotocol VPN-IPv6: advertised and received and negotiated
    Four Octet ASN: advertised and received and negotiated
    Route Refresh: advertised and received and negotiated
    Enhanced route refresh: advertised
    Send End-of-RIB messages: advertised and received and negotiated
    Additional-paths recv capability:
      VPN-IPv4: advertised
      VPN-IPv6: advertised
    Additional-paths send capability:
    Graceful Restart advertised:
      Restart-time is 120
      Restart-State bit: yes
      Graceful notification: yes
      VPN-IPv4 is enabled, Forwarding State is not preserved
      VPN-IPv6 is enabled, Forwarding State is not preserved
    Graceful Restart received:
      Restart-time is 120
      Restart-State bit: no
      Graceful notification: no
  Restart timer is inactive
  End of rib timer is inactive
    VPN-IPv4 End-of-RIB received: Yes
      Received 00:41:16
      Number of stale paths removed after graceful restart: 0
      Number of paths received before End-of-RIB: 1
    VPN-IPv6 End-of-RIB received: Yes
      Received 00:41:16
      Number of stale paths removed after graceful restart: 0
      Number of paths received before End-of-RIB: 1
  IPv4 Unicast AS_SET/AS_CONFED_SET processing: accept
  IPv6 Unicast AS_SET/AS_CONFED_SET processing: accept
  AIGP attribute send and receive for IPv4 Unicast are enabled
  AIGP attribute send and receive for IPv4 with MPLS Labels are enabled
  AIGP attribute send and receive for IPv6 Unicast are enabled
  AIGP attribute send and receive for IPv6 with MPLS Labels are enabled
  BGP session driven failover for IPv4 Unicast is disabled
  BGP session driven failover for IPv6 Unicast is disabled
  Message Statistics:
                         Sent      Rcvd
    Opens:                  1         1
    Notifications:          0         0
    Updates:               28         4
    Keepalives:            92        84
    Route Refresh:          0         0
    Total messages:       121        89
  Prefix Statistics:
                                   Sent      Rcvd     Best Paths     Best ECMP Paths
    IPv4 Unicast:                     0         0              0                   0
    VPN-IPv4:                         8         1              1                   0
    IPv6 Unicast:                     0         0              0                   0
    VPN-IPv6:                         8         1              1                   0
  Configured maximum total number of routes is 0
  Inbound updates dropped by reason:
    AS path loop detection: 0
    Cluster ID loop detection: 0
    Enforced First AS: 0
    Malformed MPBGP routes: 0
    Originator ID matches local router ID: 0
    Nexthop matches local IP address: 0
    Unexpected IPv6 nexthop for IPv4 routes: 0
    AS_SET/AS_CONFED_SET in AS_PATH for IPv4 Unicast: 0
    AS_SET/AS_CONFED_SET in AS_PATH for IPv6 Unicast: 0
  Inbound updates with attribute errors:
    Resulting in removal of all paths in update (treat as withdraw): 0
    Resulting in AFI/SAFI disable: 0
    Resulting in attribute ignore: 0
    Disabled AFI/SAFIs: None
  Inbound paths dropped by reason:
    IPv4 unicast NLRIs dropped due to martian prefix: 0
    IPv6 unicast NLRIs dropped due to martian prefix: 0
    IPv4 labeled-unicast NLRIs dropped due to excessive labels: 0
    IPv4 labeled-unicast NLRIs dropped due to martian prefix: 0
    IPv6 labeled-unicast NLRIs dropped due to excessive labels: 0
    IPv6 labeled-unicast NLRIs dropped due to martian prefix: 0
    VPN-IPv4 NLRIs dropped due to route import match failure: 0
    VPN-IPv4 NLRIs dropped due to maximum route limit violation: 0
    VPN-IPv6 NLRIs dropped due to route import match failure: 0
    VPN-IPv6 NLRIs dropped due to maximum route limit violation: 0
    L2VPN EVPN NLRIs dropped due to route import match failure: 0
    L2VPN EVPN NLRIs dropped due to unsupported route type: 0
    Link-state NLRIs dropped because reception is unsupported: 0
    RT Membership NLRIs dropped due to local origin ASN received from external peer: 0
  Outbound paths dropped by reason:
    IPv4 local address not available: 0
    IPv6 local address not available: 0
Local AS is 64512, local router ID 10.0.0.30
TTL is 255
Local TCP address is 10.0.0.30, local port is 43751
Remote TCP address is 10.0.0.217, remote port is 179
Local next hop for next hop self:
  VPN-IPv4: 10.0.0.30
  VPN-IPv6: ::ffff:10.0.0.30
TCP Socket Information:
  TCP state is ESTABLISHED
  Recv-Q: 0/32768
  Send-Q: 0/46080
  Outgoing Maximum Segment Size (MSS): 1012
  Total Number of TCP retransmissions: 0
  Options:
    Timestamps enabled: yes
    Selective Acknowledgments enabled: no
    Window Scale enabled: yes
    Explicit Congestion Notification (ECN) enabled: no
  Socket Statistics:
    Window Scale (wscale): 0,7
    Retransmission Timeout (rto): 204.0ms
    Round-trip Time (rtt/rtvar): 0.5ms/0.1ms
    Delayed Ack Timeout (ato): 40.0ms
    Congestion Window (cwnd): 10
    TCP Throughput: 152.75 Mbps
    Advertised Recv Window (rcv_space): 14480

BGP neighbor is 10.0.0.221, remote AS 64512, internal link
 Description: Ribbon-221
  BGP version 4, remote router ID 10.0.0.221, VRF default
  Inherits configuration from and member of peer-group IBGP_CLIENT_PEER
  Last read 00:00:14, last write 00:00:09
  Hold time is 180, keepalive interval is 60 seconds
  Configured hold time is 180, keepalive interval is 60 seconds
  Effective minimum hold time is 3 seconds
  Send failure hold time is 0 seconds
  Hold timer is active, time left: 00:02:46
  Keepalive timer is active, time left: 00:00:42
  Connect timer is inactive
  Idle-restart timer is inactive
  BGP state is Established, up for 00:33:41
  Number of transitions to established: 1
  Last state was OpenConfirm
  Last event was RecvKeepAlive
  Last sent socket-error:Connect (Network is unreachable), Last time 00:34:20, First time 00:41:18, Repeats 9
  Types of communities advertised: standard extended large
  Enhanced route refresh stale path removal disabled
  Outbound enhanced route refresh enabled
  Neighbor is a route reflector client
  Neighbor is using global cluster ID 10.0.0.30
  Neighbor Capabilities:
    Multiprotocol IPv4 Unicast: received
    Multiprotocol VPN-IPv4: advertised and received and negotiated
    Multiprotocol VPN-IPv6: advertised and received and negotiated
    Four Octet ASN: advertised and received and negotiated
    Route Refresh: advertised and received and negotiated
    Enhanced route refresh: advertised and received and negotiated
    Send End-of-RIB messages: advertised
    Additional-paths recv capability:
      VPN-IPv4: advertised
      VPN-IPv6: advertised
    Additional-paths send capability:
    Graceful Restart advertised:
      Restart-time is 120
      Restart-State bit: no
      Graceful notification: yes
      VPN-IPv4 is enabled, Forwarding State is not preserved
      VPN-IPv6 is enabled, Forwarding State is not preserved
  Restart timer is inactive
  End of rib timer is inactive
    VPN-IPv4 End-of-RIB received: No
      Number of stale paths removed after graceful restart: 0
    VPN-IPv6 End-of-RIB received: No
      Number of stale paths removed after graceful restart: 0
  IPv4 Unicast AS_SET/AS_CONFED_SET processing: accept
  IPv6 Unicast AS_SET/AS_CONFED_SET processing: accept
  AIGP attribute send and receive for IPv4 Unicast are enabled
  AIGP attribute send and receive for IPv4 with MPLS Labels are enabled
  AIGP attribute send and receive for IPv6 Unicast are enabled
  AIGP attribute send and receive for IPv6 with MPLS Labels are enabled
  BGP session driven failover for IPv4 Unicast is disabled
  BGP session driven failover for IPv6 Unicast is disabled
  Message Statistics:
                                  Sent      Rcvd
    Opens:                           1         1
    Notifications:                   0         0
    Updates:                        26         2
    Keepalives:                     38        93
    Enhanced Route Refresh:          0         0
    Begin of Route Refresh:          0         0
    End of Route Refresh:            0         0
    Total messages:                 65        96
  Prefix Statistics:
                                   Sent      Rcvd     Best Paths     Best ECMP Paths
    IPv4 Unicast:                     0         0              0                   0
    VPN-IPv4:                         8         1              1                   0
    IPv6 Unicast:                     0         0              0                   0
    VPN-IPv6:                         8         1              1                   0
  Configured maximum total number of routes is 0
  Inbound updates dropped by reason:
    AS path loop detection: 0
    Cluster ID loop detection: 0
    Enforced First AS: 0
    Malformed MPBGP routes: 0
    Originator ID matches local router ID: 0
    Nexthop matches local IP address: 0
    Unexpected IPv6 nexthop for IPv4 routes: 0
    AS_SET/AS_CONFED_SET in AS_PATH for IPv4 Unicast: 0
    AS_SET/AS_CONFED_SET in AS_PATH for IPv6 Unicast: 0
  Inbound updates with attribute errors:
    Resulting in removal of all paths in update (treat as withdraw): 0
    Resulting in AFI/SAFI disable: 0
    Resulting in attribute ignore: 0
    Disabled AFI/SAFIs: None
  Inbound paths dropped by reason:
    IPv4 unicast NLRIs dropped due to martian prefix: 0
    IPv6 unicast NLRIs dropped due to martian prefix: 0
    IPv4 labeled-unicast NLRIs dropped due to excessive labels: 0
    IPv4 labeled-unicast NLRIs dropped due to martian prefix: 0
    IPv6 labeled-unicast NLRIs dropped due to excessive labels: 0
    IPv6 labeled-unicast NLRIs dropped due to martian prefix: 0
    VPN-IPv4 NLRIs dropped due to route import match failure: 0
    VPN-IPv4 NLRIs dropped due to maximum route limit violation: 0
    VPN-IPv6 NLRIs dropped due to route import match failure: 0
    VPN-IPv6 NLRIs dropped due to maximum route limit violation: 0
    L2VPN EVPN NLRIs dropped due to route import match failure: 0
    L2VPN EVPN NLRIs dropped due to unsupported route type: 0
    Link-state NLRIs dropped because reception is unsupported: 0
    RT Membership NLRIs dropped due to local origin ASN received from external peer: 0
  Outbound paths dropped by reason:
    IPv4 local address not available: 0
    IPv6 local address not available: 0
Local AS is 64512, local router ID 10.0.0.30
TTL is 255
Local TCP address is 10.0.0.30, local port is 34929
Remote TCP address is 10.0.0.221, remote port is 179
Local next hop for next hop self:
  VPN-IPv4: 10.0.0.30
  VPN-IPv6: ::ffff:10.0.0.30
TCP Socket Information:
  TCP state is ESTABLISHED
  Recv-Q: 0/32768
  Send-Q: 0/46080
  Outgoing Maximum Segment Size (MSS): 1448
  Total Number of TCP retransmissions: 1
  Options:
    Timestamps enabled: yes
    Selective Acknowledgments enabled: yes
    Window Scale enabled: yes
    Explicit Congestion Notification (ECN) enabled: no
  Socket Statistics:
    Window Scale (wscale): 9,7
    Retransmission Timeout (rto): 204.0ms
    Round-trip Time (rtt/rtvar): 0.2ms/0.0ms
    Delayed Ack Timeout (ato): 40.0ms
    Congestion Window (cwnd): 10
    TCP Throughput: 541.31 Mbps
    Advertised Recv Window (rcv_space): 14480

```

## show tunnel rib system-tunnel-rib brief

```text
Tunnel RIB: system-tunnel-rib
Endpoint        Tunnel Type     Index(es)   Tunnel Preference   IGP Preference 
-------------- --------------- ----------- ------------------- ----------------
10.0.0.32/32    IS-IS SR IPv4   9           65                  115            
10.0.0.53/32    IS-IS SR IPv4   5           65                  115            
10.0.0.72/32    IS-IS SR IPv4   2           65                  115            
10.0.0.84/32    IS-IS SR IPv4   1           65                  115            
10.0.0.120/32   IS-IS SR IPv4   7           65                  115            
10.0.0.128/32   IS-IS SR IPv4   11          65                  115            
10.0.0.175/32   IS-IS SR IPv4   4           65                  115            
10.0.0.179/32   IS-IS SR IPv4   6           65                  115            
10.0.0.214/32   IS-IS SR IPv4   10          65                  115            
10.0.0.217/32   IS-IS SR IPv4   16          65                  115            
10.0.0.221/32   IS-IS SR IPv4   13          65                  115            

   IGP Metric    Metric Type
---------------- -----------
   10            metric     
   10            metric     
   20            metric     
   20            metric     
   10            metric     
   10            metric     
   20            metric     
   10            metric     
   10            metric     
   10            metric     
   10            metric     

```

## show tunnel rib colored brief

```text
Tunnel RIB: system-colored-tunnel-rib
 Endpoint     Color     Tunnel Type     Index(es)     Tunnel Preference     IGP Preference     IGP Metric   Metric Type
----------- --------- --------------- ------------- --------------------- ------------------ -------------- -----------

```

## show rib route ip

```text
VRF: default, Protocol: connected
Codes: C - Connected, S - Static, P - Route Input, G - Gribi
       B - BGP, O - Ospf, O3 - Ospf3, I - Isis, R - Rip, VL - VRF Leak
       > - Best Route, * - Unresolved Next hop
       EM - Exact match of the SR-TE Policy
       NM - Null endpoint match of the SR-TE Policy
       AM - Any endpoint match of the SR-TE Policy
       L - Part of a recursive route resolution loop
       A - Next hop not resolved in ARP/ND
       NF - Not in FEC
>C    10.0.0.30/32 [0 pref/0 metric] updated 22:20:39 ago
         via Loopback0, directly connected
>C    20.30.32.0/24 [0 pref/0 metric] updated 00:57:44 ago
         via Ethernet2, directly connected
>C    20.30.53.0/24 [0 pref/0 metric] updated 00:57:46 ago
         via Ethernet13, directly connected
>C    20.30.66.0/24 [0 pref/0 metric] updated 00:57:46 ago
         via Ethernet31, directly connected
>C    20.30.72.0/24 [0 pref/0 metric] updated 00:57:46 ago
         via Ethernet9, directly connected
>C    20.30.84.0/24 [0 pref/0 metric] updated 00:57:46 ago
         via Ethernet12, directly connected
>C    20.30.120.0/24 [0 pref/0 metric] updated 00:57:46 ago
         via Ethernet3, directly connected
>C    20.30.124.0/24 [0 pref/0 metric] updated 00:57:46 ago
         via Ethernet17, directly connected
>C    20.30.128.0/24 [0 pref/0 metric] updated 00:57:46 ago
         via Ethernet19, directly connected
>C    20.30.179.0/24 [0 pref/0 metric] updated 00:57:46 ago
         via Ethernet40, directly connected
>C    20.30.184.0/24 [0 pref/0 metric] updated 00:57:46 ago
         via Ethernet7, directly connected
>C    20.30.214.0/24 [0 pref/0 metric] updated 00:41:56 ago
         via Ethernet5, directly connected
>C    20.30.217.0/24 [0 pref/0 metric] updated 00:57:45 ago
         via Ethernet4, directly connected
>C    20.30.221.0/24 [0 pref/0 metric] updated 00:57:46 ago
         via Ethernet15, directly connected
VRF: default, Protocol: route-input
Codes: C - Connected, S - Static, P - Route Input, G - Gribi
       B - BGP, O - Ospf, O3 - Ospf3, I - Isis, R - Rip, VL - VRF Leak
       > - Best Route, * - Unresolved Next hop
       EM - Exact match of the SR-TE Policy
       NM - Null endpoint match of the SR-TE Policy
       AM - Any endpoint match of the SR-TE Policy
       L - Part of a recursive route resolution loop
       A - Next hop not resolved in ARP/ND
       NF - Not in FEC
>P    0.0.0.0/8 [1 pref/0 metric] updated 1d03h ago
         via Null0, directly connected [NF]
>P    127.0.0.0/8 [1 pref/0 metric] updated 1d03h ago
         via :: [1 pref/1 metric] type ipv4
            via , directly connected
VRF: default, Protocol: isis
Codes: C - Connected, S - Static, P - Route Input, G - Gribi
       B - BGP, O - Ospf, O3 - Ospf3, I - Isis, R - Rip, VL - VRF Leak
       > - Best Route, * - Unresolved Next hop
       EM - Exact match of the SR-TE Policy
       NM - Null endpoint match of the SR-TE Policy
       AM - Any endpoint match of the SR-TE Policy
       L - Part of a recursive route resolution loop
       A - Next hop not resolved in ARP/ND
       NF - Not in FEC
>I    10.0.0.32/32 [115 pref/10 metric] updated 00:30:31 ago
         via 20.30.32.32, Ethernet2
>I    10.0.0.53/32 [115 pref/10 metric] updated 00:57:43 ago
         via 20.30.53.53, Ethernet13
>I    10.0.0.72/32 [115 pref/20 metric] updated 00:31:49 ago
         via 20.30.72.72, Ethernet9
>I    10.0.0.84/32 [115 pref/20 metric] updated 00:57:43 ago
         via 20.30.84.84, Ethernet12
>I    10.0.0.120/32 [115 pref/10 metric] updated 00:57:37 ago
         via 20.30.120.120, Ethernet3
>I    10.0.0.128/32 [115 pref/10 metric] updated 00:09:37 ago
         via 20.30.128.128, Ethernet19
>I    10.0.0.175/32 [115 pref/20 metric] updated 00:03:41 ago
         via 20.30.32.32, Ethernet2
         via 20.30.53.53, Ethernet13
         via 20.30.72.72, Ethernet9
         via 20.30.84.84, Ethernet12
         via 20.30.124.124, Ethernet17
         via 20.30.128.128, Ethernet19
         via 20.30.179.179, Ethernet40
         via 20.30.214.214, Ethernet5
>I    10.0.0.179/32 [115 pref/10 metric] updated 00:40:34 ago
         via 20.30.179.179, Ethernet40
>I    10.0.0.214/32 [115 pref/10 metric] updated 00:41:55 ago
         via 20.30.214.214, Ethernet5
>I    10.0.0.216/32 [115 pref/20 metric] updated 00:41:55 ago
         via 20.30.214.214, Ethernet5
>I    10.0.0.217/32 [115 pref/10 metric] updated 00:57:43 ago
         via 20.30.217.217, Ethernet4
>I    10.0.0.221/32 [115 pref/10 metric] updated 00:33:41 ago
         via 20.30.221.221, Ethernet15
>I    20.32.175.0/24 [115 pref/20 metric] updated 00:03:42 ago
         via 20.30.32.32, Ethernet2
>I    20.53.175.0/24 [115 pref/20 metric] updated 00:57:43 ago
         via 20.30.53.53, Ethernet13
>I    20.66.175.0/24 [115 pref/30 metric] updated 00:03:41 ago
         via 20.30.32.32, Ethernet2
         via 20.30.53.53, Ethernet13
         via 20.30.72.72, Ethernet9
         via 20.30.84.84, Ethernet12
         via 20.30.124.124, Ethernet17
         via 20.30.128.128, Ethernet19
         via 20.30.179.179, Ethernet40
         via 20.30.214.214, Ethernet5
>I    20.72.175.0/24 [115 pref/20 metric] updated 00:31:49 ago
         via 20.30.72.72, Ethernet9
>I    20.84.175.0/24 [115 pref/30 metric] updated 00:03:41 ago
         via 20.30.32.32, Ethernet2
         via 20.30.53.53, Ethernet13
         via 20.30.72.72, Ethernet9
         via 20.30.84.84, Ethernet12
         via 20.30.124.124, Ethernet17
         via 20.30.128.128, Ethernet19
         via 20.30.179.179, Ethernet40
         via 20.30.214.214, Ethernet5
>I    20.120.175.0/24 [115 pref/30 metric] updated 00:03:41 ago
         via 20.30.32.32, Ethernet2
         via 20.30.53.53, Ethernet13
         via 20.30.72.72, Ethernet9
         via 20.30.84.84, Ethernet12
         via 20.30.124.124, Ethernet17
         via 20.30.128.128, Ethernet19
         via 20.30.179.179, Ethernet40
         via 20.30.214.214, Ethernet5
>I    20.120.214.0/24 [115 pref/20 metric] updated 00:57:37 ago
         via 20.30.120.120, Ethernet3
>I    20.124.175.0/24 [115 pref/20 metric] updated 00:08:10 ago
         via 20.30.124.124, Ethernet17
>I    20.128.175.0/24 [115 pref/20 metric] updated 00:09:37 ago
         via 20.30.128.128, Ethernet19
>I    20.131.175.0/24 [115 pref/30 metric] updated 00:03:41 ago
         via 20.30.32.32, Ethernet2
         via 20.30.53.53, Ethernet13
         via 20.30.72.72, Ethernet9
         via 20.30.84.84, Ethernet12
         via 20.30.124.124, Ethernet17
         via 20.30.128.128, Ethernet19
         via 20.30.179.179, Ethernet40
         via 20.30.214.214, Ethernet5
>I    20.175.179.0/24 [115 pref/20 metric] updated 00:40:34 ago
         via 20.30.179.179, Ethernet40
>I    20.175.184.0/24 [115 pref/30 metric] updated 00:03:41 ago
         via 20.30.32.32, Ethernet2
         via 20.30.53.53, Ethernet13
         via 20.30.72.72, Ethernet9
         via 20.30.84.84, Ethernet12
         via 20.30.124.124, Ethernet17
         via 20.30.128.128, Ethernet19
         via 20.30.179.179, Ethernet40
         via 20.30.214.214, Ethernet5
>I    20.175.214.0/24 [115 pref/20 metric] updated 00:41:55 ago
         via 20.30.214.214, Ethernet5
>I    20.175.217.0/24 [115 pref/20 metric] updated 00:57:43 ago
         via 20.30.217.217, Ethernet4
>I    20.175.221.0/24 [115 pref/20 metric] updated 00:33:41 ago
         via 20.30.221.221, Ethernet15
>I    20.214.216.0/24 [115 pref/20 metric] updated 00:41:55 ago
         via 20.30.214.214, Ethernet5
```

## show rib route ipv6

```text
VRF: default, Protocol: connected
Codes: C - Connected, S - Static, P - Route Input, G - Gribi
       B - BGP, O - Ospf, O3 - Ospf3, I - Isis, R - Rip, VL - VRF Leak
       > - Best Route, * - Unresolved Next hop
       EM - Exact match of the SR-TE Policy
       NM - Null endpoint match of the SR-TE Policy
       AM - Any endpoint match of the SR-TE Policy
       L - Part of a recursive route resolution loop
       A - Next hop not resolved in ARP/ND
       NF - Not in FEC
>C    2001:0:30:32::/64 [0 pref/0 metric] updated 00:57:44 ago
         via Ethernet2, directly connected
>C    2001:0:30:66::/64 [0 pref/0 metric] updated 00:57:46 ago
         via Ethernet31, directly connected
>C    2001:0:30:72::/64 [0 pref/0 metric] updated 00:57:46 ago
         via Ethernet9, directly connected
>C    2001:0:30:84::/64 [0 pref/0 metric] updated 00:57:46 ago
         via Ethernet12, directly connected
>C    2001:0:30:120::/64 [0 pref/0 metric] updated 00:57:46 ago
         via Ethernet3, directly connected
>C    2001:0:30:124::/64 [0 pref/0 metric] updated 00:57:46 ago
         via Ethernet17, directly connected
>C    2001:0:30:128::/64 [0 pref/0 metric] updated 00:57:46 ago
         via Ethernet19, directly connected
>C    2001:0:30:179::/64 [0 pref/0 metric] updated 00:57:46 ago
         via Ethernet40, directly connected
>C    2001:0:30:184::/64 [0 pref/0 metric] updated 00:57:46 ago
         via Ethernet7, directly connected
>C    2001:0:30:214::/64 [0 pref/0 metric] updated 00:41:56 ago
         via Ethernet5, directly connected
>C    2001:0:30:217::/64 [0 pref/0 metric] updated 00:57:45 ago
         via Ethernet4, directly connected
>C    2001:0:30:221::/64 [0 pref/0 metric] updated 00:57:46 ago
         via Ethernet15, directly connected
>C    2001:0:53:120::/64 [0 pref/0 metric] updated 00:57:46 ago
         via Ethernet13, directly connected
VRF: default, Protocol: route-input
Codes: C - Connected, S - Static, P - Route Input, G - Gribi
       B - BGP, O - Ospf, O3 - Ospf3, I - Isis, R - Rip, VL - VRF Leak
       > - Best Route, * - Unresolved Next hop
       EM - Exact match of the SR-TE Policy
       NM - Null endpoint match of the SR-TE Policy
       AM - Any endpoint match of the SR-TE Policy
       L - Part of a recursive route resolution loop
       A - Next hop not resolved in ARP/ND
       NF - Not in FEC
>P    ::/96 [1 pref/0 metric] updated 00:57:46 ago
         via Null0, directly connected [NF]
>P    ::ffff:127.0.0.0/104 [1 pref/0 metric] updated 00:57:46 ago
         via :: [1 pref/1 metric] type ipv6
            via , directly connected
>P    fe80::/10 [1 pref/0 metric] updated 00:57:46 ago
VRF: default, Protocol: isis
Codes: C - Connected, S - Static, P - Route Input, G - Gribi
       B - BGP, O - Ospf, O3 - Ospf3, I - Isis, R - Rip, VL - VRF Leak
       > - Best Route, * - Unresolved Next hop
       EM - Exact match of the SR-TE Policy
       NM - Null endpoint match of the SR-TE Policy
       AM - Any endpoint match of the SR-TE Policy
       L - Part of a recursive route resolution loop
       A - Next hop not resolved in ARP/ND
       NF - Not in FEC
>I    2001:0:32:175::/64 [115 pref/20 metric] updated 00:03:22 ago
         via fe80::d6af:f7ff:fe2f:1396, Ethernet2
>I    2001:0:120:214::/64 [115 pref/20 metric] updated 00:57:37 ago
         via fe80::be31:e2ff:fee1:ec2c, Ethernet3
```

## show platform sand l3 summary

```text
Number of vrfs: 3

Ipv4:
  Routes:       116  backlog:  0  unprogrammed:  0
  Adjacencies:  149  backlog:  0  unprogrammed:  0
Ipv6:
  Routes:       33   backlog:  0  unprogrammed:  0
  Adjacencies:  149  backlog:  0  unprogrammed:  0
Mpls:
  Routes:       24  backlog:  0  unprogrammed:  0
  Adjacencies:  14  backlog:  0  unprogrammed:  0

Jericho2 Ip Fecs:
  Non-ecmp fecs:  4148  ecmp fecs:  1  fec entries:  4156
Jericho2 Mpls Fecs:
  Non-ecmp fecs:  13  ecmp fecs:  1  fec entries:  21
Jericho2 Vxlan Tunnel Fecs:
  Non-ecmp fecs:  0  ecmp fecs:  0  fec entries:  0
  Number of vxlan tunnels configured: 0

Jericho2 Lpm Routes:
  Routes:   116  unprogrammed:   0   
  Routes6:  33   unprogrammed6:  0   
  Backlog:  0  

Jericho2 Lpm:
  TCAM entries used:   3   Percent free:  99  ADS2 entries used:   9  Percent free:  99
  Pivot buckets used:  4   Rows used:     1   Entries Per Bucket:  2  Percent free:  99
  Route buckets used:  25  Rows used:     3   Entries Per Bucket:  5  Percent free:  99

Lem:
  IPv4  Host in Lem:            disabled
  IPv4  Prefix-lengths in Lem:  None    
  IPv6  Host in Lem:            disabled
  IPv6  Prefix-lengths in Lem:  None    
  Number of downloads:        0
  Number of overflow events:  0

Egress Arp rewrite entries in use (in each fap):
  FixedSystem: 12
Egress Arp remote rewrite entries in use (in each fap):
  FixedSystem: 0
Egress Ip tunnel rewrite entries in use (in each fap):
  FixedSystem: 0
Egress Mpls (for outer 2 labels) rewrite entries in use (in each fap):
  FixedSystem: 0
Egress Mpls (for inner 2 labels) rewrite entries in use (in each fap):
  FixedSystem: 9
Egress Sflow rewrite entries in use (in each fap):
  FixedSystem: 0

Egress rewrite chains in backlog: resource-full 0, no-interface 0

Glem entries used per fap :
  FixedSystem: 4125

Jericho2 Fec:
  Maximum FEC hierarchy levels:  2
  ReusedEcmp:  153  allocs:  984  frees:  920  shuffles:  0  cmds:  0
  Zombies:     0    purges:    0
  Quarantine:  0/0  shuffles:  0  deletes:  0   
  Preserved FECs: 0
    First FEC preserved: never
    Last FEC preserved: never
  Fec insertion failures:  0
  Level1  Fecs:
    Non-ecmp fecs:            9   ecmp fecs:            1 
    Non-ecmp (Percent free):  99  ecmp (Percent free):  99
  Level2  Fecs:
    Non-ecmp fecs:            69  ecmp fecs:            2 
    Non-ecmp (Percent free):  99  ecmp (Percent free):  99
  Level3  Fecs:
    Non-ecmp fecs:            0    ecmp fecs:            0  
    Non-ecmp (Percent free):  100  ecmp (Percent free):  100

Lpm Detail:
  Requests:  2835  cleanses:  616  batches:  616  avg batch size:  4

Jericho Arp:
  ArpTable writes:      32852  queued      0   
  IngressTable writes:  68665  queued      0   
  Coprocessors:         1      in CmdRing

Tunnel Counter Status
  Number of MPLS tunnels:                  17   
  Number of uncountable MPLS tunnels:      17   
  Number of MPLSoGRE tunnels:              0    
  Number of uncountable MPLSoGRE tunnels:  0    
  Number of IP tunnels:                    0    
  Number of uncountable IP tunnels:        0    
  Shuffle tunnel enabled:                  False
```

## show platform jericho2 ip route

```text
Tunnel Type: M(mpls), G(gre), MoG(mpls-over-gre), MoU(mpls-over-udp), I(ip-in-ip), IPoU(ip-over-udp)
             vxlan-o(vxlan outer-rewrite info), vxlan-i(vxlan inner-rewrite info)
CW  - Control word
FL  - Flow label
EL  - Entropy label
ELI - Entropy label indicator
*   - Routes in LEM
D   - ECMP is divergent across switching chips
 ----------------------------------------------------------------------------------------------------------
|                                 Routing Table                                            |              |
|----------------------------------------------------------------------------------------------------------
|VRF|   Destination    |     |                    |     |        |                   | ECMP|  FEC | Tunnel
| ID|      Subnet      | Cmd |     Destination    | VID | Outlif |   MAC / CPU Code  |Index| Index|T Value
 ----------------------------------------------------------------------------------------------------------
|0  |0.0.0.0/8         |DROP | DROP               |0    |  -     |                   |  -  |183502|   -   
|0  |10.0.0.30/32      |TRAP | CoppSystemIpUcast  |0    |  -     | Receive           |  -  |314667|   -   
|0  |10.0.0.32/32      |ROUTE| Et2                |1007 |103427  | d4:af:f7:2f:13:96 |  -  |183560|   -   
|0  |10.0.0.53/32      |ROUTE| Et13               |1014 |103421  | 5c:07:58:a3:0a:aa |  -  |183510|   -   
|0  |10.0.0.72/32      |ROUTE| Et9                |1012 |103438  | e0:9b:27:c4:c5:84 |  -  |183574|   -   
|0  |10.0.0.84/32      |ROUTE| Et12               |1013 |103422  | 58:70:7f:9f:c4:03 |  -  |183511|   -   
|0  |10.0.0.120/32     |ROUTE| Et3                |1008 |103426  | bc:31:e2:e1:ec:2c |  -  |183524|   -   
|0  |10.0.0.128/32     |ROUTE| Et19               |1018 |103437  | 60:53:75:13:ba:d8 |  -  |183550|   -   
|0  |10.0.0.175/32     |ROUTE| Et19               |1018 |103437  | 60:53:75:13:ba:d8 |16385|183562|   -   
|0  |10.0.0.175/32     |ROUTE| Et13               |1014 |103421  | 5c:07:58:a3:0a:aa |16385|183563|   -   
|0  |10.0.0.175/32     |ROUTE| Et12               |1013 |103422  | 58:70:7f:9f:c4:03 |16385|183564|   -   
|0  |10.0.0.175/32     |ROUTE| Et40               |1020 |103429  | e8:24:a6:96:05:48 |16385|183565|   -   
|0  |10.0.0.175/32     |ROUTE| Et2                |1007 |103427  | d4:af:f7:2f:13:96 |16385|183566|   -   
|0  |10.0.0.175/32     |ROUTE| Et5                |1010 |103428  | 18:5b:00:61:ac:6f |16385|183567|   -   
|0  |10.0.0.175/32     |ROUTE| Et9                |1012 |103438  | e0:9b:27:c4:c5:84 |16385|183568|   -   
|0  |10.0.0.175/32     |ROUTE| Et17               |1016 |103440  | 64:6d:4e:32:e1:22 |16385|183569|   -   
|0  |10.0.0.179/32     |ROUTE| Et40               |1020 |103429  | e8:24:a6:96:05:48 |  -  |183535|   -   
|0  |10.0.0.214/32     |ROUTE| Et5                |1010 |103428  | 18:5b:00:61:ac:6f |  -  |183516|   -   
|0  |10.0.0.216/32     |ROUTE| Et5                |1010 |103428  | 18:5b:00:61:ac:6f |  -  |183516|   -   
|0  |10.0.0.217/32     |ROUTE| Et4                |1009 |103423  | c0:14:b8:21:97:90 |  -  |183509|   -   
|0  |10.0.0.221/32     |ROUTE| Et15               |1015 |103424  | 30:c5:07:84:3e:79 |  -  |183527|   -   
|0  |20.30.32.0/32     |TRAP | CoppSystemIpBcast  |0    |  -     | BcastReceive      |  -  |314666|   -   
|0  |20.30.32.30/32    |TRAP | CoppSystemIpUcast  |0    |  -     | Receive           |  -  |314667|   -   
|0  |20.30.32.32/32    |ROUTE| Et2                |1007 |103427  | d4:af:f7:2f:13:96 |  -  |183528|   -   
|0  |20.30.32.255/32   |TRAP | CoppSystemIpBcast  |0    |  -     | BcastReceive      |  -  |314666|   -   
|0  |20.30.32.0/24     |TRAP | CoppSystemL3DstMiss|1007 |1007    | ArpTrap           |  -  |315678|   -   
|0  |20.30.53.0/32     |TRAP | CoppSystemIpBcast  |0    |  -     | BcastReceive      |  -  |314666|   -   
|0  |20.30.53.30/32    |TRAP | CoppSystemIpUcast  |0    |  -     | Receive           |  -  |314667|   -   
|0  |20.30.53.53/32    |ROUTE| Et13               |1014 |103421  | 5c:07:58:a3:0a:aa |  -  |183506|   -   
|0  |20.30.53.255/32   |TRAP | CoppSystemIpBcast  |0    |  -     | BcastReceive      |  -  |314666|   -   
|0  |20.30.53.0/24     |TRAP | CoppSystemL3DstMiss|1014 |1014    | ArpTrap           |  -  |315685|   -   
|0  |20.30.66.0/32     |TRAP | CoppSystemIpBcast  |0    |  -     | BcastReceive      |  -  |314666|   -   
|0  |20.30.66.30/32    |TRAP | CoppSystemIpUcast  |0    |  -     | Receive           |  -  |314667|   -   
|0  |20.30.66.66/32    |ROUTE| Et31               |1019 |103436  | e4:6d:7f:e3:c8:08 |  -  |183532|   -   
|0  |20.30.66.255/32   |TRAP | CoppSystemIpBcast  |0    |  -     | BcastReceive      |  -  |314666|   -   
|0  |20.30.66.0/24     |TRAP | CoppSystemL3DstMiss|1019 |1019    | ArpTrap           |  -  |315690|   -   
|0  |20.30.72.0/32     |TRAP | CoppSystemIpBcast  |0    |  -     | BcastReceive      |  -  |314666|   -   
|0  |20.30.72.30/32    |TRAP | CoppSystemIpUcast  |0    |  -     | Receive           |  -  |314667|   -   
|0  |20.30.72.72/32    |ROUTE| Et9                |1012 |103438  | e0:9b:27:c4:c5:84 |  -  |183558|   -   
|0  |20.30.72.255/32   |TRAP | CoppSystemIpBcast  |0    |  -     | BcastReceive      |  -  |314666|   -   
|0  |20.30.72.0/24     |TRAP | CoppSystemL3DstMiss|1012 |1012    | ArpTrap           |  -  |315683|   -   
|0  |20.30.84.0/32     |TRAP | CoppSystemIpBcast  |0    |  -     | BcastReceive      |  -  |314666|   -   
|0  |20.30.84.30/32    |TRAP | CoppSystemIpUcast  |0    |  -     | Receive           |  -  |314667|   -   
|0  |20.30.84.84/32    |ROUTE| Et12               |1013 |103422  | 58:70:7f:9f:c4:03 |  -  |183507|   -   
|0  |20.30.84.255/32   |TRAP | CoppSystemIpBcast  |0    |  -     | BcastReceive      |  -  |314666|   -   
|0  |20.30.84.0/24     |TRAP | CoppSystemL3DstMiss|1013 |1013    | ArpTrap           |  -  |315684|   -   
|0  |20.30.120.0/32    |TRAP | CoppSystemIpBcast  |0    |  -     | BcastReceive      |  -  |314666|   -   
|0  |20.30.120.30/32   |TRAP | CoppSystemIpUcast  |0    |  -     | Receive           |  -  |314667|   -   
|0  |20.30.120.120/32  |ROUTE| Et3                |1008 |103426  | bc:31:e2:e1:ec:2c |  -  |183522|   -   
|0  |20.30.120.255/32  |TRAP | CoppSystemIpBcast  |0    |  -     | BcastReceive      |  -  |314666|   -   
|0  |20.30.120.0/24    |TRAP | CoppSystemL3DstMiss|1008 |1008    | ArpTrap           |  -  |315679|   -   
|0  |20.30.124.0/32    |TRAP | CoppSystemIpBcast  |0    |  -     | BcastReceive      |  -  |314666|   -   
|0  |20.30.124.30/32   |TRAP | CoppSystemIpUcast  |0    |  -     | Receive           |  -  |314667|   -   
|0  |20.30.124.124/32  |ROUTE| Et17               |1016 |103440  | 64:6d:4e:32:e1:22 |  -  |183571|   -   
|0  |20.30.124.255/32  |TRAP | CoppSystemIpBcast  |0    |  -     | BcastReceive      |  -  |314666|   -   
|0  |20.30.124.0/24    |TRAP | CoppSystemL3DstMiss|1016 |1016    | ArpTrap           |  -  |315687|   -   
|0  |20.30.128.0/32    |TRAP | CoppSystemIpBcast  |0    |  -     | BcastReceive      |  -  |314666|   -   
|0  |20.30.128.30/32   |TRAP | CoppSystemIpUcast  |0    |  -     | Receive           |  -  |314667|   -   
|0  |20.30.128.128/32  |ROUTE| Et19               |1018 |103437  | 60:53:75:13:ba:d8 |  -  |183549|   -   
|0  |20.30.128.255/32  |TRAP | CoppSystemIpBcast  |0    |  -     | BcastReceive      |  -  |314666|   -   
|0  |20.30.128.0/24    |TRAP | CoppSystemL3DstMiss|1018 |1018    | ArpTrap           |  -  |315689|   -   
|0  |20.30.179.0/32    |TRAP | CoppSystemIpBcast  |0    |  -     | BcastReceive      |  -  |314666|   -   
|0  |20.30.179.30/32   |TRAP | CoppSystemIpUcast  |0    |  -     | Receive           |  -  |314667|   -   
|0  |20.30.179.179/32  |ROUTE| Et40               |1020 |103429  | e8:24:a6:96:05:48 |  -  |183536|   -   
|0  |20.30.179.255/32  |TRAP | CoppSystemIpBcast  |0    |  -     | BcastReceive      |  -  |314666|   -   
|0  |20.30.179.0/24    |TRAP | CoppSystemL3DstMiss|1020 |1020    | ArpTrap           |  -  |315691|   -   
|0  |20.30.184.0/32    |TRAP | CoppSystemIpBcast  |0    |  -     | BcastReceive      |  -  |314666|   -   
|0  |20.30.184.30/32   |TRAP | CoppSystemIpUcast  |0    |  -     | Receive           |  -  |314667|   -   
|0  |20.30.184.255/32  |TRAP | CoppSystemIpBcast  |0    |  -     | BcastReceive      |  -  |314666|   -   
|0  |20.30.184.0/24    |TRAP | CoppSystemL3DstMiss|1011 |1011    | ArpTrap           |  -  |315682|   -   
|0  |20.30.214.0/32    |TRAP | CoppSystemIpBcast  |0    |  -     | BcastReceive      |  -  |314666|   -   
|0  |20.30.214.30/32   |TRAP | CoppSystemIpUcast  |0    |  -     | Receive           |  -  |314667|   -   
|0  |20.30.214.214/32  |ROUTE| Et5                |1010 |103428  | 18:5b:00:61:ac:6f |  -  |183533|   -   
|0  |20.30.214.255/32  |TRAP | CoppSystemIpBcast  |0    |  -     | BcastReceive      |  -  |314666|   -   
|0  |20.30.214.0/24    |TRAP | CoppSystemL3DstMiss|1010 |1010    | ArpTrap           |  -  |315681|   -   
|0  |20.30.217.0/32    |TRAP | CoppSystemIpBcast  |0    |  -     | BcastReceive      |  -  |314666|   -   
|0  |20.30.217.30/32   |TRAP | CoppSystemIpUcast  |0    |  -     | Receive           |  -  |314667|   -   
|0  |20.30.217.217/32  |ROUTE| Et4                |1009 |103423  | c0:14:b8:21:97:90 |  -  |183508|   -   
|0  |20.30.217.255/32  |TRAP | CoppSystemIpBcast  |0    |  -     | BcastReceive      |  -  |314666|   -   
|0  |20.30.217.0/24    |TRAP | CoppSystemL3DstMiss|1009 |1009    | ArpTrap           |  -  |315680|   -   
|0  |20.30.221.0/32    |TRAP | CoppSystemIpBcast  |0    |  -     | BcastReceive      |  -  |314666|   -   
|0  |20.30.221.30/32   |TRAP | CoppSystemIpUcast  |0    |  -     | Receive           |  -  |314667|   -   
|0  |20.30.221.221/32  |ROUTE| Et15               |1015 |103424  | 30:c5:07:84:3e:79 |  -  |183519|   -   
|0  |20.30.221.255/32  |TRAP | CoppSystemIpBcast  |0    |  -     | BcastReceive      |  -  |314666|   -   
|0  |20.30.221.0/24    |TRAP | CoppSystemL3DstMiss|1015 |1015    | ArpTrap           |  -  |315686|   -   
|0  |20.32.175.0/24    |ROUTE| Et2                |1007 |103427  | d4:af:f7:2f:13:96 |  -  |183560|   -   
|0  |20.53.175.0/24    |ROUTE| Et13               |1014 |103421  | 5c:07:58:a3:0a:aa |  -  |183510|   -   
|0  |20.66.175.0/24    |ROUTE| Et19               |1018 |103437  | 60:53:75:13:ba:d8 |16385|183562|   -   
|0  |20.66.175.0/24    |ROUTE| Et13               |1014 |103421  | 5c:07:58:a3:0a:aa |16385|183563|   -   
|0  |20.66.175.0/24    |ROUTE| Et12               |1013 |103422  | 58:70:7f:9f:c4:03 |16385|183564|   -   
|0  |20.66.175.0/24    |ROUTE| Et40               |1020 |103429  | e8:24:a6:96:05:48 |16385|183565|   -   
|0  |20.66.175.0/24    |ROUTE| Et2                |1007 |103427  | d4:af:f7:2f:13:96 |16385|183566|   -   
|0  |20.66.175.0/24    |ROUTE| Et5                |1010 |103428  | 18:5b:00:61:ac:6f |16385|183567|   -   
|0  |20.66.175.0/24    |ROUTE| Et9                |1012 |103438  | e0:9b:27:c4:c5:84 |16385|183568|   -   
|0  |20.66.175.0/24    |ROUTE| Et17               |1016 |103440  | 64:6d:4e:32:e1:22 |16385|183569|   -   
|0  |20.72.175.0/24    |ROUTE| Et9                |1012 |103438  | e0:9b:27:c4:c5:84 |  -  |183574|   -   
|0  |20.84.175.0/24    |ROUTE| Et19               |1018 |103437  | 60:53:75:13:ba:d8 |16385|183562|   -   
|0  |20.84.175.0/24    |ROUTE| Et13               |1014 |103421  | 5c:07:58:a3:0a:aa |16385|183563|   -   
|0  |20.84.175.0/24    |ROUTE| Et12               |1013 |103422  | 58:70:7f:9f:c4:03 |16385|183564|   -   
|0  |20.84.175.0/24    |ROUTE| Et40               |1020 |103429  | e8:24:a6:96:05:48 |16385|183565|   -   
|0  |20.84.175.0/24    |ROUTE| Et2                |1007 |103427  | d4:af:f7:2f:13:96 |16385|183566|   -   
|0  |20.84.175.0/24    |ROUTE| Et5                |1010 |103428  | 18:5b:00:61:ac:6f |16385|183567|   -   
|0  |20.84.175.0/24    |ROUTE| Et9                |1012 |103438  | e0:9b:27:c4:c5:84 |16385|183568|   -   
|0  |20.84.175.0/24    |ROUTE| Et17               |1016 |103440  | 64:6d:4e:32:e1:22 |16385|183569|   -   
|0  |20.120.175.0/24   |ROUTE| Et19               |1018 |103437  | 60:53:75:13:ba:d8 |16385|183562|   -   
|0  |20.120.175.0/24   |ROUTE| Et13               |1014 |103421  | 5c:07:58:a3:0a:aa |16385|183563|   -   
|0  |20.120.175.0/24   |ROUTE| Et12               |1013 |103422  | 58:70:7f:9f:c4:03 |16385|183564|   -   
|0  |20.120.175.0/24   |ROUTE| Et40               |1020 |103429  | e8:24:a6:96:05:48 |16385|183565|   -   
|0  |20.120.175.0/24   |ROUTE| Et2                |1007 |103427  | d4:af:f7:2f:13:96 |16385|183566|   -   
|0  |20.120.175.0/24   |ROUTE| Et5                |1010 |103428  | 18:5b:00:61:ac:6f |16385|183567|   -   
|0  |20.120.175.0/24   |ROUTE| Et9                |1012 |103438  | e0:9b:27:c4:c5:84 |16385|183568|   -   
|0  |20.120.175.0/24   |ROUTE| Et17               |1016 |103440  | 64:6d:4e:32:e1:22 |16385|183569|   -   
|0  |20.120.214.0/24   |ROUTE| Et3                |1008 |103426  | bc:31:e2:e1:ec:2c |  -  |183524|   -   
|0  |20.124.175.0/24   |ROUTE| Et17               |1016 |103440  | 64:6d:4e:32:e1:22 |  -  |183572|   -   
|0  |20.128.175.0/24   |ROUTE| Et19               |1018 |103437  | 60:53:75:13:ba:d8 |  -  |183550|   -   
|0  |20.131.175.0/24   |ROUTE| Et19               |1018 |103437  | 60:53:75:13:ba:d8 |16385|183562|   -   
|0  |20.131.175.0/24   |ROUTE| Et13               |1014 |103421  | 5c:07:58:a3:0a:aa |16385|183563|   -   
|0  |20.131.175.0/24   |ROUTE| Et12               |1013 |103422  | 58:70:7f:9f:c4:03 |16385|183564|   -   
|0  |20.131.175.0/24   |ROUTE| Et40               |1020 |103429  | e8:24:a6:96:05:48 |16385|183565|   -   
|0  |20.131.175.0/24   |ROUTE| Et2                |1007 |103427  | d4:af:f7:2f:13:96 |16385|183566|   -   
|0  |20.131.175.0/24   |ROUTE| Et5                |1010 |103428  | 18:5b:00:61:ac:6f |16385|183567|   -   
|0  |20.131.175.0/24   |ROUTE| Et9                |1012 |103438  | e0:9b:27:c4:c5:84 |16385|183568|   -   
|0  |20.131.175.0/24   |ROUTE| Et17               |1016 |103440  | 64:6d:4e:32:e1:22 |16385|183569|   -   
|0  |20.175.179.0/24   |ROUTE| Et40               |1020 |103429  | e8:24:a6:96:05:48 |  -  |183535|   -   
|0  |20.175.184.0/24   |ROUTE| Et19               |1018 |103437  | 60:53:75:13:ba:d8 |16385|183562|   -   
|0  |20.175.184.0/24   |ROUTE| Et13               |1014 |103421  | 5c:07:58:a3:0a:aa |16385|183563|   -   
|0  |20.175.184.0/24   |ROUTE| Et12               |1013 |103422  | 58:70:7f:9f:c4:03 |16385|183564|   -   
|0  |20.175.184.0/24   |ROUTE| Et40               |1020 |103429  | e8:24:a6:96:05:48 |16385|183565|   -   
|0  |20.175.184.0/24   |ROUTE| Et2                |1007 |103427  | d4:af:f7:2f:13:96 |16385|183566|   -   
|0  |20.175.184.0/24   |ROUTE| Et5                |1010 |103428  | 18:5b:00:61:ac:6f |16385|183567|   -   
|0  |20.175.184.0/24   |ROUTE| Et9                |1012 |103438  | e0:9b:27:c4:c5:84 |16385|183568|   -   
|0  |20.175.184.0/24   |ROUTE| Et17               |1016 |103440  | 64:6d:4e:32:e1:22 |16385|183569|   -   
|0  |20.175.214.0/24   |ROUTE| Et5                |1010 |103428  | 18:5b:00:61:ac:6f |  -  |183516|   -   
|0  |20.175.217.0/24   |ROUTE| Et4                |1009 |103423  | c0:14:b8:21:97:90 |  -  |183509|   -   
|0  |20.175.221.0/24   |ROUTE| Et15               |1015 |103424  | 30:c5:07:84:3e:79 |  -  |183527|   -   
|0  |20.214.216.0/24   |ROUTE| Et5                |1010 |103428  | 18:5b:00:61:ac:6f |  -  |183516|   -   
|0  |127.0.0.0/8       |TRAP | CoppSystemL3DstMiss|0    |  -     | ArpTrap           |  -  |314671|   -   
|0  |0.0.0.0/0         |TRAP | CoppSystemL3LpmOver|0    |  -     | SlowReceive       |  -  |314669|   -   
|1  |0.0.0.0/8         |DROP | DROP               |0    |  -     |                   |  -  |183503|   -   
|1  |127.0.0.0/8       |TRAP | CoppSystemL3DstMiss|0    |  -     | ArpTrap           |  -  |314671|   -   
|1  |192.168.20.0/32   |TRAP | CoppSystemIpBcast  |0    |  -     | BcastReceive      |  -  |314666|   -   
|1  |192.168.20.30/32  |TRAP | CoppSystemIpUcast  |0    |  -     | Receive           |  -  |314667|   -   
|1  |192.168.21.255/32 |TRAP | CoppSystemIpBcast  |0    |  -     | BcastReceive      |  -  |314666|   -   
|1  |192.168.20.0/23   |TRAP | CoppSystemL3DstMiss|0    |  -     | ArpTrap           |  -  |314671|   -   
|1  |0.0.0.0/0         |TRAP | CoppSystemL3DstMiss|0    |  -     | ArpTrap           |  -  |314671|   -   
|2  |0.0.0.0/8         |DROP | DROP               |0    |  -     |                   |  -  |183505|   -   
|2  |10.0.0.30/32      |TRAP | CoppSystemIpUcast  |0    |  -     | Receive           |  -  |314667|   -   
|2  |50.10.32.0/24     |ROUTE| FEC 183521         |0    |2097148 | 00:00:00:00:00:00 |  -  |131079|M 378528
|2  |50.10.72.0/24     |ROUTE| FEC 183559         |0    |2097147 | 00:00:00:00:00:00 |  -  |131080|M 62002
|2  |50.10.84.0/24     |ROUTE| FEC 183540         |0    |2097146 | 00:00:00:00:00:00 |  -  |131072|M 20084 720896
|2  |50.10.120.0/24    |ROUTE| FEC 183542         |0    |2097143 | 00:00:00:00:00:00 |  -  |131081|M 1277
|2  |50.10.179.0/24    |ROUTE| FEC 183520         |0    |2097151 | 00:00:00:00:00:00 |  -  |131075|M 16
|2  |50.10.214.0/24    |ROUTE| FEC 183515         |0    |2097149 | 00:00:00:00:00:00 |  -  |131073|M 20214 500000
|2  |50.10.217.0/24    |ROUTE| FEC 183518         |0    |2097145 | 00:00:00:00:00:00 |  -  |131074|M 20217 524287
|2  |50.10.221.0/24    |ROUTE| FEC 183538         |0    |2097144 | 00:00:00:00:00:00 |  -  |131078|M 524289
|2  |51.10.120.0/24    |ROUTE| FEC 183542         |0    |2097143 | 00:00:00:00:00:00 |  -  |131081|M 1277
|2  |127.0.0.0/8       |TRAP | CoppSystemL3DstMiss|0    |  -     | ArpTrap           |  -  |314671|   -   
|2  |0.0.0.0/0         |TRAP | CoppSystemL3LpmOver|0    |  -     | SlowReceive       |  -  |314669|   -   

```

## show platform jericho2 fec all

```text
Tunnel Type: Mpop(mpls pop), Mpush(mpls push), Mswap(mpls swap),
             MoG(mpls-over-gre), T(IPv4 tunnels GRE/GUE/VXLAN),
             N(Ipsec tunnel NAT-T [IP,SPORT,DPORT])
CW  - Control word
FL  - Flow label
EL  - Entropy label
ELI - Entropy label indicator
D   - ECMP is divergent across switching chips
 -----------------------------------------------------------------------------------------------
|                                              FEC Entry                                        |
 -----------------------------------------------------------------------------------------------
|     |      |     |                    |     |        |                   |
| ECMP|  FEC |     |                    |     |        |                   |
|Index| Index| Cmd |     Destination    | VID | Outlif |   MAC / CPU Code  |    Tunnel Value
 -----------------------------------------------------------------------------------------------
|16385|183562|ROUTE| Et19               |1018 |103437  | 60:53:75:13:ba:d8 |   -   
|16385|183563|ROUTE| Et13               |1014 |103421  | 5c:07:58:a3:0a:aa |   -   
|16385|183564|ROUTE| Et12               |1013 |103422  | 58:70:7f:9f:c4:03 |   -   
|16385|183565|ROUTE| Et40               |1020 |103429  | e8:24:a6:96:05:48 |   -   
|16385|183566|ROUTE| Et2                |1007 |103427  | d4:af:f7:2f:13:96 |   -   
|16385|183567|ROUTE| Et5                |1010 |103428  | 18:5b:00:61:ac:6f |   -   
|16385|183568|ROUTE| Et9                |1012 |103438  | e0:9b:27:c4:c5:84 |   -   
|16385|183569|ROUTE| Et17               |1016 |103440  | 64:6d:4e:32:e1:22 |   -   
|16387|183576|ROUTE| Et19               |1018 |103439  | 60:53:75:13:ba:d8 |Mswap 20175
|16387|183577|ROUTE| Et40               |1020 |103425  | e8:24:a6:96:05:48 |Mswap 20175
|16387|183578|ROUTE| Et17               |1016 |103441  | 64:6d:4e:32:e1:22 |Mswap 2175
|16387|183579|ROUTE| Et5                |1010 |103431  | 18:5b:00:61:ac:6f |Mswap 20175
|16387|183580|ROUTE| Et12               |1013 |103434  | 58:70:7f:9f:c4:03 |Mswap 20175
|16387|183581|ROUTE| Et9                |1012 |103446  | e0:9b:27:c4:c5:84 |Mswap 20175
|16387|183582|ROUTE| Et13               |1014 |103435  | 5c:07:58:a3:0a:aa |Mswap 20175
|16387|183583|ROUTE| Et2                |1007 |103433  | d4:af:f7:2f:13:96 |Mswap 20175
|  -  |131072|ROUTE| FEC 183540         |   - |2097146 |                 - |Mpush 20084 720896
|  -  |131073|ROUTE| FEC 183515         |   - |2097149 |                 - |Mpush 20214 500000
|  -  |131074|ROUTE| FEC 183518         |   - |2097145 |                 - |Mpush 20217 524287
|  -  |131075|ROUTE| FEC 183520         |   - |2097151 |                 - |Mpush 16
|  -  |131077|ROUTE| FEC 183541         |   - |  -     |                   |   -   
|  -  |131078|ROUTE| FEC 183538         |   - |2097144 |                 - |Mpush 524289
|  -  |131079|ROUTE| FEC 183521         |   - |2097148 |                 - |Mpush 378528
|  -  |131080|ROUTE| FEC 183559         |   - |2097147 |                 - |Mpush 62002
|  -  |131081|ROUTE| FEC 183542         |   - |2097143 |                 - |Mpush 1277
|  -  |183502|DROP | DROP               |0    |  -     |                   |   -   
|  -  |183503|DROP | DROP               |0    |  -     |                   |   -   
|  -  |183504|DROP | DROP               |0    |  -     |                   |   -   
|  -  |183505|DROP | DROP               |0    |  -     |                   |   -   
|  -  |183506|ROUTE| Et13               |1014 |103421  | 5c:07:58:a3:0a:aa |   -   
|  -  |183507|ROUTE| Et12               |1013 |103422  | 58:70:7f:9f:c4:03 |   -   
|  -  |183508|ROUTE| Et4                |1009 |103423  | c0:14:b8:21:97:90 |   -   
|  -  |183509|ROUTE| Et4                |1009 |103423  | c0:14:b8:21:97:90 |   -   
|  -  |183510|ROUTE| Et13               |1014 |103421  | 5c:07:58:a3:0a:aa |   -   
|  -  |183511|ROUTE| Et12               |1013 |103422  | 58:70:7f:9f:c4:03 |   -   
|  -  |183512|ROUTE| Et12               |1013 |103422  | 58:70:7f:9f:c4:03 |   -   
|  -  |183513|ROUTE| Et13               |1014 |103421  | 5c:07:58:a3:0a:aa |   -   
|  -  |183514|ROUTE| Et4                |1009 |103423  | c0:14:b8:21:97:90 |   -   
|  -  |183515|ROUTE| Et5                |1010 |103428  | 18:5b:00:61:ac:6f |   -   
|  -  |183516|ROUTE| Et5                |1010 |103428  | 18:5b:00:61:ac:6f |   -   
|  -  |183517|ROUTE| Et5                |1010 |103428  | 18:5b:00:61:ac:6f |   -   
|  -  |183518|ROUTE| Et4                |1009 |103423  | c0:14:b8:21:97:90 |   -   
|  -  |183519|ROUTE| Et15               |1015 |103424  | 30:c5:07:84:3e:79 |   -   
|  -  |183520|ROUTE| Et40               |1020 |103429  | e8:24:a6:96:05:48 |   -   
|  -  |183521|ROUTE| Et2                |1007 |103427  | d4:af:f7:2f:13:96 |   -   
|  -  |183522|ROUTE| Et3                |1008 |103426  | bc:31:e2:e1:ec:2c |   -   
|  -  |183523|ROUTE| Et3                |1008 |103426  | bc:31:e2:e1:ec:2c |   -   
|  -  |183524|ROUTE| Et3                |1008 |103426  | bc:31:e2:e1:ec:2c |   -   
|  -  |183525|ROUTE| Et3                |1008 |103426  | bc:31:e2:e1:ec:2c |   -   
|  -  |183526|ROUTE| Et3                |1008 |103426  | bc:31:e2:e1:ec:2c |   -   
|  -  |183527|ROUTE| Et15               |1015 |103424  | 30:c5:07:84:3e:79 |   -   
|  -  |183528|ROUTE| Et2                |1007 |103427  | d4:af:f7:2f:13:96 |   -   
|  -  |183529|ROUTE| Et2                |1007 |103427  | d4:af:f7:2f:13:96 |   -   
|  -  |183530|ROUTE| Et2                |1007 |103427  | d4:af:f7:2f:13:96 |   -   
|  -  |183531|ROUTE| Et15               |1015 |103424  | 30:c5:07:84:3e:79 |   -   
|  -  |183532|ROUTE| Et31               |1019 |103436  | e4:6d:7f:e3:c8:08 |   -   
|  -  |183533|ROUTE| Et5                |1010 |103428  | 18:5b:00:61:ac:6f |   -   
|  -  |183534|ROUTE| Et12               |1013 |103422  | 58:70:7f:9f:c4:03 |   -   
|  -  |183535|ROUTE| Et40               |1020 |103429  | e8:24:a6:96:05:48 |   -   
|  -  |183536|ROUTE| Et40               |1020 |103429  | e8:24:a6:96:05:48 |   -   
|  -  |183537|ROUTE| Et40               |1020 |103429  | e8:24:a6:96:05:48 |   -   
|  -  |183538|ROUTE| Et15               |1015 |103424  | 30:c5:07:84:3e:79 |   -   
|  -  |183539|ROUTE| Et2                |1007 |103427  | d4:af:f7:2f:13:96 |   -   
|  -  |183540|ROUTE| Et12               |1013 |103422  | 58:70:7f:9f:c4:03 |   -   
|  -  |183541|ROUTE| Et13               |1014 |103430  | 5c:07:58:a3:0a:aa |Mpush 0
|  -  |183542|ROUTE| Et3                |1008 |103426  | bc:31:e2:e1:ec:2c |   -   
|  -  |183549|ROUTE| Et19               |1018 |103437  | 60:53:75:13:ba:d8 |   -   
|  -  |183550|ROUTE| Et19               |1018 |103437  | 60:53:75:13:ba:d8 |   -   
|  -  |183558|ROUTE| Et9                |1012 |103438  | e0:9b:27:c4:c5:84 |   -   
|  -  |183559|ROUTE| Et9                |1012 |103438  | e0:9b:27:c4:c5:84 |   -   
|  -  |183560|ROUTE| Et2                |1007 |103427  | d4:af:f7:2f:13:96 |   -   
|  -  |183561|ROUTE| Et19               |1018 |103437  | 60:53:75:13:ba:d8 |   -   
|  -  |183570|ROUTE| Et19               |1018 |103437  | 60:53:75:13:ba:d8 |   -   
|  -  |183571|ROUTE| Et17               |1016 |103440  | 64:6d:4e:32:e1:22 |   -   
|  -  |183572|ROUTE| Et17               |1016 |103440  | 64:6d:4e:32:e1:22 |   -   
|  -  |183573|ROUTE| Et17               |1016 |103440  | 64:6d:4e:32:e1:22 |   -   
|  -  |183574|ROUTE| Et9                |1012 |103438  | e0:9b:27:c4:c5:84 |   -   
|  -  |183575|ROUTE| Et9                |1012 |103438  | e0:9b:27:c4:c5:84 |   -   
|  -  |314666|TRAP | CoppSystemIpBcast  |0    |  -     | BcastReceive      |   -   
|  -  |314667|TRAP | CoppSystemIpUcast  |0    |  -     | Receive           |   -   
|  -  |314669|TRAP | CoppSystemL3LpmOver|0    |  -     | SlowReceive       |   -   
|  -  |314671|TRAP | CoppSystemL3DstMiss|0    |  -     | ArpTrap           |   -   
|  -  |315678|TRAP | CoppSystemL3DstMiss|1007 |1007    | ArpTrap           |   -   
|  -  |315679|TRAP | CoppSystemL3DstMiss|1008 |1008    | ArpTrap           |   -   
|  -  |315680|TRAP | CoppSystemL3DstMiss|1009 |1009    | ArpTrap           |   -   
|  -  |315681|TRAP | CoppSystemL3DstMiss|1010 |1010    | ArpTrap           |   -   
|  -  |315682|TRAP | CoppSystemL3DstMiss|1011 |1011    | ArpTrap           |   -   
|  -  |315683|TRAP | CoppSystemL3DstMiss|1012 |1012    | ArpTrap           |   -   
|  -  |315684|TRAP | CoppSystemL3DstMiss|1013 |1013    | ArpTrap           |   -   
|  -  |315685|TRAP | CoppSystemL3DstMiss|1014 |1014    | ArpTrap           |   -   
|  -  |315686|TRAP | CoppSystemL3DstMiss|1015 |1015    | ArpTrap           |   -   
|  -  |315687|TRAP | CoppSystemL3DstMiss|1016 |1016    | ArpTrap           |   -   
|  -  |315689|TRAP | CoppSystemL3DstMiss|1018 |1018    | ArpTrap           |   -   
|  -  |315690|TRAP | CoppSystemL3DstMiss|1019 |1019    | ArpTrap           |   -   
|  -  |315691|TRAP | CoppSystemL3DstMiss|1020 |1020    | ArpTrap           |   -   

```

