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

Uptime: 2 days, 10 hours and 50 minutes
Total memory: 8099700 kB
Free memory: 4990928 kB

```

## show lldp neighbors

```text
Last table change time   : 0:02:46 ago
Number of table inserts  : 111
Number of table deletes  : 96
Number of table drops    : 0
Number of table age-outs : 1

Port      Neighbor Device ID                    Neighbor Port ID            TTL
------- ------------------------------------- ----------------------------- ---
Et2       Arista-PE32-Q2C-32.ns.eantc.de        Ethernet1                   120
Et3       H3C_M1A_120                           Ten-GigabitEthernet0/0/17   121
Et4       Nokia-SR1-217                         1610899524                  121
Et5       Nokia-SXR-214                         ethernet-1/4                120
Et11      Juniper-156-PTX10002-36QDD            590                         120
Et12      Ericsson_84_R6678                     5870.7f9f.c403              91 
Et13      Arrcus-53                             swp0                        120
Et15      30c5.0784.3e68                        et-bs/15                    121
Et17      Huawei_124_NetEngine_A816             GigabitEthernet0/2/4        120
Et19      Huawei_128_NetEngine_8000_M14         GigabitEthernet0/5/0        120
Et35      Juniper-131-JCNR                      42                          120
Et35      Juniper-131-JCNR                      eno12429                    120
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
   1    2899.3a8f.91c5    DYNAMIC     Et36       1       1 day, 1:40:51 ago
Total Mac Addresses for this criterion: 1

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
Ethernet9       20.30.72.30/24      down       down              1500          
Ethernet11      20.30.156.30/24     up         up                1500          
Ethernet12      20.30.84.30/24      up         up                1500          
Ethernet13      20.30.53.30/24      up         up                1500          
Ethernet15      20.30.221.30/24     up         up                1500          
Ethernet17      20.30.124.30/24     up         up                1500          
Ethernet19      20.30.128.30/24     up         up                1500          
Ethernet31      20.30.66.30/24      down       down              1500          
Ethernet35      20.30.131.30/24     up         up                1500          
Ethernet40      20.30.179.30/24     up         up                1500          
Loopback0       10.0.0.30/32        up         up               65535          
Loopback5001    10.0.0.30/32        up         up               65535          
Loopback5128    10.128.0.30/32      up         up               65535          
Management1     192.168.20.30/23    up         up                1500          

```

## show interfaces counters rates | nz

```text
Port      Name                 Intvl  In Mbps      %  In Kpps Out Mbps      %
Et2       Arista-PE32-Q2C-32 E  0:01    400.0   4.8%      499    346.7   4.2%
Et3       H3C_120               0:01     50.0   0.6%       62    361.1   4.3%
Et4       Nokia                 0:01      0.0   0.0%        0    411.1   4.9%
Et9       Ciena-5134-72 port 2  0:01      0.0   0.0%        0      0.0   0.0%
Et11      Juniper-156 port 590  0:01    400.0   4.8%      500    346.7   4.2%
Et13      Arrcus-53 port swp0   0:01    400.0   4.8%      499    348.7   4.2%
Et15      Ribbon-221            0:01    400.0   4.8%      499    346.7   4.2%
Et17      Huawei_124_NetEngine  0:01    738.9  88.7%      923    300.0  36.0%
Et19      Huawei_128_NetEngine  0:01    388.9   4.7%      486    288.0   3.5%
Et31      Ciena-8140-66 port 2  0:01      0.0   0.0%        0      0.0   0.0%
Et35      Juniper-131-JCNR 42   0:01      0.0   0.0%        0      0.0   0.0%
Et40      Juniper-179-ACX7024   0:01    400.0   4.8%      500    346.7   4.2%

Port      Out Kpps
Et2            451
Et3            451
Et4            513
Et11           451
Et13           451
Et15           451
Et17           375
Et19           375
Et40           451
```

## show isis neighbors

```text
 
Instance  VRF      System Id        Type Interface          SNPA              State Hold time   Circuit Id          
IGP       default  Arista-PE32-Q2C-32 L2   Ethernet2          P2P               UP    28          44                  
IGP       default  Arrcus-53        L2   Ethernet13         P2P               UP    26          00                  
IGP       default  Ericsson_84_R6678 L2   Ethernet12         P2P               UP    20          02                  
IGP       default  H3C_M1A_120      L2   Ethernet3          P2P               UP    24          01                  
IGP       default  0000.0000.0124   L2   Ethernet17         P2P               UP    29          09                  
IGP       default  0000.0000.0128   L2   Ethernet19         P2P               UP    25          09                  
IGP       default  Juniper-131-JCNR L2   Ethernet35         P2P               UP    25          01                  
IGP       default  Juniper-156-PTX10002-36QDD L2   Ethernet11         P2P               UP    26          01                  
IGP       default  Juniper-179-ACX7024 L2   Ethernet40         P2P               UP    27          01                  
IGP       default  0000.0000.0184   L2   Ethernet7          P2P               UP    28          01                  
IGP       default  Nokia-SXR-214    L2   Ethernet5          P2P               UP    23          00                  
IGP       default  Nokia-SR1-217    L2   Ethernet4          P2P               UP    26          00                  
IGP       default  221              L2   Ethernet15         P2P               UP    78          00                  
```

## show isis database detail

```text
Legend:
H - hostname conflict
U - node unreachable

IS-IS Instance: IGP VRF: default
  IS-IS Level 2 Link State Database
    LSPID                   Seq Num  Cksum  Life Length IS  Received LSPID        Flags
    Arista-Spine3-Q2A-30.00-00       643  15125  1057   1040 L2  0000.0000.0030.00-00  <>
      LSP generation remaining wait time: 0 ms
      Time remaining until refresh: 757 s
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
      LSP generation remaining wait time: 0 ms
      Time remaining until refresh: 681 s
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
      Remaining lifetime received: 1199 s Modified to: 1200 s
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
    Arrcus-53.00-00             407  57015   933    278 L2  0000.0000.0053.00-00  <>
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
 U  Arrcus-36D-3-57.00-00       200  26364 39303    331 L2  0000.0000.0057.00-00  <>
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
 U  Arrcus-36D-3-57.00-01       211  40105 39804    187 L2  0000.0000.0057.00-01  <>
      IS Neighbor          : 0000.0000.0042.00   Metric: 10
        Global IPv6 Interface Address: 2001:0:42:57::57
      IS Neighbor          : 0000.0000.0169.00   Metric: 10
        Global IPv6 Interface Address: 2001:0:57:169::57
      Reachability          : 2001:0:42:57::/64 Metric: 10 Type: 1 Up
 U  Ciena-5134-72.00-00         512  34876    35    469 L2  0000.0000.0072.00-00  <>
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
    Juniper-131-JCNR.00-00        22  36182   438    447 L2  0000.0000.0131.00-00  <>
      Remaining lifetime received: 1198 s Modified to: 1200 s
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
    Juniper-156-PTX10002-36QDD.00-00        69  52849   855    561 L2  0000.0000.0156.00-00  <>
      Remaining lifetime received: 1198 s Modified to: 1200 s
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
    Juniper-175-ACX7100-48L.00-01       175  38018  1025   1165 L2  0000.0000.0175.00-01  <>
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
      Remaining lifetime received: 1198 s Modified to: 1200 s
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
      Remaining lifetime received: 1198 s Modified to: 1200 s
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
    Nokia-SXR-214.00-00        8824  51377  1086    488 L2  0000.0000.0214.00-00  <>
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
    221.00-00                   186  13554   809     86 L2  0221.0221.0221.00-00  <>
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
      Hostname: 221
    221.00-02                  5304  55661  1198    491 L2  0221.0221.0221.00-02  <>
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
Number of times path updated: 6
Last updated: 0:39:42 ago
Metric: 10000
Next Hop      Interface 
------------- ----------
20.30.124.124 Ethernet17

Destination: 0000.0000.0124
Path ID: 641
Path constraints: algo MIN-TE
                  metric type TE
Request sequence number: 0
Response sequence number: 0
Number of times path updated: 4
Last updated: 1:04:17 ago
Metric: 100
Next Hop      Interface 
------------- ----------
20.30.124.124 Ethernet17

Destination: 0000.0000.0124
Path ID: 642
Path constraints: algo ADMIN
                  metric type IGP
                  administrative-group exclude ARISTA(2)
Request sequence number: 0
Response sequence number: 0
Number of times path updated: 6
Last updated: 0:00:00 ago
Next Hop Interface
-------- ---------

Destination: 0000.0000.0128
Path ID: 640
Path constraints: algo MIN-LATENCY
                  metric type MIN-DELAY
Request sequence number: 0
Response sequence number: 0
Number of times path updated: 6
Last updated: 0:39:42 ago
Metric: 10000
Next Hop      Interface 
------------- ----------
20.30.128.128 Ethernet19

Destination: 0000.0000.0128
Path ID: 641
Path constraints: algo MIN-TE
                  metric type TE
Request sequence number: 0
Response sequence number: 0
Number of times path updated: 5
Last updated: 1:04:17 ago
Metric: 100
Next Hop      Interface 
------------- ----------
20.30.128.128 Ethernet19

Destination: 0000.0000.0128
Path ID: 642
Path constraints: algo ADMIN
                  metric type IGP
                  administrative-group exclude ARISTA(2)
Request sequence number: 0
Response sequence number: 0
Number of times path updated: 6
Last updated: 0:00:00 ago
Next Hop Interface
-------- ---------

Destination: 0000.0000.0184
Path ID: 640
Path constraints: algo MIN-LATENCY
                  metric type MIN-DELAY
Request sequence number: 0
Response sequence number: 0
Number of times path updated: 2227
Last updated: 0:00:00 ago
Metric: 10000
Next Hop      Interface
------------- ---------
20.30.184.184 Ethernet7

Destination: 0000.0000.0184
Path ID: 641
Path constraints: algo MIN-TE
                  metric type TE
Request sequence number: 0
Response sequence number: 0
Number of times path updated: 2231
Last updated: 0:00:00 ago
Metric: 100
Next Hop      Interface
------------- ---------
20.30.184.184 Ethernet7

Destination: 0000.0000.0184
Path ID: 642
Path constraints: algo ADMIN
                  metric type IGP
                  administrative-group exclude ARISTA(2)
Request sequence number: 0
Response sequence number: 0
Number of times path updated: 2199
Last updated: 0:00:01 ago
Next Hop Interface
-------- ---------

Destination: 221
Path ID: 640
Path constraints: algo MIN-LATENCY
                  metric type MIN-DELAY
Request sequence number: 0
Response sequence number: 0
Number of times path updated: 6
Last updated: 0:39:42 ago
Metric: 10000
Next Hop      Interface 
------------- ----------
20.30.221.221 Ethernet15

Destination: 221
Path ID: 641
Path constraints: algo MIN-TE
                  metric type TE
Request sequence number: 0
Response sequence number: 0
Number of times path updated: 4
Last updated: 1:04:17 ago
Metric: 100
Next Hop      Interface 
------------- ----------
20.30.221.221 Ethernet15

Destination: 221
Path ID: 642
Path constraints: algo ADMIN
                  metric type IGP
                  administrative-group exclude ARISTA(2)
Request sequence number: 0
Response sequence number: 0
Number of times path updated: 6
Last updated: 0:00:00 ago
Next Hop Interface
-------- ---------

Destination: Arista-PE32-Q2C-32
Path ID: 640
Path constraints: algo MIN-LATENCY
                  metric type MIN-DELAY
Request sequence number: 0
Response sequence number: 0
Number of times path updated: 6
Last updated: 0:39:42 ago
Metric: 10000
Next Hop    Interface
----------- ---------
20.30.32.32 Ethernet2

Destination: Arista-PE32-Q2C-32
Path ID: 641
Path constraints: algo MIN-TE
                  metric type TE
Request sequence number: 0
Response sequence number: 0
Number of times path updated: 5
Last updated: 1:04:17 ago
Metric: 100
Next Hop    Interface
----------- ---------
20.30.32.32 Ethernet2

Destination: Arista-PE32-Q2C-32
Path ID: 642
Path constraints: algo ADMIN
                  metric type IGP
                  administrative-group exclude ARISTA(2)
Request sequence number: 0
Response sequence number: 0
Number of times path updated: 6
Last updated: 0:00:00 ago
Next Hop Interface
-------- ---------

Destination: Arista-Spine3-Q2A-30
Path ID: 640
Path constraints: algo MIN-LATENCY
                  metric type MIN-DELAY
Request sequence number: 0
Response sequence number: 0
Number of times path updated: 1
Last updated: 4:25:30 ago
Next Hop Interface
-------- ---------

Destination: Arista-Spine3-Q2A-30
Path ID: 641
Path constraints: algo MIN-TE
                  metric type TE
Request sequence number: 0
Response sequence number: 0
Number of times path updated: 1
Last updated: 4:25:30 ago
Next Hop Interface
-------- ---------

Destination: Arista-Spine3-Q2A-30
Path ID: 642
Path constraints: algo ADMIN
                  metric type IGP
                  administrative-group exclude ARISTA(2)
Request sequence number: 0
Response sequence number: 0
Number of times path updated: 1
Last updated: 4:25:30 ago
Next Hop Interface
-------- ---------

Destination: Arrcus-53
Path ID: 640
Path constraints: algo MIN-LATENCY
                  metric type MIN-DELAY
Request sequence number: 0
Response sequence number: 0
Number of times path updated: 7
Last updated: 0:39:42 ago
Metric: 10000
Next Hop    Interface 
----------- ----------
20.30.53.53 Ethernet13

Destination: Arrcus-53
Path ID: 641
Path constraints: algo MIN-TE
                  metric type TE
Request sequence number: 0
Response sequence number: 0
Number of times path updated: 5
Last updated: 1:04:17 ago
Metric: 100
Next Hop    Interface 
----------- ----------
20.30.53.53 Ethernet13

Destination: Arrcus-53
Path ID: 642
Path constraints: algo ADMIN
                  metric type IGP
                  administrative-group exclude ARISTA(2)
Request sequence number: 0
Response sequence number: 0
Number of times path updated: 7
Last updated: 0:00:00 ago
Next Hop Interface
-------- ---------

Destination: H3C_M1A_120
Path ID: 640
Path constraints: algo MIN-LATENCY
                  metric type MIN-DELAY
Request sequence number: 0
Response sequence number: 0
Number of times path updated: 6
Last updated: 0:39:42 ago
Metric: 10000
Next Hop      Interface
------------- ---------
20.30.120.120 Ethernet3

Destination: H3C_M1A_120
Path ID: 641
Path constraints: algo MIN-TE
                  metric type TE
Request sequence number: 0
Response sequence number: 0
Number of times path updated: 4
Last updated: 1:04:17 ago
Metric: 100
Next Hop      Interface
------------- ---------
20.30.120.120 Ethernet3

Destination: H3C_M1A_120
Path ID: 642
Path constraints: algo ADMIN
                  metric type IGP
                  administrative-group exclude ARISTA(2)
Request sequence number: 0
Response sequence number: 0
Number of times path updated: 4
Last updated: 0:00:00 ago
Next Hop Interface
-------- ---------

Destination: Juniper-156-PTX10002-36QDD
Path ID: 640
Path constraints: algo MIN-LATENCY
                  metric type MIN-DELAY
Request sequence number: 0
Response sequence number: 0
Number of times path updated: 6
Last updated: 0:39:42 ago
Metric: 10000
Next Hop      Interface 
------------- ----------
20.30.156.156 Ethernet11

Destination: Juniper-156-PTX10002-36QDD
Path ID: 641
Path constraints: algo MIN-TE
                  metric type TE
Request sequence number: 0
Response sequence number: 0
Number of times path updated: 4
Last updated: 1:04:17 ago
Metric: 100
Next Hop      Interface 
------------- ----------
20.30.156.156 Ethernet11

Destination: Juniper-156-PTX10002-36QDD
Path ID: 642
Path constraints: algo ADMIN
                  metric type IGP
                  administrative-group exclude ARISTA(2)
Request sequence number: 0
Response sequence number: 0
Number of times path updated: 6
Last updated: 0:00:00 ago
Next Hop Interface
-------- ---------

Destination: Juniper-175-ACX7100-48L
Path ID: 640
Path constraints: algo MIN-LATENCY
                  metric type MIN-DELAY
Request sequence number: 0
Response sequence number: 0
Number of times path updated: 6
Last updated: 0:39:42 ago
Metric: 10010
Next Hop      Interface 
------------- ----------
20.30.221.221 Ethernet15

Destination: Juniper-175-ACX7100-48L
Path ID: 641
Path constraints: algo MIN-TE
                  metric type TE
Request sequence number: 0
Response sequence number: 0
Number of times path updated: 14
Last updated: 0:17:38 ago
Metric: 110
Next Hop      Interface 
------------- ----------
20.30.221.221 Ethernet15
20.30.179.179 Ethernet40
20.30.124.124 Ethernet17
20.30.156.156 Ethernet11
20.30.128.128 Ethernet19
20.30.53.53   Ethernet13
20.30.120.120 Ethernet3 
20.30.217.217 Ethernet4 
20.30.32.32   Ethernet2 

Destination: Juniper-175-ACX7100-48L
Path ID: 642
Path constraints: algo ADMIN
                  metric type IGP
                  administrative-group exclude ARISTA(2)
Request sequence number: 0
Response sequence number: 0
Number of times path updated: 10
Last updated: 0:00:00 ago
Next Hop Interface
-------- ---------

Destination: Juniper-179-ACX7024
Path ID: 640
Path constraints: algo MIN-LATENCY
                  metric type MIN-DELAY
Request sequence number: 0
Response sequence number: 0
Number of times path updated: 6
Last updated: 0:39:42 ago
Metric: 10000
Next Hop      Interface 
------------- ----------
20.30.179.179 Ethernet40

Destination: Juniper-179-ACX7024
Path ID: 641
Path constraints: algo MIN-TE
                  metric type TE
Request sequence number: 0
Response sequence number: 0
Number of times path updated: 4
Last updated: 1:04:17 ago
Metric: 100
Next Hop      Interface 
------------- ----------
20.30.179.179 Ethernet40

Destination: Juniper-179-ACX7024
Path ID: 642
Path constraints: algo ADMIN
                  metric type IGP
                  administrative-group exclude ARISTA(2)
Request sequence number: 0
Response sequence number: 0
Number of times path updated: 4
Last updated: 0:00:00 ago
Next Hop Interface
-------- ---------

Destination: Nokia-SR1-217
Path ID: 640
Path constraints: algo MIN-LATENCY
                  metric type MIN-DELAY
Request sequence number: 0
Response sequence number: 0
Number of times path updated: 7
Last updated: 0:39:42 ago
Metric: 10000
Next Hop      Interface
------------- ---------
20.30.217.217 Ethernet4

Destination: Nokia-SR1-217
Path ID: 641
Path constraints: algo MIN-TE
                  metric type TE
Request sequence number: 0
Response sequence number: 0
Number of times path updated: 5
Last updated: 1:04:17 ago
Metric: 100
Next Hop      Interface
------------- ---------
20.30.217.217 Ethernet4

Destination: Nokia-SR1-217
Path ID: 642
Path constraints: algo ADMIN
                  metric type IGP
                  administrative-group exclude ARISTA(2)
Request sequence number: 0
Response sequence number: 0
Number of times path updated: 7
Last updated: 0:00:00 ago
Next Hop Interface
-------- ---------

```

## show isis segment-routing tunnel

```text
  Index     Endpoint          Next Hop/Tunnel Index     Interface     Labels   
--------- ----------------- ------------------------- --------------- ---------
  1         10.0.0.84/32      TI-LFA (6)                -             [ 20084 ]
  4         10.0.0.175/32     20.30.32.32               Ethernet2     [ 20175 ]
                              20.30.53.53               Ethernet13    [ 20175 ]
                              20.30.84.84               Ethernet12    [ 20175 ]
                              20.30.120.120             Ethernet3     [ 20175 ]
                              20.30.124.124             Ethernet17    [ 2175 ] 
                              20.30.128.128             Ethernet19    [ 20175 ]
                              20.30.131.131             Ethernet35    [ 20175 ]
                              20.30.156.156             Ethernet11    [ 20175 ]
  5         10.0.0.53/32      TI-LFA (10)               -             [ 3 ]    
  6         10.0.0.179/32     TI-LFA (7)                -             [ 3 ]    
  7         10.0.0.120/32     TI-LFA (0)                -             [ 3 ]    
  9         10.0.0.32/32      TI-LFA (5)                -             [ 3 ]    
  10        10.0.0.214/32     TI-LFA (12)               -             [ 20214 ]
  11        10.0.0.128/32     TI-LFA (29)               -             [ 3 ]    
  12        10.0.0.131/32     TI-LFA (1)                -             [ 3 ]    
  13        10.0.0.221/32     TI-LFA (13)               -             [ 3 ]    
  14        10.0.0.124/32     TI-LFA (8)                -             [ 3 ]    
  15        10.0.0.184/32     20.30.184.184             Ethernet7     [ 3 ]    
  16        10.0.0.217/32     TI-LFA (4)                -             [ 20217 ]
  18        10.0.0.156/32     TI-LFA (11)               -             [ 3 ]    

```

## show isis segment-routing prefix-segments

```text

System ID: Arista-Spine3-Q2A-30			Instance: 'IGP'
SR supported Data-plane: MPLS			SR Router ID: 10.0.0.30

Node: 51     Proxy-Node: 0      Prefix: 0       Total Segments: 51

Flag Descriptions: R: Re-advertised, N: Node Segment, P: no-PHP
                   E: Explicit-NULL, V: Value, L: Local
Segment status codes: * - Self originated Prefix, L1 - level 1, L2 - level 2, ! - SR-unreachable,
                      # - Some IS-IS next-hops are SR-unreachable
   Prefix                      SID   Label Type       Flags                        System ID       Level Protection  Algorithm   
   ------------------------- ----- ------- ---------- ---------------------------- --------------- ----- ----------- -------------
*  10.0.0.30/32                 30   20030 Node       R:0 N:1 P:0 E:0 V:0 L:0      Arista-Spine3-Q2A-30 L2    unprotected SPF         
*  10.0.0.30/32               1158   21158 Node       R:0 N:1 P:0 E:0 V:0 L:0      Arista-Spine3-Q2A-30 L2    unprotected MIN-LATENCY 
*  10.0.0.30/32               1159   21159 Node       R:0 N:1 P:0 E:0 V:0 L:0      Arista-Spine3-Q2A-30 L2    unprotected MIN-TE      
*  10.0.0.30/32               1160   21160 Node       R:0 N:1 P:0 E:0 V:0 L:0      Arista-Spine3-Q2A-30 L2    unprotected ADMIN       
   10.0.0.32/32                 32   20032 Node       R:0 N:1 P:0 E:0 V:0 L:0      Arista-PE32-Q2C-32 L2    node        SPF         
   10.0.0.32/32               1161   21161 Node       R:0 N:1 P:0 E:0 V:0 L:0      Arista-PE32-Q2C-32 L2    node        MIN-LATENCY 
   10.0.0.32/32               1162   21162 Node       R:0 N:1 P:0 E:0 V:0 L:0      Arista-PE32-Q2C-32 L2    node        MIN-TE      
   10.0.0.32/32               1163   21163 Node       R:0 N:1 P:0 E:0 V:0 L:0      Arista-PE32-Q2C-32 L2    unprotected ADMIN       
   10.0.0.53/32                 53   20053 Node       R:0 N:1 P:1 E:1 V:0 L:0      Arrcus-53       L2    node        SPF         
   10.0.0.53/32               1181   21181 Node       R:0 N:1 P:0 E:0 V:0 L:0      Arrcus-53       L2    node        MIN-LATENCY 
   10.0.0.53/32               1182   21182 Node       R:0 N:1 P:0 E:0 V:0 L:0      Arrcus-53       L2    node        MIN-TE      
   10.0.0.53/32               1183   21183 Node       R:0 N:1 P:0 E:0 V:0 L:0      Arrcus-53       L2    unprotected ADMIN       
   10.0.0.84/32                 84   20084 Node       R:0 N:1 P:1 E:0 V:0 L:0      Ericsson_84_R6678 L2    node        SPF         
   10.0.0.120/32               120   20120 Node       R:0 N:1 P:0 E:0 V:0 L:0      H3C_M1A_120     L2    node        SPF         
   10.0.0.120/32              1248   21248 Node       R:0 N:1 P:1 E:0 V:0 L:0      H3C_M1A_120     L2    node        MIN-LATENCY 
   10.0.0.120/32              1249   21249 Node       R:0 N:1 P:1 E:0 V:0 L:0      H3C_M1A_120     L2    node        MIN-TE      
   10.0.0.120/32              1250   21250 Node       R:0 N:1 P:1 E:0 V:0 L:0      H3C_M1A_120     L2    unprotected ADMIN       
   10.0.0.124/32               124    2124 Node       R:0 N:1 P:1 E:0 V:0 L:0      0000.0000.0124  L2    node        SPF         
   10.0.0.124/32              1252    3252 Node       R:0 N:1 P:1 E:0 V:0 L:0      0000.0000.0124  L2    node        MIN-LATENCY 
   10.0.0.124/32              1253    3253 Node       R:0 N:1 P:1 E:0 V:0 L:0      0000.0000.0124  L2    node        MIN-TE      
   10.0.0.124/32              1254    3254 Node       R:0 N:1 P:1 E:0 V:0 L:0      0000.0000.0124  L2    unprotected ADMIN       
   10.0.0.128/32               128   20128 Node       R:0 N:1 P:0 E:0 V:0 L:0      0000.0000.0128  L2    node        SPF         
   10.0.0.128/32              1256   21256 Node       R:0 N:1 P:0 E:0 V:0 L:0      0000.0000.0128  L2    node        MIN-LATENCY 
   10.0.0.128/32              1257   21257 Node       R:0 N:1 P:0 E:0 V:0 L:0      0000.0000.0128  L2    node        MIN-TE      
   10.0.0.128/32              1258   21258 Node       R:0 N:1 P:0 E:0 V:0 L:0      0000.0000.0128  L2    unprotected ADMIN       
   10.0.0.131/32               131   20131 Node       R:0 N:1 P:0 E:0 V:0 L:0      Juniper-131-JCNR L2    node        SPF         
   10.0.0.156/32               156   20156 Node       R:0 N:1 P:0 E:0 V:0 L:0      Juniper-156-PTX10002-36QDD L2    node        SPF         
   10.0.0.156/32              1284   21284 Node       R:0 N:1 P:0 E:0 V:0 L:0      Juniper-156-PTX10002-36QDD L2    node        MIN-LATENCY 
   10.0.0.156/32              1285   21285 Node       R:0 N:1 P:0 E:0 V:0 L:0      Juniper-156-PTX10002-36QDD L2    node        MIN-TE      
   10.0.0.156/32              1286   21286 Node       R:0 N:1 P:0 E:0 V:0 L:0      Juniper-156-PTX10002-36QDD L2    unprotected ADMIN       
   10.0.0.175/32               175   20175 Node       R:0 N:1 P:0 E:0 V:0 L:0      Juniper-175-ACX7100-48L L2    unprotected SPF         
   10.0.0.175/32              1303   21303 Node       R:0 N:1 P:0 E:0 V:0 L:0      Juniper-175-ACX7100-48L L2    node        MIN-LATENCY 
   10.0.0.175/32              1304   21304 Node       R:0 N:1 P:0 E:0 V:0 L:0      Juniper-175-ACX7100-48L L2    unprotected MIN-TE      
   10.0.0.175/32              1305   21305 Node       R:0 N:1 P:0 E:0 V:0 L:0      Juniper-175-ACX7100-48L L2    unprotected ADMIN       
   10.0.0.179/32               179   20179 Node       R:0 N:1 P:0 E:0 V:0 L:0      Juniper-179-ACX7024 L2    node        SPF         
   10.0.0.179/32              1307   21307 Node       R:0 N:1 P:0 E:0 V:0 L:0      Juniper-179-ACX7024 L2    node        MIN-LATENCY 
   10.0.0.179/32              1308   21308 Node       R:0 N:1 P:0 E:0 V:0 L:0      Juniper-179-ACX7024 L2    node        MIN-TE      
   10.0.0.179/32              1309   21309 Node       R:0 N:1 P:0 E:0 V:0 L:0      Juniper-179-ACX7024 L2    unprotected ADMIN       
   10.0.0.184/32               184   20184 Node       R:0 N:1 P:0 E:0 V:0 L:0      0000.0000.0184  L2    unprotected SPF         
   10.0.0.184/32              1312   21312 Node       R:0 N:1 P:0 E:0 V:0 L:0      0000.0000.0184  L2    node        MIN-LATENCY 
   10.0.0.184/32              1313   21313 Node       R:0 N:1 P:0 E:0 V:0 L:0      0000.0000.0184  L2    node        MIN-TE      
   10.0.0.184/32              1314   21314 Node       R:0 N:1 P:0 E:0 V:0 L:0      0000.0000.0184  L2    unprotected ADMIN       
   10.0.0.214/32               214   20214 Node       R:0 N:1 P:1 E:0 V:0 L:0      Nokia-SXR-214   L2    node        SPF         
   10.0.0.217/32               217   20217 Node       R:0 N:1 P:1 E:0 V:0 L:0      Nokia-SR1-217   L2    node        SPF         
   10.0.0.217/32              1345   21345 Node       R:0 N:1 P:1 E:0 V:0 L:0      Nokia-SR1-217   L2    node        MIN-LATENCY 
   10.0.0.217/32              1346   21346 Node       R:0 N:1 P:1 E:0 V:0 L:0      Nokia-SR1-217   L2    node        MIN-TE      
   10.0.0.217/32              1347   21347 Node       R:0 N:1 P:1 E:0 V:0 L:0      Nokia-SR1-217   L2    unprotected ADMIN       
   10.0.0.221/32               221  720221 Node       R:0 N:1 P:0 E:0 V:0 L:0      221             L2    node        SPF         
   10.0.0.221/32              1349  721349 Node       R:0 N:1 P:0 E:0 V:0 L:0      221             L2    node        MIN-LATENCY 
   10.0.0.221/32              1350  721350 Node       R:0 N:1 P:0 E:0 V:0 L:0      221             L2    node        MIN-TE      
   10.0.0.221/32              1351  721351 Node       R:0 N:1 P:0 E:0 V:0 L:0      221             L2    unprotected ADMIN       
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
 I L2     10.0.0.84/32 [115/20]
           via 20.30.84.84, Ethernet12
 I L2     10.0.0.120/32 [115/10]
           via 20.30.120.120, Ethernet3
 I L2     10.0.0.124/32 [115/10]
           via 20.30.124.124, Ethernet17
 I L2     10.0.0.128/32 [115/10]
           via 20.30.128.128, Ethernet19
 I L2     10.0.0.131/32 [115/10]
           via 20.30.131.131, Ethernet35
 I L2     10.0.0.156/32 [115/10]
           via 20.30.156.156, Ethernet11
 I L2     10.0.0.175/32 [115/20]
           via 20.30.32.32, Ethernet2
           via 20.30.120.120, Ethernet3
           via 20.30.156.156, Ethernet11
           via 20.30.84.84, Ethernet12
           via 20.30.53.53, Ethernet13
           via 20.30.124.124, Ethernet17
           via 20.30.128.128, Ethernet19
           via 20.30.131.131, Ethernet35
 I L2     10.0.0.179/32 [115/10]
           via 20.30.179.179, Ethernet40
 I L2     10.0.0.184/32 [115/10]
           via 20.30.184.184, Ethernet7
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
 C        20.30.84.0/24
           directly connected, Ethernet12
 C        20.30.120.0/24
           directly connected, Ethernet3
 C        20.30.124.0/24
           directly connected, Ethernet17
 C        20.30.128.0/24
           directly connected, Ethernet19
 C        20.30.131.0/24
           directly connected, Ethernet35
 C        20.30.156.0/24
           directly connected, Ethernet11
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
 I L2     20.84.175.0/24 [115/35]
           via 20.30.32.32, Ethernet2
           via 20.30.120.120, Ethernet3
           via 20.30.156.156, Ethernet11
           via 20.30.84.84, Ethernet12
           via 20.30.53.53, Ethernet13
           via 20.30.124.124, Ethernet17
           via 20.30.128.128, Ethernet19
           via 20.30.131.131, Ethernet35
 I L2     20.120.175.0/24 [115/20]
           via 20.30.120.120, Ethernet3
 I L2     20.120.214.0/24 [115/20]
           via 20.30.120.120, Ethernet3
 I L2     20.120.217.0/24 [115/10]
           via 20.30.120.120, Ethernet3
 I L2     20.124.175.0/24 [115/20]
           via 20.30.124.124, Ethernet17
 I L2     20.128.175.0/24 [115/20]
           via 20.30.128.128, Ethernet19
 I L2     20.131.175.0/24 [115/20]
           via 20.30.131.131, Ethernet35
 I L2     20.156.175.0/24 [115/20]
           via 20.30.156.156, Ethernet11
 I L2     20.175.179.0/24 [115/20]
           via 20.30.179.179, Ethernet40
 I L2     20.175.184.0/24 [115/35]
           via 20.30.32.32, Ethernet2
           via 20.30.120.120, Ethernet3
           via 20.30.156.156, Ethernet11
           via 20.30.84.84, Ethernet12
           via 20.30.53.53, Ethernet13
           via 20.30.124.124, Ethernet17
           via 20.30.128.128, Ethernet19
           via 20.30.131.131, Ethernet35
 I L2     20.175.214.0/24 [115/20]
           via 20.30.214.214, Ethernet5
 I L2     20.175.217.0/24 [115/20]
           via 20.30.217.217, Ethernet4
 I L2     20.175.221.0/24 [115/20]
           via 20.30.221.221, Ethernet15
 I L2     20.214.216.0/24 [115/20]
           via 20.30.214.214, Ethernet5
 I L2     192.168.20.0/23 [115/10]
           via 20.30.120.120, Ethernet3

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

 C        10.128.0.30/32
           directly connected, Loopback5128
 B I      50.128.32.0/24 [200/0]
           via 10.0.0.32/32, algorithm MIN-LATENCY, IS-IS FlexAlgo tunnel index 8, label 378530
              via TI-LFA tunnel index 53, label imp-null(3)
                 via 20.30.32.32, Ethernet2, label imp-null(3)
                 backup via 20.30.221.221, Ethernet15, label 721303 21161
 B I      50.128.53.0/24 [200/0]
           via 10.0.0.53/32, algorithm MIN-LATENCY, IS-IS FlexAlgo tunnel index 10, label 970000
              via TI-LFA tunnel index 47, label imp-null(3)
                 via 20.30.53.53, Ethernet13, label imp-null(3)
                 backup via 20.30.221.221, Ethernet15, label 721303 21181
 B I      50.128.120.0/24 [200/0]
           via 10.0.0.120/32, algorithm MIN-LATENCY, IS-IS FlexAlgo tunnel index 44, label 1272
              via TI-LFA tunnel index 45, label 21248
                 via 20.30.120.120, Ethernet3, label imp-null(3)
                 backup via 20.30.221.221, Ethernet15, label 721303
 B I      50.128.156.0/24 [200/0]
           via 10.0.0.156/32, algorithm MIN-LATENCY, IS-IS FlexAlgo tunnel index 27, label 21
              via TI-LFA tunnel index 50, label imp-null(3)
                 via 20.30.156.156, Ethernet11, label imp-null(3)
                 backup via 20.30.221.221, Ethernet15, label 721303 21284
 B I      50.128.179.0/24 [200/0]
           via 10.0.0.179/32, algorithm MIN-LATENCY, IS-IS FlexAlgo tunnel index 40, label 21
              via TI-LFA tunnel index 46, label imp-null(3)
                 via 20.30.179.179, Ethernet40, label imp-null(3)
                 backup via 20.30.221.221, Ethernet15, label 721303 21307
 B I      50.128.184.0/24 [200/0]
           via 10.0.0.184/32, algorithm MIN-LATENCY, IS-IS FlexAlgo tunnel index 37, label 16
              via 20.30.184.184, Ethernet7, label imp-null(3)
 B I      50.128.217.0/24 [200/0]
           via 10.0.0.217/32, algorithm MIN-LATENCY, IS-IS FlexAlgo tunnel index 4, label 524284
              via TI-LFA tunnel index 52, label 21345
                 via 20.30.217.217, Ethernet4, label imp-null(3)
                 backup via 20.30.221.221, Ethernet15, label 721303
 B I      50.128.221.0/24 [200/0]
           via 10.0.0.221/32, algorithm MIN-LATENCY, IS-IS FlexAlgo tunnel index 5, label 524291
              via TI-LFA tunnel index 15, label imp-null(3)
                 via 20.30.221.221, Ethernet15, label imp-null(3)
                 backup via 20.30.156.156, Ethernet11, label 17 21349
 B I      50.129.32.0/24 [200/0]
           via 10.0.0.32/32, algorithm MIN-TE, IS-IS FlexAlgo tunnel index 14, label 378530
              via TI-LFA tunnel index 44, label imp-null(3)
                 via 20.30.32.32, Ethernet2, label imp-null(3)
                 backup via 20.30.53.53, Ethernet13, label 21162
 B I      50.129.53.0/24 [200/0]
           via 10.0.0.53/32, algorithm MIN-TE, IS-IS FlexAlgo tunnel index 11, label 970000
              via TI-LFA tunnel index 17, label imp-null(3)
                 via 20.30.53.53, Ethernet13, label imp-null(3)
                 backup via 20.30.120.120, Ethernet3, label 21182
 B I      50.129.120.0/24 [200/0]
           via 10.0.0.120/32, algorithm MIN-TE, IS-IS FlexAlgo tunnel index 45, label 1274
              via TI-LFA tunnel index 48, label 21249
                 via 20.30.120.120, Ethernet3, label imp-null(3)
                 backup via 20.30.53.53, Ethernet13, label imp-null(3)
 B I      50.129.156.0/24 [200/0]
           via 10.0.0.156/32, algorithm MIN-TE, IS-IS FlexAlgo tunnel index 26, label 21
              via TI-LFA tunnel index 40, label imp-null(3)
                 via 20.30.156.156, Ethernet11, label imp-null(3)
                 backup via 20.30.53.53, Ethernet13, label 21285
 B I      50.129.179.0/24 [200/0]
           via 10.0.0.179/32, algorithm MIN-TE, IS-IS FlexAlgo tunnel index 38, label 21
              via TI-LFA tunnel index 28, label imp-null(3)
                 via 20.30.179.179, Ethernet40, label imp-null(3)
                 backup via 20.30.53.53, Ethernet13, label 21308
 B I      50.129.184.0/24 [200/0]
           via 10.0.0.184/32, algorithm MIN-TE, IS-IS FlexAlgo tunnel index 36, label 17
              via 20.30.184.184, Ethernet7, label imp-null(3)
 B I      50.129.217.0/24 [200/0]
           via 10.0.0.217/32, algorithm MIN-TE, IS-IS FlexAlgo tunnel index 13, label 524284
              via TI-LFA tunnel index 35, label 21346
                 via 20.30.217.217, Ethernet4, label imp-null(3)
                 backup via 20.30.53.53, Ethernet13, label imp-null(3)
 B I      50.129.221.0/24 [200/0]
           via 10.0.0.221/32, algorithm MIN-TE, IS-IS FlexAlgo tunnel index 15, label 524291
              via TI-LFA tunnel index 54, label imp-null(3)
                 via 20.30.221.221, Ethernet15, label imp-null(3)
                 backup via 20.30.53.53, Ethernet13, label 21350
 B I      50.130.32.0/24 [200/0]
           via 10.0.0.32/32, IS-IS SR tunnel index 9, label 378530
              via TI-LFA tunnel index 5, label imp-null(3)
                 via 20.30.32.32, Ethernet2, label imp-null(3)
                 backup via 20.30.156.156, Ethernet11, label 20032
 B I      50.130.53.0/24 [200/0]
           via 10.0.0.53/32, IS-IS SR tunnel index 5, label 970000
              via TI-LFA tunnel index 10, label imp-null(3)
                 via 20.30.53.53, Ethernet13, label exp-null-v4(0)
                 backup via 20.30.179.179, Ethernet40, label 20053
 B I      50.130.120.0/24 [200/0]
           via 10.0.0.120/32, IS-IS SR tunnel index 7, label 1273
              via TI-LFA tunnel index 0, label imp-null(3)
                 via 20.30.120.120, Ethernet3, label imp-null(3)
                 backup via 20.30.156.156, Ethernet11, label 20120
 B I      50.130.156.0/24 [200/0]
           via 10.0.0.156/32, IS-IS SR tunnel index 18, label 21
              via TI-LFA tunnel index 11, label imp-null(3)
                 via 20.30.156.156, Ethernet11, label imp-null(3)
                 backup via 20.30.179.179, Ethernet40, label 20156
 B I      50.130.179.0/24 [200/0]
           via 10.0.0.179/32, IS-IS SR tunnel index 6, label 21
              via TI-LFA tunnel index 7, label imp-null(3)
                 via 20.30.179.179, Ethernet40, label imp-null(3)
                 backup via 20.30.156.156, Ethernet11, label 20179
 B I      50.130.184.0/24 [200/0]
           via 10.0.0.184/32, IS-IS SR tunnel index 15, label 18
              via 20.30.184.184, Ethernet7, label imp-null(3)
 B I      50.130.217.0/24 [200/0]
           via 10.0.0.217/32, IS-IS SR tunnel index 16, label 524284
              via TI-LFA tunnel index 4, label 20217
                 via 20.30.217.217, Ethernet4, label imp-null(3)
                 backup via 20.30.156.156, Ethernet11, label imp-null(3)
 B I      50.130.221.0/24 [200/0]
           via 10.0.0.221/32, IS-IS SR tunnel index 13, label 524291
              via TI-LFA tunnel index 13, label imp-null(3)
                 via 20.30.221.221, Ethernet15, label imp-null(3)
                 backup via 20.30.179.179, Ethernet40, label 20221

```

## show mpls route

```text
MPLS forwarding table (Label [metric] Vias) - 54 routes 
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
                  via TI-LFA tunnel index 5
                    via 20.30.32.32, Ethernet2, label imp-null(3)
                    backup via 20.30.156.156, Ethernet11, label 20032
 20053   A[1]
                via M, ::, pop
                    EgressACL: apply
                  via TI-LFA tunnel index 10
                    via 20.30.53.53, Ethernet13, label exp-null-v4(0)
                    backup via 20.30.179.179, Ethernet40, label 20053
 20084   A[1]
                via M, ::, forward
                    EgressACL: apply
                  via TI-LFA tunnel index 6
                    via 20.30.84.84, Ethernet12, label imp-null(3)
                    backup via 20.30.156.156, Ethernet11, label imp-null(3)
 20120   A[1]
                via M, ::, pop
                    EgressACL: apply
                  via TI-LFA tunnel index 0
                    via 20.30.120.120, Ethernet3, label imp-null(3)
                    backup via 20.30.156.156, Ethernet11, label 20120
 20124   A[1]
                via M, ::, pop
                    EgressACL: apply
                  via TI-LFA tunnel index 8
                    via 20.30.124.124, Ethernet17, label 2124
                    backup via 20.30.179.179, Ethernet40, label 20124
 20128   A[1]
                via M, ::, pop
                    EgressACL: apply
                  via TI-LFA tunnel index 29
                    via 20.30.128.128, Ethernet19, label imp-null(3)
                    backup via 20.30.156.156, Ethernet11, label 20128
 20131   A[1]
                via M, ::, pop
                    EgressACL: apply
                  via TI-LFA tunnel index 1
                    via 20.30.131.131, Ethernet35, label imp-null(3)
                    backup via 20.30.156.156, Ethernet11, label 20131
 20156   A[1]
                via M, ::, pop
                    EgressACL: apply
                  via TI-LFA tunnel index 11
                    via 20.30.156.156, Ethernet11, label imp-null(3)
                    backup via 20.30.179.179, Ethernet40, label 20156
 20175   A[1]
                via M, 20.30.32.32, swap 20175
                    EgressACL: apply
                    directly connected, Ethernet2
                    d4:af:f7:2f:13:96, vlan 1007
                via M, 20.30.53.53, swap 20175
                    EgressACL: apply
                    directly connected, Ethernet13
                    5c:07:58:a3:0a:aa, vlan 1014
                via M, 20.30.84.84, swap 20175
                    EgressACL: apply
                    directly connected, Ethernet12
                    58:70:7f:9f:c4:03, vlan 1013
                via M, 20.30.120.120, swap 20175
                    EgressACL: apply
                    directly connected, Ethernet3
                    bc:31:e2:e1:ec:2c, vlan 1008
                via M, 20.30.124.124, swap 2175
                    EgressACL: apply
                    directly connected, Ethernet17
                    64:6d:4e:32:e1:22, vlan 1016
                via M, 20.30.128.128, swap 20175
                    EgressACL: apply
                    directly connected, Ethernet19
                    60:53:75:13:ba:d8, vlan 1018
                via M, 20.30.131.131, swap 20175
                    EgressACL: apply
                    directly connected, Ethernet35
                    40:a6:b7:94:34:cb, vlan 1022
                via M, 20.30.156.156, swap 20175
                    EgressACL: apply
                    directly connected, Ethernet11
                    d0:48:a1:ba:3c:61, vlan 1021
 20179   A[1]
                via M, ::, pop
                    EgressACL: apply
                  via TI-LFA tunnel index 7
                    via 20.30.179.179, Ethernet40, label imp-null(3)
                    backup via 20.30.156.156, Ethernet11, label 20179
 20184   A[1]
                via M, pop
                    EgressACL: apply
                    20.30.184.184 Ethernet7
 20214   A[1]
                via M, ::, forward
                    EgressACL: apply
                  via TI-LFA tunnel index 12
                    via 20.30.214.214, Ethernet5, label imp-null(3)
                    backup via 20.30.156.156, Ethernet11, label imp-null(3)
 20217   A[1]
                via M, ::, forward
                    EgressACL: apply
                  via TI-LFA tunnel index 4
                    via 20.30.217.217, Ethernet4, label imp-null(3)
                    backup via 20.30.156.156, Ethernet11, label imp-null(3)
 20221   A[1]
                via M, ::, pop
                    EgressACL: apply
                  via TI-LFA tunnel index 13
                    via 20.30.221.221, Ethernet15, label imp-null(3)
                    backup via 20.30.179.179, Ethernet40, label 20221
 21161   A[1]
                via M, ::, pop
                    EgressACL: apply
                  via TI-LFA tunnel index 53
                    via 20.30.32.32, Ethernet2, label imp-null(3)
                    backup via 20.30.221.221, Ethernet15, label 721303 21161
 21162   A[1]
                via M, ::, pop
                    EgressACL: apply
                  via TI-LFA tunnel index 44
                    via 20.30.32.32, Ethernet2, label imp-null(3)
                    backup via 20.30.53.53, Ethernet13, label 21162
 21181   A[1]
                via M, ::, pop
                    EgressACL: apply
                  via TI-LFA tunnel index 47
                    via 20.30.53.53, Ethernet13, label imp-null(3)
                    backup via 20.30.221.221, Ethernet15, label 721303 21181
 21182   A[1]
                via M, ::, pop
                    EgressACL: apply
                  via TI-LFA tunnel index 17
                    via 20.30.53.53, Ethernet13, label imp-null(3)
                    backup via 20.30.120.120, Ethernet3, label 21182
 21248   A[1]
                via M, ::, forward
                    EgressACL: apply
                  via TI-LFA tunnel index 45
                    via 20.30.120.120, Ethernet3, label imp-null(3)
                    backup via 20.30.221.221, Ethernet15, label 721303
 21249   A[1]
                via M, ::, forward
                    EgressACL: apply
                  via TI-LFA tunnel index 48
                    via 20.30.120.120, Ethernet3, label imp-null(3)
                    backup via 20.30.53.53, Ethernet13, label imp-null(3)
 21252   A[1]
                via M, ::, pop
                    EgressACL: apply
                  via TI-LFA tunnel index 51
                    via 20.30.124.124, Ethernet17, label 3252
                    backup via 20.30.221.221, Ethernet15, label 721303 21252
 21253   A[1]
                via M, ::, pop
                    EgressACL: apply
                  via TI-LFA tunnel index 56
                    via 20.30.124.124, Ethernet17, label 3253
                    backup via 20.30.53.53, Ethernet13, label 21253
 21256   A[1]
                via M, ::, pop
                    EgressACL: apply
                  via TI-LFA tunnel index 49
                    via 20.30.128.128, Ethernet19, label imp-null(3)
                    backup via 20.30.221.221, Ethernet15, label 721303 21256
 21257   A[1]
                via M, ::, pop
                    EgressACL: apply
                  via TI-LFA tunnel index 41
                    via 20.30.128.128, Ethernet19, label imp-null(3)
                    backup via 20.30.53.53, Ethernet13, label 21257
 21284   A[1]
                via M, ::, pop
                    EgressACL: apply
                  via TI-LFA tunnel index 50
                    via 20.30.156.156, Ethernet11, label imp-null(3)
                    backup via 20.30.221.221, Ethernet15, label 721303 21284
 21285   A[1]
                via M, ::, pop
                    EgressACL: apply
                  via TI-LFA tunnel index 40
                    via 20.30.156.156, Ethernet11, label imp-null(3)
                    backup via 20.30.53.53, Ethernet13, label 21285
 21303   A[1]
                via M, ::, pop
                    EgressACL: apply
                  via TI-LFA tunnel index 20
                    via 20.30.221.221, Ethernet15, label 721303
                    backup via 20.30.179.179, Ethernet40, label 19
 21304   A[1]
                via M, 20.30.53.53, swap 21304
                    EgressACL: apply
                    directly connected, Ethernet13
                    5c:07:58:a3:0a:aa, vlan 1014
                via M, 20.30.120.120, swap 21304
                    EgressACL: apply
                    directly connected, Ethernet3
                    bc:31:e2:e1:ec:2c, vlan 1008
                via M, 20.30.124.124, swap 3304
                    EgressACL: apply
                    directly connected, Ethernet17
                    64:6d:4e:32:e1:22, vlan 1016
                via M, 20.30.128.128, swap 21304
                    EgressACL: apply
                    directly connected, Ethernet19
                    60:53:75:13:ba:d8, vlan 1018
                via M, 20.30.156.156, swap 21304
                    EgressACL: apply
                    directly connected, Ethernet11
                    d0:48:a1:ba:3c:61, vlan 1021
                via M, 20.30.179.179, swap 21304
                    EgressACL: apply
                    directly connected, Ethernet40
                    e8:24:a6:96:05:48, vlan 1020
                via M, 20.30.217.217, swap 21304
                    EgressACL: apply
                    directly connected, Ethernet4
                    c0:14:b8:21:97:90, vlan 1009
                via M, 20.30.221.221, swap 721304
                    EgressACL: apply
                    directly connected, Ethernet15
                    30:c5:07:84:3e:79, vlan 1015
 21307   A[1]
                via M, ::, pop
                    EgressACL: apply
                  via TI-LFA tunnel index 46
                    via 20.30.179.179, Ethernet40, label imp-null(3)
                    backup via 20.30.221.221, Ethernet15, label 721303 21307
 21308   A[1]
                via M, ::, pop
                    EgressACL: apply
                  via TI-LFA tunnel index 28
                    via 20.30.179.179, Ethernet40, label imp-null(3)
                    backup via 20.30.53.53, Ethernet13, label 21308
 21312   A[1]
                via M, pop
                    EgressACL: apply
                    20.30.184.184 Ethernet7
 21313   A[1]
                via M, pop
                    EgressACL: apply
                    20.30.184.184 Ethernet7
 21345   A[1]
                via M, ::, forward
                    EgressACL: apply
                  via TI-LFA tunnel index 52
                    via 20.30.217.217, Ethernet4, label imp-null(3)
                    backup via 20.30.221.221, Ethernet15, label 721303
 21346   A[1]
                via M, ::, forward
                    EgressACL: apply
                  via TI-LFA tunnel index 35
                    via 20.30.217.217, Ethernet4, label imp-null(3)
                    backup via 20.30.53.53, Ethernet13, label imp-null(3)
 21349   A[1]
                via M, ::, pop
                    EgressACL: apply
                  via TI-LFA tunnel index 15
                    via 20.30.221.221, Ethernet15, label imp-null(3)
                    backup via 20.30.156.156, Ethernet11, label 17 21349
 21350   A[1]
                via M, ::, pop
                    EgressACL: apply
                  via TI-LFA tunnel index 54
                    via 20.30.221.221, Ethernet15, label imp-null(3)
                    backup via 20.30.53.53, Ethernet13, label 21350
 362188  A[1]
                via M, 20.30.120.120, pop
                    EgressACL: apply
                    directly connected, Ethernet3
                    bc:31:e2:e1:ec:2c, vlan 1008
 362189  A[1]
                via M, fe80::be31:e2ff:fee1:ec2c, pop
                    EgressACL: apply
                    directly connected, Ethernet3
                    bc:31:e2:e1:ec:2c, vlan 1008
 362190  A[1]
                via M, 20.30.32.32, pop
                    EgressACL: apply
                    directly connected, Ethernet2
                    d4:af:f7:2f:13:96, vlan 1007
 362191  A[1]
                via M, 20.30.214.214, pop
                    EgressACL: apply
                    directly connected, Ethernet5
                    18:5b:00:61:ac:6f, vlan 1010
 362192  A[1]
                via M, 20.30.124.124, pop
                    EgressACL: apply
                    directly connected, Ethernet17
                    64:6d:4e:32:e1:22, vlan 1016
 362193  A[1]
                via M, 20.30.53.53, pop
                    EgressACL: apply
                    directly connected, Ethernet13
                    5c:07:58:a3:0a:aa, vlan 1014
 362194  A[1]
                via M, 20.30.128.128, pop
                    EgressACL: apply
                    directly connected, Ethernet19
                    60:53:75:13:ba:d8, vlan 1018
 362196  A[1]
                via M, 20.30.217.217, pop
                    EgressACL: apply
                    directly connected, Ethernet4
                    c0:14:b8:21:97:90, vlan 1009
 362197  A[1]
                via M, 20.30.221.221, pop
                    EgressACL: apply
                    directly connected, Ethernet15
                    30:c5:07:84:3e:79, vlan 1015
 362198  A[1]
                via M, fe80::d6af:f7ff:fe2f:1396, pop
                    EgressACL: apply
                    directly connected, Ethernet2
                    d4:af:f7:2f:13:96, vlan 1007
 362199  A[1]
                via M, 20.30.84.84, pop
                    EgressACL: apply
                    directly connected, Ethernet12
                    58:70:7f:9f:c4:03, vlan 1013
 362200  A[1]
                via M, fe80::5a70:7fff:fe9f:c403, pop
                    EgressACL: apply
                    directly connected, Ethernet12
                    58:70:7f:9f:c4:03, vlan 1013
 362201  A[1]
                via M, 20.30.179.179, pop
                    EgressACL: apply
                    directly connected, Ethernet40
                    e8:24:a6:96:05:48, vlan 1020
 362202  A[1]
                via M, 20.30.156.156, pop
                    EgressACL: apply
                    directly connected, Ethernet11
                    d0:48:a1:ba:3c:61, vlan 1021
 362208  A[1]
                via M, 20.30.184.184, pop
                    EgressACL: apply
                    directly connected, Ethernet7
                    00:2c:01:00:00:01, vlan 1011
 362209  A[1]
                via M, 20.30.131.131, pop
                    EgressACL: apply
                    directly connected, Ethernet35
                    40:a6:b7:94:34:cb, vlan 1022
 378528   [0]
                via I, ipv4, vrf RED
 378529   [0]
                via I, ipv4, vrf FLEXALGO
```

## show mpls lfib route

```text
MPLS forwarding table (Label [metric] Vias) - 54 routes 
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
                via TI-LFA tunnel index 5, pop
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                    via 20.30.32.32, Ethernet2, label imp-null(3)
                    backup via 20.30.156.156, Ethernet11, label 20032
 IP    20053    [1], 10.0.0.53/32
                via TI-LFA tunnel index 10, pop
                 payload autoDecide, ttlMode uniform, apply egress-acl
                    via 20.30.53.53, Ethernet13, label exp-null-v4(0)
                    backup via 20.30.179.179, Ethernet40, label 20053
 IP    20084    [1], 10.0.0.84/32
                via TI-LFA tunnel index 6, forward
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                    via 20.30.84.84, Ethernet12, label imp-null(3)
                    backup via 20.30.156.156, Ethernet11, label imp-null(3)
 IP    20120    [1], 10.0.0.120/32
                via TI-LFA tunnel index 0, pop
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                    via 20.30.120.120, Ethernet3, label imp-null(3)
                    backup via 20.30.156.156, Ethernet11, label 20120
 IP    20124    [1], 10.0.0.124/32
                via TI-LFA tunnel index 8, pop
                 payload autoDecide, ttlMode uniform, apply egress-acl
                    via 20.30.124.124, Ethernet17, label 2124
                    backup via 20.30.179.179, Ethernet40, label 20124
 IP    20128    [1], 10.0.0.128/32
                via TI-LFA tunnel index 29, pop
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                    via 20.30.128.128, Ethernet19, label imp-null(3)
                    backup via 20.30.156.156, Ethernet11, label 20128
 IP    20131    [1], 10.0.0.131/32
                via TI-LFA tunnel index 1, pop
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                    via 20.30.131.131, Ethernet35, label imp-null(3)
                    backup via 20.30.156.156, Ethernet11, label 20131
 IP    20156    [1], 10.0.0.156/32
                via TI-LFA tunnel index 11, pop
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                    via 20.30.156.156, Ethernet11, label imp-null(3)
                    backup via 20.30.179.179, Ethernet40, label 20156
 IP    20175    [1], 10.0.0.175/32
                via M, 20.30.32.32, swap 20175
                 payload autoDecide, ttlMode uniform, apply egress-acl
                 interface Ethernet2
                via M, 20.30.53.53, swap 20175
                 payload autoDecide, ttlMode uniform, apply egress-acl
                 interface Ethernet13
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
                via M, 20.30.131.131, swap 20175
                 payload autoDecide, ttlMode uniform, apply egress-acl
                 interface Ethernet35
                via M, 20.30.156.156, swap 20175
                 payload autoDecide, ttlMode uniform, apply egress-acl
                 interface Ethernet11
 IP    20179    [1], 10.0.0.179/32
                via TI-LFA tunnel index 7, pop
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                    via 20.30.179.179, Ethernet40, label imp-null(3)
                    backup via 20.30.156.156, Ethernet11, label 20179
 IP    20184    [1], 10.0.0.184/32
                via M, 20.30.184.184, pop
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                 interface Ethernet7
 IP    20214    [1], 10.0.0.214/32
                via TI-LFA tunnel index 12, forward
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                    via 20.30.214.214, Ethernet5, label imp-null(3)
                    backup via 20.30.156.156, Ethernet11, label imp-null(3)
 IP    20217    [1], 10.0.0.217/32
                via TI-LFA tunnel index 4, forward
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                    via 20.30.217.217, Ethernet4, label imp-null(3)
                    backup via 20.30.156.156, Ethernet11, label imp-null(3)
 IP    20221    [1], 10.0.0.221/32
                via TI-LFA tunnel index 13, pop
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                    via 20.30.221.221, Ethernet15, label imp-null(3)
                    backup via 20.30.179.179, Ethernet40, label 20221
 IP    21161    [1], 10.0.0.32/32, algorithm MIN-LATENCY
                via TI-LFA tunnel index 53, pop
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                    via 20.30.32.32, Ethernet2, label imp-null(3)
                    backup via 20.30.221.221, Ethernet15, label 721303 21161
 IP    21162    [1], 10.0.0.32/32, algorithm MIN-TE
                via TI-LFA tunnel index 44, pop
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                    via 20.30.32.32, Ethernet2, label imp-null(3)
                    backup via 20.30.53.53, Ethernet13, label 21162
 IP    21181    [1], 10.0.0.53/32, algorithm MIN-LATENCY
                via TI-LFA tunnel index 47, pop
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                    via 20.30.53.53, Ethernet13, label imp-null(3)
                    backup via 20.30.221.221, Ethernet15, label 721303 21181
 IP    21182    [1], 10.0.0.53/32, algorithm MIN-TE
                via TI-LFA tunnel index 17, pop
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                    via 20.30.53.53, Ethernet13, label imp-null(3)
                    backup via 20.30.120.120, Ethernet3, label 21182
 IP    21248    [1], 10.0.0.120/32, algorithm MIN-LATENCY
                via TI-LFA tunnel index 45, forward
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                    via 20.30.120.120, Ethernet3, label imp-null(3)
                    backup via 20.30.221.221, Ethernet15, label 721303
 IP    21249    [1], 10.0.0.120/32, algorithm MIN-TE
                via TI-LFA tunnel index 48, forward
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                    via 20.30.120.120, Ethernet3, label imp-null(3)
                    backup via 20.30.53.53, Ethernet13, label imp-null(3)
 IP    21252    [1], 10.0.0.124/32, algorithm MIN-LATENCY
                via TI-LFA tunnel index 51, pop
                 payload autoDecide, ttlMode uniform, apply egress-acl
                    via 20.30.124.124, Ethernet17, label 3252
                    backup via 20.30.221.221, Ethernet15, label 721303 21252
 IP    21253    [1], 10.0.0.124/32, algorithm MIN-TE
                via TI-LFA tunnel index 56, pop
                 payload autoDecide, ttlMode uniform, apply egress-acl
                    via 20.30.124.124, Ethernet17, label 3253
                    backup via 20.30.53.53, Ethernet13, label 21253
 IP    21256    [1], 10.0.0.128/32, algorithm MIN-LATENCY
                via TI-LFA tunnel index 49, pop
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                    via 20.30.128.128, Ethernet19, label imp-null(3)
                    backup via 20.30.221.221, Ethernet15, label 721303 21256
 IP    21257    [1], 10.0.0.128/32, algorithm MIN-TE
                via TI-LFA tunnel index 41, pop
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                    via 20.30.128.128, Ethernet19, label imp-null(3)
                    backup via 20.30.53.53, Ethernet13, label 21257
 IP    21284    [1], 10.0.0.156/32, algorithm MIN-LATENCY
                via TI-LFA tunnel index 50, pop
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                    via 20.30.156.156, Ethernet11, label imp-null(3)
                    backup via 20.30.221.221, Ethernet15, label 721303 21284
 IP    21285    [1], 10.0.0.156/32, algorithm MIN-TE
                via TI-LFA tunnel index 40, pop
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                    via 20.30.156.156, Ethernet11, label imp-null(3)
                    backup via 20.30.53.53, Ethernet13, label 21285
 IP    21303    [1], 10.0.0.175/32, algorithm MIN-LATENCY
                via TI-LFA tunnel index 20, pop
                 payload autoDecide, ttlMode uniform, apply egress-acl
                    via 20.30.221.221, Ethernet15, label 721303
                    backup via 20.30.179.179, Ethernet40, label 19
 IP    21304    [1], 10.0.0.175/32, algorithm MIN-TE
                via M, 20.30.53.53, swap 21304
                 payload autoDecide, ttlMode uniform, apply egress-acl
                 interface Ethernet13
                via M, 20.30.120.120, swap 21304
                 payload autoDecide, ttlMode uniform, apply egress-acl
                 interface Ethernet3
                via M, 20.30.124.124, swap 3304
                 payload autoDecide, ttlMode uniform, apply egress-acl
                 interface Ethernet17
                via M, 20.30.128.128, swap 21304
                 payload autoDecide, ttlMode uniform, apply egress-acl
                 interface Ethernet19
                via M, 20.30.156.156, swap 21304
                 payload autoDecide, ttlMode uniform, apply egress-acl
                 interface Ethernet11
                via M, 20.30.179.179, swap 21304
                 payload autoDecide, ttlMode uniform, apply egress-acl
                 interface Ethernet40
                via M, 20.30.217.217, swap 21304
                 payload autoDecide, ttlMode uniform, apply egress-acl
                 interface Ethernet4
                via M, 20.30.221.221, swap 721304
                 payload autoDecide, ttlMode uniform, apply egress-acl
                 interface Ethernet15
 IP    21307    [1], 10.0.0.179/32, algorithm MIN-LATENCY
                via TI-LFA tunnel index 46, pop
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                    via 20.30.179.179, Ethernet40, label imp-null(3)
                    backup via 20.30.221.221, Ethernet15, label 721303 21307
 IP    21308    [1], 10.0.0.179/32, algorithm MIN-TE
                via TI-LFA tunnel index 28, pop
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                    via 20.30.179.179, Ethernet40, label imp-null(3)
                    backup via 20.30.53.53, Ethernet13, label 21308
 IP    21312    [1], 10.0.0.184/32, algorithm MIN-LATENCY
                via M, 20.30.184.184, pop
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                 interface Ethernet7
 IP    21313    [1], 10.0.0.184/32, algorithm MIN-TE
                via M, 20.30.184.184, pop
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                 interface Ethernet7
 IP    21345    [1], 10.0.0.217/32, algorithm MIN-LATENCY
                via TI-LFA tunnel index 52, forward
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                    via 20.30.217.217, Ethernet4, label imp-null(3)
                    backup via 20.30.221.221, Ethernet15, label 721303
 IP    21346    [1], 10.0.0.217/32, algorithm MIN-TE
                via TI-LFA tunnel index 35, forward
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                    via 20.30.217.217, Ethernet4, label imp-null(3)
                    backup via 20.30.53.53, Ethernet13, label imp-null(3)
 IP    21349    [1], 10.0.0.221/32, algorithm MIN-LATENCY
                via TI-LFA tunnel index 15, pop
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                    via 20.30.221.221, Ethernet15, label imp-null(3)
                    backup via 20.30.156.156, Ethernet11, label 17 21349
 IP    21350    [1], 10.0.0.221/32, algorithm MIN-TE
                via TI-LFA tunnel index 54, pop
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                    via 20.30.221.221, Ethernet15, label imp-null(3)
                    backup via 20.30.53.53, Ethernet13, label 21350
 IA    362188   [1]
                via M, 20.30.120.120, pop
                 payload autoDecide, ttlMode uniform, apply egress-acl
                 interface Ethernet3
 IA    362189   [1]
                via M, fe80::be31:e2ff:fee1:ec2c, pop
                 payload autoDecide, ttlMode uniform, apply egress-acl
                 interface Ethernet3
 IA    362190   [1]
                via M, 20.30.32.32, pop
                 payload autoDecide, ttlMode uniform, apply egress-acl
                 interface Ethernet2
 IA    362191   [1]
                via M, 20.30.214.214, pop
                 payload autoDecide, ttlMode uniform, apply egress-acl
                 interface Ethernet5
 IA    362192   [1]
                via M, 20.30.124.124, pop
                 payload autoDecide, ttlMode uniform, apply egress-acl
                 interface Ethernet17
 IA    362193   [1]
                via M, 20.30.53.53, pop
                 payload autoDecide, ttlMode uniform, apply egress-acl
                 interface Ethernet13
 IA    362194   [1]
                via M, 20.30.128.128, pop
                 payload autoDecide, ttlMode uniform, apply egress-acl
                 interface Ethernet19
 IA    362196   [1]
                via M, 20.30.217.217, pop
                 payload autoDecide, ttlMode uniform, apply egress-acl
                 interface Ethernet4
 IA    362197   [1]
                via M, 20.30.221.221, pop
                 payload autoDecide, ttlMode uniform, apply egress-acl
                 interface Ethernet15
 IA    362198   [1]
                via M, fe80::d6af:f7ff:fe2f:1396, pop
                 payload autoDecide, ttlMode uniform, apply egress-acl
                 interface Ethernet2
 IA    362199   [1]
                via M, 20.30.84.84, pop
                 payload autoDecide, ttlMode uniform, apply egress-acl
                 interface Ethernet12
 IA    362200   [1]
                via M, fe80::5a70:7fff:fe9f:c403, pop
                 payload autoDecide, ttlMode uniform, apply egress-acl
                 interface Ethernet12
 IA    362201   [1]
                via M, 20.30.179.179, pop
                 payload autoDecide, ttlMode uniform, apply egress-acl
                 interface Ethernet40
 IA    362202   [1]
                via M, 20.30.156.156, pop
                 payload autoDecide, ttlMode uniform, apply egress-acl
                 interface Ethernet11
 IA    362208   [1]
                via M, 20.30.184.184, pop
                 payload autoDecide, ttlMode uniform, apply egress-acl
                 interface Ethernet7
 IA    362209   [1]
                via M, 20.30.131.131, pop
                 payload autoDecide, ttlMode uniform, apply egress-acl
                 interface Ethernet35
 B3    378528   [0]
                via I, ipv4, vrf RED
 B3    378529   [0]
                via I, ipv4, vrf FLEXALGO
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
 * >      RD: 10.0.0.32:5001 IPv4 prefix 50.10.32.0/24
                                 10.0.0.32             -       100     0       i
 * >      RD: 84:5001 IPv4 prefix 50.10.84.0/24
                                 10.0.0.84             0       100     0       ?
 * >      RD: 131:5001 IPv4 prefix 50.10.131.0/24
                                 10.0.0.131            -       100     0       i
 * >      RD: 156:5001 IPv4 prefix 50.10.156.0/24
                                 10.0.0.156            -       100     0       i
 * >      RD: 179:5001 IPv4 prefix 50.10.179.0/24
                                 10.0.0.179            -       100     0       i
 * >      RD: 214:5001 IPv4 prefix 50.10.214.0/24
                                 10.0.0.214            -       100     0       i
 * >      RD: 217:5001 IPv4 prefix 50.10.217.0/24
                                 10.0.0.217            -       100     0       i
 * >      RD: 10.0.0.30:5128 IPv4 prefix 50.128.32.0/24
                                 10.0.0.32             -       100     0       i
 * >      RD: 53:5001 IPv4 prefix 50.128.53.0/24
                                 10.0.0.53             -       100     0       ?
 * >      RD: 120:5128 IPv4 prefix 50.128.120.0/24
                                 10.0.0.120            0       100     0       ?
 * >      RD: 5128:5128 IPv4 prefix 50.128.156.0/24
                                 10.0.0.156            -       100     0       i
 * >      RD: 5128:5128 IPv4 prefix 50.128.179.0/24
                                 10.0.0.179            -       100     0       i
 * >      RD: 184:5001 IPv4 prefix 50.128.184.0/24
                                 10.0.0.184            -       0       0       i
 * >      RD: 217:5128 IPv4 prefix 50.128.217.0/24
                                 10.0.0.217            -       100     0       i
 * >      RD: 221:5128 IPv4 prefix 50.128.221.0/24
                                 10.0.0.221            -       100     0       i
 * >      RD: 10.0.0.30:5128 IPv4 prefix 50.129.32.0/24
                                 10.0.0.32             -       100     0       i
 * >      RD: 53:5001 IPv4 prefix 50.129.53.0/24
                                 10.0.0.53             -       100     0       ?
 * >      RD: 120:5129 IPv4 prefix 50.129.120.0/24
                                 10.0.0.120            0       100     0       ?
 * >      RD: 5128:5128 IPv4 prefix 50.129.156.0/24
                                 10.0.0.156            -       100     0       i
 * >      RD: 5128:5128 IPv4 prefix 50.129.179.0/24
                                 10.0.0.179            -       100     0       i
 * >      RD: 184:5001 IPv4 prefix 50.129.184.0/24
                                 10.0.0.184            -       0       0       i
 * >      RD: 217:5128 IPv4 prefix 50.129.217.0/24
                                 10.0.0.217            -       100     0       i
 * >      RD: 221:5128 IPv4 prefix 50.129.221.0/24
                                 10.0.0.221            -       100     0       i
 * >      RD: 10.0.0.30:5128 IPv4 prefix 50.130.32.0/24
                                 10.0.0.32             -       100     0       i
 * >      RD: 53:5001 IPv4 prefix 50.130.53.0/24
                                 10.0.0.53             -       100     0       ?
 * >      RD: 120:5130 IPv4 prefix 50.130.120.0/24
                                 10.0.0.120            0       100     0       ?
 * >      RD: 5128:5128 IPv4 prefix 50.130.156.0/24
                                 10.0.0.156            -       100     0       i
 * >      RD: 5128:5128 IPv4 prefix 50.130.179.0/24
                                 10.0.0.179            -       100     0       i
 * >      RD: 184:5001 IPv4 prefix 50.130.184.0/24
                                 10.0.0.184            -       0       0       i
 * >      RD: 217:5128 IPv4 prefix 50.130.217.0/24
                                 10.0.0.217            -       100     0       i
 * >      RD: 221:5128 IPv4 prefix 50.130.221.0/24
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
 * >      RD: 10.0.0.32:5001 IPv6 prefix 2600:50:10:32::/64
                                 ::ffff:10.0.0.32      -       100     0       i
 * >      RD: 84:5001 IPv6 prefix 2600:50:10:84::/64
                                 ::ffff:10.0.0.84      0       100     0       ?
 * >      RD: 131:5001 IPv6 prefix 2600:50:10:131::/64
                                 ::ffff:10.0.0.131     -       100     0       i
 * >      RD: 156:5001 IPv6 prefix 2600:50:10:156::/64
                                 ::ffff:10.0.0.156     -       100     0       i
 * >      RD: 179:5001 IPv6 prefix 2600:50:10:179::/64
                                 ::ffff:10.0.0.179     -       100     0       i
 * >      RD: 214:5001 IPv6 prefix 2600:50:10:214::/64
                                 ::ffff:10.0.0.214     -       100     0       i
 * >      RD: 217:5001 IPv6 prefix 2600:50:10:217::/64
                                 ::ffff:10.0.0.217     -       100     0       i
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
  Connect timer is active, time left: 00:02:17
  Connection interval is 148 seconds
  Failed connection attempts is 52
  Idle-restart timer is inactive
  BGP state is Active
  Number of transitions to established: 0
  Last state was Connect
  Last event was TransportError
  Last sent socket-error:Connect (Network is unreachable), Last time 00:00:27, First time 1d07h, Repeats 682
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
  Last read 00:00:26, last write 00:00:51
  Hold time is 180, keepalive interval is 60 seconds
  Configured hold time is 180, keepalive interval is 60 seconds
  Effective minimum hold time is 3 seconds
  Send failure hold time is 0 seconds
  Hold timer is active, time left: 00:02:34
  Keepalive timer is active, time left: 00:00:05
  Connect timer is inactive
  Idle-restart timer is inactive
  BGP state is Established, up for 1d07h
  Number of transitions to established: 1
  Last state was OpenConfirm
  Last event was RecvUpdate
  Last sent socket-error:Connect (Network is unreachable), Last time 1d07h, First time 1d07h, Repeats 10
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
      Received 1d07h
      Number of stale paths removed after graceful restart: 0
      Number of paths received before End-of-RIB: 4
    VPN-IPv6 End-of-RIB received: Yes
      Received 1d07h
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
    Updates:                       478        38
    Keepalives:                   2149      2224
    Enhanced Route Refresh:          0         0
    Begin of Route Refresh:          0         0
    End of Route Refresh:            0         0
    Total messages:               2628      2263
  Prefix Statistics:
                                   Sent      Rcvd     Best Paths     Best ECMP Paths
    IPv4 Unicast:                     0         0              0                   0
    VPN-IPv4:                        27         4              4                   0
    IPv6 Unicast:                     0         0              0                   0
    VPN-IPv6:                         6         1              1                   0
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
  Total Number of TCP retransmissions: 2
  Options:
    Timestamps enabled: yes
    Selective Acknowledgments enabled: yes
    Window Scale enabled: yes
    Explicit Congestion Notification (ECN) enabled: no
  Socket Statistics:
    Window Scale (wscale): 7,7
    Retransmission Timeout (rto): 208.0ms
    Round-trip Time (rtt/rtvar): 4.5ms/1.6ms
    Delayed Ack Timeout (ato): 40.0ms
    Congestion Window (cwnd): 2
    Slow-start Threshold (ssthresh): 7
    TCP Throughput: 5.17 Mbps
    Advertised Recv Window (rcv_space): 14480

BGP neighbor is 10.0.0.53, remote AS 64512, internal link
 Description: Arrcus-53
  BGP version 4, remote router ID 10.0.0.53, VRF default
  Inherits configuration from and member of peer-group IBGP_CLIENT_PEER
  Last read 00:01:00, last write 00:00:10
  Hold time is 180, keepalive interval is 60 seconds
  Configured hold time is 180, keepalive interval is 60 seconds
  Effective minimum hold time is 3 seconds
  Send failure hold time is 0 seconds
  Hold timer is active, time left: 00:02:00
  Keepalive timer is active, time left: 00:00:37
  Connect timer is inactive
  Idle-restart timer is inactive
  BGP state is Established, up for 09:42:59
  Number of transitions to established: 6
  Last state was OpenConfirm
  Last event was RecvRtRefresh
  Last sent notification:Hold Timer Expired Error/None, Last time 09:46:23
  Last rcvd notification:Cease/administrative reset, Last time 1d03h, First time 1d05h, Repeats 2
  Last sent socket-error:Connect (Network is unreachable), Last time 09:43:35, First time 09:46:22, Repeats 7
  Last rcvd socket-error:Connection reset by peer, Last time 1d03h
  Types of communities advertised: standard extended large
  Neighbor is a route reflector client
  Neighbor is using global cluster ID 10.0.0.30
  Neighbor Capabilities:
    Multiprotocol IPv4 with MPLS Labels: received
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
      IPv4 with MPLS Labels is enabled, Forwarding State is preserved
      VPN-IPv4 is enabled, Forwarding State is preserved
      VPN-IPv6 is enabled, Forwarding State is preserved
  Restart timer is inactive
  End of rib timer is inactive
    VPN-IPv4 End-of-RIB received: Yes
      Received 09:42:59
      Number of stale paths removed after graceful restart: 0
      Number of paths received before End-of-RIB: 1
    VPN-IPv6 End-of-RIB received: Yes
      Received 09:42:59
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
    Opens:                766       766
    Notifications:        761         3
    Updates:              546        58
    Keepalives:          2094      1840
    Route Refresh:          0         1
    Total messages:      4167      2668
  Prefix Statistics:
                                   Sent      Rcvd     Best Paths     Best ECMP Paths
    IPv4 Unicast:                     0         0              0                   0
    VPN-IPv4:                        28         3              3                   0
    IPv6 Unicast:                     0         0              0                   0
    VPN-IPv6:                         7         0              0                   0
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
Remote TCP address is 10.0.0.53, remote port is 41721
Local next hop for next hop self:
  VPN-IPv4: 10.0.0.30
  VPN-IPv6: ::ffff:10.0.0.30
TCP Socket Information:
  TCP state is ESTABLISHED
  Recv-Q: 0/32768
  Send-Q: 0/46080
  Outgoing Maximum Segment Size (MSS): 1436
  Total Number of TCP retransmissions: 0
  Options:
    Timestamps enabled: yes
    Selective Acknowledgments enabled: yes
    Window Scale enabled: yes
    Explicit Congestion Notification (ECN) enabled: no
  Socket Statistics:
    Window Scale (wscale): 14,7
    Retransmission Timeout (rto): 204.0ms
    Round-trip Time (rtt/rtvar): 2.3ms/0.7ms
    Delayed Ack Timeout (ato): 44.0ms
    Congestion Window (cwnd): 10
    TCP Throughput: 50.85 Mbps
    Advertised Recv Window (rcv_space): 14600

BGP neighbor is 10.0.0.66, remote AS 64512, internal link
 Description: Ciena-8140-66
  BGP version 4, remote router ID 10.0.0.66, VRF default
  Inherits configuration from and member of peer-group IBGP_CLIENT_PEER
  Last read 00:15:25, last write 00:15:45
  Hold time is 180, keepalive interval is 60 seconds
  Configured hold time is 180, keepalive interval is 60 seconds
  Effective minimum hold time is 3 seconds
  Send failure hold time is 0 seconds
  Hold timer is inactive
  Keepalive timer is inactive
  Connect timer is active, time left: 00:02:40
  Connection interval is 148 seconds
  Failed connection attempts is 13
  Idle-restart timer is inactive
  BGP state is Active
  Number of transitions to established: 6
  Last state was Connect
  Last event was TransportError
  Last sent notification:Hold Timer Expired Error/None, Last time 02:53:02, First time 1d07h, Repeats 2
  Last rcvd notification:Hold Timer Expired Error/None, Last time 00:15:25, First time 00:32:05, Repeats 1
  Last sent socket-error:Connect (Network is unreachable), Last time 00:00:06, First time 00:32:04, Repeats 22
  Last rcvd socket-error:Connection reset by peer, Last time 02:47:30, First time 1d02h, Repeats 2
  Types of communities advertised: standard extended large
  Neighbor is a route reflector client
  Neighbor is using global cluster ID 10.0.0.30
  Neighbor Capabilities:
    Multiprotocol IPv4 Unicast: received
    Multiprotocol VPN-IPv4: advertised and received
    Multiprotocol VPN-IPv6: advertised
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
    Opens:                  9         6
    Notifications:          3         3
    Updates:              390        42
    Keepalives:          1825      1583
    Route Refresh:          0         0
    Total messages:      2227      1634
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
  Last read 00:18:13, last write 00:15:13
  Hold time is 180, keepalive interval is 60 seconds
  Configured hold time is 180, keepalive interval is 60 seconds
  Effective minimum hold time is 3 seconds
  Send failure hold time is 0 seconds
  Hold timer is inactive
  Keepalive timer is inactive
  Connect timer is active, time left: 00:02:35
  Connection interval is 148 seconds
  Failed connection attempts is 13
  Idle-restart timer is inactive
  BGP state is Active
  Number of transitions to established: 4
  Last state was Connect
  Last event was TransportError
  Last sent notification:Hold Timer Expired Error/None, Last time 00:15:13, First time 03:23:54, Repeats 1
  Last rcvd notification:Cease/other configuration change, Last time 03:11:25, First time 03:13:01, Repeats 1
  Last sent socket-error:Connect (Network is unreachable), Last time 00:00:12, First time 00:15:12, Repeats 12
  Last rcvd socket-error:Connection reset by peer, Last time 03:12:55
  Types of communities advertised: standard extended large
  Neighbor is a route reflector client
  Neighbor is using global cluster ID 10.0.0.30
  Neighbor Capabilities:
    Multiprotocol IPv4 Unicast: received
    Multiprotocol VPN-IPv4: advertised and received
    Multiprotocol VPN-IPv6: advertised
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
    Opens:                  5         4
    Notifications:          2         2
    Updates:              537        25
    Keepalives:          2118      1864
    Route Refresh:          0         0
    Total messages:      2662      1895
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
Remote TCP address is 10.0.0.72, remote port is 179

BGP neighbor is 10.0.0.84, remote AS 64512, internal link
 Description: Ericsson_84
  BGP version 4, remote router ID 10.0.0.84, VRF default
  Inherits configuration from and member of peer-group IBGP_CLIENT_PEER
  Last read 00:00:24, last write 00:00:19
  Hold time is 180, keepalive interval is 60 seconds
  Configured hold time is 180, keepalive interval is 60 seconds
  Effective minimum hold time is 3 seconds
  Send failure hold time is 0 seconds
  Hold timer is active, time left: 00:02:36
  Keepalive timer is active, time left: 00:00:25
  Connect timer is inactive
  Idle-restart timer is inactive
  BGP state is Established, up for 05:16:41
  Number of transitions to established: 2
  Last state was OpenConfirm
  Last event was RecvRtRefresh
  Last rcvd socket-error:Connection reset by peer, Last time 05:16:46, First time 05:16:47, Repeats 1
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
    Multiprotocol L2VPN EVPN: received
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
      Restart-State bit: no
      Graceful notification: no
      IPv4 Unicast is enabled, Forwarding State is preserved
      VPN-IPv4 is enabled, Forwarding State is preserved
      IPv6 Unicast is enabled, Forwarding State is preserved
      VPN-IPv6 is enabled, Forwarding State is preserved
      L2VPN EVPN is enabled, Forwarding State is preserved
  Restart timer is inactive
  End of rib timer is inactive
    VPN-IPv4 End-of-RIB received: Yes
      Received 05:16:41
      Number of stale paths removed after graceful restart: 0
      Number of paths received before End-of-RIB: 1
    VPN-IPv6 End-of-RIB received: Yes
      Received 05:16:41
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
    Opens:                           3         2
    Notifications:                   0         0
    Updates:                       552         8
    Keepalives:                   2134      1905
    Enhanced Route Refresh:          0         4
    Begin of Route Refresh:          2         0
    End of Route Refresh:            2         0
    Total messages:               2693      1919
  Prefix Statistics:
                                   Sent      Rcvd     Best Paths     Best ECMP Paths
    IPv4 Unicast:                     0         0              0                   0
    VPN-IPv4:                        30         1              1                   0
    IPv6 Unicast:                     0         0              0                   0
    VPN-IPv6:                         6         1              1                   0
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
Local TCP address is 10.0.0.30, local port is 38973
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
    Retransmission Timeout (rto): 436.0ms
    Round-trip Time (rtt/rtvar): 233.9ms/0.7ms
    Delayed Ack Timeout (ato): 40.0ms
    Congestion Window (cwnd): 10
    TCP Throughput: 0.49 Mbps
    Advertised Recv Window (rcv_space): 14480

BGP neighbor is 10.0.0.120, remote AS 64512, internal link
 Description: Huawei_120
  BGP version 4, remote router ID 10.0.0.120, VRF default
  Inherits configuration from and member of peer-group IBGP_CLIENT_PEER
  Last read 00:00:19, last write 00:00:44
  Hold time is 180, keepalive interval is 60 seconds
  Configured hold time is 180, keepalive interval is 60 seconds
  Effective minimum hold time is 3 seconds
  Send failure hold time is 0 seconds
  Hold timer is active, time left: 00:02:41
  Keepalive timer is inactive
  Connect timer is inactive
  Idle-restart timer is inactive
  BGP state is Established, up for 1d04h
  Number of transitions to established: 3
  Last state was OpenConfirm
  Last event was RecvRtRefresh
  Last rcvd notification:Cease/administrative reset, Last time 1d04h, First time 1d05h, Repeats 1
  Last sent socket-error:Connect (Connection refused), Last time 1d04h, First time 1d07h, Repeats 4
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
    Opens:                  3         3
    Notifications:          0         2
    Updates:              554        62
    Keepalives:          2162      2130
    Route Refresh:          0         6
    Total messages:      2719      2203
  Prefix Statistics:
                                   Sent      Rcvd     Best Paths     Best ECMP Paths
    IPv4 Unicast:                     0         0              0                   0
    VPN-IPv4:                        28         3              3                   0
    IPv6 Unicast:                     0         0              0                   0
    VPN-IPv6:                         7         0              0                   0
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
Remote TCP address is 10.0.0.120, remote port is 32601
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
    Round-trip Time (rtt/rtvar): 3.3ms/0.9ms
    Delayed Ack Timeout (ato): 44.0ms
    Congestion Window (cwnd): 10
    TCP Throughput: 33.91 Mbps
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
  Connect timer is active, time left: 00:02:50
  Connection interval is 148 seconds
  Failed connection attempts is 613
  Idle-restart timer is inactive
  BGP state is Active
  Number of transitions to established: 0
  Last state was Connect
  Last event was TransportError
  Last sent socket-error:Connect (Connection refused), Last time 00:00:04, First time 1d04h, Repeats 622
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
 Description: Juniper-131-JCNR
  BGP version 4, remote router ID 10.0.0.131, VRF default
  Inherits configuration from and member of peer-group IBGP_CLIENT_PEER
  Last read 00:00:05, last write 00:00:07
  Hold time is 90, keepalive interval is 30 seconds
  Configured hold time is 180, keepalive interval is 60 seconds
  Effective minimum hold time is 3 seconds
  Send failure hold time is 0 seconds
  Hold timer is active, time left: 00:01:25
  Keepalive timer is active, time left: 00:00:14
  Connect timer is inactive
  Idle-restart timer is inactive
  BGP state is Established, up for 03:23:37
  Number of transitions to established: 1
  Last state was OpenConfirm
  Last event was RecvKeepAlive
  Last sent socket-error:Connect (Network is unreachable), Last time 03:23:53, First time 1d07h, Repeats 605
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
      Received 03:23:37
      Number of stale paths removed after graceful restart: 0
      Number of paths received before End-of-RIB: 1
    VPN-IPv6 End-of-RIB received: Yes
      Received 03:23:37
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
    Updates:              186         4
    Keepalives:           449       451
    Route Refresh:          0         0
    Total messages:       636       456
  Prefix Statistics:
                                   Sent      Rcvd     Best Paths     Best ECMP Paths
    IPv4 Unicast:                     0         0              0                   0
    VPN-IPv4:                        30         1              1                   0
    IPv6 Unicast:                     0         0              0                   0
    VPN-IPv6:                         6         1              1                   0
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
Local TCP address is 10.0.0.30, local port is 43723
Remote TCP address is 10.0.0.131, remote port is 179
Local next hop for next hop self:
  VPN-IPv4: 10.0.0.30
  VPN-IPv6: ::ffff:10.0.0.30
TCP Socket Information:
  TCP state is ESTABLISHED
  Recv-Q: 0/32768
  Send-Q: 0/46080
  Outgoing Maximum Segment Size (MSS): 1448
  Total Number of TCP retransmissions: 3
  Options:
    Timestamps enabled: yes
    Selective Acknowledgments enabled: yes
    Window Scale enabled: yes
    Explicit Congestion Notification (ECN) enabled: no
  Socket Statistics:
    Window Scale (wscale): 1,7
    Retransmission Timeout (rto): 204.0ms
    Round-trip Time (rtt/rtvar): 2.8ms/0.4ms
    Delayed Ack Timeout (ato): 40.0ms
    Congestion Window (cwnd): 10
    TCP Throughput: 42.12 Mbps
    Advertised Recv Window (rcv_space): 14480

BGP neighbor is 10.0.0.156, remote AS 64512, internal link
 Description: Juniper-156
  BGP version 4, remote router ID 10.0.0.156, VRF default
  Inherits configuration from and member of peer-group IBGP_CLIENT_PEER
  Last read 00:00:03, last write 00:00:08
  Hold time is 90, keepalive interval is 30 seconds
  Configured hold time is 180, keepalive interval is 60 seconds
  Effective minimum hold time is 3 seconds
  Send failure hold time is 0 seconds
  Hold timer is active, time left: 00:01:27
  Keepalive timer is active, time left: 00:00:21
  Connect timer is inactive
  Idle-restart timer is inactive
  BGP state is Established, up for 09:05:44
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
      Received 09:05:43
      Number of stale paths removed after graceful restart: 0
      Number of paths received before End-of-RIB: 1
    VPN-IPv6 End-of-RIB received: Yes
      Received 09:05:43
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
    Updates:              307        10
    Keepalives:          1236      1208
    Route Refresh:          0         4
    Total messages:      1544      1223
  Prefix Statistics:
                                   Sent      Rcvd     Best Paths     Best ECMP Paths
    IPv4 Unicast:                     0         0              0                   0
    VPN-IPv4:                        27         4              4                   0
    IPv6 Unicast:                     0         0              0                   0
    VPN-IPv6:                         6         1              1                   0
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
Local TCP address is 10.0.0.30, local port is 32919
Remote TCP address is 10.0.0.156, remote port is 179
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
    Round-trip Time (rtt/rtvar): 2.4ms/0.2ms
    Delayed Ack Timeout (ato): 40.0ms
    Congestion Window (cwnd): 10
    TCP Throughput: 48.84 Mbps
    Advertised Recv Window (rcv_space): 14480

BGP neighbor is 10.0.0.179, remote AS 64512, internal link
 Description: Juniper-179
  BGP version 4, remote router ID 10.0.0.179, VRF default
  Inherits configuration from and member of peer-group IBGP_CLIENT_PEER
  Last read 00:00:23, last write 00:00:15
  Hold time is 90, keepalive interval is 30 seconds
  Configured hold time is 180, keepalive interval is 60 seconds
  Effective minimum hold time is 3 seconds
  Send failure hold time is 0 seconds
  Hold timer is active, time left: 00:01:07
  Keepalive timer is active, time left: 00:00:08
  Connect timer is inactive
  Idle-restart timer is inactive
  BGP state is Established, up for 1d04h
  Number of transitions to established: 19
  Last state was OpenConfirm
  Last event was RecvUpdate
  Last sent notification:Hold Timer Expired Error/None, Last time 1d04h, First time 1d05h, Repeats 1
  Last rcvd notification:Cease/administrative reset, Last time 1d05h, First time 1d05h, Repeats 4
  Last sent socket-error:Connect (Network is unreachable), Last time 1d04h, First time 1d04h, Repeats 5
  Last rcvd socket-error:Connection reset by peer, Last time 1d04h, First time 1d07h, Repeats 6
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
      Received 1d04h
      Number of stale paths removed after graceful restart: 0
      Number of paths received before End-of-RIB: 1
    VPN-IPv6 End-of-RIB received: Yes
      Received 1d04h
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
    Opens:                 26        25
    Notifications:          2        16
    Updates:              792        87
    Keepalives:          4342      4136
    Route Refresh:          0         6
    Total messages:      5162      4270
  Prefix Statistics:
                                   Sent      Rcvd     Best Paths     Best ECMP Paths
    IPv4 Unicast:                     0         0              0                   0
    VPN-IPv4:                        27         4              4                   0
    IPv6 Unicast:                     0         0              0                   0
    VPN-IPv6:                         6         1              1                   0
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
Local TCP address is 10.0.0.30, local port is 40433
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
    Round-trip Time (rtt/rtvar): 2.7ms/0.3ms
    Delayed Ack Timeout (ato): 40.0ms
    Congestion Window (cwnd): 10
    TCP Throughput: 43.26 Mbps
    Recv Round-trip Time (rcv_rtt): 305373.9ms
    Advertised Recv Window (rcv_space): 64351

BGP neighbor is 10.0.0.184, remote AS 64512, internal link
 Description: IXIA
  BGP version 4, remote router ID 193.0.0.1, VRF default
  Inherits configuration from and member of peer-group IBGP_CLIENT_PEER
  Last read 00:00:16, last write 00:00:27
  Hold time is 90, keepalive interval is 30 seconds
  Configured hold time is 180, keepalive interval is 60 seconds
  Effective minimum hold time is 3 seconds
  Send failure hold time is 0 seconds
  Hold timer is active, time left: 00:01:14
  Keepalive timer is inactive
  Connect timer is inactive
  Idle-restart timer is inactive
  BGP state is Established, up for 01:32:46
  Number of transitions to established: 22
  Last state was OpenConfirm
  Last event was RecvUpdate
  Last sent notification:Hold Timer Expired Error/None, Last time 07:27:12
  Last sent socket-error:Connect (Network is unreachable), Last time 01:32:55, First time 02:00:52, Repeats 13
  Last rcvd socket-error:Connection reset by peer, Last time 01:36:06, First time 1d01h, Repeats 63
  Types of communities advertised: standard extended large
  Neighbor is a route reflector client
  Neighbor is using global cluster ID 10.0.0.30
  Neighbor Capabilities:
    Multiprotocol IPv4 Unicast: received
    Multiprotocol IPv4 Multicast: received
    Multiprotocol VPN-IPv4: advertised and received and negotiated
    Multiprotocol IPv6 Unicast: received
    Multiprotocol IPv6 Multicast: received
    Multiprotocol VPN-IPv6: advertised and received and negotiated
    Multiprotocol L2VPN VPLS: received
    Four Octet ASN: advertised
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
    Opens:                 66        31
    Notifications:          1         0
    Updates:              849       105
    Keepalives:           778       669
    Route Refresh:          0         2
    Total messages:      1694       807
  Prefix Statistics:
                                   Sent      Rcvd     Best Paths     Best ECMP Paths
    IPv4 Unicast:                     0         0              0                   0
    VPN-IPv4:                        28         3              3                   0
    IPv6 Unicast:                     0         0              0                   0
    VPN-IPv6:                         7         0              0                   0
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
Local TCP address is 10.0.0.30, local port is 38437
Remote TCP address is 10.0.0.184, remote port is 179
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
    Window Scale (wscale): 9,7
    Retransmission Timeout (rto): 204.0ms
    Round-trip Time (rtt/rtvar): 2.4ms/0.3ms
    Delayed Ack Timeout (ato): 40.0ms
    Congestion Window (cwnd): 10
    TCP Throughput: 48.17 Mbps
    Advertised Recv Window (rcv_space): 14480

BGP neighbor is 10.0.0.214, remote AS 64512, internal link
 Description: Nokia-SXR-214
  BGP version 4, remote router ID 10.0.0.214, VRF default
  Inherits configuration from and member of peer-group IBGP_CLIENT_PEER
  Last read 00:00:29, last write 00:00:10
  Hold time is 90, keepalive interval is 30 seconds
  Configured hold time is 180, keepalive interval is 60 seconds
  Effective minimum hold time is 3 seconds
  Send failure hold time is 0 seconds
  Hold timer is active, time left: 00:01:01
  Keepalive timer is active, time left: 00:00:18
  Connect timer is inactive
  Idle-restart timer is inactive
  BGP state is Established, up for 1d07h
  Number of transitions to established: 1
  Last state was OpenConfirm
  Last event was RecvRtRefresh
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
      Received 1d07h
      Number of stale paths removed after graceful restart: 0
      Number of paths received before End-of-RIB: 1
    VPN-IPv6 End-of-RIB received: Yes
      Received 1d07h
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
    Updates:              526         6
    Keepalives:          4388      3816
    Route Refresh:          0         2
    Total messages:      4915      3825
  Prefix Statistics:
                                   Sent      Rcvd     Best Paths     Best ECMP Paths
    IPv4 Unicast:                     0         0              0                   0
    VPN-IPv4:                        30         1              1                   0
    IPv6 Unicast:                     0         0              0                   0
    VPN-IPv6:                         6         1              1                   0
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
  Total Number of TCP retransmissions: 4
  Options:
    Timestamps enabled: yes
    Selective Acknowledgments enabled: yes
    Window Scale enabled: yes
    Explicit Congestion Notification (ECN) enabled: no
  Socket Statistics:
    Window Scale (wscale): 0,7
    Retransmission Timeout (rto): 204.0ms
    Round-trip Time (rtt/rtvar): 2.5ms/0.3ms
    Delayed Ack Timeout (ato): 40.0ms
    Congestion Window (cwnd): 4
    Slow-start Threshold (ssthresh): 7
    TCP Throughput: 18.24 Mbps
    Recv Round-trip Time (rcv_rtt): 225323.8ms
    Advertised Recv Window (rcv_space): 64311

BGP neighbor is 10.0.0.217, remote AS 64512, internal link
 Description: Nokia
  BGP version 4, remote router ID 10.0.0.217, VRF default
  Inherits configuration from and member of peer-group IBGP_CLIENT_PEER
  Last read 00:00:29, last write 00:00:11
  Hold time is 90, keepalive interval is 30 seconds
  Configured hold time is 180, keepalive interval is 60 seconds
  Effective minimum hold time is 3 seconds
  Send failure hold time is 0 seconds
  Hold timer is active, time left: 00:01:01
  Keepalive timer is active, time left: 00:00:12
  Connect timer is inactive
  Idle-restart timer is inactive
  BGP state is Established, up for 1d07h
  Number of transitions to established: 1
  Last state was OpenConfirm
  Last event was RecvRtRefresh
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
      Received 1d07h
      Number of stale paths removed after graceful restart: 0
      Number of paths received before End-of-RIB: 1
    VPN-IPv6 End-of-RIB received: Yes
      Received 1d07h
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
    Updates:              599        16
    Keepalives:          4384      3816
    Route Refresh:          0        10
    Total messages:      4984      3843
  Prefix Statistics:
                                   Sent      Rcvd     Best Paths     Best ECMP Paths
    IPv4 Unicast:                     0         0              0                   0
    VPN-IPv4:                        27         4              4                   0
    IPv6 Unicast:                     0         0              0                   0
    VPN-IPv6:                         6         1              1                   0
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
  Total Number of TCP retransmissions: 4
  Options:
    Timestamps enabled: yes
    Selective Acknowledgments enabled: no
    Window Scale enabled: yes
    Explicit Congestion Notification (ECN) enabled: no
  Socket Statistics:
    Window Scale (wscale): 0,7
    Retransmission Timeout (rto): 204.0ms
    Round-trip Time (rtt/rtvar): 2.7ms/0.3ms
    Delayed Ack Timeout (ato): 40.0ms
    Congestion Window (cwnd): 7
    Slow-start Threshold (ssthresh): 7
    TCP Throughput: 20.95 Mbps
    Recv Round-trip Time (rcv_rtt): 296286.3ms
    Advertised Recv Window (rcv_space): 64346

BGP neighbor is 10.0.0.221, remote AS 64512, internal link
 Description: Ribbon-221
  BGP version 4, remote router ID 10.0.0.221, VRF default
  Inherits configuration from and member of peer-group IBGP_CLIENT_PEER
  Last read 00:00:04, last write 00:00:44
  Hold time is 180, keepalive interval is 60 seconds
  Configured hold time is 180, keepalive interval is 60 seconds
  Effective minimum hold time is 3 seconds
  Send failure hold time is 0 seconds
  Hold timer is active, time left: 00:02:56
  Keepalive timer is active, time left: 00:00:02
  Connect timer is inactive
  Idle-restart timer is inactive
  BGP state is Established, up for 03:08:44
  Number of transitions to established: 2
  Last state was OpenConfirm
  Last event was RecvKeepAlive
  Last sent notification:Hold Timer Expired Error/None, Last time 03:13:52
  Last sent socket-error:Connect (Network is unreachable), Last time 03:08:48, First time 1d07h, Repeats 19
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
    Opens:                           2         2
    Notifications:                   1         0
    Updates:                       537        17
    Keepalives:                   2136      5222
    Enhanced Route Refresh:          0         2
    Begin of Route Refresh:          2         0
    End of Route Refresh:            2         0
    Total messages:               2680      5243
  Prefix Statistics:
                                   Sent      Rcvd     Best Paths     Best ECMP Paths
    IPv4 Unicast:                     0         0              0                   0
    VPN-IPv4:                        28         3              3                   0
    IPv6 Unicast:                     0         0              0                   0
    VPN-IPv6:                         7         0              0                   0
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
Local TCP address is 10.0.0.30, local port is 37361
Remote TCP address is 10.0.0.221, remote port is 179
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
    Window Scale (wscale): 9,7
    Retransmission Timeout (rto): 204.0ms
    Round-trip Time (rtt/rtvar): 2.2ms/0.7ms
    Delayed Ack Timeout (ato): 40.0ms
    Congestion Window (cwnd): 10
    TCP Throughput: 51.60 Mbps
    Advertised Recv Window (rcv_space): 14480

```

## show tunnel rib system-tunnel-rib brief

```text
Tunnel RIB: system-tunnel-rib
Endpoint        Tunnel Type     Index(es)   Tunnel Preference   IGP Preference 
-------------- --------------- ----------- ------------------- ----------------
10.0.0.32/32    IS-IS SR IPv4   9           65                  115            
10.0.0.53/32    IS-IS SR IPv4   5           65                  115            
10.0.0.84/32    IS-IS SR IPv4   1           65                  115            
10.0.0.120/32   IS-IS SR IPv4   7           65                  115            
10.0.0.124/32   IS-IS SR IPv4   14          65                  115            
10.0.0.128/32   IS-IS SR IPv4   11          65                  115            
10.0.0.131/32   IS-IS SR IPv4   12          65                  115            
10.0.0.156/32   IS-IS SR IPv4   18          65                  115            
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
   20            metric     
   10            metric     
   10            metric     
   10            metric     
   10            metric     
   10            metric     
   20            metric     
   10            metric     
   10            metric     
   10            metric     
   10            metric     
   10            metric     

```

## show tunnel rib colored brief

```text
Tunnel RIB: system-colored-tunnel-rib
 Endpoint        Color   Tunnel Type       Index(es)    Tunnel Preference    IGP Preference    IGP Metric   Metric Type
--------------- ------- ----------------- ------------ -------------------- ----------------- ------------- -----------
 10.0.0.32/32    128     IS-IS FlexAlgo    8            65                   115               10000        metric     
 10.0.0.32/32    129     IS-IS FlexAlgo    14           65                   115               100          metric     
 10.0.0.53/32    128     IS-IS FlexAlgo    10           65                   115               10000        metric     
 10.0.0.53/32    129     IS-IS FlexAlgo    11           65                   115               100          metric     
 10.0.0.120/32   128     IS-IS FlexAlgo    44           65                   115               10000        metric     
 10.0.0.120/32   129     IS-IS FlexAlgo    45           65                   115               100          metric     
 10.0.0.124/32   128     IS-IS FlexAlgo    23           65                   115               10000        metric     
 10.0.0.124/32   129     IS-IS FlexAlgo    24           65                   115               100          metric     
 10.0.0.128/32   128     IS-IS FlexAlgo    6            65                   115               10000        metric     
 10.0.0.128/32   129     IS-IS FlexAlgo    16           65                   115               100          metric     
 10.0.0.156/32   128     IS-IS FlexAlgo    27           65                   115               10000        metric     
 10.0.0.156/32   129     IS-IS FlexAlgo    26           65                   115               100          metric     
 10.0.0.175/32   128     IS-IS FlexAlgo    30           65                   115               10010        metric     
 10.0.0.175/32   129     IS-IS FlexAlgo    29           65                   115               110          metric     
 10.0.0.179/32   128     IS-IS FlexAlgo    40           65                   115               10000        metric     
 10.0.0.179/32   129     IS-IS FlexAlgo    38           65                   115               100          metric     
 10.0.0.184/32   128     IS-IS FlexAlgo    37           65                   115               10000        metric     
 10.0.0.184/32   129     IS-IS FlexAlgo    36           65                   115               100          metric     
 10.0.0.217/32   128     IS-IS FlexAlgo    4            65                   115               10000        metric     
 10.0.0.217/32   129     IS-IS FlexAlgo    13           65                   115               100          metric     
 10.0.0.221/32   128     IS-IS FlexAlgo    5            65                   115               10000        metric     
 10.0.0.221/32   129     IS-IS FlexAlgo    15           65                   115               100          metric     

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
>C    10.0.0.30/32 [0 pref/0 metric] updated 2d05h ago
         via Loopback0, directly connected
>C    20.30.32.0/24 [0 pref/0 metric] updated 1d08h ago
         via Ethernet2, directly connected
>C    20.30.53.0/24 [0 pref/0 metric] updated 09:43:09 ago
         via Ethernet13, directly connected
>C    20.30.84.0/24 [0 pref/0 metric] updated 1d08h ago
         via Ethernet12, directly connected
>C    20.30.120.0/24 [0 pref/0 metric] updated 07:34:10 ago
         via Ethernet3, directly connected
>C    20.30.124.0/24 [0 pref/0 metric] updated 1d08h ago
         via Ethernet17, directly connected
>C    20.30.128.0/24 [0 pref/0 metric] updated 1d00h ago
         via Ethernet19, directly connected
>C    20.30.131.0/24 [0 pref/0 metric] updated 03:14:35 ago
         via Ethernet35, directly connected
>C    20.30.156.0/24 [0 pref/0 metric] updated 09:25:15 ago
         via Ethernet11, directly connected
>C    20.30.179.0/24 [0 pref/0 metric] updated 1d04h ago
         via Ethernet40, directly connected
>C    20.30.184.0/24 [0 pref/0 metric] updated 04:40:19 ago
         via Ethernet7, directly connected
>C    20.30.214.0/24 [0 pref/0 metric] updated 1d07h ago
         via Ethernet5, directly connected
>C    20.30.217.0/24 [0 pref/0 metric] updated 1d08h ago
         via Ethernet4, directly connected
>C    20.30.221.0/24 [0 pref/0 metric] updated 03:09:07 ago
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
>I    10.0.0.32/32 [115 pref/10 metric] updated 1d04h ago
         via 20.30.32.32, Ethernet2
>I    10.0.0.53/32 [115 pref/10 metric] updated 09:43:07 ago
         via 20.30.53.53, Ethernet13
>I    10.0.0.84/32 [115 pref/20 metric] updated 1d04h ago
         via 20.30.84.84, Ethernet12
>I    10.0.0.120/32 [115 pref/10 metric] updated 07:34:00 ago
         via 20.30.120.120, Ethernet3
>I    10.0.0.124/32 [115 pref/10 metric] updated 1d04h ago
         via 20.30.124.124, Ethernet17
>I    10.0.0.128/32 [115 pref/10 metric] updated 1d00h ago
         via 20.30.128.128, Ethernet19
>I    10.0.0.131/32 [115 pref/10 metric] updated 03:14:13 ago
         via 20.30.131.131, Ethernet35
>I    10.0.0.156/32 [115 pref/10 metric] updated 09:24:41 ago
         via 20.30.156.156, Ethernet11
>I    10.0.0.175/32 [115 pref/20 metric] updated 00:17:40 ago
         via 20.30.32.32, Ethernet2
         via 20.30.53.53, Ethernet13
         via 20.30.84.84, Ethernet12
         via 20.30.120.120, Ethernet3
         via 20.30.124.124, Ethernet17
         via 20.30.128.128, Ethernet19
         via 20.30.131.131, Ethernet35
         via 20.30.156.156, Ethernet11
>I    10.0.0.179/32 [115 pref/10 metric] updated 1d04h ago
         via 20.30.179.179, Ethernet40
>I    10.0.0.184/32 [115 pref/10 metric] updated 01:32:47 ago
         via 20.30.184.184, Ethernet7
>I    10.0.0.214/32 [115 pref/10 metric] updated 1d04h ago
         via 20.30.214.214, Ethernet5
>I    10.0.0.216/32 [115 pref/20 metric] updated 08:02:52 ago
         via 20.30.214.214, Ethernet5
>I    10.0.0.217/32 [115 pref/10 metric] updated 1d04h ago
         via 20.30.217.217, Ethernet4
>I    10.0.0.221/32 [115 pref/10 metric] updated 03:08:49 ago
         via 20.30.221.221, Ethernet15
>I    20.32.175.0/24 [115 pref/20 metric] updated 1d04h ago
         via 20.30.32.32, Ethernet2
>I    20.53.175.0/24 [115 pref/20 metric] updated 09:43:07 ago
         via 20.30.53.53, Ethernet13
>I    20.84.175.0/24 [115 pref/35 metric] updated 00:17:40 ago
         via 20.30.32.32, Ethernet2
         via 20.30.53.53, Ethernet13
         via 20.30.84.84, Ethernet12
         via 20.30.120.120, Ethernet3
         via 20.30.124.124, Ethernet17
         via 20.30.128.128, Ethernet19
         via 20.30.131.131, Ethernet35
         via 20.30.156.156, Ethernet11
>I    20.120.175.0/24 [115 pref/20 metric] updated 02:05:18 ago
         via 20.30.120.120, Ethernet3
>I    20.120.214.0/24 [115 pref/20 metric] updated 07:34:00 ago
         via 20.30.120.120, Ethernet3
>I    20.120.217.0/24 [115 pref/10 metric] updated 04:20:36 ago
         via 20.30.120.120, Ethernet3
>I    20.124.175.0/24 [115 pref/20 metric] updated 1d04h ago
         via 20.30.124.124, Ethernet17
>I    20.128.175.0/24 [115 pref/20 metric] updated 1d00h ago
         via 20.30.128.128, Ethernet19
>I    20.131.175.0/24 [115 pref/20 metric] updated 03:14:13 ago
         via 20.30.131.131, Ethernet35
>I    20.156.175.0/24 [115 pref/20 metric] updated 09:24:41 ago
         via 20.30.156.156, Ethernet11
>I    20.175.179.0/24 [115 pref/20 metric] updated 1d04h ago
         via 20.30.179.179, Ethernet40
>I    20.175.184.0/24 [115 pref/35 metric] updated 00:00:03 ago
         via 20.30.32.32, Ethernet2
         via 20.30.53.53, Ethernet13
         via 20.30.84.84, Ethernet12
         via 20.30.120.120, Ethernet3
         via 20.30.124.124, Ethernet17
         via 20.30.128.128, Ethernet19
         via 20.30.131.131, Ethernet35
         via 20.30.156.156, Ethernet11
>I    20.175.214.0/24 [115 pref/20 metric] updated 1d04h ago
         via 20.30.214.214, Ethernet5
>I    20.175.217.0/24 [115 pref/20 metric] updated 1d04h ago
         via 20.30.217.217, Ethernet4
>I    20.175.221.0/24 [115 pref/20 metric] updated 03:08:49 ago
         via 20.30.221.221, Ethernet15
>I    20.214.216.0/24 [115 pref/20 metric] updated 1d04h ago
         via 20.30.214.214, Ethernet5
>I    192.168.20.0/23 [115 pref/10 metric] updated 04:20:36 ago
         via 20.30.120.120, Ethernet3
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
         via Ethernet2, directly connected
>C    2001:0:30:84::/64 [0 pref/0 metric] updated 1d08h ago
         via Ethernet12, directly connected
>C    2001:0:30:120::/64 [0 pref/0 metric] updated 07:34:10 ago
         via Ethernet3, directly connected
>C    2001:0:30:124::/64 [0 pref/0 metric] updated 1d08h ago
         via Ethernet17, directly connected
>C    2001:0:30:128::/64 [0 pref/0 metric] updated 1d00h ago
         via Ethernet19, directly connected
>C    2001:0:30:131::/64 [0 pref/0 metric] updated 03:14:27 ago
         via Ethernet35, directly connected
>C    2001:0:30:156::/64 [0 pref/0 metric] updated 09:25:15 ago
         via Ethernet11, directly connected
>C    2001:0:30:179::/64 [0 pref/0 metric] updated 1d04h ago
         via Ethernet40, directly connected
>C    2001:0:30:184::/64 [0 pref/0 metric] updated 04:40:19 ago
         via Ethernet7, directly connected
>C    2001:0:30:214::/64 [0 pref/0 metric] updated 1d07h ago
         via Ethernet5, directly connected
>C    2001:0:30:217::/64 [0 pref/0 metric] updated 1d08h ago
         via Ethernet4, directly connected
>C    2001:0:30:221::/64 [0 pref/0 metric] updated 03:09:07 ago
         via Ethernet15, directly connected
>C    2001:0:53:120::/64 [0 pref/0 metric] updated 09:43:09 ago
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
>I    2001:0:32:175::/64 [115 pref/20 metric] updated 1d04h ago
         via fe80::d6af:f7ff:fe2f:1396, Ethernet2
>I    2001:0:84:175::/64 [115 pref/20 metric] updated 1d04h ago
         via fe80::5a70:7fff:fe9f:c403, Ethernet12
>I    2001:0:120:175::/64 [115 pref/20 metric] updated 07:34:00 ago
         via fe80::be31:e2ff:fee1:ec2c, Ethernet3
>I    2001:0:120:214::/64 [115 pref/20 metric] updated 07:34:00 ago
         via fe80::be31:e2ff:fee1:ec2c, Ethernet3
```

## show platform sand l3 summary

```text
Number of vrfs: 4

Ipv4:
  Routes:       147  backlog:  0  unprogrammed:  0
  Adjacencies:  228  backlog:  0  unprogrammed:  0
Ipv6:
  Routes:       35   backlog:  0  unprogrammed:  0
  Adjacencies:  228  backlog:  0  unprogrammed:  0
Mpls:
  Routes:       52  backlog:  0  unprogrammed:  0
  Adjacencies:  18  backlog:  0  unprogrammed:  0

Jericho2 Ip Fecs:
  Non-ecmp fecs:  4202  ecmp fecs:  1  fec entries:  4210
Jericho2 Mpls Fecs:
  Non-ecmp fecs:  16  ecmp fecs:  2  fec entries:  32
Jericho2 Vxlan Tunnel Fecs:
  Non-ecmp fecs:  0  ecmp fecs:  0  fec entries:  0
  Number of vxlan tunnels configured: 0

Jericho2 Lpm Routes:
  Routes:   147  unprogrammed:   0   
  Routes6:  35   unprogrammed6:  0   
  Backlog:  0  

Jericho2 Lpm:
  TCAM entries used:   3   Percent free:  99  ADS2 entries used:   10  Percent free:  99
  Pivot buckets used:  4   Rows used:     2   Entries Per Bucket:  2   Percent free:  99
  Route buckets used:  31  Rows used:     4   Entries Per Bucket:  5   Percent free:  99

Lem:
  IPv4  Host in Lem:            disabled
  IPv4  Prefix-lengths in Lem:  None    
  IPv6  Host in Lem:            disabled
  IPv6  Prefix-lengths in Lem:  None    
  Number of downloads:        0
  Number of overflow events:  0

Egress Arp rewrite entries in use (in each fap):
  FixedSystem: 13
Egress Arp remote rewrite entries in use (in each fap):
  FixedSystem: 0
Egress Ip tunnel rewrite entries in use (in each fap):
  FixedSystem: 0
Egress Mpls (for outer 2 labels) rewrite entries in use (in each fap):
  FixedSystem: 0
Egress Mpls (for inner 2 labels) rewrite entries in use (in each fap):
  FixedSystem: 35
Egress Sflow rewrite entries in use (in each fap):
  FixedSystem: 0

Egress rewrite chains in backlog: resource-full 0, no-interface 0

Glem entries used per fap :
  FixedSystem: 4161

Jericho2 Fec:
  Maximum FEC hierarchy levels:  2
  ReusedEcmp:  281  allocs:  8614  frees:  8492  shuffles:  0  cmds:  0
  Zombies:     0    purges:    0
  Quarantine:  0/0  shuffles:  0  deletes:  0   
  Preserved FECs: 0
    First FEC preserved: never
    Last FEC preserved: never
  Fec insertion failures:  0
  Level1  Fecs:
    Non-ecmp fecs:            36  ecmp fecs:            1 
    Non-ecmp (Percent free):  99  ecmp (Percent free):  99
  Level2  Fecs:
    Non-ecmp fecs:            107  ecmp fecs:            3 
    Non-ecmp (Percent free):  99   ecmp (Percent free):  99
  Level3  Fecs:
    Non-ecmp fecs:            0    ecmp fecs:            0  
    Non-ecmp (Percent free):  100  ecmp (Percent free):  100

Lpm Detail:
  Requests:  9145  cleanses:  5474  batches:  5474  avg batch size:  1

Jericho Arp:
  ArpTable writes:      280500  queued      0   
  IngressTable writes:  202600  queued      0   
  Coprocessors:         1       in CmdRing

Tunnel Counter Status
  Number of MPLS tunnels:                  52   
  Number of uncountable MPLS tunnels:      52   
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
|0  |10.0.0.32/32      |ROUTE| Et2                |1007 |103427  | d4:af:f7:2f:13:96 |  -  |183589|   -   
|0  |10.0.0.53/32      |ROUTE| Et13               |1014 |103432  | 5c:07:58:a3:0a:aa |  -  |183586|   -   
|0  |10.0.0.84/32      |ROUTE| Et12               |1013 |103422  | 58:70:7f:9f:c4:03 |  -  |183615|   -   
|0  |10.0.0.120/32     |ROUTE| Et3                |1008 |103426  | bc:31:e2:e1:ec:2c |  -  |183556|   -   
|0  |10.0.0.124/32     |ROUTE| Et17               |1016 |103440  | 64:6d:4e:32:e1:22 |  -  |183557|   -   
|0  |10.0.0.128/32     |ROUTE| Et19               |1018 |103431  | 60:53:75:13:ba:d8 |  -  |183549|   -   
|0  |10.0.0.131/32     |ROUTE| Et35               |1022 |103424  | 40:a6:b7:94:34:cb |  -  |183519|   -   
|0  |10.0.0.156/32     |ROUTE| Et11               |1021 |103421  | d0:48:a1:ba:3c:61 |  -  |183506|   -   
|0  |10.0.0.175/32     |ROUTE| Et35               |1022 |103424  | 40:a6:b7:94:34:cb |16385|183622|   -   
|0  |10.0.0.175/32     |ROUTE| Et19               |1018 |103431  | 60:53:75:13:ba:d8 |16385|183623|   -   
|0  |10.0.0.175/32     |ROUTE| Et13               |1014 |103432  | 5c:07:58:a3:0a:aa |16385|183624|   -   
|0  |10.0.0.175/32     |ROUTE| Et12               |1013 |103422  | 58:70:7f:9f:c4:03 |16385|183625|   -   
|0  |10.0.0.175/32     |ROUTE| Et3                |1008 |103426  | bc:31:e2:e1:ec:2c |16385|183626|   -   
|0  |10.0.0.175/32     |ROUTE| Et11               |1021 |103421  | d0:48:a1:ba:3c:61 |16385|183627|   -   
|0  |10.0.0.175/32     |ROUTE| Et2                |1007 |103427  | d4:af:f7:2f:13:96 |16385|183628|   -   
|0  |10.0.0.175/32     |ROUTE| Et17               |1016 |103440  | 64:6d:4e:32:e1:22 |16385|183629|   -   
|0  |10.0.0.179/32     |ROUTE| Et40               |1020 |103429  | e8:24:a6:96:05:48 |  -  |183618|   -   
|0  |10.0.0.184/32     |ROUTE| Et7                |1011 |103435  | 00:2c:01:00:00:01 |  -  |183612|   -   
|0  |10.0.0.214/32     |ROUTE| Et5                |1010 |103428  | 18:5b:00:61:ac:6f |  -  |183530|   -   
|0  |10.0.0.216/32     |ROUTE| Et5                |1010 |103428  | 18:5b:00:61:ac:6f |  -  |183530|   -   
|0  |10.0.0.217/32     |ROUTE| Et4                |1009 |103423  | c0:14:b8:21:97:90 |  -  |183525|   -   
|0  |10.0.0.221/32     |ROUTE| Et15               |1015 |103437  | 30:c5:07:84:3e:79 |  -  |183561|   -   
|0  |20.30.32.0/32     |TRAP | CoppSystemIpBcast  |0    |  -     | BcastReceive      |  -  |314666|   -   
|0  |20.30.32.30/32    |TRAP | CoppSystemIpUcast  |0    |  -     | Receive           |  -  |314667|   -   
|0  |20.30.32.32/32    |ROUTE| Et2                |1007 |103427  | d4:af:f7:2f:13:96 |  -  |183528|   -   
|0  |20.30.32.255/32   |TRAP | CoppSystemIpBcast  |0    |  -     | BcastReceive      |  -  |314666|   -   
|0  |20.30.32.0/24     |TRAP | CoppSystemL3DstMiss|1007 |1007    | ArpTrap           |  -  |315678|   -   
|0  |20.30.53.0/32     |TRAP | CoppSystemIpBcast  |0    |  -     | BcastReceive      |  -  |314666|   -   
|0  |20.30.53.30/32    |TRAP | CoppSystemIpUcast  |0    |  -     | Receive           |  -  |314667|   -   
|0  |20.30.53.53/32    |ROUTE| Et13               |1014 |103432  | 5c:07:58:a3:0a:aa |  -  |183521|   -   
|0  |20.30.53.255/32   |TRAP | CoppSystemIpBcast  |0    |  -     | BcastReceive      |  -  |314666|   -   
|0  |20.30.53.0/24     |TRAP | CoppSystemL3DstMiss|1014 |1014    | ArpTrap           |  -  |315685|   -   
|0  |20.30.84.0/32     |TRAP | CoppSystemIpBcast  |0    |  -     | BcastReceive      |  -  |314666|   -   
|0  |20.30.84.30/32    |TRAP | CoppSystemIpUcast  |0    |  -     | Receive           |  -  |314667|   -   
|0  |20.30.84.84/32    |ROUTE| Et12               |1013 |103422  | 58:70:7f:9f:c4:03 |  -  |183507|   -   
|0  |20.30.84.255/32   |TRAP | CoppSystemIpBcast  |0    |  -     | BcastReceive      |  -  |314666|   -   
|0  |20.30.84.0/24     |TRAP | CoppSystemL3DstMiss|1013 |1013    | ArpTrap           |  -  |315684|   -   
|0  |20.30.120.0/32    |TRAP | CoppSystemIpBcast  |0    |  -     | BcastReceive      |  -  |314666|   -   
|0  |20.30.120.30/32   |TRAP | CoppSystemIpUcast  |0    |  -     | Receive           |  -  |314667|   -   
|0  |20.30.120.120/32  |ROUTE| Et3                |1008 |103426  | bc:31:e2:e1:ec:2c |  -  |183548|   -   
|0  |20.30.120.255/32  |TRAP | CoppSystemIpBcast  |0    |  -     | BcastReceive      |  -  |314666|   -   
|0  |20.30.120.0/24    |TRAP | CoppSystemL3DstMiss|1008 |1008    | ArpTrap           |  -  |315679|   -   
|0  |20.30.124.0/32    |TRAP | CoppSystemIpBcast  |0    |  -     | BcastReceive      |  -  |314666|   -   
|0  |20.30.124.30/32   |TRAP | CoppSystemIpUcast  |0    |  -     | Receive           |  -  |314667|   -   
|0  |20.30.124.124/32  |ROUTE| Et17               |1016 |103440  | 64:6d:4e:32:e1:22 |  -  |183571|   -   
|0  |20.30.124.255/32  |TRAP | CoppSystemIpBcast  |0    |  -     | BcastReceive      |  -  |314666|   -   
|0  |20.30.124.0/24    |TRAP | CoppSystemL3DstMiss|1016 |1016    | ArpTrap           |  -  |315687|   -   
|0  |20.30.128.0/32    |TRAP | CoppSystemIpBcast  |0    |  -     | BcastReceive      |  -  |314666|   -   
|0  |20.30.128.30/32   |TRAP | CoppSystemIpUcast  |0    |  -     | Receive           |  -  |314667|   -   
|0  |20.30.128.128/32  |ROUTE| Et19               |1018 |103431  | 60:53:75:13:ba:d8 |  -  |183570|   -   
|0  |20.30.128.255/32  |TRAP | CoppSystemIpBcast  |0    |  -     | BcastReceive      |  -  |314666|   -   
|0  |20.30.128.0/24    |TRAP | CoppSystemL3DstMiss|1018 |1018    | ArpTrap           |  -  |315689|   -   
|0  |20.30.131.0/32    |TRAP | CoppSystemIpBcast  |0    |  -     | BcastReceive      |  -  |314666|   -   
|0  |20.30.131.30/32   |TRAP | CoppSystemIpUcast  |0    |  -     | Receive           |  -  |314667|   -   
|0  |20.30.131.131/32  |ROUTE| Et35               |1022 |103424  | 40:a6:b7:94:34:cb |  -  |183517|   -   
|0  |20.30.131.255/32  |TRAP | CoppSystemIpBcast  |0    |  -     | BcastReceive      |  -  |314666|   -   
|0  |20.30.131.0/24    |TRAP | CoppSystemL3DstMiss|1022 |1022    | ArpTrap           |  -  |315693|   -   
|0  |20.30.156.0/32    |TRAP | CoppSystemIpBcast  |0    |  -     | BcastReceive      |  -  |314666|   -   
|0  |20.30.156.30/32   |TRAP | CoppSystemIpUcast  |0    |  -     | Receive           |  -  |314667|   -   
|0  |20.30.156.156/32  |ROUTE| Et11               |1021 |103421  | d0:48:a1:ba:3c:61 |  -  |183513|   -   
|0  |20.30.156.255/32  |TRAP | CoppSystemIpBcast  |0    |  -     | BcastReceive      |  -  |314666|   -   
|0  |20.30.156.0/24    |TRAP | CoppSystemL3DstMiss|1021 |1021    | ArpTrap           |  -  |315692|   -   
|0  |20.30.179.0/32    |TRAP | CoppSystemIpBcast  |0    |  -     | BcastReceive      |  -  |314666|   -   
|0  |20.30.179.30/32   |TRAP | CoppSystemIpUcast  |0    |  -     | Receive           |  -  |314667|   -   
|0  |20.30.179.179/32  |ROUTE| Et40               |1020 |103429  | e8:24:a6:96:05:48 |  -  |183547|   -   
|0  |20.30.179.255/32  |TRAP | CoppSystemIpBcast  |0    |  -     | BcastReceive      |  -  |314666|   -   
|0  |20.30.179.0/24    |TRAP | CoppSystemL3DstMiss|1020 |1020    | ArpTrap           |  -  |315691|   -   
|0  |20.30.184.0/32    |TRAP | CoppSystemIpBcast  |0    |  -     | BcastReceive      |  -  |314666|   -   
|0  |20.30.184.30/32   |TRAP | CoppSystemIpUcast  |0    |  -     | Receive           |  -  |314667|   -   
|0  |20.30.184.184/32  |ROUTE| Et7                |1011 |103435  | 00:2c:01:00:00:01 |  -  |183529|   -   
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
|0  |20.30.221.221/32  |ROUTE| Et15               |1015 |103437  | 30:c5:07:84:3e:79 |  -  |183562|   -   
|0  |20.30.221.255/32  |TRAP | CoppSystemIpBcast  |0    |  -     | BcastReceive      |  -  |314666|   -   
|0  |20.30.221.0/24    |TRAP | CoppSystemL3DstMiss|1015 |1015    | ArpTrap           |  -  |315686|   -   
|0  |20.32.175.0/24    |ROUTE| Et2                |1007 |103427  | d4:af:f7:2f:13:96 |  -  |183589|   -   
|0  |20.53.175.0/24    |ROUTE| Et13               |1014 |103432  | 5c:07:58:a3:0a:aa |  -  |183586|   -   
|0  |20.84.175.0/24    |ROUTE| Et35               |1022 |103424  | 40:a6:b7:94:34:cb |16385|183622|   -   
|0  |20.84.175.0/24    |ROUTE| Et19               |1018 |103431  | 60:53:75:13:ba:d8 |16385|183623|   -   
|0  |20.84.175.0/24    |ROUTE| Et13               |1014 |103432  | 5c:07:58:a3:0a:aa |16385|183624|   -   
|0  |20.84.175.0/24    |ROUTE| Et12               |1013 |103422  | 58:70:7f:9f:c4:03 |16385|183625|   -   
|0  |20.84.175.0/24    |ROUTE| Et3                |1008 |103426  | bc:31:e2:e1:ec:2c |16385|183626|   -   
|0  |20.84.175.0/24    |ROUTE| Et11               |1021 |103421  | d0:48:a1:ba:3c:61 |16385|183627|   -   
|0  |20.84.175.0/24    |ROUTE| Et2                |1007 |103427  | d4:af:f7:2f:13:96 |16385|183628|   -   
|0  |20.84.175.0/24    |ROUTE| Et17               |1016 |103440  | 64:6d:4e:32:e1:22 |16385|183629|   -   
|0  |20.120.175.0/24   |ROUTE| Et3                |1008 |103426  | bc:31:e2:e1:ec:2c |  -  |183556|   -   
|0  |20.120.214.0/24   |ROUTE| Et3                |1008 |103426  | bc:31:e2:e1:ec:2c |  -  |183556|   -   
|0  |20.120.217.0/24   |ROUTE| Et3                |1008 |103426  | bc:31:e2:e1:ec:2c |  -  |183556|   -   
|0  |20.124.175.0/24   |ROUTE| Et17               |1016 |103440  | 64:6d:4e:32:e1:22 |  -  |183557|   -   
|0  |20.128.175.0/24   |ROUTE| Et19               |1018 |103431  | 60:53:75:13:ba:d8 |  -  |183549|   -   
|0  |20.131.175.0/24   |ROUTE| Et35               |1022 |103424  | 40:a6:b7:94:34:cb |  -  |183519|   -   
|0  |20.156.175.0/24   |ROUTE| Et11               |1021 |103421  | d0:48:a1:ba:3c:61 |  -  |183506|   -   
|0  |20.175.179.0/24   |ROUTE| Et40               |1020 |103429  | e8:24:a6:96:05:48 |  -  |183618|   -   
|0  |20.175.184.0/24   |ROUTE| Et35               |1022 |103424  | 40:a6:b7:94:34:cb |16385|183622|   -   
|0  |20.175.184.0/24   |ROUTE| Et19               |1018 |103431  | 60:53:75:13:ba:d8 |16385|183623|   -   
|0  |20.175.184.0/24   |ROUTE| Et13               |1014 |103432  | 5c:07:58:a3:0a:aa |16385|183624|   -   
|0  |20.175.184.0/24   |ROUTE| Et12               |1013 |103422  | 58:70:7f:9f:c4:03 |16385|183625|   -   
|0  |20.175.184.0/24   |ROUTE| Et3                |1008 |103426  | bc:31:e2:e1:ec:2c |16385|183626|   -   
|0  |20.175.184.0/24   |ROUTE| Et11               |1021 |103421  | d0:48:a1:ba:3c:61 |16385|183627|   -   
|0  |20.175.184.0/24   |ROUTE| Et2                |1007 |103427  | d4:af:f7:2f:13:96 |16385|183628|   -   
|0  |20.175.184.0/24   |ROUTE| Et17               |1016 |103440  | 64:6d:4e:32:e1:22 |16385|183629|   -   
|0  |20.175.214.0/24   |ROUTE| Et5                |1010 |103428  | 18:5b:00:61:ac:6f |  -  |183530|   -   
|0  |20.175.217.0/24   |ROUTE| Et4                |1009 |103423  | c0:14:b8:21:97:90 |  -  |183525|   -   
|0  |20.175.221.0/24   |ROUTE| Et15               |1015 |103437  | 30:c5:07:84:3e:79 |  -  |183561|   -   
|0  |20.214.216.0/24   |ROUTE| Et5                |1010 |103428  | 18:5b:00:61:ac:6f |  -  |183530|   -   
|0  |127.0.0.0/8       |TRAP | CoppSystemL3DstMiss|0    |  -     | ArpTrap           |  -  |314671|   -   
|0  |192.168.20.0/23   |ROUTE| Et3                |1008 |103426  | bc:31:e2:e1:ec:2c |  -  |183556|   -   
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
|2  |50.10.32.0/24     |ROUTE| FEC 183535         |0    |2097145 | 00:00:00:00:00:00 |  -  |131078|M 378528
|2  |50.10.84.0/24     |ROUTE| FEC 183536         |0    |2097142 | 00:00:00:00:00:00 |  -  |131073|M 20084 720896
|2  |50.10.131.0/24    |ROUTE| FEC 183617         |0    |2097146 | 00:00:00:00:00:00 |  -  |131098|M 18
|2  |50.10.156.0/24    |ROUTE| FEC 183516         |0    |2097140 | 00:00:00:00:00:00 |  -  |131086|M 16
|2  |50.10.179.0/24    |ROUTE| FEC 183537         |0    |2097141 | 00:00:00:00:00:00 |  -  |131081|M 16
|2  |50.10.214.0/24    |ROUTE| FEC 183514         |0    |2097136 | 00:00:00:00:00:00 |  -  |131076|M 20214 500000
|2  |50.10.217.0/24    |ROUTE| FEC 183584         |0    |2097150 | 00:00:00:00:00:00 |  -  |131077|M 20217 524287
|2  |127.0.0.0/8       |TRAP | CoppSystemL3DstMiss|0    |  -     | ArpTrap           |  -  |314671|   -   
|2  |0.0.0.0/0         |TRAP | CoppSystemL3LpmOver|0    |  -     | SlowReceive       |  -  |314669|   -   
|3  |0.0.0.0/8         |DROP | DROP               |0    |  -     |                   |  -  |183583|   -   
|3  |10.128.0.30/32    |TRAP | CoppSystemIpUcast  |0    |  -     | Receive           |  -  |314667|   -   
|3  |50.128.32.0/24    |ROUTE| FEC 183558         |0    |2097121 | 00:00:00:00:00:00 |  -  |131088|M 378530
|3  |50.128.53.0/24    |ROUTE| FEC 183603         |0    |2097133 | 00:00:00:00:00:00 |  -  |131095|M 970000
|3  |50.128.120.0/24   |ROUTE| FEC 183565         |0    |2097148 | 00:00:00:00:00:00 |  -  |131072|M 21248 1272
|3  |50.128.156.0/24   |ROUTE| FEC 183620         |0    |2097128 | 00:00:00:00:00:00 |  -  |131108|M 21
|3  |50.128.179.0/24   |ROUTE| FEC 183560         |0    |2097138 | 00:00:00:00:00:00 |  -  |131111|M 21
|3  |50.128.184.0/24   |ROUTE| FEC 183542         |0    |2097137 | 00:00:00:00:00:00 |  -  |131094|M 16
|3  |50.128.217.0/24   |ROUTE| FEC 183592         |0    |2097119 | 00:00:00:00:00:00 |  -  |131087|M 21345 524284
|3  |50.128.221.0/24   |ROUTE| FEC 183619         |0    |2097147 | 00:00:00:00:00:00 |  -  |131079|M 524291
|3  |50.129.32.0/24    |ROUTE| FEC 183648         |0    |2097110 | 00:00:00:00:00:00 |  -  |131089|M 378530
|3  |50.129.53.0/24    |ROUTE| FEC 183532         |0    |2097132 | 00:00:00:00:00:00 |  -  |131096|M 970000
|3  |50.129.120.0/24   |ROUTE| FEC 183621         |0    |2097108 | 00:00:00:00:00:00 |  -  |131074|M 21249 1274
|3  |50.129.156.0/24   |ROUTE| FEC 183590         |0    |2097114 | 00:00:00:00:00:00 |  -  |131109|M 21
|3  |50.129.179.0/24   |ROUTE| FEC 183518         |0    |2097127 | 00:00:00:00:00:00 |  -  |131112|M 21
|3  |50.129.184.0/24   |ROUTE| FEC 183542         |0    |2097120 | 00:00:00:00:00:00 |  -  |131113|M 17
|3  |50.129.217.0/24   |ROUTE| FEC 183515         |0    |2097124 | 00:00:00:00:00:00 |  -  |131084|M 21346 524284
|3  |50.129.221.0/24   |ROUTE| FEC 183582         |0    |2097107 | 00:00:00:00:00:00 |  -  |131097|M 524291
|3  |50.130.32.0/24    |ROUTE| FEC 183535         |0    |2097129 | 00:00:00:00:00:00 |  -  |131080|M 378530
|3  |50.130.53.0/24    |ROUTE| FEC 183564         |0    |2097135 | 00:00:00:00:00:00 |  -  |131082|M 970000
|3  |50.130.120.0/24   |ROUTE| FEC 183545         |0    |2097126 | 00:00:00:00:00:00 |  -  |131090|M 1273
|3  |50.130.156.0/24   |ROUTE| FEC 183516         |0    |2097130 | 00:00:00:00:00:00 |  -  |131107|M 21
|3  |50.130.179.0/24   |ROUTE| FEC 183537         |0    |2097131 | 00:00:00:00:00:00 |  -  |131110|M 21
|3  |50.130.184.0/24   |ROUTE| FEC 183542         |0    |2097143 | 00:00:00:00:00:00 |  -  |131106|M 18
|3  |50.130.217.0/24   |ROUTE| FEC 183584         |0    |2097134 | 00:00:00:00:00:00 |  -  |131085|M 20217 524284
|3  |50.130.221.0/24   |ROUTE| FEC 183543         |0    |2097125 | 00:00:00:00:00:00 |  -  |131099|M 524291
|3  |127.0.0.0/8       |TRAP | CoppSystemL3DstMiss|0    |  -     | ArpTrap           |  -  |314671|   -   
|3  |0.0.0.0/0         |TRAP | CoppSystemL3LpmOver|0    |  -     | SlowReceive       |  -  |314669|   -   

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
|16384|183572|ROUTE| Et11               |1021 |103456  | d0:48:a1:ba:3c:61 |Mswap 21304
|16384|183573|ROUTE| Et15               |1015 |103448  | 30:c5:07:84:3e:79 |Mswap 721304
|16384|183574|ROUTE| Et13               |1014 |103449  | 5c:07:58:a3:0a:aa |Mswap 21304
|16384|183575|ROUTE| Et3                |1008 |103490  | bc:31:e2:e1:ec:2c |Mswap 21304
|16384|183576|ROUTE| Et4                |1009 |103459  | c0:14:b8:21:97:90 |Mswap 21304
|16384|183577|ROUTE| Et19               |1018 |103454  | 60:53:75:13:ba:d8 |Mswap 21304
|16384|183578|ROUTE| Et17               |1016 |103455  | 64:6d:4e:32:e1:22 |Mswap 3304
|16384|183579|ROUTE| Et40               |1020 |103451  | e8:24:a6:96:05:48 |Mswap 21304
|16385|183622|ROUTE| Et35               |1022 |103424  | 40:a6:b7:94:34:cb |   -   
|16385|183623|ROUTE| Et19               |1018 |103431  | 60:53:75:13:ba:d8 |   -   
|16385|183624|ROUTE| Et13               |1014 |103432  | 5c:07:58:a3:0a:aa |   -   
|16385|183625|ROUTE| Et12               |1013 |103422  | 58:70:7f:9f:c4:03 |   -   
|16385|183626|ROUTE| Et3                |1008 |103426  | bc:31:e2:e1:ec:2c |   -   
|16385|183627|ROUTE| Et11               |1021 |103421  | d0:48:a1:ba:3c:61 |   -   
|16385|183628|ROUTE| Et2                |1007 |103427  | d4:af:f7:2f:13:96 |   -   
|16385|183629|ROUTE| Et17               |1016 |103440  | 64:6d:4e:32:e1:22 |   -   
|16386|183633|ROUTE| Et19               |1018 |103434  | 60:53:75:13:ba:d8 |Mswap 20175
|16386|183634|ROUTE| Et3                |1008 |103446  | bc:31:e2:e1:ec:2c |Mswap 20175
|16386|183635|ROUTE| Et17               |1016 |103436  | 64:6d:4e:32:e1:22 |Mswap 2175
|16386|183636|ROUTE| Et35               |1022 |103489  | 40:a6:b7:94:34:cb |Mswap 20175
|16386|183637|ROUTE| Et12               |1013 |103441  | 58:70:7f:9f:c4:03 |Mswap 20175
|16386|183638|ROUTE| Et13               |1014 |103442  | 5c:07:58:a3:0a:aa |Mswap 20175
|16386|183639|ROUTE| Et11               |1021 |103458  | d0:48:a1:ba:3c:61 |Mswap 20175
|16386|183640|ROUTE| Et2                |1007 |103444  | d4:af:f7:2f:13:96 |Mswap 20175
|  -  |131072|ROUTE| FEC 183565         |   - |2097148 |                 - |Mpush 21248 1272
|  -  |131073|ROUTE| FEC 183536         |   - |2097142 |                 - |Mpush 20084 720896
|  -  |131074|ROUTE| FEC 183621         |   - |2097108 |                 - |Mpush 21249 1274
|  -  |131075|ROUTE| FEC 183563         |   - |  -     |                   |   -   
|  -  |131076|ROUTE| FEC 183514         |   - |2097136 |                 - |Mpush 20214 500000
|  -  |131077|ROUTE| FEC 183584         |   - |2097150 |                 - |Mpush 20217 524287
|  -  |131078|ROUTE| FEC 183535         |   - |2097145 |                 - |Mpush 378528
|  -  |131079|ROUTE| FEC 183619         |   - |2097147 |                 - |Mpush 524291
|  -  |131080|ROUTE| FEC 183535         |   - |2097129 |                 - |Mpush 378530
|  -  |131081|ROUTE| FEC 183537         |   - |2097141 |                 - |Mpush 16
|  -  |131082|ROUTE| FEC 183564         |   - |2097135 |                 - |Mpush 970000
|  -  |131083|ROUTE| FEC 183564         |   - |  -     |                   |   -   
|  -  |131084|ROUTE| FEC 183515         |   - |2097124 |                 - |Mpush 21346 524284
|  -  |131085|ROUTE| FEC 183584         |   - |2097134 |                 - |Mpush 20217 524284
|  -  |131086|ROUTE| FEC 183516         |   - |2097140 |                 - |Mpush 16
|  -  |131087|ROUTE| FEC 183592         |   - |2097119 |                 - |Mpush 21345 524284
|  -  |131088|ROUTE| FEC 183558         |   - |2097121 |                 - |Mpush 378530
|  -  |131089|ROUTE| FEC 183648         |   - |2097110 |                 - |Mpush 378530
|  -  |131090|ROUTE| FEC 183545         |   - |2097126 |                 - |Mpush 1273
|  -  |131091|ROUTE| FEC 183510         |   - |  -     |                   |   -   
|  -  |131092|ROUTE| FEC 183605         |   - |  -     |                   |   -   
|  -  |131093|ROUTE| FEC 183559         |   - |  -     |                   |   -   
|  -  |131094|ROUTE| FEC 183542         |   - |2097123 |                 - |Mpush 16
|  -  |131095|ROUTE| FEC 183603         |   - |2097133 |                 - |Mpush 970000
|  -  |131096|ROUTE| FEC 183532         |   - |2097132 |                 - |Mpush 970000
|  -  |131097|ROUTE| FEC 183582         |   - |2097107 |                 - |Mpush 524291
|  -  |131098|ROUTE| FEC 183617         |   - |2097146 |                 - |Mpush 18
|  -  |131099|ROUTE| FEC 183543         |   - |2097125 |                 - |Mpush 524291
|  -  |131106|ROUTE| FEC 183542         |   - |2097143 |                 - |Mpush 18
|  -  |131107|ROUTE| FEC 183516         |   - |2097130 |                 - |Mpush 21
|  -  |131108|ROUTE| FEC 183620         |   - |2097128 |                 - |Mpush 21
|  -  |131109|ROUTE| FEC 183590         |   - |2097114 |                 - |Mpush 21
|  -  |131110|ROUTE| FEC 183537         |   - |2097131 |                 - |Mpush 21
|  -  |131111|ROUTE| FEC 183560         |   - |2097138 |                 - |Mpush 21
|  -  |131112|ROUTE| FEC 183518         |   - |2097127 |                 - |Mpush 21
|  -  |131113|ROUTE| FEC 183542         |   - |2097139 |                 - |Mpush 17
|  -  |183502|DROP | DROP               |0    |  -     |                   |   -   
|  -  |183503|DROP | DROP               |0    |  -     |                   |   -   
|  -  |183504|DROP | DROP               |0    |  -     |                   |   -   
|  -  |183505|DROP | DROP               |0    |  -     |                   |   -   
|  -  |183506|ROUTE| Et11               |1021 |103421  | d0:48:a1:ba:3c:61 |   -   
|  -  |183507|ROUTE| Et12               |1013 |103422  | 58:70:7f:9f:c4:03 |   -   
|  -  |183508|ROUTE| Et4                |1009 |103423  | c0:14:b8:21:97:90 |   -   
|  -  |183510|ROUTE| Et15               |1015 |103443  | 30:c5:07:84:3e:79 |Mpush 721303
|  -  |183511|ROUTE| Et19               |1018 |103431  | 60:53:75:13:ba:d8 |   -   
|  -  |183512|ROUTE| Et3                |1008 |103426  | bc:31:e2:e1:ec:2c |   -   
|  -  |183513|ROUTE| Et11               |1021 |103421  | d0:48:a1:ba:3c:61 |   -   
|  -  |183514|ROUTE| Et5                |1010 |103428  | 18:5b:00:61:ac:6f |   -   
|  -  |183515|ROUTE| Et4                |1009 |103423  | c0:14:b8:21:97:90 |   -   
|  -  |183516|ROUTE| Et11               |1021 |103421  | d0:48:a1:ba:3c:61 |   -   
|  -  |183517|ROUTE| Et35               |1022 |103424  | 40:a6:b7:94:34:cb |   -   
|  -  |183518|ROUTE| Et40               |1020 |103429  | e8:24:a6:96:05:48 |   -   
|  -  |183519|ROUTE| Et35               |1022 |103424  | 40:a6:b7:94:34:cb |   -   
|  -  |183521|ROUTE| Et13               |1014 |103432  | 5c:07:58:a3:0a:aa |   -   
|  -  |183522|ROUTE| Et3                |1008 |103426  | bc:31:e2:e1:ec:2c |   -   
|  -  |183524|ROUTE| Et13               |1014 |103432  | 5c:07:58:a3:0a:aa |   -   
|  -  |183525|ROUTE| Et4                |1009 |103423  | c0:14:b8:21:97:90 |   -   
|  -  |183526|ROUTE| Et3                |1008 |103426  | bc:31:e2:e1:ec:2c |   -   
|  -  |183527|ROUTE| Et4                |1009 |103423  | c0:14:b8:21:97:90 |   -   
|  -  |183528|ROUTE| Et2                |1007 |103427  | d4:af:f7:2f:13:96 |   -   
|  -  |183529|ROUTE| Et7                |1011 |103435  | 00:2c:01:00:00:01 |   -   
|  -  |183530|ROUTE| Et5                |1010 |103428  | 18:5b:00:61:ac:6f |   -   
|  -  |183531|ROUTE| Et35               |1022 |103424  | 40:a6:b7:94:34:cb |   -   
|  -  |183532|ROUTE| Et13               |1014 |103432  | 5c:07:58:a3:0a:aa |   -   
|  -  |183533|ROUTE| Et5                |1010 |103428  | 18:5b:00:61:ac:6f |   -   
|  -  |183534|ROUTE| Et12               |1013 |103422  | 58:70:7f:9f:c4:03 |   -   
|  -  |183535|ROUTE| Et2                |1007 |103427  | d4:af:f7:2f:13:96 |   -   
|  -  |183536|ROUTE| Et12               |1013 |103422  | 58:70:7f:9f:c4:03 |   -   
|  -  |183537|ROUTE| Et40               |1020 |103429  | e8:24:a6:96:05:48 |   -   
|  -  |183539|ROUTE| Et19               |1018 |103431  | 60:53:75:13:ba:d8 |   -   
|  -  |183540|ROUTE| Et15               |1015 |103437  | 30:c5:07:84:3e:79 |   -   
|  -  |183542|ROUTE| Et7                |1011 |103435  | 00:2c:01:00:00:01 |   -   
|  -  |183543|ROUTE| Et15               |1015 |103437  | 30:c5:07:84:3e:79 |   -   
|  -  |183544|ROUTE| Et40               |1020 |103429  | e8:24:a6:96:05:48 |   -   
|  -  |183545|ROUTE| Et3                |1008 |103426  | bc:31:e2:e1:ec:2c |   -   
|  -  |183546|ROUTE| Et19               |1018 |103431  | 60:53:75:13:ba:d8 |   -   
|  -  |183547|ROUTE| Et40               |1020 |103429  | e8:24:a6:96:05:48 |   -   
|  -  |183548|ROUTE| Et3                |1008 |103426  | bc:31:e2:e1:ec:2c |   -   
|  -  |183549|ROUTE| Et19               |1018 |103431  | 60:53:75:13:ba:d8 |   -   
|  -  |183550|ROUTE| Et17               |1016 |103440  | 64:6d:4e:32:e1:22 |   -   
|  -  |183551|ROUTE| Et7                |1011 |103435  | 00:2c:01:00:00:01 |   -   
|  -  |183554|ROUTE| Et11               |1021 |103421  | d0:48:a1:ba:3c:61 |   -   
|  -  |183555|ROUTE| Et5                |1010 |103428  | 18:5b:00:61:ac:6f |   -   
|  -  |183556|ROUTE| Et3                |1008 |103426  | bc:31:e2:e1:ec:2c |   -   
|  -  |183557|ROUTE| Et17               |1016 |103440  | 64:6d:4e:32:e1:22 |   -   
|  -  |183558|ROUTE| Et2                |1007 |103427  | d4:af:f7:2f:13:96 |   -   
|  -  |183559|ROUTE| Et17               |1016 |103496  | 64:6d:4e:32:e1:22 |Mpush 3252
|  -  |183560|ROUTE| Et40               |1020 |103429  | e8:24:a6:96:05:48 |   -   
|  -  |183561|ROUTE| Et15               |1015 |103437  | 30:c5:07:84:3e:79 |   -   
|  -  |183562|ROUTE| Et15               |1015 |103437  | 30:c5:07:84:3e:79 |   -   
|  -  |183563|ROUTE| Et17               |1016 |103425  | 64:6d:4e:32:e1:22 |Mpush 2124
|  -  |183564|ROUTE| Et13               |1014 |103430  | 5c:07:58:a3:0a:aa |Mpush 0
|  -  |183565|ROUTE| Et3                |1008 |103426  | bc:31:e2:e1:ec:2c |   -   
|  -  |183567|ROUTE| Et2                |1007 |103427  | d4:af:f7:2f:13:96 |   -   
|  -  |183568|ROUTE| Et2                |1007 |103427  | d4:af:f7:2f:13:96 |   -   
|  -  |183569|ROUTE| Et12               |1013 |103422  | 58:70:7f:9f:c4:03 |   -   
|  -  |183570|ROUTE| Et19               |1018 |103431  | 60:53:75:13:ba:d8 |   -   
|  -  |183571|ROUTE| Et17               |1016 |103440  | 64:6d:4e:32:e1:22 |   -   
|  -  |183582|ROUTE| Et15               |1015 |103437  | 30:c5:07:84:3e:79 |   -   
|  -  |183583|DROP | DROP               |0    |  -     |                   |   -   
|  -  |183584|ROUTE| Et4                |1009 |103423  | c0:14:b8:21:97:90 |   -   
|  -  |183586|ROUTE| Et13               |1014 |103432  | 5c:07:58:a3:0a:aa |   -   
|  -  |183587|ROUTE| Et12               |1013 |103422  | 58:70:7f:9f:c4:03 |   -   
|  -  |183588|ROUTE| Et2                |1007 |103427  | d4:af:f7:2f:13:96 |   -   
|  -  |183589|ROUTE| Et2                |1007 |103427  | d4:af:f7:2f:13:96 |   -   
|  -  |183590|ROUTE| Et11               |1021 |103421  | d0:48:a1:ba:3c:61 |   -   
|  -  |183592|ROUTE| Et4                |1009 |103423  | c0:14:b8:21:97:90 |   -   
|  -  |183603|ROUTE| Et13               |1014 |103432  | 5c:07:58:a3:0a:aa |   -   
|  -  |183605|ROUTE| Et17               |1016 |103478  | 64:6d:4e:32:e1:22 |Mpush 3253
|  -  |183612|ROUTE| Et7                |1011 |103435  | 00:2c:01:00:00:01 |   -   
|  -  |183615|ROUTE| Et12               |1013 |103422  | 58:70:7f:9f:c4:03 |   -   
|  -  |183616|ROUTE| Et12               |1013 |103422  | 58:70:7f:9f:c4:03 |   -   
|  -  |183617|ROUTE| Et35               |1022 |103424  | 40:a6:b7:94:34:cb |   -   
|  -  |183618|ROUTE| Et40               |1020 |103429  | e8:24:a6:96:05:48 |   -   
|  -  |183619|ROUTE| Et15               |1015 |103437  | 30:c5:07:84:3e:79 |   -   
|  -  |183620|ROUTE| Et11               |1021 |103421  | d0:48:a1:ba:3c:61 |   -   
|  -  |183621|ROUTE| Et3                |1008 |103426  | bc:31:e2:e1:ec:2c |   -   
|  -  |183647|ROUTE| Et19               |1018 |103431  | 60:53:75:13:ba:d8 |   -   
|  -  |183648|ROUTE| Et2                |1007 |103427  | d4:af:f7:2f:13:96 |   -   
|  -  |314666|TRAP | CoppSystemIpBcast  |0    |  -     | BcastReceive      |   -   
|  -  |314667|TRAP | CoppSystemIpUcast  |0    |  -     | Receive           |   -   
|  -  |314669|TRAP | CoppSystemL3LpmOver|0    |  -     | SlowReceive       |   -   
|  -  |314671|TRAP | CoppSystemL3DstMiss|0    |  -     | ArpTrap           |   -   
|  -  |315678|TRAP | CoppSystemL3DstMiss|1007 |1007    | ArpTrap           |   -   
|  -  |315679|TRAP | CoppSystemL3DstMiss|1008 |1008    | ArpTrap           |   -   
|  -  |315680|TRAP | CoppSystemL3DstMiss|1009 |1009    | ArpTrap           |   -   
|  -  |315681|TRAP | CoppSystemL3DstMiss|1010 |1010    | ArpTrap           |   -   
|  -  |315682|TRAP | CoppSystemL3DstMiss|1011 |1011    | ArpTrap           |   -   
|  -  |315684|TRAP | CoppSystemL3DstMiss|1013 |1013    | ArpTrap           |   -   
|  -  |315685|TRAP | CoppSystemL3DstMiss|1014 |1014    | ArpTrap           |   -   
|  -  |315686|TRAP | CoppSystemL3DstMiss|1015 |1015    | ArpTrap           |   -   
|  -  |315687|TRAP | CoppSystemL3DstMiss|1016 |1016    | ArpTrap           |   -   
|  -  |315689|TRAP | CoppSystemL3DstMiss|1018 |1018    | ArpTrap           |   -   
|  -  |315691|TRAP | CoppSystemL3DstMiss|1020 |1020    | ArpTrap           |   -   
|  -  |315692|TRAP | CoppSystemL3DstMiss|1021 |1021    | ArpTrap           |   -   
|  -  |315693|TRAP | CoppSystemL3DstMiss|1022 |1022    | ArpTrap           |   -   

```

