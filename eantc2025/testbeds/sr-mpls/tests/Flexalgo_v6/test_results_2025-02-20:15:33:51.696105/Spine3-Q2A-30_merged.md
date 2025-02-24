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

Uptime: 56 minutes
Total memory: 8099700 kB
Free memory: 5104820 kB

```

## show lldp neighbors

```text
Last table change time   : 0:38:38 ago
Number of table inserts  : 18
Number of table deletes  : 1
Number of table drops    : 0
Number of table age-outs : 0

Port       Neighbor Device ID                   Neighbor Port ID            TTL
--------- ------------------------------------ ---------------------------- ---
Et3        H3C_M1A_120                          Ten-GigabitEthernet0/0/17   121
Et4        Nokia-SR1-217                        1610899524                  121
Et5        Nokia-SXR-214                        ethernet-1/4                120
Et9        Ciena-5134-72                        2                           120
Et11       Juniper-156-PTX10002-36QDD           590                         120
Et12       Ericsson_84_R6678                    5870.7f9f.c403              91 
Et13       Arrcus-53                            swp0                        120
Et15       30c5.0784.3e68                       et-bs/15                    121
Et17       Huawei_124_NetEngine_A816            GigabitEthernet0/2/4        120
Et19       Huawei_128_NetEngine_8000_M14        GigabitEthernet0/5/0        120
Et31       Ciena-8140-66                        2                           120
Et35       Juniper-131-JCNR                     42                          120
Et35       Juniper-131-JCNR                     eno12429                    120
Et36       Arista-Harness3-JP-39.ns.eantc.de    Ethernet6                   120
Et40       Juniper-179-ACX7024                  523                         120
Et46/1     Arista-Harness3-JP-39.ns.eantc.de    Ethernet54/1                120
Ma1        extreme-x460-2                       5                           120

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
Ethernet2       20.30.32.30/24      down       down              1500          
Ethernet3       20.30.120.30/24     up         up                1500          
Ethernet4       20.30.217.30/24     up         up                1500          
Ethernet5       20.30.214.30/24     up         up                1500          
Ethernet7       20.30.184.30/24     up         up                1500          
Ethernet9       20.30.72.30/24      up         up                1500          
Ethernet11      20.30.156.30/24     up         up                1500          
Ethernet12      20.30.84.30/24      up         up                1500          
Ethernet13      20.30.53.30/24      up         up                1500          
Ethernet15      20.30.221.30/24     up         up                1500          
Ethernet17      20.30.124.30/24     up         up                1500          
Ethernet19      20.30.128.30/24     up         up                1500          
Ethernet31      20.30.66.30/24      up         up                1500          
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
Et3       H3C_120               0:01    800.0   9.6%      999    800.0   9.6%
Et4       Nokia                 0:01    800.0   9.6%      999    800.0   9.6%
Et9       Ciena-5134-72 port 2  0:01      0.0   0.0%        0      0.0   0.0%
Et11      Juniper-156 port 590  0:01    800.0   9.6%      999    768.0   9.3%
Et13      Arrcus-53 port swp0   0:01    800.0   9.6%      999    768.0   9.3%
Et31      Ciena-8140-66 port 2  0:01      0.0   0.0%        0      0.0   0.0%
Et35      Juniper-131-JCNR 42   0:01      0.0   0.0%        0      0.0   0.0%
Et40      Juniper-179-ACX7024   0:01    800.0   9.6%      999    768.0   9.3%

Port      Out Kpps
Et3            999
Et4            999
Et11           999
Et13           999
Et40           999
```

## show isis neighbors

```text
 
Instance  VRF      System Id        Type Interface          SNPA              State Hold time   Circuit Id          
IGP       default  Arrcus-53        L2   Ethernet13         P2P               UP    25          00                  
IGP       default  Ciena-8140-66    L2   Ethernet31         P2P               UP    27          03                  
IGP       default  Ciena-5134-72    L2   Ethernet9          P2P               UP    27          02                  
IGP       default  Ericsson_84_R6678 L2   Ethernet12         P2P               UP    24          02                  
IGP       default  H3C_M1A_120      L2   Ethernet3          P2P               UP    23          01                  
IGP       default  0000.0000.0124   L2   Ethernet17         P2P               UP    24          09                  
IGP       default  0000.0000.0128   L2   Ethernet19         P2P               UP    22          09                  
IGP       default  Juniper-131-JCNR L2   Ethernet35         P2P               UP    20          01                  
IGP       default  Juniper-156-PTX10002-36QDD L2   Ethernet11         P2P               UP    18          01                  
IGP       default  Juniper-179-ACX7024 L2   Ethernet40         P2P               UP    18          01                  
IGP       default  Nokia-SR1-217    L2   Ethernet4          P2P               UP    21          00                  
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
    Arista-Spine3-Q2A-30.00-00       825  53908  1136   1165 L2  0000.0000.0030.00-00  <>
      LSP generation remaining wait time: 0 ms
      Time remaining until refresh: 836 s
      NLPID: 0xCC(IPv4) 0x8E(IPv6)
      Hostname: Arista-Spine3-Q2A-30
      Area addresses: 49.0001
      Topology: 2 (IPv6)
      Topology: 0 (IPv4)
      Interface address: 20.30.53.30
      Interface address: 20.30.221.30
      Interface address: 20.30.156.30
      Interface address: 20.30.128.30
      Interface address: 20.30.217.30
      Interface address: 20.30.184.30
      Interface address: 20.30.120.30
      Interface address: 20.30.179.30
      Interface address: 20.30.84.30
      Interface address: 20.30.131.30
      Interface address: 20.30.66.30
      Interface address: 20.30.214.30
      Interface address: 20.30.72.30
      Interface address: 20.30.124.30
      Interface address: 10.0.0.30
      Interface address: 2001:0:30:53::30
      Interface address: 2001:0:30:221::30
      Interface address: 2001:0:30:156::30
      Interface address: 2001:0:30:128::30
      Interface address: 2001:0:30:217::30
      Interface address: 2001:0:30:184::30
      Interface address: 2001:0:30:120::30
      Interface address: 2001:0:30:179::30
      Interface address: 2001:0:30:84::30
      Interface address: 2001:0:30:131::30
      Interface address: 2001:0:30:66::30
      Interface address: 2001:0:30:214::30
      Interface address: 2001:0:30:72::30
      Interface address: 2001:0:30:124::30
      Interface address: 2002::30
      IS Neighbor          : Arrcus-53.00        Metric: 10
        IPv4 Neighbor Address: 20.30.53.53
        IPv4 Interface Address: 20.30.53.30
        Adj-sid: 378528 flags: [L V] weight: 0x0
      IS Neighbor          : Ericsson_84_R6678.00 Metric: 10
        IPv4 Neighbor Address: 20.30.84.84
        IPv4 Interface Address: 20.30.84.30
        Adj-sid: 378530 flags: [L V] weight: 0x0
      IS Neighbor          : 0000.0000.0128.00   Metric: 10
        IPv4 Neighbor Address: 20.30.128.128
        IPv4 Interface Address: 20.30.128.30
      IS Neighbor          : 0000.0000.0124.00   Metric: 10
        IPv4 Neighbor Address: 20.30.124.124
        IPv4 Interface Address: 20.30.124.30
      IS Neighbor (MT-IPv6): Ericsson_84_R6678.00 Metric: 10
        IPv6 Neighbor Address: 2001:0:30:84::175
        Global IPv6 Interface Address: 2001:0:30:84::30
        Adj-sid: 378531 flags: [L V F] weight: 0x0
      Reachability         : 20.30.53.0/24 Metric: 10 Type: 1 Up
      Reachability         : 20.30.221.0/24 Metric: 10 Type: 1 Up
      Reachability         : 20.30.156.0/24 Metric: 10 Type: 1 Up
      Reachability         : 20.30.128.0/24 Metric: 10 Type: 1 Up
      Reachability         : 20.30.217.0/24 Metric: 10 Type: 1 Up
      Reachability         : 20.30.184.0/24 Metric: 10 Type: 1 Up
      Reachability         : 20.30.120.0/24 Metric: 10 Type: 1 Up
      Reachability         : 20.30.179.0/24 Metric: 10 Type: 1 Up
      Reachability         : 20.30.84.0/24 Metric: 10 Type: 1 Up
      Reachability         : 20.30.131.0/24 Metric: 10 Type: 1 Up
      Reachability         : 20.30.66.0/24 Metric: 10 Type: 1 Up
      Reachability         : 20.30.214.0/24 Metric: 10 Type: 1 Up
      Reachability         : 20.30.72.0/24 Metric: 10 Type: 1 Up
      Reachability         : 20.30.124.0/24 Metric: 10 Type: 1 Up
      Reachability         : 10.0.0.30/32 Metric: 0 Type: 1 Up
        SR Prefix-SID: 30 Flags: [N] Algorithm: 0
        SR Prefix-SID: 1158 Flags: [N] Algorithm: 128
        SR Prefix-SID: 1159 Flags: [N] Algorithm: 129
        SR Prefix-SID: 1160 Flags: [N] Algorithm: 130
      Reachability (MT-IPv6): 2001:0:30:53::/64 Metric: 10 Type: 1 Up
      Reachability (MT-IPv6): 2001:0:30:156::/64 Metric: 10 Type: 1 Up
      Reachability (MT-IPv6): 2001:0:30:128::/64 Metric: 10 Type: 1 Up
      Reachability (MT-IPv6): 2001:0:30:217::/64 Metric: 10 Type: 1 Up
      Reachability (MT-IPv6): 2001:0:30:184::/64 Metric: 10 Type: 1 Up
      Reachability (MT-IPv6): 2001:0:30:120::/64 Metric: 10 Type: 1 Up
      Reachability (MT-IPv6): 2001:0:30:179::/64 Metric: 10 Type: 1 Up
      Reachability (MT-IPv6): 2001:0:30:84::/64 Metric: 10 Type: 1 Up
      Reachability (MT-IPv6): 2001:0:30:131::/64 Metric: 10 Type: 1 Up
      Reachability (MT-IPv6): 2001:0:30:66::/64 Metric: 10 Type: 1 Up
      Reachability (MT-IPv6): 2001:0:30:214::/64 Metric: 10 Type: 1 Up
      Reachability (MT-IPv6): 2001:0:30:72::/64 Metric: 10 Type: 1 Up
      Reachability (MT-IPv6): 2001:0:30:124::/64 Metric: 10 Type: 1 Up
      Reachability (MT-IPv6): 2002::30/128 Metric: 10 Type: 1 Up
        SR Prefix-SID: 430 Flags: [N] Algorithm: 0
        SR Prefix-SID: 1558 Flags: [N] Algorithm: 128
        SR Prefix-SID: 1559 Flags: [N] Algorithm: 129
        SR Prefix-SID: 1560 Flags: [N] Algorithm: 130
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
    Arista-Spine3-Q2A-30.00-01       306  26409  1055    925 L2  0000.0000.0030.00-01  <>
      LSP generation remaining wait time: 0 ms
      Time remaining until refresh: 755 s
      IS Neighbor          : Juniper-156-PTX10002-36QDD.00 Metric: 10
        IPv4 Neighbor Address: 20.30.156.156
        IPv4 Interface Address: 20.30.156.30
        Adj-sid: 378540 flags: [L V] weight: 0x0
      IS Neighbor          : Juniper-179-ACX7024.00 Metric: 10
        IPv4 Neighbor Address: 20.30.179.179
        IPv4 Interface Address: 20.30.179.30
        Adj-sid: 378538 flags: [L V] weight: 0x0
      IS Neighbor          : Ciena-8140-66.00    Metric: 10
        IPv4 Neighbor Address: 20.30.66.66
        IPv4 Interface Address: 20.30.66.30
        Adj-sid: 378537 flags: [L V] weight: 0x0
      IS Neighbor          : Ciena-5134-72.00    Metric: 10
        IPv4 Neighbor Address: 20.30.72.72
        IPv4 Interface Address: 20.30.72.30
        Adj-sid: 378536 flags: [L V] weight: 0x0
      IS Neighbor          : 221.00              Metric: 10
        IPv4 Neighbor Address: 20.30.221.221
        IPv4 Interface Address: 20.30.221.30
        Adj-sid: 378542 flags: [L V] weight: 0x0
      IS Neighbor          : H3C_M1A_120.00      Metric: 10
        IPv4 Neighbor Address: 20.30.120.120
        IPv4 Interface Address: 20.30.120.30
        Adj-sid: 378534 flags: [L V] weight: 0x0
      IS Neighbor          : Juniper-131-JCNR.00 Metric: 10
        IPv4 Neighbor Address: 20.30.131.131
        IPv4 Interface Address: 20.30.131.30
        Adj-sid: 378533 flags: [L V] weight: 0x0
      IS Neighbor (MT-IPv6): Arrcus-53.00        Metric: 10
        IPv6 Neighbor Address: 2001:0:30:53::53
        Global IPv6 Interface Address: 2001:0:30:53::30
        Adj-sid: 378529 flags: [L V F] weight: 0x0
      IS Neighbor (MT-IPv6): Juniper-156-PTX10002-36QDD.00 Metric: 10
        IPv6 Neighbor Address: 2001:0:30:156::156
        Global IPv6 Interface Address: 2001:0:30:156::30
        Adj-sid: 378541 flags: [L V F] weight: 0x0
      IS Neighbor (MT-IPv6): Juniper-179-ACX7024.00 Metric: 10
        IPv6 Neighbor Address: 2001:0:30:179::179
        Global IPv6 Interface Address: 2001:0:30:179::30
        Adj-sid: 378539 flags: [L V F] weight: 0x0
      IS Neighbor (MT-IPv6): H3C_M1A_120.00      Metric: 10
        IPv6 Neighbor Address: 2001:0:30:120::120
        Global IPv6 Interface Address: 2001:0:30:120::30
        Adj-sid: 378535 flags: [L V F] weight: 0x0
      IS Neighbor (MT-IPv6): Nokia-SR1-217.00    Metric: 10
        IPv6 Neighbor Address: 2001:0:30:217::217
        Global IPv6 Interface Address: 2001:0:30:217::30
        Adj-sid: 378532 flags: [L V F] weight: 0x0
      Reachability (MT-IPv6): 2001:0:30:221::/64 Metric: 10 Type: 1 Up
    Arrcus-53.00-00             591   9865  1023    620 L2  0000.0000.0053.00-00  <>
      Remaining lifetime received: 1199 s Modified to: 1200 s
      NLPID: 0xCC(IPv4) 0x8E(IPv6)
      Hostname: Arrcus-53
      Area addresses: 49.0001
      Topology: 0 (IPv4)
      Topology: 2 (IPv6)
      Interface address: 10.0.0.53
      Interface address: 2002::53
      IS Neighbor          : Arista-Spine3-Q2A-30.00 Metric: 10
        IPv4 Neighbor Address: 20.30.53.30
        IPv4 Interface Address: 20.30.53.53
        Global IPv6 Interface Address: 2001:0:30:53::53
      IS Neighbor          : Juniper-175-ACX7100-48L.00 Metric: 10
        IPv4 Neighbor Address: 20.53.175.175
        IPv4 Interface Address: 20.53.175.53
        Global IPv6 Interface Address: 2001:0:53:175::53
      IS Neighbor (MT-IPv6): Arista-Spine3-Q2A-30.00 Metric: 10
        IPv4 Interface Address: 20.30.53.53
        Global IPv6 Interface Address: 2001:0:30:53::53
      IS Neighbor (MT-IPv6): Juniper-175-ACX7100-48L.00 Metric: 10
        IPv4 Interface Address: 20.53.175.53
        Global IPv6 Interface Address: 2001:0:53:175::53
      Reachability         : 20.30.53.0/24 Metric: 10 Type: 1 Up
      Reachability         : 20.53.175.0/24 Metric: 10 Type: 1 Up
      Reachability         : 10.0.0.53/32 Metric: 0 Type: 1 Up
        SR Prefix-SID: 53 Flags: [N P E] Algorithm: 0
        SR Prefix-SID: 1181 Flags: [N] Algorithm: 128
        SR Prefix-SID: 1182 Flags: [N] Algorithm: 129
        SR Prefix-SID: 1183 Flags: [N] Algorithm: 130
      Reachability (MT-IPv6): 2001:0:30:53::/64 Metric: 10 Type: 1 Up
      Reachability (MT-IPv6): 2001:0:53:175::/64 Metric: 10 Type: 1 Up
      Reachability (MT-IPv6): 2002::53/128 Metric: 0 Type: 1 Up
        SR Prefix-SID: 453 Flags: [N P E] Algorithm: 0
        SR Prefix-SID: 1581 Flags: [N] Algorithm: 128
        SR Prefix-SID: 1582 Flags: [N] Algorithm: 129
        SR Prefix-SID: 1583 Flags: [N] Algorithm: 130
      Router Capabilities: Router Id: 10.0.0.53 Flags: []
        SR Local Block:
          SRLB Base: 16000 Range: 3001
        SR Capability: Flags: [I V]
          SRGB Base: 20000 Range: 780001
        Algorithms:  0, 128, 129, 130
    Ciena-8140-66.00-00         260  28093   912    469 L2  0000.0000.0066.00-00  <>
      Remaining lifetime received: 1199 s Modified to: 1200 s
      NLPID: 0xCC(IPv4)
      Hostname: Ciena-8140-66
      Area addresses: 49.0001
      Topology: 0 (IPv4)
      Interface address: 10.0.0.66
      IS Neighbor          : Juniper-175-ACX7100-48L.00 Metric: 10
        IPv4 Neighbor Address: 20.66.175.175
        IPv4 Interface Address: 20.66.175.66
        Adj-sid: 16002 flags: [L V] weight: 0x0
      IS Neighbor          : Arista-Spine3-Q2A-30.00 Metric: 10
        IPv4 Neighbor Address: 20.30.66.30
        IPv4 Interface Address: 20.30.66.66
        Adj-sid: 16003 flags: [L V] weight: 0x0
      Reachability         : 10.0.0.66/32 Metric: 10 Type: 1 Up
        SR Prefix-SID: 66 Flags: [N] Algorithm: 0
        SR Prefix-SID: 1194 Flags: [N] Algorithm: 128
        SR Prefix-SID: 1195 Flags: [N] Algorithm: 129
        SR Prefix-SID: 1196 Flags: [N] Algorithm: 130
      Reachability         : 20.66.175.0/24 Metric: 10 Type: 1 Up
      Reachability         : 20.30.66.0/24 Metric: 10 Type: 1 Up
      Router Capabilities: Router Id: 10.0.0.66 Flags: []
        SR Capability: Flags: [I]
          SRGB Base: 20000 Range: 2000
        Algorithms:  0, 128, 129, 130
    Ciena-5134-72.00-00         634  10277   914    469 L2  0000.0000.0072.00-00  <>
      Remaining lifetime received: 1199 s Modified to: 1200 s
      NLPID: 0xCC(IPv4)
      Hostname: Ciena-5134-72
      Area addresses: 49.0001
      Topology: 0 (IPv4)
      Interface address: 10.0.0.72
      IS Neighbor          : Arista-Spine3-Q2A-30.00 Metric: 10
        IPv4 Neighbor Address: 20.30.72.30
        IPv4 Interface Address: 20.30.72.72
        Adj-sid: 16001 flags: [L V] weight: 0x0
      IS Neighbor          : Juniper-175-ACX7100-48L.00 Metric: 10
        IPv4 Neighbor Address: 20.72.175.175
        IPv4 Interface Address: 20.72.175.72
        Adj-sid: 16000 flags: [L V] weight: 0x0
      Reachability         : 10.0.0.72/32 Metric: 10 Type: 1 Up
        SR Prefix-SID: 72 Flags: [N] Algorithm: 0
        SR Prefix-SID: 1200 Flags: [N] Algorithm: 128
        SR Prefix-SID: 1201 Flags: [N] Algorithm: 129
        SR Prefix-SID: 1202 Flags: [N] Algorithm: 130
      Reachability         : 20.72.175.0/24 Metric: 10 Type: 1 Up
      Reachability         : 20.30.72.0/24 Metric: 10 Type: 1 Up
      Router Capabilities: Router Id: 10.0.0.72 Flags: []
        SR Capability: Flags: [I]
          SRGB Base: 20000 Range: 2000
        Algorithms:  0, 128, 129, 130
    Ericsson_84_R6678.00-00       411  29520  1007    324 L2  0000.0000.0084.00-00  <>
      Remaining lifetime received: 1199 s Modified to: 1200 s
      NLPID: 0xCC(IPv4) 0x8E(IPv6)
      Hostname: Ericsson_84_R6678
      Area addresses: 49.0001
      Topology: 0 (IPv4)
      Topology: 2 (IPv6)
      Interface address: 10.0.0.84
      Interface address: 2001:0:30:84::175
      IS Neighbor          : Juniper-175-ACX7100-48L.00 Metric: 10
        IPv4 Interface Address: 20.84.175.84
      IS Neighbor          : Arista-Spine3-Q2A-30.00 Metric: 10
        IPv4 Interface Address: 20.30.84.84
      IS Neighbor (MT-IPv6): Juniper-175-ACX7100-48L.00 Metric: 10
        IPv6 Neighbor Address: 2001:0:84:175::175
        Global IPv6 Interface Address: 2001:0:84:175::175
      IS Neighbor (MT-IPv6): Arista-Spine3-Q2A-30.00 Metric: 10
        IPv6 Neighbor Address: 2001:0:30:84::30
        Global IPv6 Interface Address: 2001:0:30:84::175
      Reachability         : 10.0.0.84/32 Metric: 10 Type: 1 Up
        SR Prefix-SID: 84 Flags: [N P] Algorithm: 0
      Reachability (MT-IPv6): 2001:0:84:175::/64 Metric: 10 Type: 1 Up
      Reachability (MT-IPv6): 2001:0:30:84::/64 Metric: 10 Type: 1 Up
      Router Capabilities: Router Id: 10.0.0.84 Flags: []
        Maximum SID depth:
          Base MPLS imposition (MSD type 1):  8
        SR Capability: Flags: [I]
          SRGB Base: 20000 Range: 2000
        Algorithms:  0
    H3C_M1A_120.00-00          2268  16349   669   1413 L2  0000.0000.0120.00-00  <>
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
      Interface address: 2002::120
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
        Adj-sid: 1139 flags: [L V F] weight: 0x0
      IS Neighbor (MT-IPv6): Juniper-175-ACX7100-48L.00 Metric: 10
        IPv6 Neighbor Address: 2001:0:120:175::175
        Global IPv6 Interface Address: 2001:0:120:175::120
        Adj-sid: 1138 flags: [L V F] weight: 0x0
      IS Neighbor (MT-IPv6): Juniper-175-ACX7100-48L.00 Metric: 10
        IPv6 Neighbor Address: 2001:0:120:175::175
        Global IPv6 Interface Address: 2001:0:120:175::120
      Reachability         : 10.0.0.120/32 Metric: 0 Type: 1 Up
      Reachability         : 20.30.120.0/24 Metric: 100 Type: 1 Up
      Reachability         : 20.120.175.0/24 Metric: 10 Type: 1 Up
      Reachability         : 20.120.214.0/24 Metric: 10 Type: 1 Up
      Reachability         : 20.120.217.0/24 Metric: 0 Type: 1 Up
      Reachability         : 192.168.20.0/23 Metric: 0 Type: 1 Up
      Reachability (MT-IPv6): 2001:0:30:120::/64 Metric: 10 Type: 1 Up
      Reachability (MT-IPv6): 2001:0:120:175::/64 Metric: 10 Type: 1 Up
      Reachability (MT-IPv6): 2001:0:120:214::/64 Metric: 10 Type: 1 Up
      Reachability (MT-IPv6): 2002::120/128 Metric: 0 Type: 1 Up
        SR Prefix-SID: 520 Flags: [N] Algorithm: 0
        SR Prefix-SID: 1648 Flags: [N P] Algorithm: 128
        SR Prefix-SID: 1649 Flags: [N P] Algorithm: 129
        SR Prefix-SID: 1650 Flags: [N P] Algorithm: 130
      Router Capabilities: Router Id: 10.0.0.120 Flags: []
        Maximum SID depth:
          Base MPLS imposition (MSD type 1):  13
        SR Capability: Flags: [I V]
          SRGB Base: 20000 Range: 2000
        Algorithms:  0, 128, 129, 130
        Flex Algo: Algorithm: 128 Metric: Min Unidirectional Delay Metric (1) Calc: SPF (0) Prio: 128
          Flags: [M] 0x80
        Flex Algo: Algorithm: 129 Metric: TE Metric (2) Calc: SPF (0) Prio: 128
          Flags: [M] 0x80
        Flex Algo: Algorithm: 130 Metric: IGP Metric (0) Calc: SPF (0) Prio: 128
          Exclude admin groups: 1
          Flags: [M] 0x80
    H3C_M1A_120.00-01             6  31656   944    189 L2  0000.0000.0120.00-01  <>
      Remaining lifetime received: 1199 s Modified to: 1200 s
      IS Neighbor (MT-IPv6): Arista-Spine3-Q2A-30.00 Metric: 10
        IPv6 Neighbor Address: 2001:0:30:120::30
        Global IPv6 Interface Address: 2001:0:30:120::120
    0000.0000.0124.00-00        273  22250  1052    453 L2  0000.0000.0124.00-00  <>
      Remaining lifetime received: 1199 s Modified to: 1200 s
      NLPID: 0xCC(IPv4) 0x8E(IPv6)
      Area addresses: 49.0001
      Topology: 0 (IPv4)
      Topology: 2 (IPv6)
      Interface address: 20.124.175.124
      Interface address: 10.0.0.124
      Interface address: 20.30.124.124
      IS Neighbor          : Juniper-175-ACX7100-48L.00 Metric: 10
        IPv4 Neighbor Address: 20.124.175.175
        IPv4 Interface Address: 20.124.175.124
        Adj-sid: 398 flags: [L V] weight: 0x0
      IS Neighbor          : Arista-Spine3-Q2A-30.00 Metric: 10
        IPv4 Neighbor Address: 20.30.124.30
        IPv4 Interface Address: 20.30.124.124
        Adj-sid: 397 flags: [L V] weight: 0x0
      Reachability         : 20.124.175.0/24 Metric: 10 Type: 1 Up
      Reachability         : 10.0.0.124/32 Metric: 0 Type: 1 Up
        SR Prefix-SID: 124 Flags: [N P] Algorithm: 0
        SR Prefix-SID: 1252 Flags: [N P] Algorithm: 128
        SR Prefix-SID: 1253 Flags: [N P] Algorithm: 129
        SR Prefix-SID: 1254 Flags: [N P] Algorithm: 130
      Reachability         : 20.30.124.0/24 Metric: 10 Type: 1 Up
      Router Capabilities: Router Id: 10.0.0.124 Flags: []
        Flex Algo: Algorithm: 128 Metric: Min Unidirectional Delay Metric (1) Calc: SPF (0) Prio: 128
          Flags: [M] 0x80
        Flex Algo: Algorithm: 129 Metric: TE Metric (2) Calc: SPF (0) Prio: 128
          Flags: [M] 0x80
        Flex Algo: Algorithm: 130 Metric: IGP Metric (0) Calc: SPF (0) Prio: 128
          Exclude admin groups: 1
          Flags: [M] 0x80
      Router Capabilities: Router Id: 10.0.0.124 Flags: []
        Maximum SID depth:
          Base MPLS imposition (MSD type 1):  10
        SR Capability: Flags: [I]
          SRGB Base: 2000 Range: 2001
        Algorithms:  0, 128, 129, 130
    0000.0000.0128.00-00        287  54684   327    453 L2  0000.0000.0128.00-00  <>
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
        Adj-sid: 48123 flags: [L V] weight: 0x0
      IS Neighbor          : Arista-Spine3-Q2A-30.00 Metric: 10
        IPv4 Neighbor Address: 20.30.128.30
        IPv4 Interface Address: 20.30.128.128
        Adj-sid: 48122 flags: [L V] weight: 0x0
      Reachability         : 10.0.0.128/32 Metric: 0 Type: 1 Up
        SR Prefix-SID: 128 Flags: [N] Algorithm: 0
        SR Prefix-SID: 1256 Flags: [N] Algorithm: 128
        SR Prefix-SID: 1257 Flags: [N] Algorithm: 129
        SR Prefix-SID: 1258 Flags: [N] Algorithm: 130
      Reachability         : 20.128.175.0/24 Metric: 10 Type: 1 Up
      Reachability         : 20.30.128.0/24 Metric: 10 Type: 1 Up
      Router Capabilities: Router Id: 10.0.0.128 Flags: []
        Flex Algo: Algorithm: 128 Metric: Min Unidirectional Delay Metric (1) Calc: SPF (0) Prio: 128
          Flags: [M] 0x80
        Flex Algo: Algorithm: 129 Metric: TE Metric (2) Calc: SPF (0) Prio: 128
          Flags: [M] 0x80
        Flex Algo: Algorithm: 130 Metric: IGP Metric (0) Calc: SPF (0) Prio: 128
          Exclude admin groups: 1
          Flags: [M] 0x80
      Router Capabilities: Router Id: 10.0.0.128 Flags: []
        Maximum SID depth:
          Base MPLS imposition (MSD type 1):  10
        SR Capability: Flags: [I]
          SRGB Base: 20000 Range: 2000
        Algorithms:  0, 128, 129, 130
    Juniper-131-JCNR.00-00       135  22868   491    447 L2  0000.0000.0131.00-00  <>
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
        Adj-sid: 25 flags: [L V F] weight: 0x0
        Adj-sid: 24 flags: [L V] weight: 0x0
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
    Juniper-156-PTX10002-36QDD.00-00       190  60111  1041    870 L2  0000.0000.0156.00-00  <>
      Remaining lifetime received: 1198 s Modified to: 1200 s
      NLPID: 0xCC(IPv4) 0x8E(IPv6)
      Hostname: Juniper-156-PTX10002-36QDD
      Area addresses: 49.0001
      Topology: 0 (IPv4)
      Topology: 2 (IPv6)
      Interface address: 10.0.0.156
      Interface address: 2002::156
      IS Neighbor          : Arista-Spine3-Q2A-30.00 Metric: 4000
        IPv4 Neighbor Address: 20.30.156.30
        IPv4 Interface Address: 20.30.156.156
        IPv6 Neighbor Address: 2001:0:30:156::30
        Global IPv6 Interface Address: 2001:0:30:156::156
        Adj-sid: 22 flags: [L V] weight: 0x0
      IS Neighbor          : Juniper-175-ACX7100-48L.00 Metric: 10
        IPv4 Neighbor Address: 20.156.175.175
        IPv4 Interface Address: 20.156.175.156
        IPv6 Neighbor Address: 2001:0:156:175::175
        Global IPv6 Interface Address: 2001:0:156:175::156
        Adj-sid: 19 flags: [L V F] weight: 0x0
        Adj-sid: 18 flags: [L V] weight: 0x0
      IS Neighbor (MT-IPv6): Arista-Spine3-Q2A-30.00 Metric: 10
        IPv4 Interface Address: 20.30.156.156
        IPv6 Neighbor Address: 2001:0:30:156::30
        Global IPv6 Interface Address: 2001:0:30:156::156
        Adj-sid: 23 flags: [L V F] weight: 0x0
      IS Neighbor (MT-IPv6): Juniper-175-ACX7100-48L.00 Metric: 10
        IPv4 Interface Address: 20.156.175.156
        IPv6 Neighbor Address: 2001:0:156:175::175
        Global IPv6 Interface Address: 2001:0:156:175::156
        Adj-sid: 19 flags: [L V F] weight: 0x0
      Reachability         : 10.0.0.156/32 Metric: 0 Type: 1 Up
        SR Prefix-SID: 156 Flags: [N] Algorithm: 0
        SR Prefix-SID: 1286 Flags: [N] Algorithm: 130
        SR Prefix-SID: 1285 Flags: [N] Algorithm: 129
        SR Prefix-SID: 1284 Flags: [N] Algorithm: 128
      Reachability         : 20.156.175.0/24 Metric: 10 Type: 1 Up
      Reachability         : 20.30.156.0/24 Metric: 4000 Type: 1 Up
      Reachability (MT-IPv6): 2002::156/128 Metric: 0 Type: 1 Up
        SR Prefix-SID: 556 Flags: [N] Algorithm: 0
        SR Prefix-SID: 1686 Flags: [N] Algorithm: 130
        SR Prefix-SID: 1685 Flags: [N] Algorithm: 129
        SR Prefix-SID: 1684 Flags: [N] Algorithm: 128
      Reachability (MT-IPv6): 2001:0:156:175::/64 Metric: 10 Type: 1 Up
      Reachability (MT-IPv6): 2001:0:30:156::/64 Metric: 10 Type: 1 Up
      Router Capabilities: Router Id: 10.0.0.156 Flags: []
        Maximum SID depth:
          Base MPLS imposition (MSD type 1):  0
        SR Capability: Flags: [I V]
          SRGB Base: 20000 Range: 2000
        Algorithms:  0, 1, 128, 129, 130
      Unsupported TLV: Type: 14 Length: 2
    Juniper-175-ACX7100-48L.00-00       428  47015  1183   1244 L2  0000.0000.0175.00-00  <>
      Remaining lifetime received: 1198 s Modified to: 1200 s
      NLPID: 0xCC(IPv4) 0x8E(IPv6)
      Hostname: Juniper-175-ACX7100-48L
      Area addresses: 49.0001
      Topology: 0 (IPv4)
      Topology: 2 (IPv6)
      Interface address: 10.0.0.175
      Interface address: 127.0.0.1
      Interface address: 2002::175
      IS Neighbor          : Juniper-131-JCNR.00 Metric: 15
        IPv4 Neighbor Address: 20.131.175.131
        IPv4 Interface Address: 20.131.175.175
        IPv6 Neighbor Address: 2001:0:131:175::131
        Global IPv6 Interface Address: 2001:0:131:175::175
        Adj-sid: 116 flags: [L V F] weight: 0x0
        Adj-sid: 115 flags: [L V] weight: 0x0
      IS Neighbor          : Ciena-5134-72.00    Metric: 15
        IPv4 Neighbor Address: 20.72.175.72
        IPv4 Interface Address: 20.72.175.175
        Global IPv6 Interface Address: 2001:0:72:175::175
        Adj-sid: 123 flags: [L V] weight: 0x0
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
      IS Neighbor (MT-IPv6): Nokia-SR1-217.00    Metric: 10
        IPv4 Interface Address: 20.175.217.175
        IPv6 Neighbor Address: 2001:0:175:217::217
        Global IPv6 Interface Address: 2001:0:175:217::175
        Adj-sid: 98 flags: [L V F] weight: 0x0
      Reachability         : 20.131.175.0/24 Metric: 15 Type: 1 Up
      Reachability         : 20.128.175.0/24 Metric: 15 Type: 1 Up
      Reachability         : 20.175.184.0/24 Metric: 15 Type: 1 Up
      Reachability         : 20.175.214.0/24 Metric: 15 Type: 1 Up
      Reachability         : 20.175.179.0/24 Metric: 15 Type: 1 Up
      Reachability         : 20.120.175.0/24 Metric: 15 Type: 1 Up
      Reachability         : 127.0.0.1/32 Metric: 0 Type: 1 Up
      Reachability         : 10.0.0.175/32 Metric: 0 Type: 1 Up
        SR Prefix-SID: 175 Flags: [N] Algorithm: 0
        SR Prefix-SID: 1305 Flags: [N] Algorithm: 130
        SR Prefix-SID: 1304 Flags: [N] Algorithm: 129
        SR Prefix-SID: 1303 Flags: [N] Algorithm: 128
      Reachability         : 20.66.175.0/24 Metric: 15 Type: 1 Up
      Reachability         : 20.72.175.0/24 Metric: 15 Type: 1 Up
      Reachability         : 20.175.221.0/24 Metric: 15 Type: 1 Up
      Reachability         : 20.124.175.0/24 Metric: 15 Type: 1 Up
      Reachability         : 20.156.175.0/24 Metric: 10 Type: 1 Up
      Reachability         : 20.84.175.0/24 Metric: 15 Type: 1 Up
      Reachability         : 20.175.217.0/24 Metric: 15 Type: 1 Up
      Reachability         : 20.53.175.0/24 Metric: 15 Type: 1 Up
      Reachability (MT-IPv6): 2002::175/128 Metric: 0 Type: 1 Up
        SR Prefix-SID: 575 Flags: [N] Algorithm: 0
        SR Prefix-SID: 1705 Flags: [N] Algorithm: 130
        SR Prefix-SID: 1704 Flags: [N] Algorithm: 129
        SR Prefix-SID: 1703 Flags: [N] Algorithm: 128
      Reachability (MT-IPv6): 2001:0:156:175::/64 Metric: 10 Type: 1 Up
      Reachability (MT-IPv6): 2001:0:175:184::/64 Metric: 10 Type: 1 Up
      Reachability (MT-IPv6): 2001:0:66:175::/64 Metric: 10 Type: 1 Up
      Reachability (MT-IPv6): 2001:0:72:175::/64 Metric: 10 Type: 1 Up
      Reachability (MT-IPv6): 2001:0:175::/64 Metric: 10 Type: 1 Up
      Reachability (MT-IPv6): 2001:0:175:214::/64 Metric: 10 Type: 1 Up
      Reachability (MT-IPv6): 2001:0:128:175::/64 Metric: 10 Type: 1 Up
      Reachability (MT-IPv6): 2001:0:84:175::/64 Metric: 10 Type: 1 Up
      Reachability (MT-IPv6): 2001:0:175:217::/64 Metric: 10 Type: 1 Up
      Reachability (MT-IPv6): 2001:0:53:175::/64 Metric: 10 Type: 1 Up
      Router Capabilities: Router Id: 10.0.0.175 Flags: []
        Maximum SID depth:
          Base MPLS imposition (MSD type 1):  3
        SR Capability: Flags: [I V]
          SRGB Base: 20000 Range: 2000
        Algorithms:  0, 1, 128, 129, 130
        Flex Algo: Algorithm: 130 Metric: IGP Metric (0) Calc: SPF (0) Prio: 0
          Exclude admin groups: 1
          Flags: [M] 0x80
        Flex Algo: Algorithm: 129 Metric: TE Metric (2) Calc: SPF (0) Prio: 238
          Flags: [M] 0x80
        Flex Algo: Algorithm: 128 Metric: Min Unidirectional Delay Metric (1) Calc: SPF (0) Prio: 0
          Flags: [M] 0x80
      Unsupported TLV: Type: 14 Length: 2
    Juniper-175-ACX7100-48L.00-01       335  16436  1179   1244 L2  0000.0000.0175.00-01  <>
      Remaining lifetime received: 1196 s Modified to: 1200 s
      IS Neighbor          : 221.00              Metric: 15
        IPv4 Neighbor Address: 20.175.221.221
        IPv4 Interface Address: 20.175.221.175
        Global IPv6 Interface Address: 2001:0:175:221::175
        Adj-sid: 127 flags: [L V F] weight: 0x0
        Adj-sid: 126 flags: [L V] weight: 0x0
      IS Neighbor          : Ericsson_84_R6678.00 Metric: 15
        IPv4 Neighbor Address: 20.84.175.84
        IPv4 Interface Address: 20.84.175.175
        IPv6 Neighbor Address: 2001:0:84:175::175
        Global IPv6 Interface Address: 2001:0:84:175::175
        Adj-sid: 132 flags: [L V F] weight: 0x0
        Adj-sid: 131 flags: [L V] weight: 0x0
      IS Neighbor          : 0000.0000.0128.00   Metric: 15
        IPv4 Neighbor Address: 20.128.175.128
        IPv4 Interface Address: 20.128.175.175
        Global IPv6 Interface Address: 2001:0:128:175::175
        Adj-sid: 96 flags: [L V] weight: 0x0
      IS Neighbor          : Keysight-184.00     Metric: 15
        IPv4 Neighbor Address: 20.175.184.184
        IPv4 Interface Address: 20.175.184.175
        Global IPv6 Interface Address: 2001:0:175:184::175
        Adj-sid: 138 flags: [L V] weight: 0x0
      IS Neighbor          : 0000.0000.0124.00   Metric: 15
        IPv4 Neighbor Address: 20.124.175.124
        IPv4 Interface Address: 20.124.175.175
        Adj-sid: 128 flags: [L V] weight: 0x0
      IS Neighbor          : Ciena-8140-66.00    Metric: 15
        IPv4 Neighbor Address: 20.66.175.66
        IPv4 Interface Address: 20.66.175.175
        Global IPv6 Interface Address: 2001:0:66:175::175
        Adj-sid: 122 flags: [L V] weight: 0x0
      IS Neighbor          : Juniper-156-PTX10002-36QDD.00 Metric: 10
        IPv4 Neighbor Address: 20.156.175.156
        IPv4 Interface Address: 20.156.175.175
        IPv6 Neighbor Address: 2001:0:156:175::156
        Global IPv6 Interface Address: 2001:0:156:175::175
        Adj-sid: 130 flags: [L V F] weight: 0x0
        Adj-sid: 129 flags: [L V] weight: 0x0
      IS Neighbor          : Nokia-SXR-214.00    Metric: 15
        IPv4 Interface Address: 20.175.214.175
        IPv6 Neighbor Address: 2001:0:175:214::214
        Global IPv6 Interface Address: 2001:0:175:214::175
        Adj-sid: 108 flags: [L V F] weight: 0x0
      IS Neighbor (MT-IPv6): Keysight-184.00     Metric: 10
        IPv4 Interface Address: 20.175.184.175
        Global IPv6 Interface Address: 2001:0:175:184::175
        Adj-sid: 139 flags: [L V F] weight: 0x0
      IS Neighbor (MT-IPv6): 221.00              Metric: 10
        IPv4 Interface Address: 20.175.221.175
        Global IPv6 Interface Address: 2001:0:175:221::175
        Adj-sid: 127 flags: [L V F] weight: 0x0
    Juniper-175-ACX7100-48L.00-02        28  26640  1183    893 L2  0000.0000.0175.00-02  <>
      Remaining lifetime received: 1198 s Modified to: 1200 s
      IS Neighbor          : Arrcus-53.00        Metric: 15
        IPv4 Neighbor Address: 20.53.175.53
        IPv4 Interface Address: 20.53.175.175
        IPv6 Neighbor Address: 2001:0:53:175::53
        Global IPv6 Interface Address: 2001:0:53:175::175
        Adj-sid: 99 flags: [L V] weight: 0x0
      IS Neighbor (MT-IPv6): Ericsson_84_R6678.00 Metric: 10
        IPv4 Interface Address: 20.84.175.175
        IPv6 Neighbor Address: 2001:0:84:175::175
        Global IPv6 Interface Address: 2001:0:84:175::175
        Adj-sid: 132 flags: [L V F] weight: 0x0
      IS Neighbor (MT-IPv6): Juniper-179-ACX7024.00 Metric: 10
        IPv4 Interface Address: 20.175.179.175
        IPv6 Neighbor Address: 2001:0:175::179:179
        Global IPv6 Interface Address: 2001:0:175::179:175
        Adj-sid: 106 flags: [L V F] weight: 0x0
      IS Neighbor (MT-IPv6): Juniper-156-PTX10002-36QDD.00 Metric: 10
        IPv4 Interface Address: 20.156.175.175
        IPv6 Neighbor Address: 2001:0:156:175::156
        Global IPv6 Interface Address: 2001:0:156:175::175
        Adj-sid: 130 flags: [L V F] weight: 0x0
      IS Neighbor (MT-IPv6): H3C_M1A_120.00      Metric: 10
        IPv4 Interface Address: 20.120.175.175
        IPv6 Neighbor Address: 2001:0:120:175::120
        Global IPv6 Interface Address: 2001:0:120:175::175
        Adj-sid: 110 flags: [L V F] weight: 0x0
      IS Neighbor (MT-IPv6): Arrcus-53.00        Metric: 10
        IPv4 Interface Address: 20.53.175.175
        IPv6 Neighbor Address: 2001:0:53:175::53
        Global IPv6 Interface Address: 2001:0:53:175::175
        Adj-sid: 133 flags: [L V F] weight: 0x0
      Reachability (MT-IPv6): 2001:0:175:221::/64 Metric: 10 Type: 1 Up
      Reachability (MT-IPv6): 2001:0:120:175::/64 Metric: 10 Type: 1 Up
      Reachability (MT-IPv6): 2001:0:131:175::/64 Metric: 10 Type: 1 Up
    Juniper-179-ACX7024.00-00       304  39781  1002    873 L2  0000.0000.0179.00-00  <>
      Remaining lifetime received: 1198 s Modified to: 1200 s
      NLPID: 0xCC(IPv4) 0x8E(IPv6)
      Hostname: Juniper-179-ACX7024
      Area addresses: 49.0001
      Topology: 0 (IPv4)
      Topology: 2 (IPv6)
      Interface address: 10.0.0.179
      Interface address: 127.0.0.1
      Interface address: 10.0.1.179
      IS Neighbor          : Juniper-175-ACX7100-48L.00 Metric: 10
        IPv4 Neighbor Address: 20.175.179.175
        IPv4 Interface Address: 20.175.179.179
        IPv6 Neighbor Address: 2001:0:175::179:175
        Global IPv6 Interface Address: 2001:0:175::179:179
        Adj-sid: 20 flags: [L V F] weight: 0x0
        Adj-sid: 19 flags: [L V] weight: 0x0
      IS Neighbor          : Arista-Spine3-Q2A-30.00 Metric: 4000
        IPv4 Neighbor Address: 20.30.179.30
        IPv4 Interface Address: 20.30.179.179
        IPv6 Neighbor Address: 2001:0:30:179::30
        Global IPv6 Interface Address: 2001:0:30:179::179
        Adj-sid: 23 flags: [L V] weight: 0x0
      IS Neighbor (MT-IPv6): Juniper-175-ACX7100-48L.00 Metric: 10
        IPv4 Interface Address: 20.175.179.179
        IPv6 Neighbor Address: 2001:0:175::179:175
        Global IPv6 Interface Address: 2001:0:175::179:179
        Adj-sid: 20 flags: [L V F] weight: 0x0
      IS Neighbor (MT-IPv6): Arista-Spine3-Q2A-30.00 Metric: 10
        IPv4 Interface Address: 20.30.179.179
        IPv6 Neighbor Address: 2001:0:30:179::30
        Global IPv6 Interface Address: 2001:0:30:179::179
        Adj-sid: 24 flags: [L V F] weight: 0x0
      Reachability         : 10.0.0.179/32 Metric: 0 Type: 1 Up
        SR Prefix-SID: 179 Flags: [N] Algorithm: 0
        SR Prefix-SID: 1309 Flags: [N] Algorithm: 130
        SR Prefix-SID: 1308 Flags: [N] Algorithm: 129
        SR Prefix-SID: 1307 Flags: [N] Algorithm: 128
      Reachability         : 20.175.179.0/24 Metric: 10 Type: 1 Up
      Reachability         : 127.0.0.1/32 Metric: 0 Type: 1 Up
      Reachability         : 10.0.1.179/32 Metric: 0 Type: 1 Up
      Reachability         : 20.30.179.0/24 Metric: 4000 Type: 1 Up
      Reachability (MT-IPv6): 2001:0:175::/64 Metric: 10 Type: 1 Up
      Reachability (MT-IPv6): 2002::179/128 Metric: 0 Type: 1 Up
        SR Prefix-SID: 579 Flags: [N] Algorithm: 0
        SR Prefix-SID: 1709 Flags: [N] Algorithm: 130
        SR Prefix-SID: 1708 Flags: [N] Algorithm: 129
        SR Prefix-SID: 1707 Flags: [N] Algorithm: 128
      Reachability (MT-IPv6): 2001:0:30:179::/64 Metric: 10 Type: 1 Up
      Router Capabilities: Router Id: 10.0.0.179 Flags: []
        Maximum SID depth:
          Base MPLS imposition (MSD type 1):  8
        SR Capability: Flags: [I V]
          SRGB Base: 20000 Range: 2000
        Algorithms:  0, 1, 128, 129, 130
      Unsupported TLV: Type: 14 Length: 2
    Keysight-184.00-00          203  21258   656    485 L2  0000.0000.0184.00-00  <DefaultAtt>
      Remaining lifetime received: 1193 s Modified to: 1200 s
      NLPID: 0xCC(IPv4) 0x8E(IPv6) 0x81(CLNP)
      Hostname: Keysight-184
      Area addresses: 49.0001
      Topology: 0 (IPv4), attached
      Topology: 2 (IPv6)
      Interface address: 20.175.184.184
      Interface address: 2001:0:175:184::184
      IS Neighbor          : Juniper-175-ACX7100-48L.00 Metric: 10
        Adj-sid: 9001 flags: [L V F] weight: 0x0
      IS Neighbor (MT-IPv6): Juniper-175-ACX7100-48L.00 Metric: 10
        Adj-sid: 9001 flags: [L V F] weight: 0x0
      Reachability         : 20.175.184.0/24 Metric: 10 Type: 1 Up
      Reachability          : 2001:0:175:184::/64 Metric: 10 Type: 1 Up
      Reachability          : 2002::184/128 Metric: 0 Type: 1 Up
        SR Prefix-SID: 584 Flags: [N] Algorithm: 0
        SR Prefix-SID: 1712 Flags: [N] Algorithm: 128
        SR Prefix-SID: 1713 Flags: [N] Algorithm: 129
        SR Prefix-SID: 1714 Flags: [N] Algorithm: 130
      Reachability (MT-IPv6): 2001:0:175:184::/64 Metric: 10 Type: 1 Up
      Reachability (MT-IPv6): 2002::184/128 Metric: 0 Type: 1 Up
        SR Prefix-SID: 584 Flags: [N] Algorithm: 0
        SR Prefix-SID: 1712 Flags: [N] Algorithm: 128
        SR Prefix-SID: 1713 Flags: [N] Algorithm: 129
        SR Prefix-SID: 1714 Flags: [N] Algorithm: 130
      Router Capabilities: Router Id: 10.0.0.184 Flags: []
        Algorithms:  0, 128, 129, 130
    Nokia-SXR-214.00-00        8965  35230   851    382 L2  0000.0000.0214.00-00  <>
      Remaining lifetime received: 1198 s Modified to: 1200 s
      NLPID: 0xCC(IPv4) 0x8E(IPv6)
      Hostname: Nokia-SXR-214
      Area addresses: 49.0001
      Interface address: 20.214.216.214
      Interface address: 2000::214
      Interface address: 2001:0:175:214::214
      Interface address: 2001:0:214:216::214
      IS Neighbor          : Nokia-IXRe2-216.00  Metric: 10
        IPv4 Neighbor Address: 20.214.216.216
        IPv4 Interface Address: 20.214.216.214
        IPv6 Neighbor Address: 2001:0:214:216::216
        Global IPv6 Interface Address: 2001:0:214:216::214
        Adj-sid: 30021 flags: [L V B] weight: 0x0
        Adj-sid: 30022 flags: [L V B F] weight: 0x0
      IS Neighbor          : Juniper-175-ACX7100-48L.00 Metric: 10
        IPv6 Neighbor Address: 2001:0:175:214::175
        Global IPv6 Interface Address: 2001:0:175:214::214
        Adj-sid: 30023 flags: [L V B] weight: 0x0
        Adj-sid: 30024 flags: [L V B F] weight: 0x0
      Reachability         : 20.214.216.0/24 Metric: 10 Type: 1 Up
      Reachability          : 2000::214/128 Metric: 0 Type: 1 Up
      Reachability          : 2001:0:175:214::/64 Metric: 10 Type: 1 Up
      Reachability          : 2001:0:214:216::/64 Metric: 10 Type: 1 Up
      Router Capabilities: Router Id: 0.0.0.0 Flags: []
        Maximum SID depth:
          Base MPLS imposition (MSD type 1):  15
        SR Capability: Flags: [I V]
          SRGB Base: 20000 Range: 2000
        Algorithms:  0
    Nokia-IXRe2-216.00-00      1152  25697   821    435 L2  0100.0000.0216.00-00  <>
      Remaining lifetime received: 1198 s Modified to: 1200 s
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
    Nokia-SR1-217.00-00         536  58703   827    768 L2  0100.0000.0217.00-00  <>
      NLPID: 0xCC(IPv4) 0x8E(IPv6)
      Hostname: Nokia-SR1-217
      Area addresses: 49.0001.0000.0000.0217.00
      Topology: 0 (IPv4)
      Topology: 2 (IPv6)
      Interface address: 10.0.0.217
      Interface address: 2001:0:30:217::217
      Interface address: 2001:0:175:217::217
      Interface address: 2002::217
      IS Neighbor          : Juniper-175-ACX7100-48L.00 Metric: 10
        IPv6 Neighbor Address: 2001:0:175:217::175
        Global IPv6 Interface Address: 2001:0:175:217::217
        Adj-sid: 524283 flags: [L V B] weight: 0x0
      IS Neighbor          : Arista-Spine3-Q2A-30.00 Metric: 10
        IPv6 Neighbor Address: 2001:0:30:217::30
        Global IPv6 Interface Address: 2001:0:30:217::217
        Adj-sid: 524286 flags: [L V B] weight: 0x0
      IS Neighbor (MT-IPv6): Juniper-175-ACX7100-48L.00 Metric: 10
        IPv6 Neighbor Address: 2001:0:175:217::175
        Global IPv6 Interface Address: 2001:0:175:217::217
        Adj-sid: 524281 flags: [L V B F] weight: 0x0
      IS Neighbor (MT-IPv6): Arista-Spine3-Q2A-30.00 Metric: 10
        IPv6 Neighbor Address: 2001:0:30:217::30
        Global IPv6 Interface Address: 2001:0:30:217::217
        Adj-sid: 524285 flags: [L V B F] weight: 0x0
      Reachability         : 10.0.0.217/32 Metric: 0 Type: 1 Up
        SR Prefix-SID: 217 Flags: [N P] Algorithm: 0
        SR Prefix-SID: 1345 Flags: [N P] Algorithm: 128
        SR Prefix-SID: 1346 Flags: [N P] Algorithm: 129
        SR Prefix-SID: 1347 Flags: [N P] Algorithm: 130
      Reachability (MT-IPv6): 2001:0:30:217::/64 Metric: 10 Type: 1 Up
      Reachability (MT-IPv6): 2001:0:175:217::/64 Metric: 10 Type: 1 Up
      Reachability (MT-IPv6): 2002::217/128 Metric: 0 Type: 1 Up
        SR Prefix-SID: 617 Flags: [N P] Algorithm: 0
        SR Prefix-SID: 1745 Flags: [N P] Algorithm: 128
        SR Prefix-SID: 1746 Flags: [N P] Algorithm: 129
        SR Prefix-SID: 1747 Flags: [N P] Algorithm: 130
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
    221.00-00                   291  24669  1054     86 L2  0221.0221.0221.00-00  <>
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
    221.00-01                   248  60809   822     32 L2  0221.0221.0221.00-01  <>
      Hostname: 221
    221.00-02                  7041  10353  1180    541 L2  0221.0221.0221.00-02  <>
      Interface address: 10.0.0.221
      Interface address: 20.175.221.221
      Interface address: 20.30.221.221
      Interface address: 30.66.221.221
      Interface address: 1221::1
      Interface address: 2001:0:175:221::221
      Interface address: 2001:0:30:221::221
      Interface address: 2003:0:66:221::221
      IS Neighbor          : Juniper-175-ACX7100-48L.00 Metric: 10
        IPv4 Neighbor Address: 20.175.221.175
        IPv4 Interface Address: 20.175.221.221
        Adj-sid: 524294 flags: [L V B] weight: 0x0
        Adj-sid: 524289 flags: [L V] weight: 0x0
      IS Neighbor          : Arista-Spine3-Q2A-30.00 Metric: 100
        IPv4 Neighbor Address: 20.30.221.30
        IPv4 Interface Address: 20.30.221.221
        Adj-sid: 524298 flags: [L V B] weight: 0x0
        Adj-sid: 524292 flags: [L V] weight: 0x0
      Reachability         : 10.0.0.221/32 Metric: 0 Type: 1 Up
        SR Prefix-SID: 221 Flags: [N] Algorithm: 0
        SR Prefix-SID: 1349 Flags: [N] Algorithm: 128
        SR Prefix-SID: 1350 Flags: [N] Algorithm: 129
        SR Prefix-SID: 1351 Flags: [N] Algorithm: 130
      Reachability         : 20.175.221.0/24 Metric: 10 Type: 1 Up
      Reachability         : 20.30.221.0/24 Metric: 100 Type: 1 Up
      Reachability         : 30.66.221.0/24 Metric: 10 Type: 1 Up
      Reachability          : 1221::1/128 Metric: 0 Type: 1 Up
      Reachability          : 2001:0:175:221::/64 Metric: 10 Type: 1 Up
      Reachability          : 2001:0:30:221::/64 Metric: 100 Type: 1 Up
      Reachability          : 2003:0:66:221::/64 Metric: 10 Type: 1 Up

```

## show isis flex-algo

```text

IS-IS Instance: IGP VRF: default

Algorithm   Advertised Level Metric    Selected            
----------- ---------- ----- --------- --------------------
MIN-LATENCY yes        L2    min-delay Arista-Spine3-Q2A-30
MIN-TE      yes        L2    TE        Arista-Spine3-Q2A-30
ADMIN       yes        L2    default   Arista-Spine3-Q2A-30

```

## show isis flex-algo path detail

```text
Flex algo paths for IPv4 address family
Topology ID: Level-2
Destination: 221
Path ID: 640
Path constraints: algo MIN-LATENCY
                  metric type MIN-DELAY
Request sequence number: 0
Response sequence number: 0
Number of times path updated: 6
Last updated: 0:02:25 ago
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
Number of times path updated: 6
Last updated: 0:49:05 ago
Metric: 100
Next Hop      Interface 
------------- ----------
20.30.221.221 Ethernet15

Destination: 221
Path ID: 642
Path constraints: algo ADMIN
                  metric type IGP
                  administrative-group exclude 1
Request sequence number: 0
Response sequence number: 0
Number of times path updated: 2
Last updated: 0:49:05 ago
Metric: 10
Next Hop      Interface 
------------- ----------
20.30.221.221 Ethernet15

Destination: Arista-Spine3-Q2A-30
Path ID: 640
Path constraints: algo MIN-LATENCY
                  metric type MIN-DELAY
Request sequence number: 0
Response sequence number: 0
Number of times path updated: 1
Last updated: 0:53:05 ago
Next Hop Interface
-------- ---------

Destination: Arista-Spine3-Q2A-30
Path ID: 641
Path constraints: algo MIN-TE
                  metric type TE
Request sequence number: 0
Response sequence number: 0
Number of times path updated: 1
Last updated: 0:53:05 ago
Next Hop Interface
-------- ---------

Destination: Arista-Spine3-Q2A-30
Path ID: 642
Path constraints: algo ADMIN
                  metric type IGP
                  administrative-group exclude 1
Request sequence number: 0
Response sequence number: 0
Number of times path updated: 1
Last updated: 0:53:05 ago
Next Hop Interface
-------- ---------

Destination: Arrcus-53
Path ID: 640
Path constraints: algo MIN-LATENCY
                  metric type MIN-DELAY
Request sequence number: 0
Response sequence number: 0
Number of times path updated: 7
Last updated: 0:02:25 ago
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
Number of times path updated: 4
Last updated: 0:11:18 ago
Metric: 100
Next Hop    Interface 
----------- ----------
20.30.53.53 Ethernet13

Destination: Arrcus-53
Path ID: 642
Path constraints: algo ADMIN
                  metric type IGP
                  administrative-group exclude 1
Request sequence number: 0
Response sequence number: 0
Number of times path updated: 4
Last updated: 0:11:18 ago
Metric: 10
Next Hop    Interface 
----------- ----------
20.30.53.53 Ethernet13

Destination: Ciena-5134-72
Path ID: 640
Path constraints: algo MIN-LATENCY
                  metric type MIN-DELAY
Request sequence number: 0
Response sequence number: 0
Number of times path updated: 5
Last updated: 0:02:25 ago
Metric: 10000
Next Hop    Interface
----------- ---------
20.30.72.72 Ethernet9

Destination: Ciena-5134-72
Path ID: 641
Path constraints: algo MIN-TE
                  metric type TE
Request sequence number: 0
Response sequence number: 0
Number of times path updated: 4
Last updated: 0:49:52 ago
Metric: 100
Next Hop    Interface
----------- ---------
20.30.72.72 Ethernet9

Destination: Ciena-5134-72
Path ID: 642
Path constraints: algo ADMIN
                  metric type IGP
                  administrative-group exclude 1
Request sequence number: 0
Response sequence number: 0
Number of times path updated: 2
Last updated: 0:49:52 ago
Metric: 10
Next Hop    Interface
----------- ---------
20.30.72.72 Ethernet9

Destination: Ciena-8140-66
Path ID: 640
Path constraints: algo MIN-LATENCY
                  metric type MIN-DELAY
Request sequence number: 0
Response sequence number: 0
Number of times path updated: 5
Last updated: 0:02:25 ago
Metric: 10000
Next Hop    Interface 
----------- ----------
20.30.66.66 Ethernet31

Destination: Ciena-8140-66
Path ID: 641
Path constraints: algo MIN-TE
                  metric type TE
Request sequence number: 0
Response sequence number: 0
Number of times path updated: 4
Last updated: 0:49:52 ago
Metric: 100
Next Hop    Interface 
----------- ----------
20.30.66.66 Ethernet31

Destination: Ciena-8140-66
Path ID: 642
Path constraints: algo ADMIN
                  metric type IGP
                  administrative-group exclude 1
Request sequence number: 0
Response sequence number: 0
Number of times path updated: 2
Last updated: 0:49:52 ago
Metric: 10
Next Hop    Interface 
----------- ----------
20.30.66.66 Ethernet31

Destination: Juniper-156-PTX10002-36QDD
Path ID: 640
Path constraints: algo MIN-LATENCY
                  metric type MIN-DELAY
Request sequence number: 0
Response sequence number: 0
Number of times path updated: 6
Last updated: 0:02:25 ago
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
Number of times path updated: 5
Last updated: 0:49:52 ago
Metric: 100
Next Hop      Interface 
------------- ----------
20.30.156.156 Ethernet11

Destination: Juniper-156-PTX10002-36QDD
Path ID: 642
Path constraints: algo ADMIN
                  metric type IGP
                  administrative-group exclude 1
Request sequence number: 0
Response sequence number: 0
Number of times path updated: 2
Last updated: 0:49:52 ago
Metric: 10
Next Hop      Interface 
------------- ----------
20.30.156.156 Ethernet11

Destination: Juniper-175-ACX7100-48L
Path ID: 640
Path constraints: algo MIN-LATENCY
                  metric type MIN-DELAY
Request sequence number: 0
Response sequence number: 0
Number of times path updated: 6
Last updated: 0:02:25 ago
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
Number of times path updated: 16
Last updated: 0:11:18 ago
Metric: 110
Next Hop      Interface 
------------- ----------
20.30.66.66   Ethernet31
20.30.128.128 Ethernet19
20.30.179.179 Ethernet40
20.30.124.124 Ethernet17
20.30.221.221 Ethernet15
20.30.72.72   Ethernet9 
20.30.156.156 Ethernet11
20.30.53.53   Ethernet13

Destination: Juniper-175-ACX7100-48L
Path ID: 642
Path constraints: algo ADMIN
                  metric type IGP
                  administrative-group exclude 1
Request sequence number: 0
Response sequence number: 0
Number of times path updated: 2
Last updated: 0:49:56 ago
Metric: 20
Next Hop      Interface 
------------- ----------
20.30.131.131 Ethernet35

Destination: Juniper-179-ACX7024
Path ID: 640
Path constraints: algo MIN-LATENCY
                  metric type MIN-DELAY
Request sequence number: 0
Response sequence number: 0
Number of times path updated: 4
Last updated: 0:02:25 ago
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
Number of times path updated: 3
Last updated: 0:49:53 ago
Metric: 100
Next Hop      Interface 
------------- ----------
20.30.179.179 Ethernet40

Destination: Juniper-179-ACX7024
Path ID: 642
Path constraints: algo ADMIN
                  metric type IGP
                  administrative-group exclude 1
Request sequence number: 0
Response sequence number: 0
Number of times path updated: 2
Last updated: 0:49:53 ago
Metric: 10
Next Hop      Interface 
------------- ----------
20.30.179.179 Ethernet40

Flex algo paths for IPv6 address family
Topology ID: Level-2
Destination: Arista-Spine3-Q2A-30
Path ID: 640
Path constraints: algo MIN-LATENCY
                  metric type MIN-DELAY
Request sequence number: 0
Response sequence number: 0
Number of times path updated: 1
Last updated: 0:53:05 ago
Next Hop Interface
-------- ---------

Destination: Arista-Spine3-Q2A-30
Path ID: 641
Path constraints: algo MIN-TE
                  metric type TE
Request sequence number: 0
Response sequence number: 0
Number of times path updated: 1
Last updated: 0:53:05 ago
Next Hop Interface
-------- ---------

Destination: Arista-Spine3-Q2A-30
Path ID: 642
Path constraints: algo ADMIN
                  metric type IGP
                  administrative-group exclude 1
Request sequence number: 0
Response sequence number: 0
Number of times path updated: 1
Last updated: 0:53:05 ago
Next Hop Interface
-------- ---------

Destination: Arrcus-53
Path ID: 640
Path constraints: algo MIN-LATENCY
                  metric type MIN-DELAY
Request sequence number: 0
Response sequence number: 0
Number of times path updated: 7
Last updated: 0:02:25 ago
Metric: 10000
Next Hop                 Interface 
------------------------ ----------
fe80::5e07:58ff:fea3:aaa Ethernet13

Destination: Arrcus-53
Path ID: 641
Path constraints: algo MIN-TE
                  metric type TE
Request sequence number: 0
Response sequence number: 0
Number of times path updated: 4
Last updated: 0:11:18 ago
Metric: 100
Next Hop                 Interface 
------------------------ ----------
fe80::5e07:58ff:fea3:aaa Ethernet13

Destination: Arrcus-53
Path ID: 642
Path constraints: algo ADMIN
                  metric type IGP
                  administrative-group exclude 1
Request sequence number: 0
Response sequence number: 0
Number of times path updated: 4
Last updated: 0:11:18 ago
Metric: 10
Next Hop                 Interface 
------------------------ ----------
fe80::5e07:58ff:fea3:aaa Ethernet13

Destination: H3C_M1A_120
Path ID: 640
Path constraints: algo MIN-LATENCY
                  metric type MIN-DELAY
Request sequence number: 0
Response sequence number: 0
Number of times path updated: 4
Last updated: 0:02:25 ago
Metric: 10000
Next Hop                  Interface
------------------------- ---------
fe80::be31:e2ff:fee1:ec2c Ethernet3

Destination: H3C_M1A_120
Path ID: 641
Path constraints: algo MIN-TE
                  metric type TE
Request sequence number: 0
Response sequence number: 0
Number of times path updated: 2
Last updated: 0:49:55 ago
Metric: 100
Next Hop                  Interface
------------------------- ---------
fe80::be31:e2ff:fee1:ec2c Ethernet3

Destination: H3C_M1A_120
Path ID: 642
Path constraints: algo ADMIN
                  metric type IGP
                  administrative-group exclude 1
Request sequence number: 0
Response sequence number: 0
Number of times path updated: 2
Last updated: 0:49:55 ago
Metric: 10
Next Hop                  Interface
------------------------- ---------
fe80::be31:e2ff:fee1:ec2c Ethernet3

Destination: Juniper-156-PTX10002-36QDD
Path ID: 640
Path constraints: algo MIN-LATENCY
                  metric type MIN-DELAY
Request sequence number: 0
Response sequence number: 0
Number of times path updated: 2
Last updated: 0:02:25 ago
Metric: 10000
Next Hop                  Interface 
------------------------- ----------
fe80::d248:a1ff:feba:3c61 Ethernet11

Destination: Juniper-156-PTX10002-36QDD
Path ID: 641
Path constraints: algo MIN-TE
                  metric type TE
Request sequence number: 0
Response sequence number: 0
Number of times path updated: 1
Last updated: 0:02:39 ago
Metric: 100
Next Hop                  Interface 
------------------------- ----------
fe80::d248:a1ff:feba:3c61 Ethernet11

Destination: Juniper-156-PTX10002-36QDD
Path ID: 642
Path constraints: algo ADMIN
                  metric type IGP
                  administrative-group exclude 1
Request sequence number: 0
Response sequence number: 0
Number of times path updated: 2
Last updated: 0:49:52 ago
Metric: 10
Next Hop                  Interface 
------------------------- ----------
fe80::d248:a1ff:feba:3c61 Ethernet11

Destination: Juniper-175-ACX7100-48L
Path ID: 640
Path constraints: algo MIN-LATENCY
                  metric type MIN-DELAY
Request sequence number: 0
Response sequence number: 0
Number of times path updated: 1
Last updated: 0:00:51 ago
Metric: 10100
Next Hop                 Interface 
------------------------ ----------
fe80::5e07:58ff:fea3:aaa Ethernet13

Destination: Juniper-175-ACX7100-48L
Path ID: 641
Path constraints: algo MIN-TE
                  metric type TE
Request sequence number: 0
Response sequence number: 0
Number of times path updated: 1
Last updated: 0:00:51 ago
Metric: 110
Next Hop                  Interface 
------------------------- ----------
fe80::5e07:58ff:fea3:aaa  Ethernet13
fe80::c214:b8ff:fe21:9790 Ethernet4 
fe80::ea24:a6ff:fe96:548  Ethernet40
fe80::d248:a1ff:feba:3c61 Ethernet11

Destination: Juniper-175-ACX7100-48L
Path ID: 642
Path constraints: algo ADMIN
                  metric type IGP
                  administrative-group exclude 1
Request sequence number: 0
Response sequence number: 0
Number of times path updated: 1
Last updated: 0:50:02 ago
Next Hop Interface
-------- ---------

Destination: Juniper-179-ACX7024
Path ID: 640
Path constraints: algo MIN-LATENCY
                  metric type MIN-DELAY
Request sequence number: 0
Response sequence number: 0
Number of times path updated: 4
Last updated: 0:02:25 ago
Metric: 10000
Next Hop                 Interface 
------------------------ ----------
fe80::ea24:a6ff:fe96:548 Ethernet40

Destination: Juniper-179-ACX7024
Path ID: 641
Path constraints: algo MIN-TE
                  metric type TE
Request sequence number: 0
Response sequence number: 0
Number of times path updated: 3
Last updated: 0:49:53 ago
Metric: 100
Next Hop                 Interface 
------------------------ ----------
fe80::ea24:a6ff:fe96:548 Ethernet40

Destination: Juniper-179-ACX7024
Path ID: 642
Path constraints: algo ADMIN
                  metric type IGP
                  administrative-group exclude 1
Request sequence number: 0
Response sequence number: 0
Number of times path updated: 2
Last updated: 0:49:53 ago
Metric: 10
Next Hop                 Interface 
------------------------ ----------
fe80::ea24:a6ff:fe96:548 Ethernet40

Destination: Nokia-SR1-217
Path ID: 640
Path constraints: algo MIN-LATENCY
                  metric type MIN-DELAY
Request sequence number: 0
Response sequence number: 0
Number of times path updated: 5
Last updated: 0:02:25 ago
Metric: 10000
Next Hop                  Interface
------------------------- ---------
fe80::c214:b8ff:fe21:9790 Ethernet4

Destination: Nokia-SR1-217
Path ID: 641
Path constraints: algo MIN-TE
                  metric type TE
Request sequence number: 0
Response sequence number: 0
Number of times path updated: 2
Last updated: 0:49:55 ago
Metric: 100
Next Hop                  Interface
------------------------- ---------
fe80::c214:b8ff:fe21:9790 Ethernet4

Destination: Nokia-SR1-217
Path ID: 642
Path constraints: algo ADMIN
                  metric type IGP
                  administrative-group exclude 1
Request sequence number: 0
Response sequence number: 0
Number of times path updated: 2
Last updated: 0:49:55 ago
Metric: 10
Next Hop                  Interface
------------------------- ---------
fe80::c214:b8ff:fe21:9790 Ethernet4

```

## show isis segment-routing tunnel

```text
 Index    Endpoint         Next Hop/Tunnel Index         Interface    Labels   
-------- ---------------- ---------------------------- -------------- ---------
 1        2002::179/128    TI-LFA (16)                   -            [ 3 ]    
 2        2002::120/128    fe80::be31:e2ff:fee1:ec2c     Ethernet3    [ 3 ]    
 3        2002::175/128    fe80::5a70:7fff:fe9f:c403     Ethernet12   [ 20575 ]
                           fe80::5e07:58ff:fea3:aaa      Ethernet13   [ 20575 ]
                           fe80::be31:e2ff:fee1:ec2c     Ethernet3    [ 20575 ]
                           fe80::c214:b8ff:fe21:9790     Ethernet4    [ 20575 ]
                           fe80::d248:a1ff:feba:3c61     Ethernet11   [ 20575 ]
                           fe80::ea24:a6ff:fe96:548      Ethernet40   [ 20575 ]
 4        2002::217/128    TI-LFA (24)                   -            [ 20617 ]
 5        2002::156/128    TI-LFA (2)                    -            [ 3 ]    
 6        2002::53/128     TI-LFA (18)                   -            [ 3 ]    
 7        10.0.0.175/32    20.30.53.53                   Ethernet13   [ 20175 ]
                           20.30.66.66                   Ethernet31   [ 20175 ]
                           20.30.72.72                   Ethernet9    [ 20175 ]
                           20.30.84.84                   Ethernet12   [ 20175 ]
                           20.30.120.120                 Ethernet3    [ 20175 ]
                           20.30.131.131                 Ethernet35   [ 20175 ]
 8        10.0.0.84/32     20.30.84.84                   Ethernet12   [ 20084 ]
 9        10.0.0.131/32    20.30.131.131                 Ethernet35   [ 3 ]    
 10       10.0.0.53/32     20.30.53.53                   Ethernet13   [ 0 ]    
 11       10.0.0.156/32    20.30.156.156                 Ethernet11   [ 3 ]    
 12       10.0.0.179/32    20.30.179.179                 Ethernet40   [ 3 ]    
 13       10.0.0.66/32     20.30.66.66                   Ethernet31   [ 3 ]    
 14       10.0.0.72/32     20.30.72.72                   Ethernet9    [ 3 ]    
 15       10.0.0.221/32    20.30.221.221                 Ethernet15   [ 3 ]    

```

## show isis segment-routing prefix-segments

```text

System ID: Arista-Spine3-Q2A-30			Instance: 'IGP'
SR supported Data-plane: MPLS			SR Router ID: 10.0.0.30

Node: 62     Proxy-Node: 0      Prefix: 0       Total Segments: 62

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
   10.0.0.53/32                 53   20053 Node       R:0 N:1 P:1 E:1 V:0 L:0      Arrcus-53       L2    unprotected SPF         
   10.0.0.53/32               1181   21181 Node       R:0 N:1 P:0 E:0 V:0 L:0      Arrcus-53       L2    unprotected MIN-LATENCY 
   10.0.0.53/32               1182   21182 Node       R:0 N:1 P:0 E:0 V:0 L:0      Arrcus-53       L2    unprotected MIN-TE      
   10.0.0.53/32               1183   21183 Node       R:0 N:1 P:0 E:0 V:0 L:0      Arrcus-53       L2    unprotected ADMIN       
   10.0.0.66/32                 66   20066 Node       R:0 N:1 P:0 E:0 V:0 L:0      Ciena-8140-66   L2    unprotected SPF         
   10.0.0.66/32               1194   21194 Node       R:0 N:1 P:0 E:0 V:0 L:0      Ciena-8140-66   L2    unprotected MIN-LATENCY 
   10.0.0.66/32               1195   21195 Node       R:0 N:1 P:0 E:0 V:0 L:0      Ciena-8140-66   L2    unprotected MIN-TE      
   10.0.0.66/32               1196   21196 Node       R:0 N:1 P:0 E:0 V:0 L:0      Ciena-8140-66   L2    unprotected ADMIN       
   10.0.0.72/32                 72   20072 Node       R:0 N:1 P:0 E:0 V:0 L:0      Ciena-5134-72   L2    unprotected SPF         
   10.0.0.72/32               1200   21200 Node       R:0 N:1 P:0 E:0 V:0 L:0      Ciena-5134-72   L2    unprotected MIN-LATENCY 
   10.0.0.72/32               1201   21201 Node       R:0 N:1 P:0 E:0 V:0 L:0      Ciena-5134-72   L2    unprotected MIN-TE      
   10.0.0.72/32               1202   21202 Node       R:0 N:1 P:0 E:0 V:0 L:0      Ciena-5134-72   L2    unprotected ADMIN       
   10.0.0.84/32                 84   20084 Node       R:0 N:1 P:1 E:0 V:0 L:0      Ericsson_84_R6678 L2    unprotected SPF         
   10.0.0.131/32               131   20131 Node       R:0 N:1 P:0 E:0 V:0 L:0      Juniper-131-JCNR L2    unprotected SPF         
   10.0.0.156/32               156   20156 Node       R:0 N:1 P:0 E:0 V:0 L:0      Juniper-156-PTX10002-36QDD L2    unprotected SPF         
   10.0.0.156/32              1284   21284 Node       R:0 N:1 P:0 E:0 V:0 L:0      Juniper-156-PTX10002-36QDD L2    unprotected MIN-LATENCY 
   10.0.0.156/32              1285   21285 Node       R:0 N:1 P:0 E:0 V:0 L:0      Juniper-156-PTX10002-36QDD L2    unprotected MIN-TE      
   10.0.0.156/32              1286   21286 Node       R:0 N:1 P:0 E:0 V:0 L:0      Juniper-156-PTX10002-36QDD L2    unprotected ADMIN       
   10.0.0.175/32               175   20175 Node       R:0 N:1 P:0 E:0 V:0 L:0      Juniper-175-ACX7100-48L L2    unprotected SPF         
   10.0.0.175/32              1303   21303 Node       R:0 N:1 P:0 E:0 V:0 L:0      Juniper-175-ACX7100-48L L2    unprotected MIN-LATENCY 
   10.0.0.175/32              1304   21304 Node       R:0 N:1 P:0 E:0 V:0 L:0      Juniper-175-ACX7100-48L L2    unprotected MIN-TE      
   10.0.0.175/32              1305   21305 Node       R:0 N:1 P:0 E:0 V:0 L:0      Juniper-175-ACX7100-48L L2    unprotected ADMIN       
   10.0.0.179/32               179   20179 Node       R:0 N:1 P:0 E:0 V:0 L:0      Juniper-179-ACX7024 L2    unprotected SPF         
   10.0.0.179/32              1307   21307 Node       R:0 N:1 P:0 E:0 V:0 L:0      Juniper-179-ACX7024 L2    unprotected MIN-LATENCY 
   10.0.0.179/32              1308   21308 Node       R:0 N:1 P:0 E:0 V:0 L:0      Juniper-179-ACX7024 L2    unprotected MIN-TE      
   10.0.0.179/32              1309   21309 Node       R:0 N:1 P:0 E:0 V:0 L:0      Juniper-179-ACX7024 L2    unprotected ADMIN       
   10.0.0.221/32               221  720221 Node       R:0 N:1 P:0 E:0 V:0 L:0      221             L2    unprotected SPF         
   10.0.0.221/32              1349  721349 Node       R:0 N:1 P:0 E:0 V:0 L:0      221             L2    unprotected MIN-LATENCY 
   10.0.0.221/32              1350  721350 Node       R:0 N:1 P:0 E:0 V:0 L:0      221             L2    unprotected MIN-TE      
   10.0.0.221/32              1351  721351 Node       R:0 N:1 P:0 E:0 V:0 L:0      221             L2    unprotected ADMIN       
*  2002::30/128                430   20430 Node       R:0 N:1 P:0 E:0 V:0 L:0      Arista-Spine3-Q2A-30 L2    unprotected SPF         
*  2002::30/128               1558   21558 Node       R:0 N:1 P:0 E:0 V:0 L:0      Arista-Spine3-Q2A-30 L2    unprotected MIN-LATENCY 
*  2002::30/128               1559   21559 Node       R:0 N:1 P:0 E:0 V:0 L:0      Arista-Spine3-Q2A-30 L2    unprotected MIN-TE      
*  2002::30/128               1560   21560 Node       R:0 N:1 P:0 E:0 V:0 L:0      Arista-Spine3-Q2A-30 L2    unprotected ADMIN       
   2002::53/128                453   20453 Node       R:0 N:1 P:1 E:1 V:0 L:0      Arrcus-53       L2    node        SPF         
   2002::53/128               1581   21581 Node       R:0 N:1 P:0 E:0 V:0 L:0      Arrcus-53       L2    node        MIN-LATENCY 
   2002::53/128               1582   21582 Node       R:0 N:1 P:0 E:0 V:0 L:0      Arrcus-53       L2    node        MIN-TE      
   2002::53/128               1583   21583 Node       R:0 N:1 P:0 E:0 V:0 L:0      Arrcus-53       L2    node        ADMIN       
   2002::120/128               520   20520 Node       R:0 N:1 P:0 E:0 V:0 L:0      H3C_M1A_120     L2    node        SPF         
   2002::120/128              1648   21648 Node       R:0 N:1 P:1 E:0 V:0 L:0      H3C_M1A_120     L2    node        MIN-LATENCY 
   2002::120/128              1649   21649 Node       R:0 N:1 P:1 E:0 V:0 L:0      H3C_M1A_120     L2    node        MIN-TE      
   2002::120/128              1650   21650 Node       R:0 N:1 P:1 E:0 V:0 L:0      H3C_M1A_120     L2    node        ADMIN       
   2002::156/128               556   20556 Node       R:0 N:1 P:0 E:0 V:0 L:0      Juniper-156-PTX10002-36QDD L2    node        SPF         
   2002::156/128              1684   21684 Node       R:0 N:1 P:0 E:0 V:0 L:0      Juniper-156-PTX10002-36QDD L2    node        MIN-LATENCY 
   2002::156/128              1685   21685 Node       R:0 N:1 P:0 E:0 V:0 L:0      Juniper-156-PTX10002-36QDD L2    node        MIN-TE      
   2002::156/128              1686   21686 Node       R:0 N:1 P:0 E:0 V:0 L:0      Juniper-156-PTX10002-36QDD L2    node        ADMIN       
   2002::175/128               575   20575 Node       R:0 N:1 P:0 E:0 V:0 L:0      Juniper-175-ACX7100-48L L2    unprotected SPF         
   2002::175/128              1703   21703 Node       R:0 N:1 P:0 E:0 V:0 L:0      Juniper-175-ACX7100-48L L2    node        MIN-LATENCY 
   2002::175/128              1704   21704 Node       R:0 N:1 P:0 E:0 V:0 L:0      Juniper-175-ACX7100-48L L2    unprotected MIN-TE      
   2002::175/128              1705   21705 Node       R:0 N:1 P:0 E:0 V:0 L:0      Juniper-175-ACX7100-48L L2    unprotected ADMIN       
   2002::179/128               579   20579 Node       R:0 N:1 P:0 E:0 V:0 L:0      Juniper-179-ACX7024 L2    node        SPF         
   2002::179/128              1707   21707 Node       R:0 N:1 P:0 E:0 V:0 L:0      Juniper-179-ACX7024 L2    node        MIN-LATENCY 
   2002::179/128              1708   21708 Node       R:0 N:1 P:0 E:0 V:0 L:0      Juniper-179-ACX7024 L2    node        MIN-TE      
   2002::179/128              1709   21709 Node       R:0 N:1 P:0 E:0 V:0 L:0      Juniper-179-ACX7024 L2    node        ADMIN       
   2002::217/128               617   20617 Node       R:0 N:1 P:1 E:0 V:0 L:0      Nokia-SR1-217   L2    node        SPF         
   2002::217/128              1745   21745 Node       R:0 N:1 P:1 E:0 V:0 L:0      Nokia-SR1-217   L2    node        MIN-LATENCY 
   2002::217/128              1746   21746 Node       R:0 N:1 P:1 E:0 V:0 L:0      Nokia-SR1-217   L2    node        MIN-TE      
   2002::217/128              1747   21747 Node       R:0 N:1 P:1 E:0 V:0 L:0      Nokia-SR1-217   L2    node        ADMIN       
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
 I L2     10.0.0.53/32 [115/10]
           via 20.30.53.53, Ethernet13
 I L2     10.0.0.66/32 [115/20]
           via 20.30.66.66, Ethernet31
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
 I L2     10.0.0.131/32 [115/10]
           via 20.30.131.131, Ethernet35
 I L2     10.0.0.156/32 [115/10]
           via 20.30.156.156, Ethernet11
 I L2     10.0.0.175/32 [115/20]
           via 20.30.120.120, Ethernet3
           via 20.30.72.72, Ethernet9
           via 20.30.84.84, Ethernet12
           via 20.30.53.53, Ethernet13
           via 20.30.124.124, Ethernet17
           via 20.30.128.128, Ethernet19
           via 20.30.66.66, Ethernet31
           via 20.30.131.131, Ethernet35
 I L2     10.0.0.179/32 [115/10]
           via 20.30.179.179, Ethernet40
 I L2     10.0.0.216/32 [115/45]
           via 20.30.120.120, Ethernet3
           via 20.30.72.72, Ethernet9
           via 20.30.84.84, Ethernet12
           via 20.30.53.53, Ethernet13
           via 20.30.124.124, Ethernet17
           via 20.30.128.128, Ethernet19
           via 20.30.66.66, Ethernet31
           via 20.30.131.131, Ethernet35
 I L2     10.0.0.221/32 [115/10]
           via 20.30.221.221, Ethernet15
 I L2     10.0.1.179/32 [115/10]
           via 20.30.179.179, Ethernet40
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
 I L2     20.53.175.0/24 [115/20]
           via 20.30.53.53, Ethernet13
 I L2     20.66.175.0/24 [115/20]
           via 20.30.66.66, Ethernet31
 I L2     20.72.175.0/24 [115/20]
           via 20.30.72.72, Ethernet9
 I L2     20.84.175.0/24 [115/35]
           via 20.30.120.120, Ethernet3
           via 20.30.72.72, Ethernet9
           via 20.30.84.84, Ethernet12
           via 20.30.53.53, Ethernet13
           via 20.30.124.124, Ethernet17
           via 20.30.128.128, Ethernet19
           via 20.30.66.66, Ethernet31
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
           via 20.30.120.120, Ethernet3
           via 20.30.72.72, Ethernet9
           via 20.30.84.84, Ethernet12
           via 20.30.53.53, Ethernet13
           via 20.30.124.124, Ethernet17
           via 20.30.128.128, Ethernet19
           via 20.30.66.66, Ethernet31
           via 20.30.131.131, Ethernet35
 I L2     20.175.214.0/24 [115/35]
           via 20.30.120.120, Ethernet3
           via 20.30.72.72, Ethernet9
           via 20.30.84.84, Ethernet12
           via 20.30.53.53, Ethernet13
           via 20.30.124.124, Ethernet17
           via 20.30.128.128, Ethernet19
           via 20.30.66.66, Ethernet31
           via 20.30.131.131, Ethernet35
 I L2     20.175.217.0/24 [115/35]
           via 20.30.120.120, Ethernet3
           via 20.30.72.72, Ethernet9
           via 20.30.84.84, Ethernet12
           via 20.30.53.53, Ethernet13
           via 20.30.124.124, Ethernet17
           via 20.30.128.128, Ethernet19
           via 20.30.66.66, Ethernet31
           via 20.30.131.131, Ethernet35
 I L2     20.175.221.0/24 [115/20]
           via 20.30.221.221, Ethernet15
 I L2     20.214.216.0/24 [115/45]
           via 20.30.120.120, Ethernet3
           via 20.30.72.72, Ethernet9
           via 20.30.84.84, Ethernet12
           via 20.30.53.53, Ethernet13
           via 20.30.124.124, Ethernet17
           via 20.30.128.128, Ethernet19
           via 20.30.66.66, Ethernet31
           via 20.30.131.131, Ethernet35
 I L2     30.66.221.0/24 [115/20]
           via 20.30.221.221, Ethernet15
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

```

## show mpls route

```text
MPLS forwarding table (Label [metric] Vias) - 70 routes 
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

 20053   A[1]
                via M, 20.30.53.53, swap 0
                    EgressACL: apply
                    directly connected, Ethernet13
                    5c:07:58:a3:0a:aa, vlan 1022
 20066   A[1]
                via M, pop
                    EgressACL: apply
                    20.30.66.66 Ethernet31
 20072   A[1]
                via M, pop
                    EgressACL: apply
                    20.30.72.72 Ethernet9
 20084   A[1]
                via M, forward
                    EgressACL: apply
                    20.30.84.84 Ethernet12
 20131   A[1]
                via M, pop
                    EgressACL: apply
                    20.30.131.131 Ethernet35
 20156   A[1]
                via M, pop
                    EgressACL: apply
                    20.30.156.156 Ethernet11
 20175   A[1]
                via M, 20.30.53.53, swap 20175
                    EgressACL: apply
                    directly connected, Ethernet13
                    5c:07:58:a3:0a:aa, vlan 1022
                via M, 20.30.66.66, swap 20175
                    EgressACL: apply
                    directly connected, Ethernet31
                    e4:6d:7f:e3:c8:08, vlan 1020
                via M, 20.30.72.72, swap 20175
                    EgressACL: apply
                    directly connected, Ethernet9
                    e0:9b:27:c4:c5:84, vlan 1009
                via M, 20.30.84.84, swap 20175
                    EgressACL: apply
                    directly connected, Ethernet12
                    58:70:7f:9f:c4:03, vlan 1014
                via M, 20.30.120.120, swap 20175
                    EgressACL: apply
                    directly connected, Ethernet3
                    bc:31:e2:e1:ec:2c, vlan 1017
                via M, 20.30.131.131, swap 20175
                    EgressACL: apply
                    directly connected, Ethernet35
                    40:a6:b7:94:34:cb, vlan 1012
 20179   A[1]
                via M, pop
                    EgressACL: apply
                    20.30.179.179 Ethernet40
 20221   A[1]
                via M, pop
                    EgressACL: apply
                    20.30.221.221 Ethernet15
 20453   A[1]
                via M, ::, pop
                    EgressACL: apply
                  via TI-LFA tunnel index 18
                    via fe80::5e07:58ff:fea3:aaa, Ethernet13, label exp-null-v6(2)
                    backup via fe80::d248:a1ff:feba:3c61, Ethernet11, label 20575 20453
 20520   A[1]
                via M, pop
                    EgressACL: apply
                    fe80::be31:e2ff:fee1:ec2c Ethernet3
 20556   A[1]
                via M, ::, pop
                    EgressACL: apply
                  via TI-LFA tunnel index 2
                    via fe80::d248:a1ff:feba:3c61, Ethernet11, label imp-null(3)
                    backup via fe80::ea24:a6ff:fe96:548, Ethernet40, label 20575 20556
 20575   A[1]
                via M, forward
                    EgressACL: apply
                    fe80::c214:b8ff:fe21:9790 Ethernet4
                    fe80::5e07:58ff:fea3:aaa Ethernet13
                    fe80::ea24:a6ff:fe96:548 Ethernet40
                    fe80::5a70:7fff:fe9f:c403 Ethernet12
                    fe80::d248:a1ff:feba:3c61 Ethernet11
                    fe80::be31:e2ff:fee1:ec2c Ethernet3
 20579   A[1]
                via M, ::, pop
                    EgressACL: apply
                  via TI-LFA tunnel index 16
                    via fe80::ea24:a6ff:fe96:548, Ethernet40, label imp-null(3)
                    backup via fe80::d248:a1ff:feba:3c61, Ethernet11, label 20575 20579
 20617   A[1]
                via M, ::, forward
                    EgressACL: apply
                  via TI-LFA tunnel index 24
                    via fe80::c214:b8ff:fe21:9790, Ethernet4, label imp-null(3)
                    backup via fe80::ea24:a6ff:fe96:548, Ethernet40, label 20575
 21181   A[1]
                via M, pop
                    EgressACL: apply
                    20.30.53.53 Ethernet13
 21182   A[1]
                via M, pop
                    EgressACL: apply
                    20.30.53.53 Ethernet13
 21183   A[1]
                via M, pop
                    EgressACL: apply
                    20.30.53.53 Ethernet13
 21194   A[1]
                via M, pop
                    EgressACL: apply
                    20.30.66.66 Ethernet31
 21195   A[1]
                via M, pop
                    EgressACL: apply
                    20.30.66.66 Ethernet31
 21196   A[1]
                via M, pop
                    EgressACL: apply
                    20.30.66.66 Ethernet31
 21200   A[1]
                via M, pop
                    EgressACL: apply
                    20.30.72.72 Ethernet9
 21201   A[1]
                via M, pop
                    EgressACL: apply
                    20.30.72.72 Ethernet9
 21202   A[1]
                via M, pop
                    EgressACL: apply
                    20.30.72.72 Ethernet9
 21284   A[1]
                via M, pop
                    EgressACL: apply
                    20.30.156.156 Ethernet11
 21285   A[1]
                via M, pop
                    EgressACL: apply
                    20.30.156.156 Ethernet11
 21286   A[1]
                via M, pop
                    EgressACL: apply
                    20.30.156.156 Ethernet11
 21303   A[1]
                via M, 20.30.221.221, swap 721303
                    EgressACL: apply
                    directly connected, Ethernet15
                    30:c5:07:84:3e:79, vlan 1006
 21304   A[1]
                via M, 20.30.53.53, swap 21304
                    EgressACL: apply
                    directly connected, Ethernet13
                    5c:07:58:a3:0a:aa, vlan 1022
                via M, 20.30.66.66, swap 21304
                    EgressACL: apply
                    directly connected, Ethernet31
                    e4:6d:7f:e3:c8:08, vlan 1020
                via M, 20.30.72.72, swap 21304
                    EgressACL: apply
                    directly connected, Ethernet9
                    e0:9b:27:c4:c5:84, vlan 1009
                via M, 20.30.156.156, swap 21304
                    EgressACL: apply
                    directly connected, Ethernet11
                    d0:48:a1:ba:3c:61, vlan 1019
                via M, 20.30.179.179, swap 21304
                    EgressACL: apply
                    directly connected, Ethernet40
                    e8:24:a6:96:05:48, vlan 1015
                via M, 20.30.221.221, swap 721304
                    EgressACL: apply
                    directly connected, Ethernet15
                    30:c5:07:84:3e:79, vlan 1006
 21305   A[1]
                via M, forward
                    EgressACL: apply
                    20.30.131.131 Ethernet35
 21307   A[1]
                via M, pop
                    EgressACL: apply
                    20.30.179.179 Ethernet40
 21308   A[1]
                via M, pop
                    EgressACL: apply
                    20.30.179.179 Ethernet40
 21309   A[1]
                via M, pop
                    EgressACL: apply
                    20.30.179.179 Ethernet40
 21349   A[1]
                via M, pop
                    EgressACL: apply
                    20.30.221.221 Ethernet15
 21350   A[1]
                via M, pop
                    EgressACL: apply
                    20.30.221.221 Ethernet15
 21351   A[1]
                via M, pop
                    EgressACL: apply
                    20.30.221.221 Ethernet15
 21581   A[1]
                via M, ::, pop
                    EgressACL: apply
                  via TI-LFA tunnel index 4
                    via fe80::5e07:58ff:fea3:aaa, Ethernet13, label imp-null(3)
                    backup via fe80::ea24:a6ff:fe96:548, Ethernet40, label 20 21581
 21582   A[1]
                via M, ::, pop
                    EgressACL: apply
                  via TI-LFA tunnel index 9
                    via fe80::5e07:58ff:fea3:aaa, Ethernet13, label imp-null(3)
                    backup via fe80::ea24:a6ff:fe96:548, Ethernet40, label 21704 21582
 21583   A[1]
                via M, pop
                    EgressACL: apply
                    fe80::5e07:58ff:fea3:aaa Ethernet13
 21648   A[1]
                via M, forward
                    EgressACL: apply
                    fe80::be31:e2ff:fee1:ec2c Ethernet3
 21649   A[1]
                via M, forward
                    EgressACL: apply
                    fe80::be31:e2ff:fee1:ec2c Ethernet3
 21650   A[1]
                via M, forward
                    EgressACL: apply
                    fe80::be31:e2ff:fee1:ec2c Ethernet3
 21684   A[1]
                via M, ::, pop
                    EgressACL: apply
                  via TI-LFA tunnel index 0
                    via fe80::d248:a1ff:feba:3c61, Ethernet11, label imp-null(3)
                    backup via fe80::5e07:58ff:fea3:aaa, Ethernet13, label 21703 21684
 21685   A[1]
                via M, ::, pop
                    EgressACL: apply
                  via TI-LFA tunnel index 10
                    via fe80::d248:a1ff:feba:3c61, Ethernet11, label imp-null(3)
                    backup via fe80::ea24:a6ff:fe96:548, Ethernet40, label 21704 21685
 21686   A[1]
                via M, pop
                    EgressACL: apply
                    fe80::d248:a1ff:feba:3c61 Ethernet11
 21703   A[1]
                via M, ::, pop
                    EgressACL: apply
                  via TI-LFA tunnel index 6
                    via fe80::5e07:58ff:fea3:aaa, Ethernet13, label 21703
                    backup via fe80::ea24:a6ff:fe96:548, Ethernet40, label 20
 21704   A[1]
                via M, forward
                    EgressACL: apply
                    fe80::5e07:58ff:fea3:aaa Ethernet13
                    fe80::c214:b8ff:fe21:9790 Ethernet4
                    fe80::d248:a1ff:feba:3c61 Ethernet11
                    fe80::ea24:a6ff:fe96:548 Ethernet40
 21707   A[1]
                via M, ::, pop
                    EgressACL: apply
                  via TI-LFA tunnel index 5
                    via fe80::ea24:a6ff:fe96:548, Ethernet40, label imp-null(3)
                    backup via fe80::5e07:58ff:fea3:aaa, Ethernet13, label 21703 21707
 21708   A[1]
                via M, ::, pop
                    EgressACL: apply
                  via TI-LFA tunnel index 11
                    via fe80::ea24:a6ff:fe96:548, Ethernet40, label imp-null(3)
                    backup via fe80::c214:b8ff:fe21:9790, Ethernet4, label 21704 21708
 21709   A[1]
                via M, pop
                    EgressACL: apply
                    fe80::ea24:a6ff:fe96:548 Ethernet40
 21745   A[1]
                via M, ::, forward
                    EgressACL: apply
                  via TI-LFA tunnel index 3
                    via fe80::c214:b8ff:fe21:9790, Ethernet4, label imp-null(3)
                    backup via fe80::5e07:58ff:fea3:aaa, Ethernet13, label 21703
 21746   A[1]
                via M, ::, forward
                    EgressACL: apply
                  via TI-LFA tunnel index 7
                    via fe80::c214:b8ff:fe21:9790, Ethernet4, label imp-null(3)
                    backup via fe80::d248:a1ff:feba:3c61, Ethernet11, label 21704
 21747   A[1]
                via M, forward
                    EgressACL: apply
                    fe80::c214:b8ff:fe21:9790 Ethernet4
 362144   [0]
                via I, ipv4, vrf FLEXALGO
 362145   [0]
                via I, ipv4, vrf RED
 378528  A[1]
                via M, 20.30.53.53, pop
                    EgressACL: apply
                    directly connected, Ethernet13
                    5c:07:58:a3:0a:aa, vlan 1022
 378529  A[1]
                via M, fe80::5e07:58ff:fea3:aaa, pop
                    EgressACL: apply
                    directly connected, Ethernet13
                    5c:07:58:a3:0a:aa, vlan 1022
 378530  A[1]
                via M, 20.30.84.84, pop
                    EgressACL: apply
                    directly connected, Ethernet12
                    58:70:7f:9f:c4:03, vlan 1014
 378531  A[1]
                via M, fe80::5a70:7fff:fe9f:c403, pop
                    EgressACL: apply
                    directly connected, Ethernet12
                    58:70:7f:9f:c4:03, vlan 1014
 378532  A[1]
                via M, fe80::c214:b8ff:fe21:9790, pop
                    EgressACL: apply
                    directly connected, Ethernet4
                    c0:14:b8:21:97:90, vlan 1008
 378533  A[1]
                via M, 20.30.131.131, pop
                    EgressACL: apply
                    directly connected, Ethernet35
                    40:a6:b7:94:34:cb, vlan 1012
 378534  A[1]
                via M, 20.30.120.120, pop
                    EgressACL: apply
                    directly connected, Ethernet3
                    bc:31:e2:e1:ec:2c, vlan 1017
 378535  A[1]
                via M, fe80::be31:e2ff:fee1:ec2c, pop
                    EgressACL: apply
                    directly connected, Ethernet3
                    bc:31:e2:e1:ec:2c, vlan 1017
 378536  A[1]
                via M, 20.30.72.72, pop
                    EgressACL: apply
                    directly connected, Ethernet9
                    e0:9b:27:c4:c5:84, vlan 1009
 378537  A[1]
                via M, 20.30.66.66, pop
                    EgressACL: apply
                    directly connected, Ethernet31
                    e4:6d:7f:e3:c8:08, vlan 1020
 378538  A[1]
                via M, 20.30.179.179, pop
                    EgressACL: apply
                    directly connected, Ethernet40
                    e8:24:a6:96:05:48, vlan 1015
 378539  A[1]
                via M, fe80::ea24:a6ff:fe96:548, pop
                    EgressACL: apply
                    directly connected, Ethernet40
                    e8:24:a6:96:05:48, vlan 1015
 378540  A[1]
                via M, 20.30.156.156, pop
                    EgressACL: apply
                    directly connected, Ethernet11
                    d0:48:a1:ba:3c:61, vlan 1019
 378541  A[1]
                via M, fe80::d248:a1ff:feba:3c61, pop
                    EgressACL: apply
                    directly connected, Ethernet11
                    d0:48:a1:ba:3c:61, vlan 1019
 378542  A[1]
                via M, 20.30.221.221, pop
                    EgressACL: apply
                    directly connected, Ethernet15
                    30:c5:07:84:3e:79, vlan 1006
```

## show mpls lfib route

```text
MPLS forwarding table (Label [metric] Vias) - 70 routes 
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

 IP    20053    [1], 10.0.0.53/32
                via M, 20.30.53.53, swap 0
                 payload autoDecide, ttlMode uniform, apply egress-acl
                 interface Ethernet13
 IP    20066    [1], 10.0.0.66/32
                via M, 20.30.66.66, pop
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                 interface Ethernet31
 IP    20072    [1], 10.0.0.72/32
                via M, 20.30.72.72, pop
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                 interface Ethernet9
 IP    20084    [1], 10.0.0.84/32
                via M, 20.30.84.84, forward
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                 interface Ethernet12
 IP    20131    [1], 10.0.0.131/32
                via M, 20.30.131.131, pop
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                 interface Ethernet35
 IP    20156    [1], 10.0.0.156/32
                via M, 20.30.156.156, pop
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                 interface Ethernet11
 IP    20175    [1], 10.0.0.175/32
                via M, 20.30.53.53, swap 20175
                 payload autoDecide, ttlMode uniform, apply egress-acl
                 interface Ethernet13
                via M, 20.30.66.66, swap 20175
                 payload autoDecide, ttlMode uniform, apply egress-acl
                 interface Ethernet31
                via M, 20.30.72.72, swap 20175
                 payload autoDecide, ttlMode uniform, apply egress-acl
                 interface Ethernet9
                via M, 20.30.84.84, swap 20175
                 payload autoDecide, ttlMode uniform, apply egress-acl
                 interface Ethernet12
                via M, 20.30.120.120, swap 20175
                 payload autoDecide, ttlMode uniform, apply egress-acl
                 interface Ethernet3
                via M, 20.30.131.131, swap 20175
                 payload autoDecide, ttlMode uniform, apply egress-acl
                 interface Ethernet35
 IP    20179    [1], 10.0.0.179/32
                via M, 20.30.179.179, pop
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                 interface Ethernet40
 IP    20221    [1], 10.0.0.221/32
                via M, 20.30.221.221, pop
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                 interface Ethernet15
 IP    20453    [1], 2002::53/128
                via TI-LFA tunnel index 18, pop
                 payload autoDecide, ttlMode uniform, apply egress-acl
                    via fe80::5e07:58ff:fea3:aaa, Ethernet13, label exp-null-v6(2)
                    backup via fe80::d248:a1ff:feba:3c61, Ethernet11, label 20575 20453
 IP    20520    [1], 2002::120/128
                via M, fe80::be31:e2ff:fee1:ec2c, pop
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                 interface Ethernet3
 IP    20556    [1], 2002::156/128
                via TI-LFA tunnel index 2, pop
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                    via fe80::d248:a1ff:feba:3c61, Ethernet11, label imp-null(3)
                    backup via fe80::ea24:a6ff:fe96:548, Ethernet40, label 20575 20556
 IP    20575    [1], 2002::175/128
                via M, fe80::5a70:7fff:fe9f:c403, forward
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                 interface Ethernet12
                via M, fe80::5e07:58ff:fea3:aaa, forward
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                 interface Ethernet13
                via M, fe80::be31:e2ff:fee1:ec2c, forward
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                 interface Ethernet3
                via M, fe80::c214:b8ff:fe21:9790, forward
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                 interface Ethernet4
                via M, fe80::d248:a1ff:feba:3c61, forward
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                 interface Ethernet11
                via M, fe80::ea24:a6ff:fe96:548, forward
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                 interface Ethernet40
 IP    20579    [1], 2002::179/128
                via TI-LFA tunnel index 16, pop
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                    via fe80::ea24:a6ff:fe96:548, Ethernet40, label imp-null(3)
                    backup via fe80::d248:a1ff:feba:3c61, Ethernet11, label 20575 20579
 IP    20617    [1], 2002::217/128
                via TI-LFA tunnel index 24, forward
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                    via fe80::c214:b8ff:fe21:9790, Ethernet4, label imp-null(3)
                    backup via fe80::ea24:a6ff:fe96:548, Ethernet40, label 20575
 IP    21181    [1], 10.0.0.53/32, algorithm MIN-LATENCY
                via M, 20.30.53.53, pop
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                 interface Ethernet13
 IP    21182    [1], 10.0.0.53/32, algorithm MIN-TE
                via M, 20.30.53.53, pop
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                 interface Ethernet13
 IP    21183    [1], 10.0.0.53/32, algorithm ADMIN
                via M, 20.30.53.53, pop
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                 interface Ethernet13
 IP    21194    [1], 10.0.0.66/32, algorithm MIN-LATENCY
                via M, 20.30.66.66, pop
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                 interface Ethernet31
 IP    21195    [1], 10.0.0.66/32, algorithm MIN-TE
                via M, 20.30.66.66, pop
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                 interface Ethernet31
 IP    21196    [1], 10.0.0.66/32, algorithm ADMIN
                via M, 20.30.66.66, pop
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                 interface Ethernet31
 IP    21200    [1], 10.0.0.72/32, algorithm MIN-LATENCY
                via M, 20.30.72.72, pop
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                 interface Ethernet9
 IP    21201    [1], 10.0.0.72/32, algorithm MIN-TE
                via M, 20.30.72.72, pop
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                 interface Ethernet9
 IP    21202    [1], 10.0.0.72/32, algorithm ADMIN
                via M, 20.30.72.72, pop
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                 interface Ethernet9
 IP    21284    [1], 10.0.0.156/32, algorithm MIN-LATENCY
                via M, 20.30.156.156, pop
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                 interface Ethernet11
 IP    21285    [1], 10.0.0.156/32, algorithm MIN-TE
                via M, 20.30.156.156, pop
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                 interface Ethernet11
 IP    21286    [1], 10.0.0.156/32, algorithm ADMIN
                via M, 20.30.156.156, pop
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                 interface Ethernet11
 IP    21303    [1], 10.0.0.175/32, algorithm MIN-LATENCY
                via M, 20.30.221.221, swap 721303
                 payload autoDecide, ttlMode uniform, apply egress-acl
                 interface Ethernet15
 IP    21304    [1], 10.0.0.175/32, algorithm MIN-TE
                via M, 20.30.53.53, swap 21304
                 payload autoDecide, ttlMode uniform, apply egress-acl
                 interface Ethernet13
                via M, 20.30.66.66, swap 21304
                 payload autoDecide, ttlMode uniform, apply egress-acl
                 interface Ethernet31
                via M, 20.30.72.72, swap 21304
                 payload autoDecide, ttlMode uniform, apply egress-acl
                 interface Ethernet9
                via M, 20.30.156.156, swap 21304
                 payload autoDecide, ttlMode uniform, apply egress-acl
                 interface Ethernet11
                via M, 20.30.179.179, swap 21304
                 payload autoDecide, ttlMode uniform, apply egress-acl
                 interface Ethernet40
                via M, 20.30.221.221, swap 721304
                 payload autoDecide, ttlMode uniform, apply egress-acl
                 interface Ethernet15
 IP    21305    [1], 10.0.0.175/32, algorithm ADMIN
                via M, 20.30.131.131, forward
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                 interface Ethernet35
 IP    21307    [1], 10.0.0.179/32, algorithm MIN-LATENCY
                via M, 20.30.179.179, pop
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                 interface Ethernet40
 IP    21308    [1], 10.0.0.179/32, algorithm MIN-TE
                via M, 20.30.179.179, pop
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                 interface Ethernet40
 IP    21309    [1], 10.0.0.179/32, algorithm ADMIN
                via M, 20.30.179.179, pop
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                 interface Ethernet40
 IP    21349    [1], 10.0.0.221/32, algorithm MIN-LATENCY
                via M, 20.30.221.221, pop
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                 interface Ethernet15
 IP    21350    [1], 10.0.0.221/32, algorithm MIN-TE
                via M, 20.30.221.221, pop
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                 interface Ethernet15
 IP    21351    [1], 10.0.0.221/32, algorithm ADMIN
                via M, 20.30.221.221, pop
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                 interface Ethernet15
 IP    21581    [1], 2002::53/128, algorithm MIN-LATENCY
                via TI-LFA tunnel index 4, pop
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                    via fe80::5e07:58ff:fea3:aaa, Ethernet13, label imp-null(3)
                    backup via fe80::ea24:a6ff:fe96:548, Ethernet40, label 20 21581
 IP    21582    [1], 2002::53/128, algorithm MIN-TE
                via TI-LFA tunnel index 9, pop
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                    via fe80::5e07:58ff:fea3:aaa, Ethernet13, label imp-null(3)
                    backup via fe80::ea24:a6ff:fe96:548, Ethernet40, label 21704 21582
 IP    21583    [1], 2002::53/128, algorithm ADMIN
                via M, fe80::5e07:58ff:fea3:aaa, pop
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                 interface Ethernet13
 IP    21648    [1], 2002::120/128, algorithm MIN-LATENCY
                via M, fe80::be31:e2ff:fee1:ec2c, forward
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                 interface Ethernet3
 IP    21649    [1], 2002::120/128, algorithm MIN-TE
                via M, fe80::be31:e2ff:fee1:ec2c, forward
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                 interface Ethernet3
 IP    21650    [1], 2002::120/128, algorithm ADMIN
                via M, fe80::be31:e2ff:fee1:ec2c, forward
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                 interface Ethernet3
 IP    21684    [1], 2002::156/128, algorithm MIN-LATENCY
                via TI-LFA tunnel index 0, pop
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                    via fe80::d248:a1ff:feba:3c61, Ethernet11, label imp-null(3)
                    backup via fe80::5e07:58ff:fea3:aaa, Ethernet13, label 21703 21684
 IP    21685    [1], 2002::156/128, algorithm MIN-TE
                via TI-LFA tunnel index 10, pop
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                    via fe80::d248:a1ff:feba:3c61, Ethernet11, label imp-null(3)
                    backup via fe80::ea24:a6ff:fe96:548, Ethernet40, label 21704 21685
 IP    21686    [1], 2002::156/128, algorithm ADMIN
                via M, fe80::d248:a1ff:feba:3c61, pop
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                 interface Ethernet11
 IP    21703    [1], 2002::175/128, algorithm MIN-LATENCY
                via TI-LFA tunnel index 6, pop
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                    via fe80::5e07:58ff:fea3:aaa, Ethernet13, label 21703
                    backup via fe80::ea24:a6ff:fe96:548, Ethernet40, label 20
 IP    21704    [1], 2002::175/128, algorithm MIN-TE
                via M, fe80::5e07:58ff:fea3:aaa, forward
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                 interface Ethernet13
                via M, fe80::c214:b8ff:fe21:9790, forward
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                 interface Ethernet4
                via M, fe80::d248:a1ff:feba:3c61, forward
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                 interface Ethernet11
                via M, fe80::ea24:a6ff:fe96:548, forward
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                 interface Ethernet40
 IP    21707    [1], 2002::179/128, algorithm MIN-LATENCY
                via TI-LFA tunnel index 5, pop
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                    via fe80::ea24:a6ff:fe96:548, Ethernet40, label imp-null(3)
                    backup via fe80::5e07:58ff:fea3:aaa, Ethernet13, label 21703 21707
 IP    21708    [1], 2002::179/128, algorithm MIN-TE
                via TI-LFA tunnel index 11, pop
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                    via fe80::ea24:a6ff:fe96:548, Ethernet40, label imp-null(3)
                    backup via fe80::c214:b8ff:fe21:9790, Ethernet4, label 21704 21708
 IP    21709    [1], 2002::179/128, algorithm ADMIN
                via M, fe80::ea24:a6ff:fe96:548, pop
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                 interface Ethernet40
 IP    21745    [1], 2002::217/128, algorithm MIN-LATENCY
                via TI-LFA tunnel index 3, forward
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                    via fe80::c214:b8ff:fe21:9790, Ethernet4, label imp-null(3)
                    backup via fe80::5e07:58ff:fea3:aaa, Ethernet13, label 21703
 IP    21746    [1], 2002::217/128, algorithm MIN-TE
                via TI-LFA tunnel index 7, forward
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                    via fe80::c214:b8ff:fe21:9790, Ethernet4, label imp-null(3)
                    backup via fe80::d248:a1ff:feba:3c61, Ethernet11, label 21704
 IP    21747    [1], 2002::217/128, algorithm ADMIN
                via M, fe80::c214:b8ff:fe21:9790, forward
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                 interface Ethernet4
 B3    362144   [0]
                via I, ipv4, vrf FLEXALGO
 B3    362145   [0]
                via I, ipv4, vrf RED
 IA    378528   [1]
                via M, 20.30.53.53, pop
                 payload autoDecide, ttlMode uniform, apply egress-acl
                 interface Ethernet13
 IA    378529   [1]
                via M, fe80::5e07:58ff:fea3:aaa, pop
                 payload autoDecide, ttlMode uniform, apply egress-acl
                 interface Ethernet13
 IA    378530   [1]
                via M, 20.30.84.84, pop
                 payload autoDecide, ttlMode uniform, apply egress-acl
                 interface Ethernet12
 IA    378531   [1]
                via M, fe80::5a70:7fff:fe9f:c403, pop
                 payload autoDecide, ttlMode uniform, apply egress-acl
                 interface Ethernet12
 IA    378532   [1]
                via M, fe80::c214:b8ff:fe21:9790, pop
                 payload autoDecide, ttlMode uniform, apply egress-acl
                 interface Ethernet4
 IA    378533   [1]
                via M, 20.30.131.131, pop
                 payload autoDecide, ttlMode uniform, apply egress-acl
                 interface Ethernet35
 IA    378534   [1]
                via M, 20.30.120.120, pop
                 payload autoDecide, ttlMode uniform, apply egress-acl
                 interface Ethernet3
 IA    378535   [1]
                via M, fe80::be31:e2ff:fee1:ec2c, pop
                 payload autoDecide, ttlMode uniform, apply egress-acl
                 interface Ethernet3
 IA    378536   [1]
                via M, 20.30.72.72, pop
                 payload autoDecide, ttlMode uniform, apply egress-acl
                 interface Ethernet9
 IA    378537   [1]
                via M, 20.30.66.66, pop
                 payload autoDecide, ttlMode uniform, apply egress-acl
                 interface Ethernet31
 IA    378538   [1]
                via M, 20.30.179.179, pop
                 payload autoDecide, ttlMode uniform, apply egress-acl
                 interface Ethernet40
 IA    378539   [1]
                via M, fe80::ea24:a6ff:fe96:548, pop
                 payload autoDecide, ttlMode uniform, apply egress-acl
                 interface Ethernet40
 IA    378540   [1]
                via M, 20.30.156.156, pop
                 payload autoDecide, ttlMode uniform, apply egress-acl
                 interface Ethernet11
 IA    378541   [1]
                via M, fe80::d248:a1ff:feba:3c61, pop
                 payload autoDecide, ttlMode uniform, apply egress-acl
                 interface Ethernet11
 IA    378542   [1]
                via M, 20.30.221.221, pop
                 payload autoDecide, ttlMode uniform, apply egress-acl
                 interface Ethernet15
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
BGP is disabled for VRF default
BGP routing table information for VRF default
Router identifier 0.0.0.0, local AS number 0
Route status codes: * - valid, > - active, S - Stale, E - ECMP head, e - ECMP
                    c - Contributing to ECMP, % - Pending best path selection
Origin codes: i - IGP, e - EGP, ? - incomplete
AS Path Attributes: Or-ID - Originator ID, C-LST - Cluster List, LL Nexthop - Link Local Nexthop

          Network                Next Hop              Metric  LocPref Weight  Path
```

## show bgp vpn-ipv4

```text
BGP is disabled for VRF default
```

## show bgp vpn-ipv6

```text
BGP is disabled for VRF default
```

## show bgp ipv4 labeled-unicast

```text
BGP is disabled for VRF default
```

## show bgp neighbors

```text
BGP is disabled for VRF default

```

## show tunnel rib system-tunnel-rib brief

```text
Tunnel RIB: system-tunnel-rib
Endpoint        Tunnel Type     Index(es)   Tunnel Preference   IGP Preference 
-------------- --------------- ----------- ------------------- ----------------
10.0.0.53/32    IS-IS SR IPv4   10          65                  115            
10.0.0.66/32    IS-IS SR IPv4   13          65                  115            
10.0.0.72/32    IS-IS SR IPv4   14          65                  115            
10.0.0.84/32    IS-IS SR IPv4   8           65                  115            
10.0.0.131/32   IS-IS SR IPv4   9           65                  115            
10.0.0.156/32   IS-IS SR IPv4   11          65                  115            
10.0.0.175/32   IS-IS SR IPv4   7           65                  115            
10.0.0.179/32   IS-IS SR IPv4   12          65                  115            
10.0.0.221/32   IS-IS SR IPv4   15          65                  115            
2002::120/128   IS-IS SR IPv6   2           65                  115            
2002::175/128   IS-IS SR IPv6   3           65                  115            
2002::217/128   IS-IS SR IPv6   4           65                  115            
2002::53/128    IS-IS SR IPv6   6           65                  115            
2002::156/128   IS-IS SR IPv6   5           65                  115            
2002::179/128   IS-IS SR IPv6   1           65                  115            

   IGP Metric    Metric Type
---------------- -----------
   10            metric     
   20            metric     
   20            metric     
   20            metric     
   10            metric     
   10            metric     
   20            metric     
   10            metric     
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
 Endpoint        Color   Tunnel Type       Index(es)    Tunnel Preference    IGP Preference    IGP Metric   Metric Type
--------------- ------- ----------------- ------------ -------------------- ----------------- ------------- -----------
 10.0.0.53/32    128     IS-IS FlexAlgo    8            65                   115               10000        metric     
 10.0.0.53/32    129     IS-IS FlexAlgo    3            65                   115               100          metric     
 10.0.0.53/32    130     IS-IS FlexAlgo    1            65                   115               10           metric     
 10.0.0.66/32    128     IS-IS FlexAlgo    5            65                   115               10000        metric     
 10.0.0.66/32    129     IS-IS FlexAlgo    13           65                   115               100          metric     
 10.0.0.66/32    130     IS-IS FlexAlgo    33           65                   115               10           metric     
 10.0.0.72/32    128     IS-IS FlexAlgo    11           65                   115               10000        metric     
 10.0.0.72/32    129     IS-IS FlexAlgo    10           65                   115               100          metric     
 10.0.0.72/32    130     IS-IS FlexAlgo    32           65                   115               10           metric     
 10.0.0.156/32   128     IS-IS FlexAlgo    14           65                   115               10000        metric     
 10.0.0.156/32   129     IS-IS FlexAlgo    6            65                   115               100          metric     
 10.0.0.156/32   130     IS-IS FlexAlgo    37           65                   115               10           metric     
 10.0.0.175/32   128     IS-IS FlexAlgo    7            65                   115               10010        metric     
 10.0.0.175/32   129     IS-IS FlexAlgo    2            65                   115               110          metric     
 10.0.0.175/32   130     IS-IS FlexAlgo    28           65                   115               20           metric     
 10.0.0.179/32   128     IS-IS FlexAlgo    15           65                   115               10000        metric     
 10.0.0.179/32   129     IS-IS FlexAlgo    9            65                   115               100          metric     
 10.0.0.179/32   130     IS-IS FlexAlgo    34           65                   115               10           metric     
 10.0.0.221/32   128     IS-IS FlexAlgo    4            65                   115               10000        metric     
 10.0.0.221/32   129     IS-IS FlexAlgo    12           65                   115               100          metric     
 10.0.0.221/32   130     IS-IS FlexAlgo    38           65                   115               10           metric     
 2002::179/128   128     IS-IS FlexAlgo    23           65                   115               10000        metric     
 2002::179/128   129     IS-IS FlexAlgo    24           65                   115               100          metric     
 2002::179/128   130     IS-IS FlexAlgo    35           65                   115               10           metric     
 2002::120/128   128     IS-IS FlexAlgo    30           65                   115               10000        metric     
 2002::120/128   129     IS-IS FlexAlgo    31           65                   115               100          metric     
 2002::120/128   130     IS-IS FlexAlgo    29           65                   115               10           metric     
 2002::156/128   128     IS-IS FlexAlgo    21           65                   115               10000        metric     
 2002::156/128   129     IS-IS FlexAlgo    25           65                   115               100          metric     
 2002::156/128   130     IS-IS FlexAlgo    36           65                   115               10           metric     
 2002::217/128   128     IS-IS FlexAlgo    22           65                   115               10000        metric     
 2002::217/128   129     IS-IS FlexAlgo    16           65                   115               100          metric     
 2002::217/128   130     IS-IS FlexAlgo    27           65                   115               10           metric     
 2002::53/128    128     IS-IS FlexAlgo    19           65                   115               10000        metric     
 2002::53/128    129     IS-IS FlexAlgo    17           65                   115               100          metric     
 2002::53/128    130     IS-IS FlexAlgo    20           65                   115               10           metric     
 2002::175/128   128     IS-IS FlexAlgo    26           65                   115               10100        metric     
 2002::175/128   129     IS-IS FlexAlgo    18           65                   115               110          metric     

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
>C    10.0.0.30/32 [0 pref/0 metric] updated 00:53:22 ago
         via Loopback0, directly connected
>C    20.30.53.0/24 [0 pref/0 metric] updated 00:38:42 ago
         via Ethernet13, directly connected
>C    20.30.66.0/24 [0 pref/0 metric] updated 00:50:07 ago
         via Ethernet31, directly connected
>C    20.30.72.0/24 [0 pref/0 metric] updated 00:50:07 ago
         via Ethernet9, directly connected
>C    20.30.84.0/24 [0 pref/0 metric] updated 00:50:06 ago
         via Ethernet12, directly connected
>C    20.30.120.0/24 [0 pref/0 metric] updated 00:50:06 ago
         via Ethernet3, directly connected
>C    20.30.124.0/24 [0 pref/0 metric] updated 00:50:07 ago
         via Ethernet17, directly connected
>C    20.30.128.0/24 [0 pref/0 metric] updated 00:50:05 ago
         via Ethernet19, directly connected
>C    20.30.131.0/24 [0 pref/0 metric] updated 00:50:07 ago
         via Ethernet35, directly connected
>C    20.30.156.0/24 [0 pref/0 metric] updated 00:50:05 ago
         via Ethernet11, directly connected
>C    20.30.179.0/24 [0 pref/0 metric] updated 00:50:06 ago
         via Ethernet40, directly connected
>C    20.30.184.0/24 [0 pref/0 metric] updated 00:50:06 ago
         via Ethernet7, directly connected
>C    20.30.214.0/24 [0 pref/0 metric] updated 00:50:07 ago
         via Ethernet5, directly connected
>C    20.30.217.0/24 [0 pref/0 metric] updated 00:50:06 ago
         via Ethernet4, directly connected
>C    20.30.221.0/24 [0 pref/0 metric] updated 00:50:01 ago
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
>P    0.0.0.0/8 [1 pref/0 metric] updated 00:53:20 ago
         via Null0, directly connected [NF]
>P    127.0.0.0/8 [1 pref/0 metric] updated 00:53:20 ago
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
>I    10.0.0.53/32 [115 pref/10 metric] updated 00:11:23 ago
         via 20.30.53.53, Ethernet13
>I    10.0.0.66/32 [115 pref/20 metric] updated 00:49:54 ago
         via 20.30.66.66, Ethernet31
>I    10.0.0.72/32 [115 pref/20 metric] updated 00:49:54 ago
         via 20.30.72.72, Ethernet9
>I    10.0.0.84/32 [115 pref/20 metric] updated 00:50:04 ago
         via 20.30.84.84, Ethernet12
>I    10.0.0.120/32 [115 pref/10 metric] updated 00:49:56 ago
         via 20.30.120.120, Ethernet3
>I    10.0.0.124/32 [115 pref/10 metric] updated 00:50:05 ago
         via 20.30.124.124, Ethernet17
>I    10.0.0.128/32 [115 pref/10 metric] updated 00:50:04 ago
         via 20.30.128.128, Ethernet19
>I    10.0.0.131/32 [115 pref/10 metric] updated 00:49:56 ago
         via 20.30.131.131, Ethernet35
>I    10.0.0.156/32 [115 pref/10 metric] updated 00:49:54 ago
         via 20.30.156.156, Ethernet11
>I    10.0.0.175/32 [115 pref/20 metric] updated 00:11:23 ago
         via 20.30.53.53, Ethernet13
         via 20.30.66.66, Ethernet31
         via 20.30.72.72, Ethernet9
         via 20.30.84.84, Ethernet12
         via 20.30.120.120, Ethernet3
         via 20.30.124.124, Ethernet17
         via 20.30.128.128, Ethernet19
         via 20.30.131.131, Ethernet35
>I    10.0.0.179/32 [115 pref/10 metric] updated 00:49:54 ago
         via 20.30.179.179, Ethernet40
>I    10.0.0.216/32 [115 pref/45 metric] updated 00:11:23 ago
         via 20.30.53.53, Ethernet13
         via 20.30.66.66, Ethernet31
         via 20.30.72.72, Ethernet9
         via 20.30.84.84, Ethernet12
         via 20.30.120.120, Ethernet3
         via 20.30.124.124, Ethernet17
         via 20.30.128.128, Ethernet19
         via 20.30.131.131, Ethernet35
>I    10.0.0.221/32 [115 pref/10 metric] updated 00:49:07 ago
         via 20.30.221.221, Ethernet15
>I    10.0.1.179/32 [115 pref/10 metric] updated 00:49:54 ago
         via 20.30.179.179, Ethernet40
>I    20.53.175.0/24 [115 pref/20 metric] updated 00:11:23 ago
         via 20.30.53.53, Ethernet13
>I    20.66.175.0/24 [115 pref/20 metric] updated 00:49:54 ago
         via 20.30.66.66, Ethernet31
>I    20.72.175.0/24 [115 pref/20 metric] updated 00:49:54 ago
         via 20.30.72.72, Ethernet9
>I    20.84.175.0/24 [115 pref/35 metric] updated 00:11:23 ago
         via 20.30.53.53, Ethernet13
         via 20.30.66.66, Ethernet31
         via 20.30.72.72, Ethernet9
         via 20.30.84.84, Ethernet12
         via 20.30.120.120, Ethernet3
         via 20.30.124.124, Ethernet17
         via 20.30.128.128, Ethernet19
         via 20.30.131.131, Ethernet35
>I    20.120.175.0/24 [115 pref/20 metric] updated 00:49:56 ago
         via 20.30.120.120, Ethernet3
>I    20.120.214.0/24 [115 pref/20 metric] updated 00:49:56 ago
         via 20.30.120.120, Ethernet3
>I    20.120.217.0/24 [115 pref/10 metric] updated 00:49:56 ago
         via 20.30.120.120, Ethernet3
>I    20.124.175.0/24 [115 pref/20 metric] updated 00:50:05 ago
         via 20.30.124.124, Ethernet17
>I    20.128.175.0/24 [115 pref/20 metric] updated 00:50:04 ago
         via 20.30.128.128, Ethernet19
>I    20.131.175.0/24 [115 pref/20 metric] updated 00:49:56 ago
         via 20.30.131.131, Ethernet35
>I    20.156.175.0/24 [115 pref/20 metric] updated 00:49:54 ago
         via 20.30.156.156, Ethernet11
>I    20.175.179.0/24 [115 pref/20 metric] updated 00:49:54 ago
         via 20.30.179.179, Ethernet40
>I    20.175.184.0/24 [115 pref/35 metric] updated 00:11:23 ago
         via 20.30.53.53, Ethernet13
         via 20.30.66.66, Ethernet31
         via 20.30.72.72, Ethernet9
         via 20.30.84.84, Ethernet12
         via 20.30.120.120, Ethernet3
         via 20.30.124.124, Ethernet17
         via 20.30.128.128, Ethernet19
         via 20.30.131.131, Ethernet35
>I    20.175.214.0/24 [115 pref/35 metric] updated 00:11:23 ago
         via 20.30.53.53, Ethernet13
         via 20.30.66.66, Ethernet31
         via 20.30.72.72, Ethernet9
         via 20.30.84.84, Ethernet12
         via 20.30.120.120, Ethernet3
         via 20.30.124.124, Ethernet17
         via 20.30.128.128, Ethernet19
         via 20.30.131.131, Ethernet35
>I    20.175.217.0/24 [115 pref/35 metric] updated 00:11:23 ago
         via 20.30.53.53, Ethernet13
         via 20.30.66.66, Ethernet31
         via 20.30.72.72, Ethernet9
         via 20.30.84.84, Ethernet12
         via 20.30.120.120, Ethernet3
         via 20.30.124.124, Ethernet17
         via 20.30.128.128, Ethernet19
         via 20.30.131.131, Ethernet35
>I    20.175.221.0/24 [115 pref/20 metric] updated 00:49:07 ago
         via 20.30.221.221, Ethernet15
>I    20.214.216.0/24 [115 pref/45 metric] updated 00:11:23 ago
         via 20.30.53.53, Ethernet13
         via 20.30.66.66, Ethernet31
         via 20.30.72.72, Ethernet9
         via 20.30.84.84, Ethernet12
         via 20.30.120.120, Ethernet3
         via 20.30.124.124, Ethernet17
         via 20.30.128.128, Ethernet19
         via 20.30.131.131, Ethernet35
>I    30.66.221.0/24 [115 pref/20 metric] updated 00:15:39 ago
         via 20.30.221.221, Ethernet15
>I    192.168.20.0/23 [115 pref/10 metric] updated 00:49:56 ago
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
>C    2001:0:30:53::/64 [0 pref/0 metric] updated 00:38:42 ago
         via Ethernet13, directly connected
>C    2001:0:30:66::/64 [0 pref/0 metric] updated 00:50:07 ago
         via Ethernet31, directly connected
>C    2001:0:30:72::/64 [0 pref/0 metric] updated 00:50:07 ago
         via Ethernet9, directly connected
>C    2001:0:30:84::/64 [0 pref/0 metric] updated 00:50:06 ago
         via Ethernet12, directly connected
>C    2001:0:30:120::/64 [0 pref/0 metric] updated 00:50:06 ago
         via Ethernet3, directly connected
>C    2001:0:30:124::/64 [0 pref/0 metric] updated 00:50:07 ago
         via Ethernet17, directly connected
>C    2001:0:30:128::/64 [0 pref/0 metric] updated 00:50:05 ago
         via Ethernet19, directly connected
>C    2001:0:30:131::/64 [0 pref/0 metric] updated 00:50:07 ago
         via Ethernet35, directly connected
>C    2001:0:30:156::/64 [0 pref/0 metric] updated 00:50:05 ago
         via Ethernet11, directly connected
>C    2001:0:30:179::/64 [0 pref/0 metric] updated 00:50:06 ago
         via Ethernet40, directly connected
>C    2001:0:30:184::/64 [0 pref/0 metric] updated 00:50:06 ago
         via Ethernet7, directly connected
>C    2001:0:30:214::/64 [0 pref/0 metric] updated 00:50:07 ago
         via Ethernet5, directly connected
>C    2001:0:30:217::/64 [0 pref/0 metric] updated 00:50:06 ago
         via Ethernet4, directly connected
>C    2001:0:30:221::/64 [0 pref/0 metric] updated 00:50:01 ago
         via Ethernet15, directly connected
>C    2002::30/128 [0 pref/0 metric] updated 00:53:22 ago
         via Loopback0, directly connected
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
>P    ::/96 [1 pref/0 metric] updated 00:53:20 ago
         via Null0, directly connected [NF]
>P    ::ffff:127.0.0.0/104 [1 pref/0 metric] updated 00:53:20 ago
         via :: [1 pref/1 metric] type ipv6
            via , directly connected
>P    fe80::/10 [1 pref/0 metric] updated 00:53:20 ago
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
>I    2001:0:53:175::/64 [115 pref/20 metric] updated 00:11:23 ago
         via fe80::5e07:58ff:fea3:aaa, Ethernet13
>I    2001:0:66:175::/64 [115 pref/30 metric] updated 00:11:23 ago
         via fe80::c214:b8ff:fe21:9790, Ethernet4
         via fe80::5e07:58ff:fea3:aaa, Ethernet13
         via fe80::ea24:a6ff:fe96:548, Ethernet40
         via fe80::5a70:7fff:fe9f:c403, Ethernet12
         via fe80::d248:a1ff:feba:3c61, Ethernet11
         via fe80::be31:e2ff:fee1:ec2c, Ethernet3
>I    2001:0:72:175::/64 [115 pref/30 metric] updated 00:11:23 ago
         via fe80::c214:b8ff:fe21:9790, Ethernet4
         via fe80::5e07:58ff:fea3:aaa, Ethernet13
         via fe80::ea24:a6ff:fe96:548, Ethernet40
         via fe80::5a70:7fff:fe9f:c403, Ethernet12
         via fe80::d248:a1ff:feba:3c61, Ethernet11
         via fe80::be31:e2ff:fee1:ec2c, Ethernet3
>I    2001:0:84:175::/64 [115 pref/20 metric] updated 00:50:04 ago
         via fe80::5a70:7fff:fe9f:c403, Ethernet12
>I    2001:0:120:175::/64 [115 pref/20 metric] updated 00:49:56 ago
         via fe80::be31:e2ff:fee1:ec2c, Ethernet3
>I    2001:0:120:214::/64 [115 pref/20 metric] updated 00:49:56 ago
         via fe80::be31:e2ff:fee1:ec2c, Ethernet3
>I    2001:0:128:175::/64 [115 pref/30 metric] updated 00:11:23 ago
         via fe80::c214:b8ff:fe21:9790, Ethernet4
         via fe80::5e07:58ff:fea3:aaa, Ethernet13
         via fe80::ea24:a6ff:fe96:548, Ethernet40
         via fe80::5a70:7fff:fe9f:c403, Ethernet12
         via fe80::d248:a1ff:feba:3c61, Ethernet11
         via fe80::be31:e2ff:fee1:ec2c, Ethernet3
>I    2001:0:131:175::/64 [115 pref/30 metric] updated 00:11:23 ago
         via fe80::c214:b8ff:fe21:9790, Ethernet4
         via fe80::5e07:58ff:fea3:aaa, Ethernet13
         via fe80::ea24:a6ff:fe96:548, Ethernet40
         via fe80::5a70:7fff:fe9f:c403, Ethernet12
         via fe80::d248:a1ff:feba:3c61, Ethernet11
         via fe80::be31:e2ff:fee1:ec2c, Ethernet3
>I    2001:0:156:175::/64 [115 pref/20 metric] updated 00:49:54 ago
         via fe80::d248:a1ff:feba:3c61, Ethernet11
>I    2001:0:175::/64 [115 pref/20 metric] updated 00:49:54 ago
         via fe80::ea24:a6ff:fe96:548, Ethernet40
>I    2001:0:175:184::/64 [115 pref/30 metric] updated 00:11:23 ago
         via fe80::c214:b8ff:fe21:9790, Ethernet4
         via fe80::5e07:58ff:fea3:aaa, Ethernet13
         via fe80::ea24:a6ff:fe96:548, Ethernet40
         via fe80::5a70:7fff:fe9f:c403, Ethernet12
         via fe80::d248:a1ff:feba:3c61, Ethernet11
         via fe80::be31:e2ff:fee1:ec2c, Ethernet3
>I    2001:0:175:214::/64 [115 pref/30 metric] updated 00:11:23 ago
         via fe80::c214:b8ff:fe21:9790, Ethernet4
         via fe80::5e07:58ff:fea3:aaa, Ethernet13
         via fe80::ea24:a6ff:fe96:548, Ethernet40
         via fe80::5a70:7fff:fe9f:c403, Ethernet12
         via fe80::d248:a1ff:feba:3c61, Ethernet11
         via fe80::be31:e2ff:fee1:ec2c, Ethernet3
>I    2001:0:175:217::/64 [115 pref/20 metric] updated 00:49:56 ago
         via fe80::c214:b8ff:fe21:9790, Ethernet4
>I    2001:0:175:221::/64 [115 pref/30 metric] updated 00:11:23 ago
         via fe80::c214:b8ff:fe21:9790, Ethernet4
         via fe80::5e07:58ff:fea3:aaa, Ethernet13
         via fe80::ea24:a6ff:fe96:548, Ethernet40
         via fe80::5a70:7fff:fe9f:c403, Ethernet12
         via fe80::d248:a1ff:feba:3c61, Ethernet11
         via fe80::be31:e2ff:fee1:ec2c, Ethernet3
>I    2002::53/128 [115 pref/10 metric] updated 00:11:23 ago
         via fe80::5e07:58ff:fea3:aaa, Ethernet13
>I    2002::120/128 [115 pref/10 metric] updated 00:49:56 ago
         via fe80::be31:e2ff:fee1:ec2c, Ethernet3
>I    2002::156/128 [115 pref/10 metric] updated 00:49:54 ago
         via fe80::d248:a1ff:feba:3c61, Ethernet11
>I    2002::175/128 [115 pref/20 metric] updated 00:11:23 ago
         via fe80::c214:b8ff:fe21:9790, Ethernet4
         via fe80::5e07:58ff:fea3:aaa, Ethernet13
         via fe80::ea24:a6ff:fe96:548, Ethernet40
         via fe80::5a70:7fff:fe9f:c403, Ethernet12
         via fe80::d248:a1ff:feba:3c61, Ethernet11
         via fe80::be31:e2ff:fee1:ec2c, Ethernet3
>I    2002::179/128 [115 pref/10 metric] updated 00:49:54 ago
         via fe80::ea24:a6ff:fe96:548, Ethernet40
>I    2002::184/128 [115 pref/30 metric] updated 00:11:23 ago
         via fe80::c214:b8ff:fe21:9790, Ethernet4
         via fe80::5e07:58ff:fea3:aaa, Ethernet13
         via fe80::ea24:a6ff:fe96:548, Ethernet40
         via fe80::5a70:7fff:fe9f:c403, Ethernet12
         via fe80::d248:a1ff:feba:3c61, Ethernet11
         via fe80::be31:e2ff:fee1:ec2c, Ethernet3
>I    2002::217/128 [115 pref/10 metric] updated 00:49:56 ago
         via fe80::c214:b8ff:fe21:9790, Ethernet4
```

## show platform sand l3 summary

```text
Number of vrfs: 4

Ipv4:
  Routes:       119  backlog:  0  unprogrammed:  0
  Adjacencies:  160  backlog:  0  unprogrammed:  0
Ipv6:
  Routes:       55   backlog:  0  unprogrammed:  0
  Adjacencies:  160  backlog:  0  unprogrammed:  0
Mpls:
  Routes:       68  backlog:  0  unprogrammed:  0
  Adjacencies:  19  backlog:  0  unprogrammed:  0

Jericho2 Ip Fecs:
  Non-ecmp fecs:  4152  ecmp fecs:  3  fec entries:  4170
Jericho2 Mpls Fecs:
  Non-ecmp fecs:  17  ecmp fecs:  2  fec entries:  29
Jericho2 Vxlan Tunnel Fecs:
  Non-ecmp fecs:  0  ecmp fecs:  0  fec entries:  0
  Number of vxlan tunnels configured: 0

Jericho2 Lpm Routes:
  Routes:   119  unprogrammed:   0   
  Routes6:  55   unprogrammed6:  0   
  Backlog:  0  

Jericho2 Lpm:
  TCAM entries used:   3   Percent free:  99  ADS2 entries used:   10  Percent free:  99
  Pivot buckets used:  4   Rows used:     2   Entries Per Bucket:  2   Percent free:  99
  Route buckets used:  30  Rows used:     5   Entries Per Bucket:  5   Percent free:  99

Lem:
  IPv4  Host in Lem:            disabled
  IPv4  Prefix-lengths in Lem:  None    
  IPv6  Host in Lem:            disabled
  IPv6  Prefix-lengths in Lem:  None    
  Number of downloads:        1
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
  FixedSystem: 2
Egress Sflow rewrite entries in use (in each fap):
  FixedSystem: 0

Egress rewrite chains in backlog: resource-full 0, no-interface 0

Glem entries used per fap :
  FixedSystem: 4124

Jericho2 Fec:
  Maximum FEC hierarchy levels:  2
  ReusedEcmp:  31  allocs:  284  frees:  209  shuffles:  0  cmds:  0
  Zombies:     0    purges:    0
  Quarantine:  0/0  shuffles:  0  deletes:  0   
  Preserved FECs: 0
    First FEC preserved: never
    Last FEC preserved: never
  Fec insertion failures:  0
  Level1  Fecs:
    Non-ecmp fecs:            1   ecmp fecs:            1 
    Non-ecmp (Percent free):  99  ecmp (Percent free):  99
  Level2  Fecs:
    Non-ecmp fecs:            100  ecmp fecs:            6 
    Non-ecmp (Percent free):  99   ecmp (Percent free):  99
  Level3  Fecs:
    Non-ecmp fecs:            0    ecmp fecs:            0  
    Non-ecmp (Percent free):  100  ecmp (Percent free):  100

Lpm Detail:
  Requests:  475  cleanses:  56  batches:  56  avg batch size:  8

Jericho Arp:
  ArpTable writes:      25928  queued      0   
  IngressTable writes:  58385  queued      0   
  Coprocessors:         1      in CmdRing

Tunnel Counter Status
  Number of MPLS tunnels:                  16   
  Number of uncountable MPLS tunnels:      16   
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
|0  |10.0.0.53/32      |ROUTE| Et13               |1022 |103422  | 5c:07:58:a3:0a:aa |  -  |183528|   -   
|0  |10.0.0.66/32      |ROUTE| Et31               |1020 |103447  | e4:6d:7f:e3:c8:08 |  -  |183611|   -   
|0  |10.0.0.72/32      |ROUTE| Et9                |1009 |103450  | e0:9b:27:c4:c5:84 |  -  |183542|   -   
|0  |10.0.0.84/32      |ROUTE| Et12               |1014 |103423  | 58:70:7f:9f:c4:03 |  -  |183522|   -   
|0  |10.0.0.120/32     |ROUTE| Et3                |1017 |103449  | bc:31:e2:e1:ec:2c |  -  |183570|   -   
|0  |10.0.0.124/32     |ROUTE| Et17               |1016 |103421  | 64:6d:4e:32:e1:22 |  -  |183510|   -   
|0  |10.0.0.128/32     |ROUTE| Et19               |1021 |103424  | 60:53:75:13:ba:d8 |  -  |183520|   -   
|0  |10.0.0.131/32     |ROUTE| Et35               |1012 |103448  | 40:a6:b7:94:34:cb |  -  |183569|   -   
|0  |10.0.0.156/32     |ROUTE| Et11               |1019 |103452  | d0:48:a1:ba:3c:61 |  -  |183541|   -   
|0  |10.0.0.175/32     |ROUTE| Et13               |1022 |103422  | 5c:07:58:a3:0a:aa |16391|183595|   -   
|0  |10.0.0.175/32     |ROUTE| Et31               |1020 |103447  | e4:6d:7f:e3:c8:08 |16391|183596|   -   
|0  |10.0.0.175/32     |ROUTE| Et3                |1017 |103449  | bc:31:e2:e1:ec:2c |16391|183597|   -   
|0  |10.0.0.175/32     |ROUTE| Et35               |1012 |103448  | 40:a6:b7:94:34:cb |16391|183598|   -   
|0  |10.0.0.175/32     |ROUTE| Et12               |1014 |103423  | 58:70:7f:9f:c4:03 |16391|183599|   -   
|0  |10.0.0.175/32     |ROUTE| Et9                |1009 |103450  | e0:9b:27:c4:c5:84 |16391|183600|   -   
|0  |10.0.0.175/32     |ROUTE| Et19               |1021 |103424  | 60:53:75:13:ba:d8 |16391|183601|   -   
|0  |10.0.0.175/32     |ROUTE| Et17               |1016 |103421  | 64:6d:4e:32:e1:22 |16391|183602|   -   
|0  |10.0.0.179/32     |ROUTE| Et40               |1015 |103468  | e8:24:a6:96:05:48 |  -  |183610|   -   
|0  |10.0.0.216/32     |ROUTE| Et13               |1022 |103422  | 5c:07:58:a3:0a:aa |16391|183595|   -   
|0  |10.0.0.216/32     |ROUTE| Et31               |1020 |103447  | e4:6d:7f:e3:c8:08 |16391|183596|   -   
|0  |10.0.0.216/32     |ROUTE| Et3                |1017 |103449  | bc:31:e2:e1:ec:2c |16391|183597|   -   
|0  |10.0.0.216/32     |ROUTE| Et35               |1012 |103448  | 40:a6:b7:94:34:cb |16391|183598|   -   
|0  |10.0.0.216/32     |ROUTE| Et12               |1014 |103423  | 58:70:7f:9f:c4:03 |16391|183599|   -   
|0  |10.0.0.216/32     |ROUTE| Et9                |1009 |103450  | e0:9b:27:c4:c5:84 |16391|183600|   -   
|0  |10.0.0.216/32     |ROUTE| Et19               |1021 |103424  | 60:53:75:13:ba:d8 |16391|183601|   -   
|0  |10.0.0.216/32     |ROUTE| Et17               |1016 |103421  | 64:6d:4e:32:e1:22 |16391|183602|   -   
|0  |10.0.0.221/32     |ROUTE| Et15               |1006 |103425  | 30:c5:07:84:3e:79 |  -  |183540|   -   
|0  |10.0.1.179/32     |ROUTE| Et40               |1015 |103468  | e8:24:a6:96:05:48 |  -  |183610|   -   
|0  |20.30.53.0/32     |TRAP | CoppSystemIpBcast  |0    |  -     | BcastReceive      |  -  |314666|   -   
|0  |20.30.53.30/32    |TRAP | CoppSystemIpUcast  |0    |  -     | Receive           |  -  |314667|   -   
|0  |20.30.53.53/32    |ROUTE| Et13               |1022 |103422  | 5c:07:58:a3:0a:aa |  -  |183571|   -   
|0  |20.30.53.255/32   |TRAP | CoppSystemIpBcast  |0    |  -     | BcastReceive      |  -  |314666|   -   
|0  |20.30.53.0/24     |TRAP | CoppSystemL3DstMiss|1022 |1022    | ArpTrap           |  -  |315693|   -   
|0  |20.30.66.0/32     |TRAP | CoppSystemIpBcast  |0    |  -     | BcastReceive      |  -  |314666|   -   
|0  |20.30.66.30/32    |TRAP | CoppSystemIpUcast  |0    |  -     | Receive           |  -  |314667|   -   
|0  |20.30.66.66/32    |ROUTE| Et31               |1020 |103447  | e4:6d:7f:e3:c8:08 |  -  |183550|   -   
|0  |20.30.66.255/32   |TRAP | CoppSystemIpBcast  |0    |  -     | BcastReceive      |  -  |314666|   -   
|0  |20.30.66.0/24     |TRAP | CoppSystemL3DstMiss|1020 |1020    | ArpTrap           |  -  |315691|   -   
|0  |20.30.72.0/32     |TRAP | CoppSystemIpBcast  |0    |  -     | BcastReceive      |  -  |314666|   -   
|0  |20.30.72.30/32    |TRAP | CoppSystemIpUcast  |0    |  -     | Receive           |  -  |314667|   -   
|0  |20.30.72.72/32    |ROUTE| Et9                |1009 |103450  | e0:9b:27:c4:c5:84 |  -  |183553|   -   
|0  |20.30.72.255/32   |TRAP | CoppSystemIpBcast  |0    |  -     | BcastReceive      |  -  |314666|   -   
|0  |20.30.72.0/24     |TRAP | CoppSystemL3DstMiss|1009 |1009    | ArpTrap           |  -  |315680|   -   
|0  |20.30.84.0/32     |TRAP | CoppSystemIpBcast  |0    |  -     | BcastReceive      |  -  |314666|   -   
|0  |20.30.84.30/32    |TRAP | CoppSystemIpUcast  |0    |  -     | Receive           |  -  |314667|   -   
|0  |20.30.84.84/32    |ROUTE| Et12               |1014 |103423  | 58:70:7f:9f:c4:03 |  -  |183509|   -   
|0  |20.30.84.255/32   |TRAP | CoppSystemIpBcast  |0    |  -     | BcastReceive      |  -  |314666|   -   
|0  |20.30.84.0/24     |TRAP | CoppSystemL3DstMiss|1014 |1014    | ArpTrap           |  -  |315685|   -   
|0  |20.30.120.0/32    |TRAP | CoppSystemIpBcast  |0    |  -     | BcastReceive      |  -  |314666|   -   
|0  |20.30.120.30/32   |TRAP | CoppSystemIpUcast  |0    |  -     | Receive           |  -  |314667|   -   
|0  |20.30.120.120/32  |ROUTE| Et3                |1017 |103449  | bc:31:e2:e1:ec:2c |  -  |183552|   -   
|0  |20.30.120.255/32  |TRAP | CoppSystemIpBcast  |0    |  -     | BcastReceive      |  -  |314666|   -   
|0  |20.30.120.0/24    |TRAP | CoppSystemL3DstMiss|1017 |1017    | ArpTrap           |  -  |315688|   -   
|0  |20.30.124.0/32    |TRAP | CoppSystemIpBcast  |0    |  -     | BcastReceive      |  -  |314666|   -   
|0  |20.30.124.30/32   |TRAP | CoppSystemIpUcast  |0    |  -     | Receive           |  -  |314667|   -   
|0  |20.30.124.124/32  |ROUTE| Et17               |1016 |103421  | 64:6d:4e:32:e1:22 |  -  |183507|   -   
|0  |20.30.124.255/32  |TRAP | CoppSystemIpBcast  |0    |  -     | BcastReceive      |  -  |314666|   -   
|0  |20.30.124.0/24    |TRAP | CoppSystemL3DstMiss|1016 |1016    | ArpTrap           |  -  |315687|   -   
|0  |20.30.128.0/32    |TRAP | CoppSystemIpBcast  |0    |  -     | BcastReceive      |  -  |314666|   -   
|0  |20.30.128.30/32   |TRAP | CoppSystemIpUcast  |0    |  -     | Receive           |  -  |314667|   -   
|0  |20.30.128.128/32  |ROUTE| Et19               |1021 |103424  | 60:53:75:13:ba:d8 |  -  |183511|   -   
|0  |20.30.128.255/32  |TRAP | CoppSystemIpBcast  |0    |  -     | BcastReceive      |  -  |314666|   -   
|0  |20.30.128.0/24    |TRAP | CoppSystemL3DstMiss|1021 |1021    | ArpTrap           |  -  |315692|   -   
|0  |20.30.131.0/32    |TRAP | CoppSystemIpBcast  |0    |  -     | BcastReceive      |  -  |314666|   -   
|0  |20.30.131.30/32   |TRAP | CoppSystemIpUcast  |0    |  -     | Receive           |  -  |314667|   -   
|0  |20.30.131.131/32  |ROUTE| Et35               |1012 |103448  | 40:a6:b7:94:34:cb |  -  |183551|   -   
|0  |20.30.131.255/32  |TRAP | CoppSystemIpBcast  |0    |  -     | BcastReceive      |  -  |314666|   -   
|0  |20.30.131.0/24    |TRAP | CoppSystemL3DstMiss|1012 |1012    | ArpTrap           |  -  |315683|   -   
|0  |20.30.156.0/32    |TRAP | CoppSystemIpBcast  |0    |  -     | BcastReceive      |  -  |314666|   -   
|0  |20.30.156.30/32   |TRAP | CoppSystemIpUcast  |0    |  -     | Receive           |  -  |314667|   -   
|0  |20.30.156.156/32  |ROUTE| Et11               |1019 |103452  | d0:48:a1:ba:3c:61 |  -  |183583|   -   
|0  |20.30.156.255/32  |TRAP | CoppSystemIpBcast  |0    |  -     | BcastReceive      |  -  |314666|   -   
|0  |20.30.156.0/24    |TRAP | CoppSystemL3DstMiss|1019 |1019    | ArpTrap           |  -  |315690|   -   
|0  |20.30.179.0/32    |TRAP | CoppSystemIpBcast  |0    |  -     | BcastReceive      |  -  |314666|   -   
|0  |20.30.179.30/32   |TRAP | CoppSystemIpUcast  |0    |  -     | Receive           |  -  |314667|   -   
|0  |20.30.179.179/32  |ROUTE| Et40               |1015 |103468  | e8:24:a6:96:05:48 |  -  |183549|   -   
|0  |20.30.179.255/32  |TRAP | CoppSystemIpBcast  |0    |  -     | BcastReceive      |  -  |314666|   -   
|0  |20.30.179.0/24    |TRAP | CoppSystemL3DstMiss|1015 |1015    | ArpTrap           |  -  |315686|   -   
|0  |20.30.184.0/32    |TRAP | CoppSystemIpBcast  |0    |  -     | BcastReceive      |  -  |314666|   -   
|0  |20.30.184.30/32   |TRAP | CoppSystemIpUcast  |0    |  -     | Receive           |  -  |314667|   -   
|0  |20.30.184.255/32  |TRAP | CoppSystemIpBcast  |0    |  -     | BcastReceive      |  -  |314666|   -   
|0  |20.30.184.0/24    |TRAP | CoppSystemL3DstMiss|1010 |1010    | ArpTrap           |  -  |315681|   -   
|0  |20.30.214.0/32    |TRAP | CoppSystemIpBcast  |0    |  -     | BcastReceive      |  -  |314666|   -   
|0  |20.30.214.30/32   |TRAP | CoppSystemIpUcast  |0    |  -     | Receive           |  -  |314667|   -   
|0  |20.30.214.255/32  |TRAP | CoppSystemIpBcast  |0    |  -     | BcastReceive      |  -  |314666|   -   
|0  |20.30.214.0/24    |TRAP | CoppSystemL3DstMiss|1007 |1007    | ArpTrap           |  -  |315678|   -   
|0  |20.30.217.0/32    |TRAP | CoppSystemIpBcast  |0    |  -     | BcastReceive      |  -  |314666|   -   
|0  |20.30.217.30/32   |TRAP | CoppSystemIpUcast  |0    |  -     | Receive           |  -  |314667|   -   
|0  |20.30.217.255/32  |TRAP | CoppSystemIpBcast  |0    |  -     | BcastReceive      |  -  |314666|   -   
|0  |20.30.217.0/24    |TRAP | CoppSystemL3DstMiss|1008 |1008    | ArpTrap           |  -  |315679|   -   
|0  |20.30.221.0/32    |TRAP | CoppSystemIpBcast  |0    |  -     | BcastReceive      |  -  |314666|   -   
|0  |20.30.221.30/32   |TRAP | CoppSystemIpUcast  |0    |  -     | Receive           |  -  |314667|   -   
|0  |20.30.221.221/32  |ROUTE| Et15               |1006 |103425  | 30:c5:07:84:3e:79 |  -  |183525|   -   
|0  |20.30.221.255/32  |TRAP | CoppSystemIpBcast  |0    |  -     | BcastReceive      |  -  |314666|   -   
|0  |20.30.221.0/24    |TRAP | CoppSystemL3DstMiss|1006 |1006    | ArpTrap           |  -  |315677|   -   
|0  |20.53.175.0/24    |ROUTE| Et13               |1022 |103422  | 5c:07:58:a3:0a:aa |  -  |183528|   -   
|0  |20.66.175.0/24    |ROUTE| Et31               |1020 |103447  | e4:6d:7f:e3:c8:08 |  -  |183611|   -   
|0  |20.72.175.0/24    |ROUTE| Et9                |1009 |103450  | e0:9b:27:c4:c5:84 |  -  |183542|   -   
|0  |20.84.175.0/24    |ROUTE| Et13               |1022 |103422  | 5c:07:58:a3:0a:aa |16391|183595|   -   
|0  |20.84.175.0/24    |ROUTE| Et31               |1020 |103447  | e4:6d:7f:e3:c8:08 |16391|183596|   -   
|0  |20.84.175.0/24    |ROUTE| Et3                |1017 |103449  | bc:31:e2:e1:ec:2c |16391|183597|   -   
|0  |20.84.175.0/24    |ROUTE| Et35               |1012 |103448  | 40:a6:b7:94:34:cb |16391|183598|   -   
|0  |20.84.175.0/24    |ROUTE| Et12               |1014 |103423  | 58:70:7f:9f:c4:03 |16391|183599|   -   
|0  |20.84.175.0/24    |ROUTE| Et9                |1009 |103450  | e0:9b:27:c4:c5:84 |16391|183600|   -   
|0  |20.84.175.0/24    |ROUTE| Et19               |1021 |103424  | 60:53:75:13:ba:d8 |16391|183601|   -   
|0  |20.84.175.0/24    |ROUTE| Et17               |1016 |103421  | 64:6d:4e:32:e1:22 |16391|183602|   -   
|0  |20.120.175.0/24   |ROUTE| Et3                |1017 |103449  | bc:31:e2:e1:ec:2c |  -  |183570|   -   
|0  |20.120.214.0/24   |ROUTE| Et3                |1017 |103449  | bc:31:e2:e1:ec:2c |  -  |183570|   -   
|0  |20.120.217.0/24   |ROUTE| Et3                |1017 |103449  | bc:31:e2:e1:ec:2c |  -  |183570|   -   
|0  |20.124.175.0/24   |ROUTE| Et17               |1016 |103421  | 64:6d:4e:32:e1:22 |  -  |183510|   -   
|0  |20.128.175.0/24   |ROUTE| Et19               |1021 |103424  | 60:53:75:13:ba:d8 |  -  |183520|   -   
|0  |20.131.175.0/24   |ROUTE| Et35               |1012 |103448  | 40:a6:b7:94:34:cb |  -  |183569|   -   
|0  |20.156.175.0/24   |ROUTE| Et11               |1019 |103452  | d0:48:a1:ba:3c:61 |  -  |183541|   -   
|0  |20.175.179.0/24   |ROUTE| Et40               |1015 |103468  | e8:24:a6:96:05:48 |  -  |183610|   -   
|0  |20.175.184.0/24   |ROUTE| Et13               |1022 |103422  | 5c:07:58:a3:0a:aa |16391|183595|   -   
|0  |20.175.184.0/24   |ROUTE| Et31               |1020 |103447  | e4:6d:7f:e3:c8:08 |16391|183596|   -   
|0  |20.175.184.0/24   |ROUTE| Et3                |1017 |103449  | bc:31:e2:e1:ec:2c |16391|183597|   -   
|0  |20.175.184.0/24   |ROUTE| Et35               |1012 |103448  | 40:a6:b7:94:34:cb |16391|183598|   -   
|0  |20.175.184.0/24   |ROUTE| Et12               |1014 |103423  | 58:70:7f:9f:c4:03 |16391|183599|   -   
|0  |20.175.184.0/24   |ROUTE| Et9                |1009 |103450  | e0:9b:27:c4:c5:84 |16391|183600|   -   
|0  |20.175.184.0/24   |ROUTE| Et19               |1021 |103424  | 60:53:75:13:ba:d8 |16391|183601|   -   
|0  |20.175.184.0/24   |ROUTE| Et17               |1016 |103421  | 64:6d:4e:32:e1:22 |16391|183602|   -   
|0  |20.175.214.0/24   |ROUTE| Et13               |1022 |103422  | 5c:07:58:a3:0a:aa |16391|183595|   -   
|0  |20.175.214.0/24   |ROUTE| Et31               |1020 |103447  | e4:6d:7f:e3:c8:08 |16391|183596|   -   
|0  |20.175.214.0/24   |ROUTE| Et3                |1017 |103449  | bc:31:e2:e1:ec:2c |16391|183597|   -   
|0  |20.175.214.0/24   |ROUTE| Et35               |1012 |103448  | 40:a6:b7:94:34:cb |16391|183598|   -   
|0  |20.175.214.0/24   |ROUTE| Et12               |1014 |103423  | 58:70:7f:9f:c4:03 |16391|183599|   -   
|0  |20.175.214.0/24   |ROUTE| Et9                |1009 |103450  | e0:9b:27:c4:c5:84 |16391|183600|   -   
|0  |20.175.214.0/24   |ROUTE| Et19               |1021 |103424  | 60:53:75:13:ba:d8 |16391|183601|   -   
|0  |20.175.214.0/24   |ROUTE| Et17               |1016 |103421  | 64:6d:4e:32:e1:22 |16391|183602|   -   
|0  |20.175.217.0/24   |ROUTE| Et13               |1022 |103422  | 5c:07:58:a3:0a:aa |16391|183595|   -   
|0  |20.175.217.0/24   |ROUTE| Et31               |1020 |103447  | e4:6d:7f:e3:c8:08 |16391|183596|   -   
|0  |20.175.217.0/24   |ROUTE| Et3                |1017 |103449  | bc:31:e2:e1:ec:2c |16391|183597|   -   
|0  |20.175.217.0/24   |ROUTE| Et35               |1012 |103448  | 40:a6:b7:94:34:cb |16391|183598|   -   
|0  |20.175.217.0/24   |ROUTE| Et12               |1014 |103423  | 58:70:7f:9f:c4:03 |16391|183599|   -   
|0  |20.175.217.0/24   |ROUTE| Et9                |1009 |103450  | e0:9b:27:c4:c5:84 |16391|183600|   -   
|0  |20.175.217.0/24   |ROUTE| Et19               |1021 |103424  | 60:53:75:13:ba:d8 |16391|183601|   -   
|0  |20.175.217.0/24   |ROUTE| Et17               |1016 |103421  | 64:6d:4e:32:e1:22 |16391|183602|   -   
|0  |20.175.221.0/24   |ROUTE| Et15               |1006 |103425  | 30:c5:07:84:3e:79 |  -  |183540|   -   
|0  |20.214.216.0/24   |ROUTE| Et13               |1022 |103422  | 5c:07:58:a3:0a:aa |16391|183595|   -   
|0  |20.214.216.0/24   |ROUTE| Et31               |1020 |103447  | e4:6d:7f:e3:c8:08 |16391|183596|   -   
|0  |20.214.216.0/24   |ROUTE| Et3                |1017 |103449  | bc:31:e2:e1:ec:2c |16391|183597|   -   
|0  |20.214.216.0/24   |ROUTE| Et35               |1012 |103448  | 40:a6:b7:94:34:cb |16391|183598|   -   
|0  |20.214.216.0/24   |ROUTE| Et12               |1014 |103423  | 58:70:7f:9f:c4:03 |16391|183599|   -   
|0  |20.214.216.0/24   |ROUTE| Et9                |1009 |103450  | e0:9b:27:c4:c5:84 |16391|183600|   -   
|0  |20.214.216.0/24   |ROUTE| Et19               |1021 |103424  | 60:53:75:13:ba:d8 |16391|183601|   -   
|0  |20.214.216.0/24   |ROUTE| Et17               |1016 |103421  | 64:6d:4e:32:e1:22 |16391|183602|   -   
|0  |30.66.221.0/24    |ROUTE| Et15               |1006 |103425  | 30:c5:07:84:3e:79 |  -  |183540|   -   
|0  |127.0.0.0/8       |TRAP | CoppSystemL3DstMiss|0    |  -     | ArpTrap           |  -  |314671|   -   
|0  |192.168.20.0/23   |ROUTE| Et3                |1017 |103449  | bc:31:e2:e1:ec:2c |  -  |183570|   -   
|0  |0.0.0.0/0         |TRAP | CoppSystemL3LpmOver|0    |  -     | SlowReceive       |  -  |314669|   -   
|1  |0.0.0.0/8         |DROP | DROP               |0    |  -     |                   |  -  |183504|   -   
|1  |10.0.0.30/32      |TRAP | CoppSystemIpUcast  |0    |  -     | Receive           |  -  |314667|   -   
|1  |127.0.0.0/8       |TRAP | CoppSystemL3DstMiss|0    |  -     | ArpTrap           |  -  |314671|   -   
|1  |0.0.0.0/0         |TRAP | CoppSystemL3LpmOver|0    |  -     | SlowReceive       |  -  |314669|   -   
|2  |0.0.0.0/8         |DROP | DROP               |0    |  -     |                   |  -  |183505|   -   
|2  |10.128.0.30/32    |TRAP | CoppSystemIpUcast  |0    |  -     | Receive           |  -  |314667|   -   
|2  |127.0.0.0/8       |TRAP | CoppSystemL3DstMiss|0    |  -     | ArpTrap           |  -  |314671|   -   
|2  |0.0.0.0/0         |TRAP | CoppSystemL3LpmOver|0    |  -     | SlowReceive       |  -  |314669|   -   
|3  |0.0.0.0/8         |DROP | DROP               |0    |  -     |                   |  -  |183506|   -   
|3  |127.0.0.0/8       |TRAP | CoppSystemL3DstMiss|0    |  -     | ArpTrap           |  -  |314671|   -   
|3  |192.168.20.0/32   |TRAP | CoppSystemIpBcast  |0    |  -     | BcastReceive      |  -  |314666|   -   
|3  |192.168.20.30/32  |TRAP | CoppSystemIpUcast  |0    |  -     | Receive           |  -  |314667|   -   
|3  |192.168.21.255/32 |TRAP | CoppSystemIpBcast  |0    |  -     | BcastReceive      |  -  |314666|   -   
|3  |192.168.20.0/23   |TRAP | CoppSystemL3DstMiss|0    |  -     | ArpTrap           |  -  |314671|   -   
|3  |0.0.0.0/0         |TRAP | CoppSystemL3DstMiss|0    |  -     | ArpTrap           |  -  |314671|   -   

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
|16384|183584|ROUTE| Et4                |1008 |103454  | c0:14:b8:21:97:90 |   -   
|16384|183585|ROUTE| Et13               |1022 |103422  | 5c:07:58:a3:0a:aa |   -   
|16384|183586|ROUTE| Et11               |1019 |103452  | d0:48:a1:ba:3c:61 |   -   
|16384|183587|ROUTE| Et40               |1015 |103468  | e8:24:a6:96:05:48 |   -   
|16387|183531|ROUTE| Et13               |1022 |103427  | 5c:07:58:a3:0a:aa |Mswap 0
|16388|183543|ROUTE| Et3                |1017 |103460  | bc:31:e2:e1:ec:2c |Mswap 20175
|16388|183544|ROUTE| Et9                |1009 |103483  | e0:9b:27:c4:c5:84 |Mswap 20175
|16388|183545|ROUTE| Et12               |1014 |103436  | 58:70:7f:9f:c4:03 |Mswap 20175
|16388|183546|ROUTE| Et13               |1022 |103433  | 5c:07:58:a3:0a:aa |Mswap 20175
|16388|183547|ROUTE| Et35               |1012 |103461  | 40:a6:b7:94:34:cb |Mswap 20175
|16388|183548|ROUTE| Et31               |1020 |103484  | e4:6d:7f:e3:c8:08 |Mswap 20175
|16390|183589|ROUTE| Et4                |1008 |103454  | c0:14:b8:21:97:90 |   -   
|16390|183590|ROUTE| Et13               |1022 |103422  | 5c:07:58:a3:0a:aa |   -   
|16390|183591|ROUTE| Et3                |1017 |103449  | bc:31:e2:e1:ec:2c |   -   
|16390|183592|ROUTE| Et11               |1019 |103452  | d0:48:a1:ba:3c:61 |   -   
|16390|183593|ROUTE| Et12               |1014 |103423  | 58:70:7f:9f:c4:03 |   -   
|16390|183594|ROUTE| Et40               |1015 |103468  | e8:24:a6:96:05:48 |   -   
|16391|183595|ROUTE| Et13               |1022 |103422  | 5c:07:58:a3:0a:aa |   -   
|16391|183596|ROUTE| Et31               |1020 |103447  | e4:6d:7f:e3:c8:08 |   -   
|16391|183597|ROUTE| Et3                |1017 |103449  | bc:31:e2:e1:ec:2c |   -   
|16391|183598|ROUTE| Et35               |1012 |103448  | 40:a6:b7:94:34:cb |   -   
|16391|183599|ROUTE| Et12               |1014 |103423  | 58:70:7f:9f:c4:03 |   -   
|16391|183600|ROUTE| Et9                |1009 |103450  | e0:9b:27:c4:c5:84 |   -   
|16391|183601|ROUTE| Et19               |1021 |103424  | 60:53:75:13:ba:d8 |   -   
|16391|183602|ROUTE| Et17               |1016 |103421  | 64:6d:4e:32:e1:22 |   -   
|16398|183534|ROUTE| Et13               |1022 |103429  | 5c:07:58:a3:0a:aa |Mswap 21304
|16398|183535|ROUTE| Et40               |1015 |103475  | e8:24:a6:96:05:48 |Mswap 21304
|16398|183536|ROUTE| Et11               |1019 |103485  | d0:48:a1:ba:3c:61 |Mswap 21304
|16398|183537|ROUTE| Et31               |1020 |103476  | e4:6d:7f:e3:c8:08 |Mswap 21304
|16398|183538|ROUTE| Et15               |1006 |103426  | 30:c5:07:84:3e:79 |Mswap 721304
|16398|183539|ROUTE| Et9                |1009 |103477  | e0:9b:27:c4:c5:84 |Mswap 21304
|  -  |131072|ROUTE| FEC 183529         |   - |  -     |                   |   -   
|  -  |183502|DROP | DROP               |0    |  -     |                   |   -   
|  -  |183503|DROP | DROP               |0    |  -     |                   |   -   
|  -  |183504|DROP | DROP               |0    |  -     |                   |   -   
|  -  |183505|DROP | DROP               |0    |  -     |                   |   -   
|  -  |183506|DROP | DROP               |0    |  -     |                   |   -   
|  -  |183507|ROUTE| Et17               |1016 |103421  | 64:6d:4e:32:e1:22 |   -   
|  -  |183508|ROUTE| Et13               |1022 |103422  | 5c:07:58:a3:0a:aa |   -   
|  -  |183509|ROUTE| Et12               |1014 |103423  | 58:70:7f:9f:c4:03 |   -   
|  -  |183510|ROUTE| Et17               |1016 |103421  | 64:6d:4e:32:e1:22 |   -   
|  -  |183511|ROUTE| Et19               |1021 |103424  | 60:53:75:13:ba:d8 |   -   
|  -  |183512|ROUTE| Et15               |1006 |103425  | 30:c5:07:84:3e:79 |   -   
|  -  |183513|ROUTE| Et13               |1022 |103422  | 5c:07:58:a3:0a:aa |   -   
|  -  |183514|ROUTE| Et11               |1019 |103452  | d0:48:a1:ba:3c:61 |   -   
|  -  |183515|ROUTE| Et12               |1014 |103423  | 58:70:7f:9f:c4:03 |   -   
|  -  |183516|ROUTE| Et15               |1006 |103431  | 30:c5:07:84:3e:79 |Mswap 721303
|  -  |183517|ROUTE| Et40               |1015 |103468  | e8:24:a6:96:05:48 |   -   
|  -  |183519|ROUTE| Et40               |1015 |103468  | e8:24:a6:96:05:48 |   -   
|  -  |183520|ROUTE| Et19               |1021 |103424  | 60:53:75:13:ba:d8 |   -   
|  -  |183522|ROUTE| Et12               |1014 |103423  | 58:70:7f:9f:c4:03 |   -   
|  -  |183523|ROUTE| Et13               |1022 |103422  | 5c:07:58:a3:0a:aa |   -   
|  -  |183524|ROUTE| Et13               |1022 |103422  | 5c:07:58:a3:0a:aa |   -   
|  -  |183525|ROUTE| Et15               |1006 |103425  | 30:c5:07:84:3e:79 |   -   
|  -  |183526|ROUTE| Et12               |1014 |103423  | 58:70:7f:9f:c4:03 |   -   
|  -  |183527|ROUTE| Et12               |1014 |103423  | 58:70:7f:9f:c4:03 |   -   
|  -  |183528|ROUTE| Et13               |1022 |103422  | 5c:07:58:a3:0a:aa |   -   
|  -  |183529|ROUTE| Et13               |1022 |103435  | 5c:07:58:a3:0a:aa |Mpush 2
|  -  |183530|ROUTE| Et12               |1014 |103423  | 58:70:7f:9f:c4:03 |   -   
|  -  |183533|ROUTE| Et4                |1008 |103454  | c0:14:b8:21:97:90 |   -   
|  -  |183540|ROUTE| Et15               |1006 |103425  | 30:c5:07:84:3e:79 |   -   
|  -  |183541|ROUTE| Et11               |1019 |103452  | d0:48:a1:ba:3c:61 |   -   
|  -  |183542|ROUTE| Et9                |1009 |103450  | e0:9b:27:c4:c5:84 |   -   
|  -  |183549|ROUTE| Et40               |1015 |103468  | e8:24:a6:96:05:48 |   -   
|  -  |183550|ROUTE| Et31               |1020 |103447  | e4:6d:7f:e3:c8:08 |   -   
|  -  |183551|ROUTE| Et35               |1012 |103448  | 40:a6:b7:94:34:cb |   -   
|  -  |183552|ROUTE| Et3                |1017 |103449  | bc:31:e2:e1:ec:2c |   -   
|  -  |183553|ROUTE| Et9                |1009 |103450  | e0:9b:27:c4:c5:84 |   -   
|  -  |183561|ROUTE| Et4                |1008 |103454  | c0:14:b8:21:97:90 |   -   
|  -  |183562|ROUTE| Et3                |1017 |103449  | bc:31:e2:e1:ec:2c |   -   
|  -  |183568|ROUTE| Et13               |1022 |103422  | 5c:07:58:a3:0a:aa |   -   
|  -  |183569|ROUTE| Et35               |1012 |103448  | 40:a6:b7:94:34:cb |   -   
|  -  |183570|ROUTE| Et3                |1017 |103449  | bc:31:e2:e1:ec:2c |   -   
|  -  |183571|ROUTE| Et13               |1022 |103422  | 5c:07:58:a3:0a:aa |   -   
|  -  |183572|ROUTE| Et4                |1008 |103454  | c0:14:b8:21:97:90 |   -   
|  -  |183573|ROUTE| Et35               |1012 |103448  | 40:a6:b7:94:34:cb |   -   
|  -  |183574|ROUTE| Et40               |1015 |103468  | e8:24:a6:96:05:48 |   -   
|  -  |183575|ROUTE| Et11               |1019 |103452  | d0:48:a1:ba:3c:61 |   -   
|  -  |183576|ROUTE| Et3                |1017 |103449  | bc:31:e2:e1:ec:2c |   -   
|  -  |183577|ROUTE| Et4                |1008 |103454  | c0:14:b8:21:97:90 |   -   
|  -  |183578|ROUTE| Et3                |1017 |103449  | bc:31:e2:e1:ec:2c |   -   
|  -  |183579|ROUTE| Et3                |1017 |103449  | bc:31:e2:e1:ec:2c |   -   
|  -  |183580|ROUTE| Et4                |1008 |103454  | c0:14:b8:21:97:90 |   -   
|  -  |183581|ROUTE| Et4                |1008 |103454  | c0:14:b8:21:97:90 |   -   
|  -  |183582|ROUTE| Et11               |1019 |103452  | d0:48:a1:ba:3c:61 |   -   
|  -  |183583|ROUTE| Et11               |1019 |103452  | d0:48:a1:ba:3c:61 |   -   
|  -  |183588|ROUTE| Et13               |1022 |103430  | 5c:07:58:a3:0a:aa |Mpush 21703
|  -  |183610|ROUTE| Et40               |1015 |103468  | e8:24:a6:96:05:48 |   -   
|  -  |183611|ROUTE| Et31               |1020 |103447  | e4:6d:7f:e3:c8:08 |   -   
|  -  |183612|ROUTE| Et40               |1015 |103468  | e8:24:a6:96:05:48 |   -   
|  -  |183613|ROUTE| Et11               |1019 |103452  | d0:48:a1:ba:3c:61 |   -   
|  -  |183629|ROUTE| Et40               |1015 |103468  | e8:24:a6:96:05:48 |   -   
|  -  |183631|ROUTE| Et11               |1019 |103452  | d0:48:a1:ba:3c:61 |   -   
|  -  |183632|ROUTE| Et40               |1015 |103468  | e8:24:a6:96:05:48 |   -   
|  -  |183633|ROUTE| Et11               |1019 |103452  | d0:48:a1:ba:3c:61 |   -   
|  -  |183634|ROUTE| Et40               |1015 |103468  | e8:24:a6:96:05:48 |   -   
|  -  |183635|ROUTE| Et13               |1022 |103422  | 5c:07:58:a3:0a:aa |   -   
|  -  |183636|ROUTE| Et31               |1020 |103447  | e4:6d:7f:e3:c8:08 |   -   
|  -  |183637|ROUTE| Et11               |1019 |103452  | d0:48:a1:ba:3c:61 |   -   
|  -  |183641|ROUTE| Et9                |1009 |103450  | e0:9b:27:c4:c5:84 |   -   
|  -  |314666|TRAP | CoppSystemIpBcast  |0    |  -     | BcastReceive      |   -   
|  -  |314667|TRAP | CoppSystemIpUcast  |0    |  -     | Receive           |   -   
|  -  |314669|TRAP | CoppSystemL3LpmOver|0    |  -     | SlowReceive       |   -   
|  -  |314671|TRAP | CoppSystemL3DstMiss|0    |  -     | ArpTrap           |   -   
|  -  |315677|TRAP | CoppSystemL3DstMiss|1006 |1006    | ArpTrap           |   -   
|  -  |315678|TRAP | CoppSystemL3DstMiss|1007 |1007    | ArpTrap           |   -   
|  -  |315679|TRAP | CoppSystemL3DstMiss|1008 |1008    | ArpTrap           |   -   
|  -  |315680|TRAP | CoppSystemL3DstMiss|1009 |1009    | ArpTrap           |   -   
|  -  |315681|TRAP | CoppSystemL3DstMiss|1010 |1010    | ArpTrap           |   -   
|  -  |315683|TRAP | CoppSystemL3DstMiss|1012 |1012    | ArpTrap           |   -   
|  -  |315685|TRAP | CoppSystemL3DstMiss|1014 |1014    | ArpTrap           |   -   
|  -  |315686|TRAP | CoppSystemL3DstMiss|1015 |1015    | ArpTrap           |   -   
|  -  |315687|TRAP | CoppSystemL3DstMiss|1016 |1016    | ArpTrap           |   -   
|  -  |315688|TRAP | CoppSystemL3DstMiss|1017 |1017    | ArpTrap           |   -   
|  -  |315690|TRAP | CoppSystemL3DstMiss|1019 |1019    | ArpTrap           |   -   
|  -  |315691|TRAP | CoppSystemL3DstMiss|1020 |1020    | ArpTrap           |   -   
|  -  |315692|TRAP | CoppSystemL3DstMiss|1021 |1021    | ArpTrap           |   -   
|  -  |315693|TRAP | CoppSystemL3DstMiss|1022 |1022    | ArpTrap           |   -   

```

