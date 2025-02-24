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

Uptime: 2 days, 10 hours and 50 minutes
Total memory: 65734472 kB
Free memory: 61768648 kB

```

## show lldp neighbors

```text
Last table change time   : 1 day, 8:03:52 ago
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
Interface         IP Address          Status     Protocol         MTU   Owner  
----------------- ------------------- ---------- ------------ --------- -------
Ethernet1         20.30.32.32/24      up         up              1500          
Ethernet5         20.32.175.32/24     up         up              1500          
Ethernet40.4      50.10.32.1/24       up         up              1500          
Ethernet40.128    50.128.32.1/24      up         up              1500          
Ethernet40.129    50.129.32.1/24      up         up              1500          
Ethernet40.130    50.130.32.1/24      up         up              1500          
Loopback0         10.0.0.32/32        up         up             65535          
Management1       192.168.20.32/23    up         up              1500          

```

## show interfaces counters rates | nz

```text
Port      Name                Intvl  In Mbps      %  In Kpps Out Mbps      %
Et1       Arista_Spine30_Eth2  0:01    346.6   4.2%      451    399.9   4.8%
Et40                           0:01    479.9   5.8%      624    346.6   4.2%

Port      Out Kpps
Et1            499
Et40           451
```

## show isis neighbors

```text
 
Instance  VRF      System Id        Type Interface          SNPA              State Hold time   Circuit Id          
IGP       default  Arista-Spine3-Q2A-30 L2   Ethernet1          P2P               UP    30          2C                  
IGP       default  Juniper-175-ACX7100-48L L2   Ethernet5          P2P               UP    27          01                  
```

## show isis database detail

```text
Legend:
H - hostname conflict
U - node unreachable

IS-IS Instance: IGP VRF: default
  IS-IS Level 2 Link State Database
    LSPID                   Seq Num  Cksum  Life Length IS  Received LSPID        Flags
    Arista-Spine3-Q2A-30.00-00       643  15125  1056   1040 L2  0000.0000.0030.00-00  <>
      Remaining lifetime received: 1199 s Modified to: 1200 s
      NLPID: 0xCC(IPv4) 0x8E(IPv6)
      Hostname: Arista-Spine3-Q2A-30
      Area addresses: 49.0001
      Topology: 2 (IPv6)
      Topology: 0 (IPv4)
      Interface address: 20.30.221.30
      Interface address: 20.30.131.30
      Interface address: 20.30.184.30
      Interface address: 20.30.120.30
      Interface address: 20.30.156.30
      Interface address: 20.30.53.30
      Interface address: 20.30.128.30
      Interface address: 20.30.179.30
      Interface address: 20.30.124.30
      Interface address: 20.30.217.30
      Interface address: 20.30.84.30
      Interface address: 20.30.214.30
      Interface address: 20.30.32.30
      Interface address: 10.0.0.30
      Interface address: 2001:0:30:221::30
      Interface address: 2001:0:30:131::30
      Interface address: 2001:0:30:184::30
      Interface address: 2001:0:30:120::30
      Interface address: 2001:0:30:156::30
      Interface address: 2001:0:53:120::30
      Interface address: 2001:0:30:128::30
      Interface address: 2001:0:30:179::30
      Interface address: 2001:0:30:124::30
      Interface address: 2001:0:30:217::30
      Interface address: 2001:0:30:84::30
      Interface address: 2001:0:30:214::30
      Interface address: 2001:0:30:32::30
      IS Neighbor          : Juniper-131-JCNR.00 Metric: 10
        IPv4 Neighbor Address: 20.30.131.131
        IPv4 Interface Address: 20.30.131.30
        Adj-sid: 362209 flags: [L V] weight: 0x0
      IS Neighbor          : Nokia-SR1-217.00    Metric: 10
        IPv4 Neighbor Address: 20.30.217.217
        IPv4 Interface Address: 20.30.217.30
        Adj-sid: 362196 flags: [L V] weight: 0x0
      IS Neighbor          : H3C_M1A_120.00      Metric: 10
        IPv4 Neighbor Address: 20.30.120.120
        IPv4 Interface Address: 20.30.120.30
        Adj-sid: 362188 flags: [L V] weight: 0x0
      IS Neighbor          : Arista-PE32-Q2C-32.00 Metric: 10
        IPv4 Neighbor Address: 20.30.32.32
        IPv4 Interface Address: 20.30.32.30
        Adj-sid: 362190 flags: [L V] weight: 0x0
      IS Neighbor          : Juniper-156-PTX10002-36QDD.00 Metric: 10
        IPv4 Neighbor Address: 20.30.156.156
        IPv4 Interface Address: 20.30.156.30
        Adj-sid: 362202 flags: [L V] weight: 0x0
      Reachability         : 20.30.221.0/24 Metric: 10 Type: 1 Up
      Reachability         : 20.30.131.0/24 Metric: 10 Type: 1 Up
      Reachability         : 10.0.0.30/32 Metric: 0 Type: 1 Up
        SR Prefix-SID: 30 Flags: [N] Algorithm: 0
        SR Prefix-SID: 1158 Flags: [N] Algorithm: 128
        SR Prefix-SID: 1159 Flags: [N] Algorithm: 129
        SR Prefix-SID: 1160 Flags: [N] Algorithm: 130
      Reachability         : 20.30.184.0/24 Metric: 10 Type: 1 Up
      Reachability         : 20.30.120.0/24 Metric: 10 Type: 1 Up
      Reachability         : 20.30.156.0/24 Metric: 10 Type: 1 Up
      Reachability         : 20.30.53.0/24 Metric: 10 Type: 1 Up
      Reachability         : 20.30.128.0/24 Metric: 10 Type: 1 Up
      Reachability         : 20.30.179.0/24 Metric: 10 Type: 1 Up
      Reachability         : 20.30.124.0/24 Metric: 10 Type: 1 Up
      Reachability         : 20.30.217.0/24 Metric: 10 Type: 1 Up
      Reachability         : 20.30.84.0/24 Metric: 10 Type: 1 Up
      Reachability         : 20.30.214.0/24 Metric: 10 Type: 1 Up
      Reachability         : 20.30.32.0/24 Metric: 10 Type: 1 Up
      Reachability (MT-IPv6): 2001:0:30:131::/64 Metric: 10 Type: 1 Up
      Reachability (MT-IPv6): 2001:0:30:184::/64 Metric: 10 Type: 1 Up
      Reachability (MT-IPv6): 2001:0:30:120::/64 Metric: 10 Type: 1 Up
      Reachability (MT-IPv6): 2001:0:30:156::/64 Metric: 10 Type: 1 Up
      Reachability (MT-IPv6): 2001:0:53:120::/64 Metric: 10 Type: 1 Up
      Reachability (MT-IPv6): 2001:0:30:128::/64 Metric: 10 Type: 1 Up
      Reachability (MT-IPv6): 2001:0:30:179::/64 Metric: 10 Type: 1 Up
      Reachability (MT-IPv6): 2001:0:30:124::/64 Metric: 10 Type: 1 Up
      Reachability (MT-IPv6): 2001:0:30:217::/64 Metric: 10 Type: 1 Up
      Reachability (MT-IPv6): 2001:0:30:84::/64 Metric: 10 Type: 1 Up
      Reachability (MT-IPv6): 2001:0:30:214::/64 Metric: 10 Type: 1 Up
      Reachability (MT-IPv6): 2001:0:30:32::/64 Metric: 10 Type: 1 Up
      Router Capabilities: Router Id: 10.0.0.30 Flags: []
        SR Local Block:
          SRLB Base: 965536 Range: 65536
        Area leader priority: 250 algorithm: 0
        Maximum SID depth:
          Base MPLS imposition (MSD type 1):  12
        SR Capability: Flags: [I V]
          SRGB Base: 20000 Range: 2000
        Algorithms:  0, 128, 129, 130
        Flex Algo: Algorithm: 130 Metric: IGP Metric (0) Calc: SPF (0) Prio: 237
          Exclude admin groups: 1
        Flex Algo: Algorithm: 129 Metric: TE Metric (2) Calc: SPF (0) Prio: 255
        Flex Algo: Algorithm: 128 Metric: Min Unidirectional Delay Metric (1) Calc: SPF (0) Prio: 255
    Arista-Spine3-Q2A-30.00-01        95  48635   981    813 L2  0000.0000.0030.00-01  <>
      Remaining lifetime received: 1199 s Modified to: 1200 s
      IS Neighbor          : 0000.0000.0184.00   Metric: 10
        IPv4 Neighbor Address: 20.30.184.184
        IPv4 Interface Address: 20.30.184.30
        Adj-sid: 362208 flags: [L V] weight: 0x0
      IS Neighbor          : 221.00              Metric: 10
        IPv4 Neighbor Address: 20.30.221.221
        IPv4 Interface Address: 20.30.221.30
        Adj-sid: 362197 flags: [L V] weight: 0x0
      IS Neighbor          : 0000.0000.0124.00   Metric: 10
        IPv4 Neighbor Address: 20.30.124.124
        IPv4 Interface Address: 20.30.124.30
        Adj-sid: 362192 flags: [L V] weight: 0x0
      IS Neighbor          : Arrcus-53.00        Metric: 10
        IPv4 Neighbor Address: 20.30.53.53
        IPv4 Interface Address: 20.30.53.30
        Adj-sid: 362193 flags: [L V] weight: 0x0
      IS Neighbor          : Ericsson_84_R6678.00 Metric: 10
        IPv4 Neighbor Address: 20.30.84.84
        IPv4 Interface Address: 20.30.84.30
        Adj-sid: 362199 flags: [L V] weight: 0x0
      IS Neighbor          : Nokia-SXR-214.00    Metric: 10
        IPv4 Neighbor Address: 20.30.214.214
        IPv4 Interface Address: 20.30.214.30
        Adj-sid: 362191 flags: [L V] weight: 0x0
      IS Neighbor          : Juniper-179-ACX7024.00 Metric: 10
        IPv4 Neighbor Address: 20.30.179.179
        IPv4 Interface Address: 20.30.179.30
        Adj-sid: 362201 flags: [L V] weight: 0x0
      IS Neighbor          : 0000.0000.0128.00   Metric: 10
        IPv4 Neighbor Address: 20.30.128.128
        IPv4 Interface Address: 20.30.128.30
        Adj-sid: 362194 flags: [L V] weight: 0x0
      IS Neighbor (MT-IPv6): Ericsson_84_R6678.00 Metric: 10
        IPv6 Neighbor Address: 2001:0:30:84::175
        Global IPv6 Interface Address: 2001:0:30:84::30
        Adj-sid: 362200 flags: [L V F] weight: 0x0
      IS Neighbor (MT-IPv6): H3C_M1A_120.00      Metric: 10
        IPv6 Neighbor Address: 2001:0:30:120::120
        Global IPv6 Interface Address: 2001:0:30:120::30
        Adj-sid: 362189 flags: [L V F] weight: 0x0
      IS Neighbor (MT-IPv6): Arista-PE32-Q2C-32.00 Metric: 10
        IPv6 Neighbor Address: 2001:0:30:32::32
        Global IPv6 Interface Address: 2001:0:30:32::30
        Adj-sid: 362198 flags: [L V F] weight: 0x0
      Reachability (MT-IPv6): 2001:0:30:221::/64 Metric: 10 Type: 1 Up
    Arista-PE32-Q2C-32.00-00       193  54182   843    432 L2  0000.0000.0032.00-00  <>
      LSP generation remaining wait time: 0 ms
      Time remaining until refresh: 543 s
      NLPID: 0xCC(IPv4) 0x8E(IPv6)
      Hostname: Arista-PE32-Q2C-32
      Area addresses: 49.0001
      Topology: 2 (IPv6)
      Topology: 0 (IPv4)
      Interface address: 20.32.175.32
      Interface address: 20.30.32.32
      Interface address: 10.0.0.32
      Interface address: 2001:0:32:175::32
      Interface address: 2001:0:30:32::32
      IS Neighbor          : Juniper-175-ACX7100-48L.00 Metric: 10
        IPv4 Neighbor Address: 20.32.175.175
        IPv4 Interface Address: 20.32.175.32
        Adj-sid: 362167 flags: [L V] weight: 0x0
      IS Neighbor          : Arista-Spine3-Q2A-30.00 Metric: 10
        IPv4 Neighbor Address: 20.30.32.30
        IPv4 Interface Address: 20.30.32.32
        Adj-sid: 362165 flags: [L V] weight: 0x0
      IS Neighbor (MT-IPv6): Arista-Spine3-Q2A-30.00 Metric: 10
        IPv6 Neighbor Address: 2001:0:30:32::30
        Global IPv6 Interface Address: 2001:0:30:32::32
        Adj-sid: 362166 flags: [L V F] weight: 0x0
      Reachability         : 10.0.0.32/32 Metric: 0 Type: 1 Up
        SR Prefix-SID: 32 Flags: [N] Algorithm: 0
        SR Prefix-SID: 1161 Flags: [N] Algorithm: 128
        SR Prefix-SID: 1162 Flags: [N] Algorithm: 129
        SR Prefix-SID: 1163 Flags: [N] Algorithm: 130
      Reachability         : 20.32.175.0/24 Metric: 10 Type: 1 Up
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
        Algorithms:  0, 128, 129, 130
    Arrcus-53.00-00             407  57015   932    278 L2  0000.0000.0053.00-00  <>
      Remaining lifetime received: 1199 s Modified to: 1200 s
      NLPID: 0xCC(IPv4)
      Hostname: Arrcus-53
      Area addresses: 49.0001
      Interface address: 10.0.0.53
      IS Neighbor          : Arista-Spine3-Q2A-30.00 Metric: 10
        IPv4 Neighbor Address: 20.30.53.30
        IPv4 Interface Address: 20.30.53.53
        Adj-sid: 30000 flags: [L V] weight: 0x0
      IS Neighbor          : Juniper-175-ACX7100-48L.00 Metric: 10
        IPv4 Neighbor Address: 20.53.175.175
        IPv4 Interface Address: 20.53.175.53
      Reachability         : 20.30.53.0/24 Metric: 10 Type: 1 Up
      Reachability         : 20.53.175.0/24 Metric: 10 Type: 1 Up
      Reachability         : 10.0.0.53/32 Metric: 0 Type: 1 Up
        SR Prefix-SID: 53 Flags: [N P E] Algorithm: 0
        SR Prefix-SID: 1181 Flags: [N] Algorithm: 128
        SR Prefix-SID: 1182 Flags: [N] Algorithm: 129
        SR Prefix-SID: 1183 Flags: [N] Algorithm: 130
      Router Capabilities: Router Id: 10.0.0.53 Flags: []
        SR Local Block:
          SRLB Base: 30000 Range: 2001
        SR Capability: Flags: [I V]
          SRGB Base: 20000 Range: 2000
        Algorithms:  0, 128, 129, 130
 U  Arrcus-36D-3-57.00-00       200  26364 39302    331 L2  0000.0000.0057.00-00  <>
      NLPID: 0x8E(IPv6)
      Hostname: Arrcus-36D-3-57
      Area addresses: 49.0002
      Interface address: 2002::57
      IS Neighbor          : 0000.0000.0130.00   Metric: 11
        Global IPv6 Interface Address: 2001:0:57:130::57
      Reachability          : 5f00:0:2057::/48 Metric: 10 Type: 1 Up
      Reachability          : 2001:0:57:130::/64 Metric: 11 Type: 1 Up
      Reachability          : 2001:0:57:169::/64 Metric: 10 Type: 1 Up
      Reachability          : 2002::57/128 Metric: 0 Type: 1 Up
      SRv6 Locator: 5f00:0:2057::/48 Topology: 0
        Metric: 10 Algorithm: 0 Flags: []
        SRv6 SID End with NEXT-CSID PSP USD
          SID : 5f00:0:2057::
          SID structure: Block length: 32 Node length: 16
                         Function length: 0 Argument length: 0
      Router Capabilities: Router Id: 0.0.0.0 Flags: []
        SRv6 Capability: Flags: []
        Algorithms:  0
 U  Arrcus-36D-3-57.00-01       211  40105 39803    187 L2  0000.0000.0057.00-01  <>
      IS Neighbor          : 0000.0000.0042.00   Metric: 10
        Global IPv6 Interface Address: 2001:0:42:57::57
      IS Neighbor          : 0000.0000.0169.00   Metric: 10
        Global IPv6 Interface Address: 2001:0:57:169::57
      Reachability          : 2001:0:42:57::/64 Metric: 10 Type: 1 Up
 U  Ciena-5134-72.00-00         512  34876    34    469 L2  0000.0000.0072.00-00  <>
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
      Reachability         : 10.0.0.72/32 Metric: 10 Type: 1 Up
        SR Prefix-SID: 72 Flags: [N] Algorithm: 0
        SR Prefix-SID: 1200 Flags: [N] Algorithm: 128
        SR Prefix-SID: 1201 Flags: [N] Algorithm: 129
        SR Prefix-SID: 1202 Flags: [N] Algorithm: 130
      Reachability         : 20.30.72.0/24 Metric: 10 Type: 1 Up
      Router Capabilities: Router Id: 10.0.0.72 Flags: []
        SR Capability: Flags: [I]
          SRGB Base: 20000 Range: 2000
        Algorithms:  0, 128, 129, 130
    Ericsson_84_R6678.00-00       277  42964   757    277 L2  0000.0000.0084.00-00  <>
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
      IS Neighbor (MT-IPv6): Arista-Spine3-Q2A-30.00 Metric: 10
        IPv6 Neighbor Address: 2001:0:30:84::30
        Global IPv6 Interface Address: 2001:0:30:84::175
      Reachability         : 10.0.0.84/32 Metric: 10 Type: 1 Up
        SR Prefix-SID: 84 Flags: [N P] Algorithm: 0
      Reachability (MT-IPv6): 2001:0:30:84::/64 Metric: 10 Type: 1 Up
      Reachability (MT-IPv6): 2001:0:84:175::/64 Metric: 10 Type: 1 Up
      Router Capabilities: Router Id: 10.0.0.84 Flags: []
        Maximum SID depth:
          Base MPLS imposition (MSD type 1):  8
        SR Capability: Flags: [I]
          SRGB Base: 20000 Range: 2000
        Algorithms:  0
    H3C_M1A_120.00-00          1732  10714  1198   1121 L2  0000.0000.0120.00-00  <>
      Remaining lifetime received: 1197 s Modified to: 1200 s
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
      IS Neighbor          : Arista-Spine3-Q2A-30.00 Metric: 100
        IPv4 Neighbor Address: 20.30.120.30
        IPv4 Interface Address: 20.30.120.120
        Adj-sid: 1140 flags: [L V] weight: 0x0
      IS Neighbor          : Arista-Spine3-Q2A-30.00 Metric: 100
        IPv4 Neighbor Address: 20.30.120.30
        IPv4 Interface Address: 20.30.120.120
      IS Neighbor          : Juniper-175-ACX7100-48L.00 Metric: 10
        IPv4 Neighbor Address: 20.120.175.175
        IPv4 Interface Address: 20.120.175.120
        Adj-sid: 1141 flags: [L V] weight: 0x0
      IS Neighbor          : Juniper-175-ACX7100-48L.00 Metric: 10
        IPv4 Neighbor Address: 20.120.175.175
        IPv4 Interface Address: 20.120.175.120
      IS Neighbor (MT-IPv6): Arista-Spine3-Q2A-30.00 Metric: 10
        IPv6 Neighbor Address: 2001:0:30:120::30
        Global IPv6 Interface Address: 2001:0:30:120::120
      IS Neighbor (MT-IPv6): Arista-Spine3-Q2A-30.00 Metric: 10
        IPv6 Neighbor Address: 2001:0:30:120::30
        Global IPv6 Interface Address: 2001:0:30:120::120
      Reachability         : 10.0.0.120/32 Metric: 0 Type: 1 Up
        SR Prefix-SID: 120 Flags: [N] Algorithm: 0
        SR Prefix-SID: 1248 Flags: [N P] Algorithm: 128
        SR Prefix-SID: 1249 Flags: [N P] Algorithm: 129
        SR Prefix-SID: 1250 Flags: [N P] Algorithm: 130
      Reachability         : 20.30.120.0/24 Metric: 100 Type: 1 Up
      Reachability         : 20.120.175.0/24 Metric: 10 Type: 1 Up
      Reachability         : 20.120.214.0/24 Metric: 10 Type: 1 Up
      Reachability         : 20.120.217.0/24 Metric: 0 Type: 1 Up
      Reachability         : 192.168.20.0/23 Metric: 0 Type: 1 Up
      Reachability (MT-IPv6): 2001:0:30:120::/64 Metric: 10 Type: 1 Up
      Reachability (MT-IPv6): 2001:0:120:175::/64 Metric: 10 Type: 1 Up
      Reachability (MT-IPv6): 2001:0:120:214::/64 Metric: 10 Type: 1 Up
      Router Capabilities: Router Id: 10.0.0.120 Flags: []
        Maximum SID depth:
          Base MPLS imposition (MSD type 1):  13
        SR Capability: Flags: [I]
          SRGB Base: 20000 Range: 2000
        Algorithms:  0, 128, 129, 130
        Flex Algo: Algorithm: 128 Metric: Min Unidirectional Delay Metric (1) Calc: SPF (0) Prio: 128
          Flags: [M] 0x80
        Flex Algo: Algorithm: 129 Metric: TE Metric (2) Calc: SPF (0) Prio: 128
          Flags: [M] 0x80
        Flex Algo: Algorithm: 130 Metric: IGP Metric (0) Calc: SPF (0) Prio: 128
          Exclude admin groups: 1
          Flags: [M] 0x80
    0000.0000.0124.00-00        159  33805   478    453 L2  0000.0000.0124.00-00  <>
      Remaining lifetime received: 1199 s Modified to: 1200 s
      NLPID: 0xCC(IPv4) 0x8E(IPv6)
      Area addresses: 49.0001
      Topology: 0 (IPv4)
      Topology: 2 (IPv6)
      Interface address: 20.124.175.124
      Interface address: 20.30.124.124
      Interface address: 10.0.0.124
      IS Neighbor          : Arista-Spine3-Q2A-30.00 Metric: 10
        IPv4 Neighbor Address: 20.30.124.30
        IPv4 Interface Address: 20.30.124.124
        Adj-sid: 397 flags: [L V] weight: 0x0
      IS Neighbor          : Juniper-175-ACX7100-48L.00 Metric: 10
        IPv4 Neighbor Address: 20.124.175.175
        IPv4 Interface Address: 20.124.175.124
        Adj-sid: 396 flags: [L V] weight: 0x0
      Reachability         : 20.30.124.0/24 Metric: 10 Type: 1 Up
      Reachability         : 20.124.175.0/24 Metric: 10 Type: 1 Up
      Reachability         : 10.0.0.124/32 Metric: 0 Type: 1 Up
        SR Prefix-SID: 124 Flags: [N P] Algorithm: 0
        SR Prefix-SID: 1252 Flags: [N P] Algorithm: 128
        SR Prefix-SID: 1253 Flags: [N P] Algorithm: 129
        SR Prefix-SID: 1254 Flags: [N P] Algorithm: 130
      Router Capabilities: Router Id: 10.0.0.124 Flags: []
        Maximum SID depth:
          Base MPLS imposition (MSD type 1):  10
        SR Capability: Flags: [I]
          SRGB Base: 2000 Range: 2001
        Algorithms:  0, 128, 129, 130
      Router Capabilities: Router Id: 10.0.0.124 Flags: []
        Flex Algo: Algorithm: 128 Metric: Min Unidirectional Delay Metric (1) Calc: SPF (0) Prio: 128
          Flags: [M] 0x80
        Flex Algo: Algorithm: 129 Metric: TE Metric (2) Calc: SPF (0) Prio: 128
          Flags: [M] 0x80
        Flex Algo: Algorithm: 130 Metric: IGP Metric (0) Calc: SPF (0) Prio: 128
          Exclude admin groups: 1
          Flags: [M] 0x80
    0000.0000.0128.00-00        174  15511   652    453 L2  0000.0000.0128.00-00  <>
      Remaining lifetime received: 1199 s Modified to: 1200 s
      NLPID: 0xCC(IPv4) 0x8E(IPv6)
      Area addresses: 49.0001
      Topology: 0 (IPv4)
      Topology: 2 (IPv6)
      Interface address: 10.0.0.128
      Interface address: 20.128.175.128
      Interface address: 20.30.128.128
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
        SR Prefix-SID: 1256 Flags: [N] Algorithm: 128
        SR Prefix-SID: 1257 Flags: [N] Algorithm: 129
        SR Prefix-SID: 1258 Flags: [N] Algorithm: 130
      Reachability         : 20.128.175.0/24 Metric: 10 Type: 1 Up
      Reachability         : 20.30.128.0/24 Metric: 10 Type: 1 Up
      Router Capabilities: Router Id: 10.0.0.128 Flags: []
        Maximum SID depth:
          Base MPLS imposition (MSD type 1):  10
        SR Capability: Flags: [I]
          SRGB Base: 20000 Range: 2000
        Algorithms:  0, 128, 129, 130
      Router Capabilities: Router Id: 10.0.0.128 Flags: []
        Flex Algo: Algorithm: 128 Metric: Min Unidirectional Delay Metric (1) Calc: SPF (0) Prio: 128
          Flags: [M] 0x80
        Flex Algo: Algorithm: 129 Metric: TE Metric (2) Calc: SPF (0) Prio: 128
          Flags: [M] 0x80
        Flex Algo: Algorithm: 130 Metric: IGP Metric (0) Calc: SPF (0) Prio: 128
          Exclude admin groups: 1
          Flags: [M] 0x80
    Juniper-131-JCNR.00-00        22  36182   437    447 L2  0000.0000.0131.00-00  <>
      Remaining lifetime received: 1199 s Modified to: 1200 s
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
        Adj-sid: 21 flags: [L V F] weight: 0x0
        Adj-sid: 20 flags: [L V] weight: 0x0
      IS Neighbor          : Arista-Spine3-Q2A-30.00 Metric: 10
        IPv4 Neighbor Address: 20.30.131.30
        IPv4 Interface Address: 20.30.131.131
        IPv6 Neighbor Address: 2001:0:30:131::30
        Global IPv6 Interface Address: 2001:0:30:131::131
        Adj-sid: 23 flags: [L V F] weight: 0x0
        Adj-sid: 22 flags: [L V] weight: 0x0
      Reachability         : 20.131.175.0/24 Metric: 10 Type: 1 Up
      Reachability         : 10.0.0.131/32 Metric: 0 Type: 1 Up
        SR Prefix-SID: 131 Flags: [N] Algorithm: 0
      Reachability         : 20.30.131.0/24 Metric: 10 Type: 1 Up
      Reachability          : 2001:0:131:175::/64 Metric: 10 Type: 1 Up
      Reachability          : fe80::ec97:fbff:fe06:5964/128 Metric: 0 Type: 1 Up
      Reachability          : 2001:0:30:131::/64 Metric: 10 Type: 1 Up
      Router Capabilities: Router Id: 10.0.0.131 Flags: []
        Maximum SID depth:
          Base MPLS imposition (MSD type 1):  0
        SR Capability: Flags: [I V]
          SRGB Base: 20000 Range: 2000
        Algorithms:  0, 1, 128, 129, 130
      Unsupported TLV: Type: 14 Length: 2
    Juniper-156-PTX10002-36QDD.00-00        69  52849   854    561 L2  0000.0000.0156.00-00  <>
      Remaining lifetime received: 1199 s Modified to: 1200 s
      NLPID: 0xCC(IPv4) 0x8E(IPv6)
      Hostname: Juniper-156-PTX10002-36QDD
      Area addresses: 49.0001
      Interface address: 10.0.0.156
      Interface address: 127.0.0.1
      IS Neighbor          : Juniper-175-ACX7100-48L.00 Metric: 10
        IPv4 Neighbor Address: 20.156.175.175
        IPv4 Interface Address: 20.156.175.156
        IPv6 Neighbor Address: 2001:0:156:175::175
        Global IPv6 Interface Address: 2001:0:156:175::156
        Adj-sid: 18 flags: [L V F] weight: 0x0
        Adj-sid: 17 flags: [L V] weight: 0x0
      IS Neighbor          : Arista-Spine3-Q2A-30.00 Metric: 4000
        IPv4 Neighbor Address: 20.30.156.30
        IPv4 Interface Address: 20.30.156.156
        IPv6 Neighbor Address: 2001:0:30:156::30
        Global IPv6 Interface Address: 2001:0:30:156::156
        Adj-sid: 20 flags: [L V F] weight: 0x0
        Adj-sid: 19 flags: [L V] weight: 0x0
      Reachability         : 10.0.0.156/32 Metric: 0 Type: 1 Up
        SR Prefix-SID: 156 Flags: [N] Algorithm: 0
        SR Prefix-SID: 1286 Flags: [N] Algorithm: 130
        SR Prefix-SID: 1285 Flags: [N] Algorithm: 129
        SR Prefix-SID: 1284 Flags: [N] Algorithm: 128
      Reachability         : 20.156.175.0/24 Metric: 10 Type: 1 Up
      Reachability         : 127.0.0.1/32 Metric: 0 Type: 1 Up
      Reachability         : 20.30.156.0/24 Metric: 4000 Type: 1 Up
      Reachability          : 2001:0:156:175::/64 Metric: 10 Type: 1 Up
      Reachability          : 2001:0:30:156::/64 Metric: 4000 Type: 1 Up
      Router Capabilities: Router Id: 10.0.0.156 Flags: []
        Maximum SID depth:
          Base MPLS imposition (MSD type 1):  0
        SR Capability: Flags: [I V]
          SRGB Base: 20000 Range: 2000
        Algorithms:  0, 1, 128, 129, 130
      Unsupported TLV: Type: 14 Length: 2
    Juniper-175-ACX7100-48L.00-00       283  47243  1199   1097 L2  0000.0000.0175.00-00  <>
      Remaining lifetime received: 1198 s Modified to: 1200 s
      NLPID: 0xCC(IPv4) 0x8E(IPv6)
      Hostname: Juniper-175-ACX7100-48L
      Area addresses: 49.0001
      Interface address: 10.0.0.175
      Interface address: 127.0.0.1
      Interface address: 2001:0:32:175::175
      IS Neighbor          : Juniper-131-JCNR.00 Metric: 15
        IPv4 Neighbor Address: 20.131.175.131
        IPv4 Interface Address: 20.131.175.175
        IPv6 Neighbor Address: 2001:0:131:175::131
        Global IPv6 Interface Address: 2001:0:131:175::175
        Adj-sid: 116 flags: [L V F] weight: 0x0
        Adj-sid: 115 flags: [L V] weight: 0x0
      IS Neighbor          : Nokia-SR1-217.00    Metric: 15
        IPv4 Neighbor Address: 20.175.217.217
        IPv4 Interface Address: 20.175.217.175
        IPv6 Neighbor Address: 2001:0:175:217::217
        Global IPv6 Interface Address: 2001:0:175:217::175
        Adj-sid: 98 flags: [L V F] weight: 0x0
        Adj-sid: 97 flags: [L V] weight: 0x0
      IS Neighbor          : Juniper-179-ACX7024.00 Metric: 15
        IPv4 Neighbor Address: 20.175.179.179
        IPv4 Interface Address: 20.175.179.175
        IPv6 Neighbor Address: 2001:0:175::179:179
        Global IPv6 Interface Address: 2001:0:175::179:175
        Adj-sid: 106 flags: [L V F] weight: 0x0
        Adj-sid: 105 flags: [L V] weight: 0x0
      IS Neighbor          : H3C_M1A_120.00      Metric: 15
        IPv4 Neighbor Address: 20.120.175.120
        IPv4 Interface Address: 20.120.175.175
        IPv6 Neighbor Address: 2001:0:120:175::120
        Global IPv6 Interface Address: 2001:0:120:175::175
        Adj-sid: 110 flags: [L V F] weight: 0x0
        Adj-sid: 109 flags: [L V] weight: 0x0
      Reachability         : 20.131.175.0/24 Metric: 15 Type: 1 Up
      Reachability         : 20.175.217.0/24 Metric: 15 Type: 1 Up
      Reachability         : 20.84.175.0/24 Metric: 15 Type: 1 Up
      Reachability         : 20.128.175.0/24 Metric: 15 Type: 1 Up
      Reachability         : 20.175.184.0/24 Metric: 15 Type: 1 Up
      Reachability         : 20.124.175.0/24 Metric: 15 Type: 1 Up
      Reachability         : 20.175.214.0/24 Metric: 15 Type: 1 Up
      Reachability         : 20.32.175.0/24 Metric: 15 Type: 1 Up
      Reachability         : 20.175.179.0/24 Metric: 15 Type: 1 Up
      Reachability         : 20.156.175.0/24 Metric: 10 Type: 1 Up
      Reachability         : 20.120.175.0/24 Metric: 15 Type: 1 Up
      Reachability         : 20.53.175.0/24 Metric: 15 Type: 1 Up
      Reachability         : 127.0.0.1/32 Metric: 0 Type: 1 Up
      Reachability         : 10.0.0.175/32 Metric: 0 Type: 1 Up
        SR Prefix-SID: 175 Flags: [N] Algorithm: 0
        SR Prefix-SID: 1305 Flags: [N] Algorithm: 130
        SR Prefix-SID: 1304 Flags: [N] Algorithm: 129
        SR Prefix-SID: 1303 Flags: [N] Algorithm: 128
      Reachability         : 20.175.221.0/24 Metric: 15 Type: 1 Up
      Reachability          : 2001:0:131:175::/64 Metric: 15 Type: 1 Up
      Reachability          : 2001:0:175:217::/64 Metric: 15 Type: 1 Up
      Reachability          : 2001:0:84:175::/64 Metric: 15 Type: 1 Up
      Reachability          : 2001:0:128:175::/64 Metric: 15 Type: 1 Up
      Reachability          : 2001:0:175:184::/64 Metric: 15 Type: 1 Up
      Reachability          : 2001:0:175:214::/64 Metric: 15 Type: 1 Up
      Reachability          : 2001:0:32:175::/64 Metric: 15 Type: 1 Up
      Reachability          : 2001:0:175::/64 Metric: 15 Type: 1 Up
      Reachability          : 2001:0:156:175::/64 Metric: 10 Type: 1 Up
      Reachability          : 2001:0:120:175::/64 Metric: 15 Type: 1 Up
      Reachability          : 2001:0:53:175::/64 Metric: 15 Type: 1 Up
      Reachability          : 2001:0:175:221::/64 Metric: 15 Type: 1 Up
      Router Capabilities: Router Id: 10.0.0.175 Flags: []
        Maximum SID depth:
          Base MPLS imposition (MSD type 1):  3
        SR Capability: Flags: [I V]
          SRGB Base: 20000 Range: 2000
        Algorithms:  0, 1, 128, 129, 130
        Flex Algo: Algorithm: 130 Metric: IGP Metric (0) Calc: SPF (0) Prio: 238
          Exclude admin groups: 2
          Flags: [M] 0x80
        Flex Algo: Algorithm: 129 Metric: TE Metric (2) Calc: SPF (0) Prio: 238
          Flags: [M] 0x80
        Flex Algo: Algorithm: 128 Metric: Min Unidirectional Delay Metric (1) Calc: SPF (0) Prio: 0
          Flags: [M] 0x80
      Unsupported TLV: Type: 14 Length: 2
    Juniper-175-ACX7100-48L.00-01       175  38018  1024   1165 L2  0000.0000.0175.00-01  <>
      Remaining lifetime received: 1198 s Modified to: 1200 s
      IS Neighbor          : 221.00              Metric: 15
        IPv4 Neighbor Address: 20.175.221.221
        IPv4 Interface Address: 20.175.221.175
        Global IPv6 Interface Address: 2001:0:175:221::175
        Adj-sid: 119 flags: [L V F] weight: 0x0
        Adj-sid: 118 flags: [L V] weight: 0x0
      IS Neighbor          : Ericsson_84_R6678.00 Metric: 15
        IPv4 Neighbor Address: 20.84.175.84
        IPv4 Interface Address: 20.84.175.175
        IPv6 Neighbor Address: 2001:0:84:175::175
        Global IPv6 Interface Address: 2001:0:84:175::175
        Adj-sid: 95 flags: [L V F] weight: 0x0
        Adj-sid: 94 flags: [L V] weight: 0x0
      IS Neighbor          : 0000.0000.0128.00   Metric: 15
        IPv4 Neighbor Address: 20.128.175.128
        IPv4 Interface Address: 20.128.175.175
        Global IPv6 Interface Address: 2001:0:128:175::175
        Adj-sid: 96 flags: [L V] weight: 0x0
      IS Neighbor          : 0000.0000.0184.00   Metric: 15
        IPv4 Neighbor Address: 20.175.184.184
        IPv4 Interface Address: 20.175.184.175
        Global IPv6 Interface Address: 2001:0:175:184::175
        Adj-sid: 117 flags: [L V] weight: 0x0
      IS Neighbor          : 0000.0000.0124.00   Metric: 15
        IPv4 Neighbor Address: 20.124.175.124
        IPv4 Interface Address: 20.124.175.175
        Adj-sid: 102 flags: [L V] weight: 0x0
      IS Neighbor          : Nokia-SXR-214.00    Metric: 15
        IPv4 Neighbor Address: 20.175.214.214
        IPv4 Interface Address: 20.175.214.175
        IPv6 Neighbor Address: 2001:0:175:214::214
        Global IPv6 Interface Address: 2001:0:175:214::175
        Adj-sid: 108 flags: [L V F] weight: 0x0
        Adj-sid: 107 flags: [L V] weight: 0x0
      IS Neighbor          : Arista-PE32-Q2C-32.00 Metric: 15
        IPv4 Neighbor Address: 20.32.175.32
        IPv4 Interface Address: 20.32.175.175
        IPv6 Neighbor Address: 2001:0:32:175::32
        Global IPv6 Interface Address: 2001:0:32:175::175
        Adj-sid: 104 flags: [L V F] weight: 0x0
        Adj-sid: 103 flags: [L V] weight: 0x0
      IS Neighbor          : Juniper-156-PTX10002-36QDD.00 Metric: 10
        IPv4 Neighbor Address: 20.156.175.156
        IPv4 Interface Address: 20.156.175.175
        IPv6 Neighbor Address: 2001:0:156:175::156
        Global IPv6 Interface Address: 2001:0:156:175::175
        Adj-sid: 101 flags: [L V F] weight: 0x0
        Adj-sid: 100 flags: [L V] weight: 0x0
      IS Neighbor          : Arrcus-53.00        Metric: 15
        IPv4 Neighbor Address: 20.53.175.53
        IPv4 Interface Address: 20.53.175.175
        Global IPv6 Interface Address: 2001:0:53:175::175
        Adj-sid: 99 flags: [L V] weight: 0x0
    Juniper-179-ACX7024.00-00       178  14024  1058    554 L2  0000.0000.0179.00-00  <>
      Remaining lifetime received: 1199 s Modified to: 1200 s
      NLPID: 0xCC(IPv4) 0x8E(IPv6)
      Hostname: Juniper-179-ACX7024
      Area addresses: 49.0001
      Interface address: 10.0.0.179
      Interface address: 127.0.0.1
      IS Neighbor          : Arista-Spine3-Q2A-30.00 Metric: 4000
        IPv4 Neighbor Address: 20.30.179.30
        IPv4 Interface Address: 20.30.179.179
        IPv6 Neighbor Address: 2001:0:30:179::30
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
        SR Prefix-SID: 1309 Flags: [N] Algorithm: 130
        SR Prefix-SID: 1308 Flags: [N] Algorithm: 129
        SR Prefix-SID: 1307 Flags: [N] Algorithm: 128
      Reachability         : 20.175.179.0/24 Metric: 10 Type: 1 Up
      Reachability         : 127.0.0.1/32 Metric: 0 Type: 1 Up
      Reachability         : 20.30.179.0/24 Metric: 4000 Type: 1 Up
      Reachability          : 2001:0:175::/64 Metric: 10 Type: 1 Up
      Reachability          : 2001:0:30:179::/64 Metric: 4000 Type: 1 Up
      Router Capabilities: Router Id: 10.0.0.179 Flags: []
        Maximum SID depth:
          Base MPLS imposition (MSD type 1):  8
        SR Capability: Flags: [I V]
          SRGB Base: 20000 Range: 2000
        Algorithms:  0, 1, 128, 129, 130
      Unsupported TLV: Type: 14 Length: 2
    0000.0000.0184.00-00       2457   9057  1199    253 L2  0000.0000.0184.00-00  <DefaultAtt>
      Remaining lifetime received: 1197 s Modified to: 1200 s
      NLPID: 0xCC(IPv4) 0x8E(IPv6) 0x81(CLNP)
      Area addresses:
        49.0001
        49.0002
      Interface address: 20.30.184.184
      IS Neighbor          : Arista-Spine3-Q2A-30.00 Metric: 10
        Adj-sid: 9001 flags: [L V] weight: 0x0
      Reachability         : 10.0.0.184/32 Metric: 10 Type: 1 Up
        SR Prefix-SID: 20184 Flags: [N] Algorithm: 0
      Reachability         : 20.30.184.0/24 Metric: 10 Type: 1 Up
      Reachability         : 10.0.0.184/32 Metric: 0 Type: 1 Up
        SR Prefix-SID: 1312 Flags: [N] Algorithm: 128
        SR Prefix-SID: 1313 Flags: [N] Algorithm: 129
        SR Prefix-SID: 1314 Flags: [N] Algorithm: 130
        SR Prefix-SID: 184 Flags: [N] Algorithm: 0
      Router Capabilities: Router Id: 10.0.0.184 Flags: []
        SR Capability: Flags: [I V]
          SRGB Base: 20000 Range: 2000
        Algorithms:  0, 128, 129, 130
    Nokia-SXR-214.00-00        8824  51377  1085    488 L2  0000.0000.0214.00-00  <>
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
      IS Neighbor          : Arista-Spine3-Q2A-30.00 Metric: 10
        IPv4 Neighbor Address: 20.30.214.30
        IPv4 Interface Address: 20.30.214.214
        Adj-sid: 30018 flags: [L V B] weight: 0x0
        Adj-sid: 30019 flags: [L V B F] weight: 0x0
      IS Neighbor          : Nokia-IXRe2-216.00  Metric: 10
        IPv4 Neighbor Address: 20.214.216.216
        IPv4 Interface Address: 20.214.216.214
        IPv6 Neighbor Address: 2001:0:214:216::216
        Global IPv6 Interface Address: 2001:0:214:216::214
        Adj-sid: 30021 flags: [L V B] weight: 0x0
        Adj-sid: 30022 flags: [L V B F] weight: 0x0
      IS Neighbor          : Juniper-175-ACX7100-48L.00 Metric: 10
        IPv4 Neighbor Address: 20.175.214.175
        IPv4 Interface Address: 20.175.214.214
        IPv6 Neighbor Address: 2001:0:175:214::175
        Global IPv6 Interface Address: 2001:0:175:214::214
        Adj-sid: 30023 flags: [L V B] weight: 0x0
        Adj-sid: 30024 flags: [L V B F] weight: 0x0
      Reachability         : 20.30.214.0/24 Metric: 10 Type: 1 Up
      Reachability         : 20.175.214.0/24 Metric: 10 Type: 1 Up
      Reachability         : 20.214.216.0/24 Metric: 10 Type: 1 Up
      Reachability         : 10.0.0.214/32 Metric: 0 Type: 1 Up
        SR Prefix-SID: 214 Flags: [N P] Algorithm: 0
      Reachability          : 2000::214/128 Metric: 0 Type: 1 Up
      Reachability          : 2001:0:175:214::/64 Metric: 10 Type: 1 Up
      Reachability          : 2001:0:214:216::/64 Metric: 10 Type: 1 Up
      Router Capabilities: Router Id: 10.0.0.214 Flags: []
        Maximum SID depth:
          Base MPLS imposition (MSD type 1):  15
        SR Capability: Flags: [I V]
          SRGB Base: 20000 Range: 2000
        Algorithms:  0
    Nokia-IXRe2-216.00-00      1022  27357  1109    435 L2  0100.0000.0216.00-00  <>
      Remaining lifetime received: 1199 s Modified to: 1200 s
      NLPID: 0xCC(IPv4) 0x8E(IPv6)
      Hostname: Nokia-IXRe2-216
      Area addresses: 49.0001.0000.0000.0216.00
      Topology: 0 (IPv4)
      Topology: 2 (IPv6)
      Interface address: 10.0.0.216
      Interface address: 20.214.216.216
      Interface address: 2001:0:214:216::216
      Interface address: 2002::216
      IS Neighbor          : Nokia-SXR-214.00    Metric: 10
        IPv4 Neighbor Address: 20.214.216.214
        IPv4 Interface Address: 20.214.216.216
        IPv6 Neighbor Address: 2001:0:214:216::214
        Global IPv6 Interface Address: 2001:0:214:216::216
        Adj-sid: 1048575 flags: [L V B] weight: 0x0
        Adj-sid: 1048574 flags: [L V B F] weight: 0x0
      Reachability         : 20.214.216.0/24 Metric: 10 Type: 1 Up
      Reachability         : 10.0.0.216/32 Metric: 0 Type: 1 Up
      Reachability          : 2001:0:214:216::/64 Metric: 10 Type: 1 Up
      Reachability          : 2002::216/128 Metric: 0 Type: 1 Up
      Reachability          : 5f00:0:2216::/48 Metric: 0 Type: 1 Up
      Reachability (MT-IPv6): 2001:0:214:216::/64 Metric: 10 Type: 1 Up
      Reachability (MT-IPv6): 2002::216/128 Metric: 0 Type: 1 Up
      SRv6 Locator: 5f00:0:2216::/48 Topology: 0
        Metric: 0 Algorithm: 0 Flags: []
        SRv6 SID End with NEXT-CSID PSP
          SID : 5f00:0:2216::
          SID structure: Block length: 32 Node length: 16
                         Function length: 0 Argument length: 80
      Router Capabilities: Router Id: 10.0.0.216 Flags: []
        Maximum SID depth:
          Base MPLS imposition (MSD type 1):  11
        SRv6 Capability: Flags: []
        SR Capability: Flags: [I V]
          SRGB Base: 20000 Range: 2000
        Algorithms:  0
    Nokia-SR1-217.00-00         367  26297   969    545 L2  0100.0000.0217.00-00  <>
      Remaining lifetime received: 1199 s Modified to: 1200 s
      NLPID: 0xCC(IPv4) 0x8E(IPv6)
      Hostname: Nokia-SR1-217
      Area addresses: 49.0001.0000.0000.0217.00
      Topology: 0 (IPv4)
      Topology: 2 (IPv6)
      Interface address: 10.0.0.217
      Interface address: 20.30.217.217
      Interface address: 20.175.217.217
      Interface address: 2001:0:175:217::217
      Interface address: 2002::217
      IS Neighbor          : Arista-Spine3-Q2A-30.00 Metric: 10
        IPv4 Neighbor Address: 20.30.217.30
        IPv4 Interface Address: 20.30.217.217
        Adj-sid: 524282 flags: [L V B] weight: 0x0
        Adj-sid: 524281 flags: [L V B F] weight: 0x0
      IS Neighbor          : Juniper-175-ACX7100-48L.00 Metric: 10
        IPv4 Neighbor Address: 20.175.217.175
        IPv4 Interface Address: 20.175.217.217
        IPv6 Neighbor Address: 2001:0:175:217::175
        Global IPv6 Interface Address: 2001:0:175:217::217
        Adj-sid: 524286 flags: [L V B] weight: 0x0
        Adj-sid: 524285 flags: [L V B F] weight: 0x0
      Reachability         : 10.0.0.217/32 Metric: 0 Type: 1 Up
        SR Prefix-SID: 217 Flags: [N P] Algorithm: 0
        SR Prefix-SID: 1345 Flags: [N P] Algorithm: 128
        SR Prefix-SID: 1346 Flags: [N P] Algorithm: 129
        SR Prefix-SID: 1347 Flags: [N P] Algorithm: 130
      Reachability         : 20.30.217.0/24 Metric: 10 Type: 1 Up
      Reachability         : 20.175.217.0/24 Metric: 10 Type: 1 Up
      Reachability          : 2001:0:175:217::/64 Metric: 10 Type: 1 Up
      Reachability          : 2002::217/128 Metric: 0 Type: 1 Up
      Reachability (MT-IPv6): 2001:0:175:217::/64 Metric: 10 Type: 1 Up
      Reachability (MT-IPv6): 2002::217/128 Metric: 0 Type: 1 Up
      Router Capabilities: Router Id: 10.0.0.217 Flags: []
        Maximum SID depth:
          Base MPLS imposition (MSD type 1):  12
        SR Capability: Flags: [I V]
          SRGB Base: 20000 Range: 2000
        Algorithms:  0, 128, 129, 130
        Flex Algo: Algorithm: 128 Metric: Min Unidirectional Delay Metric (1) Calc: SPF (0) Prio: 100
          Flags: [M] 0x80
        Flex Algo: Algorithm: 129 Metric: TE Metric (2) Calc: SPF (0) Prio: 100
          Flags: [M] 0x80
        Flex Algo: Algorithm: 130 Metric: IGP Metric (0) Calc: SPF (0) Prio: 100
          Exclude admin groups: 1
          Flags: [M] 0x80
    221.00-00                   186  13554   808     86 L2  0221.0221.0221.00-00  <>
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
        Algorithms:  0, 128, 129, 130
      Unsupported TLV: Type: 14 Length: 2
    221.00-01                   147  47140   461     32 L2  0221.0221.0221.00-01  <>
      Remaining lifetime received: 1199 s Modified to: 1200 s
      Hostname: 221
    221.00-02                  5304  55661  1198    491 L2  0221.0221.0221.00-02  <>
      Remaining lifetime received: 1199 s Modified to: 1200 s
      Interface address: 10.0.0.221
      Interface address: 20.175.221.221
      Interface address: 20.30.221.221
      Interface address: 1221::1
      Interface address: 2001:0:175:221::221
      Interface address: 2001:0:30:221::221
      IS Neighbor          : Juniper-175-ACX7100-48L.00 Metric: 10
        IPv4 Neighbor Address: 20.175.221.175
        IPv4 Interface Address: 20.175.221.221
        Adj-sid: 524294 flags: [L V B] weight: 0x0
        Adj-sid: 524289 flags: [L V] weight: 0x0
      IS Neighbor          : Arista-Spine3-Q2A-30.00 Metric: 100
        IPv4 Neighbor Address: 20.30.221.30
        IPv4 Interface Address: 20.30.221.221
        Adj-sid: 524293 flags: [L V B] weight: 0x0
        Adj-sid: 524292 flags: [L V] weight: 0x0
      Reachability         : 10.0.0.221/32 Metric: 0 Type: 1 Up
        SR Prefix-SID: 221 Flags: [N] Algorithm: 0
        SR Prefix-SID: 1349 Flags: [N] Algorithm: 128
        SR Prefix-SID: 1350 Flags: [N] Algorithm: 129
        SR Prefix-SID: 1351 Flags: [N] Algorithm: 130
      Reachability         : 20.175.221.0/24 Metric: 10 Type: 1 Up
      Reachability         : 20.30.221.0/24 Metric: 100 Type: 1 Up
      Reachability          : 1221::1/128 Metric: 0 Type: 1 Up
      Reachability          : 2001:0:175:221::/64 Metric: 10 Type: 1 Up
      Reachability          : 2001:0:30:221::/64 Metric: 100 Type: 1 Up

```

## show isis flex-algo

```text

IS-IS Instance: IGP VRF: default

Algorithm   Advertised Level Metric    Selected               
----------- ---------- ----- --------- -----------------------
MIN-LATENCY yes        L2    min-delay Arista-Spine3-Q2A-30   
MIN-TE      yes        L2    TE        Arista-Spine3-Q2A-30   
ADMIN       yes        L2    default   Juniper-175-ACX7100-48L

```

## show isis flex-algo path detail

```text
Flex algo paths for IPv4 address family
Topology ID: Level-2
Destination: 0000.0000.0124
Path ID: 640
Path constraints: algo MIN-LATENCY
                  metric type MIN-DELAY
Request sequence number: 0
Response sequence number: 0
Number of times path updated: 7
Last updated: 0:39:42 ago
Metric: 20000
Next Hop    Interface
----------- ---------
20.30.32.30 Ethernet1

Destination: 0000.0000.0124
Path ID: 641
Path constraints: algo MIN-TE
                  metric type TE
Request sequence number: 0
Response sequence number: 0
Number of times path updated: 7
Last updated: 0:16:25 ago
Metric: 20
Next Hop      Interface
------------- ---------
20.32.175.175 Ethernet5

Destination: 0000.0000.0124
Path ID: 642
Path constraints: algo ADMIN
                  metric type IGP
                  administrative-group exclude 2
Request sequence number: 0
Response sequence number: 0
Number of times path updated: 6
Last updated: 0:00:01 ago
Metric: 25
Next Hop      Interface
------------- ---------
20.32.175.175 Ethernet5

Destination: 0000.0000.0128
Path ID: 640
Path constraints: algo MIN-LATENCY
                  metric type MIN-DELAY
Request sequence number: 0
Response sequence number: 0
Number of times path updated: 8
Last updated: 0:39:42 ago
Metric: 20000
Next Hop    Interface
----------- ---------
20.30.32.30 Ethernet1

Destination: 0000.0000.0128
Path ID: 641
Path constraints: algo MIN-TE
                  metric type TE
Request sequence number: 0
Response sequence number: 0
Number of times path updated: 9
Last updated: 0:16:25 ago
Metric: 20
Next Hop      Interface
------------- ---------
20.32.175.175 Ethernet5

Destination: 0000.0000.0128
Path ID: 642
Path constraints: algo ADMIN
                  metric type IGP
                  administrative-group exclude 2
Request sequence number: 0
Response sequence number: 0
Number of times path updated: 6
Last updated: 0:00:01 ago
Metric: 25
Next Hop      Interface
------------- ---------
20.32.175.175 Ethernet5

Destination: 0000.0000.0184
Path ID: 640
Path constraints: algo MIN-LATENCY
                  metric type MIN-DELAY
Request sequence number: 0
Response sequence number: 0
Number of times path updated: 2226
Last updated: 0:00:00 ago
Metric: 20000
Next Hop    Interface
----------- ---------
20.30.32.30 Ethernet1

Destination: 0000.0000.0184
Path ID: 641
Path constraints: algo MIN-TE
                  metric type TE
Request sequence number: 0
Response sequence number: 0
Number of times path updated: 2225
Last updated: 0:00:00 ago
Metric: 200
Next Hop    Interface
----------- ---------
20.30.32.30 Ethernet1

Destination: 0000.0000.0184
Path ID: 642
Path constraints: algo ADMIN
                  metric type IGP
                  administrative-group exclude 2
Request sequence number: 0
Response sequence number: 0
Number of times path updated: 2225
Last updated: 0:00:00 ago
Next Hop Interface
-------- ---------

Destination: 221
Path ID: 640
Path constraints: algo MIN-LATENCY
                  metric type MIN-DELAY
Request sequence number: 0
Response sequence number: 0
Number of times path updated: 7
Last updated: 0:39:42 ago
Metric: 20000
Next Hop    Interface
----------- ---------
20.30.32.30 Ethernet1

Destination: 221
Path ID: 641
Path constraints: algo MIN-TE
                  metric type TE
Request sequence number: 0
Response sequence number: 0
Number of times path updated: 8
Last updated: 0:16:25 ago
Metric: 20
Next Hop      Interface
------------- ---------
20.32.175.175 Ethernet5

Destination: 221
Path ID: 642
Path constraints: algo ADMIN
                  metric type IGP
                  administrative-group exclude 2
Request sequence number: 0
Response sequence number: 0
Number of times path updated: 6
Last updated: 0:00:01 ago
Metric: 25
Next Hop      Interface
------------- ---------
20.32.175.175 Ethernet5

Destination: Arista-PE32-Q2C-32
Path ID: 640
Path constraints: algo MIN-LATENCY
                  metric type MIN-DELAY
Request sequence number: 0
Response sequence number: 0
Number of times path updated: 1
Last updated: 3:58:04 ago
Next Hop Interface
-------- ---------

Destination: Arista-PE32-Q2C-32
Path ID: 641
Path constraints: algo MIN-TE
                  metric type TE
Request sequence number: 0
Response sequence number: 0
Number of times path updated: 1
Last updated: 3:58:04 ago
Next Hop Interface
-------- ---------

Destination: Arista-PE32-Q2C-32
Path ID: 642
Path constraints: algo ADMIN
                  metric type IGP
                  administrative-group exclude 2
Request sequence number: 0
Response sequence number: 0
Number of times path updated: 1
Last updated: 3:58:04 ago
Next Hop Interface
-------- ---------

Destination: Arista-Spine3-Q2A-30
Path ID: 640
Path constraints: algo MIN-LATENCY
                  metric type MIN-DELAY
Request sequence number: 0
Response sequence number: 0
Number of times path updated: 2
Last updated: 3:57:27 ago
Metric: 10000
Next Hop    Interface
----------- ---------
20.30.32.30 Ethernet1

Destination: Arista-Spine3-Q2A-30
Path ID: 641
Path constraints: algo MIN-TE
                  metric type TE
Request sequence number: 0
Response sequence number: 0
Number of times path updated: 4
Last updated: 2:02:16 ago
Metric: 100
Next Hop    Interface
----------- ---------
20.30.32.30 Ethernet1

Destination: Arista-Spine3-Q2A-30
Path ID: 642
Path constraints: algo ADMIN
                  metric type IGP
                  administrative-group exclude 2
Request sequence number: 0
Response sequence number: 0
Number of times path updated: 4
Last updated: 2:34:07 ago
Metric: 10
Next Hop    Interface
----------- ---------
20.30.32.30 Ethernet1

Destination: Arrcus-53
Path ID: 640
Path constraints: algo MIN-LATENCY
                  metric type MIN-DELAY
Request sequence number: 0
Response sequence number: 0
Number of times path updated: 8
Last updated: 0:39:42 ago
Metric: 20000
Next Hop    Interface
----------- ---------
20.30.32.30 Ethernet1

Destination: Arrcus-53
Path ID: 641
Path constraints: algo MIN-TE
                  metric type TE
Request sequence number: 0
Response sequence number: 0
Number of times path updated: 9
Last updated: 0:16:25 ago
Metric: 20
Next Hop      Interface
------------- ---------
20.32.175.175 Ethernet5

Destination: Arrcus-53
Path ID: 642
Path constraints: algo ADMIN
                  metric type IGP
                  administrative-group exclude 2
Request sequence number: 0
Response sequence number: 0
Number of times path updated: 7
Last updated: 0:00:01 ago
Metric: 25
Next Hop      Interface
------------- ---------
20.32.175.175 Ethernet5

Destination: H3C_M1A_120
Path ID: 640
Path constraints: algo MIN-LATENCY
                  metric type MIN-DELAY
Request sequence number: 0
Response sequence number: 0
Number of times path updated: 7
Last updated: 0:39:42 ago
Metric: 20000
Next Hop    Interface
----------- ---------
20.30.32.30 Ethernet1

Destination: H3C_M1A_120
Path ID: 641
Path constraints: algo MIN-TE
                  metric type TE
Request sequence number: 0
Response sequence number: 0
Number of times path updated: 7
Last updated: 0:16:25 ago
Metric: 20
Next Hop      Interface
------------- ---------
20.32.175.175 Ethernet5

Destination: H3C_M1A_120
Path ID: 642
Path constraints: algo ADMIN
                  metric type IGP
                  administrative-group exclude 2
Request sequence number: 0
Response sequence number: 0
Number of times path updated: 4
Last updated: 0:00:01 ago
Metric: 25
Next Hop      Interface
------------- ---------
20.32.175.175 Ethernet5

Destination: Juniper-156-PTX10002-36QDD
Path ID: 640
Path constraints: algo MIN-LATENCY
                  metric type MIN-DELAY
Request sequence number: 0
Response sequence number: 0
Number of times path updated: 7
Last updated: 0:39:42 ago
Metric: 20000
Next Hop    Interface
----------- ---------
20.30.32.30 Ethernet1

Destination: Juniper-156-PTX10002-36QDD
Path ID: 641
Path constraints: algo MIN-TE
                  metric type TE
Request sequence number: 0
Response sequence number: 0
Number of times path updated: 7
Last updated: 0:16:25 ago
Metric: 20
Next Hop      Interface
------------- ---------
20.32.175.175 Ethernet5

Destination: Juniper-156-PTX10002-36QDD
Path ID: 642
Path constraints: algo ADMIN
                  metric type IGP
                  administrative-group exclude 2
Request sequence number: 0
Response sequence number: 0
Number of times path updated: 6
Last updated: 0:00:01 ago
Metric: 20
Next Hop      Interface
------------- ---------
20.32.175.175 Ethernet5

Destination: Juniper-175-ACX7100-48L
Path ID: 640
Path constraints: algo MIN-LATENCY
                  metric type MIN-DELAY
Request sequence number: 0
Response sequence number: 0
Number of times path updated: 7
Last updated: 0:39:42 ago
Metric: 20010
Next Hop    Interface
----------- ---------
20.30.32.30 Ethernet1

Destination: Juniper-175-ACX7100-48L
Path ID: 641
Path constraints: algo MIN-TE
                  metric type TE
Request sequence number: 0
Response sequence number: 0
Number of times path updated: 1
Last updated: 2:58:39 ago
Metric: 10
Next Hop      Interface
------------- ---------
20.32.175.175 Ethernet5

Destination: Juniper-175-ACX7100-48L
Path ID: 642
Path constraints: algo ADMIN
                  metric type IGP
                  administrative-group exclude 2
Request sequence number: 0
Response sequence number: 0
Number of times path updated: 3
Last updated: 2:34:07 ago
Metric: 10
Next Hop      Interface
------------- ---------
20.32.175.175 Ethernet5

Destination: Juniper-179-ACX7024
Path ID: 640
Path constraints: algo MIN-LATENCY
                  metric type MIN-DELAY
Request sequence number: 0
Response sequence number: 0
Number of times path updated: 6
Last updated: 0:39:42 ago
Metric: 20000
Next Hop    Interface
----------- ---------
20.30.32.30 Ethernet1

Destination: Juniper-179-ACX7024
Path ID: 641
Path constraints: algo MIN-TE
                  metric type TE
Request sequence number: 0
Response sequence number: 0
Number of times path updated: 7
Last updated: 0:16:25 ago
Metric: 20
Next Hop      Interface
------------- ---------
20.32.175.175 Ethernet5

Destination: Juniper-179-ACX7024
Path ID: 642
Path constraints: algo ADMIN
                  metric type IGP
                  administrative-group exclude 2
Request sequence number: 0
Response sequence number: 0
Number of times path updated: 4
Last updated: 0:00:01 ago
Metric: 25
Next Hop      Interface
------------- ---------
20.32.175.175 Ethernet5

Destination: Nokia-SR1-217
Path ID: 640
Path constraints: algo MIN-LATENCY
                  metric type MIN-DELAY
Request sequence number: 0
Response sequence number: 0
Number of times path updated: 8
Last updated: 0:39:42 ago
Metric: 20000
Next Hop    Interface
----------- ---------
20.30.32.30 Ethernet1

Destination: Nokia-SR1-217
Path ID: 641
Path constraints: algo MIN-TE
                  metric type TE
Request sequence number: 0
Response sequence number: 0
Number of times path updated: 9
Last updated: 0:16:25 ago
Metric: 20
Next Hop      Interface
------------- ---------
20.32.175.175 Ethernet5

Destination: Nokia-SR1-217
Path ID: 642
Path constraints: algo ADMIN
                  metric type IGP
                  administrative-group exclude 2
Request sequence number: 0
Response sequence number: 0
Number of times path updated: 7
Last updated: 0:00:01 ago
Metric: 25
Next Hop      Interface
------------- ---------
20.32.175.175 Ethernet5

```

## show isis segment-routing tunnel

```text
  Index     Endpoint          Next Hop/Tunnel Index      Interface    Labels   
--------- ----------------- -------------------------- -------------- ---------
  1         10.0.0.175/32     TI-LFA (3)                 -            [ 3 ]    
  2         10.0.0.84/32      TI-LFA (0)                 -            [ 20084 ]
  5         10.0.0.30/32      TI-LFA (1)                 -            [ 3 ]    
  6         10.0.0.53/32      TI-LFA (0)                 -            [ 20053 ]
  7         10.0.0.179/32     TI-LFA (0)                 -            [ 20179 ]
  8         10.0.0.120/32     TI-LFA (0)                 -            [ 20120 ]
  10        10.0.0.214/32     TI-LFA (0)                 -            [ 20214 ]
  11        10.0.0.128/32     TI-LFA (0)                 -            [ 20128 ]
  12        10.0.0.131/32     TI-LFA (0)                 -            [ 20131 ]
  13        10.0.0.221/32     TI-LFA (0)                 -            [ 20221 ]
  14        10.0.0.124/32     TI-LFA (0)                 -            [ 20124 ]
  15        10.0.0.184/32     20.30.32.30                Ethernet1    [ 20184 ]
  16        10.0.0.217/32     TI-LFA (0)                 -            [ 20217 ]
  18        10.0.0.156/32     20.30.32.30                Ethernet1    [ 20156 ]
                              20.32.175.175              Ethernet5    [ 20156 ]

```

## show isis segment-routing prefix-segments

```text

System ID: Arista-PE32-Q2C-32			Instance: 'IGP'
SR supported Data-plane: MPLS			SR Router ID: 10.0.0.32

Node: 51     Proxy-Node: 0      Prefix: 0       Total Segments: 51

Flag Descriptions: R: Re-advertised, N: Node Segment, P: no-PHP
                   E: Explicit-NULL, V: Value, L: Local
Segment status codes: * - Self originated Prefix, L1 - level 1, L2 - level 2, ! - SR-unreachable,
                      # - Some IS-IS next-hops are SR-unreachable
   Prefix                      SID   Label Type       Flags                        System ID       Level Protection  Algorithm   
   ------------------------- ----- ------- ---------- ---------------------------- --------------- ----- ----------- -------------
   10.0.0.30/32                 30   20030 Node       R:0 N:1 P:0 E:0 V:0 L:0      Arista-Spine3-Q2A-30 L2    node        SPF         
   10.0.0.30/32               1158   21158 Node       R:0 N:1 P:0 E:0 V:0 L:0      Arista-Spine3-Q2A-30 L2    node        MIN-LATENCY 
   10.0.0.30/32               1159   21159 Node       R:0 N:1 P:0 E:0 V:0 L:0      Arista-Spine3-Q2A-30 L2    node        MIN-TE      
   10.0.0.30/32               1160   21160 Node       R:0 N:1 P:0 E:0 V:0 L:0      Arista-Spine3-Q2A-30 L2    node        ADMIN       
*  10.0.0.32/32                 32   20032 Node       R:0 N:1 P:0 E:0 V:0 L:0      Arista-PE32-Q2C-32 L2    unprotected SPF         
*  10.0.0.32/32               1161   21161 Node       R:0 N:1 P:0 E:0 V:0 L:0      Arista-PE32-Q2C-32 L2    unprotected MIN-LATENCY 
*  10.0.0.32/32               1162   21162 Node       R:0 N:1 P:0 E:0 V:0 L:0      Arista-PE32-Q2C-32 L2    unprotected MIN-TE      
*  10.0.0.32/32               1163   21163 Node       R:0 N:1 P:0 E:0 V:0 L:0      Arista-PE32-Q2C-32 L2    unprotected ADMIN       
   10.0.0.53/32                 53   20053 Node       R:0 N:1 P:1 E:1 V:0 L:0      Arrcus-53       L2    node        SPF         
   10.0.0.53/32               1181   21181 Node       R:0 N:1 P:0 E:0 V:0 L:0      Arrcus-53       L2    node        MIN-LATENCY 
   10.0.0.53/32               1182   21182 Node       R:0 N:1 P:0 E:0 V:0 L:0      Arrcus-53       L2    node        MIN-TE      
   10.0.0.53/32               1183   21183 Node       R:0 N:1 P:0 E:0 V:0 L:0      Arrcus-53       L2    node        ADMIN       
   10.0.0.84/32                 84   20084 Node       R:0 N:1 P:1 E:0 V:0 L:0      Ericsson_84_R6678 L2    node        SPF         
   10.0.0.120/32               120   20120 Node       R:0 N:1 P:0 E:0 V:0 L:0      H3C_M1A_120     L2    node        SPF         
   10.0.0.120/32              1248   21248 Node       R:0 N:1 P:1 E:0 V:0 L:0      H3C_M1A_120     L2    node        MIN-LATENCY 
   10.0.0.120/32              1249   21249 Node       R:0 N:1 P:1 E:0 V:0 L:0      H3C_M1A_120     L2    node        MIN-TE      
   10.0.0.120/32              1250   21250 Node       R:0 N:1 P:1 E:0 V:0 L:0      H3C_M1A_120     L2    node        ADMIN       
   10.0.0.124/32               124    2124 Node       R:0 N:1 P:1 E:0 V:0 L:0      0000.0000.0124  L2    node        SPF         
   10.0.0.124/32              1252    3252 Node       R:0 N:1 P:1 E:0 V:0 L:0      0000.0000.0124  L2    node        MIN-LATENCY 
   10.0.0.124/32              1253    3253 Node       R:0 N:1 P:1 E:0 V:0 L:0      0000.0000.0124  L2    node        MIN-TE      
   10.0.0.124/32              1254    3254 Node       R:0 N:1 P:1 E:0 V:0 L:0      0000.0000.0124  L2    node        ADMIN       
   10.0.0.128/32               128   20128 Node       R:0 N:1 P:0 E:0 V:0 L:0      0000.0000.0128  L2    node        SPF         
   10.0.0.128/32              1256   21256 Node       R:0 N:1 P:0 E:0 V:0 L:0      0000.0000.0128  L2    node        MIN-LATENCY 
   10.0.0.128/32              1257   21257 Node       R:0 N:1 P:0 E:0 V:0 L:0      0000.0000.0128  L2    node        MIN-TE      
   10.0.0.128/32              1258   21258 Node       R:0 N:1 P:0 E:0 V:0 L:0      0000.0000.0128  L2    node        ADMIN       
   10.0.0.131/32               131   20131 Node       R:0 N:1 P:0 E:0 V:0 L:0      Juniper-131-JCNR L2    node        SPF         
   10.0.0.156/32               156   20156 Node       R:0 N:1 P:0 E:0 V:0 L:0      Juniper-156-PTX10002-36QDD L2    unprotected SPF         
   10.0.0.156/32              1284   21284 Node       R:0 N:1 P:0 E:0 V:0 L:0      Juniper-156-PTX10002-36QDD L2    node        MIN-LATENCY 
   10.0.0.156/32              1285   21285 Node       R:0 N:1 P:0 E:0 V:0 L:0      Juniper-156-PTX10002-36QDD L2    node        MIN-TE      
   10.0.0.156/32              1286   21286 Node       R:0 N:1 P:0 E:0 V:0 L:0      Juniper-156-PTX10002-36QDD L2    node        ADMIN       
   10.0.0.175/32               175   20175 Node       R:0 N:1 P:0 E:0 V:0 L:0      Juniper-175-ACX7100-48L L2    node        SPF         
   10.0.0.175/32              1303   21303 Node       R:0 N:1 P:0 E:0 V:0 L:0      Juniper-175-ACX7100-48L L2    node        MIN-LATENCY 
   10.0.0.175/32              1304   21304 Node       R:0 N:1 P:0 E:0 V:0 L:0      Juniper-175-ACX7100-48L L2    node        MIN-TE      
   10.0.0.175/32              1305   21305 Node       R:0 N:1 P:0 E:0 V:0 L:0      Juniper-175-ACX7100-48L L2    node        ADMIN       
   10.0.0.179/32               179   20179 Node       R:0 N:1 P:0 E:0 V:0 L:0      Juniper-179-ACX7024 L2    node        SPF         
   10.0.0.179/32              1307   21307 Node       R:0 N:1 P:0 E:0 V:0 L:0      Juniper-179-ACX7024 L2    node        MIN-LATENCY 
   10.0.0.179/32              1308   21308 Node       R:0 N:1 P:0 E:0 V:0 L:0      Juniper-179-ACX7024 L2    node        MIN-TE      
   10.0.0.179/32              1309   21309 Node       R:0 N:1 P:0 E:0 V:0 L:0      Juniper-179-ACX7024 L2    node        ADMIN       
   10.0.0.184/32               184   20184 Node       R:0 N:1 P:0 E:0 V:0 L:0      0000.0000.0184  L2    unprotected SPF         
   10.0.0.184/32              1312   21312 Node       R:0 N:1 P:0 E:0 V:0 L:0      0000.0000.0184  L2    node        MIN-LATENCY 
   10.0.0.184/32              1313   21313 Node       R:0 N:1 P:0 E:0 V:0 L:0      0000.0000.0184  L2    node        MIN-TE      
   10.0.0.184/32              1314   21314 Node       R:0 N:1 P:0 E:0 V:0 L:0      0000.0000.0184  L2    unprotected ADMIN       
   10.0.0.214/32               214   20214 Node       R:0 N:1 P:1 E:0 V:0 L:0      Nokia-SXR-214   L2    node        SPF         
   10.0.0.217/32               217   20217 Node       R:0 N:1 P:1 E:0 V:0 L:0      Nokia-SR1-217   L2    node        SPF         
   10.0.0.217/32              1345   21345 Node       R:0 N:1 P:1 E:0 V:0 L:0      Nokia-SR1-217   L2    node        MIN-LATENCY 
   10.0.0.217/32              1346   21346 Node       R:0 N:1 P:1 E:0 V:0 L:0      Nokia-SR1-217   L2    node        MIN-TE      
   10.0.0.217/32              1347   21347 Node       R:0 N:1 P:1 E:0 V:0 L:0      Nokia-SR1-217   L2    node        ADMIN       
   10.0.0.221/32               221  720221 Node       R:0 N:1 P:0 E:0 V:0 L:0      221             L2    node        SPF         
   10.0.0.221/32              1349  721349 Node       R:0 N:1 P:0 E:0 V:0 L:0      221             L2    node        MIN-LATENCY 
   10.0.0.221/32              1350  721350 Node       R:0 N:1 P:0 E:0 V:0 L:0      221             L2    node        MIN-TE      
   10.0.0.221/32              1351  721351 Node       R:0 N:1 P:0 E:0 V:0 L:0      221             L2    node        ADMIN       
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
 I L2     10.0.0.84/32 [115/30]
           via 20.30.32.30, Ethernet1
 I L2     10.0.0.120/32 [115/20]
           via 20.30.32.30, Ethernet1
 I L2     10.0.0.124/32 [115/20]
           via 20.30.32.30, Ethernet1
 I L2     10.0.0.128/32 [115/20]
           via 20.30.32.30, Ethernet1
 I L2     10.0.0.131/32 [115/20]
           via 20.30.32.30, Ethernet1
 I L2     10.0.0.156/32 [115/20]
           via 20.30.32.30, Ethernet1
           via 20.32.175.175, Ethernet5
 I L2     10.0.0.175/32 [115/10]
           via 20.32.175.175, Ethernet5
 I L2     10.0.0.179/32 [115/20]
           via 20.30.32.30, Ethernet1
 I L2     10.0.0.184/32 [115/20]
           via 20.30.32.30, Ethernet1
 I L2     10.0.0.214/32 [115/20]
           via 20.30.32.30, Ethernet1
 I L2     10.0.0.216/32 [115/30]
           via 20.30.32.30, Ethernet1
 I L2     10.0.0.217/32 [115/20]
           via 20.30.32.30, Ethernet1
 I L2     10.0.0.221/32 [115/20]
           via 20.30.32.30, Ethernet1
 C        20.30.32.0/24
           directly connected, Ethernet1
 I L2     20.30.53.0/24 [115/20]
           via 20.30.32.30, Ethernet1
 I L2     20.30.84.0/24 [115/20]
           via 20.30.32.30, Ethernet1
 I L2     20.30.120.0/24 [115/20]
           via 20.30.32.30, Ethernet1
 I L2     20.30.124.0/24 [115/20]
           via 20.30.32.30, Ethernet1
 I L2     20.30.128.0/24 [115/20]
           via 20.30.32.30, Ethernet1
 I L2     20.30.131.0/24 [115/20]
           via 20.30.32.30, Ethernet1
 I L2     20.30.156.0/24 [115/20]
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
 I L2     20.53.175.0/24 [115/25]
           via 20.32.175.175, Ethernet5
 I L2     20.84.175.0/24 [115/25]
           via 20.32.175.175, Ethernet5
 I L2     20.120.175.0/24 [115/25]
           via 20.32.175.175, Ethernet5
 I L2     20.120.214.0/24 [115/30]
           via 20.30.32.30, Ethernet1
 I L2     20.120.217.0/24 [115/20]
           via 20.30.32.30, Ethernet1
 I L2     20.124.175.0/24 [115/25]
           via 20.32.175.175, Ethernet5
 I L2     20.128.175.0/24 [115/25]
           via 20.32.175.175, Ethernet5
 I L2     20.131.175.0/24 [115/25]
           via 20.32.175.175, Ethernet5
 I L2     20.156.175.0/24 [115/20]
           via 20.32.175.175, Ethernet5
 I L2     20.175.179.0/24 [115/25]
           via 20.32.175.175, Ethernet5
 I L2     20.175.184.0/24 [115/25]
           via 20.32.175.175, Ethernet5
 I L2     20.175.214.0/24 [115/25]
           via 20.32.175.175, Ethernet5
 I L2     20.175.217.0/24 [115/25]
           via 20.32.175.175, Ethernet5
 I L2     20.175.221.0/24 [115/25]
           via 20.32.175.175, Ethernet5
 I L2     20.214.216.0/24 [115/30]
           via 20.30.32.30, Ethernet1
 I L2     192.168.20.0/23 [115/20]
           via 20.30.32.30, Ethernet1

```

## show ip route vrf FLEXALGO

```text

VRF: FLEXALGO
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

 C        50.128.32.0/24
           directly connected, Ethernet40.128
 B I      50.128.53.0/24 [200/0]
           via 10.0.0.53/32, algorithm MIN-LATENCY, IS-IS FlexAlgo tunnel index 6, label 970000
              via TI-LFA tunnel index 0, label 21181
                 via 20.30.32.30, Ethernet1, label imp-null(3)
                 backup via 20.32.175.175, Ethernet5, label imp-null(3)
 B I      50.128.120.0/24 [200/0]
           via 10.0.0.120/32, algorithm MIN-LATENCY, IS-IS FlexAlgo tunnel index 44, label 1272
              via TI-LFA tunnel index 0, label 21248
                 via 20.30.32.30, Ethernet1, label imp-null(3)
                 backup via 20.32.175.175, Ethernet5, label imp-null(3)
 B I      50.128.124.0/24 [200/0]
           via 10.0.0.124/32, algorithm MIN-LATENCY, IS-IS FlexAlgo tunnel index 23, label 454
              via TI-LFA tunnel index 0, label 21252
                 via 20.30.32.30, Ethernet1, label imp-null(3)
                 backup via 20.32.175.175, Ethernet5, label imp-null(3)
 B I      50.128.128.0/24 [200/0]
           via 10.0.0.128/32, algorithm MIN-LATENCY, IS-IS FlexAlgo tunnel index 8, label 48182
              via TI-LFA tunnel index 0, label 21256
                 via 20.30.32.30, Ethernet1, label imp-null(3)
                 backup via 20.32.175.175, Ethernet5, label imp-null(3)
 B I      50.128.156.0/24 [200/0]
           via 10.0.0.156/32, algorithm MIN-LATENCY, IS-IS FlexAlgo tunnel index 27, label 21
              via TI-LFA tunnel index 0, label 21284
                 via 20.30.32.30, Ethernet1, label imp-null(3)
                 backup via 20.32.175.175, Ethernet5, label imp-null(3)
 B I      50.128.179.0/24 [200/0]
           via 10.0.0.179/32, algorithm MIN-LATENCY, IS-IS FlexAlgo tunnel index 40, label 21
              via TI-LFA tunnel index 0, label 21307
                 via 20.30.32.30, Ethernet1, label imp-null(3)
                 backup via 20.32.175.175, Ethernet5, label imp-null(3)
 B I      50.128.184.0/24 [200/0]
           via 10.0.0.184/32, algorithm MIN-LATENCY, IS-IS FlexAlgo tunnel index 37, label 16
              via TI-LFA tunnel index 0, label 21312
                 via 20.30.32.30, Ethernet1, label imp-null(3)
                 backup via 20.32.175.175, Ethernet5, label imp-null(3)
 B I      50.128.217.0/24 [200/0]
           via 10.0.0.217/32, algorithm MIN-LATENCY, IS-IS FlexAlgo tunnel index 10, label 524284
              via TI-LFA tunnel index 0, label 21345
                 via 20.30.32.30, Ethernet1, label imp-null(3)
                 backup via 20.32.175.175, Ethernet5, label imp-null(3)
 B I      50.128.221.0/24 [200/0]
           via 10.0.0.221/32, algorithm MIN-LATENCY, IS-IS FlexAlgo tunnel index 5, label 524291
              via TI-LFA tunnel index 0, label 21349
                 via 20.30.32.30, Ethernet1, label imp-null(3)
                 backup via 20.32.175.175, Ethernet5, label imp-null(3)
 C        50.129.32.0/24
           directly connected, Ethernet40.129
 B I      50.129.53.0/24 [200/0]
           via 10.0.0.53/32, algorithm MIN-TE, IS-IS FlexAlgo tunnel index 12, label 970000
              via TI-LFA tunnel index 30, label 21182
                 via 20.32.175.175, Ethernet5, label imp-null(3)
                 backup via 20.30.32.30, Ethernet1, label imp-null(3)
 B I      50.129.120.0/24 [200/0]
           via 10.0.0.120/32, algorithm MIN-TE, IS-IS FlexAlgo tunnel index 45, label 1274
              via TI-LFA tunnel index 30, label 21249
                 via 20.32.175.175, Ethernet5, label imp-null(3)
                 backup via 20.30.32.30, Ethernet1, label imp-null(3)
 B I      50.129.124.0/24 [200/0]
           via 10.0.0.124/32, algorithm MIN-TE, IS-IS FlexAlgo tunnel index 24, label 457
              via TI-LFA tunnel index 30, label 21253
                 via 20.32.175.175, Ethernet5, label imp-null(3)
                 backup via 20.30.32.30, Ethernet1, label imp-null(3)
 B I      50.129.128.0/24 [200/0]
           via 10.0.0.128/32, algorithm MIN-TE, IS-IS FlexAlgo tunnel index 16, label 48185
              via TI-LFA tunnel index 30, label 21257
                 via 20.32.175.175, Ethernet5, label imp-null(3)
                 backup via 20.30.32.30, Ethernet1, label imp-null(3)
 B I      50.129.156.0/24 [200/0]
           via 10.0.0.156/32, algorithm MIN-TE, IS-IS FlexAlgo tunnel index 26, label 21
              via TI-LFA tunnel index 30, label 21285
                 via 20.32.175.175, Ethernet5, label imp-null(3)
                 backup via 20.30.32.30, Ethernet1, label imp-null(3)
 B I      50.129.179.0/24 [200/0]
           via 10.0.0.179/32, algorithm MIN-TE, IS-IS FlexAlgo tunnel index 38, label 21
              via TI-LFA tunnel index 30, label 21308
                 via 20.32.175.175, Ethernet5, label imp-null(3)
                 backup via 20.30.32.30, Ethernet1, label imp-null(3)
 B I      50.129.184.0/24 [200/0]
           via 10.0.0.184/32, algorithm MIN-TE, IS-IS FlexAlgo tunnel index 36, label 17
              via TI-LFA tunnel index 29, label 21313
                 via 20.30.32.30, Ethernet1, label imp-null(3)
                 backup via 20.32.175.175, Ethernet5, label 21308
 B I      50.129.217.0/24 [200/0]
           via 10.0.0.217/32, algorithm MIN-TE, IS-IS FlexAlgo tunnel index 14, label 524284
              via TI-LFA tunnel index 30, label 21346
                 via 20.32.175.175, Ethernet5, label imp-null(3)
                 backup via 20.30.32.30, Ethernet1, label imp-null(3)
 B I      50.129.221.0/24 [200/0]
           via 10.0.0.221/32, algorithm MIN-TE, IS-IS FlexAlgo tunnel index 15, label 524291
              via TI-LFA tunnel index 30, label 21350
                 via 20.32.175.175, Ethernet5, label imp-null(3)
                 backup via 20.30.32.30, Ethernet1, label imp-null(3)
 C        50.130.32.0/24
           directly connected, Ethernet40.130
 B I      50.130.53.0/24 [200/0]
           via 10.0.0.53/32, algorithm ADMIN, IS-IS FlexAlgo tunnel index 4, label 970000
              via 20.32.175.175, Ethernet5, label 21183
 B I      50.130.120.0/24 [200/0]
           via 10.0.0.120/32, algorithm ADMIN, IS-IS FlexAlgo tunnel index 46, label 1273
              via 20.32.175.175, Ethernet5, label 21250
 B I      50.130.124.0/24 [200/0]
           via 10.0.0.124/32, algorithm ADMIN, IS-IS FlexAlgo tunnel index 25, label 458
              via 20.32.175.175, Ethernet5, label 21254
 B I      50.130.128.0/24 [200/0]
           via 10.0.0.128/32, algorithm ADMIN, IS-IS FlexAlgo tunnel index 18, label 48186
              via 20.32.175.175, Ethernet5, label 21258
 B I      50.130.156.0/24 [200/0]
           via 10.0.0.156/32, algorithm ADMIN, IS-IS FlexAlgo tunnel index 28, label 21
              via 20.32.175.175, Ethernet5, label 21286
 B I      50.130.179.0/24 [200/0]
           via 10.0.0.179/32, algorithm ADMIN, IS-IS FlexAlgo tunnel index 39, label 21
              via 20.32.175.175, Ethernet5, label 21309
 B I      50.130.184.0/24 [200/0]
           via 10.0.0.184/32, IS-IS SR tunnel index 15, label 18
              via 20.30.32.30, Ethernet1, label 20184
 B I      50.130.217.0/24 [200/0]
           via 10.0.0.217/32, algorithm ADMIN, IS-IS FlexAlgo tunnel index 3, label 524284
              via 20.32.175.175, Ethernet5, label 21347
 B I      50.130.221.0/24 [200/0]
           via 10.0.0.221/32, algorithm ADMIN, IS-IS FlexAlgo tunnel index 17, label 524291
              via 20.32.175.175, Ethernet5, label 21351

```

## show mpls route

```text
MPLS forwarding table (Label [metric] Vias) - 52 routes 
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
                    backup via 20.32.175.175, Ethernet5, label 20214 20030
 20053   A[1]
                via M, ::, forward
                    EgressACL: apply
                  via TI-LFA tunnel index 0
                    via 20.30.32.30, Ethernet1, label imp-null(3)
                    backup via 20.32.175.175, Ethernet5, label imp-null(3)
 20084   A[1]
                via M, ::, forward
                    EgressACL: apply
                  via TI-LFA tunnel index 0
                    via 20.30.32.30, Ethernet1, label imp-null(3)
                    backup via 20.32.175.175, Ethernet5, label imp-null(3)
 20120   A[1]
                via M, ::, forward
                    EgressACL: apply
                  via TI-LFA tunnel index 0
                    via 20.30.32.30, Ethernet1, label imp-null(3)
                    backup via 20.32.175.175, Ethernet5, label imp-null(3)
 20124   A[1]
                via M, ::, forward
                    EgressACL: apply
                  via TI-LFA tunnel index 0
                    via 20.30.32.30, Ethernet1, label imp-null(3)
                    backup via 20.32.175.175, Ethernet5, label imp-null(3)
 20128   A[1]
                via M, ::, forward
                    EgressACL: apply
                  via TI-LFA tunnel index 0
                    via 20.30.32.30, Ethernet1, label imp-null(3)
                    backup via 20.32.175.175, Ethernet5, label imp-null(3)
 20131   A[1]
                via M, ::, forward
                    EgressACL: apply
                  via TI-LFA tunnel index 0
                    via 20.30.32.30, Ethernet1, label imp-null(3)
                    backup via 20.32.175.175, Ethernet5, label imp-null(3)
 20156   A[1]
                via M, forward
                    EgressACL: apply
                    20.30.32.30 Ethernet1
                    20.32.175.175 Ethernet5
 20175   A[1]
                via M, ::, pop
                    EgressACL: apply
                  via TI-LFA tunnel index 3
                    via 20.32.175.175, Ethernet5, label imp-null(3)
                    backup via 20.30.32.30, Ethernet1, label 20217 20175
 20179   A[1]
                via M, ::, forward
                    EgressACL: apply
                  via TI-LFA tunnel index 0
                    via 20.30.32.30, Ethernet1, label imp-null(3)
                    backup via 20.32.175.175, Ethernet5, label imp-null(3)
 20184   A[1]
                via M, forward
                    EgressACL: apply
                    20.30.32.30 Ethernet1
 20214   A[1]
                via M, ::, forward
                    EgressACL: apply
                  via TI-LFA tunnel index 0
                    via 20.30.32.30, Ethernet1, label imp-null(3)
                    backup via 20.32.175.175, Ethernet5, label imp-null(3)
 20217   A[1]
                via M, ::, forward
                    EgressACL: apply
                  via TI-LFA tunnel index 0
                    via 20.30.32.30, Ethernet1, label imp-null(3)
                    backup via 20.32.175.175, Ethernet5, label imp-null(3)
 20221   A[1]
                via M, ::, forward
                    EgressACL: apply
                  via TI-LFA tunnel index 0
                    via 20.30.32.30, Ethernet1, label imp-null(3)
                    backup via 20.32.175.175, Ethernet5, label imp-null(3)
 21158   A[1]
                via M, ::, pop
                    EgressACL: apply
                  via TI-LFA tunnel index 4
                    via 20.30.32.30, Ethernet1, label imp-null(3)
                    backup via 20.32.175.175, Ethernet5, label 21158
 21159   A[1]
                via M, ::, pop
                    EgressACL: apply
                  via TI-LFA tunnel index 25
                    via 20.30.32.30, Ethernet1, label imp-null(3)
                    backup via 20.32.175.175, Ethernet5, label 21346 21159
 21160   A[1]
                via M, pop
                    EgressACL: apply
                    20.30.32.30 Ethernet1
 21181   A[1]
                via M, ::, forward
                    EgressACL: apply
                  via TI-LFA tunnel index 0
                    via 20.30.32.30, Ethernet1, label imp-null(3)
                    backup via 20.32.175.175, Ethernet5, label imp-null(3)
 21182   A[1]
                via M, ::, forward
                    EgressACL: apply
                  via TI-LFA tunnel index 30
                    via 20.32.175.175, Ethernet5, label imp-null(3)
                    backup via 20.30.32.30, Ethernet1, label imp-null(3)
 21183   A[1]
                via M, forward
                    EgressACL: apply
                    20.32.175.175 Ethernet5
 21248   A[1]
                via M, ::, forward
                    EgressACL: apply
                  via TI-LFA tunnel index 0
                    via 20.30.32.30, Ethernet1, label imp-null(3)
                    backup via 20.32.175.175, Ethernet5, label imp-null(3)
 21249   A[1]
                via M, ::, forward
                    EgressACL: apply
                  via TI-LFA tunnel index 30
                    via 20.32.175.175, Ethernet5, label imp-null(3)
                    backup via 20.30.32.30, Ethernet1, label imp-null(3)
 21250   A[1]
                via M, forward
                    EgressACL: apply
                    20.32.175.175 Ethernet5
 21252   A[1]
                via M, ::, forward
                    EgressACL: apply
                  via TI-LFA tunnel index 0
                    via 20.30.32.30, Ethernet1, label imp-null(3)
                    backup via 20.32.175.175, Ethernet5, label imp-null(3)
 21253   A[1]
                via M, ::, forward
                    EgressACL: apply
                  via TI-LFA tunnel index 30
                    via 20.32.175.175, Ethernet5, label imp-null(3)
                    backup via 20.30.32.30, Ethernet1, label imp-null(3)
 21254   A[1]
                via M, forward
                    EgressACL: apply
                    20.32.175.175 Ethernet5
 21256   A[1]
                via M, ::, forward
                    EgressACL: apply
                  via TI-LFA tunnel index 0
                    via 20.30.32.30, Ethernet1, label imp-null(3)
                    backup via 20.32.175.175, Ethernet5, label imp-null(3)
 21257   A[1]
                via M, ::, forward
                    EgressACL: apply
                  via TI-LFA tunnel index 30
                    via 20.32.175.175, Ethernet5, label imp-null(3)
                    backup via 20.30.32.30, Ethernet1, label imp-null(3)
 21258   A[1]
                via M, forward
                    EgressACL: apply
                    20.32.175.175 Ethernet5
 21284   A[1]
                via M, ::, forward
                    EgressACL: apply
                  via TI-LFA tunnel index 0
                    via 20.30.32.30, Ethernet1, label imp-null(3)
                    backup via 20.32.175.175, Ethernet5, label imp-null(3)
 21285   A[1]
                via M, ::, forward
                    EgressACL: apply
                  via TI-LFA tunnel index 30
                    via 20.32.175.175, Ethernet5, label imp-null(3)
                    backup via 20.30.32.30, Ethernet1, label imp-null(3)
 21286   A[1]
                via M, forward
                    EgressACL: apply
                    20.32.175.175 Ethernet5
 21303   A[1]
                via M, ::, pop
                    EgressACL: apply
                  via TI-LFA tunnel index 8
                    via 20.30.32.30, Ethernet1, label 21303
                    backup via 20.32.175.175, Ethernet5, label imp-null(3)
 21304   A[1]
                via M, ::, pop
                    EgressACL: apply
                  via TI-LFA tunnel index 2
                    via 20.32.175.175, Ethernet5, label imp-null(3)
                    backup via 20.30.32.30, Ethernet1, label 21257 21304
 21305   A[1]
                via M, pop
                    EgressACL: apply
                    20.32.175.175 Ethernet5
 21307   A[1]
                via M, ::, forward
                    EgressACL: apply
                  via TI-LFA tunnel index 0
                    via 20.30.32.30, Ethernet1, label imp-null(3)
                    backup via 20.32.175.175, Ethernet5, label imp-null(3)
 21308   A[1]
                via M, ::, forward
                    EgressACL: apply
                  via TI-LFA tunnel index 30
                    via 20.32.175.175, Ethernet5, label imp-null(3)
                    backup via 20.30.32.30, Ethernet1, label imp-null(3)
 21309   A[1]
                via M, forward
                    EgressACL: apply
                    20.32.175.175 Ethernet5
 21312   A[1]
                via M, ::, forward
                    EgressACL: apply
                  via TI-LFA tunnel index 0
                    via 20.30.32.30, Ethernet1, label imp-null(3)
                    backup via 20.32.175.175, Ethernet5, label imp-null(3)
 21313   A[1]
                via M, ::, forward
                    EgressACL: apply
                  via TI-LFA tunnel index 29
                    via 20.30.32.30, Ethernet1, label imp-null(3)
                    backup via 20.32.175.175, Ethernet5, label 21308
 21345   A[1]
                via M, ::, forward
                    EgressACL: apply
                  via TI-LFA tunnel index 0
                    via 20.30.32.30, Ethernet1, label imp-null(3)
                    backup via 20.32.175.175, Ethernet5, label imp-null(3)
 21346   A[1]
                via M, ::, forward
                    EgressACL: apply
                  via TI-LFA tunnel index 30
                    via 20.32.175.175, Ethernet5, label imp-null(3)
                    backup via 20.30.32.30, Ethernet1, label imp-null(3)
 21347   A[1]
                via M, forward
                    EgressACL: apply
                    20.32.175.175 Ethernet5
 21349   A[1]
                via M, ::, forward
                    EgressACL: apply
                  via TI-LFA tunnel index 0
                    via 20.30.32.30, Ethernet1, label imp-null(3)
                    backup via 20.32.175.175, Ethernet5, label imp-null(3)
 21350   A[1]
                via M, ::, forward
                    EgressACL: apply
                  via TI-LFA tunnel index 30
                    via 20.32.175.175, Ethernet5, label imp-null(3)
                    backup via 20.30.32.30, Ethernet1, label imp-null(3)
 21351   A[1]
                via M, forward
                    EgressACL: apply
                    20.32.175.175 Ethernet5
 362165  A[1]
                via M, 20.30.32.30, pop
                    EgressACL: apply
                    directly connected, Ethernet1
                    c4:ca:2b:45:a2:15, vlan 1006
 362166  A[1]
                via M, fe80::c6ca:2bff:fe45:a215, pop
                    EgressACL: apply
                    directly connected, Ethernet1
                    c4:ca:2b:45:a2:15, vlan 1006
 362167  A[1]
                via M, 20.32.175.175, pop
                    EgressACL: apply
                    directly connected, Ethernet5
                    3c:08:cd:8d:ba:dc, vlan 1010
 378528   [0]
                via I, ipv4, vrf RED
 378529   [0]
                via I, ipv6, vrf RED
 378530   [0]
                via I, ipv4, vrf FLEXALGO
```

## show mpls lfib route

```text
MPLS forwarding table (Label [metric] Vias) - 52 routes 
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
                    backup via 20.32.175.175, Ethernet5, label 20214 20030
 IP    20053    [1], 10.0.0.53/32
                via TI-LFA tunnel index 0, forward
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                    via 20.30.32.30, Ethernet1, label imp-null(3)
                    backup via 20.32.175.175, Ethernet5, label imp-null(3)
 IP    20084    [1], 10.0.0.84/32
                via TI-LFA tunnel index 0, forward
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                    via 20.30.32.30, Ethernet1, label imp-null(3)
                    backup via 20.32.175.175, Ethernet5, label imp-null(3)
 IP    20120    [1], 10.0.0.120/32
                via TI-LFA tunnel index 0, forward
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                    via 20.30.32.30, Ethernet1, label imp-null(3)
                    backup via 20.32.175.175, Ethernet5, label imp-null(3)
 IP    20124    [1], 10.0.0.124/32
                via TI-LFA tunnel index 0, forward
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                    via 20.30.32.30, Ethernet1, label imp-null(3)
                    backup via 20.32.175.175, Ethernet5, label imp-null(3)
 IP    20128    [1], 10.0.0.128/32
                via TI-LFA tunnel index 0, forward
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                    via 20.30.32.30, Ethernet1, label imp-null(3)
                    backup via 20.32.175.175, Ethernet5, label imp-null(3)
 IP    20131    [1], 10.0.0.131/32
                via TI-LFA tunnel index 0, forward
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                    via 20.30.32.30, Ethernet1, label imp-null(3)
                    backup via 20.32.175.175, Ethernet5, label imp-null(3)
 IP    20156    [1], 10.0.0.156/32
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
                    backup via 20.30.32.30, Ethernet1, label 20217 20175
 IP    20179    [1], 10.0.0.179/32
                via TI-LFA tunnel index 0, forward
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                    via 20.30.32.30, Ethernet1, label imp-null(3)
                    backup via 20.32.175.175, Ethernet5, label imp-null(3)
 IP    20184    [1], 10.0.0.184/32
                via M, 20.30.32.30, forward
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                 interface Ethernet1
 IP    20214    [1], 10.0.0.214/32
                via TI-LFA tunnel index 0, forward
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                    via 20.30.32.30, Ethernet1, label imp-null(3)
                    backup via 20.32.175.175, Ethernet5, label imp-null(3)
 IP    20217    [1], 10.0.0.217/32
                via TI-LFA tunnel index 0, forward
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                    via 20.30.32.30, Ethernet1, label imp-null(3)
                    backup via 20.32.175.175, Ethernet5, label imp-null(3)
 IP    20221    [1], 10.0.0.221/32
                via TI-LFA tunnel index 0, forward
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                    via 20.30.32.30, Ethernet1, label imp-null(3)
                    backup via 20.32.175.175, Ethernet5, label imp-null(3)
 IP    21158    [1], 10.0.0.30/32, algorithm MIN-LATENCY
                via TI-LFA tunnel index 4, pop
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                    via 20.30.32.30, Ethernet1, label imp-null(3)
                    backup via 20.32.175.175, Ethernet5, label 21158
 IP    21159    [1], 10.0.0.30/32, algorithm MIN-TE
                via TI-LFA tunnel index 25, pop
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                    via 20.30.32.30, Ethernet1, label imp-null(3)
                    backup via 20.32.175.175, Ethernet5, label 21346 21159
 IP    21160    [1], 10.0.0.30/32, algorithm ADMIN
                via M, 20.30.32.30, pop
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                 interface Ethernet1
 IP    21181    [1], 10.0.0.53/32, algorithm MIN-LATENCY
                via TI-LFA tunnel index 0, forward
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                    via 20.30.32.30, Ethernet1, label imp-null(3)
                    backup via 20.32.175.175, Ethernet5, label imp-null(3)
 IP    21182    [1], 10.0.0.53/32, algorithm MIN-TE
                via TI-LFA tunnel index 30, forward
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                    via 20.32.175.175, Ethernet5, label imp-null(3)
                    backup via 20.30.32.30, Ethernet1, label imp-null(3)
 IP    21183    [1], 10.0.0.53/32, algorithm ADMIN
                via M, 20.32.175.175, forward
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                 interface Ethernet5
 IP    21248    [1], 10.0.0.120/32, algorithm MIN-LATENCY
                via TI-LFA tunnel index 0, forward
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                    via 20.30.32.30, Ethernet1, label imp-null(3)
                    backup via 20.32.175.175, Ethernet5, label imp-null(3)
 IP    21249    [1], 10.0.0.120/32, algorithm MIN-TE
                via TI-LFA tunnel index 30, forward
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                    via 20.32.175.175, Ethernet5, label imp-null(3)
                    backup via 20.30.32.30, Ethernet1, label imp-null(3)
 IP    21250    [1], 10.0.0.120/32, algorithm ADMIN
                via M, 20.32.175.175, forward
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                 interface Ethernet5
 IP    21252    [1], 10.0.0.124/32, algorithm MIN-LATENCY
                via TI-LFA tunnel index 0, forward
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                    via 20.30.32.30, Ethernet1, label imp-null(3)
                    backup via 20.32.175.175, Ethernet5, label imp-null(3)
 IP    21253    [1], 10.0.0.124/32, algorithm MIN-TE
                via TI-LFA tunnel index 30, forward
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                    via 20.32.175.175, Ethernet5, label imp-null(3)
                    backup via 20.30.32.30, Ethernet1, label imp-null(3)
 IP    21254    [1], 10.0.0.124/32, algorithm ADMIN
                via M, 20.32.175.175, forward
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                 interface Ethernet5
 IP    21256    [1], 10.0.0.128/32, algorithm MIN-LATENCY
                via TI-LFA tunnel index 0, forward
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                    via 20.30.32.30, Ethernet1, label imp-null(3)
                    backup via 20.32.175.175, Ethernet5, label imp-null(3)
 IP    21257    [1], 10.0.0.128/32, algorithm MIN-TE
                via TI-LFA tunnel index 30, forward
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                    via 20.32.175.175, Ethernet5, label imp-null(3)
                    backup via 20.30.32.30, Ethernet1, label imp-null(3)
 IP    21258    [1], 10.0.0.128/32, algorithm ADMIN
                via M, 20.32.175.175, forward
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                 interface Ethernet5
 IP    21284    [1], 10.0.0.156/32, algorithm MIN-LATENCY
                via TI-LFA tunnel index 0, forward
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                    via 20.30.32.30, Ethernet1, label imp-null(3)
                    backup via 20.32.175.175, Ethernet5, label imp-null(3)
 IP    21285    [1], 10.0.0.156/32, algorithm MIN-TE
                via TI-LFA tunnel index 30, forward
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                    via 20.32.175.175, Ethernet5, label imp-null(3)
                    backup via 20.30.32.30, Ethernet1, label imp-null(3)
 IP    21286    [1], 10.0.0.156/32, algorithm ADMIN
                via M, 20.32.175.175, forward
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                 interface Ethernet5
 IP    21303    [1], 10.0.0.175/32, algorithm MIN-LATENCY
                via TI-LFA tunnel index 8, pop
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                    via 20.30.32.30, Ethernet1, label 21303
                    backup via 20.32.175.175, Ethernet5, label imp-null(3)
 IP    21304    [1], 10.0.0.175/32, algorithm MIN-TE
                via TI-LFA tunnel index 2, pop
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                    via 20.32.175.175, Ethernet5, label imp-null(3)
                    backup via 20.30.32.30, Ethernet1, label 21257 21304
 IP    21305    [1], 10.0.0.175/32, algorithm ADMIN
                via M, 20.32.175.175, pop
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                 interface Ethernet5
 IP    21307    [1], 10.0.0.179/32, algorithm MIN-LATENCY
                via TI-LFA tunnel index 0, forward
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                    via 20.30.32.30, Ethernet1, label imp-null(3)
                    backup via 20.32.175.175, Ethernet5, label imp-null(3)
 IP    21308    [1], 10.0.0.179/32, algorithm MIN-TE
                via TI-LFA tunnel index 30, forward
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                    via 20.32.175.175, Ethernet5, label imp-null(3)
                    backup via 20.30.32.30, Ethernet1, label imp-null(3)
 IP    21309    [1], 10.0.0.179/32, algorithm ADMIN
                via M, 20.32.175.175, forward
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                 interface Ethernet5
 IP    21312    [1], 10.0.0.184/32, algorithm MIN-LATENCY
                via TI-LFA tunnel index 0, forward
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                    via 20.30.32.30, Ethernet1, label imp-null(3)
                    backup via 20.32.175.175, Ethernet5, label imp-null(3)
 IP    21313    [1], 10.0.0.184/32, algorithm MIN-TE
                via TI-LFA tunnel index 29, forward
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                    via 20.30.32.30, Ethernet1, label imp-null(3)
                    backup via 20.32.175.175, Ethernet5, label 21308
 IP    21345    [1], 10.0.0.217/32, algorithm MIN-LATENCY
                via TI-LFA tunnel index 0, forward
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                    via 20.30.32.30, Ethernet1, label imp-null(3)
                    backup via 20.32.175.175, Ethernet5, label imp-null(3)
 IP    21346    [1], 10.0.0.217/32, algorithm MIN-TE
                via TI-LFA tunnel index 30, forward
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                    via 20.32.175.175, Ethernet5, label imp-null(3)
                    backup via 20.30.32.30, Ethernet1, label imp-null(3)
 IP    21347    [1], 10.0.0.217/32, algorithm ADMIN
                via M, 20.32.175.175, forward
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                 interface Ethernet5
 IP    21349    [1], 10.0.0.221/32, algorithm MIN-LATENCY
                via TI-LFA tunnel index 0, forward
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                    via 20.30.32.30, Ethernet1, label imp-null(3)
                    backup via 20.32.175.175, Ethernet5, label imp-null(3)
 IP    21350    [1], 10.0.0.221/32, algorithm MIN-TE
                via TI-LFA tunnel index 30, forward
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                    via 20.32.175.175, Ethernet5, label imp-null(3)
                    backup via 20.30.32.30, Ethernet1, label imp-null(3)
 IP    21351    [1], 10.0.0.221/32, algorithm ADMIN
                via M, 20.32.175.175, forward
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                 interface Ethernet5
 IA    362165   [1]
                via M, 20.30.32.30, pop
                 payload autoDecide, ttlMode uniform, apply egress-acl
                 interface Ethernet1
 IA    362166   [1]
                via M, fe80::c6ca:2bff:fe45:a215, pop
                 payload autoDecide, ttlMode uniform, apply egress-acl
                 interface Ethernet1
 IA    362167   [1]
                via M, 20.32.175.175, pop
                 payload autoDecide, ttlMode uniform, apply egress-acl
                 interface Ethernet5
 B3    378528   [0]
                via I, ipv4, vrf RED
 B3    378529   [0]
                via I, ipv6, vrf RED
 B3    378530   [0]
                via I, ipv4, vrf FLEXALGO
```

## show ip ospf segment-routing

```text
! OSPF (Instance Id: 1) Segment Routing has been administratively shutdown
```

## show ip ospf segment-routing global-blocks

```text
! OSPF (Instance Id: 1) Segment Routing has been administratively shutdown
```

## show ip ospf segment-routing bindings

```text
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
 * >Ec    RD: 84:5001 IPv4 prefix 50.10.84.0/24
                                 10.0.0.84             0       100     0       ? Or-ID: 10.0.0.84 C-LST: 10.0.0.30 
 *  ec    RD: 84:5001 IPv4 prefix 50.10.84.0/24
                                 10.0.0.84             0       100     0       ? Or-ID: 10.0.0.84 C-LST: 10.0.0.175 
 * >Ec    RD: 131:5001 IPv4 prefix 50.10.131.0/24
                                 10.0.0.131            -       100     0       i Or-ID: 10.0.0.131 C-LST: 10.0.0.30 
 *  ec    RD: 131:5001 IPv4 prefix 50.10.131.0/24
                                 10.0.0.131            -       100     0       i Or-ID: 10.0.0.131 C-LST: 10.0.0.175 
 * >Ec    RD: 156:5001 IPv4 prefix 50.10.156.0/24
                                 10.0.0.156            -       100     0       i Or-ID: 10.0.0.156 C-LST: 10.0.0.30 
 *  ec    RD: 156:5001 IPv4 prefix 50.10.156.0/24
                                 10.0.0.156            -       100     0       i Or-ID: 10.0.0.156 C-LST: 10.0.0.175 
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
 * >      RD: 10.0.0.30:5128 IPv4 prefix 50.128.32.0/24
                                 -                     -       -       0       i
 * >Ec    RD: 53:5001 IPv4 prefix 50.128.53.0/24
                                 10.0.0.53             -       100     0       ? Or-ID: 10.0.0.53 C-LST: 10.0.0.30 
 *  ec    RD: 53:5001 IPv4 prefix 50.128.53.0/24
                                 10.0.0.53             -       100     0       ? Or-ID: 10.0.0.53 C-LST: 10.0.0.175 
 * >Ec    RD: 120:5128 IPv4 prefix 50.128.120.0/24
                                 10.0.0.120            0       100     0       ? Or-ID: 10.0.0.120 C-LST: 10.0.0.30 
 *  ec    RD: 120:5128 IPv4 prefix 50.128.120.0/24
                                 10.0.0.120            0       100     0       ? Or-ID: 10.0.0.120 C-LST: 10.0.0.175 
 * >      RD: 124:5128 IPv4 prefix 50.128.124.0/24
                                 10.0.0.124            0       100     0       ? Or-ID: 10.0.0.124 C-LST: 10.0.0.175 
 * >      RD: 128:5128 IPv4 prefix 50.128.128.0/24
                                 10.0.0.128            0       100     0       ? Or-ID: 10.0.0.128 C-LST: 10.0.0.175 
 * >Ec    RD: 5128:5128 IPv4 prefix 50.128.156.0/24
                                 10.0.0.156            -       100     0       i Or-ID: 10.0.0.156 C-LST: 10.0.0.30 
 *  ec    RD: 5128:5128 IPv4 prefix 50.128.156.0/24
                                 10.0.0.156            -       100     0       i Or-ID: 10.0.0.156 C-LST: 10.0.0.175 
 * >Ec    RD: 5128:5128 IPv4 prefix 50.128.179.0/24
                                 10.0.0.179            -       100     0       i Or-ID: 10.0.0.179 C-LST: 10.0.0.30 
 *  ec    RD: 5128:5128 IPv4 prefix 50.128.179.0/24
                                 10.0.0.179            -       100     0       i Or-ID: 10.0.0.179 C-LST: 10.0.0.175 
 * >      RD: 184:5001 IPv4 prefix 50.128.184.0/24
                                 10.0.0.184            -       0       0       i Or-ID: 193.0.0.1 C-LST: 10.0.0.30 
 * >Ec    RD: 217:5128 IPv4 prefix 50.128.217.0/24
                                 10.0.0.217            -       100     0       i Or-ID: 10.0.0.217 C-LST: 10.0.0.30 
 *  ec    RD: 217:5128 IPv4 prefix 50.128.217.0/24
                                 10.0.0.217            -       100     0       i Or-ID: 10.0.0.217 C-LST: 10.0.0.175 
 * >Ec    RD: 221:5128 IPv4 prefix 50.128.221.0/24
                                 10.0.0.221            -       100     0       i Or-ID: 10.0.0.221 C-LST: 10.0.0.30 
 *  ec    RD: 221:5128 IPv4 prefix 50.128.221.0/24
                                 10.0.0.221            -       100     0       i Or-ID: 10.0.0.221 C-LST: 10.0.0.175 
 * >      RD: 10.0.0.30:5128 IPv4 prefix 50.129.32.0/24
                                 -                     -       -       0       i
 * >Ec    RD: 53:5001 IPv4 prefix 50.129.53.0/24
                                 10.0.0.53             -       100     0       ? Or-ID: 10.0.0.53 C-LST: 10.0.0.30 
 *  ec    RD: 53:5001 IPv4 prefix 50.129.53.0/24
                                 10.0.0.53             -       100     0       ? Or-ID: 10.0.0.53 C-LST: 10.0.0.175 
 * >Ec    RD: 120:5129 IPv4 prefix 50.129.120.0/24
                                 10.0.0.120            0       100     0       ? Or-ID: 10.0.0.120 C-LST: 10.0.0.30 
 *  ec    RD: 120:5129 IPv4 prefix 50.129.120.0/24
                                 10.0.0.120            0       100     0       ? Or-ID: 10.0.0.120 C-LST: 10.0.0.175 
 * >      RD: 124:5129 IPv4 prefix 50.129.124.0/24
                                 10.0.0.124            0       100     0       ? Or-ID: 10.0.0.124 C-LST: 10.0.0.175 
 * >      RD: 128:5129 IPv4 prefix 50.129.128.0/24
                                 10.0.0.128            0       100     0       ? Or-ID: 10.0.0.128 C-LST: 10.0.0.175 
 * >Ec    RD: 5128:5128 IPv4 prefix 50.129.156.0/24
                                 10.0.0.156            -       100     0       i Or-ID: 10.0.0.156 C-LST: 10.0.0.30 
 *  ec    RD: 5128:5128 IPv4 prefix 50.129.156.0/24
                                 10.0.0.156            -       100     0       i Or-ID: 10.0.0.156 C-LST: 10.0.0.175 
 * >Ec    RD: 5128:5128 IPv4 prefix 50.129.179.0/24
                                 10.0.0.179            -       100     0       i Or-ID: 10.0.0.179 C-LST: 10.0.0.30 
 *  ec    RD: 5128:5128 IPv4 prefix 50.129.179.0/24
                                 10.0.0.179            -       100     0       i Or-ID: 10.0.0.179 C-LST: 10.0.0.175 
 * >      RD: 184:5001 IPv4 prefix 50.129.184.0/24
                                 10.0.0.184            -       0       0       i Or-ID: 193.0.0.1 C-LST: 10.0.0.30 
 * >Ec    RD: 217:5128 IPv4 prefix 50.129.217.0/24
                                 10.0.0.217            -       100     0       i Or-ID: 10.0.0.217 C-LST: 10.0.0.30 
 *  ec    RD: 217:5128 IPv4 prefix 50.129.217.0/24
                                 10.0.0.217            -       100     0       i Or-ID: 10.0.0.217 C-LST: 10.0.0.175 
 * >Ec    RD: 221:5128 IPv4 prefix 50.129.221.0/24
                                 10.0.0.221            -       100     0       i Or-ID: 10.0.0.221 C-LST: 10.0.0.30 
 *  ec    RD: 221:5128 IPv4 prefix 50.129.221.0/24
                                 10.0.0.221            -       100     0       i Or-ID: 10.0.0.221 C-LST: 10.0.0.175 
 * >      RD: 10.0.0.30:5128 IPv4 prefix 50.130.32.0/24
                                 -                     -       -       0       i
 * >Ec    RD: 53:5001 IPv4 prefix 50.130.53.0/24
                                 10.0.0.53             -       100     0       ? Or-ID: 10.0.0.53 C-LST: 10.0.0.30 
 *  ec    RD: 53:5001 IPv4 prefix 50.130.53.0/24
                                 10.0.0.53             -       100     0       ? Or-ID: 10.0.0.53 C-LST: 10.0.0.175 
 * >Ec    RD: 120:5130 IPv4 prefix 50.130.120.0/24
                                 10.0.0.120            0       100     0       ? Or-ID: 10.0.0.120 C-LST: 10.0.0.30 
 *  ec    RD: 120:5130 IPv4 prefix 50.130.120.0/24
                                 10.0.0.120            0       100     0       ? Or-ID: 10.0.0.120 C-LST: 10.0.0.175 
 * >      RD: 124:5130 IPv4 prefix 50.130.124.0/24
                                 10.0.0.124            0       100     0       ? Or-ID: 10.0.0.124 C-LST: 10.0.0.175 
 * >      RD: 128:5130 IPv4 prefix 50.130.128.0/24
                                 10.0.0.128            0       100     0       ? Or-ID: 10.0.0.128 C-LST: 10.0.0.175 
 * >Ec    RD: 5128:5128 IPv4 prefix 50.130.156.0/24
                                 10.0.0.156            -       100     0       i Or-ID: 10.0.0.156 C-LST: 10.0.0.30 
 *  ec    RD: 5128:5128 IPv4 prefix 50.130.156.0/24
                                 10.0.0.156            -       100     0       i Or-ID: 10.0.0.156 C-LST: 10.0.0.175 
 * >Ec    RD: 5128:5128 IPv4 prefix 50.130.179.0/24
                                 10.0.0.179            -       100     0       i Or-ID: 10.0.0.179 C-LST: 10.0.0.30 
 *  ec    RD: 5128:5128 IPv4 prefix 50.130.179.0/24
                                 10.0.0.179            -       100     0       i Or-ID: 10.0.0.179 C-LST: 10.0.0.175 
 * >      RD: 184:5001 IPv4 prefix 50.130.184.0/24
                                 10.0.0.184            -       0       0       i Or-ID: 193.0.0.1 C-LST: 10.0.0.30 
 * >Ec    RD: 217:5128 IPv4 prefix 50.130.217.0/24
                                 10.0.0.217            -       100     0       i Or-ID: 10.0.0.217 C-LST: 10.0.0.30 
 *  ec    RD: 217:5128 IPv4 prefix 50.130.217.0/24
                                 10.0.0.217            -       100     0       i Or-ID: 10.0.0.217 C-LST: 10.0.0.175 
 * >Ec    RD: 221:5128 IPv4 prefix 50.130.221.0/24
                                 10.0.0.221            -       100     0       i Or-ID: 10.0.0.221 C-LST: 10.0.0.30 
 *  ec    RD: 221:5128 IPv4 prefix 50.130.221.0/24
                                 10.0.0.221            -       100     0       i Or-ID: 10.0.0.221 C-LST: 10.0.0.175 
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
 * >Ec    RD: 84:5001 IPv6 prefix 2600:50:10:84::/64
                                 ::ffff:10.0.0.84      0       100     0       ? Or-ID: 10.0.0.84 C-LST: 10.0.0.30 
 *  ec    RD: 84:5001 IPv6 prefix 2600:50:10:84::/64
                                 ::ffff:10.0.0.84      0       100     0       ? Or-ID: 10.0.0.84 C-LST: 10.0.0.175 
 * >      RD: 124:5001 IPv6 prefix 2600:50:10:124::/64
                                 ::ffff:10.0.0.124     0       100     0       ? Or-ID: 10.0.0.124 C-LST: 10.0.0.175 
 * >Ec    RD: 131:5001 IPv6 prefix 2600:50:10:131::/64
                                 ::ffff:10.0.0.131     -       100     0       i Or-ID: 10.0.0.131 C-LST: 10.0.0.30 
 *  ec    RD: 131:5001 IPv6 prefix 2600:50:10:131::/64
                                 ::ffff:10.0.0.131     -       100     0       i Or-ID: 10.0.0.131 C-LST: 10.0.0.175 
 * >Ec    RD: 156:5001 IPv6 prefix 2600:50:10:156::/64
                                 ::ffff:10.0.0.156     -       100     0       i Or-ID: 10.0.0.156 C-LST: 10.0.0.30 
 *  ec    RD: 156:5001 IPv6 prefix 2600:50:10:156::/64
                                 ::ffff:10.0.0.156     -       100     0       i Or-ID: 10.0.0.156 C-LST: 10.0.0.175 
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
  Last read 00:00:51, last write 00:00:26
  Hold time is 180, keepalive interval is 60 seconds
  Configured hold time is 180, keepalive interval is 60 seconds
  Effective minimum hold time is 3 seconds
  Send failure hold time is 0 seconds
  Hold timer is active, time left: 00:02:09
  Keepalive timer is active, time left: 00:00:18
  Connect timer is inactive
  Idle-restart timer is inactive
  BGP state is Established, up for 1d07h
  Number of transitions to established: 3
  Last state was OpenConfirm
  Last event was ReapplyOutboundPolicy
  Last sent notification:Hold Timer Expired Error/None, Last time 1d08h, First time 1d09h, Repeats 1
  Last sent socket-error:Connect (Network is unreachable), Last time 1d08h, First time 1d09h, Repeats 38
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
      Received 1d07h
      Number of stale paths removed after graceful restart: 0
      Number of paths received before End-of-RIB: 9
    VPN-IPv6 End-of-RIB received: Yes
      Received 1d07h
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
    Updates:                        56       925
    Keepalives:                   3576      3468
    Enhanced Route Refresh:          0         0
    Begin of Route Refresh:          0         0
    End of Route Refresh:            0         0
    Total messages:               3637      4396
  Prefix Statistics:
                                   Sent      Rcvd     Best Paths     Best ECMP Paths
    IPv4 Unicast:                     0         0              0                   0
    VPN-IPv4:                         4        27             27                  24
    IPv6 Unicast:                     0         0              0                   0
    VPN-IPv6:                         1         6              6                   6
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
  Total Number of TCP retransmissions: 2
  Options:
    Timestamps enabled: yes
    Selective Acknowledgments enabled: yes
    Window Scale enabled: yes
    Explicit Congestion Notification (ECN) enabled: no
  Socket Statistics:
    Window Scale (wscale): 7,7
    Retransmission Timeout (rto): 208.0ms
    Round-trip Time (rtt/rtvar): 4.4ms/1.7ms
    Delayed Ack Timeout (ato): 40.0ms
    Congestion Window (cwnd): 2
    Slow-start Threshold (ssthresh): 7
    TCP Throughput: 5.25 Mbps
    Recv Round-trip Time (rcv_rtt): 28546.1ms
    Advertised Recv Window (rcv_space): 65323

BGP neighbor is 10.0.0.175, remote AS 64512, internal link
 Description: Juniper_175
  BGP version 4, remote router ID 10.0.0.175, VRF default
  Inherits configuration from and member of peer-group IBGP_CLIENT_PEER
  Last read 00:00:15, last write 00:00:11
  Hold time is 90, keepalive interval is 30 seconds
  Configured hold time is 180, keepalive interval is 60 seconds
  Effective minimum hold time is 3 seconds
  Send failure hold time is 0 seconds
  Hold timer is active, time left: 00:01:15
  Keepalive timer is active, time left: 00:00:14
  Connect timer is inactive
  Idle-restart timer is inactive
  BGP state is Established, up for 07:47:37
  Number of transitions to established: 12
  Last state was OpenConfirm
  Last event was ReapplyOutboundPolicy
  Last sent notification:Hold Timer Expired Error/None, Last time 1d07h, First time 1d21h, Repeats 9
  Last sent socket-error:Connect (Network is unreachable), Last time 07:47:42, First time 07:47:54, Repeats 3
  Last rcvd socket-error:Connection reset by peer, Last time 07:47:59
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
      Received 07:47:36
      Number of stale paths removed after graceful restart: 0
      Number of paths received before End-of-RIB: 3
    VPN-IPv6 End-of-RIB received: Yes
      Received 07:47:36
      Number of stale paths removed after graceful restart: 0
      Number of paths received before End-of-RIB: 3
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
    Opens:                 12        12
    Notifications:         10         0
    Updates:               82      1298
    Keepalives:          7120      6301
    Route Refresh:          0         0
    Total messages:      7224      7611
  Prefix Statistics:
                                   Sent      Rcvd     Best Paths     Best ECMP Paths
    IPv4 Unicast:                     0         0              0                   0
    VPN-IPv4:                         4        30             30                   0
    IPv6 Unicast:                     0         0              0                   0
    VPN-IPv6:                         1         7              7                   0
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
  Outbound route map for VPN-IPv6 is SET_COLOR_101
Local AS is 64512, local router ID 10.0.0.32
TTL is 255
Local TCP address is 10.0.0.32, local port is 39895
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
    Retransmission Timeout (rto): 208.0ms
    Round-trip Time (rtt/rtvar): 5.8ms/5.2ms
    Delayed Ack Timeout (ato): 40.0ms
    Congestion Window (cwnd): 10
    TCP Throughput: 20.04 Mbps
    Recv Round-trip Time (rcv_rtt): 428986.5ms
    Advertised Recv Window (rcv_space): 64602

```

## show tunnel rib system-tunnel-rib brief

```text
Tunnel RIB: system-tunnel-rib
Endpoint        Tunnel Type     Index(es)   Tunnel Preference   IGP Preference 
-------------- --------------- ----------- ------------------- ----------------
10.0.0.30/32    IS-IS SR IPv4   5           65                  115            
10.0.0.53/32    IS-IS SR IPv4   6           65                  115            
10.0.0.84/32    IS-IS SR IPv4   2           65                  115            
10.0.0.120/32   IS-IS SR IPv4   8           65                  115            
10.0.0.124/32   IS-IS SR IPv4   14          65                  115            
10.0.0.128/32   IS-IS SR IPv4   11          65                  115            
10.0.0.131/32   IS-IS SR IPv4   12          65                  115            
10.0.0.156/32   IS-IS SR IPv4   18          65                  115            
10.0.0.175/32   IS-IS SR IPv4   1           65                  115            
10.0.0.179/32   IS-IS SR IPv4   7           65                  115            
10.0.0.184/32   IS-IS SR IPv4   15          65                  115            
10.0.0.214/32   IS-IS SR IPv4   10          65                  115            
10.0.0.217/32   IS-IS SR IPv4   16          65                  115            
10.0.0.221/32   IS-IS SR IPv4   13          65                  115            

   IGP Metric    Metric Type
---------------- -----------
   10            metric     
   20            metric     
   30            metric     
   20            metric     
   20            metric     
   20            metric     
   20            metric     
   20            metric     
   10            metric     
   20            metric     
   20            metric     
   20            metric     
   20            metric     
   20            metric     

```

## show tunnel rib colored brief

```text
Tunnel RIB: system-colored-tunnel-rib
 Endpoint        Color   Tunnel Type       Index(es)    Tunnel Preference    IGP Preference    IGP Metric   Metric Type
--------------- ------- ----------------- ------------ -------------------- ----------------- ------------- -----------
 10.0.0.30/32    128     IS-IS FlexAlgo    7            65                   115               10000        metric     
 10.0.0.30/32    129     IS-IS FlexAlgo    11           65                   115               100          metric     
 10.0.0.30/32    130     IS-IS FlexAlgo    2            65                   115               10           metric     
 10.0.0.53/32    128     IS-IS FlexAlgo    6            65                   115               20000        metric     
 10.0.0.53/32    129     IS-IS FlexAlgo    12           65                   115               20           metric     
 10.0.0.53/32    130     IS-IS FlexAlgo    4            65                   115               25           metric     
 10.0.0.120/32   128     IS-IS FlexAlgo    44           65                   115               20000        metric     
 10.0.0.120/32   129     IS-IS FlexAlgo    45           65                   115               20           metric     
 10.0.0.120/32   130     IS-IS FlexAlgo    46           65                   115               25           metric     
 10.0.0.124/32   128     IS-IS FlexAlgo    23           65                   115               20000        metric     
 10.0.0.124/32   129     IS-IS FlexAlgo    24           65                   115               20           metric     
 10.0.0.124/32   130     IS-IS FlexAlgo    25           65                   115               25           metric     
 10.0.0.128/32   128     IS-IS FlexAlgo    8            65                   115               20000        metric     
 10.0.0.128/32   129     IS-IS FlexAlgo    16           65                   115               20           metric     
 10.0.0.128/32   130     IS-IS FlexAlgo    18           65                   115               25           metric     
 10.0.0.156/32   128     IS-IS FlexAlgo    27           65                   115               20000        metric     
 10.0.0.156/32   129     IS-IS FlexAlgo    26           65                   115               20           metric     
 10.0.0.156/32   130     IS-IS FlexAlgo    28           65                   115               20           metric     
 10.0.0.175/32   128     IS-IS FlexAlgo    30           65                   115               20010        metric     
 10.0.0.175/32   129     IS-IS FlexAlgo    29           65                   115               10           metric     
 10.0.0.175/32   130     IS-IS FlexAlgo    31           65                   115               10           metric     
 10.0.0.179/32   128     IS-IS FlexAlgo    40           65                   115               20000        metric     
 10.0.0.179/32   129     IS-IS FlexAlgo    38           65                   115               20           metric     
 10.0.0.179/32   130     IS-IS FlexAlgo    39           65                   115               25           metric     
 10.0.0.184/32   128     IS-IS FlexAlgo    37           65                   115               20000        metric     
 10.0.0.184/32   129     IS-IS FlexAlgo    36           65                   115               200          metric     
 10.0.0.217/32   128     IS-IS FlexAlgo    10           65                   115               20000        metric     
 10.0.0.217/32   129     IS-IS FlexAlgo    14           65                   115               20           metric     
 10.0.0.217/32   130     IS-IS FlexAlgo    3            65                   115               25           metric     
 10.0.0.221/32   128     IS-IS FlexAlgo    5            65                   115               20000        metric     
 10.0.0.221/32   129     IS-IS FlexAlgo    15           65                   115               20           metric     
 10.0.0.221/32   130     IS-IS FlexAlgo    17           65                   115               25           metric     

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
>C    10.0.0.32/32 [0 pref/0 metric] updated 2d04h ago
         via Loopback0, directly connected
>C    20.30.32.0/24 [0 pref/0 metric] updated 1d08h ago
         via Ethernet1, directly connected
>C    20.32.175.0/24 [0 pref/0 metric] updated 1d09h ago
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
>P    0.0.0.0/8 [1 pref/0 metric] updated 2d10h ago
         via Null0, directly connected [NF]
>P    127.0.0.0/8 [1 pref/0 metric] updated 2d10h ago
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
>I    10.0.0.30/32 [115 pref/10 metric] updated 1d04h ago
         via 20.30.32.30, Ethernet1
>I    10.0.0.53/32 [115 pref/20 metric] updated 09:43:07 ago
         via 20.30.32.30, Ethernet1
>I    10.0.0.84/32 [115 pref/30 metric] updated 1d03h ago
         via 20.30.32.30, Ethernet1
>I    10.0.0.120/32 [115 pref/20 metric] updated 07:33:59 ago
         via 20.30.32.30, Ethernet1
>I    10.0.0.124/32 [115 pref/20 metric] updated 1d03h ago
         via 20.30.32.30, Ethernet1
>I    10.0.0.128/32 [115 pref/20 metric] updated 1d00h ago
         via 20.30.32.30, Ethernet1
>I    10.0.0.131/32 [115 pref/20 metric] updated 03:14:13 ago
         via 20.30.32.30, Ethernet1
>I    10.0.0.156/32 [115 pref/20 metric] updated 03:31:11 ago
         via 20.30.32.30, Ethernet1
         via 20.32.175.175, Ethernet5
>I    10.0.0.175/32 [115 pref/10 metric] updated 07:47:10 ago
         via 20.32.175.175, Ethernet5
>I    10.0.0.179/32 [115 pref/20 metric] updated 1d03h ago
         via 20.30.32.30, Ethernet1
>I    10.0.0.184/32 [115 pref/20 metric] updated 00:00:02 ago
         via 20.30.32.30, Ethernet1
>I    10.0.0.214/32 [115 pref/20 metric] updated 1d03h ago
         via 20.30.32.30, Ethernet1
>I    10.0.0.216/32 [115 pref/30 metric] updated 08:02:52 ago
         via 20.30.32.30, Ethernet1
>I    10.0.0.217/32 [115 pref/20 metric] updated 1d03h ago
         via 20.30.32.30, Ethernet1
>I    10.0.0.221/32 [115 pref/20 metric] updated 03:08:49 ago
         via 20.30.32.30, Ethernet1
>I    20.30.53.0/24 [115 pref/20 metric] updated 09:43:08 ago
         via 20.30.32.30, Ethernet1
>I    20.30.84.0/24 [115 pref/20 metric] updated 1d04h ago
         via 20.30.32.30, Ethernet1
>I    20.30.120.0/24 [115 pref/20 metric] updated 07:34:10 ago
         via 20.30.32.30, Ethernet1
>I    20.30.124.0/24 [115 pref/20 metric] updated 1d04h ago
         via 20.30.32.30, Ethernet1
>I    20.30.128.0/24 [115 pref/20 metric] updated 1d00h ago
         via 20.30.32.30, Ethernet1
>I    20.30.131.0/24 [115 pref/20 metric] updated 03:14:23 ago
         via 20.30.32.30, Ethernet1
>I    20.30.156.0/24 [115 pref/20 metric] updated 09:25:14 ago
         via 20.30.32.30, Ethernet1
>I    20.30.179.0/24 [115 pref/20 metric] updated 1d04h ago
         via 20.30.32.30, Ethernet1
>I    20.30.184.0/24 [115 pref/20 metric] updated 04:40:18 ago
         via 20.30.32.30, Ethernet1
>I    20.30.214.0/24 [115 pref/20 metric] updated 1d04h ago
         via 20.30.32.30, Ethernet1
>I    20.30.217.0/24 [115 pref/20 metric] updated 1d04h ago
         via 20.30.32.30, Ethernet1
>I    20.30.221.0/24 [115 pref/20 metric] updated 03:09:06 ago
         via 20.30.32.30, Ethernet1
>I    20.53.175.0/24 [115 pref/25 metric] updated 07:47:10 ago
         via 20.32.175.175, Ethernet5
>I    20.84.175.0/24 [115 pref/25 metric] updated 07:47:10 ago
         via 20.32.175.175, Ethernet5
>I    20.120.175.0/24 [115 pref/25 metric] updated 07:47:10 ago
         via 20.32.175.175, Ethernet5
>I    20.120.214.0/24 [115 pref/30 metric] updated 07:33:59 ago
         via 20.30.32.30, Ethernet1
>I    20.120.217.0/24 [115 pref/20 metric] updated 04:20:36 ago
         via 20.30.32.30, Ethernet1
>I    20.124.175.0/24 [115 pref/25 metric] updated 07:47:10 ago
         via 20.32.175.175, Ethernet5
>I    20.128.175.0/24 [115 pref/25 metric] updated 07:47:10 ago
         via 20.32.175.175, Ethernet5
>I    20.131.175.0/24 [115 pref/25 metric] updated 07:47:10 ago
         via 20.32.175.175, Ethernet5
>I    20.156.175.0/24 [115 pref/20 metric] updated 07:47:10 ago
         via 20.32.175.175, Ethernet5
>I    20.175.179.0/24 [115 pref/25 metric] updated 07:47:10 ago
         via 20.32.175.175, Ethernet5
>I    20.175.184.0/24 [115 pref/25 metric] updated 07:47:10 ago
         via 20.32.175.175, Ethernet5
>I    20.175.214.0/24 [115 pref/25 metric] updated 07:47:10 ago
         via 20.32.175.175, Ethernet5
>I    20.175.217.0/24 [115 pref/25 metric] updated 07:47:10 ago
         via 20.32.175.175, Ethernet5
>I    20.175.221.0/24 [115 pref/25 metric] updated 03:09:11 ago
         via 20.32.175.175, Ethernet5
>I    20.214.216.0/24 [115 pref/30 metric] updated 1d03h ago
         via 20.30.32.30, Ethernet1
>I    192.168.20.0/23 [115 pref/20 metric] updated 04:20:36 ago
         via 20.30.32.30, Ethernet1
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
>C    2001:0:30:32::/64 [0 pref/0 metric] updated 1d08h ago
         via Ethernet1, directly connected
>C    2001:0:32:175::/64 [0 pref/0 metric] updated 1d07h ago
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
>P    ::/96 [1 pref/0 metric] updated 1d08h ago
         via Null0, directly connected [NF]
>P    ::ffff:127.0.0.0/104 [1 pref/0 metric] updated 1d08h ago
         via :: [1 pref/1 metric] type ipv6
            via , directly connected
>P    fe80::/10 [1 pref/0 metric] updated 1d08h ago
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
>I    2001:0:30:84::/64 [115 pref/20 metric] updated 1d04h ago
         via fe80::c6ca:2bff:fe45:a215, Ethernet1
>I    2001:0:30:120::/64 [115 pref/20 metric] updated 07:34:10 ago
         via fe80::c6ca:2bff:fe45:a215, Ethernet1
>I    2001:0:30:124::/64 [115 pref/20 metric] updated 1d04h ago
         via fe80::c6ca:2bff:fe45:a215, Ethernet1
>I    2001:0:30:128::/64 [115 pref/20 metric] updated 1d00h ago
         via fe80::c6ca:2bff:fe45:a215, Ethernet1
>I    2001:0:30:131::/64 [115 pref/20 metric] updated 03:14:23 ago
         via fe80::c6ca:2bff:fe45:a215, Ethernet1
>I    2001:0:30:156::/64 [115 pref/20 metric] updated 09:25:14 ago
         via fe80::c6ca:2bff:fe45:a215, Ethernet1
>I    2001:0:30:179::/64 [115 pref/20 metric] updated 1d04h ago
         via fe80::c6ca:2bff:fe45:a215, Ethernet1
>I    2001:0:30:184::/64 [115 pref/20 metric] updated 04:40:18 ago
         via fe80::c6ca:2bff:fe45:a215, Ethernet1
>I    2001:0:30:214::/64 [115 pref/20 metric] updated 1d04h ago
         via fe80::c6ca:2bff:fe45:a215, Ethernet1
>I    2001:0:30:217::/64 [115 pref/20 metric] updated 1d04h ago
         via fe80::c6ca:2bff:fe45:a215, Ethernet1
>I    2001:0:30:221::/64 [115 pref/20 metric] updated 03:09:06 ago
         via fe80::c6ca:2bff:fe45:a215, Ethernet1
>I    2001:0:53:120::/64 [115 pref/20 metric] updated 09:43:08 ago
         via fe80::c6ca:2bff:fe45:a215, Ethernet1
>I    2001:0:84:175::/64 [115 pref/30 metric] updated 1d04h ago
         via fe80::c6ca:2bff:fe45:a215, Ethernet1
>I    2001:0:120:175::/64 [115 pref/30 metric] updated 07:33:59 ago
         via fe80::c6ca:2bff:fe45:a215, Ethernet1
>I    2001:0:120:214::/64 [115 pref/30 metric] updated 07:33:59 ago
         via fe80::c6ca:2bff:fe45:a215, Ethernet1
```

## show platform sand l3 summary

```text
Number of vrfs: 4

Ipv4:
  Routes:       122  backlog:  0  unprogrammed:  0
  Adjacencies:  141  backlog:  0  unprogrammed:  0
Ipv6:
  Routes:       36   backlog:  0  unprogrammed:  0
  Adjacencies:  141  backlog:  0  unprogrammed:  0
Mpls:
  Routes:       49  backlog:  0  unprogrammed:  0
  Adjacencies:  3   backlog:  0  unprogrammed:  0

Jericho2 Ip Fecs:
  Non-ecmp fecs:  4188  ecmp fecs:  2  fec entries:  4192
Jericho2 Mpls Fecs:
  Non-ecmp fecs:  3  ecmp fecs:  0  fec entries:  3
Jericho2 Vxlan Tunnel Fecs:
  Non-ecmp fecs:  0  ecmp fecs:  0  fec entries:  0
  Number of vxlan tunnels configured: 0

Jericho2 Lpm Routes:
  Routes:   122  unprogrammed:   0   
  Routes6:  36   unprogrammed6:  0   
  Backlog:  0  

Jericho2 Lpm:
  TCAM entries used:   4   Percent free:  99  ADS2 entries used:   6  Percent free:  99
  Pivot buckets used:  6   Rows used:     2   Entries Per Bucket:  1  Percent free:  99
  Route buckets used:  30  Rows used:     4   Entries Per Bucket:  5  Percent free:  99

Lem:
  IPv4  Host in Lem:            disabled
  IPv4  Prefix-lengths in Lem:  None    
  IPv6  Host in Lem:            disabled
  IPv6  Prefix-lengths in Lem:  None    
  Number of downloads:        0
  Number of overflow events:  0

Egress Arp rewrite entries in use (in each fap):
  FixedSystem: 5
Egress Arp remote rewrite entries in use (in each fap):
  FixedSystem: 0
Egress Ip tunnel rewrite entries in use (in each fap):
  FixedSystem: 0
Egress Mpls (for outer 2 labels) rewrite entries in use (in each fap):
  FixedSystem: 0
Egress Mpls (for inner 2 labels) rewrite entries in use (in each fap):
  FixedSystem: 44
Egress Sflow rewrite entries in use (in each fap):
  FixedSystem: 0

Egress rewrite chains in backlog: resource-full 0, no-interface 0

Glem entries used per fap :
  FixedSystem: 4169

Jericho2 Fec:
  Maximum FEC hierarchy levels:  2
  ReusedEcmp:  0  allocs:  13416  frees:  13322  shuffles:  0  cmds:  0
  Zombies:     0    purges:    0
  Quarantine:  0/0  shuffles:  0  deletes:  0   
  Preserved FECs: 0
    First FEC preserved: never
    Last FEC preserved: never
  Fec insertion failures:  0
  Level1  Fecs:
    Non-ecmp fecs:            40  ecmp fecs:            1 
    Non-ecmp (Percent free):  99  ecmp (Percent free):  99
  Level2  Fecs:
    Non-ecmp fecs:            56  ecmp fecs:            2 
    Non-ecmp (Percent free):  99  ecmp (Percent free):  99
  Level3  Fecs:
    Non-ecmp fecs:            0    ecmp fecs:            0  
    Non-ecmp (Percent free):  100  ecmp (Percent free):  100

Lpm Detail:
  Requests:  8093  cleanses:  5474  batches:  5474  avg batch size:  1

Jericho Arp:
  ArpTable writes:      194320  queued      0   
  IngressTable writes:  152466  queued      0   
  Coprocessors:         1       in CmdRing

Tunnel Counter Status
  Number of MPLS tunnels:                  68   
  Number of uncountable MPLS tunnels:      25   
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
|0  |10.0.0.30/32      |ROUTE| Et1                |1006 |107517  | c4:ca:2b:45:a2:15 |  -  |288369|   -   
|0  |10.0.0.32/32      |TRAP | CoppSystemIpUcast  |0    |  -     | Receive           |  -  |524291|   -   
|0  |10.0.0.53/32      |ROUTE| Et1                |1006 |107517  | c4:ca:2b:45:a2:15 |  -  |288369|   -   
|0  |10.0.0.84/32      |ROUTE| Et1                |1006 |107517  | c4:ca:2b:45:a2:15 |  -  |288369|   -   
|0  |10.0.0.120/32     |ROUTE| Et1                |1006 |107517  | c4:ca:2b:45:a2:15 |  -  |288369|   -   
|0  |10.0.0.124/32     |ROUTE| Et1                |1006 |107517  | c4:ca:2b:45:a2:15 |  -  |288369|   -   
|0  |10.0.0.128/32     |ROUTE| Et1                |1006 |107517  | c4:ca:2b:45:a2:15 |  -  |288369|   -   
|0  |10.0.0.131/32     |ROUTE| Et1                |1006 |107517  | c4:ca:2b:45:a2:15 |  -  |288369|   -   
|0  |10.0.0.156/32     |ROUTE| Et5                |1010 |107518  | 3c:08:cd:8d:ba:dc |16386|288389|   -   
|0  |10.0.0.156/32     |ROUTE| Et1                |1006 |107517  | c4:ca:2b:45:a2:15 |16386|288390|   -   
|0  |10.0.0.175/32     |ROUTE| Et5                |1010 |107518  | 3c:08:cd:8d:ba:dc |  -  |288386|   -   
|0  |10.0.0.179/32     |ROUTE| Et1                |1006 |107517  | c4:ca:2b:45:a2:15 |  -  |288369|   -   
|0  |10.0.0.184/32     |ROUTE| Et1                |1006 |107517  | c4:ca:2b:45:a2:15 |  -  |288369|   -   
|0  |10.0.0.214/32     |ROUTE| Et1                |1006 |107517  | c4:ca:2b:45:a2:15 |  -  |288369|   -   
|0  |10.0.0.216/32     |ROUTE| Et1                |1006 |107517  | c4:ca:2b:45:a2:15 |  -  |288369|   -   
|0  |10.0.0.217/32     |ROUTE| Et1                |1006 |107517  | c4:ca:2b:45:a2:15 |  -  |288369|   -   
|0  |10.0.0.221/32     |ROUTE| Et1                |1006 |107517  | c4:ca:2b:45:a2:15 |  -  |288369|   -   
|0  |20.30.32.0/32     |TRAP | CoppSystemIpBcast  |0    |  -     | BcastReceive      |  -  |524290|   -   
|0  |20.30.32.30/32    |ROUTE| Et1                |1006 |107517  | c4:ca:2b:45:a2:15 |  -  |288368|   -   
|0  |20.30.32.32/32    |TRAP | CoppSystemIpUcast  |0    |  -     | Receive           |  -  |524291|   -   
|0  |20.30.32.255/32   |TRAP | CoppSystemIpBcast  |0    |  -     | BcastReceive      |  -  |524290|   -   
|0  |20.30.32.0/24     |TRAP | CoppSystemL3DstMiss|1006 |1006    | ArpTrap           |  -  |525301|   -   
|0  |20.30.53.0/24     |ROUTE| Et1                |1006 |107517  | c4:ca:2b:45:a2:15 |  -  |288369|   -   
|0  |20.30.84.0/24     |ROUTE| Et1                |1006 |107517  | c4:ca:2b:45:a2:15 |  -  |288369|   -   
|0  |20.30.120.0/24    |ROUTE| Et1                |1006 |107517  | c4:ca:2b:45:a2:15 |  -  |288369|   -   
|0  |20.30.124.0/24    |ROUTE| Et1                |1006 |107517  | c4:ca:2b:45:a2:15 |  -  |288369|   -   
|0  |20.30.128.0/24    |ROUTE| Et1                |1006 |107517  | c4:ca:2b:45:a2:15 |  -  |288369|   -   
|0  |20.30.131.0/24    |ROUTE| Et1                |1006 |107517  | c4:ca:2b:45:a2:15 |  -  |288369|   -   
|0  |20.30.156.0/24    |ROUTE| Et1                |1006 |107517  | c4:ca:2b:45:a2:15 |  -  |288369|   -   
|0  |20.30.179.0/24    |ROUTE| Et1                |1006 |107517  | c4:ca:2b:45:a2:15 |  -  |288369|   -   
|0  |20.30.184.0/24    |ROUTE| Et1                |1006 |107517  | c4:ca:2b:45:a2:15 |  -  |288369|   -   
|0  |20.30.214.0/24    |ROUTE| Et1                |1006 |107517  | c4:ca:2b:45:a2:15 |  -  |288369|   -   
|0  |20.30.217.0/24    |ROUTE| Et1                |1006 |107517  | c4:ca:2b:45:a2:15 |  -  |288369|   -   
|0  |20.30.221.0/24    |ROUTE| Et1                |1006 |107517  | c4:ca:2b:45:a2:15 |  -  |288369|   -   
|0  |20.32.175.0/32    |TRAP | CoppSystemIpBcast  |0    |  -     | BcastReceive      |  -  |524290|   -   
|0  |20.32.175.32/32   |TRAP | CoppSystemIpUcast  |0    |  -     | Receive           |  -  |524291|   -   
|0  |20.32.175.175/32  |ROUTE| Et5                |1010 |107518  | 3c:08:cd:8d:ba:dc |  -  |288367|   -   
|0  |20.32.175.255/32  |TRAP | CoppSystemIpBcast  |0    |  -     | BcastReceive      |  -  |524290|   -   
|0  |20.32.175.0/24    |TRAP | CoppSystemL3DstMiss|1010 |1010    | ArpTrap           |  -  |525305|   -   
|0  |20.53.175.0/24    |ROUTE| Et5                |1010 |107518  | 3c:08:cd:8d:ba:dc |  -  |288386|   -   
|0  |20.84.175.0/24    |ROUTE| Et5                |1010 |107518  | 3c:08:cd:8d:ba:dc |  -  |288386|   -   
|0  |20.120.175.0/24   |ROUTE| Et5                |1010 |107518  | 3c:08:cd:8d:ba:dc |  -  |288386|   -   
|0  |20.120.214.0/24   |ROUTE| Et1                |1006 |107517  | c4:ca:2b:45:a2:15 |  -  |288369|   -   
|0  |20.120.217.0/24   |ROUTE| Et1                |1006 |107517  | c4:ca:2b:45:a2:15 |  -  |288369|   -   
|0  |20.124.175.0/24   |ROUTE| Et5                |1010 |107518  | 3c:08:cd:8d:ba:dc |  -  |288386|   -   
|0  |20.128.175.0/24   |ROUTE| Et5                |1010 |107518  | 3c:08:cd:8d:ba:dc |  -  |288386|   -   
|0  |20.131.175.0/24   |ROUTE| Et5                |1010 |107518  | 3c:08:cd:8d:ba:dc |  -  |288386|   -   
|0  |20.156.175.0/24   |ROUTE| Et5                |1010 |107518  | 3c:08:cd:8d:ba:dc |  -  |288386|   -   
|0  |20.175.179.0/24   |ROUTE| Et5                |1010 |107518  | 3c:08:cd:8d:ba:dc |  -  |288386|   -   
|0  |20.175.184.0/24   |ROUTE| Et5                |1010 |107518  | 3c:08:cd:8d:ba:dc |  -  |288386|   -   
|0  |20.175.214.0/24   |ROUTE| Et5                |1010 |107518  | 3c:08:cd:8d:ba:dc |  -  |288386|   -   
|0  |20.175.217.0/24   |ROUTE| Et5                |1010 |107518  | 3c:08:cd:8d:ba:dc |  -  |288386|   -   
|0  |20.175.221.0/24   |ROUTE| Et5                |1010 |107518  | 3c:08:cd:8d:ba:dc |  -  |288386|   -   
|0  |20.214.216.0/24   |ROUTE| Et1                |1006 |107517  | c4:ca:2b:45:a2:15 |  -  |288369|   -   
|0  |127.0.0.0/8       |TRAP | CoppSystemL3DstMiss|0    |  -     | ArpTrap           |  -  |524295|   -   
|0  |192.168.20.0/23   |ROUTE| Et1                |1006 |107517  | c4:ca:2b:45:a2:15 |  -  |288369|   -   
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
|2  |50.10.32.255/32   |TRAP | CoppSystemIpBcast  |0    |  -     | BcastReceive      |  -  |524290|   -   
|2  |50.10.32.0/24     |TRAP | CoppSystemL3DstMiss|1008 |1008    | ArpTrap           |  -  |525303|   -   
|2  |50.10.84.0/24     |ROUTE| FEC 288399         |0    |2097101 | 00:00:00:00:00:00 |  -  |157319|M 720896
|2  |50.10.131.0/24    |ROUTE| FEC 288404         |0    |2097148 | 00:00:00:00:00:00 |  -  |157288|M 18
|2  |50.10.156.0/24    |ROUTE| FEC 16387          |0    |2097143 | 00:00:00:00:00:00 |  -  |157296|M 20156 16
|2  |50.10.179.0/24    |ROUTE| FEC 288375         |0    |2097092 | 00:00:00:00:00:00 |  -  |157294|M 16
|2  |50.10.214.0/24    |ROUTE| FEC 288400         |0    |2097100 | 00:00:00:00:00:00 |  -  |157305|M 500000
|2  |50.10.217.0/24    |ROUTE| FEC 288379         |0    |2097087 | 00:00:00:00:00:00 |  -  |157306|M 524287
|2  |127.0.0.0/8       |TRAP | CoppSystemL3DstMiss|0    |  -     | ArpTrap           |  -  |524295|   -   
|2  |0.0.0.0/0         |TRAP | CoppSystemL3LpmOver|0    |  -     | SlowReceive       |  -  |524293|   -   
|3  |0.0.0.0/8         |DROP | DROP               |0    |  -     |                   |  -  |288402|   -   
|3  |50.128.32.0/32    |TRAP | CoppSystemIpBcast  |0    |  -     | BcastReceive      |  -  |524290|   -   
|3  |50.128.32.1/32    |TRAP | CoppSystemIpUcast  |0    |  -     | Receive           |  -  |524291|   -   
|3  |50.128.32.2/32    |ROUTE| Et40               |1011 |107522  | 00:28:01:00:00:01 |  -  |288417|   -   
|3  |50.128.32.255/32  |TRAP | CoppSystemIpBcast  |0    |  -     | BcastReceive      |  -  |524290|   -   
|3  |50.128.32.0/24    |TRAP | CoppSystemL3DstMiss|1011 |1011    | ArpTrap           |  -  |525306|   -   
|3  |50.128.53.0/24    |ROUTE| FEC 288408         |0    |2097130 | 00:00:00:00:00:00 |  -  |157292|M 970000
|3  |50.128.120.0/24   |ROUTE| FEC 288362         |0    |2097131 | 00:00:00:00:00:00 |  -  |157322|M 1272
|3  |50.128.124.0/24   |ROUTE| FEC 288410         |0    |2097112 | 00:00:00:00:00:00 |  -  |157314|M 454
|3  |50.128.128.0/24   |ROUTE| FEC 288394         |0    |2097118 | 00:00:00:00:00:00 |  -  |157297|M 48182
|3  |50.128.156.0/24   |ROUTE| FEC 288370         |0    |2097128 | 00:00:00:00:00:00 |  -  |157333|M 21
|3  |50.128.179.0/24   |ROUTE| FEC 288374         |0    |2097113 | 00:00:00:00:00:00 |  -  |157328|M 21
|3  |50.128.184.0/24   |ROUTE| FEC 288384         |0    |2097135 | 00:00:00:00:00:00 |  -  |157310|M 16
|3  |50.128.217.0/24   |ROUTE| FEC 288373         |0    |2097114 | 00:00:00:00:00:00 |  -  |157320|M 524284
|3  |50.128.221.0/24   |ROUTE| FEC 288383         |0    |2097127 | 00:00:00:00:00:00 |  -  |157299|M 524291
|3  |50.129.32.0/32    |TRAP | CoppSystemIpBcast  |0    |  -     | BcastReceive      |  -  |524290|   -   
|3  |50.129.32.1/32    |TRAP | CoppSystemIpUcast  |0    |  -     | Receive           |  -  |524291|   -   
|3  |50.129.32.2/32    |ROUTE| Et40               |1012 |107520  | 00:28:01:00:00:02 |  -  |288385|   -   
|3  |50.129.32.255/32  |TRAP | CoppSystemIpBcast  |0    |  -     | BcastReceive      |  -  |524290|   -   
|3  |50.129.32.0/24    |TRAP | CoppSystemL3DstMiss|1012 |1012    | ArpTrap           |  -  |525307|   -   
|3  |50.129.53.0/24    |ROUTE| FEC 288420         |0    |2097119 | 00:00:00:00:00:00 |  -  |157318|M 970000
|3  |50.129.120.0/24   |ROUTE| FEC 288378         |0    |2097137 | 00:00:00:00:00:00 |  -  |157290|M 1274
|3  |50.129.124.0/24   |ROUTE| FEC 288396         |0    |2097115 | 00:00:00:00:00:00 |  -  |157324|M 457
|3  |50.129.128.0/24   |ROUTE| FEC 288397         |0    |2097111 | 00:00:00:00:00:00 |  -  |157331|M 48185
|3  |50.129.156.0/24   |ROUTE| FEC 288395         |0    |2097116 | 00:00:00:00:00:00 |  -  |157334|M 21
|3  |50.129.179.0/24   |ROUTE| FEC 288405         |0    |2097136 | 00:00:00:00:00:00 |  -  |157329|M 21
|3  |50.129.184.0/24   |ROUTE| FEC 288418         |0    |2097147 | 00:00:00:00:00:00 |  -  |157307|M 17
|3  |50.129.217.0/24   |ROUTE| FEC 288393         |0    |2097139 | 00:00:00:00:00:00 |  -  |157313|M 524284
|3  |50.129.221.0/24   |ROUTE| FEC 288382         |0    |2097117 | 00:00:00:00:00:00 |  -  |157291|M 524291
|3  |50.130.32.0/32    |TRAP | CoppSystemIpBcast  |0    |  -     | BcastReceive      |  -  |524290|   -   
|3  |50.130.32.1/32    |TRAP | CoppSystemIpUcast  |0    |  -     | Receive           |  -  |524291|   -   
|3  |50.130.32.2/32    |ROUTE| Et40               |1013 |107519  | 00:28:01:00:00:03 |  -  |288388|   -   
|3  |50.130.32.255/32  |TRAP | CoppSystemIpBcast  |0    |  -     | BcastReceive      |  -  |524290|   -   
|3  |50.130.32.0/24    |TRAP | CoppSystemL3DstMiss|1013 |1013    | ArpTrap           |  -  |525308|   -   
|3  |50.130.53.0/24    |ROUTE| FEC 288411         |0    |2097149 | 00:00:00:00:00:00 |  -  |157309|M 21183 970000
|3  |50.130.120.0/24   |ROUTE| FEC 288411         |0    |2097151 | 00:00:00:00:00:00 |  -  |157311|M 21250 1273
|3  |50.130.124.0/24   |ROUTE| FEC 288411         |0    |2097138 | 00:00:00:00:00:00 |  -  |157325|M 21254 458
|3  |50.130.128.0/24   |ROUTE| FEC 288411         |0    |2097134 | 00:00:00:00:00:00 |  -  |157332|M 21258 48186
|3  |50.130.156.0/24   |ROUTE| FEC 288411         |0    |2097140 | 00:00:00:00:00:00 |  -  |157335|M 21286 21
|3  |50.130.179.0/24   |ROUTE| FEC 288411         |0    |2097142 | 00:00:00:00:00:00 |  -  |157330|M 21309 21
|3  |50.130.184.0/24   |ROUTE| FEC 288406         |0    |2097144 | 00:00:00:00:00:00 |  -  |157300|M 20184 18
|3  |50.130.217.0/24   |ROUTE| FEC 288411         |0    |2097133 | 00:00:00:00:00:00 |  -  |157304|M 21347 524284
|3  |50.130.221.0/24   |ROUTE| FEC 288411         |0    |2097141 | 00:00:00:00:00:00 |  -  |157302|M 21351 524291
|3  |127.0.0.0/8       |TRAP | CoppSystemL3DstMiss|0    |  -     | ArpTrap           |  -  |524295|   -   
|3  |0.0.0.0/0         |TRAP | CoppSystemL3LpmOver|0    |  -     | SlowReceive       |  -  |524293|   -   

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
|16386|288389|ROUTE| Et5                |1010 |107518  | 3c:08:cd:8d:ba:dc |   -   
|16386|288390|ROUTE| Et1                |1006 |107517  | c4:ca:2b:45:a2:15 |   -   
|16387|288391|ROUTE| Et5                |1010 |107518  | 3c:08:cd:8d:ba:dc |   -   
|16387|288392|ROUTE| Et1                |1006 |107517  | c4:ca:2b:45:a2:15 |   -   
|  -  |157288|ROUTE| FEC 288404         |   - |2097148 |                 - |Mpush 18
|  -  |157289|ROUTE| FEC 288404         |   - |2097148 |                 - |Mpush 18
|  -  |157290|ROUTE| FEC 288378         |   - |2097137 |                 - |Mpush 1274
|  -  |157291|ROUTE| FEC 288382         |   - |2097117 |                 - |Mpush 524291
|  -  |157292|ROUTE| FEC 288408         |   - |2097130 |                 - |Mpush 970000
|  -  |157294|ROUTE| FEC 288375         |   - |2097092 |                 - |Mpush 16
|  -  |157295|ROUTE| FEC 288375         |   - |2097092 |                 - |Mpush 16
|  -  |157296|ROUTE| FEC 16387          |   - |2097143 |                 - |Mpush 20156 16
|  -  |157297|ROUTE| FEC 288394         |   - |2097118 |                 - |Mpush 48182
|  -  |157298|ROUTE| FEC 16387          |   - |2097143 |                 - |Mpush 20156 16
|  -  |157299|ROUTE| FEC 288383         |   - |2097127 |                 - |Mpush 524291
|  -  |157300|ROUTE| FEC 288412         |   - |2097147 |                 - |Mpush 20184 18
|  -  |157302|ROUTE| FEC 288411         |   - |2097141 |                 - |Mpush 21351 524291
|  -  |157303|ROUTE| FEC 288401         |   - |2097098 |                 - |Mpush 333
|  -  |157304|ROUTE| FEC 288411         |   - |2097133 |                 - |Mpush 21347 524284
|  -  |157305|ROUTE| FEC 288400         |   - |2097100 |                 - |Mpush 500000
|  -  |157306|ROUTE| FEC 288379         |   - |2097087 |                 - |Mpush 524287
|  -  |157307|ROUTE| FEC 288409         |   - |2097145 |                 - |Mpush 17
|  -  |157308|ROUTE| FEC 288399         |   - |2097102 |                 - |Mpush 720897
|  -  |157309|ROUTE| FEC 288411         |   - |2097149 |                 - |Mpush 21183 970000
|  -  |157310|ROUTE| FEC 288384         |   - |2097146 |                 - |Mpush 16
|  -  |157311|ROUTE| FEC 288411         |   - |2097151 |                 - |Mpush 21250 1273
|  -  |157313|ROUTE| FEC 288393         |   - |2097139 |                 - |Mpush 524284
|  -  |157314|ROUTE| FEC 288410         |   - |2097112 |                 - |Mpush 454
|  -  |157318|ROUTE| FEC 288420         |   - |2097119 |                 - |Mpush 970000
|  -  |157319|ROUTE| FEC 288399         |   - |2097101 |                 - |Mpush 720896
|  -  |157320|ROUTE| FEC 288373         |   - |2097114 |                 - |Mpush 524284
|  -  |157321|ROUTE| FEC 288400         |   - |2097100 |                 - |Mpush 500000
|  -  |157322|ROUTE| FEC 288362         |   - |2097131 |                 - |Mpush 1272
|  -  |157323|ROUTE| FEC 288379         |   - |2097087 |                 - |Mpush 524287
|  -  |157324|ROUTE| FEC 288396         |   - |2097115 |                 - |Mpush 457
|  -  |157325|ROUTE| FEC 288411         |   - |2097138 |                 - |Mpush 21254 458
|  -  |157328|ROUTE| FEC 288374         |   - |2097113 |                 - |Mpush 21
|  -  |157329|ROUTE| FEC 288405         |   - |2097136 |                 - |Mpush 21
|  -  |157330|ROUTE| FEC 288411         |   - |2097142 |                 - |Mpush 21309 21
|  -  |157331|ROUTE| FEC 288397         |   - |2097111 |                 - |Mpush 48185
|  -  |157332|ROUTE| FEC 288411         |   - |2097134 |                 - |Mpush 21258 48186
|  -  |157333|ROUTE| FEC 288370         |   - |2097128 |                 - |Mpush 21
|  -  |157334|ROUTE| FEC 288395         |   - |2097116 |                 - |Mpush 21
|  -  |157335|ROUTE| FEC 288411         |   - |2097140 |                 - |Mpush 21286 21
|  -  |288360|DROP | DROP               |0    |  -     |                   |   -   
|  -  |288361|DROP | DROP               |0    |  -     |                   |   -   
|  -  |288362|ROUTE| Et1                |1006 |107531  | c4:ca:2b:45:a2:15 |Mpush 21248
|  -  |288363|ROUTE| Et1                |1006 |107517  | c4:ca:2b:45:a2:15 |   -   
|  -  |288364|DROP | DROP               |0    |  -     |                   |   -   
|  -  |288365|ROUTE| Et1                |1006 |107517  | c4:ca:2b:45:a2:15 |   -   
|  -  |288366|DROP | DROP               |0    |  -     |                   |   -   
|  -  |288367|ROUTE| Et5                |1010 |107518  | 3c:08:cd:8d:ba:dc |   -   
|  -  |288368|ROUTE| Et1                |1006 |107517  | c4:ca:2b:45:a2:15 |   -   
|  -  |288369|ROUTE| Et1                |1006 |107517  | c4:ca:2b:45:a2:15 |   -   
|  -  |288370|ROUTE| Et1                |1006 |107533  | c4:ca:2b:45:a2:15 |Mpush 21284
|  -  |288371|ROUTE| Et1                |1006 |107537  | c4:ca:2b:45:a2:15 |   -   
|  -  |288372|ROUTE| Et5                |1010 |107518  | 3c:08:cd:8d:ba:dc |   -   
|  -  |288373|ROUTE| Et1                |1006 |107566  | c4:ca:2b:45:a2:15 |Mpush 21345
|  -  |288374|ROUTE| Et1                |1006 |107567  | c4:ca:2b:45:a2:15 |Mpush 21307
|  -  |288375|ROUTE| Et1                |1006 |107549  | c4:ca:2b:45:a2:15 |Mpush 20179
|  -  |288376|DROP | DROP               |0    |  -     |                   |   -   
|  -  |288377|ROUTE| Et1                |1006 |107538  | c4:ca:2b:45:a2:15 |Mpush 21303
|  -  |288378|ROUTE| Et5                |1010 |107548  | 3c:08:cd:8d:ba:dc |Mpush 21249
|  -  |288379|ROUTE| Et1                |1006 |107552  | c4:ca:2b:45:a2:15 |Mpush 20217
|  -  |288380|ROUTE| Et1                |1006 |107530  | c4:ca:2b:45:a2:15 |   -   
|  -  |288381|ROUTE| Et1                |1006 |107579  | c4:ca:2b:45:a2:15 |   -   
|  -  |288382|ROUTE| Et5                |1010 |107562  | 3c:08:cd:8d:ba:dc |Mpush 21350
|  -  |288383|ROUTE| Et1                |1006 |107557  | c4:ca:2b:45:a2:15 |Mpush 21349
|  -  |288384|ROUTE| Et1                |1006 |107526  | c4:ca:2b:45:a2:15 |Mpush 21312
|  -  |288385|ROUTE| Et40               |1012 |107520  | 00:28:01:00:00:02 |   -   
|  -  |288386|ROUTE| Et5                |1010 |107518  | 3c:08:cd:8d:ba:dc |   -   
|  -  |288387|ROUTE| Et5                |1010 |107555  | 3c:08:cd:8d:ba:dc |   -   
|  -  |288388|ROUTE| Et40               |1013 |107519  | 00:28:01:00:00:03 |   -   
|  -  |288393|ROUTE| Et5                |1010 |107547  | 3c:08:cd:8d:ba:dc |Mpush 21346
|  -  |288394|ROUTE| Et1                |1006 |107561  | c4:ca:2b:45:a2:15 |Mpush 21256
|  -  |288395|ROUTE| Et5                |1010 |107563  | 3c:08:cd:8d:ba:dc |Mpush 21285
|  -  |288396|ROUTE| Et5                |1010 |107564  | 3c:08:cd:8d:ba:dc |Mpush 21253
|  -  |288397|ROUTE| Et5                |1010 |107569  | 3c:08:cd:8d:ba:dc |Mpush 21257
|  -  |288398|ROUTE| Et1                |1006 |107517  | c4:ca:2b:45:a2:15 |   -   
|  -  |288399|ROUTE| Et1                |1006 |107534  | c4:ca:2b:45:a2:15 |Mpush 20084
|  -  |288400|ROUTE| Et1                |1006 |107535  | c4:ca:2b:45:a2:15 |Mpush 20214
|  -  |288401|ROUTE| Et1                |1006 |107536  | c4:ca:2b:45:a2:15 |Mpush 20124
|  -  |288402|DROP | DROP               |0    |  -     |                   |   -   
|  -  |288403|ROUTE| Et1                |1006 |107525  | c4:ca:2b:45:a2:15 |   -   
|  -  |288404|ROUTE| Et1                |1006 |107523  | c4:ca:2b:45:a2:15 |Mpush 20131
|  -  |288405|ROUTE| Et5                |1010 |107550  | 3c:08:cd:8d:ba:dc |Mpush 21308
|  -  |288406|ROUTE| Et1                |1006 |107527  | c4:ca:2b:45:a2:15 |   -   
|  -  |288407|ROUTE| Et5                |1010 |107541  | 3c:08:cd:8d:ba:dc |   -   
|  -  |288408|ROUTE| Et1                |1006 |107532  | c4:ca:2b:45:a2:15 |Mpush 21181
|  -  |288409|ROUTE| Et1                |1006 |107540  | c4:ca:2b:45:a2:15 |Mpush 21313
|  -  |288410|ROUTE| Et1                |1006 |107568  | c4:ca:2b:45:a2:15 |Mpush 21252
|  -  |288411|ROUTE| Et5                |1010 |107518  | 3c:08:cd:8d:ba:dc |   -   
|  -  |288412|ROUTE| Et1                |1006 |107517  | c4:ca:2b:45:a2:15 |   -   
|  -  |288417|ROUTE| Et40               |1011 |107522  | 00:28:01:00:00:01 |   -   
|  -  |288419|ROUTE| Et5                |1010 |107529  | 3c:08:cd:8d:ba:dc |   -   
|  -  |288420|ROUTE| Et5                |1010 |107560  | 3c:08:cd:8d:ba:dc |Mpush 21182
|  -  |524290|TRAP | CoppSystemIpBcast  |0    |  -     | BcastReceive      |   -   
|  -  |524291|TRAP | CoppSystemIpUcast  |0    |  -     | Receive           |   -   
|  -  |524293|TRAP | CoppSystemL3LpmOver|0    |  -     | SlowReceive       |   -   
|  -  |524295|TRAP | CoppSystemL3DstMiss|0    |  -     | ArpTrap           |   -   
|  -  |525301|TRAP | CoppSystemL3DstMiss|1006 |1006    | ArpTrap           |   -   
|  -  |525303|TRAP | CoppSystemL3DstMiss|1008 |1008    | ArpTrap           |   -   
|  -  |525304|TRAP | CoppSystemL3DstMiss|1009 |1009    | ArpTrap           |   -   
|  -  |525305|TRAP | CoppSystemL3DstMiss|1010 |1010    | ArpTrap           |   -   
|  -  |525306|TRAP | CoppSystemL3DstMiss|1011 |1011    | ArpTrap           |   -   
|  -  |525307|TRAP | CoppSystemL3DstMiss|1012 |1012    | ArpTrap           |   -   
|  -  |525308|TRAP | CoppSystemL3DstMiss|1013 |1013    | ArpTrap           |   -   

```

