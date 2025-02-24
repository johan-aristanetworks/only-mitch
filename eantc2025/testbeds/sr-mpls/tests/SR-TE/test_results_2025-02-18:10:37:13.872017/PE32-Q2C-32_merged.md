# Test results for PE32-Q2C-32

## show version

```text
Arista DCS-7280SR3K-48YC8-F
Hardware version: 10.05
Serial number: JAS20300015
Hardware MAC address: d4af.f72f.1396
System MAC address: d4af.f72f.1396

Software image version: 4.33.1.1F
Architecture: x86_64
Internal build version: 4.33.1.1F-40155285.43311F
Internal build ID: 2170da2c-90c5-421e-adc1-86266708cffc
Image format version: 3.0
Image optimization: Default

Uptime: 1 day, 3 hours and 44 minutes
Total memory: 65734472 kB
Free memory: 61859000 kB

```

## show lldp neighbors

```text
Last table change time   : 0:57:40 ago
Number of table inserts  : 8
Number of table deletes  : 4
Number of table drops    : 0
Number of table age-outs : 0

Port          Neighbor Device ID                      Neighbor Port ID    TTL
---------- --------------------------------------- ---------------------- ---
Et1           Arista-Spine3-Q2A-30.ns.eantc.de        Ethernet2           120
Et5           Juniper-175-ACX7100-48L                 509                 120
Et40          Arista-Harness3-JP-39.ns.eantc.de       Ethernet2           120
Ma1           extreme-x460-2                          2                   120

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
Interface        IP Address           Status     Protocol         MTU   Owner  
---------------- -------------------- ---------- ------------ --------- -------
Ethernet1        20.30.32.32/24       up         up              1500          
Ethernet5        20.32.175.32/24      up         up              1500          
Ethernet40.4     50.10.32.1/24        up         up              1500          
Loopback0        10.0.0.32/32         up         up             65535          
Management1      192.168.20.32/23     up         up              1500          

```

## show interfaces counters rates | nz

```text
Port      Name                Intvl  In Mbps      %  In Kpps Out Mbps      %
Ma1                            0:05      0.0   0.0%        0      0.1   0.0%

Port      Out Kpps
```

## show isis neighbors

```text
 
Instance  VRF      System Id        Type Interface          SNPA              State Hold time   Circuit Id          
IGP       default  Arista-Spine3-Q2A-30 L2   Ethernet1          P2P               UP    24          2C                  
IGP       default  Juniper-175-ACX7100-48L L2   Ethernet5          P2P               UP    23          01                  
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
      Remaining lifetime received: 1199 s Modified to: 1200 s
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
    Arista-PE32-Q2C-32.00-00        20  40455   999    300 L2  0000.0000.0032.00-00  <>
      LSP generation remaining wait time: 0 ms
      Time remaining until refresh: 699 s
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
    0000.0000.0128.00-00         20  22209  1123    290 L2  0000.0000.0128.00-00  <>
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
    Juniper-175-ACX7100-48L.00-00        18  15373   988   1180 L2  0000.0000.0175.00-00  <>
      Remaining lifetime received: 1199 s Modified to: 1200 s
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
      Remaining lifetime received: 1199 s Modified to: 1200 s
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
      Remaining lifetime received: 1199 s Modified to: 1200 s
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
      Remaining lifetime received: 1199 s Modified to: 1200 s
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
      Remaining lifetime received: 1199 s Modified to: 1200 s
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
    221.00-00                     4  61582   637     80 L2  0221.0221.0221.00-00  <>
      Remaining lifetime received: 1199 s Modified to: 1200 s
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
    221.00-01                     3  55699   650     32 L2  0221.0221.0221.00-01  <>
      Remaining lifetime received: 1199 s Modified to: 1200 s
      Hostname: 221
    221.00-02                     5  33627   745    273 L2  0221.0221.0221.00-02  <>
      Remaining lifetime received: 1199 s Modified to: 1200 s
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
  Index     Endpoint          Next Hop/Tunnel Index      Interface    Labels   
--------- ----------------- -------------------------- -------------- ---------
  1         10.0.0.175/32     TI-LFA (3)                 -            [ 3 ]    
  2         10.0.0.84/32      20.30.32.30                Ethernet1    [ 20084 ]
                              20.32.175.175              Ethernet5    [ 20084 ]
  5         10.0.0.30/32      TI-LFA (1)                 -            [ 3 ]    
  6         10.0.0.53/32      20.30.32.30                Ethernet1    [ 20053 ]
                              20.32.175.175              Ethernet5    [ 20053 ]
  7         10.0.0.179/32     20.30.32.30                Ethernet1    [ 20179 ]
                              20.32.175.175              Ethernet5    [ 20179 ]
  8         10.0.0.120/32     TI-LFA (2)                 -            [ 20120 ]
  9         10.0.0.72/32      20.30.32.30                Ethernet1    [ 20072 ]
                              20.32.175.175              Ethernet5    [ 20072 ]
  10        10.0.0.214/32     20.30.32.30                Ethernet1    [ 20214 ]
                              20.32.175.175              Ethernet5    [ 20214 ]
  11        10.0.0.128/32     20.30.32.30                Ethernet1    [ 20128 ]
                              20.32.175.175              Ethernet5    [ 20128 ]
  13        10.0.0.221/32     20.30.32.30                Ethernet1    [ 21221 ]
                              20.32.175.175              Ethernet5    [ 21221 ]
  16        10.0.0.217/32     20.30.32.30                Ethernet1    [ 20217 ]
                              20.32.175.175              Ethernet5    [ 20217 ]

```

## show isis segment-routing prefix-segments

```text

System ID: Arista-PE32-Q2C-32			Instance: 'IGP'
SR supported Data-plane: MPLS			SR Router ID: 10.0.0.32

Node: 12     Proxy-Node: 0      Prefix: 0       Total Segments: 12

Flag Descriptions: R: Re-advertised, N: Node Segment, P: no-PHP
                   E: Explicit-NULL, V: Value, L: Local
Segment status codes: * - Self originated Prefix, L1 - level 1, L2 - level 2, ! - SR-unreachable,
                      # - Some IS-IS next-hops are SR-unreachable
   Prefix                      SID   Label Type       Flags                        System ID       Level Protection  Algorithm   
   ------------------------- ----- ------- ---------- ---------------------------- --------------- ----- ----------- -------------
   10.0.0.30/32                 30   20030 Node       R:0 N:1 P:0 E:0 V:0 L:0      Arista-Spine3-Q2A-30 L2    node        SPF         
*  10.0.0.32/32                 32   20032 Node       R:0 N:1 P:0 E:0 V:0 L:0      Arista-PE32-Q2C-32 L2    unprotected SPF         
   10.0.0.53/32                 53   20053 Node       R:0 N:1 P:1 E:1 V:0 L:0      Arrcus-53       L2    unprotected SPF         
   10.0.0.72/32                 72   20072 Node       R:0 N:1 P:0 E:0 V:0 L:0      Ciena-5134-72   L2    unprotected SPF         
   10.0.0.84/32                 84   20084 Node       R:0 N:1 P:1 E:0 V:0 L:0      Ericsson_84_R6678 L2    unprotected SPF         
   10.0.0.120/32               120   20120 Node       R:0 N:1 P:0 E:0 V:0 L:0      H3C_M1A_120     L2    node        SPF         
   10.0.0.128/32               128   20128 Node       R:0 N:1 P:0 E:0 V:0 L:0      0000.0000.0128  L2    unprotected SPF         
   10.0.0.175/32               175   20175 Node       R:0 N:1 P:0 E:0 V:0 L:0      Juniper-175-ACX7100-48L L2    node        SPF         
   10.0.0.179/32               179   20179 Node       R:0 N:1 P:0 E:0 V:0 L:0      Juniper-179-ACX7024 L2    unprotected SPF         
   10.0.0.214/32               214   20214 Node       R:0 N:1 P:1 E:0 V:0 L:0      Nokia-SXR-214   L2    unprotected SPF         
   10.0.0.217/32               217   20217 Node       R:0 N:1 P:1 E:0 V:0 L:0      Nokia-SR1-217   L2    unprotected SPF         
   10.0.0.221/32              1221  721221 Node       R:0 N:1 P:0 E:0 V:0 L:0      221             L2    unprotected SPF         
```

## show traffic-engineering segment-routing policy

```text
Endpoint 10.0.0.53 Color 100, Counters: not available
	Path group: State: active (for 00:09:10), modified: 00:05:30 ago
		Protocol: Static
		Endpoint provisioning: Static
		Originator: 0.0.0.0(AS0)
		Discriminator: 32769
		Preference: 10
		IGP metric: 0 (static)
		Binding SID: 1004053
		Path computation: Configured
		Explicit null label policy: IPv6 (system default)
		Segment List: State: Valid, ID: 7, Counters: not available
		Protected: Yes
			Label Stack: [20030], Weight: 1
			Resolved Label Stack: [3], Next hop: 20.30.32.30, Interface: Ethernet1
			Backup Resolved Label Stack: [20128 20030 3], Next hop: 20.32.175.175, Interface: Ethernet5
Endpoint 10.0.0.53 Color 101, Counters: not available
	Path group: State: active (for 00:03:39), modified: 00:05:30 ago
		Protocol: Static
		Endpoint provisioning: Static
		Originator: 0.0.0.0(AS0)
		Discriminator: 32769
		Preference: 10
		IGP metric: 0 (static)
		Binding SID: 1006053
		Path computation: Configured
		Explicit null label policy: IPv6 (system default)
		Segment List: State: Valid, ID: 12, Counters: not available
		Protected: Yes
			Label Stack: [20175], Weight: 1
			Resolved Label Stack: [3], Next hop: 20.32.175.175, Interface: Ethernet5
			Backup Resolved Label Stack: [20179 20175 3], Next hop: 20.30.32.30, Interface: Ethernet1
Endpoint 10.0.0.66 Color 100, Counters: not available
	Path group: State: active (for 00:05:30), modified: 00:05:30 ago
		Protocol: Static
		Endpoint provisioning: Static
		Originator: 0.0.0.0(AS0)
		Discriminator: 32769
		Preference: 10
		IGP metric: 0 (static)
		Binding SID: 1004066
		Path computation: Configured
		Explicit null label policy: IPv6 (system default)
		Segment List: State: Valid, ID: 6, Counters: not available
		Protected: Yes
			Label Stack: [20030], Weight: 1
			Resolved Label Stack: [3], Next hop: 20.30.32.30, Interface: Ethernet1
			Backup Resolved Label Stack: [20128 20030 3], Next hop: 20.32.175.175, Interface: Ethernet5
Endpoint 10.0.0.66 Color 101, Counters: not available
	Path group: State: active (for 00:03:39), modified: 00:05:30 ago
		Protocol: Static
		Endpoint provisioning: Static
		Originator: 0.0.0.0(AS0)
		Discriminator: 32769
		Preference: 10
		IGP metric: 0 (static)
		Binding SID: 1006066
		Path computation: Configured
		Explicit null label policy: IPv6 (system default)
		Segment List: State: Valid, ID: 13, Counters: not available
		Protected: Yes
			Label Stack: [20175], Weight: 1
			Resolved Label Stack: [3], Next hop: 20.32.175.175, Interface: Ethernet5
			Backup Resolved Label Stack: [20179 20175 3], Next hop: 20.30.32.30, Interface: Ethernet1
Endpoint 10.0.0.72 Color 100, Counters: not available
	Path group: State: active (for 00:05:30), modified: 00:05:30 ago
		Protocol: Static
		Endpoint provisioning: Static
		Originator: 0.0.0.0(AS0)
		Discriminator: 32769
		Preference: 10
		IGP metric: 0 (static)
		Binding SID: 1004072
		Path computation: Configured
		Explicit null label policy: IPv6 (system default)
		Segment List: State: Valid, ID: 10, Counters: not available
		Protected: Yes
			Label Stack: [20030], Weight: 1
			Resolved Label Stack: [3], Next hop: 20.30.32.30, Interface: Ethernet1
			Backup Resolved Label Stack: [20128 20030 3], Next hop: 20.32.175.175, Interface: Ethernet5
Endpoint 10.0.0.72 Color 101, Counters: not available
	Path group: State: active (for 00:03:39), modified: 00:05:30 ago
		Protocol: Static
		Endpoint provisioning: Static
		Originator: 0.0.0.0(AS0)
		Discriminator: 32769
		Preference: 10
		IGP metric: 0 (static)
		Binding SID: 1006072
		Path computation: Configured
		Explicit null label policy: IPv6 (system default)
		Segment List: State: Valid, ID: 14, Counters: not available
		Protected: Yes
			Label Stack: [20175], Weight: 1
			Resolved Label Stack: [3], Next hop: 20.32.175.175, Interface: Ethernet5
			Backup Resolved Label Stack: [20179 20175 3], Next hop: 20.30.32.30, Interface: Ethernet1
Endpoint 10.0.0.84 Color 100, Counters: not available
	Path group: State: active (for 00:05:30), modified: 00:05:30 ago
		Protocol: Static
		Endpoint provisioning: Static
		Originator: 0.0.0.0(AS0)
		Discriminator: 32769
		Preference: 10
		IGP metric: 0 (static)
		Binding SID: 1004084
		Path computation: Configured
		Explicit null label policy: IPv6 (system default)
		Segment List: State: Valid, ID: 2, Counters: not available
		Protected: Yes
			Label Stack: [20030], Weight: 1
			Resolved Label Stack: [3], Next hop: 20.30.32.30, Interface: Ethernet1
			Backup Resolved Label Stack: [20128 20030 3], Next hop: 20.32.175.175, Interface: Ethernet5
Endpoint 10.0.0.84 Color 101, Counters: not available
	Path group: State: active (for 00:03:39), modified: 00:05:30 ago
		Protocol: Static
		Endpoint provisioning: Static
		Originator: 0.0.0.0(AS0)
		Discriminator: 32769
		Preference: 10
		IGP metric: 0 (static)
		Binding SID: 1006084
		Path computation: Configured
		Explicit null label policy: IPv6 (system default)
		Segment List: State: Valid, ID: 15, Counters: not available
		Protected: Yes
			Label Stack: [20175], Weight: 1
			Resolved Label Stack: [3], Next hop: 20.32.175.175, Interface: Ethernet5
			Backup Resolved Label Stack: [20179 20175 3], Next hop: 20.30.32.30, Interface: Ethernet1
Endpoint 10.0.0.120 Color 100, Counters: not available
	Path group: State: active (for 00:05:30), modified: 00:05:30 ago
		Protocol: Static
		Endpoint provisioning: Static
		Originator: 0.0.0.0(AS0)
		Discriminator: 32769
		Preference: 10
		IGP metric: 0 (static)
		Binding SID: 1004120
		Path computation: Configured
		Explicit null label policy: IPv6 (system default)
		Segment List: State: Valid, ID: 5, Counters: not available
		Protected: Yes
			Label Stack: [20030], Weight: 1
			Resolved Label Stack: [3], Next hop: 20.30.32.30, Interface: Ethernet1
			Backup Resolved Label Stack: [20128 20030 3], Next hop: 20.32.175.175, Interface: Ethernet5
Endpoint 10.0.0.120 Color 101, Counters: not available
	Path group: State: active (for 00:03:39), modified: 00:05:30 ago
		Protocol: Static
		Endpoint provisioning: Static
		Originator: 0.0.0.0(AS0)
		Discriminator: 32769
		Preference: 10
		IGP metric: 0 (static)
		Binding SID: 1006120
		Path computation: Configured
		Explicit null label policy: IPv6 (system default)
		Segment List: State: Valid, ID: 16, Counters: not available
		Protected: Yes
			Label Stack: [20175], Weight: 1
			Resolved Label Stack: [3], Next hop: 20.32.175.175, Interface: Ethernet5
			Backup Resolved Label Stack: [20179 20175 3], Next hop: 20.30.32.30, Interface: Ethernet1
Endpoint 10.0.0.124 Color 100, Counters: not available
	Path group: State: active (for 00:05:30), modified: 00:05:30 ago
		Protocol: Static
		Endpoint provisioning: Static
		Originator: 0.0.0.0(AS0)
		Discriminator: 32769
		Preference: 10
		IGP metric: 0 (static)
		Binding SID: 1004124
		Path computation: Configured
		Explicit null label policy: IPv6 (system default)
		Segment List: State: Valid, ID: 1, Counters: not available
		Protected: Yes
			Label Stack: [20030], Weight: 1
			Resolved Label Stack: [3], Next hop: 20.30.32.30, Interface: Ethernet1
			Backup Resolved Label Stack: [20128 20030 3], Next hop: 20.32.175.175, Interface: Ethernet5
Endpoint 10.0.0.124 Color 101, Counters: not available
	Path group: State: active (for 00:03:39), modified: 00:05:30 ago
		Protocol: Static
		Endpoint provisioning: Static
		Originator: 0.0.0.0(AS0)
		Discriminator: 32769
		Preference: 10
		IGP metric: 0 (static)
		Binding SID: 1006124
		Path computation: Configured
		Explicit null label policy: IPv6 (system default)
		Segment List: State: Valid, ID: 17, Counters: not available
		Protected: Yes
			Label Stack: [20175], Weight: 1
			Resolved Label Stack: [3], Next hop: 20.32.175.175, Interface: Ethernet5
			Backup Resolved Label Stack: [20179 20175 3], Next hop: 20.30.32.30, Interface: Ethernet1
Endpoint 10.0.0.128 Color 100, Counters: not available
	Path group: State: active (for 00:05:30), modified: 00:05:30 ago
		Protocol: Static
		Endpoint provisioning: Static
		Originator: 0.0.0.0(AS0)
		Discriminator: 32769
		Preference: 10
		IGP metric: 0 (static)
		Binding SID: 1004128
		Path computation: Configured
		Explicit null label policy: IPv6 (system default)
		Segment List: State: Valid, ID: 11, Counters: not available
		Protected: Yes
			Label Stack: [20030], Weight: 1
			Resolved Label Stack: [3], Next hop: 20.30.32.30, Interface: Ethernet1
			Backup Resolved Label Stack: [20128 20030 3], Next hop: 20.32.175.175, Interface: Ethernet5
Endpoint 10.0.0.128 Color 101, Counters: not available
	Path group: State: active (for 00:03:39), modified: 00:05:30 ago
		Protocol: Static
		Endpoint provisioning: Static
		Originator: 0.0.0.0(AS0)
		Discriminator: 32769
		Preference: 10
		IGP metric: 0 (static)
		Binding SID: 1006128
		Path computation: Configured
		Explicit null label policy: IPv6 (system default)
		Segment List: State: Valid, ID: 18, Counters: not available
		Protected: Yes
			Label Stack: [20175], Weight: 1
			Resolved Label Stack: [3], Next hop: 20.32.175.175, Interface: Ethernet5
			Backup Resolved Label Stack: [20179 20175 3], Next hop: 20.30.32.30, Interface: Ethernet1
Endpoint 10.0.0.179 Color 100, Counters: not available
	Path group: State: active (for 00:05:30), modified: 00:05:30 ago
		Protocol: Static
		Endpoint provisioning: Static
		Originator: 0.0.0.0(AS0)
		Discriminator: 32769
		Preference: 10
		IGP metric: 0 (static)
		Binding SID: 1004179
		Path computation: Configured
		Explicit null label policy: IPv6 (system default)
		Segment List: State: Valid, ID: 8, Counters: not available
		Protected: Yes
			Label Stack: [20030], Weight: 1
			Resolved Label Stack: [3], Next hop: 20.30.32.30, Interface: Ethernet1
			Backup Resolved Label Stack: [20128 20030 3], Next hop: 20.32.175.175, Interface: Ethernet5
Endpoint 10.0.0.179 Color 101, Counters: not available
	Path group: State: active (for 00:03:39), modified: 00:05:30 ago
		Protocol: Static
		Endpoint provisioning: Static
		Originator: 0.0.0.0(AS0)
		Discriminator: 32769
		Preference: 10
		IGP metric: 0 (static)
		Binding SID: 1006179
		Path computation: Configured
		Explicit null label policy: IPv6 (system default)
		Segment List: State: Valid, ID: 19, Counters: not available
		Protected: Yes
			Label Stack: [20175], Weight: 1
			Resolved Label Stack: [3], Next hop: 20.32.175.175, Interface: Ethernet5
			Backup Resolved Label Stack: [20179 20175 3], Next hop: 20.30.32.30, Interface: Ethernet1
Endpoint 10.0.0.214 Color 100, Counters: not available
	Path group: State: active (for 00:05:30), modified: 00:05:30 ago
		Protocol: Static
		Endpoint provisioning: Static
		Originator: 0.0.0.0(AS0)
		Discriminator: 32769
		Preference: 10
		IGP metric: 0 (static)
		Binding SID: 1004214
		Path computation: Configured
		Explicit null label policy: IPv6 (system default)
		Segment List: State: Valid, ID: 3, Counters: not available
		Protected: Yes
			Label Stack: [20030], Weight: 1
			Resolved Label Stack: [3], Next hop: 20.30.32.30, Interface: Ethernet1
			Backup Resolved Label Stack: [20128 20030 3], Next hop: 20.32.175.175, Interface: Ethernet5
Endpoint 10.0.0.214 Color 101, Counters: not available
	Path group: State: active (for 00:03:39), modified: 00:05:30 ago
		Protocol: Static
		Endpoint provisioning: Static
		Originator: 0.0.0.0(AS0)
		Discriminator: 32769
		Preference: 10
		IGP metric: 0 (static)
		Binding SID: 1006214
		Path computation: Configured
		Explicit null label policy: IPv6 (system default)
		Segment List: State: Valid, ID: 20, Counters: not available
		Protected: Yes
			Label Stack: [20175], Weight: 1
			Resolved Label Stack: [3], Next hop: 20.32.175.175, Interface: Ethernet5
			Backup Resolved Label Stack: [20179 20175 3], Next hop: 20.30.32.30, Interface: Ethernet1
Endpoint 10.0.0.217 Color 100, Counters: not available
	Path group: State: active (for 00:05:30), modified: 00:05:30 ago
		Protocol: Static
		Endpoint provisioning: Static
		Originator: 0.0.0.0(AS0)
		Discriminator: 32769
		Preference: 10
		IGP metric: 0 (static)
		Binding SID: 1004217
		Path computation: Configured
		Explicit null label policy: IPv6 (system default)
		Segment List: State: Valid, ID: 9, Counters: not available
		Protected: Yes
			Label Stack: [20030], Weight: 1
			Resolved Label Stack: [3], Next hop: 20.30.32.30, Interface: Ethernet1
			Backup Resolved Label Stack: [20128 20030 3], Next hop: 20.32.175.175, Interface: Ethernet5
Endpoint 10.0.0.217 Color 101, Counters: not available
	Path group: State: active (for 00:03:39), modified: 00:05:30 ago
		Protocol: Static
		Endpoint provisioning: Static
		Originator: 0.0.0.0(AS0)
		Discriminator: 32769
		Preference: 10
		IGP metric: 0 (static)
		Binding SID: 1006217
		Path computation: Configured
		Explicit null label policy: IPv6 (system default)
		Segment List: State: Valid, ID: 21, Counters: not available
		Protected: Yes
			Label Stack: [20175], Weight: 1
			Resolved Label Stack: [3], Next hop: 20.32.175.175, Interface: Ethernet5
			Backup Resolved Label Stack: [20179 20175 3], Next hop: 20.30.32.30, Interface: Ethernet1
Endpoint 10.0.0.221 Color 100, Counters: not available
	Path group: State: active (for 00:05:30), modified: 00:05:30 ago
		Protocol: Static
		Endpoint provisioning: Static
		Originator: 0.0.0.0(AS0)
		Discriminator: 32769
		Preference: 10
		IGP metric: 0 (static)
		Binding SID: 1004221
		Path computation: Configured
		Explicit null label policy: IPv6 (system default)
		Segment List: State: Valid, ID: 4, Counters: not available
		Protected: Yes
			Label Stack: [20030], Weight: 1
			Resolved Label Stack: [3], Next hop: 20.30.32.30, Interface: Ethernet1
			Backup Resolved Label Stack: [20128 20030 3], Next hop: 20.32.175.175, Interface: Ethernet5
Endpoint 10.0.0.221 Color 101, Counters: not available
	Path group: State: active (for 00:03:39), modified: 00:05:30 ago
		Protocol: Static
		Endpoint provisioning: Static
		Originator: 0.0.0.0(AS0)
		Discriminator: 32769
		Preference: 10
		IGP metric: 0 (static)
		Binding SID: 1006221
		Path computation: Configured
		Explicit null label policy: IPv6 (system default)
		Segment List: State: Valid, ID: 22, Counters: not available
		Protected: Yes
			Label Stack: [20175], Weight: 1
			Resolved Label Stack: [3], Next hop: 20.32.175.175, Interface: Ethernet5
			Backup Resolved Label Stack: [20179 20175 3], Next hop: 20.30.32.30, Interface: Ethernet1
```

## show mpls segment-routing bindings detail

```text
10.0.0.30/32
   Local binding:  Label: 20030
      Uptime: 0:57:33
   Remote binding: Peer ID: Arista-Spine3-Q2A-30, Label: imp-null
      Uptime: 0:57:33
   Remote binding: Peer ID: Ciena-5134-72, Label: 20030
      Uptime: 0:03:39
   Remote binding: Peer ID: 0000.0000.0128, Label: 20030
      Uptime: 0:03:39
   Remote binding: Peer ID: Juniper-175-ACX7100-48L, Label: 20030
      Uptime: 0:03:39
   Remote binding: Peer ID: Juniper-179-ACX7024, Label: 20030
      Uptime: 0:03:39
10.0.0.32/32
   Local binding:  Label: imp-null
      Uptime: 0:30:29
   Remote binding: Peer ID: Arista-Spine3-Q2A-30, Label: 20032
      Uptime: 0:30:29
   Remote binding: Peer ID: Ciena-5134-72, Label: 20032
      Uptime: 0:03:39
   Remote binding: Peer ID: 0000.0000.0128, Label: 20032
      Uptime: 0:03:39
   Remote binding: Peer ID: Juniper-175-ACX7100-48L, Label: 20032
      Uptime: 0:03:39
   Remote binding: Peer ID: Juniper-179-ACX7024, Label: 20032
      Uptime: 0:03:39
10.0.0.53/32
   Local binding:  Label: 20053
      Uptime: 0:57:33
   Remote binding: Peer ID: Arista-Spine3-Q2A-30, Label: 20053
      Uptime: 0:57:33
   Remote binding: Peer ID: Ciena-5134-72, Label: 20053
      Uptime: 0:03:39
   Remote binding: Peer ID: 0000.0000.0128, Label: 20053
      Uptime: 0:03:39
   Remote binding: Peer ID: Juniper-175-ACX7100-48L, Label: 20053
      Uptime: 0:03:39
   Remote binding: Peer ID: Juniper-179-ACX7024, Label: 20053
      Uptime: 0:03:39
10.0.0.72/32
   Local binding:  Label: 20072
      Uptime: 0:31:53
   Remote binding: Peer ID: Arista-Spine3-Q2A-30, Label: 20072
      Uptime: 0:31:53
   Remote binding: Peer ID: Ciena-5134-72, Label: imp-null
      Uptime: 0:03:39
   Remote binding: Peer ID: 0000.0000.0128, Label: 20072
      Uptime: 0:03:39
   Remote binding: Peer ID: Juniper-175-ACX7100-48L, Label: 20072
      Uptime: 0:03:39
   Remote binding: Peer ID: Juniper-179-ACX7024, Label: 20072
      Uptime: 0:03:39
10.0.0.84/32
   Local binding:  Label: 20084
      Uptime: 0:57:33
   Remote binding: Peer ID: Arista-Spine3-Q2A-30, Label: 20084
      Uptime: 0:57:33
   Remote binding: Peer ID: Ciena-5134-72, Label: 20084
      Uptime: 0:03:39
   Remote binding: Peer ID: 0000.0000.0128, Label: 20084
      Uptime: 0:03:39
   Remote binding: Peer ID: Juniper-175-ACX7100-48L, Label: 20084
      Uptime: 0:03:39
   Remote binding: Peer ID: Juniper-179-ACX7024, Label: 20084
      Uptime: 0:03:39
10.0.0.120/32
   Local binding:  Label: 20120
      Uptime: 0:57:33
   Remote binding: Peer ID: Arista-Spine3-Q2A-30, Label: 20120
      Uptime: 0:57:33
   Remote binding: Peer ID: Ciena-5134-72, Label: 20120
      Uptime: 0:03:39
   Remote binding: Peer ID: 0000.0000.0128, Label: 20120
      Uptime: 0:03:39
   Remote binding: Peer ID: Juniper-175-ACX7100-48L, Label: 20120
      Uptime: 0:03:39
   Remote binding: Peer ID: Juniper-179-ACX7024, Label: 20120
      Uptime: 0:03:39
10.0.0.128/32
   Local binding:  Label: 20128
      Uptime: 0:09:35
   Remote binding: Peer ID: Arista-Spine3-Q2A-30, Label: 20128
      Uptime: 0:09:35
   Remote binding: Peer ID: Ciena-5134-72, Label: 20128
      Uptime: 0:03:39
   Remote binding: Peer ID: 0000.0000.0128, Label: imp-null
      Uptime: 0:03:39
   Remote binding: Peer ID: Juniper-175-ACX7100-48L, Label: 20128
      Uptime: 0:03:39
   Remote binding: Peer ID: Juniper-179-ACX7024, Label: 20128
      Uptime: 0:03:39
10.0.0.175/32
   Local binding:  Label: 20175
      Uptime: 0:39:21
   Remote binding: Peer ID: Arista-Spine3-Q2A-30, Label: 20175
      Uptime: 0:39:21
   Remote binding: Peer ID: Ciena-5134-72, Label: 20175
      Uptime: 0:03:39
   Remote binding: Peer ID: 0000.0000.0128, Label: 20175
      Uptime: 0:03:39
   Remote binding: Peer ID: Juniper-175-ACX7100-48L, Label: imp-null
      Uptime: 0:03:39
   Remote binding: Peer ID: Juniper-179-ACX7024, Label: 20175
      Uptime: 0:03:39
10.0.0.179/32
   Local binding:  Label: 20179
      Uptime: 0:40:33
   Remote binding: Peer ID: Arista-Spine3-Q2A-30, Label: 20179
      Uptime: 0:40:33
   Remote binding: Peer ID: Ciena-5134-72, Label: 20179
      Uptime: 0:03:39
   Remote binding: Peer ID: 0000.0000.0128, Label: 20179
      Uptime: 0:03:39
   Remote binding: Peer ID: Juniper-175-ACX7100-48L, Label: 20179
      Uptime: 0:03:39
   Remote binding: Peer ID: Juniper-179-ACX7024, Label: imp-null
      Uptime: 0:03:39
10.0.0.214/32
   Local binding:  Label: 20214
      Uptime: 0:41:53
   Remote binding: Peer ID: Arista-Spine3-Q2A-30, Label: 20214
      Uptime: 0:41:53
   Remote binding: Peer ID: Ciena-5134-72, Label: 20214
      Uptime: 0:03:39
   Remote binding: Peer ID: 0000.0000.0128, Label: 20214
      Uptime: 0:03:39
   Remote binding: Peer ID: Juniper-175-ACX7100-48L, Label: 20214
      Uptime: 0:03:39
   Remote binding: Peer ID: Juniper-179-ACX7024, Label: 20214
      Uptime: 0:03:39
10.0.0.217/32
   Local binding:  Label: 20217
      Uptime: 0:57:33
   Remote binding: Peer ID: Arista-Spine3-Q2A-30, Label: 20217
      Uptime: 0:57:33
   Remote binding: Peer ID: Ciena-5134-72, Label: 20217
      Uptime: 0:03:39
   Remote binding: Peer ID: 0000.0000.0128, Label: 20217
      Uptime: 0:03:39
   Remote binding: Peer ID: Juniper-175-ACX7100-48L, Label: 20217
      Uptime: 0:03:39
   Remote binding: Peer ID: Juniper-179-ACX7024, Label: 20217
      Uptime: 0:03:39
10.0.0.221/32
   Local binding:  Label: 21221
      Uptime: 0:33:41
   Remote binding: Peer ID: Arista-Spine3-Q2A-30, Label: 21221
      Uptime: 0:33:41
   Remote binding: Peer ID: Ciena-5134-72, Label: 21221
      Uptime: 0:03:39
   Remote binding: Peer ID: 0000.0000.0128, Label: 21221
      Uptime: 0:03:39
   Remote binding: Peer ID: Juniper-175-ACX7100-48L, Label: 21221
      Uptime: 0:03:39
   Remote binding: Peer ID: Juniper-179-ACX7024, Label: 21221
      Uptime: 0:03:39
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

 I L2     10.0.0.30/32 [115/10]
           via 20.30.32.30, Ethernet1
 C        10.0.0.32/32
           directly connected, Loopback0
 I L2     10.0.0.53/32 [115/20]
           via 20.30.32.30, Ethernet1
           via 20.32.175.175, Ethernet5
 I L2     10.0.0.72/32 [115/30]
           via 20.30.32.30, Ethernet1
           via 20.32.175.175, Ethernet5
 I L2     10.0.0.84/32 [115/30]
           via 20.30.32.30, Ethernet1
           via 20.32.175.175, Ethernet5
 I L2     10.0.0.120/32 [115/20]
           via 20.30.32.30, Ethernet1
 I L2     10.0.0.128/32 [115/20]
           via 20.30.32.30, Ethernet1
           via 20.32.175.175, Ethernet5
 I L2     10.0.0.175/32 [115/10]
           via 20.32.175.175, Ethernet5
 I L2     10.0.0.179/32 [115/20]
           via 20.30.32.30, Ethernet1
           via 20.32.175.175, Ethernet5
 I L2     10.0.0.214/32 [115/20]
           via 20.30.32.30, Ethernet1
           via 20.32.175.175, Ethernet5
 I L2     10.0.0.216/32 [115/30]
           via 20.30.32.30, Ethernet1
           via 20.32.175.175, Ethernet5
 I L2     10.0.0.217/32 [115/20]
           via 20.30.32.30, Ethernet1
           via 20.32.175.175, Ethernet5
 I L2     10.0.0.221/32 [115/20]
           via 20.30.32.30, Ethernet1
           via 20.32.175.175, Ethernet5
 C        20.30.32.0/24
           directly connected, Ethernet1
 I L2     20.30.53.0/24 [115/20]
           via 20.30.32.30, Ethernet1
 I L2     20.30.66.0/24 [115/20]
           via 20.30.32.30, Ethernet1
 I L2     20.30.72.0/24 [115/20]
           via 20.30.32.30, Ethernet1
 I L2     20.30.84.0/24 [115/20]
           via 20.30.32.30, Ethernet1
 I L2     20.30.120.0/24 [115/20]
           via 20.30.32.30, Ethernet1
 I L2     20.30.124.0/24 [115/20]
           via 20.30.32.30, Ethernet1
 I L2     20.30.128.0/24 [115/20]
           via 20.30.32.30, Ethernet1
 I L2     20.30.179.0/24 [115/20]
           via 20.30.32.30, Ethernet1
 I L2     20.30.184.0/24 [115/20]
           via 20.30.32.30, Ethernet1
 I L2     20.30.214.0/24 [115/20]
           via 20.30.32.30, Ethernet1
 I L2     20.30.217.0/24 [115/20]
           via 20.30.32.30, Ethernet1
 I L2     20.30.221.0/24 [115/20]
           via 20.30.32.30, Ethernet1
 C        20.32.175.0/24
           directly connected, Ethernet5
 I L2     20.53.175.0/24 [115/20]
           via 20.32.175.175, Ethernet5
 I L2     20.66.175.0/24 [115/20]
           via 20.32.175.175, Ethernet5
 I L2     20.72.175.0/24 [115/20]
           via 20.32.175.175, Ethernet5
 I L2     20.84.175.0/24 [115/20]
           via 20.32.175.175, Ethernet5
 I L2     20.120.175.0/24 [115/20]
           via 20.32.175.175, Ethernet5
 I L2     20.120.214.0/24 [115/30]
           via 20.30.32.30, Ethernet1
 I L2     20.124.175.0/24 [115/20]
           via 20.32.175.175, Ethernet5
 I L2     20.128.175.0/24 [115/20]
           via 20.32.175.175, Ethernet5
 I L2     20.131.175.0/24 [115/20]
           via 20.32.175.175, Ethernet5
 I L2     20.175.179.0/24 [115/20]
           via 20.32.175.175, Ethernet5
 I L2     20.175.184.0/24 [115/20]
           via 20.32.175.175, Ethernet5
 I L2     20.175.214.0/24 [115/20]
           via 20.32.175.175, Ethernet5
 I L2     20.175.217.0/24 [115/20]
           via 20.32.175.175, Ethernet5
 I L2     20.175.221.0/24 [115/20]
           via 20.32.175.175, Ethernet5
 I L2     20.214.216.0/24 [115/30]
           via 20.30.32.30, Ethernet1
           via 20.32.175.175, Ethernet5

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

 C        50.10.32.0/24
           directly connected, Ethernet40.4
 B I      50.10.72.0/24 [200/0]
           via 10.0.0.72/32, IS-IS SR tunnel index 9, label 62002
              via 20.30.32.30, Ethernet1, label 20072
              via 20.32.175.175, Ethernet5, label 20072
 B I      50.10.84.0/24 [200/0]
           via 10.0.0.84/32, IS-IS SR tunnel index 2, label 720896
              via 20.30.32.30, Ethernet1, label 20084
              via 20.32.175.175, Ethernet5, label 20084
 B I      50.10.120.0/24 [200/0]
           via 10.0.0.120/32, IS-IS SR tunnel index 8, label 1277
              via TI-LFA tunnel index 2, label 20120
                 via 20.30.32.30, Ethernet1, label imp-null(3)
                 backup via 20.32.175.175, Ethernet5, label 20072
 B I      50.10.128.0/24 [200/0]
           via 10.0.0.128/32, IS-IS SR tunnel index 11, label 48060
              via 20.30.32.30, Ethernet1, label 20128
              via 20.32.175.175, Ethernet5, label 20128
 B I      50.10.179.0/24 [200/0]
           via 10.0.0.179/32, IS-IS SR tunnel index 7, label 16
              via 20.30.32.30, Ethernet1, label 20179
              via 20.32.175.175, Ethernet5, label 20179
 B I      50.10.214.0/24 [200/0]
           via 10.0.0.214/32, IS-IS SR tunnel index 10, label 500000
              via 20.30.32.30, Ethernet1, label 20214
              via 20.32.175.175, Ethernet5, label 20214
 B I      50.10.217.0/24 [200/0]
           via 10.0.0.217/32, IS-IS SR tunnel index 16, label 524287
              via 20.30.32.30, Ethernet1, label 20217
              via 20.32.175.175, Ethernet5, label 20217
 B I      50.10.221.0/24 [200/0]
           via 10.0.0.221/32, IS-IS SR tunnel index 13, label 524289
              via 20.30.32.30, Ethernet1, label 21221
              via 20.32.175.175, Ethernet5, label 21221
 B I      51.10.120.0/24 [200/0]
           via 10.0.0.120/32, IS-IS SR tunnel index 8, label 1277
              via TI-LFA tunnel index 2, label 20120
                 via 20.30.32.30, Ethernet1, label imp-null(3)
                 backup via 20.32.175.175, Ethernet5, label 20072

```

## show ipv6 route

```text

VRF: default
Displaying 15 of 20 IPv6 routing table entries
Source Codes:
       C - connected, S - static, K - kernel, O3 - OSPFv3,
       B - Other BGP Routes, A B - BGP Aggregate, R - RIP,
       I L1 - IS-IS level 1, I L2 - IS-IS level 2, DH - DHCP,
       NG - Nexthop Group Static Route, M - Martian,
       DP - Dynamic Policy Route, L - VRF Leaked,
       G  - gRIBI, RC - Route Cache Route,
       CL - CBF Leaked Route

 C        2001:0:30:32::/64 [0/0]
           via Ethernet1, directly connected
 I L2     2001:0:30:66::/64 [115/20]
           via fe80::c6ca:2bff:fe45:a215, Ethernet1
 I L2     2001:0:30:72::/64 [115/20]
           via fe80::c6ca:2bff:fe45:a215, Ethernet1
 I L2     2001:0:30:84::/64 [115/20]
           via fe80::c6ca:2bff:fe45:a215, Ethernet1
 I L2     2001:0:30:120::/64 [115/20]
           via fe80::c6ca:2bff:fe45:a215, Ethernet1
 I L2     2001:0:30:124::/64 [115/20]
           via fe80::c6ca:2bff:fe45:a215, Ethernet1
 I L2     2001:0:30:128::/64 [115/20]
           via fe80::c6ca:2bff:fe45:a215, Ethernet1
 I L2     2001:0:30:179::/64 [115/20]
           via fe80::c6ca:2bff:fe45:a215, Ethernet1
 I L2     2001:0:30:184::/64 [115/20]
           via fe80::c6ca:2bff:fe45:a215, Ethernet1
 I L2     2001:0:30:214::/64 [115/20]
           via fe80::c6ca:2bff:fe45:a215, Ethernet1
 I L2     2001:0:30:217::/64 [115/20]
           via fe80::c6ca:2bff:fe45:a215, Ethernet1
 I L2     2001:0:30:221::/64 [115/20]
           via fe80::c6ca:2bff:fe45:a215, Ethernet1
 C        2001:0:32:175::/64 [0/0]
           via Ethernet5, directly connected
 I L2     2001:0:53:120::/64 [115/20]
           via fe80::c6ca:2bff:fe45:a215, Ethernet1
 I L2     2001:0:120:214::/64 [115/30]
           via fe80::c6ca:2bff:fe45:a215, Ethernet1

```

## show ipv6 route vrf RED

```text

VRF: RED
Displaying 10 of 14 IPv6 routing table entries
Source Codes:
       C - connected, S - static, K - kernel, O3 - OSPFv3,
       B - Other BGP Routes, A B - BGP Aggregate, R - RIP,
       I L1 - IS-IS level 1, I L2 - IS-IS level 2, DH - DHCP,
       NG - Nexthop Group Static Route, M - Martian,
       DP - Dynamic Policy Route, L - VRF Leaked,
       G  - gRIBI, RC - Route Cache Route,
       CL - CBF Leaked Route

 C        2600:50:10:32::/64 [0/0]
           via Ethernet40.6, directly connected
 B I      2600:50:10:72::/64 [200/0]
           via 10.0.0.72/32, IS-IS SR tunnel index 9, label 62003
              via 20.30.32.30, Ethernet1, label 20072
              via 20.32.175.175, Ethernet5, label 20072
 B I      2600:50:10:84::/64 [200/0]
           via 10.0.0.84/32, IS-IS SR tunnel index 2, label 720897
              via 20.30.32.30, Ethernet1, label 20084
              via 20.32.175.175, Ethernet5, label 20084
 B I      2600:50:10:120::/64 [200/0]
           via 10.0.0.120/32, IS-IS SR tunnel index 8, label 1276
              via TI-LFA tunnel index 2, label 20120
                 via 20.30.32.30, Ethernet1, label imp-null(3)
                 backup via 20.32.175.175, Ethernet5, label 20072
 B I      2600:50:10:128::/64 [200/0]
           via 10.0.0.128/32, IS-IS SR tunnel index 11, label 48061
              via 20.30.32.30, Ethernet1, label 20128
              via 20.32.175.175, Ethernet5, label 20128
 B I      2600:50:10:179::/64 [200/0]
           via 10.0.0.179/32, IS-IS SR tunnel index 7, label 16
              via 20.30.32.30, Ethernet1, label 20179
              via 20.32.175.175, Ethernet5, label 20179
 B I      2600:50:10:214::/64 [200/0]
           via 10.0.0.214/32, IS-IS SR tunnel index 10, label 500000
              via 20.30.32.30, Ethernet1, label 20214
              via 20.32.175.175, Ethernet5, label 20214
 B I      2600:50:10:217::/64 [200/0]
           via 10.0.0.217/32, IS-IS SR tunnel index 16, label 524287
              via 20.30.32.30, Ethernet1, label 20217
              via 20.32.175.175, Ethernet5, label 20217
 B I      2600:50:10:221::/64 [200/0]
           via 10.0.0.221/32, IS-IS SR tunnel index 13, label 524289
              via 20.30.32.30, Ethernet1, label 21221
              via 20.32.175.175, Ethernet5, label 21221
 B I      2600:51:10:120::/64 [200/0]
           via 10.0.0.120/32, IS-IS SR tunnel index 8, label 1276
              via TI-LFA tunnel index 2, label 20120
                 via 20.30.32.30, Ethernet1, label imp-null(3)
                 backup via 20.32.175.175, Ethernet5, label 20072

```

## show mpls route

```text
MPLS forwarding table (Label [metric] Vias) - 38 routes 
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

 20030   A[1]
                via M, ::, pop
                    EgressACL: apply
                  via TI-LFA tunnel index 1
                    via 20.30.32.30, Ethernet1, label imp-null(3)
                    backup via 20.32.175.175, Ethernet5, label 20128 20030
 20053   A[1]
                via M, forward
                    EgressACL: apply
                    20.30.32.30 Ethernet1
                    20.32.175.175 Ethernet5
 20072   A[1]
                via M, forward
                    EgressACL: apply
                    20.30.32.30 Ethernet1
                    20.32.175.175 Ethernet5
 20084   A[1]
                via M, forward
                    EgressACL: apply
                    20.30.32.30 Ethernet1
                    20.32.175.175 Ethernet5
 20120   A[1]
                via M, ::, forward
                    EgressACL: apply
                  via TI-LFA tunnel index 2
                    via 20.30.32.30, Ethernet1, label imp-null(3)
                    backup via 20.32.175.175, Ethernet5, label 20072
 20128   A[1]
                via M, forward
                    EgressACL: apply
                    20.30.32.30 Ethernet1
                    20.32.175.175 Ethernet5
 20175   A[1]
                via M, ::, pop
                    EgressACL: apply
                  via TI-LFA tunnel index 3
                    via 20.32.175.175, Ethernet5, label imp-null(3)
                    backup via 20.30.32.30, Ethernet1, label 20179 20175
 20179   A[1]
                via M, forward
                    EgressACL: apply
                    20.30.32.30 Ethernet1
                    20.32.175.175 Ethernet5
 20214   A[1]
                via M, forward
                    EgressACL: apply
                    20.30.32.30 Ethernet1
                    20.32.175.175 Ethernet5
 20217   A[1]
                via M, forward
                    EgressACL: apply
                    20.30.32.30 Ethernet1
                    20.32.175.175 Ethernet5
 21221   A[1]
                via M, forward
                    EgressACL: apply
                    20.30.32.30 Ethernet1
                    20.32.175.175 Ethernet5
 362149  A[1]
                via M, 20.30.32.30, pop
                    EgressACL: apply
                    directly connected, Ethernet1
                    c4:ca:2b:45:a2:15, vlan 1006
 362150  A[1]
                via M, fe80::c6ca:2bff:fe45:a215, pop
                    EgressACL: apply
                    directly connected, Ethernet1
                    c4:ca:2b:45:a2:15, vlan 1006
 362151  A[1]
                via M, 20.32.175.175, pop
                    EgressACL: apply
                    directly connected, Ethernet5
                    3c:08:cd:8d:ba:dc, vlan 1010
 378528   [0]
                via I, ipv4, vrf RED
 378529   [0]
                via I, ipv6, vrf RED
 1004053 A[1]
                SR-TE Policy 10.0.0.53, color 100, pop
                    EgressACL: apply
                  via SR-TE tunnel index 7
                    via TI-LFA tunnel index 1, label imp-null(3)
                       via 20.30.32.30, Ethernet1, label imp-null(3)
                       backup via 20.32.175.175, Ethernet5, label 20128 20030
 1004066 A[1]
                SR-TE Policy 10.0.0.66, color 100, pop
                    EgressACL: apply
                  via SR-TE tunnel index 6
                    via TI-LFA tunnel index 1, label imp-null(3)
                       via 20.30.32.30, Ethernet1, label imp-null(3)
                       backup via 20.32.175.175, Ethernet5, label 20128 20030
 1004072 A[1]
                SR-TE Policy 10.0.0.72, color 100, pop
                    EgressACL: apply
                  via SR-TE tunnel index 10
                    via TI-LFA tunnel index 1, label imp-null(3)
                       via 20.30.32.30, Ethernet1, label imp-null(3)
                       backup via 20.32.175.175, Ethernet5, label 20128 20030
 1004084 A[1]
                SR-TE Policy 10.0.0.84, color 100, pop
                    EgressACL: apply
                  via SR-TE tunnel index 2
                    via TI-LFA tunnel index 1, label imp-null(3)
                       via 20.30.32.30, Ethernet1, label imp-null(3)
                       backup via 20.32.175.175, Ethernet5, label 20128 20030
 1004120 A[1]
                SR-TE Policy 10.0.0.120, color 100, pop
                    EgressACL: apply
                  via SR-TE tunnel index 5
                    via TI-LFA tunnel index 1, label imp-null(3)
                       via 20.30.32.30, Ethernet1, label imp-null(3)
                       backup via 20.32.175.175, Ethernet5, label 20128 20030
 1004124 A[1]
                SR-TE Policy 10.0.0.124, color 100, pop
                    EgressACL: apply
                  via SR-TE tunnel index 1
                    via TI-LFA tunnel index 1, label imp-null(3)
                       via 20.30.32.30, Ethernet1, label imp-null(3)
                       backup via 20.32.175.175, Ethernet5, label 20128 20030
 1004128 A[1]
                SR-TE Policy 10.0.0.128, color 100, pop
                    EgressACL: apply
                  via SR-TE tunnel index 11
                    via TI-LFA tunnel index 1, label imp-null(3)
                       via 20.30.32.30, Ethernet1, label imp-null(3)
                       backup via 20.32.175.175, Ethernet5, label 20128 20030
 1004179 A[1]
                SR-TE Policy 10.0.0.179, color 100, pop
                    EgressACL: apply
                  via SR-TE tunnel index 8
                    via TI-LFA tunnel index 1, label imp-null(3)
                       via 20.30.32.30, Ethernet1, label imp-null(3)
                       backup via 20.32.175.175, Ethernet5, label 20128 20030
 1004214 A[1]
                SR-TE Policy 10.0.0.214, color 100, pop
                    EgressACL: apply
                  via SR-TE tunnel index 3
                    via TI-LFA tunnel index 1, label imp-null(3)
                       via 20.30.32.30, Ethernet1, label imp-null(3)
                       backup via 20.32.175.175, Ethernet5, label 20128 20030
 1004217 A[1]
                SR-TE Policy 10.0.0.217, color 100, pop
                    EgressACL: apply
                  via SR-TE tunnel index 9
                    via TI-LFA tunnel index 1, label imp-null(3)
                       via 20.30.32.30, Ethernet1, label imp-null(3)
                       backup via 20.32.175.175, Ethernet5, label 20128 20030
 1004221 A[1]
                SR-TE Policy 10.0.0.221, color 100, pop
                    EgressACL: apply
                  via SR-TE tunnel index 4
                    via TI-LFA tunnel index 1, label imp-null(3)
                       via 20.30.32.30, Ethernet1, label imp-null(3)
                       backup via 20.32.175.175, Ethernet5, label 20128 20030
 1006053 A[1]
                SR-TE Policy 10.0.0.53, color 101, pop
                    EgressACL: apply
                  via SR-TE tunnel index 12
                    via TI-LFA tunnel index 3, label imp-null(3)
                       via 20.32.175.175, Ethernet5, label imp-null(3)
                       backup via 20.30.32.30, Ethernet1, label 20179 20175
 1006066 A[1]
                SR-TE Policy 10.0.0.66, color 101, pop
                    EgressACL: apply
                  via SR-TE tunnel index 13
                    via TI-LFA tunnel index 3, label imp-null(3)
                       via 20.32.175.175, Ethernet5, label imp-null(3)
                       backup via 20.30.32.30, Ethernet1, label 20179 20175
 1006072 A[1]
                SR-TE Policy 10.0.0.72, color 101, pop
                    EgressACL: apply
                  via SR-TE tunnel index 14
                    via TI-LFA tunnel index 3, label imp-null(3)
                       via 20.32.175.175, Ethernet5, label imp-null(3)
                       backup via 20.30.32.30, Ethernet1, label 20179 20175
 1006084 A[1]
                SR-TE Policy 10.0.0.84, color 101, pop
                    EgressACL: apply
                  via SR-TE tunnel index 15
                    via TI-LFA tunnel index 3, label imp-null(3)
                       via 20.32.175.175, Ethernet5, label imp-null(3)
                       backup via 20.30.32.30, Ethernet1, label 20179 20175
 1006120 A[1]
                SR-TE Policy 10.0.0.120, color 101, pop
                    EgressACL: apply
                  via SR-TE tunnel index 16
                    via TI-LFA tunnel index 3, label imp-null(3)
                       via 20.32.175.175, Ethernet5, label imp-null(3)
                       backup via 20.30.32.30, Ethernet1, label 20179 20175
 1006124 A[1]
                SR-TE Policy 10.0.0.124, color 101, pop
                    EgressACL: apply
                  via SR-TE tunnel index 17
                    via TI-LFA tunnel index 3, label imp-null(3)
                       via 20.32.175.175, Ethernet5, label imp-null(3)
                       backup via 20.30.32.30, Ethernet1, label 20179 20175
 1006128 A[1]
                SR-TE Policy 10.0.0.128, color 101, pop
                    EgressACL: apply
                  via SR-TE tunnel index 18
                    via TI-LFA tunnel index 3, label imp-null(3)
                       via 20.32.175.175, Ethernet5, label imp-null(3)
                       backup via 20.30.32.30, Ethernet1, label 20179 20175
 1006179 A[1]
                SR-TE Policy 10.0.0.179, color 101, pop
                    EgressACL: apply
                  via SR-TE tunnel index 19
                    via TI-LFA tunnel index 3, label imp-null(3)
                       via 20.32.175.175, Ethernet5, label imp-null(3)
                       backup via 20.30.32.30, Ethernet1, label 20179 20175
 1006214 A[1]
                SR-TE Policy 10.0.0.214, color 101, pop
                    EgressACL: apply
                  via SR-TE tunnel index 20
                    via TI-LFA tunnel index 3, label imp-null(3)
                       via 20.32.175.175, Ethernet5, label imp-null(3)
                       backup via 20.30.32.30, Ethernet1, label 20179 20175
 1006217 A[1]
                SR-TE Policy 10.0.0.217, color 101, pop
                    EgressACL: apply
                  via SR-TE tunnel index 21
                    via TI-LFA tunnel index 3, label imp-null(3)
                       via 20.32.175.175, Ethernet5, label imp-null(3)
                       backup via 20.30.32.30, Ethernet1, label 20179 20175
 1006221 A[1]
                SR-TE Policy 10.0.0.221, color 101, pop
                    EgressACL: apply
                  via SR-TE tunnel index 22
                    via TI-LFA tunnel index 3, label imp-null(3)
                       via 20.32.175.175, Ethernet5, label imp-null(3)
                       backup via 20.30.32.30, Ethernet1, label 20179 20175
```

## show mpls lfib route

```text
MPLS forwarding table (Label [metric] Vias) - 38 routes 
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

 IP    20030    [1], 10.0.0.30/32
                via TI-LFA tunnel index 1, pop
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                    via 20.30.32.30, Ethernet1, label imp-null(3)
                    backup via 20.32.175.175, Ethernet5, label 20128 20030
 IP    20053    [1], 10.0.0.53/32
                via M, 20.30.32.30, forward
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                 interface Ethernet1
                via M, 20.32.175.175, forward
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                 interface Ethernet5
 IP    20072    [1], 10.0.0.72/32
                via M, 20.30.32.30, forward
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                 interface Ethernet1
                via M, 20.32.175.175, forward
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                 interface Ethernet5
 IP    20084    [1], 10.0.0.84/32
                via M, 20.30.32.30, forward
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                 interface Ethernet1
                via M, 20.32.175.175, forward
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                 interface Ethernet5
 IP    20120    [1], 10.0.0.120/32
                via TI-LFA tunnel index 2, forward
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                    via 20.30.32.30, Ethernet1, label imp-null(3)
                    backup via 20.32.175.175, Ethernet5, label 20072
 IP    20128    [1], 10.0.0.128/32
                via M, 20.30.32.30, forward
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                 interface Ethernet1
                via M, 20.32.175.175, forward
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                 interface Ethernet5
 IP    20175    [1], 10.0.0.175/32
                via TI-LFA tunnel index 3, pop
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                    via 20.32.175.175, Ethernet5, label imp-null(3)
                    backup via 20.30.32.30, Ethernet1, label 20179 20175
 IP    20179    [1], 10.0.0.179/32
                via M, 20.30.32.30, forward
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                 interface Ethernet1
                via M, 20.32.175.175, forward
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                 interface Ethernet5
 IP    20214    [1], 10.0.0.214/32
                via M, 20.30.32.30, forward
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                 interface Ethernet1
                via M, 20.32.175.175, forward
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                 interface Ethernet5
 IP    20217    [1], 10.0.0.217/32
                via M, 20.30.32.30, forward
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                 interface Ethernet1
                via M, 20.32.175.175, forward
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                 interface Ethernet5
 IP    21221    [1], 10.0.0.221/32
                via M, 20.30.32.30, forward
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                 interface Ethernet1
                via M, 20.32.175.175, forward
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                 interface Ethernet5
 IA    362149   [1]
                via M, 20.30.32.30, pop
                 payload autoDecide, ttlMode uniform, apply egress-acl
                 interface Ethernet1
 IA    362150   [1]
                via M, fe80::c6ca:2bff:fe45:a215, pop
                 payload autoDecide, ttlMode uniform, apply egress-acl
                 interface Ethernet1
 IA    362151   [1]
                via M, 20.32.175.175, pop
                 payload autoDecide, ttlMode uniform, apply egress-acl
                 interface Ethernet5
 B3    378528   [0]
                via I, ipv4, vrf RED
 B3    378529   [0]
                via I, ipv6, vrf RED
 ST    1004053  [1], SR-TE Policy 10.0.0.53, color 100
                via SR-TE tunnel index 7, pop
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                    via TI-LFA tunnel index 1, label imp-null(3)
                       via 20.30.32.30, Ethernet1, label imp-null(3)
                       backup via 20.32.175.175, Ethernet5, label 20128 20030
 ST    1004066  [1], SR-TE Policy 10.0.0.66, color 100
                via SR-TE tunnel index 6, pop
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                    via TI-LFA tunnel index 1, label imp-null(3)
                       via 20.30.32.30, Ethernet1, label imp-null(3)
                       backup via 20.32.175.175, Ethernet5, label 20128 20030
 ST    1004072  [1], SR-TE Policy 10.0.0.72, color 100
                via SR-TE tunnel index 10, pop
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                    via TI-LFA tunnel index 1, label imp-null(3)
                       via 20.30.32.30, Ethernet1, label imp-null(3)
                       backup via 20.32.175.175, Ethernet5, label 20128 20030
 ST    1004084  [1], SR-TE Policy 10.0.0.84, color 100
                via SR-TE tunnel index 2, pop
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                    via TI-LFA tunnel index 1, label imp-null(3)
                       via 20.30.32.30, Ethernet1, label imp-null(3)
                       backup via 20.32.175.175, Ethernet5, label 20128 20030
 ST    1004120  [1], SR-TE Policy 10.0.0.120, color 100
                via SR-TE tunnel index 5, pop
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                    via TI-LFA tunnel index 1, label imp-null(3)
                       via 20.30.32.30, Ethernet1, label imp-null(3)
                       backup via 20.32.175.175, Ethernet5, label 20128 20030
 ST    1004124  [1], SR-TE Policy 10.0.0.124, color 100
                via SR-TE tunnel index 1, pop
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                    via TI-LFA tunnel index 1, label imp-null(3)
                       via 20.30.32.30, Ethernet1, label imp-null(3)
                       backup via 20.32.175.175, Ethernet5, label 20128 20030
 ST    1004128  [1], SR-TE Policy 10.0.0.128, color 100
                via SR-TE tunnel index 11, pop
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                    via TI-LFA tunnel index 1, label imp-null(3)
                       via 20.30.32.30, Ethernet1, label imp-null(3)
                       backup via 20.32.175.175, Ethernet5, label 20128 20030
 ST    1004179  [1], SR-TE Policy 10.0.0.179, color 100
                via SR-TE tunnel index 8, pop
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                    via TI-LFA tunnel index 1, label imp-null(3)
                       via 20.30.32.30, Ethernet1, label imp-null(3)
                       backup via 20.32.175.175, Ethernet5, label 20128 20030
 ST    1004214  [1], SR-TE Policy 10.0.0.214, color 100
                via SR-TE tunnel index 3, pop
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                    via TI-LFA tunnel index 1, label imp-null(3)
                       via 20.30.32.30, Ethernet1, label imp-null(3)
                       backup via 20.32.175.175, Ethernet5, label 20128 20030
 ST    1004217  [1], SR-TE Policy 10.0.0.217, color 100
                via SR-TE tunnel index 9, pop
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                    via TI-LFA tunnel index 1, label imp-null(3)
                       via 20.30.32.30, Ethernet1, label imp-null(3)
                       backup via 20.32.175.175, Ethernet5, label 20128 20030
 ST    1004221  [1], SR-TE Policy 10.0.0.221, color 100
                via SR-TE tunnel index 4, pop
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                    via TI-LFA tunnel index 1, label imp-null(3)
                       via 20.30.32.30, Ethernet1, label imp-null(3)
                       backup via 20.32.175.175, Ethernet5, label 20128 20030
 ST    1006053  [1], SR-TE Policy 10.0.0.53, color 101
                via SR-TE tunnel index 12, pop
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                    via TI-LFA tunnel index 3, label imp-null(3)
                       via 20.32.175.175, Ethernet5, label imp-null(3)
                       backup via 20.30.32.30, Ethernet1, label 20179 20175
 ST    1006066  [1], SR-TE Policy 10.0.0.66, color 101
                via SR-TE tunnel index 13, pop
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                    via TI-LFA tunnel index 3, label imp-null(3)
                       via 20.32.175.175, Ethernet5, label imp-null(3)
                       backup via 20.30.32.30, Ethernet1, label 20179 20175
 ST    1006072  [1], SR-TE Policy 10.0.0.72, color 101
                via SR-TE tunnel index 14, pop
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                    via TI-LFA tunnel index 3, label imp-null(3)
                       via 20.32.175.175, Ethernet5, label imp-null(3)
                       backup via 20.30.32.30, Ethernet1, label 20179 20175
 ST    1006084  [1], SR-TE Policy 10.0.0.84, color 101
                via SR-TE tunnel index 15, pop
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                    via TI-LFA tunnel index 3, label imp-null(3)
                       via 20.32.175.175, Ethernet5, label imp-null(3)
                       backup via 20.30.32.30, Ethernet1, label 20179 20175
 ST    1006120  [1], SR-TE Policy 10.0.0.120, color 101
                via SR-TE tunnel index 16, pop
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                    via TI-LFA tunnel index 3, label imp-null(3)
                       via 20.32.175.175, Ethernet5, label imp-null(3)
                       backup via 20.30.32.30, Ethernet1, label 20179 20175
 ST    1006124  [1], SR-TE Policy 10.0.0.124, color 101
                via SR-TE tunnel index 17, pop
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                    via TI-LFA tunnel index 3, label imp-null(3)
                       via 20.32.175.175, Ethernet5, label imp-null(3)
                       backup via 20.30.32.30, Ethernet1, label 20179 20175
 ST    1006128  [1], SR-TE Policy 10.0.0.128, color 101
                via SR-TE tunnel index 18, pop
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                    via TI-LFA tunnel index 3, label imp-null(3)
                       via 20.32.175.175, Ethernet5, label imp-null(3)
                       backup via 20.30.32.30, Ethernet1, label 20179 20175
 ST    1006179  [1], SR-TE Policy 10.0.0.179, color 101
                via SR-TE tunnel index 19, pop
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                    via TI-LFA tunnel index 3, label imp-null(3)
                       via 20.32.175.175, Ethernet5, label imp-null(3)
                       backup via 20.30.32.30, Ethernet1, label 20179 20175
 ST    1006214  [1], SR-TE Policy 10.0.0.214, color 101
                via SR-TE tunnel index 20, pop
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                    via TI-LFA tunnel index 3, label imp-null(3)
                       via 20.32.175.175, Ethernet5, label imp-null(3)
                       backup via 20.30.32.30, Ethernet1, label 20179 20175
 ST    1006217  [1], SR-TE Policy 10.0.0.217, color 101
                via SR-TE tunnel index 21, pop
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                    via TI-LFA tunnel index 3, label imp-null(3)
                       via 20.32.175.175, Ethernet5, label imp-null(3)
                       backup via 20.30.32.30, Ethernet1, label 20179 20175
 ST    1006221  [1], SR-TE Policy 10.0.0.221, color 101
                via SR-TE tunnel index 22, pop
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                    via TI-LFA tunnel index 3, label imp-null(3)
                       via 20.32.175.175, Ethernet5, label imp-null(3)
                       backup via 20.30.32.30, Ethernet1, label 20179 20175
```

## show bgp evpn

```text
BGP routing table information for VRF default
Router identifier 10.0.0.32, local AS number 64512
Route status codes: * - valid, > - active, S - Stale, E - ECMP head, e - ECMP
                    c - Contributing to ECMP, % - Pending best path selection
Origin codes: i - IGP, e - EGP, ? - incomplete
AS Path Attributes: Or-ID - Originator ID, C-LST - Cluster List, LL Nexthop - Link Local Nexthop

          Network                Next Hop              Metric  LocPref Weight  Path
```

## show bgp vpn-ipv4

```text
BGP routing table information for VRF default
Router identifier 10.0.0.32, local AS number 64512
Route status codes: s - suppressed contributor, * - valid, > - active, E - ECMP head, e - ECMP
                    S - Stale, c - Contributing to ECMP, b - backup, L - labeled-unicast
                    % - Pending best path selection
Origin codes: i - IGP, e - EGP, ? - incomplete
AS Path Attributes: Or-ID - Originator ID, C-LST - Cluster List, LL Nexthop - Link Local Nexthop

          Network                Next Hop              Metric  LocPref Weight  Path
 * >      RD: 10.0.0.32:5001 IPv4 prefix 50.10.32.0/24
                                 -                     -       -       0       i
 * >Ec    RD: 72:5001 IPv4 prefix 50.10.72.0/24
                                 10.0.0.72             -       100     0       ? Or-ID: 10.0.0.72 C-LST: 10.0.0.30 
 *  ec    RD: 72:5001 IPv4 prefix 50.10.72.0/24
                                 10.0.0.72             -       100     0       ? Or-ID: 10.0.0.72 C-LST: 10.0.0.175 
 * >Ec    RD: 84:5001 IPv4 prefix 50.10.84.0/24
                                 10.0.0.84             0       100     0       ? Or-ID: 10.0.0.84 C-LST: 10.0.0.30 
 *  ec    RD: 84:5001 IPv4 prefix 50.10.84.0/24
                                 10.0.0.84             0       100     0       ? Or-ID: 10.0.0.84 C-LST: 10.0.0.175 
 * >Ec    RD: 120:5001 IPv4 prefix 50.10.120.0/24
                                 10.0.0.120            0       100     0       ? Or-ID: 10.0.0.120 C-LST: 10.0.0.30 
 *  ec    RD: 120:5001 IPv4 prefix 50.10.120.0/24
                                 10.0.0.120            0       100     0       ? Or-ID: 10.0.0.120 C-LST: 10.0.0.175 
 * >      RD: 128:5001 IPv4 prefix 50.10.128.0/24
                                 10.0.0.128            0       100     0       ? Or-ID: 10.0.0.128 C-LST: 10.0.0.175 
 * >Ec    RD: 179:5001 IPv4 prefix 50.10.179.0/24
                                 10.0.0.179            -       100     0       i Or-ID: 10.0.0.179 C-LST: 10.0.0.30 
 *  ec    RD: 179:5001 IPv4 prefix 50.10.179.0/24
                                 10.0.0.179            -       100     0       i Or-ID: 10.0.0.179 C-LST: 10.0.0.175 
 * >Ec    RD: 214:5001 IPv4 prefix 50.10.214.0/24
                                 10.0.0.214            -       100     0       i Or-ID: 10.0.0.214 C-LST: 10.0.0.30 
 *  ec    RD: 214:5001 IPv4 prefix 50.10.214.0/24
                                 10.0.0.214            -       100     0       i Or-ID: 10.0.0.214 C-LST: 10.0.0.175 
 * >Ec    RD: 217:5001 IPv4 prefix 50.10.217.0/24
                                 10.0.0.217            -       100     0       i Or-ID: 10.0.0.217 C-LST: 10.0.0.30 
 *  ec    RD: 217:5001 IPv4 prefix 50.10.217.0/24
                                 10.0.0.217            -       100     0       i Or-ID: 10.0.0.217 C-LST: 10.0.0.175 
 * >Ec    RD: 210:5001 IPv4 prefix 50.10.221.0/24
                                 10.0.0.221            -       100     0       i Or-ID: 10.0.0.221 C-LST: 10.0.0.30 
 *  ec    RD: 210:5001 IPv4 prefix 50.10.221.0/24
                                 10.0.0.221            -       100     0       i Or-ID: 10.0.0.221 C-LST: 10.0.0.175 
 * >Ec    RD: 120:5001 IPv4 prefix 51.10.120.0/24
                                 10.0.0.120            0       100     0       ? Or-ID: 10.0.0.120 C-LST: 10.0.0.30 
 *  ec    RD: 120:5001 IPv4 prefix 51.10.120.0/24
                                 10.0.0.120            0       100     0       ? Or-ID: 10.0.0.120 C-LST: 10.0.0.175 
```

## show bgp vpn-ipv6

```text
BGP routing table information for VRF default
Router identifier 10.0.0.32, local AS number 64512
Route status codes: s - suppressed contributor, * - valid, > - active, E - ECMP head, e - ECMP
                    S - Stale, c - Contributing to ECMP, b - backup, L - labeled-unicast
                    % - Pending best path selection
Origin codes: i - IGP, e - EGP, ? - incomplete
AS Path Attributes: Or-ID - Originator ID, C-LST - Cluster List, LL Nexthop - Link Local Nexthop

          Network                Next Hop              Metric  LocPref Weight  Path
 * >      RD: 10.0.0.32:5001 IPv6 prefix 2600:50:10:32::/64
                                 -                     -       -       0       i
 * >Ec    RD: 72:5001 IPv6 prefix 2600:50:10:72::/64
                                 ::ffff:10.0.0.72      -       100     0       ? Or-ID: 10.0.0.72 C-LST: 10.0.0.30 
 *  ec    RD: 72:5001 IPv6 prefix 2600:50:10:72::/64
                                 ::ffff:10.0.0.72      -       100     0       ? Or-ID: 10.0.0.72 C-LST: 10.0.0.175 
 * >Ec    RD: 84:5001 IPv6 prefix 2600:50:10:84::/64
                                 ::ffff:10.0.0.84      0       100     0       ? Or-ID: 10.0.0.84 C-LST: 10.0.0.30 
 *  ec    RD: 84:5001 IPv6 prefix 2600:50:10:84::/64
                                 ::ffff:10.0.0.84      0       100     0       ? Or-ID: 10.0.0.84 C-LST: 10.0.0.175 
 * >Ec    RD: 120:5001 IPv6 prefix 2600:50:10:120::/64
                                 ::ffff:10.0.0.120     0       100     0       ? Or-ID: 10.0.0.120 C-LST: 10.0.0.30 
 *  ec    RD: 120:5001 IPv6 prefix 2600:50:10:120::/64
                                 ::ffff:10.0.0.120     0       100     0       ? Or-ID: 10.0.0.120 C-LST: 10.0.0.175 
 * >      RD: 128:5001 IPv6 prefix 2600:50:10:128::/64
                                 ::ffff:10.0.0.128     0       100     0       ? Or-ID: 10.0.0.128 C-LST: 10.0.0.175 
 * >Ec    RD: 179:5001 IPv6 prefix 2600:50:10:179::/64
                                 ::ffff:10.0.0.179     -       100     0       i Or-ID: 10.0.0.179 C-LST: 10.0.0.30 
 *  ec    RD: 179:5001 IPv6 prefix 2600:50:10:179::/64
                                 ::ffff:10.0.0.179     -       100     0       i Or-ID: 10.0.0.179 C-LST: 10.0.0.175 
 * >Ec    RD: 214:5001 IPv6 prefix 2600:50:10:214::/64
                                 ::ffff:10.0.0.214     -       100     0       i Or-ID: 10.0.0.214 C-LST: 10.0.0.30 
 *  ec    RD: 214:5001 IPv6 prefix 2600:50:10:214::/64
                                 ::ffff:10.0.0.214     -       100     0       i Or-ID: 10.0.0.214 C-LST: 10.0.0.175 
 * >Ec    RD: 217:5001 IPv6 prefix 2600:50:10:217::/64
                                 ::ffff:10.0.0.217     -       100     0       i Or-ID: 10.0.0.217 C-LST: 10.0.0.30 
 *  ec    RD: 217:5001 IPv6 prefix 2600:50:10:217::/64
                                 ::ffff:10.0.0.217     -       100     0       i Or-ID: 10.0.0.217 C-LST: 10.0.0.175 
 * >Ec    RD: 210:5001 IPv6 prefix 2600:50:10:221::/64
                                 ::ffff:10.0.0.221     -       100     0       i Or-ID: 10.0.0.221 C-LST: 10.0.0.30 
 *  ec    RD: 210:5001 IPv6 prefix 2600:50:10:221::/64
                                 ::ffff:10.0.0.221     -       100     0       i Or-ID: 10.0.0.221 C-LST: 10.0.0.175 
 * >Ec    RD: 120:5001 IPv6 prefix 2600:51:10:120::/64
                                 ::ffff:10.0.0.120     0       100     0       ? Or-ID: 10.0.0.120 C-LST: 10.0.0.30 
 *  ec    RD: 120:5001 IPv6 prefix 2600:51:10:120::/64
                                 ::ffff:10.0.0.120     0       100     0       ? Or-ID: 10.0.0.120 C-LST: 10.0.0.175 
```

## show bgp ipv4 labeled-unicast

```text
BGP routing table information for VRF default
Router identifier 10.0.0.32, local AS number 64512
Route status codes: s - suppressed contributor, * - valid, > - active, E - ECMP head, e - ECMP
                    S - Stale, c - Contributing to ECMP, b - backup, L - labeled-unicast
                    % - Pending best path selection
Origin codes: i - IGP, e - EGP, ? - incomplete
AS Path Attributes: Or-ID - Originator ID, C-LST - Cluster List, LL Nexthop - Link Local Nexthop

          Network                Next Hop              Metric  AIGP       LocPref Weight  Path
```

## show bgp neighbors

```text
BGP neighbor is 10.0.0.30, remote AS 64512, internal link
 Description: Arista-Spine30
  BGP version 4, remote router ID 10.0.0.30, VRF default
  Inherits configuration from and member of peer-group IBGP_CLIENT_PEER
  Last read 00:00:08, last write 00:00:13
  Hold time is 180, keepalive interval is 60 seconds
  Configured hold time is 180, keepalive interval is 60 seconds
  Effective minimum hold time is 3 seconds
  Send failure hold time is 0 seconds
  Hold timer is active, time left: 00:02:52
  Keepalive timer is active, time left: 00:00:44
  Connect timer is inactive
  Idle-restart timer is inactive
  BGP state is Established, up for 00:30:30
  Number of transitions to established: 3
  Last state was OpenConfirm
  Last event was ReapplyOutboundPolicy
  Last sent notification:Hold Timer Expired Error/None, Last time 01:09:49, First time 02:11:41, Repeats 1
  Last sent socket-error:Connect (Network is unreachable), Last time 00:57:34, First time 02:11:40, Repeats 38
  Types of communities advertised: standard extended large
  Enhanced route refresh stale path removal disabled
  Outbound enhanced route refresh enabled
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
      Received 00:30:29
      Number of stale paths removed after graceful restart: 0
      Number of paths received before End-of-RIB: 9
    VPN-IPv6 End-of-RIB received: Yes
      Received 00:30:29
      Number of stale paths removed after graceful restart: 0
      Number of paths received before End-of-RIB: 9
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
    Opens:                           3         3
    Notifications:                   2         0
    Updates:                        30       471
    Keepalives:                   1388      1354
    Enhanced Route Refresh:          0         0
    Begin of Route Refresh:          0         0
    End of Route Refresh:            0         0
    Total messages:               1423      1828
  Prefix Statistics:
                                   Sent      Rcvd     Best Paths     Best ECMP Paths
    IPv4 Unicast:                     0         0              0                   0
    VPN-IPv4:                         1         8              8                   8
    IPv6 Unicast:                     0         0              0                   0
    VPN-IPv6:                         1         8              8                   8
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
  Outbound route map for VPN-IPv4 is SET_COLOR_100
  Outbound route map for VPN-IPv6 is SET_COLOR_101
Local AS is 64512, local router ID 10.0.0.32
TTL is 255
Local TCP address is 10.0.0.32, local port is 179
Remote TCP address is 10.0.0.30, remote port is 39565
Local next hop for next hop self:
  VPN-IPv4: 10.0.0.32
  VPN-IPv6: ::ffff:10.0.0.32
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
    TCP Throughput: 416.69 Mbps
    Advertised Recv Window (rcv_space): 14600

BGP neighbor is 10.0.0.175, remote AS 64512, internal link
 Description: Juniper_175
  BGP version 4, remote router ID 10.0.0.175, VRF default
  Inherits configuration from and member of peer-group IBGP_CLIENT_PEER
  Last read 00:00:04, last write 00:00:13
  Hold time is 90, keepalive interval is 30 seconds
  Configured hold time is 180, keepalive interval is 60 seconds
  Effective minimum hold time is 3 seconds
  Send failure hold time is 0 seconds
  Hold timer is active, time left: 00:01:26
  Keepalive timer is active, time left: 00:00:13
  Connect timer is inactive
  Idle-restart timer is inactive
  BGP state is Established, up for 00:30:15
  Number of transitions to established: 11
  Last state was OpenConfirm
  Last event was ReapplyOutboundPolicy
  Last sent notification:Hold Timer Expired Error/None, Last time 00:41:07, First time 14:02:13, Repeats 9
  Last sent socket-error:Connect (Network is unreachable), Last time 00:58:46, First time 14:02:12, Repeats 25
  Types of communities advertised: standard extended large
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
      Received 00:30:14
      Number of stale paths removed after graceful restart: 0
      Number of paths received before End-of-RIB: 9
    VPN-IPv6 End-of-RIB received: Yes
      Received 00:30:14
      Number of stale paths removed after graceful restart: 0
      Number of paths received before End-of-RIB: 9
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
    Opens:                 11        11
    Notifications:         10         0
    Updates:               52       436
    Keepalives:          2736      2453
    Route Refresh:          0         0
    Total messages:      2809      2900
  Prefix Statistics:
                                   Sent      Rcvd     Best Paths     Best ECMP Paths
    IPv4 Unicast:                     0         0              0                   0
    VPN-IPv4:                         1         9              9                   0
    IPv6 Unicast:                     0         0              0                   0
    VPN-IPv6:                         1         9              9                   0
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
  Outbound route map for VPN-IPv4 is SET_COLOR_100
  Outbound route map for VPN-IPv6 is SET_COLOR_101
Local AS is 64512, local router ID 10.0.0.32
TTL is 255
Local TCP address is 10.0.0.32, local port is 32981
Remote TCP address is 10.0.0.175, remote port is 179
Local next hop for next hop self:
  VPN-IPv4: 10.0.0.32
  VPN-IPv6: ::ffff:10.0.0.32
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
    Round-trip Time (rtt/rtvar): 0.5ms/0.1ms
    Delayed Ack Timeout (ato): 40.0ms
    Congestion Window (cwnd): 10
    TCP Throughput: 224.06 Mbps
    Advertised Recv Window (rcv_space): 14480

```

## show tunnel rib system-tunnel-rib brief

```text
Tunnel RIB: system-tunnel-rib
Endpoint        Tunnel Type     Index(es)   Tunnel Preference   IGP Preference 
-------------- --------------- ----------- ------------------- ----------------
10.0.0.30/32    IS-IS SR IPv4   5           65                  115            
10.0.0.53/32    IS-IS SR IPv4   6           65                  115            
10.0.0.72/32    IS-IS SR IPv4   9           65                  115            
10.0.0.84/32    IS-IS SR IPv4   2           65                  115            
10.0.0.120/32   IS-IS SR IPv4   8           65                  115            
10.0.0.128/32   IS-IS SR IPv4   11          65                  115            
10.0.0.175/32   IS-IS SR IPv4   1           65                  115            
10.0.0.179/32   IS-IS SR IPv4   7           65                  115            
10.0.0.214/32   IS-IS SR IPv4   10          65                  115            
10.0.0.217/32   IS-IS SR IPv4   16          65                  115            
10.0.0.221/32   IS-IS SR IPv4   13          65                  115            

   IGP Metric    Metric Type
---------------- -----------
   10            metric     
   20            metric     
   30            metric     
   30            metric     
   20            metric     
   20            metric     
   10            metric     
   20            metric     
   20            metric     
   20            metric     
   20            metric     

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
>C    10.0.0.32/32 [0 pref/0 metric] updated 21:15:56 ago
         via Loopback0, directly connected
>C    20.30.32.0/24 [0 pref/0 metric] updated 00:57:44 ago
         via Ethernet1, directly connected
>C    20.32.175.0/24 [0 pref/0 metric] updated 02:35:44 ago
         via Ethernet5, directly connected
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
>I    10.0.0.30/32 [115 pref/10 metric] updated 00:57:34 ago
         via 20.30.32.30, Ethernet1
>I    10.0.0.53/32 [115 pref/20 metric] updated 00:03:40 ago
         via 20.30.32.30, Ethernet1
         via 20.32.175.175, Ethernet5
>I    10.0.0.72/32 [115 pref/30 metric] updated 00:03:40 ago
         via 20.30.32.30, Ethernet1
         via 20.32.175.175, Ethernet5
>I    10.0.0.84/32 [115 pref/30 metric] updated 00:03:40 ago
         via 20.30.32.30, Ethernet1
         via 20.32.175.175, Ethernet5
>I    10.0.0.120/32 [115 pref/20 metric] updated 00:57:34 ago
         via 20.30.32.30, Ethernet1
>I    10.0.0.128/32 [115 pref/20 metric] updated 00:03:40 ago
         via 20.30.32.30, Ethernet1
         via 20.32.175.175, Ethernet5
>I    10.0.0.175/32 [115 pref/10 metric] updated 00:03:40 ago
         via 20.32.175.175, Ethernet5
>I    10.0.0.179/32 [115 pref/20 metric] updated 00:03:40 ago
         via 20.30.32.30, Ethernet1
         via 20.32.175.175, Ethernet5
>I    10.0.0.214/32 [115 pref/20 metric] updated 00:03:40 ago
         via 20.30.32.30, Ethernet1
         via 20.32.175.175, Ethernet5
>I    10.0.0.216/32 [115 pref/30 metric] updated 00:03:40 ago
         via 20.30.32.30, Ethernet1
         via 20.32.175.175, Ethernet5
>I    10.0.0.217/32 [115 pref/20 metric] updated 00:03:40 ago
         via 20.30.32.30, Ethernet1
         via 20.32.175.175, Ethernet5
>I    10.0.0.221/32 [115 pref/20 metric] updated 00:03:40 ago
         via 20.30.32.30, Ethernet1
         via 20.32.175.175, Ethernet5
>I    20.30.53.0/24 [115 pref/20 metric] updated 00:57:34 ago
         via 20.30.32.30, Ethernet1
>I    20.30.66.0/24 [115 pref/20 metric] updated 00:57:34 ago
         via 20.30.32.30, Ethernet1
>I    20.30.72.0/24 [115 pref/20 metric] updated 00:57:34 ago
         via 20.30.32.30, Ethernet1
>I    20.30.84.0/24 [115 pref/20 metric] updated 00:57:34 ago
         via 20.30.32.30, Ethernet1
>I    20.30.120.0/24 [115 pref/20 metric] updated 00:57:34 ago
         via 20.30.32.30, Ethernet1
>I    20.30.124.0/24 [115 pref/20 metric] updated 00:57:34 ago
         via 20.30.32.30, Ethernet1
>I    20.30.128.0/24 [115 pref/20 metric] updated 00:57:34 ago
         via 20.30.32.30, Ethernet1
>I    20.30.179.0/24 [115 pref/20 metric] updated 00:57:34 ago
         via 20.30.32.30, Ethernet1
>I    20.30.184.0/24 [115 pref/20 metric] updated 00:57:34 ago
         via 20.30.32.30, Ethernet1
>I    20.30.214.0/24 [115 pref/20 metric] updated 00:41:56 ago
         via 20.30.32.30, Ethernet1
>I    20.30.217.0/24 [115 pref/20 metric] updated 00:57:34 ago
         via 20.30.32.30, Ethernet1
>I    20.30.221.0/24 [115 pref/20 metric] updated 00:57:34 ago
         via 20.30.32.30, Ethernet1
>I    20.53.175.0/24 [115 pref/20 metric] updated 00:03:40 ago
         via 20.32.175.175, Ethernet5
>I    20.66.175.0/24 [115 pref/20 metric] updated 00:03:40 ago
         via 20.32.175.175, Ethernet5
>I    20.72.175.0/24 [115 pref/20 metric] updated 00:03:40 ago
         via 20.32.175.175, Ethernet5
>I    20.84.175.0/24 [115 pref/20 metric] updated 00:03:40 ago
         via 20.32.175.175, Ethernet5
>I    20.120.175.0/24 [115 pref/20 metric] updated 00:03:40 ago
         via 20.32.175.175, Ethernet5
>I    20.120.214.0/24 [115 pref/30 metric] updated 00:57:34 ago
         via 20.30.32.30, Ethernet1
>I    20.124.175.0/24 [115 pref/20 metric] updated 00:03:40 ago
         via 20.32.175.175, Ethernet5
>I    20.128.175.0/24 [115 pref/20 metric] updated 00:03:40 ago
         via 20.32.175.175, Ethernet5
>I    20.131.175.0/24 [115 pref/20 metric] updated 00:03:40 ago
         via 20.32.175.175, Ethernet5
>I    20.175.179.0/24 [115 pref/20 metric] updated 00:03:40 ago
         via 20.32.175.175, Ethernet5
>I    20.175.184.0/24 [115 pref/20 metric] updated 00:03:40 ago
         via 20.32.175.175, Ethernet5
>I    20.175.214.0/24 [115 pref/20 metric] updated 00:03:40 ago
         via 20.32.175.175, Ethernet5
>I    20.175.217.0/24 [115 pref/20 metric] updated 00:03:40 ago
         via 20.32.175.175, Ethernet5
>I    20.175.221.0/24 [115 pref/20 metric] updated 00:03:40 ago
         via 20.32.175.175, Ethernet5
>I    20.214.216.0/24 [115 pref/30 metric] updated 00:03:40 ago
         via 20.30.32.30, Ethernet1
         via 20.32.175.175, Ethernet5
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
         via Ethernet1, directly connected
>C    2001:0:32:175::/64 [0 pref/0 metric] updated 00:03:22 ago
         via Ethernet5, directly connected
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
>P    ::/96 [1 pref/0 metric] updated 00:57:44 ago
         via Null0, directly connected [NF]
>P    ::ffff:127.0.0.0/104 [1 pref/0 metric] updated 00:57:44 ago
         via :: [1 pref/1 metric] type ipv6
            via , directly connected
>P    fe80::/10 [1 pref/0 metric] updated 00:57:44 ago
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
>I    2001:0:30:66::/64 [115 pref/20 metric] updated 00:57:34 ago
         via fe80::c6ca:2bff:fe45:a215, Ethernet1
>I    2001:0:30:72::/64 [115 pref/20 metric] updated 00:57:34 ago
         via fe80::c6ca:2bff:fe45:a215, Ethernet1
>I    2001:0:30:84::/64 [115 pref/20 metric] updated 00:57:34 ago
         via fe80::c6ca:2bff:fe45:a215, Ethernet1
>I    2001:0:30:120::/64 [115 pref/20 metric] updated 00:57:34 ago
         via fe80::c6ca:2bff:fe45:a215, Ethernet1
>I    2001:0:30:124::/64 [115 pref/20 metric] updated 00:57:34 ago
         via fe80::c6ca:2bff:fe45:a215, Ethernet1
>I    2001:0:30:128::/64 [115 pref/20 metric] updated 00:57:34 ago
         via fe80::c6ca:2bff:fe45:a215, Ethernet1
>I    2001:0:30:179::/64 [115 pref/20 metric] updated 00:57:34 ago
         via fe80::c6ca:2bff:fe45:a215, Ethernet1
>I    2001:0:30:184::/64 [115 pref/20 metric] updated 00:57:34 ago
         via fe80::c6ca:2bff:fe45:a215, Ethernet1
>I    2001:0:30:214::/64 [115 pref/20 metric] updated 00:41:56 ago
         via fe80::c6ca:2bff:fe45:a215, Ethernet1
>I    2001:0:30:217::/64 [115 pref/20 metric] updated 00:57:34 ago
         via fe80::c6ca:2bff:fe45:a215, Ethernet1
>I    2001:0:30:221::/64 [115 pref/20 metric] updated 00:57:34 ago
         via fe80::c6ca:2bff:fe45:a215, Ethernet1
>I    2001:0:53:120::/64 [115 pref/20 metric] updated 00:57:34 ago
         via fe80::c6ca:2bff:fe45:a215, Ethernet1
>I    2001:0:120:214::/64 [115 pref/30 metric] updated 00:57:34 ago
         via fe80::c6ca:2bff:fe45:a215, Ethernet1
```

## show platform sand l3 summary

```text
Number of vrfs: 3

Ipv4:
  Routes:       77   backlog:  0  unprogrammed:  0
  Adjacencies:  115  backlog:  0  unprogrammed:  0
Ipv6:
  Routes:       37   backlog:  0  unprogrammed:  0
  Adjacencies:  115  backlog:  0  unprogrammed:  0
Mpls:
  Routes:       36  backlog:  0  unprogrammed:  0
  Adjacencies:  3   backlog:  0  unprogrammed:  0

Jericho2 Ip Fecs:
  Non-ecmp fecs:  4152  ecmp fecs:  2  fec entries:  4156
Jericho2 Mpls Fecs:
  Non-ecmp fecs:  3  ecmp fecs:  0  fec entries:  3
Jericho2 Vxlan Tunnel Fecs:
  Non-ecmp fecs:  0  ecmp fecs:  0  fec entries:  0
  Number of vxlan tunnels configured: 0

Jericho2 Lpm Routes:
  Routes:   77  unprogrammed:   0   
  Routes6:  37  unprogrammed6:  0   
  Backlog:  0 

Jericho2 Lpm:
  TCAM entries used:   4   Percent free:  99  ADS2 entries used:   5  Percent free:  99
  Pivot buckets used:  6   Rows used:     2   Entries Per Bucket:  0  Percent free:  99
  Route buckets used:  24  Rows used:     3   Entries Per Bucket:  4  Percent free:  99

Lem:
  IPv4  Host in Lem:            disabled
  IPv4  Prefix-lengths in Lem:  None    
  IPv6  Host in Lem:            disabled
  IPv6  Prefix-lengths in Lem:  None    
  Number of downloads:        0
  Number of overflow events:  0

Egress Arp rewrite entries in use (in each fap):
  FixedSystem: 4
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
  FixedSystem: 4112

Jericho2 Fec:
  Maximum FEC hierarchy levels:  2
  ReusedEcmp:  0  allocs:  535  frees:  477  shuffles:  0  cmds:  0
  Zombies:     0    purges:    0
  Quarantine:  0/0  shuffles:  0  deletes:  0   
  Preserved FECs: 0
    First FEC preserved: never
    Last FEC preserved: never
  Fec insertion failures:  0
  Level1  Fecs:
    Non-ecmp fecs:            38  ecmp fecs:            1 
    Non-ecmp (Percent free):  99  ecmp (Percent free):  99
  Level2  Fecs:
    Non-ecmp fecs:            22  ecmp fecs:            2 
    Non-ecmp (Percent free):  99  ecmp (Percent free):  99
  Level3  Fecs:
    Non-ecmp fecs:            0    ecmp fecs:            0  
    Non-ecmp (Percent free):  100  ecmp (Percent free):  100

Lpm Detail:
  Requests:  2031  cleanses:  517  batches:  517  avg batch size:  3

Jericho Arp:
  ArpTable writes:      28437  queued      0   
  IngressTable writes:  79710  queued      0   
  Coprocessors:         1      in CmdRing

Tunnel Counter Status
  Number of MPLS tunnels:                  12   
  Number of uncountable MPLS tunnels:      12   
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
|0  |0.0.0.0/8         |DROP | DROP               |0    |  -     |                   |  -  |288360|   -   
|0  |10.0.0.30/32      |ROUTE| Et1                |1006 |107517  | c4:ca:2b:45:a2:15 |  -  |288362|   -   
|0  |10.0.0.32/32      |TRAP | CoppSystemIpUcast  |0    |  -     | Receive           |  -  |524291|   -   
|0  |10.0.0.53/32      |ROUTE| Et5                |1010 |107518  | 3c:08:cd:8d:ba:dc |16384|288373|   -   
|0  |10.0.0.53/32      |ROUTE| Et1                |1006 |107517  | c4:ca:2b:45:a2:15 |16384|288374|   -   
|0  |10.0.0.72/32      |ROUTE| Et5                |1010 |107518  | 3c:08:cd:8d:ba:dc |16384|288373|   -   
|0  |10.0.0.72/32      |ROUTE| Et1                |1006 |107517  | c4:ca:2b:45:a2:15 |16384|288374|   -   
|0  |10.0.0.84/32      |ROUTE| Et5                |1010 |107518  | 3c:08:cd:8d:ba:dc |16384|288373|   -   
|0  |10.0.0.84/32      |ROUTE| Et1                |1006 |107517  | c4:ca:2b:45:a2:15 |16384|288374|   -   
|0  |10.0.0.120/32     |ROUTE| Et1                |1006 |107517  | c4:ca:2b:45:a2:15 |  -  |288362|   -   
|0  |10.0.0.128/32     |ROUTE| Et5                |1010 |107518  | 3c:08:cd:8d:ba:dc |16384|288373|   -   
|0  |10.0.0.128/32     |ROUTE| Et1                |1006 |107517  | c4:ca:2b:45:a2:15 |16384|288374|   -   
|0  |10.0.0.175/32     |ROUTE| Et5                |1010 |107518  | 3c:08:cd:8d:ba:dc |  -  |288372|   -   
|0  |10.0.0.179/32     |ROUTE| Et5                |1010 |107518  | 3c:08:cd:8d:ba:dc |16384|288373|   -   
|0  |10.0.0.179/32     |ROUTE| Et1                |1006 |107517  | c4:ca:2b:45:a2:15 |16384|288374|   -   
|0  |10.0.0.214/32     |ROUTE| Et5                |1010 |107518  | 3c:08:cd:8d:ba:dc |16384|288373|   -   
|0  |10.0.0.214/32     |ROUTE| Et1                |1006 |107517  | c4:ca:2b:45:a2:15 |16384|288374|   -   
|0  |10.0.0.216/32     |ROUTE| Et5                |1010 |107518  | 3c:08:cd:8d:ba:dc |16384|288373|   -   
|0  |10.0.0.216/32     |ROUTE| Et1                |1006 |107517  | c4:ca:2b:45:a2:15 |16384|288374|   -   
|0  |10.0.0.217/32     |ROUTE| Et5                |1010 |107518  | 3c:08:cd:8d:ba:dc |16384|288373|   -   
|0  |10.0.0.217/32     |ROUTE| Et1                |1006 |107517  | c4:ca:2b:45:a2:15 |16384|288374|   -   
|0  |10.0.0.221/32     |ROUTE| Et5                |1010 |107518  | 3c:08:cd:8d:ba:dc |16384|288373|   -   
|0  |10.0.0.221/32     |ROUTE| Et1                |1006 |107517  | c4:ca:2b:45:a2:15 |16384|288374|   -   
|0  |20.30.32.0/32     |TRAP | CoppSystemIpBcast  |0    |  -     | BcastReceive      |  -  |524290|   -   
|0  |20.30.32.30/32    |ROUTE| Et1                |1006 |107517  | c4:ca:2b:45:a2:15 |  -  |288368|   -   
|0  |20.30.32.32/32    |TRAP | CoppSystemIpUcast  |0    |  -     | Receive           |  -  |524291|   -   
|0  |20.30.32.255/32   |TRAP | CoppSystemIpBcast  |0    |  -     | BcastReceive      |  -  |524290|   -   
|0  |20.30.32.0/24     |TRAP | CoppSystemL3DstMiss|1006 |1006    | ArpTrap           |  -  |525301|   -   
|0  |20.30.53.0/24     |ROUTE| Et1                |1006 |107517  | c4:ca:2b:45:a2:15 |  -  |288362|   -   
|0  |20.30.66.0/24     |ROUTE| Et1                |1006 |107517  | c4:ca:2b:45:a2:15 |  -  |288362|   -   
|0  |20.30.72.0/24     |ROUTE| Et1                |1006 |107517  | c4:ca:2b:45:a2:15 |  -  |288362|   -   
|0  |20.30.84.0/24     |ROUTE| Et1                |1006 |107517  | c4:ca:2b:45:a2:15 |  -  |288362|   -   
|0  |20.30.120.0/24    |ROUTE| Et1                |1006 |107517  | c4:ca:2b:45:a2:15 |  -  |288362|   -   
|0  |20.30.124.0/24    |ROUTE| Et1                |1006 |107517  | c4:ca:2b:45:a2:15 |  -  |288362|   -   
|0  |20.30.128.0/24    |ROUTE| Et1                |1006 |107517  | c4:ca:2b:45:a2:15 |  -  |288362|   -   
|0  |20.30.179.0/24    |ROUTE| Et1                |1006 |107517  | c4:ca:2b:45:a2:15 |  -  |288362|   -   
|0  |20.30.184.0/24    |ROUTE| Et1                |1006 |107517  | c4:ca:2b:45:a2:15 |  -  |288362|   -   
|0  |20.30.214.0/24    |ROUTE| Et1                |1006 |107517  | c4:ca:2b:45:a2:15 |  -  |288362|   -   
|0  |20.30.217.0/24    |ROUTE| Et1                |1006 |107517  | c4:ca:2b:45:a2:15 |  -  |288362|   -   
|0  |20.30.221.0/24    |ROUTE| Et1                |1006 |107517  | c4:ca:2b:45:a2:15 |  -  |288362|   -   
|0  |20.32.175.0/32    |TRAP | CoppSystemIpBcast  |0    |  -     | BcastReceive      |  -  |524290|   -   
|0  |20.32.175.32/32   |TRAP | CoppSystemIpUcast  |0    |  -     | Receive           |  -  |524291|   -   
|0  |20.32.175.175/32  |ROUTE| Et5                |1010 |107518  | 3c:08:cd:8d:ba:dc |  -  |288367|   -   
|0  |20.32.175.255/32  |TRAP | CoppSystemIpBcast  |0    |  -     | BcastReceive      |  -  |524290|   -   
|0  |20.32.175.0/24    |TRAP | CoppSystemL3DstMiss|1010 |1010    | ArpTrap           |  -  |525305|   -   
|0  |20.53.175.0/24    |ROUTE| Et5                |1010 |107518  | 3c:08:cd:8d:ba:dc |  -  |288372|   -   
|0  |20.66.175.0/24    |ROUTE| Et5                |1010 |107518  | 3c:08:cd:8d:ba:dc |  -  |288372|   -   
|0  |20.72.175.0/24    |ROUTE| Et5                |1010 |107518  | 3c:08:cd:8d:ba:dc |  -  |288372|   -   
|0  |20.84.175.0/24    |ROUTE| Et5                |1010 |107518  | 3c:08:cd:8d:ba:dc |  -  |288372|   -   
|0  |20.120.175.0/24   |ROUTE| Et5                |1010 |107518  | 3c:08:cd:8d:ba:dc |  -  |288372|   -   
|0  |20.120.214.0/24   |ROUTE| Et1                |1006 |107517  | c4:ca:2b:45:a2:15 |  -  |288362|   -   
|0  |20.124.175.0/24   |ROUTE| Et5                |1010 |107518  | 3c:08:cd:8d:ba:dc |  -  |288372|   -   
|0  |20.128.175.0/24   |ROUTE| Et5                |1010 |107518  | 3c:08:cd:8d:ba:dc |  -  |288372|   -   
|0  |20.131.175.0/24   |ROUTE| Et5                |1010 |107518  | 3c:08:cd:8d:ba:dc |  -  |288372|   -   
|0  |20.175.179.0/24   |ROUTE| Et5                |1010 |107518  | 3c:08:cd:8d:ba:dc |  -  |288372|   -   
|0  |20.175.184.0/24   |ROUTE| Et5                |1010 |107518  | 3c:08:cd:8d:ba:dc |  -  |288372|   -   
|0  |20.175.214.0/24   |ROUTE| Et5                |1010 |107518  | 3c:08:cd:8d:ba:dc |  -  |288372|   -   
|0  |20.175.217.0/24   |ROUTE| Et5                |1010 |107518  | 3c:08:cd:8d:ba:dc |  -  |288372|   -   
|0  |20.175.221.0/24   |ROUTE| Et5                |1010 |107518  | 3c:08:cd:8d:ba:dc |  -  |288372|   -   
|0  |20.214.216.0/24   |ROUTE| Et5                |1010 |107518  | 3c:08:cd:8d:ba:dc |16384|288373|   -   
|0  |20.214.216.0/24   |ROUTE| Et1                |1006 |107517  | c4:ca:2b:45:a2:15 |16384|288374|   -   
|0  |127.0.0.0/8       |TRAP | CoppSystemL3DstMiss|0    |  -     | ArpTrap           |  -  |524295|   -   
|0  |0.0.0.0/0         |TRAP | CoppSystemL3LpmOver|0    |  -     | SlowReceive       |  -  |524293|   -   
|1  |0.0.0.0/8         |DROP | DROP               |0    |  -     |                   |  -  |288361|   -   
|1  |127.0.0.0/8       |TRAP | CoppSystemL3DstMiss|0    |  -     | ArpTrap           |  -  |524295|   -   
|1  |192.168.20.0/32   |TRAP | CoppSystemIpBcast  |0    |  -     | BcastReceive      |  -  |524290|   -   
|1  |192.168.20.32/32  |TRAP | CoppSystemIpUcast  |0    |  -     | Receive           |  -  |524291|   -   
|1  |192.168.21.255/32 |TRAP | CoppSystemIpBcast  |0    |  -     | BcastReceive      |  -  |524290|   -   
|1  |192.168.20.0/23   |TRAP | CoppSystemL3DstMiss|0    |  -     | ArpTrap           |  -  |524295|   -   
|1  |0.0.0.0/0         |TRAP | CoppSystemL3DstMiss|0    |  -     | ArpTrap           |  -  |524295|   -   
|2  |0.0.0.0/8         |DROP | DROP               |0    |  -     |                   |  -  |288364|   -   
|2  |50.10.32.0/32     |TRAP | CoppSystemIpBcast  |0    |  -     | BcastReceive      |  -  |524290|   -   
|2  |50.10.32.1/32     |TRAP | CoppSystemIpUcast  |0    |  -     | Receive           |  -  |524291|   -   
|2  |50.10.32.2/32     |ROUTE| Et40               |1008 |107519  | 00:28:01:00:00:01 |  -  |288370|   -   
|2  |50.10.32.255/32   |TRAP | CoppSystemIpBcast  |0    |  -     | BcastReceive      |  -  |524290|   -   
|2  |50.10.32.0/24     |TRAP | CoppSystemL3DstMiss|1008 |1008    | ArpTrap           |  -  |525303|   -   
|2  |50.10.72.0/24     |ROUTE| FEC 16385          |0    |2097132 | 00:00:00:00:00:00 |  -  |157300|M 20072 62002
|2  |50.10.84.0/24     |ROUTE| FEC 16385          |0    |2097136 | 00:00:00:00:00:00 |  -  |157292|M 20084 720896
|2  |50.10.120.0/24    |ROUTE| FEC 288377         |0    |2097138 | 00:00:00:00:00:00 |  -  |157305|M 20120 1277
|2  |50.10.128.0/24    |ROUTE| FEC 16385          |0    |2097128 | 00:00:00:00:00:00 |  -  |157291|M 20128 48060
|2  |50.10.179.0/24    |ROUTE| FEC 16385          |0    |2097127 | 00:00:00:00:00:00 |  -  |157302|M 20179 16
|2  |50.10.214.0/24    |ROUTE| FEC 16385          |0    |2097131 | 00:00:00:00:00:00 |  -  |157299|M 20214 500000
|2  |50.10.217.0/24    |ROUTE| FEC 16385          |0    |2097130 | 00:00:00:00:00:00 |  -  |157297|M 20217 524287
|2  |50.10.221.0/24    |ROUTE| FEC 16385          |0    |2097134 | 00:00:00:00:00:00 |  -  |157295|M 21221 524289
|2  |51.10.120.0/24    |ROUTE| FEC 288377         |0    |2097138 | 00:00:00:00:00:00 |  -  |157305|M 20120 1277
|2  |127.0.0.0/8       |TRAP | CoppSystemL3DstMiss|0    |  -     | ArpTrap           |  -  |524295|   -   
|2  |0.0.0.0/0         |TRAP | CoppSystemL3LpmOver|0    |  -     | SlowReceive       |  -  |524293|   -   

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
|16384|288373|ROUTE| Et5                |1010 |107518  | 3c:08:cd:8d:ba:dc |   -   
|16384|288374|ROUTE| Et1                |1006 |107517  | c4:ca:2b:45:a2:15 |   -   
|16385|288380|ROUTE| Et5                |1010 |107518  | 3c:08:cd:8d:ba:dc |   -   
|16385|288381|ROUTE| Et1                |1006 |107517  | c4:ca:2b:45:a2:15 |   -   
|  -  |157288|ROUTE| FEC 16385          |   - |2097131 |                 - |Mpush 20214 500000
|  -  |157290|ROUTE| FEC 288379         |   - |  -     |                   |   -   
|  -  |157291|ROUTE| FEC 16385          |   - |2097128 |                 - |Mpush 20128 48060
|  -  |157292|ROUTE| FEC 16385          |   - |2097136 |                 - |Mpush 20084 720896
|  -  |157293|ROUTE| FEC 16385          |   - |2097127 |                 - |Mpush 20179 16
|  -  |157294|ROUTE| FEC 16385          |   - |2097133 |                 - |Mpush 20072 62003
|  -  |157295|ROUTE| FEC 16385          |   - |2097134 |                 - |Mpush 21221 524289
|  -  |157296|ROUTE| FEC 16385          |   - |2097134 |                 - |Mpush 21221 524289
|  -  |157297|ROUTE| FEC 16385          |   - |2097130 |                 - |Mpush 20217 524287
|  -  |157298|ROUTE| FEC 16385          |   - |2097129 |                 - |Mpush 20128 48061
|  -  |157299|ROUTE| FEC 16385          |   - |2097131 |                 - |Mpush 20214 500000
|  -  |157300|ROUTE| FEC 16385          |   - |2097132 |                 - |Mpush 20072 62002
|  -  |157301|ROUTE| FEC 16385          |   - |2097130 |                 - |Mpush 20217 524287
|  -  |157302|ROUTE| FEC 16385          |   - |2097127 |                 - |Mpush 20179 16
|  -  |157303|ROUTE| FEC 16385          |   - |2097135 |                 - |Mpush 20084 720897
|  -  |157304|ROUTE| FEC 288378         |   - |  -     |                   |   -   
|  -  |157305|ROUTE| FEC 288377         |   - |2097138 |                 - |Mpush 20120 1277
|  -  |157306|ROUTE| FEC 288378         |   - |  -     |                   |   -   
|  -  |157308|ROUTE| FEC 288378         |   - |  -     |                   |   -   
|  -  |157310|ROUTE| FEC 288378         |   - |  -     |                   |   -   
|  -  |157312|ROUTE| FEC 288378         |   - |  -     |                   |   -   
|  -  |157314|ROUTE| FEC 288378         |   - |  -     |                   |   -   
|  -  |157316|ROUTE| FEC 288378         |   - |  -     |                   |   -   
|  -  |157318|ROUTE| FEC 288378         |   - |  -     |                   |   -   
|  -  |157320|ROUTE| FEC 288378         |   - |  -     |                   |   -   
|  -  |157322|ROUTE| FEC 288378         |   - |  -     |                   |   -   
|  -  |157324|ROUTE| FEC 288378         |   - |  -     |                   |   -   
|  -  |157326|ROUTE| FEC 288377         |   - |2097137 |                 - |Mpush 20120 1276
|  -  |157327|ROUTE| FEC 288379         |   - |  -     |                   |   -   
|  -  |157328|ROUTE| FEC 288379         |   - |  -     |                   |   -   
|  -  |157329|ROUTE| FEC 288379         |   - |  -     |                   |   -   
|  -  |157330|ROUTE| FEC 288379         |   - |  -     |                   |   -   
|  -  |157331|ROUTE| FEC 288379         |   - |  -     |                   |   -   
|  -  |157332|ROUTE| FEC 288379         |   - |  -     |                   |   -   
|  -  |157333|ROUTE| FEC 288379         |   - |  -     |                   |   -   
|  -  |157334|ROUTE| FEC 288379         |   - |  -     |                   |   -   
|  -  |157335|ROUTE| FEC 288379         |   - |  -     |                   |   -   
|  -  |157336|ROUTE| FEC 288379         |   - |  -     |                   |   -   
|  -  |288360|DROP | DROP               |0    |  -     |                   |   -   
|  -  |288361|DROP | DROP               |0    |  -     |                   |   -   
|  -  |288362|ROUTE| Et1                |1006 |107517  | c4:ca:2b:45:a2:15 |   -   
|  -  |288363|ROUTE| Et1                |1006 |107517  | c4:ca:2b:45:a2:15 |   -   
|  -  |288364|DROP | DROP               |0    |  -     |                   |   -   
|  -  |288366|DROP | DROP               |0    |  -     |                   |   -   
|  -  |288367|ROUTE| Et5                |1010 |107518  | 3c:08:cd:8d:ba:dc |   -   
|  -  |288368|ROUTE| Et1                |1006 |107517  | c4:ca:2b:45:a2:15 |   -   
|  -  |288369|ROUTE| Et1                |1006 |107517  | c4:ca:2b:45:a2:15 |   -   
|  -  |288370|ROUTE| Et40               |1008 |107519  | 00:28:01:00:00:01 |   -   
|  -  |288371|ROUTE| Et1                |1006 |107517  | c4:ca:2b:45:a2:15 |   -   
|  -  |288372|ROUTE| Et5                |1010 |107518  | 3c:08:cd:8d:ba:dc |   -   
|  -  |288375|ROUTE| Et5                |1010 |107518  | 3c:08:cd:8d:ba:dc |   -   
|  -  |288376|DROP | DROP               |0    |  -     |                   |   -   
|  -  |288377|ROUTE| Et1                |1006 |107517  | c4:ca:2b:45:a2:15 |   -   
|  -  |288378|ROUTE| Et1                |1006 |107517  | c4:ca:2b:45:a2:15 |   -   
|  -  |288379|ROUTE| Et5                |1010 |107518  | 3c:08:cd:8d:ba:dc |   -   
|  -  |288383|ROUTE| Et40               |1009 |107520  | 00:29:01:00:00:01 |   -   
|  -  |524290|TRAP | CoppSystemIpBcast  |0    |  -     | BcastReceive      |   -   
|  -  |524291|TRAP | CoppSystemIpUcast  |0    |  -     | Receive           |   -   
|  -  |524293|TRAP | CoppSystemL3LpmOver|0    |  -     | SlowReceive       |   -   
|  -  |524295|TRAP | CoppSystemL3DstMiss|0    |  -     | ArpTrap           |   -   
|  -  |525301|TRAP | CoppSystemL3DstMiss|1006 |1006    | ArpTrap           |   -   
|  -  |525303|TRAP | CoppSystemL3DstMiss|1008 |1008    | ArpTrap           |   -   
|  -  |525304|TRAP | CoppSystemL3DstMiss|1009 |1009    | ArpTrap           |   -   
|  -  |525305|TRAP | CoppSystemL3DstMiss|1010 |1010    | ArpTrap           |   -   

```

