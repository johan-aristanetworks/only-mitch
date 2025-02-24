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

Uptime: 9 hours and 32 minutes
Total memory: 8099700 kB
Free memory: 5125536 kB

```

## show lldp neighbors

```text
Last table change time   : 0:03:58 ago
Number of table inserts  : 58
Number of table deletes  : 44
Number of table drops    : 0
Number of table age-outs : 0

Port      Neighbor Device ID                    Neighbor Port ID            TTL
------- ------------------------------------- ----------------------------- ---
Et1       Arista-PE31-Q2C-31.ns.eantc.de        Ethernet1                   120
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
Ethernet1       20.30.31.30/24      up         up                1500          
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
Ethernet40      20.30.179.30/24     up         up                1500          
Loopback0       10.0.0.30/32        up         up               65535          
Loopback5001    10.0.0.30/32        up         up               65535          
Management1     192.168.20.30/23    up         up                1500          

```

## show interfaces counters rates | nz

```text
Port      Name                 Intvl  In Mbps      %  In Kpps Out Mbps      %
Et9       Ciena-5134-72 port 2  0:01      0.0   0.0%        0      0.0   0.0%

Port      Out Kpps
```

## show isis neighbors

```text
 
Instance  VRF      System Id        Type Interface          SNPA              State Hold time   Circuit Id          
IGP       default  Arista-PE31-Q2C-31 L2   Ethernet1          P2P               UP    22          2B                  
IGP       default  Arista-PE32-Q2C-32 L2   Ethernet2          P2P               UP    22          44                  
IGP       default  Arrcus-53        L2   Ethernet13         P2P               UP    23          00                  
IGP       default  Ciena-5134-72    L2   Ethernet9          P2P               UP    27          02                  
IGP       default  Ericsson_84_R6678 L2   Ethernet12         P2P               UP    29          02                  
IGP       default  H3C_M1A_120      L2   Ethernet3          P2P               UP    23          01                  
IGP       default  0000.0000.0124   L2   Ethernet17         P2P               UP    26          09                  
IGP       default  0000.0000.0128   L2   Ethernet19         P2P               UP    28          09                  
IGP       default  Juniper-179-ACX7024 L2   Ethernet40         P2P               UP    24          01                  
IGP       default  Nokia-SXR-214    L2   Ethernet5          P2P               UP    22          00                  
IGP       default  Nokia-SR1-217    L2   Ethernet4          P2P               UP    20          00                  
IGP       default  221              L2   Ethernet15         P2P               UP    83          00                  
```

## show isis database detail

```text
Legend:
H - hostname conflict
U - node unreachable

IS-IS Instance: IGP VRF: default
  IS-IS Level 2 Link State Database
    LSPID                   Seq Num  Cksum  Life Length IS  Received LSPID        Flags
    Arista-Spine3-Q2A-30.00-00       195  43916   896   1102 L2  0000.0000.0030.00-00  <>
      LSP generation remaining wait time: 0 ms
      Time remaining until refresh: 596 s
      NLPID: 0xCC(IPv4) 0x8E(IPv6)
      Hostname: Arista-Spine3-Q2A-30
      Area addresses: 49.0001
      Topology: 2 (IPv6)
      Topology: 0 (IPv4)
      Interface address: 20.30.179.30
      Interface address: 20.30.124.30
      Interface address: 20.30.128.30
      Interface address: 20.30.184.30
      Interface address: 20.30.217.30
      Interface address: 20.30.221.30
      Interface address: 20.30.72.30
      Interface address: 20.30.53.30
      Interface address: 20.30.84.30
      Interface address: 20.30.214.30
      Interface address: 20.30.120.30
      Interface address: 20.30.31.30
      Interface address: 20.30.32.30
      Interface address: 10.0.0.30
      Interface address: 2001:0:30:179::30
      Interface address: 2001:0:30:124::30
      Interface address: 2001:0:30:128::30
      Interface address: 2001:0:30:184::30
      Interface address: 2001:0:30:217::30
      Interface address: 2001:0:30:221::30
      Interface address: 2001:0:30:72::30
      Interface address: 2001:0:53:120::30
      Interface address: 2001:0:30:84::30
      Interface address: 2001:0:30:214::30
      Interface address: 2001:0:30:120::30
      Interface address: 2001:0:30:31::30
      Interface address: 2001:0:30:32::30
      IS Neighbor          : Juniper-179-ACX7024.00 Metric: 10
        IPv4 Neighbor Address: 20.30.179.179
        IPv4 Interface Address: 20.30.179.30
        Adj-sid: 362168 flags: [L V] weight: 0x0
      IS Neighbor          : 0000.0000.0124.00   Metric: 10
        IPv4 Neighbor Address: 20.30.124.124
        IPv4 Interface Address: 20.30.124.30
        Adj-sid: 362175 flags: [L V] weight: 0x0
      IS Neighbor          : 0000.0000.0128.00   Metric: 10
        IPv4 Neighbor Address: 20.30.128.128
        IPv4 Interface Address: 20.30.128.30
        Adj-sid: 362174 flags: [L V] weight: 0x0
      IS Neighbor          : Nokia-SR1-217.00    Metric: 10
        IPv4 Neighbor Address: 20.30.217.217
        IPv4 Interface Address: 20.30.217.30
        Adj-sid: 362171 flags: [L V] weight: 0x0
      IS Neighbor          : Arista-PE31-Q2C-31.00 Metric: 10
        IPv4 Neighbor Address: 20.30.31.31
        IPv4 Interface Address: 20.30.31.30
        Adj-sid: 362164 flags: [L V] weight: 0x0
      IS Neighbor          : Arista-PE32-Q2C-32.00 Metric: 10
        IPv4 Neighbor Address: 20.30.32.32
        IPv4 Interface Address: 20.30.32.30
        Adj-sid: 362159 flags: [L V] weight: 0x0
      IS Neighbor          : Ericsson_84_R6678.00 Metric: 10
        IPv4 Neighbor Address: 20.30.84.84
        IPv4 Interface Address: 20.30.84.30
        Adj-sid: 362167 flags: [L V] weight: 0x0
      IS Neighbor          : Nokia-SXR-214.00    Metric: 10
        IPv4 Neighbor Address: 20.30.214.214
        IPv4 Interface Address: 20.30.214.30
        Adj-sid: 362166 flags: [L V] weight: 0x0
      IS Neighbor          : Arrcus-53.00        Metric: 10
        IPv4 Neighbor Address: 20.30.53.53
        IPv4 Interface Address: 20.30.53.30
        Adj-sid: 362165 flags: [L V] weight: 0x0
      IS Neighbor          : H3C_M1A_120.00      Metric: 10
        IPv4 Neighbor Address: 20.30.120.120
        IPv4 Interface Address: 20.30.120.30
        Adj-sid: 362162 flags: [L V] weight: 0x0
      IS Neighbor          : Ciena-5134-72.00    Metric: 10
        IPv4 Neighbor Address: 20.30.72.72
        IPv4 Interface Address: 20.30.72.30
        Adj-sid: 362161 flags: [L V] weight: 0x0
      IS Neighbor          : 221.00              Metric: 10
        IPv4 Neighbor Address: 20.30.221.221
        IPv4 Interface Address: 20.30.221.30
        Adj-sid: 362160 flags: [L V] weight: 0x0
      IS Neighbor (MT-IPv6): Arista-PE31-Q2C-31.00 Metric: 10
        Adj-sid: 362170 flags: [L V F] weight: 0x0
      IS Neighbor (MT-IPv6): Arista-PE32-Q2C-32.00 Metric: 10
        Adj-sid: 362169 flags: [L V F] weight: 0x0
      IS Neighbor (MT-IPv6): H3C_M1A_120.00      Metric: 10
        Adj-sid: 362163 flags: [L V F] weight: 0x0
      Reachability         : 20.30.179.0/24 Metric: 10 Type: 1 Up
      Reachability         : 20.30.124.0/24 Metric: 10 Type: 1 Up
      Reachability         : 20.30.128.0/24 Metric: 10 Type: 1 Up
      Reachability         : 20.30.184.0/24 Metric: 10 Type: 1 Up
      Reachability         : 20.30.217.0/24 Metric: 10 Type: 1 Up
      Reachability         : 20.30.221.0/24 Metric: 10 Type: 1 Up
      Reachability         : 20.30.72.0/24 Metric: 10 Type: 1 Up
      Reachability         : 20.30.53.0/24 Metric: 10 Type: 1 Up
      Reachability         : 20.30.84.0/24 Metric: 10 Type: 1 Up
      Reachability         : 20.30.214.0/24 Metric: 10 Type: 1 Up
      Reachability         : 20.30.120.0/24 Metric: 10 Type: 1 Up
      Reachability         : 20.30.31.0/24 Metric: 10 Type: 1 Up
      Reachability         : 20.30.32.0/24 Metric: 10 Type: 1 Up
      Reachability         : 10.0.0.30/32 Metric: 0 Type: 1 Up
        SR Prefix-SID: 30 Flags: [N] Algorithm: 0
      Reachability (MT-IPv6): 2001:0:30:179::/64 Metric: 10 Type: 1 Up
      Reachability (MT-IPv6): 2001:0:30:124::/64 Metric: 10 Type: 1 Up
      Reachability (MT-IPv6): 2001:0:30:128::/64 Metric: 10 Type: 1 Up
      Reachability (MT-IPv6): 2001:0:30:184::/64 Metric: 10 Type: 1 Up
      Reachability (MT-IPv6): 2001:0:30:217::/64 Metric: 10 Type: 1 Up
      Reachability (MT-IPv6): 2001:0:30:221::/64 Metric: 10 Type: 1 Up
      Reachability (MT-IPv6): 2001:0:30:72::/64 Metric: 10 Type: 1 Up
      Reachability (MT-IPv6): 2001:0:53:120::/64 Metric: 10 Type: 1 Up
      Reachability (MT-IPv6): 2001:0:30:84::/64 Metric: 10 Type: 1 Up
      Reachability (MT-IPv6): 2001:0:30:214::/64 Metric: 10 Type: 1 Up
      Reachability (MT-IPv6): 2001:0:30:120::/64 Metric: 10 Type: 1 Up
      Reachability (MT-IPv6): 2001:0:30:31::/64 Metric: 10 Type: 1 Up
      Reachability (MT-IPv6): 2001:0:30:32::/64 Metric: 10 Type: 1 Up
      Router Capabilities: Router Id: 10.0.0.30 Flags: []
        SR Local Block:
          SRLB Base: 965536 Range: 65536
        Area leader priority: 250 algorithm: 0
        Maximum SID depth:
          Base MPLS imposition (MSD type 1):  12
        SR Capability: Flags: [I V]
          SRGB Base: 20000 Range: 2000
    Arista-PE31-Q2C-31.00-00        43  20866   619    234 L2  0000.0000.0031.00-00  <>
      Remaining lifetime received: 1199 s Modified to: 1200 s
      NLPID: 0xCC(IPv4) 0x8E(IPv6)
      Hostname: Arista-PE31-Q2C-31
      Area addresses: 49.0001
      Topology: 2 (IPv6)
      Topology: 0 (IPv4)
      Interface address: 20.31.175.31
      Interface address: 20.30.31.31
      Interface address: 10.0.0.31
      IS Neighbor          : Juniper-175-ACX7100-48L.00 Metric: 10
        IPv4 Neighbor Address: 20.31.175.175
        IPv4 Interface Address: 20.31.175.31
        Adj-sid: 394915 flags: [L V] weight: 0x0
      IS Neighbor          : Arista-Spine3-Q2A-30.00 Metric: 10
        IPv4 Neighbor Address: 20.30.31.30
        IPv4 Interface Address: 20.30.31.31
        Adj-sid: 394914 flags: [L V] weight: 0x0
      IS Neighbor (MT-IPv6): Arista-Spine3-Q2A-30.00 Metric: 10
        Adj-sid: 394916 flags: [L V F] weight: 0x0
      Reachability         : 20.31.175.0/24 Metric: 10 Type: 1 Up
      Reachability         : 20.30.31.0/24 Metric: 10 Type: 1 Up
      Reachability         : 10.0.0.31/32 Metric: 0 Type: 1 Up
        SR Prefix-SID: 31 Flags: [N] Algorithm: 0
      Router Capabilities: Router Id: 10.0.0.31 Flags: []
        SR Local Block:
          SRLB Base: 965536 Range: 65536
        Area leader priority: 250 algorithm: 0
        Maximum SID depth:
          Base MPLS imposition (MSD type 1):  12
        SR Capability: Flags: [I V]
          SRGB Base: 20000 Range: 2000
    Arista-PE32-Q2C-32.00-00        30  35910   539    270 L2  0000.0000.0032.00-00  <>
      Remaining lifetime received: 1199 s Modified to: 1200 s
      NLPID: 0xCC(IPv4) 0x8E(IPv6)
      Hostname: Arista-PE32-Q2C-32
      Area addresses: 49.0001
      Topology: 2 (IPv6)
      Topology: 0 (IPv4)
      Interface address: 20.32.175.32
      Interface address: 20.30.32.32
      Interface address: 10.0.0.32
      Interface address: 2001:0:30:32::32
      IS Neighbor          : Juniper-175-ACX7100-48L.00 Metric: 10
        IPv4 Neighbor Address: 20.32.175.175
        IPv4 Interface Address: 20.32.175.32
        Adj-sid: 362148 flags: [L V] weight: 0x0
      IS Neighbor          : Arista-Spine3-Q2A-30.00 Metric: 10
        IPv4 Neighbor Address: 20.30.32.30
        IPv4 Interface Address: 20.30.32.32
        Adj-sid: 362146 flags: [L V] weight: 0x0
      IS Neighbor (MT-IPv6): Arista-Spine3-Q2A-30.00 Metric: 10
        Adj-sid: 362147 flags: [L V F] weight: 0x0
      Reachability         : 20.32.175.0/24 Metric: 10 Type: 1 Up
      Reachability         : 20.30.32.0/24 Metric: 10 Type: 1 Up
      Reachability         : 10.0.0.32/32 Metric: 0 Type: 1 Up
        SR Prefix-SID: 32 Flags: [N] Algorithm: 0
      Reachability (MT-IPv6): 2001:0:30:32::/64 Metric: 10 Type: 1 Up
      Router Capabilities: Router Id: 10.0.0.32 Flags: []
        SR Local Block:
          SRLB Base: 965536 Range: 65536
        Area leader priority: 250 algorithm: 0
        Maximum SID depth:
          Base MPLS imposition (MSD type 1):  12
        SR Capability: Flags: [I V]
          SRGB Base: 20000 Range: 2000
    Arrcus-53.00-00              32  37636   739    175 L2  0000.0000.0053.00-00  <>
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
    Ciena-5134-72.00-00          40  33751   956    308 L2  0000.0000.0072.00-00  <>
      Remaining lifetime received: 1199 s Modified to: 1200 s
      NLPID: 0xCC(IPv4)
      Hostname: Ciena-5134-72
      Area addresses: 49.0001
      Topology: 0 (IPv4)
      Interface address: 10.0.0.72
      IS Neighbor          : Arista-Spine3-Q2A-30.00 Metric: 10
        IPv4 Neighbor Address: 20.30.72.30
        IPv4 Interface Address: 20.30.72.72
        Adj-sid: 16000 flags: [L V] weight: 0x0
      IS Neighbor          : Juniper-175-ACX7100-48L.00 Metric: 10
        IPv4 Neighbor Address: 20.72.175.175
        IPv4 Interface Address: 20.72.175.72
        Adj-sid: 16001 flags: [L V] weight: 0x0
      Reachability         : 20.72.175.0/24 Metric: 10 Type: 1 Up
      Reachability         : 20.30.72.0/24 Metric: 10 Type: 1 Up
      Reachability         : 10.0.0.72/32 Metric: 10 Type: 1 Up
        SR Prefix-SID: 72 Flags: [N] Algorithm: 0
      Router Capabilities: Router Id: 10.0.0.72 Flags: []
        SR Capability: Flags: [I]
          SRGB Base: 20000 Range: 2000
        Algorithms:  0
    Ericsson_84_R6678.00-00        35   7833  1054    204 L2  0000.0000.0084.00-00  <>
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
    H3C_M1A_120.00-00            79  41506   845    355 L2  0000.0000.0120.00-00  <>
      Remaining lifetime received: 1199 s Modified to: 1200 s
      NLPID: 0xCC(IPv4) 0x8E(IPv6)
      Hostname: H3C_M1A_120
      Area addresses: 49.0001
      Topology: 0 (IPv4)
      Topology: 2 (IPv6)
      Interface address: 10.0.0.120
      Interface address: 20.30.120.120
      Interface address: 20.120.175.120
      Interface address: 20.120.214.120
      Interface address: 2001:0:30:120::120
      Interface address: 2001:0:120:175::120
      Interface address: 2001:0:120:214::120
      IS Neighbor          : Arista-Spine3-Q2A-30.00 Metric: 10
        IPv4 Neighbor Address: 20.30.120.30
        IPv4 Interface Address: 20.30.120.120
        Adj-sid: 1151 flags: [L V] weight: 0x0
      IS Neighbor          : Juniper-175-ACX7100-48L.00 Metric: 10
        IPv4 Neighbor Address: 20.120.175.175
        IPv4 Interface Address: 20.120.175.120
        Adj-sid: 1150 flags: [L V] weight: 0x0
      IS Neighbor (MT-IPv6): Arista-Spine3-Q2A-30.00 Metric: 10
      Reachability         : 10.0.0.120/32 Metric: 0 Type: 1 Up
        SR Prefix-SID: 120 Flags: [N] Algorithm: 0
      Reachability         : 20.30.120.0/24 Metric: 10 Type: 1 Up
      Reachability         : 20.120.175.0/24 Metric: 10 Type: 1 Up
      Reachability         : 20.120.214.0/24 Metric: 10 Type: 1 Up
      Reachability (MT-IPv6): 2001:0:30:120::/64 Metric: 10 Type: 1 Up
      Reachability (MT-IPv6): 2001:0:120:175::/64 Metric: 10 Type: 1 Up
      Reachability (MT-IPv6): 2001:0:120:214::/64 Metric: 10 Type: 1 Up
      Router Capabilities: Router Id: 10.0.0.120 Flags: []
        Maximum SID depth:
          Base MPLS imposition (MSD type 1):  13
        SR Capability: Flags: [I]
          SRGB Base: 20000 Range: 2000
    0000.0000.0124.00-00         54  20942   961    177 L2  0000.0000.0124.00-00  <>
      Remaining lifetime received: 1199 s Modified to: 1200 s
      NLPID: 0xCC(IPv4) 0x8E(IPv6)
      Area addresses: 49.0001
      Topology: 0 (IPv4)
      Topology: 2 (IPv6)
      Interface address: 10.0.0.124
      Interface address: 20.124.175.124
      Interface address: 20.30.124.124
      IS Neighbor          : Juniper-175-ACX7100-48L.00 Metric: 10
        IPv4 Neighbor Address: 20.124.175.175
        IPv4 Interface Address: 20.124.175.124
        Adj-sid: 273 flags: [L V] weight: 0x0
      IS Neighbor          : Arista-Spine3-Q2A-30.00 Metric: 10
        IPv4 Neighbor Address: 20.30.124.30
        IPv4 Interface Address: 20.30.124.124
        Adj-sid: 274 flags: [L V] weight: 0x0
      Reachability         : 10.0.0.124/32 Metric: 0 Type: 1 Up
        SR Prefix-SID: 124 Flags: [N P] Algorithm: 0
      Reachability         : 20.124.175.0/24 Metric: 10 Type: 1 Up
      Reachability         : 20.30.124.0/24 Metric: 10 Type: 1 Up
      Router Capabilities: Router Id: 10.0.0.124 Flags: []
        Maximum SID depth:
          Base MPLS imposition (MSD type 1):  10
        SR Capability: Flags: [I]
          SRGB Base: 2000 Range: 200
    0000.0000.0128.00-00         32   3590   437    177 L2  0000.0000.0128.00-00  <>
      Remaining lifetime received: 1199 s Modified to: 1200 s
      NLPID: 0xCC(IPv4) 0x8E(IPv6)
      Area addresses: 49.0001
      Topology: 0 (IPv4)
      Topology: 2 (IPv6)
      Interface address: 10.0.0.128
      Interface address: 20.128.175.128
      Interface address: 20.30.128.128
      IS Neighbor          : Juniper-175-ACX7100-48L.00 Metric: 10
        IPv4 Neighbor Address: 20.128.175.175
        IPv4 Interface Address: 20.128.175.128
        Adj-sid: 48002 flags: [L V] weight: 0x0
      IS Neighbor          : Arista-Spine3-Q2A-30.00 Metric: 10
        IPv4 Neighbor Address: 20.30.128.30
        IPv4 Interface Address: 20.30.128.128
        Adj-sid: 48003 flags: [L V] weight: 0x0
      Reachability         : 10.0.0.128/32 Metric: 0 Type: 1 Up
        SR Prefix-SID: 128 Flags: [N] Algorithm: 0
      Reachability         : 20.128.175.0/24 Metric: 10 Type: 1 Up
      Reachability         : 20.30.128.0/24 Metric: 10 Type: 1 Up
      Router Capabilities: Router Id: 10.0.0.128 Flags: []
        Maximum SID depth:
          Base MPLS imposition (MSD type 1):  10
        SR Capability: Flags: [I]
          SRGB Base: 20000 Range: 2000
    Juniper-131-JCNR.00-00        22    426   694    308 L2  0000.0000.0131.00-00  <>
      Remaining lifetime received: 1196 s Modified to: 1200 s
      NLPID: 0xCC(IPv4) 0x8E(IPv6)
      Hostname: Juniper-131-JCNR
      Area addresses: 49.0001
      Interface address: 10.0.0.131
      Interface address: ::af4:0
      IS Neighbor          : Juniper-175-ACX7100-48L.00 Metric: 10
        IPv4 Neighbor Address: 20.131.175.175
        IPv4 Interface Address: 20.131.175.131
        IPv6 Neighbor Address: 2001:0:131:175::175
        Global IPv6 Interface Address: 2001:0:131:175::131
        Adj-sid: 17 flags: [L V F] weight: 0x0
        Adj-sid: 16 flags: [L V] weight: 0x0
      Reachability         : 20.131.175.0/24 Metric: 10 Type: 1 Up
      Reachability         : 10.0.0.131/32 Metric: 0 Type: 1 Up
        SR Prefix-SID: 131 Flags: [N] Algorithm: 0
      Reachability          : 2001:0:131:175::/64 Metric: 10 Type: 1 Up
      Reachability          : fe80::ec97:fbff:fe06:5964/128 Metric: 0 Type: 1 Up
      Router Capabilities: Router Id: 10.0.0.131 Flags: []
        Maximum SID depth:
          Base MPLS imposition (MSD type 1):  0
        SR Capability: Flags: [I V]
          SRGB Base: 20000 Range: 2000
        Algorithms:  0, 1
      Unsupported TLV: Type: 14 Length: 2
    Juniper-175-ACX7100-48L.00-00        94  28277   553   1040 L2  0000.0000.0175.00-00  <>
      Remaining lifetime received: 1198 s Modified to: 1200 s
      NLPID: 0xCC(IPv4) 0x8E(IPv6)
      Hostname: Juniper-175-ACX7100-48L
      Area addresses: 49.0001
      Interface address: 10.0.0.175
      IS Neighbor          : Juniper-131-JCNR.00 Metric: 10
        IPv4 Neighbor Address: 20.131.175.131
        IPv4 Interface Address: 20.131.175.175
        IPv6 Neighbor Address: 2001:0:131:175::131
        Global IPv6 Interface Address: 2001:0:131:175::175
        Adj-sid: 30 flags: [L V F] weight: 0x0
        Adj-sid: 31 flags: [L V] weight: 0x0
      IS Neighbor          : 221.00              Metric: 10
        IPv4 Neighbor Address: 20.175.221.221
        IPv4 Interface Address: 20.175.221.175
        Global IPv6 Interface Address: 2001:0:175:221::175
        Adj-sid: 36 flags: [L V F] weight: 0x0
        Adj-sid: 35 flags: [L V] weight: 0x0
      IS Neighbor          : 0000.0000.0128.00   Metric: 10
        IPv4 Neighbor Address: 20.128.175.128
        IPv4 Interface Address: 20.128.175.175
        Global IPv6 Interface Address: 2001:0:128:175::175
        Adj-sid: 29 flags: [L V] weight: 0x0
      IS Neighbor          : 0000.0000.0124.00   Metric: 10
        IPv4 Neighbor Address: 20.124.175.124
        IPv4 Interface Address: 20.124.175.175
        Adj-sid: 28 flags: [L V] weight: 0x0
      IS Neighbor          : Nokia-SXR-214.00    Metric: 10
        IPv4 Neighbor Address: 20.175.214.214
        IPv4 Interface Address: 20.175.214.175
        Global IPv6 Interface Address: 2001:0:175:214::175
        Adj-sid: 19 flags: [L V F] weight: 0x0
        Adj-sid: 18 flags: [L V] weight: 0x0
      IS Neighbor          : Arista-PE32-Q2C-32.00 Metric: 10
        IPv4 Neighbor Address: 20.32.175.32
        IPv4 Interface Address: 20.32.175.175
        Global IPv6 Interface Address: 2001:0:32:175::175
        Adj-sid: 34 flags: [L V] weight: 0x0
      IS Neighbor          : Ciena-5134-72.00    Metric: 10
        IPv4 Neighbor Address: 20.72.175.72
        IPv4 Interface Address: 20.72.175.175
        Global IPv6 Interface Address: 2001:0:72:175::175
        Adj-sid: 21 flags: [L V] weight: 0x0
      IS Neighbor          : Arista-PE31-Q2C-31.00 Metric: 10
        IPv4 Neighbor Address: 20.31.175.31
        IPv4 Interface Address: 20.31.175.175
        Global IPv6 Interface Address: 2001:0:31:175::175
        Adj-sid: 32 flags: [L V] weight: 0x0
      IS Neighbor          : H3C_M1A_120.00      Metric: 10
        IPv4 Neighbor Address: 20.120.175.120
        IPv4 Interface Address: 20.120.175.175
        IPv6 Neighbor Address: 2001:0:120:175::120
        Global IPv6 Interface Address: 2001:0:120:175::175
        Adj-sid: 27 flags: [L V F] weight: 0x0
        Adj-sid: 26 flags: [L V] weight: 0x0
      IS Neighbor          : Arrcus-53.00        Metric: 10
        IPv4 Neighbor Address: 20.53.175.53
        IPv4 Interface Address: 20.53.175.175
        Global IPv6 Interface Address: 2001:0:53:175::175
        Adj-sid: 20 flags: [L V] weight: 0x0
      Reachability         : 20.131.175.0/24 Metric: 10 Type: 1 Up
      Reachability         : 20.175.221.0/24 Metric: 10 Type: 1 Up
      Reachability         : 20.128.175.0/24 Metric: 10 Type: 1 Up
      Reachability         : 20.175.184.0/24 Metric: 10 Type: 1 Up
      Reachability         : 20.124.175.0/24 Metric: 10 Type: 1 Up
      Reachability         : 20.175.214.0/24 Metric: 10 Type: 1 Up
      Reachability         : 20.32.175.0/24 Metric: 10 Type: 1 Up
      Reachability         : 20.72.175.0/24 Metric: 10 Type: 1 Up
      Reachability         : 20.31.175.0/24 Metric: 10 Type: 1 Up
      Reachability         : 20.120.175.0/24 Metric: 10 Type: 1 Up
      Reachability         : 20.53.175.0/24 Metric: 10 Type: 1 Up
      Reachability         : 10.0.0.175/32 Metric: 0 Type: 1 Up
        SR Prefix-SID: 175 Flags: [N] Algorithm: 0
      Reachability         : 20.175.217.0/24 Metric: 10 Type: 1 Up
      Reachability          : 2001:0:131:175::/64 Metric: 10 Type: 1 Up
      Reachability          : 2001:0:175:221::/64 Metric: 10 Type: 1 Up
      Reachability          : 2001:0:128:175::/64 Metric: 10 Type: 1 Up
      Reachability          : 2001:0:175:184::/64 Metric: 10 Type: 1 Up
      Reachability          : 2001:0:175:214::/64 Metric: 10 Type: 1 Up
      Reachability          : 2001:0:32:175::/64 Metric: 10 Type: 1 Up
      Reachability          : 2001:0:72:175::/64 Metric: 10 Type: 1 Up
      Reachability          : 2001:0:31:175::/64 Metric: 10 Type: 1 Up
      Reachability          : 2001:0:120:175::/64 Metric: 10 Type: 1 Up
      Reachability          : 2001:0:53:175::/64 Metric: 10 Type: 1 Up
      Reachability          : 2001:0:175:217::/64 Metric: 10 Type: 1 Up
      Router Capabilities: Router Id: 10.0.0.175 Flags: []
        SR Capability: Flags: [I V]
          SRGB Base: 20000 Range: 2000
        Algorithms:  0, 1
      Unsupported TLV: Type: 14 Length: 2
    Juniper-175-ACX7100-48L.00-01        29  42631   922    386 L2  0000.0000.0175.00-01  <>
      Remaining lifetime received: 1198 s Modified to: 1200 s
      IS Neighbor          : Nokia-SR1-217.00    Metric: 10
        IPv4 Neighbor Address: 20.175.217.217
        IPv4 Interface Address: 20.175.217.175
        IPv6 Neighbor Address: 2001:0:175:217::217
        Global IPv6 Interface Address: 2001:0:175:217::175
        Adj-sid: 39 flags: [L V F] weight: 0x0
        Adj-sid: 38 flags: [L V] weight: 0x0
      IS Neighbor          : Ericsson_84_R6678.00 Metric: 10
        IPv4 Neighbor Address: 20.84.175.84
        IPv4 Interface Address: 20.84.175.175
        IPv6 Neighbor Address: 2001:0:84:175::175
        Global IPv6 Interface Address: 2001:0:84:175::175
        Adj-sid: 25 flags: [L V F] weight: 0x0
        Adj-sid: 24 flags: [L V] weight: 0x0
      IS Neighbor          : Keysight-184.00     Metric: 10
        IPv4 Neighbor Address: 20.175.184.184
        IPv4 Interface Address: 20.175.184.175
        Global IPv6 Interface Address: 2001:0:175:184::175
        Adj-sid: 40 flags: [L V] weight: 0x0
      IS Neighbor          : Juniper-179-ACX7024.00 Metric: 10
        IPv4 Neighbor Address: 20.175.179.179
        IPv4 Interface Address: 20.175.179.175
        IPv6 Neighbor Address: 2001:0:175::179:179
        Global IPv6 Interface Address: 2001:0:175::179:175
        Adj-sid: 42 flags: [L V F] weight: 0x0
        Adj-sid: 41 flags: [L V] weight: 0x0
      Reachability         : 20.84.175.0/24 Metric: 10 Type: 1 Up
      Reachability         : 20.175.179.0/24 Metric: 10 Type: 1 Up
      Reachability          : 2001:0:84:175::/64 Metric: 10 Type: 1 Up
      Reachability          : 2001:0:175::/64 Metric: 10 Type: 1 Up
    Juniper-179-ACX7024.00-00        37  46252   922    380 L2  0000.0000.0179.00-00  <>
      Remaining lifetime received: 1198 s Modified to: 1200 s
      NLPID: 0xCC(IPv4) 0x8E(IPv6)
      Hostname: Juniper-179-ACX7024
      Area addresses: 49.0001
      Interface address: 10.0.0.179
      Interface address: 2001:0:30:179::179
      IS Neighbor          : Arista-Spine3-Q2A-30.00 Metric: 10
        IPv4 Neighbor Address: 20.30.179.30
        IPv4 Interface Address: 20.30.179.179
        Global IPv6 Interface Address: 2001:0:30:179::179
        Adj-sid: 18 flags: [L V F] weight: 0x0
        Adj-sid: 17 flags: [L V] weight: 0x0
      IS Neighbor          : Juniper-175-ACX7100-48L.00 Metric: 10
        IPv4 Neighbor Address: 20.175.179.175
        IPv4 Interface Address: 20.175.179.179
        IPv6 Neighbor Address: 2001:0:175::179:175
        Global IPv6 Interface Address: 2001:0:175::179:179
        Adj-sid: 20 flags: [L V F] weight: 0x0
        Adj-sid: 19 flags: [L V] weight: 0x0
      Reachability         : 10.0.0.179/32 Metric: 0 Type: 1 Up
        SR Prefix-SID: 179 Flags: [N] Algorithm: 0
      Reachability         : 20.175.179.0/24 Metric: 10 Type: 1 Up
      Reachability         : 20.30.179.0/24 Metric: 10 Type: 1 Up
      Reachability          : 2001:0:175::/64 Metric: 10 Type: 1 Up
      Reachability          : 2001:0:30:179::/64 Metric: 10 Type: 1 Up
      Router Capabilities: Router Id: 10.0.0.179 Flags: []
        Maximum SID depth:
          Base MPLS imposition (MSD type 1):  4
        SR Capability: Flags: [I V]
          SRGB Base: 20000 Range: 2000
        Algorithms:  0, 1
      Unsupported TLV: Type: 14 Length: 2
    Keysight-184.00-00            5  38173   764    132 L2  0000.0000.0184.00-00  <DefaultAtt>
      Remaining lifetime received: 1193 s Modified to: 1200 s
      NLPID: 0xCC(IPv4) 0x8E(IPv6) 0x81(CLNP)
      Hostname: Keysight-184
      Area addresses: 49.0001
      Interface address: 20.175.184.184
      IS Neighbor          : Juniper-175-ACX7100-48L.00 Metric: 10
        Adj-sid: 9001 flags: [L V] weight: 0x0
      Reachability         : 10.0.0.184/32 Metric: 10 Type: 1 Up
        SR Prefix-SID: 484 Flags: [N] Algorithm: 0
      Reachability         : 20.175.184.0/24 Metric: 10 Type: 1 Up
      Router Capabilities: Router Id: 10.0.0.184 Flags: []
        SR Capability: Flags: [I V]
          SRGB Base: 20000 Range: 2000
        Algorithms:  0
    Nokia-SXR-214.00-00        1696  18508  1175    357 L2  0000.0000.0214.00-00  <>
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
      IS Neighbor          : Juniper-175-ACX7100-48L.00 Metric: 10
        IPv4 Neighbor Address: 20.175.214.175
        IPv4 Interface Address: 20.175.214.214
        Adj-sid: 30001 flags: [L V B] weight: 0x0
        Adj-sid: 30002 flags: [L V B F] weight: 0x0
      IS Neighbor          : Nokia-IXRe2-216.00  Metric: 10
        IPv4 Neighbor Address: 20.214.216.216
        IPv4 Interface Address: 20.214.216.214
        Adj-sid: 30003 flags: [L V B] weight: 0x0
      IS Neighbor          : Arista-Spine3-Q2A-30.00 Metric: 10
        IPv4 Neighbor Address: 20.30.214.30
        IPv4 Interface Address: 20.30.214.214
        Adj-sid: 30004 flags: [L V B] weight: 0x0
        Adj-sid: 30005 flags: [L V B F] weight: 0x0
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
    Nokia-IXRe2-216.00-00        26  18954  1133    120 L2  0100.0000.0216.00-00  <>
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
    Nokia-SR1-217.00-00          16  54205   650    349 L2  0100.0000.0217.00-00  <>
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
        Adj-sid: 524285 flags: [L V] weight: 0x0
        Adj-sid: 524284 flags: [L V F] weight: 0x0
      IS Neighbor          : Juniper-175-ACX7100-48L.00 Metric: 10
        IPv4 Neighbor Address: 20.175.217.175
        IPv4 Interface Address: 20.175.217.217
        IPv6 Neighbor Address: 2001:0:175:217::175
        Global IPv6 Interface Address: 2001:0:175:217::217
        Adj-sid: 524286 flags: [L V] weight: 0x0
        Adj-sid: 524283 flags: [L V F] weight: 0x0
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
    221.00-00                    18  54428  1012     80 L2  0221.0221.0221.00-00  <>
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
    221.00-01                    18  48034   901     32 L2  0221.0221.0221.00-01  <>
      Hostname: 221
    221.00-02                    33  35934   542    273 L2  0221.0221.0221.00-02  <>
      Interface address: 10.0.0.221
      Interface address: 20.175.221.221
      Interface address: 20.30.221.221
      Interface address: 1221::1
      Interface address: 2001:0:175:221::221
      Interface address: 2001:0:30:221::221
      IS Neighbor          : Juniper-175-ACX7100-48L.00 Metric: 10
        IPv4 Neighbor Address: 20.175.221.175
        IPv4 Interface Address: 20.175.221.221
        Adj-sid: 524291 flags: [L V B] weight: 0x0
        Adj-sid: 524290 flags: [L V] weight: 0x0
      IS Neighbor          : Arista-Spine3-Q2A-30.00 Metric: 10
        IPv4 Neighbor Address: 20.30.221.30
        IPv4 Interface Address: 20.30.221.221
        Adj-sid: 524293 flags: [L V B] weight: 0x0
        Adj-sid: 524292 flags: [L V] weight: 0x0
      Reachability         : 10.0.0.221/32 Metric: 0 Type: 1 Up
        SR Prefix-SID: 1221 Flags: [N] Algorithm: 0
      Reachability         : 20.175.221.0/24 Metric: 10 Type: 1 Up
      Reachability         : 20.30.221.0/24 Metric: 10 Type: 1 Up
      Reachability          : 1221::1/128 Metric: 0 Type: 1 Up
      Reachability          : 2001:0:175:221::/64 Metric: 10 Type: 1 Up
      Reachability          : 2001:0:30:221::/64 Metric: 10 Type: 1 Up

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
  1         10.0.0.84/32      TI-LFA (0)                -             [ 20084 ]
  2         10.0.0.72/32      TI-LFA (8)                -             [ 3 ]    
  4         10.0.0.175/32     20.30.31.31               Ethernet1     [ 20175 ]
                              20.30.32.32               Ethernet2     [ 20175 ]
                              20.30.53.53               Ethernet13    [ 20175 ]
                              20.30.72.72               Ethernet9     [ 20175 ]
                              20.30.84.84               Ethernet12    [ 20175 ]
                              20.30.120.120             Ethernet3     [ 20175 ]
                              20.30.124.124             Ethernet17    [ 2175 ] 
                              20.30.128.128             Ethernet19    [ 20175 ]
  5         10.0.0.53/32      TI-LFA (2)                -             [ 3 ]    
  6         10.0.0.179/32     TI-LFA (6)                -             [ 3 ]    
  7         10.0.0.120/32     TI-LFA (5)                -             [ 3 ]    
  8         10.0.0.31/32      TI-LFA (1)                -             [ 3 ]    
  9         10.0.0.32/32      TI-LFA (12)               -             [ 3 ]    
  10        10.0.0.214/32     TI-LFA (3)                -             [ 20214 ]
  11        10.0.0.128/32     TI-LFA (7)                -             [ 3 ]    
  12        10.0.0.131/32     20.30.31.31               Ethernet1     [ 20131 ]
                              20.30.32.32               Ethernet2     [ 20131 ]
                              20.30.53.53               Ethernet13    [ 20131 ]
                              20.30.72.72               Ethernet9     [ 20131 ]
                              20.30.84.84               Ethernet12    [ 20131 ]
                              20.30.120.120             Ethernet3     [ 20131 ]
                              20.30.124.124             Ethernet17    [ 2131 ] 
                              20.30.128.128             Ethernet19    [ 20131 ]
  13        10.0.0.221/32     TI-LFA (9)                -             [ 3 ]    
  14        10.0.0.124/32     TI-LFA (11)               -             [ 3 ]    
  15        10.0.0.184/32     20.30.31.31               Ethernet1     [ 20484 ]
                              20.30.32.32               Ethernet2     [ 20484 ]
                              20.30.53.53               Ethernet13    [ 20484 ]
                              20.30.72.72               Ethernet9     [ 20484 ]
                              20.30.84.84               Ethernet12    [ 20484 ]
                              20.30.120.120             Ethernet3     [ 20484 ]
                              20.30.128.128             Ethernet19    [ 20484 ]
  16        10.0.0.217/32     TI-LFA (4)                -             [ 20217 ]

```

## show isis segment-routing prefix-segments

```text

System ID: Arista-Spine3-Q2A-30			Instance: 'IGP'
SR supported Data-plane: MPLS			SR Router ID: 10.0.0.30

Node: 16     Proxy-Node: 0      Prefix: 0       Total Segments: 16

Flag Descriptions: R: Re-advertised, N: Node Segment, P: no-PHP
                   E: Explicit-NULL, V: Value, L: Local
Segment status codes: * - Self originated Prefix, L1 - level 1, L2 - level 2, ! - SR-unreachable,
                      # - Some IS-IS next-hops are SR-unreachable
   Prefix                      SID   Label Type       Flags                        System ID       Level Protection  Algorithm   
   ------------------------- ----- ------- ---------- ---------------------------- --------------- ----- ----------- -------------
*  10.0.0.30/32                 30   20030 Node       R:0 N:1 P:0 E:0 V:0 L:0      Arista-Spine3-Q2A-30 L2    unprotected SPF         
   10.0.0.31/32                 31   20031 Node       R:0 N:1 P:0 E:0 V:0 L:0      Arista-PE31-Q2C-31 L2    node        SPF         
   10.0.0.32/32                 32   20032 Node       R:0 N:1 P:0 E:0 V:0 L:0      Arista-PE32-Q2C-32 L2    node        SPF         
   10.0.0.53/32                 53   20053 Node       R:0 N:1 P:1 E:1 V:0 L:0      Arrcus-53       L2    node        SPF         
   10.0.0.72/32                 72   20072 Node       R:0 N:1 P:0 E:0 V:0 L:0      Ciena-5134-72   L2    node        SPF         
   10.0.0.84/32                 84   20084 Node       R:0 N:1 P:1 E:0 V:0 L:0      Ericsson_84_R6678 L2    node        SPF         
   10.0.0.120/32               120   20120 Node       R:0 N:1 P:0 E:0 V:0 L:0      H3C_M1A_120     L2    node        SPF         
   10.0.0.124/32               124    2124 Node       R:0 N:1 P:1 E:0 V:0 L:0      0000.0000.0124  L2    node        SPF         
   10.0.0.128/32               128   20128 Node       R:0 N:1 P:0 E:0 V:0 L:0      0000.0000.0128  L2    node        SPF         
   10.0.0.131/32               131   20131 Node       R:0 N:1 P:0 E:0 V:0 L:0      Juniper-131-JCNR L2    unprotected SPF         
   10.0.0.175/32               175   20175 Node       R:0 N:1 P:0 E:0 V:0 L:0      Juniper-175-ACX7100-48L L2    unprotected SPF         
   10.0.0.179/32               179   20179 Node       R:0 N:1 P:0 E:0 V:0 L:0      Juniper-179-ACX7024 L2    node        SPF         
   10.0.0.184/32               484   20484 Node       R:0 N:1 P:0 E:0 V:0 L:0      Keysight-184    L2    unprotected SPF         
   10.0.0.214/32               214   20214 Node       R:0 N:1 P:1 E:0 V:0 L:0      Nokia-SXR-214   L2    node        SPF         
   10.0.0.217/32               217   20217 Node       R:0 N:1 P:1 E:0 V:0 L:0      Nokia-SR1-217   L2    node        SPF         
   10.0.0.221/32              1221  721221 Node       R:0 N:1 P:0 E:0 V:0 L:0      221             L2    node        SPF         
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
 I L2     10.0.0.31/32 [115/10]
           via 20.30.31.31, Ethernet1
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
 I L2     10.0.0.124/32 [115/10]
           via 20.30.124.124, Ethernet17
 I L2     10.0.0.128/32 [115/10]
           via 20.30.128.128, Ethernet19
 I L2     10.0.0.131/32 [115/30]
           via 20.30.31.31, Ethernet1
           via 20.30.32.32, Ethernet2
           via 20.30.120.120, Ethernet3
           via 20.30.72.72, Ethernet9
           via 20.30.84.84, Ethernet12
           via 20.30.53.53, Ethernet13
           via 20.30.124.124, Ethernet17
           via 20.30.128.128, Ethernet19
 I L2     10.0.0.175/32 [115/20]
           via 20.30.31.31, Ethernet1
           via 20.30.32.32, Ethernet2
           via 20.30.120.120, Ethernet3
           via 20.30.72.72, Ethernet9
           via 20.30.84.84, Ethernet12
           via 20.30.53.53, Ethernet13
           via 20.30.124.124, Ethernet17
           via 20.30.128.128, Ethernet19
 I L2     10.0.0.179/32 [115/10]
           via 20.30.179.179, Ethernet40
 I L2     10.0.0.184/32 [115/40]
           via 20.30.31.31, Ethernet1
           via 20.30.32.32, Ethernet2
           via 20.30.120.120, Ethernet3
           via 20.30.72.72, Ethernet9
           via 20.30.84.84, Ethernet12
           via 20.30.53.53, Ethernet13
           via 20.30.124.124, Ethernet17
           via 20.30.128.128, Ethernet19
 I L2     10.0.0.214/32 [115/10]
           via 20.30.214.214, Ethernet5
 I L2     10.0.0.216/32 [115/20]
           via 20.30.214.214, Ethernet5
 I L2     10.0.0.217/32 [115/10]
           via 20.30.217.217, Ethernet4
 I L2     10.0.0.221/32 [115/10]
           via 20.30.221.221, Ethernet15
 C        20.30.31.0/24
           directly connected, Ethernet1
 C        20.30.32.0/24
           directly connected, Ethernet2
 C        20.30.53.0/24
           directly connected, Ethernet13
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
 I L2     20.31.175.0/24 [115/20]
           via 20.30.31.31, Ethernet1
 I L2     20.32.175.0/24 [115/20]
           via 20.30.32.32, Ethernet2
 I L2     20.53.175.0/24 [115/20]
           via 20.30.53.53, Ethernet13
 I L2     20.72.175.0/24 [115/20]
           via 20.30.72.72, Ethernet9
 I L2     20.84.175.0/24 [115/30]
           via 20.30.31.31, Ethernet1
           via 20.30.32.32, Ethernet2
           via 20.30.120.120, Ethernet3
           via 20.30.72.72, Ethernet9
           via 20.30.84.84, Ethernet12
           via 20.30.53.53, Ethernet13
           via 20.30.124.124, Ethernet17
           via 20.30.128.128, Ethernet19
 I L2     20.120.175.0/24 [115/20]
           via 20.30.120.120, Ethernet3
 I L2     20.120.214.0/24 [115/20]
           via 20.30.120.120, Ethernet3
 I L2     20.124.175.0/24 [115/20]
           via 20.30.124.124, Ethernet17
 I L2     20.128.175.0/24 [115/20]
           via 20.30.128.128, Ethernet19
 I L2     20.131.175.0/24 [115/30]
           via 20.30.31.31, Ethernet1
           via 20.30.32.32, Ethernet2
           via 20.30.120.120, Ethernet3
           via 20.30.72.72, Ethernet9
           via 20.30.84.84, Ethernet12
           via 20.30.53.53, Ethernet13
           via 20.30.124.124, Ethernet17
           via 20.30.128.128, Ethernet19
 I L2     20.175.179.0/24 [115/20]
           via 20.30.179.179, Ethernet40
 I L2     20.175.184.0/24 [115/30]
           via 20.30.31.31, Ethernet1
           via 20.30.32.32, Ethernet2
           via 20.30.120.120, Ethernet3
           via 20.30.72.72, Ethernet9
           via 20.30.84.84, Ethernet12
           via 20.30.53.53, Ethernet13
           via 20.30.124.124, Ethernet17
           via 20.30.128.128, Ethernet19
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
 B I      50.10.31.0/24 [200/0]
           via 10.0.0.31/32, IS-IS SR tunnel index 8, label 362145
              via TI-LFA tunnel index 1, label imp-null(3)
                 via 20.30.31.31, Ethernet1, label imp-null(3)
                 backup via 20.30.72.72, Ethernet9, label 20175 20031
 B I      50.10.32.0/24 [200/0]
           via 10.0.0.32/32, IS-IS SR tunnel index 9, label 378528
              via TI-LFA tunnel index 12, label imp-null(3)
                 via 20.30.32.32, Ethernet2, label imp-null(3)
                 backup via 20.30.221.221, Ethernet15, label 720175 20032
 B I      50.10.53.0/24 [200/0]
           via 10.0.0.53/32, IS-IS SR tunnel index 5, label 970000
              via TI-LFA tunnel index 2, label imp-null(3)
                 via 20.30.53.53, Ethernet13, label exp-null-v4(0)
                 backup via 20.30.72.72, Ethernet9, label 20175 20053
 B I      50.10.72.0/24 [200/0]
           via 10.0.0.72/32, IS-IS SR tunnel index 2, label 62002
              via TI-LFA tunnel index 8, label imp-null(3)
                 via 20.30.72.72, Ethernet9, label imp-null(3)
                 backup via 20.30.53.53, Ethernet13, label 20175 20072
 B I      50.10.84.0/24 [200/0]
           via 10.0.0.84/32, IS-IS SR tunnel index 1, label 720896
              via TI-LFA tunnel index 0, label 20084
                 via 20.30.84.84, Ethernet12, label imp-null(3)
                 backup via 20.30.128.128, Ethernet19, label 20175
 B I      50.10.120.0/24 [200/0]
           via 10.0.0.120/32, IS-IS SR tunnel index 7, label 1277
              via TI-LFA tunnel index 5, label imp-null(3)
                 via 20.30.120.120, Ethernet3, label imp-null(3)
                 backup via 20.30.214.214, Ethernet5, label 20175 20120
 B I      50.10.131.0/24 [200/0]
           via 10.0.0.131/32, IS-IS SR tunnel index 12, label 18
              via 20.30.31.31, Ethernet1, label 20131
              via 20.30.32.32, Ethernet2, label 20131
              via 20.30.53.53, Ethernet13, label 20131
              via 20.30.72.72, Ethernet9, label 20131
              via 20.30.84.84, Ethernet12, label 20131
              via 20.30.120.120, Ethernet3, label 20131
              via 20.30.124.124, Ethernet17, label 2131
              via 20.30.128.128, Ethernet19, label 20131
 B I      50.10.179.0/24 [200/0]
           via 10.0.0.179/32, IS-IS SR tunnel index 6, label 16
              via TI-LFA tunnel index 6, label imp-null(3)
                 via 20.30.179.179, Ethernet40, label imp-null(3)
                 backup via 20.30.124.124, Ethernet17, label 2175 20179
 B I      50.10.214.0/24 [200/0]
           via 10.0.0.214/32, IS-IS SR tunnel index 10, label 500000
              via TI-LFA tunnel index 3, label 20214
                 via 20.30.214.214, Ethernet5, label imp-null(3)
                 backup via 20.30.72.72, Ethernet9, label 20175
 B I      50.10.217.0/24 [200/0]
           via 10.0.0.217/32, IS-IS SR tunnel index 16, label 524287
              via TI-LFA tunnel index 4, label 20217
                 via 20.30.217.217, Ethernet4, label imp-null(3)
                 backup via 20.30.124.124, Ethernet17, label 2175
 B I      50.10.221.0/24 [200/0]
           via 10.0.0.221/32, IS-IS SR tunnel index 13, label 524289
              via TI-LFA tunnel index 9, label imp-null(3)
                 via 20.30.221.221, Ethernet15, label imp-null(3)
                 backup via 20.30.53.53, Ethernet13, label 20175 21221

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

 C        2001:0:30:31::/64 [0/0]
           via Ethernet1, directly connected
 C        2001:0:30:32::/64 [0/0]
           via Ethernet2, directly connected
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
 C        2001:0:53:120::/64 [0/0]
           via Ethernet13, directly connected
 I L2     2001:0:120:175::/64 [115/20]
           via fe80::be31:e2ff:fee1:ec2c, Ethernet3
 I L2     2001:0:120:214::/64 [115/20]
           via fe80::be31:e2ff:fee1:ec2c, Ethernet3

```

## show ipv6 route vrf RED

```text

VRF: RED
Displaying 11 of 14 IPv6 routing table entries
Source Codes:
       C - connected, S - static, K - kernel, O3 - OSPFv3,
       B - Other BGP Routes, A B - BGP Aggregate, R - RIP,
       I L1 - IS-IS level 1, I L2 - IS-IS level 2, DH - DHCP,
       NG - Nexthop Group Static Route, M - Martian,
       DP - Dynamic Policy Route, L - VRF Leaked,
       G  - gRIBI, RC - Route Cache Route,
       CL - CBF Leaked Route

 B I      2600:50:10:31::/64 [200/0]
           via 10.0.0.31/32, IS-IS SR tunnel index 8, label 362144
              via TI-LFA tunnel index 1, label imp-null(3)
                 via 20.30.31.31, Ethernet1, label imp-null(3)
                 backup via 20.30.72.72, Ethernet9, label 20175 20031
 B I      2600:50:10:32::/64 [200/0]
           via 10.0.0.32/32, IS-IS SR tunnel index 9, label 378529
              via TI-LFA tunnel index 12, label imp-null(3)
                 via 20.30.32.32, Ethernet2, label imp-null(3)
                 backup via 20.30.221.221, Ethernet15, label 720175 20032
 B I      2600:50:10:53::/64 [200/0]
           via 10.0.0.53/32, IS-IS SR tunnel index 5, label 970001
              via TI-LFA tunnel index 2, label imp-null(3)
                 via 20.30.53.53, Ethernet13, label exp-null-v4(0)
                 backup via 20.30.72.72, Ethernet9, label 20175 20053
 B I      2600:50:10:72::/64 [200/0]
           via 10.0.0.72/32, IS-IS SR tunnel index 2, label 62003
              via TI-LFA tunnel index 8, label imp-null(3)
                 via 20.30.72.72, Ethernet9, label imp-null(3)
                 backup via 20.30.53.53, Ethernet13, label 20175 20072
 B I      2600:50:10:84::/64 [200/0]
           via 10.0.0.84/32, IS-IS SR tunnel index 1, label 720897
              via TI-LFA tunnel index 0, label 20084
                 via 20.30.84.84, Ethernet12, label imp-null(3)
                 backup via 20.30.128.128, Ethernet19, label 20175
 B I      2600:50:10:120::/64 [200/0]
           via 10.0.0.120/32, IS-IS SR tunnel index 7, label 1276
              via TI-LFA tunnel index 5, label imp-null(3)
                 via 20.30.120.120, Ethernet3, label imp-null(3)
                 backup via 20.30.214.214, Ethernet5, label 20175 20120
 B I      2600:50:10:131::/64 [200/0]
           via 10.0.0.131/32, IS-IS SR tunnel index 12, label 18
              via 20.30.31.31, Ethernet1, label 20131
              via 20.30.32.32, Ethernet2, label 20131
              via 20.30.53.53, Ethernet13, label 20131
              via 20.30.72.72, Ethernet9, label 20131
              via 20.30.84.84, Ethernet12, label 20131
              via 20.30.120.120, Ethernet3, label 20131
              via 20.30.124.124, Ethernet17, label 2131
              via 20.30.128.128, Ethernet19, label 20131
 B I      2600:50:10:179::/64 [200/0]
           via 10.0.0.179/32, IS-IS SR tunnel index 6, label 16
              via TI-LFA tunnel index 6, label imp-null(3)
                 via 20.30.179.179, Ethernet40, label imp-null(3)
                 backup via 20.30.124.124, Ethernet17, label 2175 20179
 B I      2600:50:10:214::/64 [200/0]
           via 10.0.0.214/32, IS-IS SR tunnel index 10, label 500000
              via TI-LFA tunnel index 3, label 20214
                 via 20.30.214.214, Ethernet5, label imp-null(3)
                 backup via 20.30.72.72, Ethernet9, label 20175
 B I      2600:50:10:217::/64 [200/0]
           via 10.0.0.217/32, IS-IS SR tunnel index 16, label 524287
              via TI-LFA tunnel index 4, label 20217
                 via 20.30.217.217, Ethernet4, label imp-null(3)
                 backup via 20.30.124.124, Ethernet17, label 2175
 B I      2600:50:10:221::/64 [200/0]
           via 10.0.0.221/32, IS-IS SR tunnel index 13, label 524289
              via TI-LFA tunnel index 9, label imp-null(3)
                 via 20.30.221.221, Ethernet15, label imp-null(3)
                 backup via 20.30.53.53, Ethernet13, label 20175 21221

! IPv6 routing not enabled
```

## show mpls route

```text
MPLS forwarding table (Label [metric] Vias) - 31 routes 
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

 20031   A[1]
                via M, ::, pop
                    EgressACL: apply
                  via TI-LFA tunnel index 1
                    via 20.30.31.31, Ethernet1, label imp-null(3)
                    backup via 20.30.72.72, Ethernet9, label 20175 20031
 20032   A[1]
                via M, ::, pop
                    EgressACL: apply
                  via TI-LFA tunnel index 12
                    via 20.30.32.32, Ethernet2, label imp-null(3)
                    backup via 20.30.221.221, Ethernet15, label 720175 20032
 20053   A[1]
                via M, ::, pop
                    EgressACL: apply
                  via TI-LFA tunnel index 2
                    via 20.30.53.53, Ethernet13, label exp-null-v4(0)
                    backup via 20.30.72.72, Ethernet9, label 20175 20053
 20072   A[1]
                via M, ::, pop
                    EgressACL: apply
                  via TI-LFA tunnel index 8
                    via 20.30.72.72, Ethernet9, label imp-null(3)
                    backup via 20.30.53.53, Ethernet13, label 20175 20072
 20084   A[1]
                via M, ::, forward
                    EgressACL: apply
                  via TI-LFA tunnel index 0
                    via 20.30.84.84, Ethernet12, label imp-null(3)
                    backup via 20.30.128.128, Ethernet19, label 20175
 20120   A[1]
                via M, ::, pop
                    EgressACL: apply
                  via TI-LFA tunnel index 5
                    via 20.30.120.120, Ethernet3, label imp-null(3)
                    backup via 20.30.214.214, Ethernet5, label 20175 20120
 20124   A[1]
                via M, ::, pop
                    EgressACL: apply
                  via TI-LFA tunnel index 11
                    via 20.30.124.124, Ethernet17, label 2124
                    backup via 20.30.53.53, Ethernet13, label 20175 20124
 20128   A[1]
                via M, ::, pop
                    EgressACL: apply
                  via TI-LFA tunnel index 7
                    via 20.30.128.128, Ethernet19, label imp-null(3)
                    backup via 20.30.120.120, Ethernet3, label 20175 20128
 20131   A[1]
                via M, 20.30.31.31, swap 20131
                    EgressACL: apply
                    directly connected, Ethernet1
                    68:bf:6c:35:1e:31, vlan 1007
                via M, 20.30.32.32, swap 20131
                    EgressACL: apply
                    directly connected, Ethernet2
                    d4:af:f7:2f:13:96, vlan 1014
                via M, 20.30.53.53, swap 20131
                    EgressACL: apply
                    directly connected, Ethernet13
                    5c:07:58:a3:0a:aa, vlan 1010
                via M, 20.30.72.72, swap 20131
                    EgressACL: apply
                    directly connected, Ethernet9
                    e0:9b:27:c4:c5:84, vlan 1009
                via M, 20.30.84.84, swap 20131
                    EgressACL: apply
                    directly connected, Ethernet12
                    58:70:7f:9f:c4:03, vlan 1011
                via M, 20.30.120.120, swap 20131
                    EgressACL: apply
                    directly connected, Ethernet3
                    bc:31:e2:e1:ec:2c, vlan 1008
                via M, 20.30.124.124, swap 2131
                    EgressACL: apply
                    directly connected, Ethernet17
                    64:6d:4e:32:e1:22, vlan 1012
                via M, 20.30.128.128, swap 20131
                    EgressACL: apply
                    directly connected, Ethernet19
                    60:53:75:13:ba:d8, vlan 1016
 20175   A[1]
                via M, 20.30.31.31, swap 20175
                    EgressACL: apply
                    directly connected, Ethernet1
                    68:bf:6c:35:1e:31, vlan 1007
                via M, 20.30.32.32, swap 20175
                    EgressACL: apply
                    directly connected, Ethernet2
                    d4:af:f7:2f:13:96, vlan 1014
                via M, 20.30.53.53, swap 20175
                    EgressACL: apply
                    directly connected, Ethernet13
                    5c:07:58:a3:0a:aa, vlan 1010
                via M, 20.30.72.72, swap 20175
                    EgressACL: apply
                    directly connected, Ethernet9
                    e0:9b:27:c4:c5:84, vlan 1009
                via M, 20.30.84.84, swap 20175
                    EgressACL: apply
                    directly connected, Ethernet12
                    58:70:7f:9f:c4:03, vlan 1011
                via M, 20.30.120.120, swap 20175
                    EgressACL: apply
                    directly connected, Ethernet3
                    bc:31:e2:e1:ec:2c, vlan 1008
                via M, 20.30.124.124, swap 2175
                    EgressACL: apply
                    directly connected, Ethernet17
                    64:6d:4e:32:e1:22, vlan 1012
                via M, 20.30.128.128, swap 20175
                    EgressACL: apply
                    directly connected, Ethernet19
                    60:53:75:13:ba:d8, vlan 1016
 20179   A[1]
                via M, ::, pop
                    EgressACL: apply
                  via TI-LFA tunnel index 6
                    via 20.30.179.179, Ethernet40, label imp-null(3)
                    backup via 20.30.124.124, Ethernet17, label 2175 20179
 20214   A[1]
                via M, ::, forward
                    EgressACL: apply
                  via TI-LFA tunnel index 3
                    via 20.30.214.214, Ethernet5, label imp-null(3)
                    backup via 20.30.72.72, Ethernet9, label 20175
 20217   A[1]
                via M, ::, forward
                    EgressACL: apply
                  via TI-LFA tunnel index 4
                    via 20.30.217.217, Ethernet4, label imp-null(3)
                    backup via 20.30.124.124, Ethernet17, label 2175
 20484   A[1]
                via M, 20.30.31.31, swap 20484
                    EgressACL: apply
                    directly connected, Ethernet1
                    68:bf:6c:35:1e:31, vlan 1007
                via M, 20.30.32.32, swap 20484
                    EgressACL: apply
                    directly connected, Ethernet2
                    d4:af:f7:2f:13:96, vlan 1014
                via M, 20.30.53.53, swap 20484
                    EgressACL: apply
                    directly connected, Ethernet13
                    5c:07:58:a3:0a:aa, vlan 1010
                via M, 20.30.72.72, swap 20484
                    EgressACL: apply
                    directly connected, Ethernet9
                    e0:9b:27:c4:c5:84, vlan 1009
                via M, 20.30.84.84, swap 20484
                    EgressACL: apply
                    directly connected, Ethernet12
                    58:70:7f:9f:c4:03, vlan 1011
                via M, 20.30.120.120, swap 20484
                    EgressACL: apply
                    directly connected, Ethernet3
                    bc:31:e2:e1:ec:2c, vlan 1008
                via M, 20.30.128.128, swap 20484
                    EgressACL: apply
                    directly connected, Ethernet19
                    60:53:75:13:ba:d8, vlan 1016
 21221   A[1]
                via M, ::, pop
                    EgressACL: apply
                  via TI-LFA tunnel index 9
                    via 20.30.221.221, Ethernet15, label imp-null(3)
                    backup via 20.30.53.53, Ethernet13, label 20175 21221
 362159  A[1]
                via M, 20.30.32.32, pop
                    EgressACL: apply
                    directly connected, Ethernet2
                    d4:af:f7:2f:13:96, vlan 1014
 362160  A[1]
                via M, 20.30.221.221, pop
                    EgressACL: apply
                    directly connected, Ethernet15
                    30:c5:07:84:3e:79, vlan 1015
 362161  A[1]
                via M, 20.30.72.72, pop
                    EgressACL: apply
                    directly connected, Ethernet9
                    e0:9b:27:c4:c5:84, vlan 1009
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
 362164  A[1]
                via M, 20.30.31.31, pop
                    EgressACL: apply
                    directly connected, Ethernet1
                    68:bf:6c:35:1e:31, vlan 1007
 362165  A[1]
                via M, 20.30.53.53, pop
                    EgressACL: apply
                    directly connected, Ethernet13
                    5c:07:58:a3:0a:aa, vlan 1010
 362166  A[1]
                via M, 20.30.214.214, pop
                    EgressACL: apply
                    directly connected, Ethernet5
                    18:5b:00:61:ac:6f, vlan 1006
 362167  A[1]
                via M, 20.30.84.84, pop
                    EgressACL: apply
                    directly connected, Ethernet12
                    58:70:7f:9f:c4:03, vlan 1011
 362168  A[1]
                via M, 20.30.179.179, pop
                    EgressACL: apply
                    directly connected, Ethernet40
                    e8:24:a6:96:05:48, vlan 1013
 362169  A[1]
                via M, fe80::d6af:f7ff:fe2f:1396, pop
                    EgressACL: apply
                    directly connected, Ethernet2
                    d4:af:f7:2f:13:96, vlan 1014
 362170  A[1]
                via M, fe80::6abf:6cff:fe35:1e31, pop
                    EgressACL: apply
                    directly connected, Ethernet1
                    68:bf:6c:35:1e:31, vlan 1007
 362171  A[1]
                via M, 20.30.217.217, pop
                    EgressACL: apply
                    directly connected, Ethernet4
                    c0:14:b8:21:97:90, vlan 1018
 362174  A[1]
                via M, 20.30.128.128, pop
                    EgressACL: apply
                    directly connected, Ethernet19
                    60:53:75:13:ba:d8, vlan 1016
 362175  A[1]
                via M, 20.30.124.124, pop
                    EgressACL: apply
                    directly connected, Ethernet17
                    64:6d:4e:32:e1:22, vlan 1012
 378528   [0]
                via I, ipv4, vrf RED
```

## show mpls lfib route

```text
MPLS forwarding table (Label [metric] Vias) - 31 routes 
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

 IP    20031    [1], 10.0.0.31/32
                via TI-LFA tunnel index 1, pop
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                    via 20.30.31.31, Ethernet1, label imp-null(3)
                    backup via 20.30.72.72, Ethernet9, label 20175 20031
 IP    20032    [1], 10.0.0.32/32
                via TI-LFA tunnel index 12, pop
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                    via 20.30.32.32, Ethernet2, label imp-null(3)
                    backup via 20.30.221.221, Ethernet15, label 720175 20032
 IP    20053    [1], 10.0.0.53/32
                via TI-LFA tunnel index 2, pop
                 payload autoDecide, ttlMode uniform, apply egress-acl
                    via 20.30.53.53, Ethernet13, label exp-null-v4(0)
                    backup via 20.30.72.72, Ethernet9, label 20175 20053
 IP    20072    [1], 10.0.0.72/32
                via TI-LFA tunnel index 8, pop
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                    via 20.30.72.72, Ethernet9, label imp-null(3)
                    backup via 20.30.53.53, Ethernet13, label 20175 20072
 IP    20084    [1], 10.0.0.84/32
                via TI-LFA tunnel index 0, forward
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                    via 20.30.84.84, Ethernet12, label imp-null(3)
                    backup via 20.30.128.128, Ethernet19, label 20175
 IP    20120    [1], 10.0.0.120/32
                via TI-LFA tunnel index 5, pop
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                    via 20.30.120.120, Ethernet3, label imp-null(3)
                    backup via 20.30.214.214, Ethernet5, label 20175 20120
 IP    20124    [1], 10.0.0.124/32
                via TI-LFA tunnel index 11, pop
                 payload autoDecide, ttlMode uniform, apply egress-acl
                    via 20.30.124.124, Ethernet17, label 2124
                    backup via 20.30.53.53, Ethernet13, label 20175 20124
 IP    20128    [1], 10.0.0.128/32
                via TI-LFA tunnel index 7, pop
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                    via 20.30.128.128, Ethernet19, label imp-null(3)
                    backup via 20.30.120.120, Ethernet3, label 20175 20128
 IP    20131    [1], 10.0.0.131/32
                via M, 20.30.31.31, swap 20131
                 payload autoDecide, ttlMode uniform, apply egress-acl
                 interface Ethernet1
                via M, 20.30.32.32, swap 20131
                 payload autoDecide, ttlMode uniform, apply egress-acl
                 interface Ethernet2
                via M, 20.30.53.53, swap 20131
                 payload autoDecide, ttlMode uniform, apply egress-acl
                 interface Ethernet13
                via M, 20.30.72.72, swap 20131
                 payload autoDecide, ttlMode uniform, apply egress-acl
                 interface Ethernet9
                via M, 20.30.84.84, swap 20131
                 payload autoDecide, ttlMode uniform, apply egress-acl
                 interface Ethernet12
                via M, 20.30.120.120, swap 20131
                 payload autoDecide, ttlMode uniform, apply egress-acl
                 interface Ethernet3
                via M, 20.30.124.124, swap 2131
                 payload autoDecide, ttlMode uniform, apply egress-acl
                 interface Ethernet17
                via M, 20.30.128.128, swap 20131
                 payload autoDecide, ttlMode uniform, apply egress-acl
                 interface Ethernet19
 IP    20175    [1], 10.0.0.175/32
                via M, 20.30.31.31, swap 20175
                 payload autoDecide, ttlMode uniform, apply egress-acl
                 interface Ethernet1
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
                via M, 20.30.120.120, swap 20175
                 payload autoDecide, ttlMode uniform, apply egress-acl
                 interface Ethernet3
                via M, 20.30.124.124, swap 2175
                 payload autoDecide, ttlMode uniform, apply egress-acl
                 interface Ethernet17
                via M, 20.30.128.128, swap 20175
                 payload autoDecide, ttlMode uniform, apply egress-acl
                 interface Ethernet19
 IP    20179    [1], 10.0.0.179/32
                via TI-LFA tunnel index 6, pop
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                    via 20.30.179.179, Ethernet40, label imp-null(3)
                    backup via 20.30.124.124, Ethernet17, label 2175 20179
 IP    20214    [1], 10.0.0.214/32
                via TI-LFA tunnel index 3, forward
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                    via 20.30.214.214, Ethernet5, label imp-null(3)
                    backup via 20.30.72.72, Ethernet9, label 20175
 IP    20217    [1], 10.0.0.217/32
                via TI-LFA tunnel index 4, forward
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                    via 20.30.217.217, Ethernet4, label imp-null(3)
                    backup via 20.30.124.124, Ethernet17, label 2175
 IP    20484    [1], 10.0.0.184/32
                via M, 20.30.31.31, swap 20484
                 payload autoDecide, ttlMode uniform, apply egress-acl
                 interface Ethernet1
                via M, 20.30.32.32, swap 20484
                 payload autoDecide, ttlMode uniform, apply egress-acl
                 interface Ethernet2
                via M, 20.30.53.53, swap 20484
                 payload autoDecide, ttlMode uniform, apply egress-acl
                 interface Ethernet13
                via M, 20.30.72.72, swap 20484
                 payload autoDecide, ttlMode uniform, apply egress-acl
                 interface Ethernet9
                via M, 20.30.84.84, swap 20484
                 payload autoDecide, ttlMode uniform, apply egress-acl
                 interface Ethernet12
                via M, 20.30.120.120, swap 20484
                 payload autoDecide, ttlMode uniform, apply egress-acl
                 interface Ethernet3
                via M, 20.30.128.128, swap 20484
                 payload autoDecide, ttlMode uniform, apply egress-acl
                 interface Ethernet19
 IP    21221    [1], 10.0.0.221/32
                via TI-LFA tunnel index 9, pop
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
 IA    362164   [1]
                via M, 20.30.31.31, pop
                 payload autoDecide, ttlMode uniform, apply egress-acl
                 interface Ethernet1
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
 IA    362170   [1]
                via M, fe80::6abf:6cff:fe35:1e31, pop
                 payload autoDecide, ttlMode uniform, apply egress-acl
                 interface Ethernet1
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

## show ip ospf segment-routing

```text
```

## show ip ospf segment-routing global-blocks

```text
```

## show ip ospf segment-routing bindings

```text
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
 * >      RD: 10.0.0.31:5001 IPv4 prefix 50.10.31.0/24
                                 10.0.0.31             -       100     0       i
 * >      RD: 10.0.0.32:5001 IPv4 prefix 50.10.32.0/24
                                 10.0.0.32             -       100     0       i
 * >      RD: 53:5001 IPv4 prefix 50.10.53.0/24
                                 10.0.0.53             -       100     0       ?
 * >      RD: 72:5001 IPv4 prefix 50.10.72.0/24
                                 10.0.0.72             -       100     0       ?
 * >      RD: 84:5001 IPv4 prefix 50.10.84.0/24
                                 10.0.0.84             0       100     0       ?
 * >      RD: 120:5001 IPv4 prefix 50.10.120.0/24
                                 10.0.0.120            0       100     0       ?
 * >      RD: 131:5001 IPv4 prefix 50.10.131.0/24
                                 10.0.0.131            -       100     0       i
 * >      RD: 179:5001 IPv4 prefix 50.10.179.0/24
                                 10.0.0.179            -       100     0       i
 * >      RD: 214:5001 IPv4 prefix 50.10.214.0/24
                                 10.0.0.214            -       100     0       i
 * >      RD: 217:5001 IPv4 prefix 50.10.217.0/24
                                 10.0.0.217            -       100     0       i
 * >      RD: 210:5001 IPv4 prefix 50.10.221.0/24
                                 10.0.0.221            -       100     0       i
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
 * >      RD: 10.0.0.31:5001 IPv6 prefix 2600:50:10:31::/64
                                 ::ffff:10.0.0.31      -       100     0       i
 * >      RD: 10.0.0.32:5001 IPv6 prefix 2600:50:10:32::/64
                                 ::ffff:10.0.0.32      -       100     0       i
 * >      RD: 53:5001 IPv6 prefix 2600:50:10:53::/64
                                 ::ffff:10.0.0.53      -       100     0       ?
 * >      RD: 72:5001 IPv6 prefix 2600:50:10:72::/64
                                 ::ffff:10.0.0.72      -       100     0       ?
 * >      RD: 84:5001 IPv6 prefix 2600:50:10:84::/64
                                 ::ffff:10.0.0.84      0       100     0       ?
 * >      RD: 120:5001 IPv6 prefix 2600:50:10:120::/64
                                 ::ffff:10.0.0.120     0       100     0       ?
 * >      RD: 131:5001 IPv6 prefix 2600:50:10:131::/64
                                 ::ffff:10.0.0.131     -       100     0       i
 * >      RD: 179:5001 IPv6 prefix 2600:50:10:179::/64
                                 ::ffff:10.0.0.179     -       100     0       i
 * >      RD: 214:5001 IPv6 prefix 2600:50:10:214::/64
                                 ::ffff:10.0.0.214     -       100     0       i
 * >      RD: 217:5001 IPv6 prefix 2600:50:10:217::/64
                                 ::ffff:10.0.0.217     -       100     0       i
 * >      RD: 210:5001 IPv6 prefix 2600:50:10:221::/64
                                 ::ffff:10.0.0.221     -       100     0       i
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
  BGP version 4, remote router ID 10.0.0.31, VRF default
  Inherits configuration from and member of peer-group IBGP_CLIENT_PEER
  Last read 00:00:35, last write 00:00:40
  Hold time is 180, keepalive interval is 60 seconds
  Configured hold time is 180, keepalive interval is 60 seconds
  Effective minimum hold time is 3 seconds
  Send failure hold time is 0 seconds
  Hold timer is active, time left: 00:02:25
  Keepalive timer is active, time left: 00:00:11
  Connect timer is inactive
  Idle-restart timer is inactive
  BGP state is Established, up for 03:04:27
  Number of transitions to established: 1
  Last state was OpenConfirm
  Last event was ReapplyOutboundPolicy
  Last sent socket-error:Connect (Network is unreachable), Last time 03:07:06, First time 03:14:23, Repeats 9
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
      Restart-State bit: yes
      Graceful notification: yes
      VPN-IPv4 is enabled, Forwarding State is not preserved
      VPN-IPv6 is enabled, Forwarding State is not preserved
  Restart timer is inactive
  End of rib timer is inactive
    VPN-IPv4 End-of-RIB received: Yes
      Received 03:04:26
      Number of stale paths removed after graceful restart: 0
      Number of paths received before End-of-RIB: 1
    VPN-IPv6 End-of-RIB received: Yes
      Received 03:04:26
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
    Updates:                       423        14
    Keepalives:                    197       212
    Enhanced Route Refresh:          0         0
    Begin of Route Refresh:          0         0
    End of Route Refresh:            0         0
    Total messages:                621       227
  Prefix Statistics:
                                   Sent      Rcvd     Best Paths     Best ECMP Paths
    IPv4 Unicast:                     0         0              0                   0
    VPN-IPv4:                        10         1              1                   0
    IPv6 Unicast:                     0         0              0                   0
    VPN-IPv6:                        10         1              1                   0
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
Local TCP address is 10.0.0.30, local port is 37921
Remote TCP address is 10.0.0.31, remote port is 179
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
    Round-trip Time (rtt/rtvar): 0.4ms/0.3ms
    Delayed Ack Timeout (ato): 40.0ms
    Congestion Window (cwnd): 10
    TCP Throughput: 299.33 Mbps
    Advertised Recv Window (rcv_space): 14480

BGP neighbor is 10.0.0.32, remote AS 64512, internal link
 Description: Arista-PE32-Q2C
  BGP version 4, remote router ID 10.0.0.32, VRF default
  Inherits configuration from and member of peer-group IBGP_CLIENT_PEER
  Last read 00:00:54, last write 00:00:34
  Hold time is 180, keepalive interval is 60 seconds
  Configured hold time is 180, keepalive interval is 60 seconds
  Effective minimum hold time is 3 seconds
  Send failure hold time is 0 seconds
  Hold timer is active, time left: 00:02:06
  Keepalive timer is active, time left: 00:00:20
  Connect timer is inactive
  Idle-restart timer is inactive
  BGP state is Established, up for 03:03:48
  Number of transitions to established: 1
  Last state was OpenConfirm
  Last event was ReapplyOutboundPolicy
  Last sent socket-error:Connect (Connection refused), Last time 03:03:53, First time 03:04:12, Repeats 4
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
      Restart-State bit: yes
      Graceful notification: yes
      VPN-IPv4 is enabled, Forwarding State is not preserved
      VPN-IPv6 is enabled, Forwarding State is not preserved
  Restart timer is inactive
  End of rib timer is inactive
    VPN-IPv4 End-of-RIB received: Yes
      Received 03:03:47
      Number of stale paths removed after graceful restart: 0
      Number of paths received before End-of-RIB: 1
    VPN-IPv6 End-of-RIB received: Yes
      Received 03:03:47
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
    Updates:                       419        14
    Keepalives:                    194       215
    Enhanced Route Refresh:          0         0
    Begin of Route Refresh:          0         0
    End of Route Refresh:            0         0
    Total messages:                614       230
  Prefix Statistics:
                                   Sent      Rcvd     Best Paths     Best ECMP Paths
    IPv4 Unicast:                     0         0              0                   0
    VPN-IPv4:                        10         1              1                   0
    IPv6 Unicast:                     0         0              0                   0
    VPN-IPv6:                        10         1              1                   0
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
Remote TCP address is 10.0.0.32, remote port is 42379
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
    Round-trip Time (rtt/rtvar): 0.3ms/0.0ms
    Delayed Ack Timeout (ato): 40.0ms
    Congestion Window (cwnd): 10
    TCP Throughput: 437.13 Mbps
    Advertised Recv Window (rcv_space): 14600

BGP neighbor is 10.0.0.53, remote AS 64512, internal link
 Description: Arrcus-53
  BGP version 4, remote router ID 10.0.0.53, VRF default
  Inherits configuration from and member of peer-group IBGP_CLIENT_PEER
  Last read 00:00:55, last write 00:00:18
  Hold time is 180, keepalive interval is 60 seconds
  Configured hold time is 180, keepalive interval is 60 seconds
  Effective minimum hold time is 3 seconds
  Send failure hold time is 0 seconds
  Hold timer is active, time left: 00:02:05
  Keepalive timer is active, time left: 00:00:29
  Connect timer is inactive
  Idle-restart timer is inactive
  BGP state is Established, up for 03:05:55
  Number of transitions to established: 2
  Last state was OpenConfirm
  Last event was ReapplyOutboundPolicy
  Last rcvd notification:Cease/other configuration change, Last time 03:05:56
  Last sent socket-error:Connect (Connection refused), Last time 03:10:13, First time 03:14:24, Repeats 8
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
      Restart-State bit: no
      Graceful notification: yes
      VPN-IPv4 is enabled, Forwarding State is not preserved
      VPN-IPv6 is enabled, Forwarding State is not preserved
    Graceful Restart received:
      Restart-time is 120
      Restart-State bit: no
      Graceful notification: no
      VPN-IPv4 is enabled, Forwarding State is preserved
      VPN-IPv6 is enabled, Forwarding State is preserved
  Restart timer is inactive
  End of rib timer is inactive
    VPN-IPv4 End-of-RIB received: Yes
      Received 03:05:55
      Number of stale paths removed after graceful restart: 0
    VPN-IPv6 End-of-RIB received: Yes
      Received 03:05:55
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
    Opens:                  2         2
    Notifications:          0         1
    Updates:              151       323
    Keepalives:           206       188
    Route Refresh:          0         0
    Total messages:       359       514
  Prefix Statistics:
                                   Sent      Rcvd     Best Paths     Best ECMP Paths
    IPv4 Unicast:                     0         0              0                   0
    VPN-IPv4:                        10         1              1                   0
    IPv6 Unicast:                     0         0              0                   0
    VPN-IPv6:                        10         1              1                   0
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
Local TCP address is 10.0.0.30, local port is 35537
Remote TCP address is 10.0.0.53, remote port is 179
Local next hop for next hop self:
  VPN-IPv4: 10.0.0.30
  VPN-IPv6: ::ffff:10.0.0.30
TCP Socket Information:
  TCP state is ESTABLISHED
  Recv-Q: 0/32768
  Send-Q: 0/46080
  Outgoing Maximum Segment Size (MSS): 1436
  Total Number of TCP retransmissions: 8
  Options:
    Timestamps enabled: yes
    Selective Acknowledgments enabled: yes
    Window Scale enabled: yes
    Explicit Congestion Notification (ECN) enabled: no
  Socket Statistics:
    Window Scale (wscale): 14,7
    Retransmission Timeout (rto): 204.0ms
    Round-trip Time (rtt/rtvar): 0.2ms/0.0ms
    Delayed Ack Timeout (ato): 40.0ms
    Congestion Window (cwnd): 5
    Slow-start Threshold (ssthresh): 8
    TCP Throughput: 249.74 Mbps
    Advertised Recv Window (rcv_space): 14480

BGP neighbor is 10.0.0.72, remote AS 64512, internal link
 Description: Ciena-5134-72
  BGP version 4, remote router ID 10.0.0.72, VRF default
  Inherits configuration from and member of peer-group IBGP_CLIENT_PEER
  Last read 00:00:29, last write 00:00:53
  Hold time is 180, keepalive interval is 60 seconds
  Configured hold time is 180, keepalive interval is 60 seconds
  Effective minimum hold time is 3 seconds
  Send failure hold time is 0 seconds
  Hold timer is active, time left: 00:02:31
  Keepalive timer is active, time left: 00:00:05
  Connect timer is inactive
  Idle-restart timer is inactive
  BGP state is Established, up for 03:13:29
  Number of transitions to established: 1
  Last state was OpenConfirm
  Last event was ReapplyOutboundPolicy
  Last sent socket-error:Connect (Connection refused), Last time 03:13:59, First time 03:14:23, Repeats 5
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
      Received 03:13:19
      Number of stale paths removed after graceful restart: 0
      Number of paths received before End-of-RIB: 1
    VPN-IPv6 End-of-RIB received: Yes
      Received 03:13:19
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
    Updates:              421        20
    Keepalives:           206       194
    Route Refresh:          0         0
    Total messages:       628       215
  Prefix Statistics:
                                   Sent      Rcvd     Best Paths     Best ECMP Paths
    IPv4 Unicast:                     0         0              0                   0
    VPN-IPv4:                        10         1              1                   0
    IPv6 Unicast:                     0         0              0                   0
    VPN-IPv6:                        10         1              1                   0
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
Remote TCP address is 10.0.0.72, remote port is 40127
Local next hop for next hop self:
  VPN-IPv4: 10.0.0.30
  VPN-IPv6: ::ffff:10.0.0.30
TCP Socket Information:
  TCP state is ESTABLISHED
  Recv-Q: 0/32768
  Send-Q: 0/46080
  Outgoing Maximum Segment Size (MSS): 1460
  Total Number of TCP retransmissions: 10
  Options:
    Timestamps enabled: no
    Selective Acknowledgments enabled: yes
    Window Scale enabled: yes
    Explicit Congestion Notification (ECN) enabled: no
  Socket Statistics:
    Window Scale (wscale): 7,7
    Retransmission Timeout (rto): 204.0ms
    Round-trip Time (rtt/rtvar): 0.6ms/0.0ms
    Delayed Ack Timeout (ato): 40.0ms
    Congestion Window (cwnd): 2
    Slow-start Threshold (ssthresh): 2
    TCP Throughput: 36.33 Mbps
    Advertised Recv Window (rcv_space): 14600

BGP neighbor is 10.0.0.84, remote AS 64512, internal link
 Description: Ericsson_84
  BGP version 4, remote router ID 10.0.0.84, VRF default
  Inherits configuration from and member of peer-group IBGP_CLIENT_PEER
  Last read 00:00:47, last write 00:00:37
  Hold time is 180, keepalive interval is 60 seconds
  Configured hold time is 180, keepalive interval is 60 seconds
  Effective minimum hold time is 3 seconds
  Send failure hold time is 0 seconds
  Hold timer is active, time left: 00:02:13
  Keepalive timer is active, time left: 00:00:10
  Connect timer is inactive
  Idle-restart timer is inactive
  BGP state is Established, up for 03:09:40
  Number of transitions to established: 1
  Last state was OpenConfirm
  Last event was ReapplyOutboundPolicy
  Last sent notification:Open Message Error/bad AS number, Last time 03:10:28, First time 03:14:24, Repeats 10
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
      Restart-State bit: no
      Graceful notification: yes
      VPN-IPv4 is enabled, Forwarding State is not preserved
      VPN-IPv6 is enabled, Forwarding State is not preserved
    Graceful Restart received:
      Restart-time is 120
      Restart-State bit: yes
      Graceful notification: no
      IPv4 Unicast is enabled, Forwarding State is preserved
      VPN-IPv4 is enabled, Forwarding State is preserved
      IPv6 Unicast is enabled, Forwarding State is preserved
      VPN-IPv6 is enabled, Forwarding State is preserved
  Restart timer is inactive
  End of rib timer is inactive
    VPN-IPv4 End-of-RIB received: Yes
      Received 03:08:55
      Number of stale paths removed after graceful restart: 0
    VPN-IPv6 End-of-RIB received: Yes
      Received 03:08:55
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
    Opens:                          12        12
    Notifications:                  11         0
    Updates:                       453         6
    Keepalives:                    198       187
    Enhanced Route Refresh:          0         8
    Begin of Route Refresh:          8         0
    End of Route Refresh:            8         0
    Total messages:                690       213
  Prefix Statistics:
                                   Sent      Rcvd     Best Paths     Best ECMP Paths
    IPv4 Unicast:                     0         0              0                   0
    VPN-IPv4:                        10         1              1                   0
    IPv6 Unicast:                     0         0              0                   0
    VPN-IPv6:                        10         1              1                   0
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
Remote TCP address is 10.0.0.84, remote port is 56758
Local next hop for next hop self:
  VPN-IPv4: 10.0.0.30
  VPN-IPv6: ::ffff:10.0.0.30
TCP Socket Information:
  TCP state is ESTABLISHED
  Recv-Q: 0/32768
  Send-Q: 0/46080
  Outgoing Maximum Segment Size (MSS): 1428
  Total Number of TCP retransmissions: 7
  Options:
    Timestamps enabled: yes
    Selective Acknowledgments enabled: yes
    Window Scale enabled: yes
    Explicit Congestion Notification (ECN) enabled: no
  Socket Statistics:
    Window Scale (wscale): 0,7
    Retransmission Timeout (rto): 432.0ms
    Round-trip Time (rtt/rtvar): 231.9ms/0.2ms
    Delayed Ack Timeout (ato): 40.0ms
    Congestion Window (cwnd): 10
    TCP Throughput: 0.49 Mbps
    Advertised Recv Window (rcv_space): 14600

BGP neighbor is 10.0.0.120, remote AS 64512, internal link
 Description: Huawei_120
  BGP version 4, remote router ID 10.0.0.120, VRF default
  Inherits configuration from and member of peer-group IBGP_CLIENT_PEER
  Last read 00:00:19, last write 00:00:27
  Hold time is 180, keepalive interval is 60 seconds
  Configured hold time is 180, keepalive interval is 60 seconds
  Effective minimum hold time is 3 seconds
  Send failure hold time is 0 seconds
  Hold timer is active, time left: 00:02:41
  Keepalive timer is active, time left: 00:00:31
  Connect timer is inactive
  Idle-restart timer is inactive
  BGP state is Established, up for 03:09:02
  Number of transitions to established: 1
  Last state was OpenConfirm
  Last event was ReapplyOutboundPolicy
  Last sent notification:Open Message Error/bad AS number, Last time 03:09:41, First time 03:10:12, Repeats 2
  Last sent socket-error:Connect (Connection refused), Last time 03:09:47, First time 03:10:05, Repeats 4
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
    Opens:                  4         4
    Notifications:          3         0
    Updates:              421        20
    Keepalives:           198       223
    Route Refresh:          0         2
    Total messages:       626       249
  Prefix Statistics:
                                   Sent      Rcvd     Best Paths     Best ECMP Paths
    IPv4 Unicast:                     0         0              0                   0
    VPN-IPv4:                        10         1              1                   0
    IPv6 Unicast:                     0         0              0                   0
    VPN-IPv6:                        10         1              1                   0
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
Remote TCP address is 10.0.0.120, remote port is 62412
Local next hop for next hop self:
  VPN-IPv4: 10.0.0.30
  VPN-IPv6: ::ffff:10.0.0.30
TCP Socket Information:
  TCP state is ESTABLISHED
  Recv-Q: 0/32768
  Send-Q: 0/46080
  Outgoing Maximum Segment Size (MSS): 1384
  Total Number of TCP retransmissions: 2
  Options:
    Timestamps enabled: yes
    Selective Acknowledgments enabled: yes
    Window Scale enabled: yes
    Explicit Congestion Notification (ECN) enabled: no
  Socket Statistics:
    Window Scale (wscale): 3,7
    Retransmission Timeout (rto): 204.0ms
    Round-trip Time (rtt/rtvar): 0.4ms/0.1ms
    Delayed Ack Timeout (ato): 40.0ms
    Congestion Window (cwnd): 7
    Slow-start Threshold (ssthresh): 7
    TCP Throughput: 210.61 Mbps
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
  Connect timer is active, time left: 00:02:09
  Connection interval is 148 seconds
  Failed connection attempts is 35
  Idle-restart timer is inactive
  BGP state is Active
  Number of transitions to established: 0
  Last state was Connect
  Last event was TransportError
  Last sent socket-error:Connect (Connection refused), Last time 00:00:48, First time 01:54:16, Repeats 50
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
  BGP version 4, remote router ID 10.0.0.131, VRF default
  Inherits configuration from and member of peer-group IBGP_CLIENT_PEER
  Last read 00:00:17, last write 00:00:04
  Hold time is 90, keepalive interval is 30 seconds
  Configured hold time is 180, keepalive interval is 60 seconds
  Effective minimum hold time is 3 seconds
  Send failure hold time is 0 seconds
  Hold timer is active, time left: 00:01:13
  Keepalive timer is active, time left: 00:00:20
  Connect timer is inactive
  Idle-restart timer is inactive
  BGP state is Established, up for 01:37:36
  Number of transitions to established: 1
  Last state was OpenConfirm
  Last event was RecvUpdate
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
      Restart-State bit: no
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
      Received 01:37:35
      Number of stale paths removed after graceful restart: 0
      Number of paths received before End-of-RIB: 1
    VPN-IPv6 End-of-RIB received: Yes
      Received 01:37:35
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
    Updates:               95         4
    Keepalives:           223       217
    Route Refresh:          0         0
    Total messages:       319       222
  Prefix Statistics:
                                   Sent      Rcvd     Best Paths     Best ECMP Paths
    IPv4 Unicast:                     0         0              0                   0
    VPN-IPv4:                        10         1              1                   0
    IPv6 Unicast:                     0         0              0                   0
    VPN-IPv6:                        10         1              1                   0
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
Local TCP address is 10.0.0.30, local port is 41961
Remote TCP address is 10.0.0.131, remote port is 179
Local next hop for next hop self:
  VPN-IPv4: 10.0.0.30
  VPN-IPv6: ::ffff:10.0.0.30
TCP Socket Information:
  TCP state is ESTABLISHED
  Recv-Q: 0/32768
  Send-Q: 0/332800
  Outgoing Maximum Segment Size (MSS): 1448
  Total Number of TCP retransmissions: 1
  Options:
    Timestamps enabled: yes
    Selective Acknowledgments enabled: yes
    Window Scale enabled: yes
    Explicit Congestion Notification (ECN) enabled: no
  Socket Statistics:
    Window Scale (wscale): 1,7
    Retransmission Timeout (rto): 204.0ms
    Round-trip Time (rtt/rtvar): 0.6ms/0.2ms
    Delayed Ack Timeout (ato): 40.0ms
    Congestion Window (cwnd): 10
    TCP Throughput: 199.72 Mbps
    Advertised Recv Window (rcv_space): 14480

BGP neighbor is 10.0.0.179, remote AS 64512, internal link
 Description: Juniper-179
  BGP version 4, remote router ID 10.0.0.179, VRF default
  Inherits configuration from and member of peer-group IBGP_CLIENT_PEER
  Last read 00:00:15, last write 00:00:03
  Hold time is 90, keepalive interval is 30 seconds
  Configured hold time is 180, keepalive interval is 60 seconds
  Effective minimum hold time is 3 seconds
  Send failure hold time is 0 seconds
  Hold timer is active, time left: 00:01:15
  Keepalive timer is active, time left: 00:00:24
  Connect timer is inactive
  Idle-restart timer is inactive
  BGP state is Established, up for 00:04:43
  Number of transitions to established: 3
  Last state was OpenConfirm
  Last event was RecvUpdate
  Last sent notification:Hold Timer Expired Error/None, Last time 00:09:30
  Last rcvd notification:Cease/peer de-configured, Last time 02:49:27
  Last sent socket-error:Connect (Network is unreachable), Last time 00:05:14, First time 00:09:28, Repeats 8
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
      Restart-State bit: no
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
      Received 00:04:43
      Number of stale paths removed after graceful restart: 0
      Number of paths received before End-of-RIB: 1
    VPN-IPv6 End-of-RIB received: Yes
      Received 00:04:43
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
    Opens:                  3         3
    Notifications:          1         1
    Updates:              185        12
    Keepalives:           376       370
    Route Refresh:          0         2
    Total messages:       565       388
  Prefix Statistics:
                                   Sent      Rcvd     Best Paths     Best ECMP Paths
    IPv4 Unicast:                     0         0              0                   0
    VPN-IPv4:                        10         1              1                   0
    IPv6 Unicast:                     0         0              0                   0
    VPN-IPv6:                        10         1              1                   0
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
Local TCP address is 10.0.0.30, local port is 46105
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
    Retransmission Timeout (rto): 204.0ms
    Round-trip Time (rtt/rtvar): 1.6ms/1.4ms
    Delayed Ack Timeout (ato): 40.0ms
    Congestion Window (cwnd): 10
    TCP Throughput: 73.18 Mbps
    Advertised Recv Window (rcv_space): 14480

BGP neighbor is 10.0.0.214, remote AS 64512, internal link
 Description: Nokia-SXR-214
  BGP version 4, remote router ID 10.0.0.214, VRF default
  Inherits configuration from and member of peer-group IBGP_CLIENT_PEER
  Last read 00:00:19, last write 00:00:17
  Hold time is 90, keepalive interval is 30 seconds
  Configured hold time is 180, keepalive interval is 60 seconds
  Effective minimum hold time is 3 seconds
  Send failure hold time is 0 seconds
  Hold timer is active, time left: 00:01:11
  Keepalive timer is active, time left: 00:00:08
  Connect timer is inactive
  Idle-restart timer is inactive
  BGP state is Established, up for 02:53:49
  Number of transitions to established: 1
  Last state was OpenConfirm
  Last event was ReapplyOutboundPolicy
  Last sent socket-error:Connect (Network is unreachable), Last time 02:53:53, First time 03:14:23, Repeats 14
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
      Restart-State bit: no
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
      Received 02:53:45
      Number of stale paths removed after graceful restart: 0
    VPN-IPv6 End-of-RIB received: Yes
      Received 02:53:45
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
    Updates:              162        12
    Keepalives:           393       349
    Route Refresh:          0         4
    Total messages:       556       366
  Prefix Statistics:
                                   Sent      Rcvd     Best Paths     Best ECMP Paths
    IPv4 Unicast:                     0         0              0                   0
    VPN-IPv4:                        10         1              1                   0
    IPv6 Unicast:                     0         0              0                   0
    VPN-IPv6:                        10         1              1                   0
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
Local TCP address is 10.0.0.30, local port is 42259
Remote TCP address is 10.0.0.214, remote port is 179
Local next hop for next hop self:
  VPN-IPv4: 10.0.0.30
  VPN-IPv6: ::ffff:10.0.0.30
TCP Socket Information:
  TCP state is ESTABLISHED
  Recv-Q: 0/32768
  Send-Q: 0/332800
  Outgoing Maximum Segment Size (MSS): 1448
  Total Number of TCP retransmissions: 1
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
    TCP Throughput: 277.79 Mbps
    Advertised Recv Window (rcv_space): 14480

BGP neighbor is 10.0.0.217, remote AS 64512, internal link
 Description: Nokia
  BGP version 4, remote router ID 10.0.0.217, VRF default
  Inherits configuration from and member of peer-group IBGP_CLIENT_PEER
  Last read 00:00:22, last write 00:00:18
  Hold time is 90, keepalive interval is 30 seconds
  Configured hold time is 180, keepalive interval is 60 seconds
  Effective minimum hold time is 3 seconds
  Send failure hold time is 0 seconds
  Hold timer is active, time left: 00:01:08
  Keepalive timer is active, time left: 00:00:04
  Connect timer is inactive
  Idle-restart timer is inactive
  BGP state is Established, up for 01:03:22
  Number of transitions to established: 2
  Last state was OpenConfirm
  Last event was RecvUpdate
  Last rcvd notification:Cease/administrative shutdown, Last time 01:03:25
  Last sent socket-error:Connect (Connection refused), Last time 01:03:24, First time 01:04:01, Repeats 6
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
      Restart-State bit: no
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
      Received 01:03:21
      Number of stale paths removed after graceful restart: 0
      Number of paths received before End-of-RIB: 1
    VPN-IPv6 End-of-RIB received: Yes
      Received 01:03:21
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
    Opens:                  2         2
    Notifications:          0         1
    Updates:               48        10
    Keepalives:           149       130
    Route Refresh:          0         0
    Total messages:       199       143
  Prefix Statistics:
                                   Sent      Rcvd     Best Paths     Best ECMP Paths
    IPv4 Unicast:                     0         0              0                   0
    VPN-IPv4:                        10         1              1                   0
    IPv6 Unicast:                     0         0              0                   0
    VPN-IPv6:                        10         1              1                   0
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
Remote TCP address is 10.0.0.217, remote port is 51165
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
    TCP Throughput: 156.90 Mbps
    Advertised Recv Window (rcv_space): 14600

BGP neighbor is 10.0.0.221, remote AS 64512, internal link
 Description: Ribbon-221
  BGP version 4, remote router ID 10.0.0.221, VRF default
  Inherits configuration from and member of peer-group IBGP_CLIENT_PEER
  Last read 00:00:06, last write 00:00:18
  Hold time is 180, keepalive interval is 60 seconds
  Configured hold time is 180, keepalive interval is 60 seconds
  Effective minimum hold time is 3 seconds
  Send failure hold time is 0 seconds
  Hold timer is active, time left: 00:02:54
  Keepalive timer is active, time left: 00:00:25
  Connect timer is inactive
  Idle-restart timer is inactive
  BGP state is Established, up for 01:38:48
  Number of transitions to established: 1
  Last state was OpenConfirm
  Last event was RecvKeepAlive
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
    Updates:                        93         2
    Keepalives:                    110       273
    Enhanced Route Refresh:          0         0
    Begin of Route Refresh:          0         0
    End of Route Refresh:            0         0
    Total messages:                204       276
  Prefix Statistics:
                                   Sent      Rcvd     Best Paths     Best ECMP Paths
    IPv4 Unicast:                     0         0              0                   0
    VPN-IPv4:                        10         1              1                   0
    IPv6 Unicast:                     0         0              0                   0
    VPN-IPv6:                        10         1              1                   0
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
Local TCP address is 10.0.0.30, local port is 34309
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
    TCP Throughput: 524.16 Mbps
    Advertised Recv Window (rcv_space): 14480

```

## show tunnel rib system-tunnel-rib brief

```text
Tunnel RIB: system-tunnel-rib
Endpoint        Tunnel Type     Index(es)   Tunnel Preference   IGP Preference 
-------------- --------------- ----------- ------------------- ----------------
10.0.0.31/32    IS-IS SR IPv4   8           65                  115            
10.0.0.32/32    IS-IS SR IPv4   9           65                  115            
10.0.0.53/32    IS-IS SR IPv4   5           65                  115            
10.0.0.72/32    IS-IS SR IPv4   2           65                  115            
10.0.0.84/32    IS-IS SR IPv4   1           65                  115            
10.0.0.120/32   IS-IS SR IPv4   7           65                  115            
10.0.0.124/32   IS-IS SR IPv4   14          65                  115            
10.0.0.128/32   IS-IS SR IPv4   11          65                  115            
10.0.0.131/32   IS-IS SR IPv4   12          65                  115            
10.0.0.175/32   IS-IS SR IPv4   4           65                  115            
10.0.0.179/32   IS-IS SR IPv4   6           65                  115            
10.0.0.184/32   IS-IS SR IPv4   15          65                  115            
10.0.0.214/32   IS-IS SR IPv4   10          65                  115            
10.0.0.217/32   IS-IS SR IPv4   16          65                  115            
10.0.0.221/32   IS-IS SR IPv4   13          65                  115            

   IGP Metric    Metric Type
---------------- -----------
   10            metric     
   10            metric     
   10            metric     
   20            metric     
   20            metric     
   10            metric     
   10            metric     
   10            metric     
   30            metric     
   20            metric     
   10            metric     
   40            metric     
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
>C    10.0.0.30/32 [0 pref/0 metric] updated 04:08:56 ago
         via Loopback0, directly connected
>C    20.30.31.0/24 [0 pref/0 metric] updated 04:05:10 ago
         via Ethernet1, directly connected
>C    20.30.32.0/24 [0 pref/0 metric] updated 03:44:56 ago
         via Ethernet2, directly connected
>C    20.30.53.0/24 [0 pref/0 metric] updated 03:54:28 ago
         via Ethernet13, directly connected
>C    20.30.72.0/24 [0 pref/0 metric] updated 03:58:16 ago
         via Ethernet9, directly connected
>C    20.30.84.0/24 [0 pref/0 metric] updated 03:51:51 ago
         via Ethernet12, directly connected
>C    20.30.120.0/24 [0 pref/0 metric] updated 01:46:23 ago
         via Ethernet3, directly connected
>C    20.30.124.0/24 [0 pref/0 metric] updated 00:32:27 ago
         via Ethernet17, directly connected
>C    20.30.128.0/24 [0 pref/0 metric] updated 00:32:47 ago
         via Ethernet19, directly connected
>C    20.30.179.0/24 [0 pref/0 metric] updated 00:05:06 ago
         via Ethernet40, directly connected
>C    20.30.184.0/24 [0 pref/0 metric] updated 00:46:21 ago
         via Ethernet7, directly connected
>C    20.30.214.0/24 [0 pref/0 metric] updated 04:40:32 ago
         via Ethernet5, directly connected
>C    20.30.217.0/24 [0 pref/0 metric] updated 01:05:59 ago
         via Ethernet4, directly connected
>C    20.30.221.0/24 [0 pref/0 metric] updated 01:39:17 ago
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
>P    0.0.0.0/8 [1 pref/0 metric] updated 09:31:13 ago
         via Null0, directly connected [NF]
>P    127.0.0.0/8 [1 pref/0 metric] updated 09:31:13 ago
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
>I    10.0.0.31/32 [115 pref/10 metric] updated 01:17:56 ago
         via 20.30.31.31, Ethernet1
>I    10.0.0.32/32 [115 pref/10 metric] updated 01:18:23 ago
         via 20.30.32.32, Ethernet2
>I    10.0.0.53/32 [115 pref/10 metric] updated 01:19:02 ago
         via 20.30.53.53, Ethernet13
>I    10.0.0.72/32 [115 pref/20 metric] updated 01:19:06 ago
         via 20.30.72.72, Ethernet9
>I    10.0.0.84/32 [115 pref/20 metric] updated 01:19:00 ago
         via 20.30.84.84, Ethernet12
>I    10.0.0.120/32 [115 pref/10 metric] updated 01:19:05 ago
         via 20.30.120.120, Ethernet3
>I    10.0.0.124/32 [115 pref/10 metric] updated 00:32:26 ago
         via 20.30.124.124, Ethernet17
>I    10.0.0.128/32 [115 pref/10 metric] updated 00:32:37 ago
         via 20.30.128.128, Ethernet19
>I    10.0.0.131/32 [115 pref/30 metric] updated 00:25:12 ago
         via 20.30.31.31, Ethernet1
         via 20.30.32.32, Ethernet2
         via 20.30.53.53, Ethernet13
         via 20.30.72.72, Ethernet9
         via 20.30.84.84, Ethernet12
         via 20.30.120.120, Ethernet3
         via 20.30.124.124, Ethernet17
         via 20.30.128.128, Ethernet19
>I    10.0.0.175/32 [115 pref/20 metric] updated 00:25:12 ago
         via 20.30.31.31, Ethernet1
         via 20.30.32.32, Ethernet2
         via 20.30.53.53, Ethernet13
         via 20.30.72.72, Ethernet9
         via 20.30.84.84, Ethernet12
         via 20.30.120.120, Ethernet3
         via 20.30.124.124, Ethernet17
         via 20.30.128.128, Ethernet19
>I    10.0.0.179/32 [115 pref/10 metric] updated 00:05:06 ago
         via 20.30.179.179, Ethernet40
>I    10.0.0.184/32 [115 pref/40 metric] updated 00:18:21 ago
         via 20.30.31.31, Ethernet1
         via 20.30.32.32, Ethernet2
         via 20.30.53.53, Ethernet13
         via 20.30.72.72, Ethernet9
         via 20.30.84.84, Ethernet12
         via 20.30.120.120, Ethernet3
         via 20.30.124.124, Ethernet17
         via 20.30.128.128, Ethernet19
>I    10.0.0.214/32 [115 pref/10 metric] updated 01:19:01 ago
         via 20.30.214.214, Ethernet5
>I    10.0.0.216/32 [115 pref/20 metric] updated 01:19:01 ago
         via 20.30.214.214, Ethernet5
>I    10.0.0.217/32 [115 pref/10 metric] updated 01:04:37 ago
         via 20.30.217.217, Ethernet4
>I    10.0.0.221/32 [115 pref/10 metric] updated 01:19:06 ago
         via 20.30.221.221, Ethernet15
>I    20.31.175.0/24 [115 pref/20 metric] updated 00:49:41 ago
         via 20.30.31.31, Ethernet1
>I    20.32.175.0/24 [115 pref/20 metric] updated 01:18:23 ago
         via 20.30.32.32, Ethernet2
>I    20.53.175.0/24 [115 pref/20 metric] updated 01:19:02 ago
         via 20.30.53.53, Ethernet13
>I    20.72.175.0/24 [115 pref/20 metric] updated 01:19:06 ago
         via 20.30.72.72, Ethernet9
>I    20.84.175.0/24 [115 pref/30 metric] updated 00:25:12 ago
         via 20.30.31.31, Ethernet1
         via 20.30.32.32, Ethernet2
         via 20.30.53.53, Ethernet13
         via 20.30.72.72, Ethernet9
         via 20.30.84.84, Ethernet12
         via 20.30.120.120, Ethernet3
         via 20.30.124.124, Ethernet17
         via 20.30.128.128, Ethernet19
>I    20.120.175.0/24 [115 pref/20 metric] updated 01:03:32 ago
         via 20.30.120.120, Ethernet3
>I    20.120.214.0/24 [115 pref/20 metric] updated 01:19:05 ago
         via 20.30.120.120, Ethernet3
>I    20.124.175.0/24 [115 pref/20 metric] updated 00:32:26 ago
         via 20.30.124.124, Ethernet17
>I    20.128.175.0/24 [115 pref/20 metric] updated 00:32:37 ago
         via 20.30.128.128, Ethernet19
>I    20.131.175.0/24 [115 pref/30 metric] updated 00:25:12 ago
         via 20.30.31.31, Ethernet1
         via 20.30.32.32, Ethernet2
         via 20.30.53.53, Ethernet13
         via 20.30.72.72, Ethernet9
         via 20.30.84.84, Ethernet12
         via 20.30.120.120, Ethernet3
         via 20.30.124.124, Ethernet17
         via 20.30.128.128, Ethernet19
>I    20.175.179.0/24 [115 pref/20 metric] updated 00:05:06 ago
         via 20.30.179.179, Ethernet40
>I    20.175.184.0/24 [115 pref/30 metric] updated 00:25:12 ago
         via 20.30.31.31, Ethernet1
         via 20.30.32.32, Ethernet2
         via 20.30.53.53, Ethernet13
         via 20.30.72.72, Ethernet9
         via 20.30.84.84, Ethernet12
         via 20.30.120.120, Ethernet3
         via 20.30.124.124, Ethernet17
         via 20.30.128.128, Ethernet19
>I    20.175.214.0/24 [115 pref/20 metric] updated 01:19:01 ago
         via 20.30.214.214, Ethernet5
>I    20.175.217.0/24 [115 pref/20 metric] updated 00:47:24 ago
         via 20.30.217.217, Ethernet4
>I    20.175.221.0/24 [115 pref/20 metric] updated 01:19:06 ago
         via 20.30.221.221, Ethernet15
>I    20.214.216.0/24 [115 pref/20 metric] updated 01:19:01 ago
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
>C    2001:0:30:31::/64 [0 pref/0 metric] updated 02:07:33 ago
         via Ethernet1, directly connected
>C    2001:0:30:32::/64 [0 pref/0 metric] updated 02:07:21 ago
         via Ethernet2, directly connected
>C    2001:0:30:72::/64 [0 pref/0 metric] updated 02:04:58 ago
         via Ethernet9, directly connected
>C    2001:0:30:84::/64 [0 pref/0 metric] updated 02:04:58 ago
         via Ethernet12, directly connected
>C    2001:0:30:120::/64 [0 pref/0 metric] updated 01:46:23 ago
         via Ethernet3, directly connected
>C    2001:0:30:124::/64 [0 pref/0 metric] updated 00:32:27 ago
         via Ethernet17, directly connected
>C    2001:0:30:128::/64 [0 pref/0 metric] updated 00:32:47 ago
         via Ethernet19, directly connected
>C    2001:0:30:179::/64 [0 pref/0 metric] updated 00:05:06 ago
         via Ethernet40, directly connected
>C    2001:0:30:184::/64 [0 pref/0 metric] updated 00:46:21 ago
         via Ethernet7, directly connected
>C    2001:0:30:214::/64 [0 pref/0 metric] updated 02:04:58 ago
         via Ethernet5, directly connected
>C    2001:0:30:217::/64 [0 pref/0 metric] updated 01:05:43 ago
         via Ethernet4, directly connected
>C    2001:0:30:221::/64 [0 pref/0 metric] updated 01:39:17 ago
         via Ethernet15, directly connected
>C    2001:0:53:120::/64 [0 pref/0 metric] updated 02:04:58 ago
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
>P    ::/96 [1 pref/0 metric] updated 02:07:34 ago
         via Null0, directly connected [NF]
>P    ::ffff:127.0.0.0/104 [1 pref/0 metric] updated 02:07:34 ago
         via :: [1 pref/1 metric] type ipv6
            via , directly connected
>P    fe80::/10 [1 pref/0 metric] updated 02:07:34 ago
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
>I    2001:0:120:175::/64 [115 pref/20 metric] updated 01:03:30 ago
         via fe80::be31:e2ff:fee1:ec2c, Ethernet3
>I    2001:0:120:214::/64 [115 pref/20 metric] updated 01:19:05 ago
         via fe80::be31:e2ff:fee1:ec2c, Ethernet3
```

## show platform sand l3 summary

```text
Number of vrfs: 3

Ipv4:
  Routes:       122  backlog:  0  unprogrammed:  0
  Adjacencies:  163  backlog:  0  unprogrammed:  0
Ipv6:
  Routes:       34   backlog:  0  unprogrammed:  0
  Adjacencies:  163  backlog:  0  unprogrammed:  0
Mpls:
  Routes:       30  backlog:  0  unprogrammed:  0
  Adjacencies:  18  backlog:  0  unprogrammed:  0

Jericho2 Ip Fecs:
  Non-ecmp fecs:  4155  ecmp fecs:  2  fec entries:  4171
Jericho2 Mpls Fecs:
  Non-ecmp fecs:  15  ecmp fecs:  3  fec entries:  38
Jericho2 Vxlan Tunnel Fecs:
  Non-ecmp fecs:  0  ecmp fecs:  0  fec entries:  0
  Number of vxlan tunnels configured: 0

Jericho2 Lpm Routes:
  Routes:   122  unprogrammed:   0   
  Routes6:  34   unprogrammed6:  0   
  Backlog:  0  

Jericho2 Lpm:
  TCAM entries used:   3   Percent free:  99  ADS2 entries used:   8  Percent free:  99
  Pivot buckets used:  4   Rows used:     2   Entries Per Bucket:  2  Percent free:  99
  Route buckets used:  25  Rows used:     4   Entries Per Bucket:  6  Percent free:  99

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
  FixedSystem: 12
Egress Sflow rewrite entries in use (in each fap):
  FixedSystem: 0

Egress rewrite chains in backlog: resource-full 0, no-interface 0

Glem entries used per fap :
  FixedSystem: 4152

Jericho2 Fec:
  Maximum FEC hierarchy levels:  2
  ReusedEcmp:  117  allocs:  565  frees:  489  shuffles:  0  cmds:  0
  Zombies:     0    purges:    0
  Quarantine:  0/0  shuffles:  0  deletes:  0   
  Preserved FECs: 0
    First FEC preserved: never
    Last FEC preserved: never
  Fec insertion failures:  0
  Level1  Fecs:
    Non-ecmp fecs:            13  ecmp fecs:            1 
    Non-ecmp (Percent free):  99  ecmp (Percent free):  99
  Level2  Fecs:
    Non-ecmp fecs:            97  ecmp fecs:            5 
    Non-ecmp (Percent free):  99  ecmp (Percent free):  99
  Level3  Fecs:
    Non-ecmp fecs:            0    ecmp fecs:            0  
    Non-ecmp (Percent free):  100  ecmp (Percent free):  100

Lpm Detail:
  Requests:  1592  cleanses:  407  batches:  407  avg batch size:  3

Jericho Arp:
  ArpTable writes:      30223  queued      0   
  IngressTable writes:  63312  queued      0   
  Coprocessors:         1      in CmdRing

Tunnel Counter Status
  Number of MPLS tunnels:                  44   
  Number of uncountable MPLS tunnels:      44   
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
|0  |10.0.0.31/32      |ROUTE| Et1                |1007 |103422  | 68:bf:6c:35:1e:31 |  -  |183511|   -   
|0  |10.0.0.32/32      |ROUTE| Et2                |1014 |103425  | d4:af:f7:2f:13:96 |  -  |183524|   -   
|0  |10.0.0.53/32      |ROUTE| Et13               |1010 |103426  | 5c:07:58:a3:0a:aa |  -  |183607|   -   
|0  |10.0.0.72/32      |ROUTE| Et9                |1009 |103423  | e0:9b:27:c4:c5:84 |  -  |183558|   -   
|0  |10.0.0.84/32      |ROUTE| Et12               |1011 |103424  | 58:70:7f:9f:c4:03 |  -  |183567|   -   
|0  |10.0.0.120/32     |ROUTE| Et3                |1008 |103427  | bc:31:e2:e1:ec:2c |  -  |183513|   -   
|0  |10.0.0.124/32     |ROUTE| Et17               |1012 |103430  | 64:6d:4e:32:e1:22 |  -  |183543|   -   
|0  |10.0.0.128/32     |ROUTE| Et19               |1016 |103431  | 60:53:75:13:ba:d8 |  -  |183624|   -   
|0  |10.0.0.131/32     |ROUTE| Et19               |1016 |103431  | 60:53:75:13:ba:d8 |16385|183527|   -   
|0  |10.0.0.131/32     |ROUTE| Et1                |1007 |103422  | 68:bf:6c:35:1e:31 |16385|183528|   -   
|0  |10.0.0.131/32     |ROUTE| Et3                |1008 |103427  | bc:31:e2:e1:ec:2c |16385|183529|   -   
|0  |10.0.0.131/32     |ROUTE| Et9                |1009 |103423  | e0:9b:27:c4:c5:84 |16385|183530|   -   
|0  |10.0.0.131/32     |ROUTE| Et13               |1010 |103426  | 5c:07:58:a3:0a:aa |16385|183531|   -   
|0  |10.0.0.131/32     |ROUTE| Et2                |1014 |103425  | d4:af:f7:2f:13:96 |16385|183532|   -   
|0  |10.0.0.131/32     |ROUTE| Et12               |1011 |103424  | 58:70:7f:9f:c4:03 |16385|183533|   -   
|0  |10.0.0.131/32     |ROUTE| Et17               |1012 |103430  | 64:6d:4e:32:e1:22 |16385|183534|   -   
|0  |10.0.0.175/32     |ROUTE| Et19               |1016 |103431  | 60:53:75:13:ba:d8 |16385|183527|   -   
|0  |10.0.0.175/32     |ROUTE| Et1                |1007 |103422  | 68:bf:6c:35:1e:31 |16385|183528|   -   
|0  |10.0.0.175/32     |ROUTE| Et3                |1008 |103427  | bc:31:e2:e1:ec:2c |16385|183529|   -   
|0  |10.0.0.175/32     |ROUTE| Et9                |1009 |103423  | e0:9b:27:c4:c5:84 |16385|183530|   -   
|0  |10.0.0.175/32     |ROUTE| Et13               |1010 |103426  | 5c:07:58:a3:0a:aa |16385|183531|   -   
|0  |10.0.0.175/32     |ROUTE| Et2                |1014 |103425  | d4:af:f7:2f:13:96 |16385|183532|   -   
|0  |10.0.0.175/32     |ROUTE| Et12               |1011 |103424  | 58:70:7f:9f:c4:03 |16385|183533|   -   
|0  |10.0.0.175/32     |ROUTE| Et17               |1012 |103430  | 64:6d:4e:32:e1:22 |16385|183534|   -   
|0  |10.0.0.179/32     |ROUTE| Et40               |1013 |103432  | e8:24:a6:96:05:48 |  -  |183548|   -   
|0  |10.0.0.184/32     |ROUTE| Et19               |1016 |103431  | 60:53:75:13:ba:d8 |16385|183527|   -   
|0  |10.0.0.184/32     |ROUTE| Et1                |1007 |103422  | 68:bf:6c:35:1e:31 |16385|183528|   -   
|0  |10.0.0.184/32     |ROUTE| Et3                |1008 |103427  | bc:31:e2:e1:ec:2c |16385|183529|   -   
|0  |10.0.0.184/32     |ROUTE| Et9                |1009 |103423  | e0:9b:27:c4:c5:84 |16385|183530|   -   
|0  |10.0.0.184/32     |ROUTE| Et13               |1010 |103426  | 5c:07:58:a3:0a:aa |16385|183531|   -   
|0  |10.0.0.184/32     |ROUTE| Et2                |1014 |103425  | d4:af:f7:2f:13:96 |16385|183532|   -   
|0  |10.0.0.184/32     |ROUTE| Et12               |1011 |103424  | 58:70:7f:9f:c4:03 |16385|183533|   -   
|0  |10.0.0.184/32     |ROUTE| Et17               |1012 |103430  | 64:6d:4e:32:e1:22 |16385|183534|   -   
|0  |10.0.0.214/32     |ROUTE| Et5                |1006 |103421  | 18:5b:00:61:ac:6f |  -  |183568|   -   
|0  |10.0.0.216/32     |ROUTE| Et5                |1006 |103421  | 18:5b:00:61:ac:6f |  -  |183568|   -   
|0  |10.0.0.217/32     |ROUTE| Et4                |1018 |103429  | c0:14:b8:21:97:90 |  -  |183547|   -   
|0  |10.0.0.221/32     |ROUTE| Et15               |1015 |103428  | 30:c5:07:84:3e:79 |  -  |183510|   -   
|0  |20.30.31.0/32     |TRAP | CoppSystemIpBcast  |0    |  -     | BcastReceive      |  -  |314666|   -   
|0  |20.30.31.30/32    |TRAP | CoppSystemIpUcast  |0    |  -     | Receive           |  -  |314667|   -   
|0  |20.30.31.31/32    |ROUTE| Et1                |1007 |103422  | 68:bf:6c:35:1e:31 |  -  |183506|   -   
|0  |20.30.31.255/32   |TRAP | CoppSystemIpBcast  |0    |  -     | BcastReceive      |  -  |314666|   -   
|0  |20.30.31.0/24     |TRAP | CoppSystemL3DstMiss|1007 |1007    | ArpTrap           |  -  |315678|   -   
|0  |20.30.32.0/32     |TRAP | CoppSystemIpBcast  |0    |  -     | BcastReceive      |  -  |314666|   -   
|0  |20.30.32.30/32    |TRAP | CoppSystemIpUcast  |0    |  -     | Receive           |  -  |314667|   -   
|0  |20.30.32.32/32    |ROUTE| Et2                |1014 |103425  | d4:af:f7:2f:13:96 |  -  |183512|   -   
|0  |20.30.32.255/32   |TRAP | CoppSystemIpBcast  |0    |  -     | BcastReceive      |  -  |314666|   -   
|0  |20.30.32.0/24     |TRAP | CoppSystemL3DstMiss|1014 |1014    | ArpTrap           |  -  |315685|   -   
|0  |20.30.53.0/32     |TRAP | CoppSystemIpBcast  |0    |  -     | BcastReceive      |  -  |314666|   -   
|0  |20.30.53.30/32    |TRAP | CoppSystemIpUcast  |0    |  -     | Receive           |  -  |314667|   -   
|0  |20.30.53.53/32    |ROUTE| Et13               |1010 |103426  | 5c:07:58:a3:0a:aa |  -  |183515|   -   
|0  |20.30.53.255/32   |TRAP | CoppSystemIpBcast  |0    |  -     | BcastReceive      |  -  |314666|   -   
|0  |20.30.53.0/24     |TRAP | CoppSystemL3DstMiss|1010 |1010    | ArpTrap           |  -  |315681|   -   
|0  |20.30.72.0/32     |TRAP | CoppSystemIpBcast  |0    |  -     | BcastReceive      |  -  |314666|   -   
|0  |20.30.72.30/32    |TRAP | CoppSystemIpUcast  |0    |  -     | Receive           |  -  |314667|   -   
|0  |20.30.72.72/32    |ROUTE| Et9                |1009 |103423  | e0:9b:27:c4:c5:84 |  -  |183507|   -   
|0  |20.30.72.255/32   |TRAP | CoppSystemIpBcast  |0    |  -     | BcastReceive      |  -  |314666|   -   
|0  |20.30.72.0/24     |TRAP | CoppSystemL3DstMiss|1009 |1009    | ArpTrap           |  -  |315680|   -   
|0  |20.30.84.0/32     |TRAP | CoppSystemIpBcast  |0    |  -     | BcastReceive      |  -  |314666|   -   
|0  |20.30.84.30/32    |TRAP | CoppSystemIpUcast  |0    |  -     | Receive           |  -  |314667|   -   
|0  |20.30.84.84/32    |ROUTE| Et12               |1011 |103424  | 58:70:7f:9f:c4:03 |  -  |183509|   -   
|0  |20.30.84.255/32   |TRAP | CoppSystemIpBcast  |0    |  -     | BcastReceive      |  -  |314666|   -   
|0  |20.30.84.0/24     |TRAP | CoppSystemL3DstMiss|1011 |1011    | ArpTrap           |  -  |315682|   -   
|0  |20.30.120.0/32    |TRAP | CoppSystemIpBcast  |0    |  -     | BcastReceive      |  -  |314666|   -   
|0  |20.30.120.30/32   |TRAP | CoppSystemIpUcast  |0    |  -     | Receive           |  -  |314667|   -   
|0  |20.30.120.120/32  |ROUTE| Et3                |1008 |103427  | bc:31:e2:e1:ec:2c |  -  |183554|   -   
|0  |20.30.120.255/32  |TRAP | CoppSystemIpBcast  |0    |  -     | BcastReceive      |  -  |314666|   -   
|0  |20.30.120.0/24    |TRAP | CoppSystemL3DstMiss|1008 |1008    | ArpTrap           |  -  |315679|   -   
|0  |20.30.124.0/32    |TRAP | CoppSystemIpBcast  |0    |  -     | BcastReceive      |  -  |314666|   -   
|0  |20.30.124.30/32   |TRAP | CoppSystemIpUcast  |0    |  -     | Receive           |  -  |314667|   -   
|0  |20.30.124.124/32  |ROUTE| Et17               |1012 |103430  | 64:6d:4e:32:e1:22 |  -  |183545|   -   
|0  |20.30.124.255/32  |TRAP | CoppSystemIpBcast  |0    |  -     | BcastReceive      |  -  |314666|   -   
|0  |20.30.124.0/24    |TRAP | CoppSystemL3DstMiss|1012 |1012    | ArpTrap           |  -  |315683|   -   
|0  |20.30.128.0/32    |TRAP | CoppSystemIpBcast  |0    |  -     | BcastReceive      |  -  |314666|   -   
|0  |20.30.128.30/32   |TRAP | CoppSystemIpUcast  |0    |  -     | Receive           |  -  |314667|   -   
|0  |20.30.128.128/32  |ROUTE| Et19               |1016 |103431  | 60:53:75:13:ba:d8 |  -  |183521|   -   
|0  |20.30.128.255/32  |TRAP | CoppSystemIpBcast  |0    |  -     | BcastReceive      |  -  |314666|   -   
|0  |20.30.128.0/24    |TRAP | CoppSystemL3DstMiss|1016 |1016    | ArpTrap           |  -  |315687|   -   
|0  |20.30.179.0/32    |TRAP | CoppSystemIpBcast  |0    |  -     | BcastReceive      |  -  |314666|   -   
|0  |20.30.179.30/32   |TRAP | CoppSystemIpUcast  |0    |  -     | Receive           |  -  |314667|   -   
|0  |20.30.179.179/32  |ROUTE| Et40               |1013 |103432  | e8:24:a6:96:05:48 |  -  |183540|   -   
|0  |20.30.179.255/32  |TRAP | CoppSystemIpBcast  |0    |  -     | BcastReceive      |  -  |314666|   -   
|0  |20.30.179.0/24    |TRAP | CoppSystemL3DstMiss|1013 |1013    | ArpTrap           |  -  |315684|   -   
|0  |20.30.184.0/32    |TRAP | CoppSystemIpBcast  |0    |  -     | BcastReceive      |  -  |314666|   -   
|0  |20.30.184.30/32   |TRAP | CoppSystemIpUcast  |0    |  -     | Receive           |  -  |314667|   -   
|0  |20.30.184.255/32  |TRAP | CoppSystemIpBcast  |0    |  -     | BcastReceive      |  -  |314666|   -   
|0  |20.30.184.0/24    |TRAP | CoppSystemL3DstMiss|1017 |1017    | ArpTrap           |  -  |315688|   -   
|0  |20.30.214.0/32    |TRAP | CoppSystemIpBcast  |0    |  -     | BcastReceive      |  -  |314666|   -   
|0  |20.30.214.30/32   |TRAP | CoppSystemIpUcast  |0    |  -     | Receive           |  -  |314667|   -   
|0  |20.30.214.214/32  |ROUTE| Et5                |1006 |103421  | 18:5b:00:61:ac:6f |  -  |183504|   -   
|0  |20.30.214.255/32  |TRAP | CoppSystemIpBcast  |0    |  -     | BcastReceive      |  -  |314666|   -   
|0  |20.30.214.0/24    |TRAP | CoppSystemL3DstMiss|1006 |1006    | ArpTrap           |  -  |315677|   -   
|0  |20.30.217.0/32    |TRAP | CoppSystemIpBcast  |0    |  -     | BcastReceive      |  -  |314666|   -   
|0  |20.30.217.30/32   |TRAP | CoppSystemIpUcast  |0    |  -     | Receive           |  -  |314667|   -   
|0  |20.30.217.217/32  |ROUTE| Et4                |1018 |103429  | c0:14:b8:21:97:90 |  -  |183508|   -   
|0  |20.30.217.255/32  |TRAP | CoppSystemIpBcast  |0    |  -     | BcastReceive      |  -  |314666|   -   
|0  |20.30.217.0/24    |TRAP | CoppSystemL3DstMiss|1018 |1018    | ArpTrap           |  -  |315689|   -   
|0  |20.30.221.0/32    |TRAP | CoppSystemIpBcast  |0    |  -     | BcastReceive      |  -  |314666|   -   
|0  |20.30.221.30/32   |TRAP | CoppSystemIpUcast  |0    |  -     | Receive           |  -  |314667|   -   
|0  |20.30.221.221/32  |ROUTE| Et15               |1015 |103428  | 30:c5:07:84:3e:79 |  -  |183523|   -   
|0  |20.30.221.255/32  |TRAP | CoppSystemIpBcast  |0    |  -     | BcastReceive      |  -  |314666|   -   
|0  |20.30.221.0/24    |TRAP | CoppSystemL3DstMiss|1015 |1015    | ArpTrap           |  -  |315686|   -   
|0  |20.31.175.0/24    |ROUTE| Et1                |1007 |103422  | 68:bf:6c:35:1e:31 |  -  |183511|   -   
|0  |20.32.175.0/24    |ROUTE| Et2                |1014 |103425  | d4:af:f7:2f:13:96 |  -  |183524|   -   
|0  |20.53.175.0/24    |ROUTE| Et13               |1010 |103426  | 5c:07:58:a3:0a:aa |  -  |183607|   -   
|0  |20.72.175.0/24    |ROUTE| Et9                |1009 |103423  | e0:9b:27:c4:c5:84 |  -  |183558|   -   
|0  |20.84.175.0/24    |ROUTE| Et19               |1016 |103431  | 60:53:75:13:ba:d8 |16385|183527|   -   
|0  |20.84.175.0/24    |ROUTE| Et1                |1007 |103422  | 68:bf:6c:35:1e:31 |16385|183528|   -   
|0  |20.84.175.0/24    |ROUTE| Et3                |1008 |103427  | bc:31:e2:e1:ec:2c |16385|183529|   -   
|0  |20.84.175.0/24    |ROUTE| Et9                |1009 |103423  | e0:9b:27:c4:c5:84 |16385|183530|   -   
|0  |20.84.175.0/24    |ROUTE| Et13               |1010 |103426  | 5c:07:58:a3:0a:aa |16385|183531|   -   
|0  |20.84.175.0/24    |ROUTE| Et2                |1014 |103425  | d4:af:f7:2f:13:96 |16385|183532|   -   
|0  |20.84.175.0/24    |ROUTE| Et12               |1011 |103424  | 58:70:7f:9f:c4:03 |16385|183533|   -   
|0  |20.84.175.0/24    |ROUTE| Et17               |1012 |103430  | 64:6d:4e:32:e1:22 |16385|183534|   -   
|0  |20.120.175.0/24   |ROUTE| Et3                |1008 |103427  | bc:31:e2:e1:ec:2c |  -  |183513|   -   
|0  |20.120.214.0/24   |ROUTE| Et3                |1008 |103427  | bc:31:e2:e1:ec:2c |  -  |183513|   -   
|0  |20.124.175.0/24   |ROUTE| Et17               |1012 |103430  | 64:6d:4e:32:e1:22 |  -  |183543|   -   
|0  |20.128.175.0/24   |ROUTE| Et19               |1016 |103431  | 60:53:75:13:ba:d8 |  -  |183624|   -   
|0  |20.131.175.0/24   |ROUTE| Et19               |1016 |103431  | 60:53:75:13:ba:d8 |16385|183527|   -   
|0  |20.131.175.0/24   |ROUTE| Et1                |1007 |103422  | 68:bf:6c:35:1e:31 |16385|183528|   -   
|0  |20.131.175.0/24   |ROUTE| Et3                |1008 |103427  | bc:31:e2:e1:ec:2c |16385|183529|   -   
|0  |20.131.175.0/24   |ROUTE| Et9                |1009 |103423  | e0:9b:27:c4:c5:84 |16385|183530|   -   
|0  |20.131.175.0/24   |ROUTE| Et13               |1010 |103426  | 5c:07:58:a3:0a:aa |16385|183531|   -   
|0  |20.131.175.0/24   |ROUTE| Et2                |1014 |103425  | d4:af:f7:2f:13:96 |16385|183532|   -   
|0  |20.131.175.0/24   |ROUTE| Et12               |1011 |103424  | 58:70:7f:9f:c4:03 |16385|183533|   -   
|0  |20.131.175.0/24   |ROUTE| Et17               |1012 |103430  | 64:6d:4e:32:e1:22 |16385|183534|   -   
|0  |20.175.179.0/24   |ROUTE| Et40               |1013 |103432  | e8:24:a6:96:05:48 |  -  |183548|   -   
|0  |20.175.184.0/24   |ROUTE| Et19               |1016 |103431  | 60:53:75:13:ba:d8 |16385|183527|   -   
|0  |20.175.184.0/24   |ROUTE| Et1                |1007 |103422  | 68:bf:6c:35:1e:31 |16385|183528|   -   
|0  |20.175.184.0/24   |ROUTE| Et3                |1008 |103427  | bc:31:e2:e1:ec:2c |16385|183529|   -   
|0  |20.175.184.0/24   |ROUTE| Et9                |1009 |103423  | e0:9b:27:c4:c5:84 |16385|183530|   -   
|0  |20.175.184.0/24   |ROUTE| Et13               |1010 |103426  | 5c:07:58:a3:0a:aa |16385|183531|   -   
|0  |20.175.184.0/24   |ROUTE| Et2                |1014 |103425  | d4:af:f7:2f:13:96 |16385|183532|   -   
|0  |20.175.184.0/24   |ROUTE| Et12               |1011 |103424  | 58:70:7f:9f:c4:03 |16385|183533|   -   
|0  |20.175.184.0/24   |ROUTE| Et17               |1012 |103430  | 64:6d:4e:32:e1:22 |16385|183534|   -   
|0  |20.175.214.0/24   |ROUTE| Et5                |1006 |103421  | 18:5b:00:61:ac:6f |  -  |183568|   -   
|0  |20.175.217.0/24   |ROUTE| Et4                |1018 |103429  | c0:14:b8:21:97:90 |  -  |183547|   -   
|0  |20.175.221.0/24   |ROUTE| Et15               |1015 |103428  | 30:c5:07:84:3e:79 |  -  |183510|   -   
|0  |20.214.216.0/24   |ROUTE| Et5                |1006 |103421  | 18:5b:00:61:ac:6f |  -  |183568|   -   
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
|2  |50.10.31.0/24     |ROUTE| FEC 183602         |0    |2097149 | 00:00:00:00:00:00 |  -  |131074|M 362145
|2  |50.10.32.0/24     |ROUTE| FEC 183544         |0    |2097150 | 00:00:00:00:00:00 |  -  |131072|M 378528
|2  |50.10.53.0/24     |ROUTE| FEC 183546         |0    |2097141 | 00:00:00:00:00:00 |  -  |131076|M 970000
|2  |50.10.72.0/24     |ROUTE| FEC 183538         |0    |2097147 | 00:00:00:00:00:00 |  -  |131075|M 62002
|2  |50.10.84.0/24     |ROUTE| FEC 183535         |0    |2097140 | 00:00:00:00:00:00 |  -  |131073|M 20084 720896
|2  |50.10.120.0/24    |ROUTE| FEC 183516         |0    |2097144 | 00:00:00:00:00:00 |  -  |131078|M 1277
|2  |50.10.131.0/24    |ROUTE| FEC 16387          |0    |2097151 | 00:00:00:00:00:00 |  -  |131080|M 18
|2  |50.10.179.0/24    |ROUTE| FEC 183552         |0    |2097145 | 00:00:00:00:00:00 |  -  |131077|M 16
|2  |50.10.214.0/24    |ROUTE| FEC 183601         |0    |2097142 | 00:00:00:00:00:00 |  -  |131079|M 20214 500000
|2  |50.10.217.0/24    |ROUTE| FEC 183537         |0    |2097146 | 00:00:00:00:00:00 |  -  |131083|M 20217 524287
|2  |50.10.221.0/24    |ROUTE| FEC 183625         |0    |2097143 | 00:00:00:00:00:00 |  -  |131081|M 524289
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
|16384|183560|ROUTE| Et12               |1011 |103433  | 58:70:7f:9f:c4:03 |Mswap 20484
|16384|183561|ROUTE| Et13               |1010 |103434  | 5c:07:58:a3:0a:aa |Mswap 20484
|16384|183562|ROUTE| Et1                |1007 |103435  | 68:bf:6c:35:1e:31 |Mswap 20484
|16384|183563|ROUTE| Et9                |1009 |103436  | e0:9b:27:c4:c5:84 |Mswap 20484
|16384|183564|ROUTE| Et19               |1016 |103438  | 60:53:75:13:ba:d8 |Mswap 20484
|16384|183565|ROUTE| Et3                |1008 |103441  | bc:31:e2:e1:ec:2c |Mswap 20484
|16384|183566|ROUTE| Et2                |1014 |103442  | d4:af:f7:2f:13:96 |Mswap 20484
|16385|183527|ROUTE| Et19               |1016 |103431  | 60:53:75:13:ba:d8 |   -   
|16385|183528|ROUTE| Et1                |1007 |103422  | 68:bf:6c:35:1e:31 |   -   
|16385|183529|ROUTE| Et3                |1008 |103427  | bc:31:e2:e1:ec:2c |   -   
|16385|183530|ROUTE| Et9                |1009 |103423  | e0:9b:27:c4:c5:84 |   -   
|16385|183531|ROUTE| Et13               |1010 |103426  | 5c:07:58:a3:0a:aa |   -   
|16385|183532|ROUTE| Et2                |1014 |103425  | d4:af:f7:2f:13:96 |   -   
|16385|183533|ROUTE| Et12               |1011 |103424  | 58:70:7f:9f:c4:03 |   -   
|16385|183534|ROUTE| Et17               |1012 |103430  | 64:6d:4e:32:e1:22 |   -   
|16387|183626|ROUTE| Et19               |1016 |103448  | 60:53:75:13:ba:d8 |Mpush 20131
|16387|183627|ROUTE| Et17               |1012 |103449  | 64:6d:4e:32:e1:22 |Mpush 2131
|16387|183628|ROUTE| Et13               |1010 |103450  | 5c:07:58:a3:0a:aa |Mpush 20131
|16387|183629|ROUTE| Et2                |1014 |103451  | d4:af:f7:2f:13:96 |Mpush 20131
|16387|183630|ROUTE| Et9                |1009 |103452  | e0:9b:27:c4:c5:84 |Mpush 20131
|16387|183631|ROUTE| Et1                |1007 |103453  | 68:bf:6c:35:1e:31 |Mpush 20131
|16387|183632|ROUTE| Et12               |1011 |103437  | 58:70:7f:9f:c4:03 |Mpush 20131
|16387|183633|ROUTE| Et3                |1008 |103455  | bc:31:e2:e1:ec:2c |Mpush 20131
|16389|183642|ROUTE| Et2                |1014 |103464  | d4:af:f7:2f:13:96 |Mswap 20175
|16389|183643|ROUTE| Et19               |1016 |103465  | 60:53:75:13:ba:d8 |Mswap 20175
|16389|183644|ROUTE| Et3                |1008 |103466  | bc:31:e2:e1:ec:2c |Mswap 20175
|16389|183645|ROUTE| Et9                |1009 |103467  | e0:9b:27:c4:c5:84 |Mswap 20175
|16389|183646|ROUTE| Et13               |1010 |103468  | 5c:07:58:a3:0a:aa |Mswap 20175
|16389|183647|ROUTE| Et17               |1012 |103469  | 64:6d:4e:32:e1:22 |Mswap 2175
|16389|183648|ROUTE| Et12               |1011 |103439  | 58:70:7f:9f:c4:03 |Mswap 20175
|16389|183649|ROUTE| Et1                |1007 |103471  | 68:bf:6c:35:1e:31 |Mswap 20175
|16390|183569|ROUTE| Et12               |1011 |103440  | 58:70:7f:9f:c4:03 |Mswap 20131
|16390|183570|ROUTE| Et3                |1008 |103474  | bc:31:e2:e1:ec:2c |Mswap 20131
|16390|183571|ROUTE| Et9                |1009 |103475  | e0:9b:27:c4:c5:84 |Mswap 20131
|16390|183572|ROUTE| Et1                |1007 |103476  | 68:bf:6c:35:1e:31 |Mswap 20131
|16390|183573|ROUTE| Et17               |1012 |103477  | 64:6d:4e:32:e1:22 |Mswap 2131
|16390|183574|ROUTE| Et2                |1014 |103478  | d4:af:f7:2f:13:96 |Mswap 20131
|16390|183575|ROUTE| Et13               |1010 |103479  | 5c:07:58:a3:0a:aa |Mswap 20131
|16390|183576|ROUTE| Et19               |1016 |103480  | 60:53:75:13:ba:d8 |Mswap 20131
|  -  |131072|ROUTE| FEC 183544         |   - |2097150 |                 - |Mpush 378528
|  -  |131073|ROUTE| FEC 183535         |   - |2097140 |                 - |Mpush 20084 720896
|  -  |131074|ROUTE| FEC 183602         |   - |2097149 |                 - |Mpush 362145
|  -  |131075|ROUTE| FEC 183538         |   - |2097147 |                 - |Mpush 62002
|  -  |131076|ROUTE| FEC 183546         |   - |2097141 |                 - |Mpush 970000
|  -  |131077|ROUTE| FEC 183552         |   - |2097145 |                 - |Mpush 16
|  -  |131078|ROUTE| FEC 183516         |   - |2097144 |                 - |Mpush 1277
|  -  |131079|ROUTE| FEC 183601         |   - |2097142 |                 - |Mpush 20214 500000
|  -  |131080|ROUTE| FEC 16387          |   - |2097151 |                 - |Mpush 18
|  -  |131081|ROUTE| FEC 183625         |   - |2097143 |                 - |Mpush 524289
|  -  |131082|ROUTE| FEC 183546         |   - |  -     |                   |   -   
|  -  |131083|ROUTE| FEC 183537         |   - |2097146 |                 - |Mpush 20217 524287
|  -  |131084|ROUTE| FEC 183539         |   - |  -     |                   |   -   
|  -  |183502|DROP | DROP               |0    |  -     |                   |   -   
|  -  |183503|DROP | DROP               |0    |  -     |                   |   -   
|  -  |183504|ROUTE| Et5                |1006 |103421  | 18:5b:00:61:ac:6f |   -   
|  -  |183505|DROP | DROP               |0    |  -     |                   |   -   
|  -  |183506|ROUTE| Et1                |1007 |103422  | 68:bf:6c:35:1e:31 |   -   
|  -  |183507|ROUTE| Et9                |1009 |103423  | e0:9b:27:c4:c5:84 |   -   
|  -  |183508|ROUTE| Et4                |1018 |103429  | c0:14:b8:21:97:90 |   -   
|  -  |183509|ROUTE| Et12               |1011 |103424  | 58:70:7f:9f:c4:03 |   -   
|  -  |183510|ROUTE| Et15               |1015 |103428  | 30:c5:07:84:3e:79 |   -   
|  -  |183511|ROUTE| Et1                |1007 |103422  | 68:bf:6c:35:1e:31 |   -   
|  -  |183512|ROUTE| Et2                |1014 |103425  | d4:af:f7:2f:13:96 |   -   
|  -  |183513|ROUTE| Et3                |1008 |103427  | bc:31:e2:e1:ec:2c |   -   
|  -  |183514|ROUTE| Et15               |1015 |103428  | 30:c5:07:84:3e:79 |   -   
|  -  |183515|ROUTE| Et13               |1010 |103426  | 5c:07:58:a3:0a:aa |   -   
|  -  |183516|ROUTE| Et3                |1008 |103427  | bc:31:e2:e1:ec:2c |   -   
|  -  |183521|ROUTE| Et19               |1016 |103431  | 60:53:75:13:ba:d8 |   -   
|  -  |183522|ROUTE| Et3                |1008 |103427  | bc:31:e2:e1:ec:2c |   -   
|  -  |183523|ROUTE| Et15               |1015 |103428  | 30:c5:07:84:3e:79 |   -   
|  -  |183524|ROUTE| Et2                |1014 |103425  | d4:af:f7:2f:13:96 |   -   
|  -  |183525|ROUTE| Et12               |1011 |103424  | 58:70:7f:9f:c4:03 |   -   
|  -  |183526|ROUTE| Et2                |1014 |103425  | d4:af:f7:2f:13:96 |   -   
|  -  |183535|ROUTE| Et12               |1011 |103424  | 58:70:7f:9f:c4:03 |   -   
|  -  |183536|ROUTE| Et17               |1012 |103430  | 64:6d:4e:32:e1:22 |   -   
|  -  |183537|ROUTE| Et4                |1018 |103429  | c0:14:b8:21:97:90 |   -   
|  -  |183538|ROUTE| Et9                |1009 |103423  | e0:9b:27:c4:c5:84 |   -   
|  -  |183539|ROUTE| Et17               |1012 |103490  | 64:6d:4e:32:e1:22 |Mpush 2124
|  -  |183540|ROUTE| Et40               |1013 |103432  | e8:24:a6:96:05:48 |   -   
|  -  |183541|ROUTE| Et40               |1013 |103432  | e8:24:a6:96:05:48 |   -   
|  -  |183542|ROUTE| Et9                |1009 |103423  | e0:9b:27:c4:c5:84 |   -   
|  -  |183543|ROUTE| Et17               |1012 |103430  | 64:6d:4e:32:e1:22 |   -   
|  -  |183544|ROUTE| Et2                |1014 |103425  | d4:af:f7:2f:13:96 |   -   
|  -  |183545|ROUTE| Et17               |1012 |103430  | 64:6d:4e:32:e1:22 |   -   
|  -  |183546|ROUTE| Et13               |1010 |103473  | 5c:07:58:a3:0a:aa |Mpush 0
|  -  |183547|ROUTE| Et4                |1018 |103429  | c0:14:b8:21:97:90 |   -   
|  -  |183548|ROUTE| Et40               |1013 |103432  | e8:24:a6:96:05:48 |   -   
|  -  |183549|ROUTE| Et2                |1014 |103425  | d4:af:f7:2f:13:96 |   -   
|  -  |183550|ROUTE| Et12               |1011 |103424  | 58:70:7f:9f:c4:03 |   -   
|  -  |183552|ROUTE| Et40               |1013 |103432  | e8:24:a6:96:05:48 |   -   
|  -  |183554|ROUTE| Et3                |1008 |103427  | bc:31:e2:e1:ec:2c |   -   
|  -  |183555|DROP | DROP               |0    |  -     |                   |   -   
|  -  |183556|ROUTE| Et3                |1008 |103427  | bc:31:e2:e1:ec:2c |   -   
|  -  |183557|ROUTE| Et3                |1008 |103427  | bc:31:e2:e1:ec:2c |   -   
|  -  |183558|ROUTE| Et9                |1009 |103423  | e0:9b:27:c4:c5:84 |   -   
|  -  |183559|ROUTE| Et2                |1014 |103425  | d4:af:f7:2f:13:96 |   -   
|  -  |183567|ROUTE| Et12               |1011 |103424  | 58:70:7f:9f:c4:03 |   -   
|  -  |183568|ROUTE| Et5                |1006 |103421  | 18:5b:00:61:ac:6f |   -   
|  -  |183599|ROUTE| Et19               |1016 |103431  | 60:53:75:13:ba:d8 |   -   
|  -  |183600|ROUTE| Et1                |1007 |103422  | 68:bf:6c:35:1e:31 |   -   
|  -  |183601|ROUTE| Et5                |1006 |103421  | 18:5b:00:61:ac:6f |   -   
|  -  |183602|ROUTE| Et1                |1007 |103422  | 68:bf:6c:35:1e:31 |   -   
|  -  |183603|ROUTE| Et1                |1007 |103422  | 68:bf:6c:35:1e:31 |   -   
|  -  |183604|ROUTE| Et4                |1018 |103429  | c0:14:b8:21:97:90 |   -   
|  -  |183605|ROUTE| Et19               |1016 |103431  | 60:53:75:13:ba:d8 |   -   
|  -  |183606|ROUTE| Et5                |1006 |103421  | 18:5b:00:61:ac:6f |   -   
|  -  |183607|ROUTE| Et13               |1010 |103426  | 5c:07:58:a3:0a:aa |   -   
|  -  |183608|ROUTE| Et13               |1010 |103426  | 5c:07:58:a3:0a:aa |   -   
|  -  |183624|ROUTE| Et19               |1016 |103431  | 60:53:75:13:ba:d8 |   -   
|  -  |183625|ROUTE| Et15               |1015 |103428  | 30:c5:07:84:3e:79 |   -   
|  -  |314666|TRAP | CoppSystemIpBcast  |0    |  -     | BcastReceive      |   -   
|  -  |314667|TRAP | CoppSystemIpUcast  |0    |  -     | Receive           |   -   
|  -  |314669|TRAP | CoppSystemL3LpmOver|0    |  -     | SlowReceive       |   -   
|  -  |314671|TRAP | CoppSystemL3DstMiss|0    |  -     | ArpTrap           |   -   
|  -  |315677|TRAP | CoppSystemL3DstMiss|1006 |1006    | ArpTrap           |   -   
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
|  -  |315688|TRAP | CoppSystemL3DstMiss|1017 |1017    | ArpTrap           |   -   
|  -  |315689|TRAP | CoppSystemL3DstMiss|1018 |1018    | ArpTrap           |   -   

```

