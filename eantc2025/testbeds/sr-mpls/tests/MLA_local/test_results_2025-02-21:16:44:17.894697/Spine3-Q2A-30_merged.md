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

Uptime: 1 day, 2 hours and 6 minutes
Total memory: 8099700 kB
Free memory: 4932756 kB

```

## show lldp neighbors

```text
Last table change time   : 0:00:22 ago
Number of table inserts  : 107
Number of table deletes  : 84
Number of table drops    : 0
Number of table age-outs : 2

Port       Neighbor Device ID                   Neighbor Port ID            TTL
--------- ------------------------------------ ---------------------------- ---
Et2        Arista-PE32-Q2C-32.ns.eantc.de       Ethernet1                   120
Et3        H3C_M1A_120                          Ten-GigabitEthernet0/0/17   121
Et4        Nokia-SR1-217                        1610899524                  121
Et5        Nokia-SXR-214                        ethernet-1/4                120
Et6        Nokia-SXR-214                        ethernet-1/8                120
Et8        Nokia-SR1-217                        1610899528                  121
Et9        Ciena-5134-72                        2                           120
Et10       H3C_M1A_120                          Ten-GigabitEthernet0/0/23   121
Et11       Juniper-156-PTX10002-36QDD           590                         120
Et12       Ericsson_84_R6678                    5870.7f9f.c403              91 
Et13       Arrcus-53                            swp0                        120
Et15       30c5.0784.3e68                       et-bs/15                    121
Et17       Huawei_124_NetEngine_A816            GigabitEthernet0/2/4        120
Et18       Huawei_124_NetEngine_A816            GigabitEthernet0/2/5        120
Et20       Huawei_128_NetEngine_8000_M14        GigabitEthernet0/5/5        120
Et21       Juniper-156-PTX10002-36QDD           592                         120
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
Interface      IP Address          Status        Protocol         MTU   Owner  
-------------- ------------------- ------------- ------------- -------- -------
Ethernet1      20.30.31.30/24      down          down            1500          
Ethernet2      20.30.32.30/24      up            up              1500          
Ethernet3      20.30.120.30/24     up            up              1500          
Ethernet4      20.30.217.30/24     up            up              1500          
Ethernet5      20.30.214.30/24     up            up              1500          
Ethernet6      21.30.214.30/24     up            up              1500          
Ethernet7      20.30.184.30/24     up            up              1500          
Ethernet8      21.30.217.30/24     up            up              1500          
Ethernet9      20.30.72.30/24      up            up              1500          
Ethernet10     21.30.120.30/24     up            up              1500          
Ethernet11     20.30.156.30/24     up            up              1500          
Ethernet12     20.30.84.30/24      up            up              1500          
Ethernet13     20.30.53.30/24      up            up              1500          
Ethernet15     20.30.221.30/24     up            up              1500          
Ethernet16     21.30.84.30/24      admin down    down            1500          
Ethernet17     20.30.124.30/24     up            up              1500          
Ethernet18     21.30.124.30/24     up            up              1500          
Ethernet19     20.30.128.30/24     down          notpresent      1500          
Ethernet20     21.30.128.30/24     up            up              1500          
Ethernet21     21.30.156.30/24     up            up              1500          
Ethernet29     21.30.32.30/24      down          down            1500          
Ethernet31     20.30.66.30/24      up            up              1500          
Ethernet35     20.30.131.30/24     up            up              1500          
Ethernet40     20.30.179.30/24     up            up              1500          
Loopback0      10.0.0.30/32        up            up             65535          
Loopback5001   10.0.0.30/32        up            up             65535          
Loopback5128   10.128.0.30/32      up            up             65535          
Management1    192.168.20.30/23    up            up              1500          

```

## show interfaces counters rates | nz

```text
Port      Name                 Intvl  In Mbps      %  In Kpps Out Mbps      %
Et2       Arista-PE32-Q2C-32 E  0:01      8.0   0.1%       10      0.0   0.0%
Et9       Ciena-5134-72 port 2  0:01      0.0   0.0%        0      0.0   0.0%
Et11      Juniper-156 port 590  0:01      0.0   0.0%        0      0.0   0.0%
Et15      Ribbon-221            0:01      0.0   0.0%        0      7.7   0.1%
Et21      Juniper-156 port 592  0:01      0.0   0.0%        0      0.0   0.0%
Et31      Ciena-8140-66 port 2  0:01      0.0   0.0%        0      0.0   0.0%
Et35      Juniper-131-JCNR 42   0:01      0.0   0.0%        0      0.0   0.0%

Port      Out Kpps
Et15            10
```

## show isis neighbors

```text
 
Instance  VRF      System Id        Type Interface          SNPA              State Hold time   Circuit Id          
IGP       default  Arista-PE32-Q2C-32 L2   Ethernet2          P2P               UP    25          44                  
IGP       default  Arrcus-53        L2   Ethernet13         P2P               UP    27          00                  
IGP       default  Ciena-8140-66    L2   Ethernet31         P2P               UP    28          02                  
IGP       default  Ciena-5134-72    L2   Ethernet9          P2P               UP    28          02                  
IGP       default  Ericsson_84_R6678 L2   Ethernet12         P2P               UP    26          02                  
IGP       default  H3C_M1A_120      L2   Ethernet10         P2P               UP    26          01                  
IGP       default  H3C_M1A_120      L2   Ethernet3          P2P               UP    21          01                  
IGP       default  0000.0000.0124   L2   Ethernet18         P2P               UP    26          0A                  
IGP       default  0000.0000.0124   L2   Ethernet17         P2P               UP    24          09                  
IGP       default  0000.0000.0128   L2   Ethernet20         P2P               UP    27          0E                  
IGP       default  Juniper-131-JCNR L2   Ethernet35         P2P               UP    20          01                  
IGP       default  Juniper-156-PTX10002-36QDD L2   Ethernet11         P2P               UP    25          01                  
IGP       default  Juniper-156-PTX10002-36QDD L2   Ethernet21         P2P               UP    25          01                  
IGP       default  Juniper-179-ACX7024 L2   Ethernet40         P2P               UP    24          01                  
IGP       default  Nokia-SXR-214    L2   Ethernet5          P2P               UP    22          00                  
IGP       default  Nokia-SXR-214    L2   Ethernet6          P2P               UP    20          00                  
IGP       default  Nokia-SR1-217    L2   Ethernet4          P2P               UP    25          00                  
IGP       default  221              L2   Ethernet15         P2P               UP    82          00                  
```

## show isis database detail

```text
Legend:
H - hostname conflict
U - node unreachable

IS-IS Instance: IGP VRF: default
  IS-IS Level 2 Link State Database
    LSPID                   Seq Num  Cksum  Life Length IS  Received LSPID        Flags
    Arista-Spine3-Q2A-30.00-00      1190   8498  1183   1168 L2  0000.0000.0030.00-00  <>
      LSP generation remaining wait time: 0 ms
      Time remaining until refresh: 883 s
      NLPID: 0xCC(IPv4) 0x8E(IPv6)
      Hostname: Arista-Spine3-Q2A-30
      Area addresses: 49.0001
      Topology: 2 (IPv6)
      Topology: 0 (IPv4)
      Interface address: 20.30.32.30
      Interface address: 20.30.217.30
      Interface address: 20.30.53.30
      Interface address: 20.30.124.30
      Interface address: 21.30.124.30
      Interface address: 20.30.221.30
      Interface address: 20.30.120.30
      Interface address: 21.30.120.30
      Interface address: 20.30.84.30
      Interface address: 21.30.128.30
      Interface address: 20.30.66.30
      Interface address: 20.30.72.30
      Interface address: 21.30.156.30
      Interface address: 20.30.156.30
      Interface address: 20.30.179.30
      Interface address: 21.30.217.30
      Interface address: 21.30.214.30
      Interface address: 20.30.214.30
      Interface address: 20.30.184.30
      Interface address: 20.30.131.30
      Interface address: 10.0.0.30
      Interface address: 2001:0:30:32::30
      Interface address: 2001:0:30:217::30
      Interface address: 2001:0:30:53::30
      Interface address: 2001:0:30:221::30
      Interface address: 2001:0:30:120::30
      Interface address: 2001:0:30:84::30
      Interface address: 2001:0:30:66::30
      Interface address: 2001:0:30:72::30
      Interface address: 2001:0:30:156::30
      Interface address: 2001:0:30:179::30
      Interface address: 2001:0:30:214::30
      Interface address: 2001:0:30:184::30
      Interface address: 2001:0:30:131::30
      Interface address: 2002::30
      IS Neighbor          : Arista-PE32-Q2C-32.00 Metric: 1
        IPv4 Neighbor Address: 20.30.32.32
        IPv4 Interface Address: 20.30.32.30
        Adj-sid: 378588 flags: [L V] weight: 0x0
      IS Neighbor          : Nokia-SR1-217.00    Metric: 1
        IPv4 Neighbor Address: 20.30.217.217
        IPv4 Interface Address: 20.30.217.30
        Adj-sid: 378582 flags: [L V] weight: 0x0
      IS Neighbor          : Arrcus-53.00        Metric: 1
        IPv4 Neighbor Address: 20.30.53.53
        IPv4 Interface Address: 20.30.53.30
        Adj-sid: 378528 flags: [L V] weight: 0x0
      IS Neighbor          : 221.00              Metric: 1
        IPv4 Neighbor Address: 20.30.221.221
        IPv4 Interface Address: 20.30.221.30
        Adj-sid: 378542 flags: [L V] weight: 0x0
      IS Neighbor          : H3C_M1A_120.00      Metric: 1
        IPv4 Neighbor Address: 21.30.120.120
        IPv4 Interface Address: 21.30.120.30
        Adj-sid: 378590 flags: [L V] weight: 0x0
      IS Neighbor          : Nokia-SXR-214.00    Metric: 1
        IPv4 Neighbor Address: 21.30.214.214
        IPv4 Interface Address: 21.30.214.30
        Adj-sid: 378562 flags: [L V] weight: 0x0
      Reachability         : 20.30.32.0/24 Metric: 1 Type: 1 Up
      Reachability         : 20.30.217.0/24 Metric: 1 Type: 1 Up
      Reachability         : 20.30.53.0/24 Metric: 1 Type: 1 Up
      Reachability         : 21.30.124.0/24 Metric: 1 Type: 1 Up
      Reachability         : 20.30.221.0/24 Metric: 1 Type: 1 Up
      Reachability         : 20.30.120.0/24 Metric: 1 Type: 1 Up
      Reachability         : 21.30.120.0/24 Metric: 1 Type: 1 Up
      Reachability         : 20.30.84.0/24 Metric: 1 Type: 1 Up
      Reachability         : 21.30.128.0/24 Metric: 1 Type: 1 Up
      Reachability         : 20.30.66.0/24 Metric: 1 Type: 1 Up
      Reachability         : 20.30.72.0/24 Metric: 1 Type: 1 Up
      Reachability         : 21.30.156.0/24 Metric: 1 Type: 1 Up
      Reachability         : 20.30.156.0/24 Metric: 1 Type: 1 Up
      Reachability         : 20.30.179.0/24 Metric: 1 Type: 1 Up
      Reachability         : 21.30.217.0/24 Metric: 1 Type: 1 Up
      Reachability         : 21.30.214.0/24 Metric: 1 Type: 1 Up
      Reachability         : 20.30.214.0/24 Metric: 1 Type: 1 Up
      Reachability         : 20.30.184.0/24 Metric: 1 Type: 1 Up
      Reachability         : 20.30.131.0/24 Metric: 1 Type: 1 Up
      Reachability (MT-IPv6): 2001:0:30:32::/64 Metric: 10 Type: 1 Up
      Reachability (MT-IPv6): 2001:0:30:217::/64 Metric: 10 Type: 1 Up
      Reachability (MT-IPv6): 2001:0:30:53::/64 Metric: 10 Type: 1 Up
      Reachability (MT-IPv6): 2001:0:30:221::/64 Metric: 10 Type: 1 Up
      Reachability (MT-IPv6): 2001:0:30:120::/64 Metric: 10 Type: 1 Up
      Reachability (MT-IPv6): 2001:0:30:84::/64 Metric: 10 Type: 1 Up
      Reachability (MT-IPv6): 2001:0:30:66::/64 Metric: 10 Type: 1 Up
      Reachability (MT-IPv6): 2001:0:30:72::/64 Metric: 10 Type: 1 Up
      Reachability (MT-IPv6): 2001:0:30:156::/64 Metric: 10 Type: 1 Up
      Reachability (MT-IPv6): 2001:0:30:179::/64 Metric: 10 Type: 1 Up
      Reachability (MT-IPv6): 2001:0:30:214::/64 Metric: 10 Type: 1 Up
      Reachability (MT-IPv6): 2001:0:30:184::/64 Metric: 10 Type: 1 Up
      Reachability (MT-IPv6): 2001:0:30:131::/64 Metric: 10 Type: 1 Up
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
    Arista-Spine3-Q2A-30.00-01       590   3933  1183   1253 L2  0000.0000.0030.00-01  <>
      LSP generation remaining wait time: 0 ms
      Time remaining until refresh: 883 s
      Interface address: 2001:0:30:124::30
      IS Neighbor          : 0000.0000.0124.00   Metric: 1
        IPv4 Neighbor Address: 20.30.124.124
        IPv4 Interface Address: 20.30.124.30
      IS Neighbor          : Ericsson_84_R6678.00 Metric: 1
        IPv4 Neighbor Address: 20.30.84.84
        IPv4 Interface Address: 20.30.84.30
        Adj-sid: 378586 flags: [L V] weight: 0x0
      IS Neighbor          : Ciena-8140-66.00    Metric: 1
        IPv4 Neighbor Address: 20.30.66.66
        IPv4 Interface Address: 20.30.66.30
        Adj-sid: 378578 flags: [L V] weight: 0x0
      IS Neighbor          : Ciena-5134-72.00    Metric: 1
        IPv4 Neighbor Address: 20.30.72.72
        IPv4 Interface Address: 20.30.72.30
        Adj-sid: 378577 flags: [L V] weight: 0x0
      IS Neighbor          : 0000.0000.0124.00   Metric: 1
        IPv4 Neighbor Address: 21.30.124.124
        IPv4 Interface Address: 21.30.124.30
      IS Neighbor          : 0000.0000.0128.00   Metric: 1
        IPv4 Neighbor Address: 21.30.128.128
        IPv4 Interface Address: 21.30.128.30
      IS Neighbor          : Nokia-SXR-214.00    Metric: 1
        IPv4 Neighbor Address: 20.30.214.214
        IPv4 Interface Address: 20.30.214.30
        Adj-sid: 378553 flags: [L V] weight: 0x0
      IS Neighbor          : Juniper-156-PTX10002-36QDD.00 Metric: 1
        IPv4 Neighbor Address: 20.30.156.156
        IPv4 Interface Address: 20.30.156.30
        Adj-sid: 378540 flags: [L V] weight: 0x0
      IS Neighbor          : Juniper-156-PTX10002-36QDD.00 Metric: 1
        IPv4 Neighbor Address: 21.30.156.156
        IPv4 Interface Address: 21.30.156.30
        Adj-sid: 378574 flags: [L V] weight: 0x0
      IS Neighbor          : Juniper-179-ACX7024.00 Metric: 1
        IPv4 Neighbor Address: 20.30.179.179
        IPv4 Interface Address: 20.30.179.30
        Adj-sid: 378538 flags: [L V] weight: 0x0
      IS Neighbor          : H3C_M1A_120.00      Metric: 1
        IPv4 Neighbor Address: 20.30.120.120
        IPv4 Interface Address: 20.30.120.30
        Adj-sid: 378597 flags: [L V] weight: 0x0
      IS Neighbor          : Juniper-131-JCNR.00 Metric: 1
        IPv4 Neighbor Address: 20.30.131.131
        IPv4 Interface Address: 20.30.131.30
        Adj-sid: 378533 flags: [L V] weight: 0x0
      IS Neighbor (MT-IPv6): Arista-PE32-Q2C-32.00 Metric: 10
        IPv6 Neighbor Address: 2001:0:30:32::32
        Global IPv6 Interface Address: 2001:0:30:32::30
        Adj-sid: 378589 flags: [L V F] weight: 0x0
      IS Neighbor (MT-IPv6): Juniper-156-PTX10002-36QDD.00 Metric: 10
        IPv6 Neighbor Address: 2001:0:30:156::156
        Global IPv6 Interface Address: 2001:0:30:156::30
        Adj-sid: 378541 flags: [L V F] weight: 0x0
      IS Neighbor (MT-IPv6): Nokia-SR1-217.00    Metric: 10
        IPv6 Neighbor Address: 2001:0:30:217::217
        Global IPv6 Interface Address: 2001:0:30:217::30
        Adj-sid: 378583 flags: [L V F] weight: 0x0
      IS Neighbor (MT-IPv6): Arrcus-53.00        Metric: 10
        IPv6 Neighbor Address: 2001:0:30:53::53
        Global IPv6 Interface Address: 2001:0:30:53::30
        Adj-sid: 378529 flags: [L V F] weight: 0x0
      Reachability         : 20.30.124.0/24 Metric: 1 Type: 1 Up
      Reachability         : 10.0.0.30/32 Metric: 0 Type: 1 Up
        SR Prefix-SID: 30 Flags: [N] Algorithm: 0
        SR Prefix-SID: 158 Flags: [N] Algorithm: 128
        SR Prefix-SID: 159 Flags: [N] Algorithm: 129
        SR Prefix-SID: 160 Flags: [N] Algorithm: 130
      Reachability (MT-IPv6): 2001:0:30:124::/64 Metric: 10 Type: 1 Up
      Reachability (MT-IPv6): 2002::30/128 Metric: 10 Type: 1 Up
        SR Prefix-SID: 430 Flags: [N] Algorithm: 0
        SR Prefix-SID: 558 Flags: [N] Algorithm: 128
        SR Prefix-SID: 559 Flags: [N] Algorithm: 129
        SR Prefix-SID: 560 Flags: [N] Algorithm: 130
    Arista-Spine3-Q2A-30.00-02        20  20897  1051    203 L2  0000.0000.0030.00-02  <>
      LSP generation remaining wait time: 0 ms
      Time remaining until refresh: 751 s
      IS Neighbor (MT-IPv6): H3C_M1A_120.00      Metric: 10
        IPv6 Neighbor Address: 2001:0:30:120::120
        Global IPv6 Interface Address: 2001:0:30:120::30
        Adj-sid: 378598 flags: [L V F] weight: 0x0
      IS Neighbor (MT-IPv6): Ericsson_84_R6678.00 Metric: 10
        IPv6 Neighbor Address: 2001:0:30:84::175
        Global IPv6 Interface Address: 2001:0:30:84::30
        Adj-sid: 378587 flags: [L V F] weight: 0x0
    Arista-PE32-Q2C-32.00-00       489  51571  1183    592 L2  0000.0000.0032.00-00  <>
      Remaining lifetime received: 1199 s Modified to: 1200 s
      NLPID: 0xCC(IPv4) 0x8E(IPv6)
      Hostname: Arista-PE32-Q2C-32
      Area addresses: 49.0001
      Topology: 2 (IPv6)
      Topology: 0 (IPv4)
      Interface address: 20.30.32.32
      Interface address: 20.32.175.32
      Interface address: 10.0.0.32
      Interface address: 2001:0:30:32::32
      Interface address: 2001:0:32:175::32
      Interface address: 2002::32
      IS Neighbor          : Arista-Spine3-Q2A-30.00 Metric: 10
        IPv4 Neighbor Address: 20.30.32.30
        IPv4 Interface Address: 20.30.32.32
        Adj-sid: 362168 flags: [L V] weight: 0x0
      IS Neighbor          : Juniper-175-ACX7100-48L.00 Metric: 10
        IPv4 Neighbor Address: 20.32.175.175
        IPv4 Interface Address: 20.32.175.32
        Adj-sid: 362170 flags: [L V] weight: 0x0
      IS Neighbor (MT-IPv6): Arista-Spine3-Q2A-30.00 Metric: 10
        IPv6 Neighbor Address: 2001:0:30:32::30
        Global IPv6 Interface Address: 2001:0:30:32::32
        Adj-sid: 362169 flags: [L V F] weight: 0x0
      IS Neighbor (MT-IPv6): Juniper-175-ACX7100-48L.00 Metric: 10
        IPv6 Neighbor Address: 2001:0:32:175::175
        Global IPv6 Interface Address: 2001:0:32:175::32
        Adj-sid: 362171 flags: [L V F] weight: 0x0
      Reachability         : 20.30.32.0/24 Metric: 10 Type: 1 Up
      Reachability         : 20.32.175.0/24 Metric: 10 Type: 1 Up
      Reachability         : 10.0.0.32/32 Metric: 0 Type: 1 Up
        SR Prefix-SID: 32 Flags: [N] Algorithm: 0
        SR Prefix-SID: 161 Flags: [N] Algorithm: 128
        SR Prefix-SID: 162 Flags: [N] Algorithm: 129
        SR Prefix-SID: 163 Flags: [N] Algorithm: 130
      Reachability (MT-IPv6): 2001:0:30:32::/64 Metric: 10 Type: 1 Up
      Reachability (MT-IPv6): 2001:0:32:175::/64 Metric: 10 Type: 1 Up
      Reachability (MT-IPv6): 2002::32/128 Metric: 10 Type: 1 Up
      Router Capabilities: Router Id: 10.0.0.32 Flags: []
        SR Local Block:
          SRLB Base: 965536 Range: 65536
        Area leader priority: 250 algorithm: 0
        Maximum SID depth:
          Base MPLS imposition (MSD type 1):  12
        SR Capability: Flags: [I V]
          SRGB Base: 20000 Range: 2000
        Algorithms:  0, 128, 129, 130
    Arrcus-53.00-00             779  43847  1105    620 L2  0000.0000.0053.00-00  <>
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
    Ciena-8140-66.00-00          48  23617   584    337 L2  0000.0000.0066.00-00  <>
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
        SR Prefix-SID: 1195 Flags: [N] Algorithm: 129
      Reachability         : 20.30.66.0/24 Metric: 10 Type: 1 Up
      Reachability         : 20.66.175.0/24 Metric: 10 Type: 1 Up
      Router Capabilities: Router Id: 10.0.0.66 Flags: []
        SR Capability: Flags: [I]
          SRGB Base: 20000 Range: 2000
        Algorithms:  0, 129
    Ciena-5134-72.00-00          51  54637   584    337 L2  0000.0000.0072.00-00  <>
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
        SR Prefix-SID: 1201 Flags: [N] Algorithm: 129
      Reachability         : 20.72.175.0/24 Metric: 10 Type: 1 Up
      Reachability         : 20.30.72.0/24 Metric: 10 Type: 1 Up
      Router Capabilities: Router Id: 10.0.0.72 Flags: []
        SR Capability: Flags: [I]
          SRGB Base: 20000 Range: 2000
        Algorithms:  0, 129
    Ericsson_84_R6678.00-00       552  22494   988    324 L2  0000.0000.0084.00-00  <>
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
    H3C_M1A_120.00-00          3712  19594  1184   1422 L2  0000.0000.0120.00-00  <>
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
      Interface address: 21.30.120.120
      Interface address: 2001:0:30:120::120
      Interface address: 2001:0:120:175::120
      Interface address: 2001:0:120:214::120
      Interface address: 2001:1:30:120::120
      Interface address: 2002::120
      IS Neighbor          : Arista-Spine3-Q2A-30.00 Metric: 10
        IPv4 Neighbor Address: 20.30.120.30
        IPv4 Interface Address: 20.30.120.120
        Adj-sid: 1916 flags: [L V] weight: 0x0
      IS Neighbor          : Arista-Spine3-Q2A-30.00 Metric: 10
        IPv4 Neighbor Address: 20.30.120.30
        IPv4 Interface Address: 20.30.120.120
      IS Neighbor          : Arista-Spine3-Q2A-30.00 Metric: 15
        IPv4 Neighbor Address: 21.30.120.30
        IPv4 Interface Address: 21.30.120.120
        Adj-sid: 1912 flags: [L V] weight: 0x0
      IS Neighbor          : Arista-Spine3-Q2A-30.00 Metric: 15
        IPv4 Neighbor Address: 21.30.120.30
        IPv4 Interface Address: 21.30.120.120
      IS Neighbor          : Juniper-175-ACX7100-48L.00 Metric: 10
        IPv4 Neighbor Address: 20.120.175.175
        IPv4 Interface Address: 20.120.175.120
        Adj-sid: 1915 flags: [L V] weight: 0x0
      IS Neighbor (MT-IPv6): Arista-Spine3-Q2A-30.00 Metric: 10
        IPv6 Neighbor Address: 2001:0:30:120::30
        Global IPv6 Interface Address: 2001:0:30:120::120
        Adj-sid: 1914 flags: [L V F] weight: 0x0
      Reachability         : 10.0.0.120/32 Metric: 0 Type: 1 Up
        SR Prefix-SID: 120 Flags: [N] Algorithm: 0
        SR Prefix-SID: 1248 Flags: [N] Algorithm: 128
        SR Prefix-SID: 1249 Flags: [N] Algorithm: 129
        SR Prefix-SID: 1250 Flags: [N] Algorithm: 130
      Reachability         : 20.30.120.0/24 Metric: 10 Type: 1 Up
      Reachability         : 20.120.175.0/24 Metric: 10 Type: 1 Up
      Reachability         : 20.120.214.0/24 Metric: 10 Type: 1 Up
      Reachability         : 20.120.217.0/24 Metric: 0 Type: 1 Up
      Reachability         : 21.30.120.0/24 Metric: 15 Type: 1 Up
      Reachability         : 192.168.20.0/23 Metric: 0 Type: 1 Up
      Reachability (MT-IPv6): 2001:0:30:120::/64 Metric: 10 Type: 1 Up
      Reachability (MT-IPv6): 2001:0:120:175::/64 Metric: 10 Type: 1 Up
      Reachability (MT-IPv6): 2001:0:120:214::/64 Metric: 10 Type: 1 Up
      Reachability (MT-IPv6): 2001:0:120:217::/64 Metric: 0 Type: 1 Up
      Reachability (MT-IPv6): 2001:1:30:120::/64 Metric: 15 Type: 1 Up
      Reachability (MT-IPv6): 2002::120/128 Metric: 0 Type: 1 Up
        SR Prefix-SID: 520 Flags: [N] Algorithm: 0
        SR Prefix-SID: 1648 Flags: [N] Algorithm: 128
        SR Prefix-SID: 1649 Flags: [N] Algorithm: 129
        SR Prefix-SID: 1650 Flags: [N] Algorithm: 130
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
    H3C_M1A_120.00-01            34  48806   561    677 L2  0000.0000.0120.00-01  <>
      Remaining lifetime received: 1199 s Modified to: 1200 s
      IS Neighbor          : Juniper-175-ACX7100-48L.00 Metric: 10
        IPv4 Neighbor Address: 20.120.175.175
        IPv4 Interface Address: 20.120.175.120
      IS Neighbor (MT-IPv6): Arista-Spine3-Q2A-30.00 Metric: 10
        IPv6 Neighbor Address: 2001:0:30:120::30
        Global IPv6 Interface Address: 2001:0:30:120::120
      IS Neighbor (MT-IPv6): Juniper-175-ACX7100-48L.00 Metric: 10
        IPv6 Neighbor Address: 2001:0:120:175::175
        Global IPv6 Interface Address: 2001:0:120:175::120
        Adj-sid: 1913 flags: [L V F] weight: 0x0
      IS Neighbor (MT-IPv6): Juniper-175-ACX7100-48L.00 Metric: 10
        IPv6 Neighbor Address: 2001:0:120:175::175
        Global IPv6 Interface Address: 2001:0:120:175::120
    0000.0000.0124.00-00       1606  61639   461    401 L2  0000.0000.0124.00-00  <>
      Remaining lifetime received: 1199 s Modified to: 1200 s
      NLPID: 0xCC(IPv4) 0x8E(IPv6)
      Area addresses: 49.0001
      Topology: 0 (IPv4)
      Topology: 2 (IPv6)
      Interface address: 20.124.175.124
      Interface address: 10.0.0.124
      Interface address: 20.30.124.124
      Interface address: 21.30.124.124
      IS Neighbor          : Arista-Spine3-Q2A-30.00 Metric: 10
        IPv4 Neighbor Address: 20.30.124.30
        IPv4 Interface Address: 20.30.124.124
        Adj-sid: 402 flags: [L V] weight: 0x0
      IS Neighbor          : Arista-Spine3-Q2A-30.00 Metric: 15
        IPv4 Neighbor Address: 21.30.124.30
        IPv4 Interface Address: 21.30.124.124
        Adj-sid: 403 flags: [L V] weight: 0x0
      IS Neighbor          : Juniper-175-ACX7100-48L.00 Metric: 10
        IPv4 Neighbor Address: 20.124.175.175
        IPv4 Interface Address: 20.124.175.124
        Adj-sid: 404 flags: [L V] weight: 0x0
      Reachability         : 10.0.0.124/32 Metric: 0 Type: 1 Up
        SR Prefix-SID: 124 Flags: [N P] Algorithm: 0
        SR Prefix-SID: 1252 Flags: [N P] Algorithm: 128
      Reachability         : 20.124.175.0/24 Metric: 10 Type: 1 Up
      Reachability         : 20.30.124.0/24 Metric: 10 Type: 1 Up
      Reachability         : 21.30.124.0/24 Metric: 15 Type: 1 Up
      Router Capabilities: Router Id: 10.0.0.124 Flags: []
        Flex Algo: Algorithm: 128 Metric: Min Unidirectional Delay Metric (1) Calc: SPF (0) Prio: 128
          Flags: [M] 0x80
      Router Capabilities: Router Id: 10.0.0.124 Flags: []
        Maximum SID depth:
          Base MPLS imposition (MSD type 1):  10
        SR Capability: Flags: [I]
          SRGB Base: 2000 Range: 2001
        Algorithms:  0, 128
    0000.0000.0128.00-00       1660  27216   461    290 L2  0000.0000.0128.00-00  <>
      Remaining lifetime received: 1199 s Modified to: 1200 s
      NLPID: 0xCC(IPv4) 0x8E(IPv6)
      Area addresses: 49.0001
      Topology: 0 (IPv4)
      Topology: 2 (IPv6)
      Interface address: 10.0.0.128
      Interface address: 20.128.175.128
      Interface address: 21.30.128.128
      IS Neighbor          : Juniper-175-ACX7100-48L.00 Metric: 10
        IPv4 Neighbor Address: 20.128.175.175
        IPv4 Interface Address: 20.128.175.128
        Adj-sid: 48134 flags: [L V] weight: 0x0
      IS Neighbor          : Arista-Spine3-Q2A-30.00 Metric: 15
        IPv4 Neighbor Address: 21.30.128.30
        IPv4 Interface Address: 21.30.128.128
        Adj-sid: 48136 flags: [L V] weight: 0x0
      Reachability         : 10.0.0.128/32 Metric: 0 Type: 1 Up
        SR Prefix-SID: 128 Flags: [N] Algorithm: 0
        SR Prefix-SID: 1256 Flags: [N] Algorithm: 128
      Reachability         : 20.128.175.0/24 Metric: 10 Type: 1 Up
      Reachability         : 21.30.128.0/24 Metric: 15 Type: 1 Up
      Router Capabilities: Router Id: 10.0.0.128 Flags: []
        Flex Algo: Algorithm: 128 Metric: Min Unidirectional Delay Metric (1) Calc: SPF (0) Prio: 128
          Flags: [M] 0x80
      Router Capabilities: Router Id: 10.0.0.128 Flags: []
        Maximum SID depth:
          Base MPLS imposition (MSD type 1):  10
        SR Capability: Flags: [I]
          SRGB Base: 20000 Range: 2000
        Algorithms:  0, 128
    Juniper-131-JCNR.00-00       254  27339   761    447 L2  0000.0000.0131.00-00  <>
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
    Juniper-156-PTX10002-36QDD.00-00       317   9292   848   1014 L2  0000.0000.0156.00-00  <>
      Remaining lifetime received: 1198 s Modified to: 1200 s
      NLPID: 0xCC(IPv4) 0x8E(IPv6)
      Hostname: Juniper-156-PTX10002-36QDD
      Area addresses: 49.0001
      Topology: 0 (IPv4)
      Topology: 2 (IPv6)
      Interface address: 10.0.0.156
      Interface address: 2002::156
      IS Neighbor          : Arista-Spine3-Q2A-30.00 Metric: 10
        IPv4 Neighbor Address: 20.30.156.30
        IPv4 Interface Address: 20.30.156.156
        IPv6 Neighbor Address: 2001:0:30:156::30
        Global IPv6 Interface Address: 2001:0:30:156::156
        Adj-sid: 22 flags: [L V B] weight: 0x0
      IS Neighbor          : Juniper-175-ACX7100-48L.00 Metric: 10
        IPv4 Neighbor Address: 20.156.175.175
        IPv4 Interface Address: 20.156.175.156
        IPv6 Neighbor Address: 2001:0:156:175::175
        Global IPv6 Interface Address: 2001:0:156:175::156
        Adj-sid: 18 flags: [L V B] weight: 0x0
      IS Neighbor          : Arista-Spine3-Q2A-30.00 Metric: 15
        IPv4 Neighbor Address: 21.30.156.30
        IPv4 Interface Address: 21.30.156.156
        Adj-sid: 24 flags: [L V B] weight: 0x0
      IS Neighbor (MT-IPv6): Arista-Spine3-Q2A-30.00 Metric: 10
        IPv4 Interface Address: 20.30.156.156
        IPv6 Neighbor Address: 2001:0:30:156::30
        Global IPv6 Interface Address: 2001:0:30:156::156
        Adj-sid: 23 flags: [L V B F] weight: 0x0
      IS Neighbor (MT-IPv6): Juniper-175-ACX7100-48L.00 Metric: 10
        IPv4 Interface Address: 20.156.175.156
        IPv6 Neighbor Address: 2001:0:156:175::175
        Global IPv6 Interface Address: 2001:0:156:175::156
        Adj-sid: 19 flags: [L V B F] weight: 0x0
      Reachability         : 10.0.0.156/32 Metric: 0 Type: 1 Up
        SR Prefix-SID: 156 Flags: [N] Algorithm: 0
        SR Prefix-SID: 1286 Flags: [N] Algorithm: 130
        SR Prefix-SID: 1285 Flags: [N] Algorithm: 129
        SR Prefix-SID: 1284 Flags: [N] Algorithm: 128
      Reachability         : 20.30.156.0/24 Metric: 10 Type: 1 Up
      Reachability         : 21.30.156.0/24 Metric: 15 Type: 1 Up
      Reachability         : 20.156.175.0/24 Metric: 10 Type: 1 Up
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
    Juniper-175-ACX7100-48L.00-00       673  12331  1154   1297 L2  0000.0000.0175.00-00  <>
      Remaining lifetime received: 1198 s Modified to: 1200 s
      NLPID: 0xCC(IPv4) 0x8E(IPv6)
      Hostname: Juniper-175-ACX7100-48L
      Area addresses: 49.0001
      Topology: 0 (IPv4)
      Topology: 2 (IPv6)
      Interface address: 10.0.0.175
      Interface address: 127.0.0.1
      Interface address: 2002::175
      IS Neighbor          : Juniper-131-JCNR.00 Metric: 10
        IPv4 Neighbor Address: 20.131.175.131
        IPv4 Interface Address: 20.131.175.175
        IPv6 Neighbor Address: 2001:0:131:175::131
        Global IPv6 Interface Address: 2001:0:131:175::175
        Adj-sid: 116 flags: [L V F] weight: 0x0
        Adj-sid: 115 flags: [L V] weight: 0x0
      IS Neighbor          : Juniper-179-ACX7024.00 Metric: 10
        IPv4 Neighbor Address: 20.175.179.179
        IPv4 Interface Address: 20.175.179.175
        IPv6 Neighbor Address: 2001:0:175::179:179
        Global IPv6 Interface Address: 2001:0:175::179:175
        Adj-sid: 106 flags: [L V F] weight: 0x0
        Adj-sid: 105 flags: [L V] weight: 0x0
      IS Neighbor          : 221.00              Metric: 10
        IPv4 Neighbor Address: 20.175.221.221
        IPv4 Interface Address: 20.175.221.175
        Global IPv6 Interface Address: 2001:0:175:221::175
        Adj-sid: 168 flags: [L V] weight: 0x0
      IS Neighbor (MT-IPv6): Nokia-SR1-217.00    Metric: 10
        IPv4 Interface Address: 20.175.217.175
        IPv6 Neighbor Address: 2001:0:175:217::217
        Global IPv6 Interface Address: 2001:0:175:217::175
        Adj-sid: 98 flags: [L V F] weight: 0x0
      IS Neighbor (MT-IPv6): H3C_M1A_120.00      Metric: 10
        IPv4 Interface Address: 20.120.175.175
        IPv6 Neighbor Address: 2001:0:120:175::120
        Global IPv6 Interface Address: 2001:0:120:175::175
        Adj-sid: 166 flags: [L V F] weight: 0x0
      Reachability         : 127.0.0.1/32 Metric: 0 Type: 1 Up
      Reachability         : 10.0.0.175/32 Metric: 0 Type: 1 Up
        SR Prefix-SID: 175 Flags: [N] Algorithm: 0
        SR Prefix-SID: 1305 Flags: [N] Algorithm: 130
        SR Prefix-SID: 1304 Flags: [N] Algorithm: 129
        SR Prefix-SID: 1303 Flags: [N] Algorithm: 128
      Reachability         : 20.156.175.0/24 Metric: 10 Type: 1 Up
      Reachability         : 20.175.184.0/24 Metric: 10 Type: 1 Up
      Reachability         : 20.53.175.0/24 Metric: 10 Type: 1 Up
      Reachability         : 20.66.175.0/24 Metric: 10 Type: 1 Up
      Reachability         : 20.72.175.0/24 Metric: 10 Type: 1 Up
      Reachability         : 20.175.179.0/24 Metric: 10 Type: 1 Up
      Reachability         : 20.175.214.0/24 Metric: 10 Type: 1 Up
      Reachability         : 20.84.175.0/24 Metric: 10 Type: 1 Up
      Reachability         : 20.175.217.0/24 Metric: 10 Type: 1 Up
      Reachability         : 20.131.175.0/24 Metric: 10 Type: 1 Up
      Reachability         : 20.32.175.0/24 Metric: 10 Type: 1 Up
      Reachability         : 20.128.175.0/24 Metric: 10 Type: 1 Up
      Reachability         : 20.120.175.0/24 Metric: 10 Type: 1 Up
      Reachability         : 20.175.221.0/24 Metric: 10 Type: 1 Up
      Reachability         : 20.124.175.0/24 Metric: 10 Type: 1 Up
      Reachability (MT-IPv6): 2002::175/128 Metric: 0 Type: 1 Up
        SR Prefix-SID: 575 Flags: [N] Algorithm: 0
        SR Prefix-SID: 1705 Flags: [N] Algorithm: 130
        SR Prefix-SID: 1704 Flags: [N] Algorithm: 129
        SR Prefix-SID: 1703 Flags: [N] Algorithm: 128
      Reachability (MT-IPv6): 2001:0:156:175::/64 Metric: 10 Type: 1 Up
      Reachability (MT-IPv6): 2001:0:175:184::/64 Metric: 10 Type: 1 Up
      Reachability (MT-IPv6): 2001:0:175::/64 Metric: 10 Type: 1 Up
      Reachability (MT-IPv6): 2001:0:175:214::/64 Metric: 10 Type: 1 Up
      Reachability (MT-IPv6): 2001:0:84:175::/64 Metric: 10 Type: 1 Up
      Reachability (MT-IPv6): 2001:0:175:217::/64 Metric: 10 Type: 1 Up
      Reachability (MT-IPv6): 2001:0:53:175::/64 Metric: 10 Type: 1 Up
      Reachability (MT-IPv6): 2001:0:66:175::/64 Metric: 10 Type: 1 Up
      Reachability (MT-IPv6): 2001:0:72:175::/64 Metric: 10 Type: 1 Up
      Reachability (MT-IPv6): 2001:0:32:175::/64 Metric: 10 Type: 1 Up
      Reachability (MT-IPv6): 2001:0:128:175::/64 Metric: 10 Type: 1 Up
      Reachability (MT-IPv6): 2001:0:120:175::/64 Metric: 10 Type: 1 Up
      Reachability (MT-IPv6): 2001:0:175:221::/64 Metric: 10 Type: 1 Up
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
    Juniper-175-ACX7100-48L.00-01       549  44208   998   1357 L2  0000.0000.0175.00-01  <>
      Remaining lifetime received: 1198 s Modified to: 1200 s
      IS Neighbor          : Ericsson_84_R6678.00 Metric: 10
        IPv4 Neighbor Address: 20.84.175.84
        IPv4 Interface Address: 20.84.175.175
        IPv6 Neighbor Address: 2001:0:84:175::175
        Global IPv6 Interface Address: 2001:0:84:175::175
        Adj-sid: 132 flags: [L V F] weight: 0x0
        Adj-sid: 131 flags: [L V] weight: 0x0
      IS Neighbor          : Nokia-SXR-214.00    Metric: 10
        IPv4 Neighbor Address: 20.175.214.214
        IPv4 Interface Address: 20.175.214.175
        IPv6 Neighbor Address: 2001:0:175:214::214
        Global IPv6 Interface Address: 2001:0:175:214::175
        Adj-sid: 151 flags: [L V] weight: 0x0
      IS Neighbor          : Juniper-156-PTX10002-36QDD.00 Metric: 10
        IPv4 Neighbor Address: 20.156.175.156
        IPv4 Interface Address: 20.156.175.175
        IPv6 Neighbor Address: 2001:0:156:175::156
        Global IPv6 Interface Address: 2001:0:156:175::175
        Adj-sid: 130 flags: [L V F] weight: 0x0
        Adj-sid: 129 flags: [L V] weight: 0x0
      IS Neighbor          : Nokia-SR1-217.00    Metric: 10
        IPv4 Neighbor Address: 20.175.217.217
        IPv4 Interface Address: 20.175.217.175
        IPv6 Neighbor Address: 2001:0:175:217::217
        Global IPv6 Interface Address: 2001:0:175:217::175
        Adj-sid: 140 flags: [L V] weight: 0x0
      IS Neighbor          : Ciena-8140-66.00    Metric: 10
        IPv4 Neighbor Address: 20.66.175.66
        IPv4 Interface Address: 20.66.175.175
        Global IPv6 Interface Address: 2001:0:66:175::175
        Adj-sid: 163 flags: [L V] weight: 0x0
      IS Neighbor          : Arista-PE32-Q2C-32.00 Metric: 10
        IPv4 Neighbor Address: 20.32.175.32
        IPv4 Interface Address: 20.32.175.175
        IPv6 Neighbor Address: 2001:0:32:175::32
        Global IPv6 Interface Address: 2001:0:32:175::175
        Adj-sid: 147 flags: [L V] weight: 0x0
      IS Neighbor          : H3C_M1A_120.00      Metric: 10
        IPv4 Neighbor Address: 20.120.175.120
        IPv4 Interface Address: 20.120.175.175
        IPv6 Neighbor Address: 2001:0:120:175::120
        Global IPv6 Interface Address: 2001:0:120:175::175
        Adj-sid: 165 flags: [L V] weight: 0x0
      IS Neighbor          : 0000.0000.0128.00   Metric: 10
        IPv4 Neighbor Address: 20.128.175.128
        IPv4 Interface Address: 20.128.175.175
        Global IPv6 Interface Address: 2001:0:128:175::175
        Adj-sid: 96 flags: [L V] weight: 0x0
      IS Neighbor (MT-IPv6): Nokia-SXR-214.00    Metric: 10
        IPv4 Interface Address: 20.175.214.175
        IPv6 Neighbor Address: 2001:0:175:214::214
        Global IPv6 Interface Address: 2001:0:175:214::175
        Adj-sid: 108 flags: [L V F] weight: 0x0
      IS Neighbor (MT-IPv6): Arista-PE32-Q2C-32.00 Metric: 10
        IPv4 Interface Address: 20.32.175.175
        IPv6 Neighbor Address: 2001:0:32:175::32
        Global IPv6 Interface Address: 2001:0:32:175::175
        Adj-sid: 148 flags: [L V F] weight: 0x0
    Juniper-175-ACX7100-48L.00-02       182   4912  1154    805 L2  0000.0000.0175.00-02  <>
      Remaining lifetime received: 1198 s Modified to: 1200 s
      IS Neighbor          : Ciena-5134-72.00    Metric: 10
        IPv4 Neighbor Address: 20.72.175.72
        IPv4 Interface Address: 20.72.175.175
        Global IPv6 Interface Address: 2001:0:72:175::175
        Adj-sid: 167 flags: [L V] weight: 0x0
      IS Neighbor          : Arrcus-53.00        Metric: 10
        IPv4 Neighbor Address: 20.53.175.53
        IPv4 Interface Address: 20.53.175.175
        IPv6 Neighbor Address: 2001:0:53:175::53
        Global IPv6 Interface Address: 2001:0:53:175::175
        Adj-sid: 99 flags: [L V] weight: 0x0
      IS Neighbor          : 0000.0000.0124.00   Metric: 10
        IPv4 Neighbor Address: 20.124.175.124
        IPv4 Interface Address: 20.124.175.175
        Adj-sid: 170 flags: [L V] weight: 0x0
      IS Neighbor (MT-IPv6): Ericsson_84_R6678.00 Metric: 10
        IPv4 Interface Address: 20.84.175.175
        IPv6 Neighbor Address: 2001:0:84:175::175
        Global IPv6 Interface Address: 2001:0:84:175::175
        Adj-sid: 132 flags: [L V F] weight: 0x0
      IS Neighbor (MT-IPv6): Juniper-156-PTX10002-36QDD.00 Metric: 10
        IPv4 Interface Address: 20.156.175.175
        IPv6 Neighbor Address: 2001:0:156:175::156
        Global IPv6 Interface Address: 2001:0:156:175::175
        Adj-sid: 130 flags: [L V F] weight: 0x0
      IS Neighbor (MT-IPv6): Arrcus-53.00        Metric: 10
        IPv4 Interface Address: 20.53.175.175
        IPv6 Neighbor Address: 2001:0:53:175::53
        Global IPv6 Interface Address: 2001:0:53:175::175
        Adj-sid: 133 flags: [L V F] weight: 0x0
      Reachability (MT-IPv6): 2001:0:131:175::/64 Metric: 10 Type: 1 Up
    Juniper-179-ACX7024.00-00       426  51393  1038    543 L2  0000.0000.0179.00-00  <>
      Remaining lifetime received: 1198 s Modified to: 1200 s
      NLPID: 0xCC(IPv4) 0x8E(IPv6)
      Hostname: Juniper-179-ACX7024
      Area addresses: 49.0001
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
        Adj-sid: 24 flags: [L V F] weight: 0x0
        Adj-sid: 23 flags: [L V] weight: 0x0
      Reachability         : 10.0.0.179/32 Metric: 0 Type: 1 Up
        SR Prefix-SID: 179 Flags: [N] Algorithm: 0
        SR Prefix-SID: 1309 Flags: [N] Algorithm: 130
        SR Prefix-SID: 1308 Flags: [N] Algorithm: 129
        SR Prefix-SID: 1307 Flags: [N] Algorithm: 128
      Reachability         : 20.175.179.0/24 Metric: 10 Type: 1 Up
      Reachability         : 127.0.0.1/32 Metric: 0 Type: 1 Up
      Reachability         : 10.0.1.179/32 Metric: 0 Type: 1 Up
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
    Nokia-SXR-214.00-00       11047  11798  1191    743 L2  0000.0000.0214.00-00  <>
      NLPID: 0xCC(IPv4) 0x8E(IPv6)
      Hostname: Nokia-SXR-214
      Area addresses: 49.0001
      Topology: 0 (IPv4)
      Topology: 2 (IPv6)
      Interface address: 10.0.0.214
      Interface address: 20.30.214.214
      Interface address: 21.30.214.214
      Interface address: 20.175.214.214
      Interface address: 20.214.216.214
      Interface address: 2000::214
      Interface address: 2001:0:175:214::214
      Interface address: 2001:0:214:216::214
      IS Neighbor          : Nokia-IXRe2-216.00  Metric: 10
        IPv4 Neighbor Address: 20.214.216.216
        IPv4 Interface Address: 20.214.216.214
        Adj-sid: 30031 flags: [L V B] weight: 0x0
      IS Neighbor          : Juniper-175-ACX7100-48L.00 Metric: 100
        IPv4 Neighbor Address: 20.175.214.175
        IPv4 Interface Address: 20.175.214.214
        Adj-sid: 30033 flags: [L V B] weight: 0x0
      IS Neighbor          : Arista-Spine3-Q2A-30.00 Metric: 1
        IPv4 Neighbor Address: 20.30.214.30
        IPv4 Interface Address: 20.30.214.214
        Adj-sid: 30037 flags: [L V B] weight: 0x0
      IS Neighbor          : Arista-Spine3-Q2A-30.00 Metric: 10
        IPv4 Neighbor Address: 21.30.214.30
        IPv4 Interface Address: 21.30.214.214
        Adj-sid: 30039 flags: [L V B] weight: 0x0
      IS Neighbor (MT-IPv6): Nokia-IXRe2-216.00  Metric: 10
        IPv6 Neighbor Address: 2001:0:214:216::216
        Global IPv6 Interface Address: 2001:0:214:216::214
        Adj-sid: 30032 flags: [L V B F] weight: 0x0
      IS Neighbor (MT-IPv6): Juniper-175-ACX7100-48L.00 Metric: 10
        IPv6 Neighbor Address: 2001:0:175:214::175
        Global IPv6 Interface Address: 2001:0:175:214::214
        Adj-sid: 30034 flags: [L V B F] weight: 0x0
      Reachability         : 20.30.214.0/24 Metric: 1 Type: 1 Up
      Reachability         : 21.30.214.0/24 Metric: 10 Type: 1 Up
      Reachability         : 20.175.214.0/24 Metric: 100 Type: 1 Up
      Reachability         : 20.214.216.0/24 Metric: 10 Type: 1 Up
      Reachability         : 10.0.0.214/32 Metric: 0 Type: 1 Up
        SR Prefix-SID: 214 Flags: [N P] Algorithm: 0
      Reachability (MT-IPv6): 2000::214/128 Metric: 0 Type: 1 Up
      Reachability (MT-IPv6): 2001:0:175:214::/64 Metric: 10 Type: 1 Up
      Reachability (MT-IPv6): 2001:0:214:216::/64 Metric: 10 Type: 1 Up
      Router Capabilities: Router Id: 10.0.0.214 Flags: []
        Maximum SID depth:
          Base MPLS imposition (MSD type 1):  15
        SR Capability: Flags: [I V]
          SRGB Base: 20000 Range: 2000
        Algorithms:  0
    Nokia-IXRe2-216.00-00      1304  25446   801    486 L2  0100.0000.0216.00-00  <>
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
        Adj-sid: 1048573 flags: [L V B F] weight: 0x0
      IS Neighbor (MT-IPv6): Nokia-SXR-214.00    Metric: 10
        IPv6 Neighbor Address: 2001:0:214:216::214
        Global IPv6 Interface Address: 2001:0:214:216::216
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
    Nokia-SR1-217.00-00         724  16014  1116    594 L2  0100.0000.0217.00-00  <>
      NLPID: 0xCC(IPv4) 0x8E(IPv6)
      Hostname: Nokia-SR1-217
      Area addresses: 49.0001.0000.0000.0217.00
      Topology: 0 (IPv4)
      Topology: 2 (IPv6)
      Interface address: 10.0.0.217
      Interface address: 20.30.217.217
      Interface address: 20.175.217.217
      Interface address: 2001:0:30:217::217
      Interface address: 2001:0:175:217::217
      Interface address: 2002::217
      IS Neighbor          : Juniper-175-ACX7100-48L.00 Metric: 10
        IPv4 Neighbor Address: 20.175.217.175
        IPv4 Interface Address: 20.175.217.217
        Adj-sid: 524283 flags: [L V B] weight: 0x0
      IS Neighbor          : Arista-Spine3-Q2A-30.00 Metric: 10
        IPv4 Neighbor Address: 20.30.217.30
        IPv4 Interface Address: 20.30.217.217
        Adj-sid: 524285 flags: [L V B] weight: 0x0
      IS Neighbor (MT-IPv6): Juniper-175-ACX7100-48L.00 Metric: 10
      IS Neighbor (MT-IPv6): Arista-Spine3-Q2A-30.00 Metric: 10
      Reachability         : 10.0.0.217/32 Metric: 0 Type: 1 Up
        SR Prefix-SID: 217 Flags: [N P] Algorithm: 0
        SR Prefix-SID: 1345 Flags: [N P] Algorithm: 128
        SR Prefix-SID: 1346 Flags: [N P] Algorithm: 129
        SR Prefix-SID: 1347 Flags: [N P] Algorithm: 130
      Reachability         : 20.30.217.0/24 Metric: 10 Type: 1 Up
      Reachability         : 20.175.217.0/24 Metric: 10 Type: 1 Up
      Reachability (MT-IPv6): 2001:0:30:217::/64 Metric: 10 Type: 1 Up
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
    221.00-00                   424  21353   660     85 L2  0221.0221.0221.00-00  <>
      NLPID: 0xCC(IPv4) 0x8E(IPv6)
      Area addresses: 49.0001
      Router Capabilities: Router Id: 10.0.0.221 Flags: []
        SR Local Block:
          SRLB Base: 626688 Range: 14336
        Maximum SID depth:
          Base MPLS imposition (MSD type 1):  10
        SR Capability: Flags: [I]
          SRGB Base: 720000 Range: 2000
        Algorithms:  0, 128, 129
      Unsupported TLV: Type: 14 Length: 2
    221.00-01                   363   1789   473     32 L2  0221.0221.0221.00-01  <>
      Hostname: 221
    221.00-02                  8582  29014  1184    483 L2  0221.0221.0221.00-02  <>
      Remaining lifetime received: 1198 s Modified to: 1200 s
      Interface address: 10.0.0.221
      Interface address: 20.175.221.221
      Interface address: 20.30.221.221
      Interface address: 1221::1
      Interface address: 2001:0:175:221::221
      Interface address: 2001:0:30:221::221
      IS Neighbor          : Juniper-175-ACX7100-48L.00 Metric: 10
        IPv4 Neighbor Address: 20.175.221.175
        IPv4 Interface Address: 20.175.221.221
        Adj-sid: 524296 flags: [L V B] weight: 0x0
        Adj-sid: 524290 flags: [L V] weight: 0x0
      IS Neighbor          : Arista-Spine3-Q2A-30.00 Metric: 10
        IPv4 Neighbor Address: 20.30.221.30
        IPv4 Interface Address: 20.30.221.221
        Adj-sid: 524295 flags: [L V B] weight: 0x0
        Adj-sid: 524294 flags: [L V] weight: 0x0
      Reachability         : 10.0.0.221/32 Metric: 0 Type: 1 Up
        SR Prefix-SID: 221 Flags: [N] Algorithm: 0
        SR Prefix-SID: 1349 Flags: [N] Algorithm: 128
        SR Prefix-SID: 1350 Flags: [N] Algorithm: 129
      Reachability         : 20.175.221.0/24 Metric: 10 Type: 1 Up
      Reachability         : 20.30.221.0/24 Metric: 10 Type: 1 Up
      Reachability          : 1221::1/128 Metric: 0 Type: 1 Up
      Reachability          : 2001:0:175:221::/64 Metric: 10 Type: 1 Up
      Reachability          : 2001:0:30:221::/64 Metric: 10 Type: 1 Up

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
Number of times path updated: 1
Last updated: 0:33:04 ago
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
Number of times path updated: 1
Last updated: 0:33:04 ago
Metric: 100
Next Hop      Interface 
------------- ----------
20.30.221.221 Ethernet15

Destination: Arista-PE32-Q2C-32
Path ID: 640
Path constraints: algo MIN-LATENCY
                  metric type MIN-DELAY
Request sequence number: 0
Response sequence number: 0
Number of times path updated: 14
Last updated: 0:00:16 ago
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
Number of times path updated: 14
Last updated: 0:00:16 ago
Metric: 100
Next Hop    Interface
----------- ---------
20.30.32.32 Ethernet2

Destination: Arista-PE32-Q2C-32
Path ID: 642
Path constraints: algo ADMIN
                  metric type IGP
                  administrative-group exclude 1
Request sequence number: 0
Response sequence number: 0
Number of times path updated: 12
Last updated: 0:00:16 ago
Metric: 1
Next Hop    Interface
----------- ---------
20.30.32.32 Ethernet2

Destination: Arista-Spine3-Q2A-30
Path ID: 640
Path constraints: algo MIN-LATENCY
                  metric type MIN-DELAY
Request sequence number: 0
Response sequence number: 0
Number of times path updated: 1
Last updated: 7:42:48 ago
Next Hop Interface
-------- ---------

Destination: Arista-Spine3-Q2A-30
Path ID: 641
Path constraints: algo MIN-TE
                  metric type TE
Request sequence number: 0
Response sequence number: 0
Number of times path updated: 1
Last updated: 7:42:48 ago
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
Last updated: 7:42:48 ago
Next Hop Interface
-------- ---------

Destination: Arrcus-53
Path ID: 640
Path constraints: algo MIN-LATENCY
                  metric type MIN-DELAY
Request sequence number: 0
Response sequence number: 0
Number of times path updated: 26
Last updated: 0:11:30 ago
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
Number of times path updated: 26
Last updated: 0:11:30 ago
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
Number of times path updated: 21
Last updated: 0:11:30 ago
Metric: 1
Next Hop    Interface 
----------- ----------
20.30.53.53 Ethernet13

Destination: Ciena-5134-72
Path ID: 641
Path constraints: algo MIN-TE
                  metric type TE
Request sequence number: 0
Response sequence number: 0
Number of times path updated: 5
Last updated: 2:10:21 ago
Metric: 100
Next Hop    Interface
----------- ---------
20.30.72.72 Ethernet9

Destination: Ciena-8140-66
Path ID: 641
Path constraints: algo MIN-TE
                  metric type TE
Request sequence number: 0
Response sequence number: 0
Number of times path updated: 5
Last updated: 2:10:21 ago
Metric: 100
Next Hop    Interface 
----------- ----------
20.30.66.66 Ethernet31

Destination: H3C_M1A_120
Path ID: 640
Path constraints: algo MIN-LATENCY
                  metric type MIN-DELAY
Request sequence number: 0
Response sequence number: 0
Number of times path updated: 10
Last updated: 0:32:45 ago
Metric: 110010
Next Hop      Interface 
------------- ----------
20.30.221.221 Ethernet15

Destination: H3C_M1A_120
Path ID: 641
Path constraints: algo MIN-TE
                  metric type TE
Request sequence number: 0
Response sequence number: 0
Number of times path updated: 29
Last updated: 0:00:16 ago
Metric: 120
Next Hop      Interface 
------------- ----------
20.30.217.217 Ethernet4 
20.30.179.179 Ethernet40
20.30.221.221 Ethernet15
20.30.156.156 Ethernet11
20.30.53.53   Ethernet13
21.30.156.156 Ethernet21
20.30.32.32   Ethernet2 

Destination: H3C_M1A_120
Path ID: 642
Path constraints: algo ADMIN
                  metric type IGP
                  administrative-group exclude 1
Request sequence number: 0
Response sequence number: 0
Number of times path updated: 4
Last updated: 0:49:46 ago
Next Hop Interface
-------- ---------

Destination: Juniper-156-PTX10002-36QDD
Path ID: 640
Path constraints: algo MIN-LATENCY
                  metric type MIN-DELAY
Request sequence number: 0
Response sequence number: 0
Number of times path updated: 12
Last updated: 2:38:44 ago
Metric: 10000
Next Hop      Interface 
------------- ----------
20.30.156.156 Ethernet11
21.30.156.156 Ethernet21

Destination: Juniper-156-PTX10002-36QDD
Path ID: 641
Path constraints: algo MIN-TE
                  metric type TE
Request sequence number: 0
Response sequence number: 0
Number of times path updated: 15
Last updated: 2:38:44 ago
Metric: 100
Next Hop      Interface 
------------- ----------
20.30.156.156 Ethernet11
21.30.156.156 Ethernet21

Destination: Juniper-156-PTX10002-36QDD
Path ID: 642
Path constraints: algo ADMIN
                  metric type IGP
                  administrative-group exclude 1
Request sequence number: 0
Response sequence number: 0
Number of times path updated: 10
Last updated: 2:38:44 ago
Metric: 1
Next Hop      Interface 
------------- ----------
20.30.156.156 Ethernet11
21.30.156.156 Ethernet21

Destination: Juniper-175-ACX7100-48L
Path ID: 640
Path constraints: algo MIN-LATENCY
                  metric type MIN-DELAY
Request sequence number: 0
Response sequence number: 0
Number of times path updated: 30
Last updated: 0:32:45 ago
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
Number of times path updated: 177
Last updated: 0:00:16 ago
Metric: 110
Next Hop      Interface 
------------- ----------
20.30.217.217 Ethernet4 
20.30.179.179 Ethernet40
20.30.221.221 Ethernet15
20.30.156.156 Ethernet11
20.30.53.53   Ethernet13
21.30.156.156 Ethernet21
20.30.32.32   Ethernet2 

Destination: Juniper-175-ACX7100-48L
Path ID: 642
Path constraints: algo ADMIN
                  metric type IGP
                  administrative-group exclude 1
Request sequence number: 0
Response sequence number: 0
Number of times path updated: 16
Last updated: 0:49:46 ago
Metric: 11
Next Hop      Interface 
------------- ----------
20.30.131.131 Ethernet35

Destination: Juniper-179-ACX7024
Path ID: 640
Path constraints: algo MIN-LATENCY
                  metric type MIN-DELAY
Request sequence number: 0
Response sequence number: 0
Number of times path updated: 7
Last updated: 2:44:17 ago
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
Number of times path updated: 6
Last updated: 2:44:17 ago
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
Number of times path updated: 7
Last updated: 2:44:17 ago
Metric: 1
Next Hop      Interface 
------------- ----------
20.30.179.179 Ethernet40

Destination: Nokia-SR1-217
Path ID: 640
Path constraints: algo MIN-LATENCY
                  metric type MIN-DELAY
Request sequence number: 0
Response sequence number: 0
Number of times path updated: 29
Last updated: 0:10:42 ago
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
Number of times path updated: 29
Last updated: 0:10:42 ago
Metric: 100
Next Hop      Interface
------------- ---------
20.30.217.217 Ethernet4

Destination: Nokia-SR1-217
Path ID: 642
Path constraints: algo ADMIN
                  metric type IGP
                  administrative-group exclude 1
Request sequence number: 0
Response sequence number: 0
Number of times path updated: 24
Last updated: 0:10:42 ago
Metric: 1
Next Hop      Interface
------------- ---------
20.30.217.217 Ethernet4

Flex algo paths for IPv6 address family
Topology ID: Level-2
Destination: Arista-Spine3-Q2A-30
Path ID: 640
Path constraints: algo MIN-LATENCY
                  metric type MIN-DELAY
Request sequence number: 0
Response sequence number: 0
Number of times path updated: 1
Last updated: 1:39:27 ago
Next Hop Interface
-------- ---------

Destination: Arista-Spine3-Q2A-30
Path ID: 641
Path constraints: algo MIN-TE
                  metric type TE
Request sequence number: 0
Response sequence number: 0
Number of times path updated: 1
Last updated: 1:39:27 ago
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
Last updated: 1:39:27 ago
Next Hop Interface
-------- ---------

Destination: Arrcus-53
Path ID: 640
Path constraints: algo MIN-LATENCY
                  metric type MIN-DELAY
Request sequence number: 0
Response sequence number: 0
Number of times path updated: 24
Last updated: 0:11:30 ago
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
Number of times path updated: 21
Last updated: 0:11:30 ago
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
Number of times path updated: 16
Last updated: 0:11:30 ago
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
Number of times path updated: 2
Last updated: 0:45:03 ago
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
Last updated: 0:45:03 ago
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
Last updated: 0:45:03 ago
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
Number of times path updated: 5
Last updated: 2:38:44 ago
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
Number of times path updated: 4
Last updated: 2:38:44 ago
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
Number of times path updated: 6
Last updated: 2:38:44 ago
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
Number of times path updated: 18
Last updated: 0:11:30 ago
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
Number of times path updated: 34
Last updated: 0:00:16 ago
Metric: 110
Next Hop                  Interface 
------------------------- ----------
fe80::5e07:58ff:fea3:aaa  Ethernet13
fe80::d248:a1ff:feba:3c61 Ethernet11
fe80::d6af:f7ff:fe2f:1396 Ethernet2 

Destination: Juniper-175-ACX7100-48L
Path ID: 642
Path constraints: algo ADMIN
                  metric type IGP
                  administrative-group exclude 1
Request sequence number: 0
Response sequence number: 0
Number of times path updated: 20
Last updated: 0:10:42 ago
Metric: 20
Next Hop                  Interface
------------------------- ---------
fe80::c214:b8ff:fe21:9790 Ethernet4

```

## show isis segment-routing tunnel

```text
 Index    Endpoint         Next Hop/Tunnel Index         Interface    Labels   
-------- ---------------- ---------------------------- -------------- ---------
 2        2002::120/128    fe80::be31:e2ff:fee1:ec2c     Ethernet3    [ 3 ]    
 3        2002::175/128    fe80::5a70:7fff:fe9f:c403     Ethernet12   [ 20575 ]
                           fe80::5e07:58ff:fea3:aaa      Ethernet13   [ 20575 ]
                           fe80::be31:e2ff:fee1:ec2c     Ethernet3    [ 20575 ]
                           fe80::c214:b8ff:fe21:9790     Ethernet4    [ 20575 ]
                           fe80::d248:a1ff:feba:3c61     Ethernet11   [ 20575 ]
                           fe80::d6af:f7ff:fe2f:1396     Ethernet2    [ 20575 ]
 5        2002::156/128    TI-LFA (8)                    -            [ 3 ]    
 6        2002::53/128     TI-LFA (10)                   -            [ 3 ]    
 7        10.0.0.175/32    20.30.32.32                   Ethernet2    [ 20175 ]
                           20.30.53.53                   Ethernet13   [ 20175 ]
                           20.30.66.66                   Ethernet31   [ 20175 ]
                           20.30.72.72                   Ethernet9    [ 20175 ]
                           20.30.84.84                   Ethernet12   [ 20175 ]
                           20.30.120.120                 Ethernet3    [ 20175 ]
                           20.30.131.131                 Ethernet35   [ 20175 ]
 8        10.0.0.84/32     TI-LFA (2)                    -            [ 20084 ]
 9        10.0.0.131/32    TI-LFA (3)                    -            [ 3 ]    
 10       10.0.0.53/32     TI-LFA (17)                   -            [ 3 ]    
 11       10.0.0.156/32    20.30.156.156                 Ethernet11   [ 3 ]    
                           21.30.156.156                 Ethernet21   [ 3 ]    
 12       10.0.0.179/32    20.30.179.179                 Ethernet40   [ 3 ]    
 13       10.0.0.66/32     TI-LFA (18)                   -            [ 3 ]    
 14       10.0.0.72/32     TI-LFA (4)                    -            [ 3 ]    
 15       10.0.0.221/32    TI-LFA (6)                    -            [ 3 ]    
 16       10.0.0.217/32    TI-LFA (0)                    -            [ 20217 ]
 17       10.0.0.120/32    20.30.120.120                 Ethernet3    [ 3 ]    
                           21.30.120.120                 Ethernet10   [ 3 ]    
 20       10.0.0.32/32     TI-LFA (11)                   -            [ 3 ]    
 21       10.0.0.214/32    20.30.214.214                 Ethernet5    [ 20214 ]
                           21.30.214.214                 Ethernet6    [ 20214 ]

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
*  10.0.0.30/32                158   20158 Node       R:0 N:1 P:0 E:0 V:0 L:0      Arista-Spine3-Q2A-30 L2    unprotected MIN-LATENCY 
*  10.0.0.30/32                159   20159 Node       R:0 N:1 P:0 E:0 V:0 L:0      Arista-Spine3-Q2A-30 L2    unprotected MIN-TE      
*  10.0.0.30/32                160   20160 Node       R:0 N:1 P:0 E:0 V:0 L:0      Arista-Spine3-Q2A-30 L2    unprotected ADMIN       
   10.0.0.32/32                 32   20032 Node       R:0 N:1 P:0 E:0 V:0 L:0      Arista-PE32-Q2C-32 L2    node        SPF         
   10.0.0.32/32                161   20161 Node       R:0 N:1 P:0 E:0 V:0 L:0      Arista-PE32-Q2C-32 L2    node        MIN-LATENCY 
   10.0.0.32/32                162   20162 Node       R:0 N:1 P:0 E:0 V:0 L:0      Arista-PE32-Q2C-32 L2    node        MIN-TE      
   10.0.0.32/32                163   20163 Node       R:0 N:1 P:0 E:0 V:0 L:0      Arista-PE32-Q2C-32 L2    node        ADMIN       
   10.0.0.53/32                 53   20053 Node       R:0 N:1 P:1 E:1 V:0 L:0      Arrcus-53       L2    node        SPF         
   10.0.0.53/32               1181   21181 Node       R:0 N:1 P:0 E:0 V:0 L:0      Arrcus-53       L2    node        MIN-LATENCY 
   10.0.0.53/32               1182   21182 Node       R:0 N:1 P:0 E:0 V:0 L:0      Arrcus-53       L2    node        MIN-TE      
   10.0.0.53/32               1183   21183 Node       R:0 N:1 P:0 E:0 V:0 L:0      Arrcus-53       L2    node        ADMIN       
   10.0.0.66/32                 66   20066 Node       R:0 N:1 P:0 E:0 V:0 L:0      Ciena-8140-66   L2    node        SPF         
   10.0.0.66/32               1195   21195 Node       R:0 N:1 P:0 E:0 V:0 L:0      Ciena-8140-66   L2    node        MIN-TE      
   10.0.0.72/32                 72   20072 Node       R:0 N:1 P:0 E:0 V:0 L:0      Ciena-5134-72   L2    node        SPF         
   10.0.0.72/32               1201   21201 Node       R:0 N:1 P:0 E:0 V:0 L:0      Ciena-5134-72   L2    node        MIN-TE      
   10.0.0.84/32                 84   20084 Node       R:0 N:1 P:1 E:0 V:0 L:0      Ericsson_84_R6678 L2    node        SPF         
   10.0.0.120/32               120   20120 Node       R:0 N:1 P:0 E:0 V:0 L:0      H3C_M1A_120     L2    unprotected SPF         
   10.0.0.120/32              1248   21248 Node       R:0 N:1 P:0 E:0 V:0 L:0      H3C_M1A_120     L2    node        MIN-LATENCY 
   10.0.0.120/32              1249   21249 Node       R:0 N:1 P:0 E:0 V:0 L:0      H3C_M1A_120     L2    unprotected MIN-TE      
   10.0.0.120/32              1250   21250 Node       R:0 N:1 P:0 E:0 V:0 L:0      H3C_M1A_120     L2    unprotected ADMIN       
   10.0.0.131/32               131   20131 Node       R:0 N:1 P:0 E:0 V:0 L:0      Juniper-131-JCNR L2    node        SPF         
   10.0.0.156/32               156   20156 Node       R:0 N:1 P:0 E:0 V:0 L:0      Juniper-156-PTX10002-36QDD L2    unprotected SPF         
   10.0.0.156/32              1284   21284 Node       R:0 N:1 P:0 E:0 V:0 L:0      Juniper-156-PTX10002-36QDD L2    unprotected MIN-LATENCY 
   10.0.0.156/32              1285   21285 Node       R:0 N:1 P:0 E:0 V:0 L:0      Juniper-156-PTX10002-36QDD L2    unprotected MIN-TE      
   10.0.0.156/32              1286   21286 Node       R:0 N:1 P:0 E:0 V:0 L:0      Juniper-156-PTX10002-36QDD L2    unprotected ADMIN       
   10.0.0.175/32               175   20175 Node       R:0 N:1 P:0 E:0 V:0 L:0      Juniper-175-ACX7100-48L L2    unprotected SPF         
   10.0.0.175/32              1303   21303 Node       R:0 N:1 P:0 E:0 V:0 L:0      Juniper-175-ACX7100-48L L2    node        MIN-LATENCY 
   10.0.0.175/32              1304   21304 Node       R:0 N:1 P:0 E:0 V:0 L:0      Juniper-175-ACX7100-48L L2    unprotected MIN-TE      
   10.0.0.175/32              1305   21305 Node       R:0 N:1 P:0 E:0 V:0 L:0      Juniper-175-ACX7100-48L L2    node        ADMIN       
   10.0.0.179/32               179   20179 Node       R:0 N:1 P:0 E:0 V:0 L:0      Juniper-179-ACX7024 L2    node        SPF         
   10.0.0.179/32              1307   21307 Node       R:0 N:1 P:0 E:0 V:0 L:0      Juniper-179-ACX7024 L2    node        MIN-LATENCY 
   10.0.0.179/32              1308   21308 Node       R:0 N:1 P:0 E:0 V:0 L:0      Juniper-179-ACX7024 L2    node        MIN-TE      
   10.0.0.179/32              1309   21309 Node       R:0 N:1 P:0 E:0 V:0 L:0      Juniper-179-ACX7024 L2    node        ADMIN       
   10.0.0.214/32               214   20214 Node       R:0 N:1 P:1 E:0 V:0 L:0      Nokia-SXR-214   L2    unprotected SPF         
   10.0.0.217/32               217   20217 Node       R:0 N:1 P:1 E:0 V:0 L:0      Nokia-SR1-217   L2    node        SPF         
   10.0.0.217/32              1345   21345 Node       R:0 N:1 P:1 E:0 V:0 L:0      Nokia-SR1-217   L2    node        MIN-LATENCY 
   10.0.0.217/32              1346   21346 Node       R:0 N:1 P:1 E:0 V:0 L:0      Nokia-SR1-217   L2    node        MIN-TE      
   10.0.0.217/32              1347   21347 Node       R:0 N:1 P:1 E:0 V:0 L:0      Nokia-SR1-217   L2    node        ADMIN       
   10.0.0.221/32               221  720221 Node       R:0 N:1 P:0 E:0 V:0 L:0      221             L2    node        SPF         
   10.0.0.221/32              1349  721349 Node       R:0 N:1 P:0 E:0 V:0 L:0      221             L2    node        MIN-LATENCY 
   10.0.0.221/32              1350  721350 Node       R:0 N:1 P:0 E:0 V:0 L:0      221             L2    node        MIN-TE      
*  2002::30/128                430   20430 Node       R:0 N:1 P:0 E:0 V:0 L:0      Arista-Spine3-Q2A-30 L2    unprotected SPF         
*  2002::30/128                558   20558 Node       R:0 N:1 P:0 E:0 V:0 L:0      Arista-Spine3-Q2A-30 L2    unprotected MIN-LATENCY 
*  2002::30/128                559   20559 Node       R:0 N:1 P:0 E:0 V:0 L:0      Arista-Spine3-Q2A-30 L2    unprotected MIN-TE      
*  2002::30/128                560   20560 Node       R:0 N:1 P:0 E:0 V:0 L:0      Arista-Spine3-Q2A-30 L2    unprotected ADMIN       
   2002::53/128                453   20453 Node       R:0 N:1 P:1 E:1 V:0 L:0      Arrcus-53       L2    node        SPF         
   2002::53/128               1581   21581 Node       R:0 N:1 P:0 E:0 V:0 L:0      Arrcus-53       L2    node        MIN-LATENCY 
   2002::53/128               1582   21582 Node       R:0 N:1 P:0 E:0 V:0 L:0      Arrcus-53       L2    node        MIN-TE      
   2002::53/128               1583   21583 Node       R:0 N:1 P:0 E:0 V:0 L:0      Arrcus-53       L2    node        ADMIN       
   2002::120/128               520   20520 Node       R:0 N:1 P:0 E:0 V:0 L:0      H3C_M1A_120     L2    node        SPF         
   2002::120/128              1648   21648 Node       R:0 N:1 P:0 E:0 V:0 L:0      H3C_M1A_120     L2    node        MIN-LATENCY 
   2002::120/128              1649   21649 Node       R:0 N:1 P:0 E:0 V:0 L:0      H3C_M1A_120     L2    node        MIN-TE      
   2002::120/128              1650   21650 Node       R:0 N:1 P:0 E:0 V:0 L:0      H3C_M1A_120     L2    node        ADMIN       
   2002::156/128               556   20556 Node       R:0 N:1 P:0 E:0 V:0 L:0      Juniper-156-PTX10002-36QDD L2    node        SPF         
   2002::156/128              1684   21684 Node       R:0 N:1 P:0 E:0 V:0 L:0      Juniper-156-PTX10002-36QDD L2    node        MIN-LATENCY 
   2002::156/128              1685   21685 Node       R:0 N:1 P:0 E:0 V:0 L:0      Juniper-156-PTX10002-36QDD L2    node        MIN-TE      
   2002::156/128              1686   21686 Node       R:0 N:1 P:0 E:0 V:0 L:0      Juniper-156-PTX10002-36QDD L2    node        ADMIN       
   2002::175/128               575   20575 Node       R:0 N:1 P:0 E:0 V:0 L:0      Juniper-175-ACX7100-48L L2    unprotected SPF         
   2002::175/128              1703   21703 Node       R:0 N:1 P:0 E:0 V:0 L:0      Juniper-175-ACX7100-48L L2    node        MIN-LATENCY 
   2002::175/128              1704   21704 Node       R:0 N:1 P:0 E:0 V:0 L:0      Juniper-175-ACX7100-48L L2    unprotected MIN-TE      
   2002::175/128              1705   21705 Node       R:0 N:1 P:0 E:0 V:0 L:0      Juniper-175-ACX7100-48L L2    node        ADMIN       
```

## show isis ti-lfa path detail

```text
TI-LFA paths for IPv4 address family
   Topology ID: Level-2
   Destination: Arista-PE32-Q2C-32
      Path constraint: exclude Ethernet2
                       algorithm SPF (0)
         Request sequence number: 1
         Response sequence number: 1
         Number of times path updated: 1
         Last updated: 0:00:16 ago
         ID: 0x16
         Path:
            Juniper-179-ACX7024 [PQ-node]
      Path constraint: exclude node 0000.0000.0032
                       algorithm SPF (0)
         Request sequence number: 1
         Response sequence number: 1
         Number of times path updated: 1
         Last updated: 0:00:16 ago
         ID: 0x17
         Path: Path not found
      Path constraint: exclude Ethernet2
                       flex-algo algorithm MIN-LATENCY (128)
                         metric type TE
         Request sequence number: 1
         Response sequence number: 1
         Number of times path updated: 1
         Last updated: 0:00:16 ago
         ID: 0x18
         Path:
            Juniper-175-ACX7100-48L [PQ-node]
      Path constraint: exclude node 0000.0000.0032
                       flex-algo algorithm MIN-LATENCY (128)
                         metric type TE
         Request sequence number: 1
         Response sequence number: 1
         Number of times path updated: 1
         Last updated: 0:00:16 ago
         ID: 0x19
         Path: Path not found
      Path constraint: exclude Ethernet2
                       flex-algo algorithm MIN-TE (129)
                         metric type TE
         Request sequence number: 1
         Response sequence number: 1
         Number of times path updated: 1
         Last updated: 0:00:16 ago
         ID: 0x1a
         Path:
            Nokia-SR1-217 [PQ-node]
      Path constraint: exclude node 0000.0000.0032
                       flex-algo algorithm MIN-TE (129)
                         metric type TE
         Request sequence number: 1
         Response sequence number: 1
         Number of times path updated: 1
         Last updated: 0:00:16 ago
         ID: 0x1b
         Path: Path not found
      Path constraint: exclude Ethernet2
                       flex-algo algorithm ADMIN (130)
                         metric type TE
         Request sequence number: 1
         Response sequence number: 1
         Number of times path updated: 1
         Last updated: 0:00:16 ago
         ID: 0x1c
         Path: Path not found
      Path constraint: exclude node 0000.0000.0032
                       flex-algo algorithm ADMIN (130)
                         metric type TE
         Request sequence number: 1
         Response sequence number: 1
         Number of times path updated: 1
         Last updated: 0:00:16 ago
         ID: 0x1d
         Path: Path not found

   Destination: Arrcus-53
      Path constraint: exclude Ethernet13
                       algorithm SPF (0)
         Request sequence number: 1
         Response sequence number: 1
         Number of times path updated: 1
         Last updated: 0:11:30 ago
         ID: 0xe
         Path:
            Juniper-179-ACX7024 [PQ-node]
      Path constraint: exclude node 0000.0000.0053
                       algorithm SPF (0)
         Request sequence number: 1
         Response sequence number: 1
         Number of times path updated: 1
         Last updated: 0:11:30 ago
         ID: 0xf
         Path: Path not found
      Path constraint: exclude Ethernet13
                       flex-algo algorithm MIN-LATENCY (128)
                         metric type TE
         Request sequence number: 1
         Response sequence number: 1
         Number of times path updated: 1
         Last updated: 0:11:30 ago
         ID: 0x10
         Path:
            Juniper-175-ACX7100-48L [PQ-node]
      Path constraint: exclude node 0000.0000.0053
                       flex-algo algorithm MIN-LATENCY (128)
                         metric type TE
         Request sequence number: 1
         Response sequence number: 1
         Number of times path updated: 1
         Last updated: 0:11:30 ago
         ID: 0x11
         Path: Path not found
      Path constraint: exclude Ethernet13
                       flex-algo algorithm MIN-TE (129)
                         metric type TE
         Request sequence number: 1
         Response sequence number: 1
         Number of times path updated: 2
         Last updated: 0:11:07 ago
         ID: 0x12
         Path:
            221 [PQ-node]
      Path constraint: exclude node 0000.0000.0053
                       flex-algo algorithm MIN-TE (129)
                         metric type TE
         Request sequence number: 1
         Response sequence number: 1
         Number of times path updated: 1
         Last updated: 0:11:30 ago
         ID: 0x13
         Path: Path not found
      Path constraint: exclude Ethernet13
                       flex-algo algorithm ADMIN (130)
                         metric type TE
         Request sequence number: 1
         Response sequence number: 1
         Number of times path updated: 1
         Last updated: 0:11:30 ago
         ID: 0x24
         Path: Path not found
      Path constraint: exclude node 0000.0000.0053
                       flex-algo algorithm ADMIN (130)
                         metric type TE
         Request sequence number: 1
         Response sequence number: 1
         Number of times path updated: 1
         Last updated: 0:11:30 ago
         ID: 0x25
         Path: Path not found

   Destination: Ciena-8140-66
      Path constraint: exclude Ethernet31
                       algorithm SPF (0)
         Request sequence number: 1
         Response sequence number: 1
         Number of times path updated: 1
         Last updated: 2:10:21 ago
         ID: 0xc
         Path:
            Juniper-179-ACX7024 [PQ-node]
      Path constraint: exclude node 0000.0000.0066
                       algorithm SPF (0)
         Request sequence number: 1
         Response sequence number: 1
         Number of times path updated: 1
         Last updated: 2:10:21 ago
         ID: 0xd
         Path: Path not found
      Path constraint: exclude Ethernet31
                       flex-algo algorithm MIN-TE (129)
                         metric type TE
         Request sequence number: 1
         Response sequence number: 1
         Number of times path updated: 2
         Last updated: 2:01:03 ago
         ID: 0x20
         Path:
            Juniper-179-ACX7024 [PQ-node]
      Path constraint: exclude node 0000.0000.0066
                       flex-algo algorithm MIN-TE (129)
                         metric type TE
         Request sequence number: 1
         Response sequence number: 1
         Number of times path updated: 1
         Last updated: 2:10:21 ago
         ID: 0x21
         Path: Path not found

   Destination: Ciena-5134-72
      Path constraint: exclude Ethernet9
                       algorithm SPF (0)
         Request sequence number: 1
         Response sequence number: 1
         Number of times path updated: 1
         Last updated: 2:10:22 ago
         ID: 0x8
         Path:
            Juniper-179-ACX7024 [PQ-node]
      Path constraint: exclude node 0000.0000.0072
                       algorithm SPF (0)
         Request sequence number: 1
         Response sequence number: 1
         Number of times path updated: 1
         Last updated: 2:10:22 ago
         ID: 0x9
         Path: Path not found
      Path constraint: exclude Ethernet9
                       flex-algo algorithm MIN-TE (129)
                         metric type TE
         Request sequence number: 1
         Response sequence number: 1
         Number of times path updated: 4
         Last updated: 0:04:00 ago
         ID: 0x1e
         Path:
            Juniper-156-PTX10002-36QDD [PQ-node]
      Path constraint: exclude node 0000.0000.0072
                       flex-algo algorithm MIN-TE (129)
                         metric type TE
         Request sequence number: 1
         Response sequence number: 1
         Number of times path updated: 1
         Last updated: 2:10:21 ago
         ID: 0x1f
         Path: Path not found

   Destination: Ericsson_84_R6678
      Path constraint: exclude Ethernet12
                       algorithm SPF (0)
         Request sequence number: 1
         Response sequence number: 1
         Number of times path updated: 1
         Last updated: 1:21:44 ago
         ID: 0x0
         Path:
            Juniper-179-ACX7024 [PQ-node]
      Path constraint: exclude node 0000.0000.0084
                       algorithm SPF (0)
         Request sequence number: 1
         Response sequence number: 1
         Number of times path updated: 1
         Last updated: 1:21:44 ago
         ID: 0x1
         Path: Path not found

   Destination: H3C_M1A_120
      Path constraint: exclude Ethernet15
                       flex-algo algorithm MIN-LATENCY (128)
                         metric type TE
         Request sequence number: 1
         Response sequence number: 1
         Number of times path updated: 7
         Last updated: 0:11:30 ago
         ID: 0x2e
         Path:
            Arrcus-53 [PQ-node]
      Path constraint: exclude node 0221.0221.0221
                       flex-algo algorithm MIN-LATENCY (128)
                         metric type TE
         Request sequence number: 1
         Response sequence number: 1
         Number of times path updated: 7
         Last updated: 0:11:30 ago
         ID: 0x2f
         Path:
            Arrcus-53 [PQ-node]

   Destination: Juniper-131-JCNR
      Path constraint: exclude Ethernet35
                       algorithm SPF (0)
         Request sequence number: 1
         Response sequence number: 1
         Number of times path updated: 4
         Last updated: 2:44:17 ago
         ID: 0x30
         Path:
            Juniper-179-ACX7024 [PQ-node]
      Path constraint: exclude node 0000.0000.0131
                       algorithm SPF (0)
         Request sequence number: 1
         Response sequence number: 1
         Number of times path updated: 1
         Last updated: 23:34:28 ago
         ID: 0x31
         Path: Path not found

   Destination: Juniper-175-ACX7100-48L
      Path constraint: exclude Ethernet35
                       flex-algo algorithm ADMIN (130)
                         metric type TE
         Request sequence number: 1
         Response sequence number: 1
         Number of times path updated: 1
         Last updated: 0:49:46 ago
         ID: 0x26
         Path: Path not found
      Path constraint: exclude node 0000.0000.0131
                       flex-algo algorithm ADMIN (130)
                         metric type TE
         Request sequence number: 1
         Response sequence number: 1
         Number of times path updated: 1
         Last updated: 0:49:46 ago
         ID: 0x27
         Path: Path not found
      Path constraint: exclude Ethernet15
                       flex-algo algorithm MIN-LATENCY (128)
                         metric type TE
         Request sequence number: 1
         Response sequence number: 1
         Number of times path updated: 7
         Last updated: 0:11:30 ago
         ID: 0x2a
         Path:
            Arrcus-53 [PQ-node]
      Path constraint: exclude node 0221.0221.0221
                       flex-algo algorithm MIN-LATENCY (128)
                         metric type TE
         Request sequence number: 1
         Response sequence number: 1
         Number of times path updated: 7
         Last updated: 0:11:30 ago
         ID: 0x2b
         Path:
            Arrcus-53 [PQ-node]

   Destination: Juniper-179-ACX7024
      Path constraint: exclude Ethernet40
                       algorithm SPF (0)
         Request sequence number: 1
         Response sequence number: 1
         Number of times path updated: 5
         Last updated: 0:32:34 ago
         ID: 0x14
         Path:
            Juniper-175-ACX7100-48L [PQ-node]
      Path constraint: exclude node 0000.0000.0179
                       algorithm SPF (0)
         Request sequence number: 1
         Response sequence number: 1
         Number of times path updated: 1
         Last updated: 2:44:17 ago
         ID: 0x15
         Path: Path not found
      Path constraint: exclude Ethernet40
                       flex-algo algorithm MIN-LATENCY (128)
                         metric type TE
         Request sequence number: 1
         Response sequence number: 1
         Number of times path updated: 4
         Last updated: 0:32:45 ago
         ID: 0x22
         Path:
            Juniper-175-ACX7100-48L [PQ-node]
      Path constraint: exclude node 0000.0000.0179
                       flex-algo algorithm MIN-LATENCY (128)
                         metric type TE
         Request sequence number: 1
         Response sequence number: 1
         Number of times path updated: 1
         Last updated: 2:44:17 ago
         ID: 0x23
         Path: Path not found
      Path constraint: exclude Ethernet40
                       flex-algo algorithm ADMIN (130)
                         metric type TE
         Request sequence number: 1
         Response sequence number: 1
         Number of times path updated: 1
         Last updated: 2:44:17 ago
         ID: 0x28
         Path: Path not found
      Path constraint: exclude node 0000.0000.0179
                       flex-algo algorithm ADMIN (130)
                         metric type TE
         Request sequence number: 1
         Response sequence number: 1
         Number of times path updated: 1
         Last updated: 2:44:17 ago
         ID: 0x29
         Path: Path not found
      Path constraint: exclude Ethernet40
                       flex-algo algorithm MIN-TE (129)
                         metric type TE
         Request sequence number: 1
         Response sequence number: 1
         Number of times path updated: 4
         Last updated: 0:32:51 ago
         ID: 0x2c
         Path:
            Juniper-156-PTX10002-36QDD [PQ-node]
      Path constraint: exclude node 0000.0000.0179
                       flex-algo algorithm MIN-TE (129)
                         metric type TE
         Request sequence number: 1
         Response sequence number: 1
         Number of times path updated: 1
         Last updated: 2:44:17 ago
         ID: 0x2d
         Path: Path not found

   Destination: Nokia-SR1-217
      Path constraint: exclude Ethernet4
                       algorithm SPF (0)
         Request sequence number: 1
         Response sequence number: 1
         Number of times path updated: 1
         Last updated: 0:10:42 ago
         ID: 0x6
         Path:
            Juniper-179-ACX7024 [PQ-node]
      Path constraint: exclude node 0100.0000.0217
                       algorithm SPF (0)
         Request sequence number: 1
         Response sequence number: 1
         Number of times path updated: 1
         Last updated: 0:10:42 ago
         ID: 0x7
         Path: Path not found
      Path constraint: exclude Ethernet4
                       flex-algo algorithm MIN-LATENCY (128)
                         metric type TE
         Request sequence number: 1
         Response sequence number: 1
         Number of times path updated: 1
         Last updated: 0:10:42 ago
         ID: 0x34
         Path:
            Juniper-175-ACX7100-48L [PQ-node]
      Path constraint: exclude node 0100.0000.0217
                       flex-algo algorithm MIN-LATENCY (128)
                         metric type TE
         Request sequence number: 1
         Response sequence number: 1
         Number of times path updated: 1
         Last updated: 0:10:42 ago
         ID: 0x35
         Path: Path not found
      Path constraint: exclude Ethernet4
                       flex-algo algorithm MIN-TE (129)
                         metric type TE
         Request sequence number: 1
         Response sequence number: 1
         Number of times path updated: 1
         Last updated: 0:10:42 ago
         ID: 0x36
         Path:
            Juniper-179-ACX7024 [PQ-node]
      Path constraint: exclude node 0100.0000.0217
                       flex-algo algorithm MIN-TE (129)
                         metric type TE
         Request sequence number: 1
         Response sequence number: 1
         Number of times path updated: 1
         Last updated: 0:10:42 ago
         ID: 0x37
         Path: Path not found
      Path constraint: exclude Ethernet4
                       flex-algo algorithm ADMIN (130)
                         metric type TE
         Request sequence number: 1
         Response sequence number: 1
         Number of times path updated: 1
         Last updated: 0:10:42 ago
         ID: 0x38
         Path: Path not found
      Path constraint: exclude node 0100.0000.0217
                       flex-algo algorithm ADMIN (130)
                         metric type TE
         Request sequence number: 1
         Response sequence number: 1
         Number of times path updated: 1
         Last updated: 0:10:42 ago
         ID: 0x39
         Path: Path not found

   Destination: 221
      Path constraint: exclude Ethernet15
                       algorithm SPF (0)
         Request sequence number: 1
         Response sequence number: 1
         Number of times path updated: 1
         Last updated: 0:26:38 ago
         ID: 0x2
         Path:
            Juniper-179-ACX7024 [PQ-node]
      Path constraint: exclude node 0221.0221.0221
                       algorithm SPF (0)
         Request sequence number: 1
         Response sequence number: 1
         Number of times path updated: 1
         Last updated: 0:26:38 ago
         ID: 0x3
         Path: Path not found
      Path constraint: exclude Ethernet15
                       flex-algo algorithm MIN-TE (129)
                         metric type TE
         Request sequence number: 1
         Response sequence number: 1
         Number of times path updated: 2
         Last updated: 0:32:45 ago
         ID: 0x4
         Path:
            Juniper-179-ACX7024 [PQ-node]
      Path constraint: exclude node 0221.0221.0221
                       flex-algo algorithm MIN-TE (129)
                         metric type TE
         Request sequence number: 1
         Response sequence number: 1
         Number of times path updated: 1
         Last updated: 0:33:04 ago
         ID: 0x5
         Path: Path not found
      Path constraint: exclude Ethernet15
                       flex-algo algorithm MIN-LATENCY (128)
                         metric type TE
         Request sequence number: 1
         Response sequence number: 1
         Number of times path updated: 8
         Last updated: 0:11:30 ago
         ID: 0xa
         Path:
            Juniper-175-ACX7100-48L [PQ-node]
      Path constraint: exclude node 0221.0221.0221
                       flex-algo algorithm MIN-LATENCY (128)
                         metric type TE
         Request sequence number: 1
         Response sequence number: 1
         Number of times path updated: 1
         Last updated: 0:33:04 ago
         ID: 0xb
         Path: Path not found

TI-LFA paths for IPv6 address family
   Topology ID: Level-2
   Destination: Arrcus-53
      Path constraint: exclude Ethernet13
                       algorithm SPF (0)
         Request sequence number: 1
         Response sequence number: 1
         Number of times path updated: 2
         Last updated: 0:08:00 ago
         ID: 0x4
         Path:
            Juniper-175-ACX7100-48L [PQ-node]
      Path constraint: exclude node 0000.0000.0053
                       algorithm SPF (0)
         Request sequence number: 1
         Response sequence number: 1
         Number of times path updated: 1
         Last updated: 0:11:30 ago
         ID: 0x5
         Path: Path not found
      Path constraint: exclude Ethernet13
                       flex-algo algorithm MIN-TE (129)
                         metric type TE
         Request sequence number: 1
         Response sequence number: 1
         Number of times path updated: 1
         Last updated: 0:11:30 ago
         ID: 0x6
         Path:
            Juniper-156-PTX10002-36QDD [PQ-node]
      Path constraint: exclude node 0000.0000.0053
                       flex-algo algorithm MIN-TE (129)
                         metric type TE
         Request sequence number: 1
         Response sequence number: 1
         Number of times path updated: 1
         Last updated: 0:11:30 ago
         ID: 0x7
         Path: Path not found
      Path constraint: exclude Ethernet13
                       flex-algo algorithm ADMIN (130)
                         metric type TE
         Request sequence number: 1
         Response sequence number: 1
         Number of times path updated: 1
         Last updated: 0:11:30 ago
         ID: 0xa
         Path: Path not found
      Path constraint: exclude node 0000.0000.0053
                       flex-algo algorithm ADMIN (130)
                         metric type TE
         Request sequence number: 1
         Response sequence number: 1
         Number of times path updated: 1
         Last updated: 0:11:30 ago
         ID: 0xb
         Path: Path not found
      Path constraint: exclude Ethernet13
                       flex-algo algorithm MIN-LATENCY (128)
                         metric type TE
         Request sequence number: 1
         Response sequence number: 1
         Number of times path updated: 1
         Last updated: 0:11:30 ago
         ID: 0xc
         Path:
            Juniper-156-PTX10002-36QDD [P-node]
            Juniper-175-ACX7100-48L [Q-node]
      Path constraint: exclude node 0000.0000.0053
                       flex-algo algorithm MIN-LATENCY (128)
                         metric type TE
         Request sequence number: 1
         Response sequence number: 1
         Number of times path updated: 1
         Last updated: 0:11:30 ago
         ID: 0xd
         Path: Path not found

   Destination: H3C_M1A_120
      Path constraint: exclude Ethernet3
                       algorithm SPF (0)
         Request sequence number: 1
         Response sequence number: 1
         Number of times path updated: 1
         Last updated: 0:45:04 ago
         ID: 0x8
         Path: Path not found
      Path constraint: exclude node 0000.0000.0120
                       algorithm SPF (0)
         Request sequence number: 1
         Response sequence number: 1
         Number of times path updated: 1
         Last updated: 0:45:04 ago
         ID: 0x9
         Path: Path not found
      Path constraint: exclude Ethernet3
                       flex-algo algorithm MIN-TE (129)
                         metric type TE
         Request sequence number: 1
         Response sequence number: 1
         Number of times path updated: 1
         Last updated: 0:45:04 ago
         ID: 0x16
         Path: Path not found
      Path constraint: exclude node 0000.0000.0120
                       flex-algo algorithm MIN-TE (129)
                         metric type TE
         Request sequence number: 1
         Response sequence number: 1
         Number of times path updated: 1
         Last updated: 0:45:04 ago
         ID: 0x17
         Path: Path not found
      Path constraint: exclude Ethernet3
                       flex-algo algorithm MIN-LATENCY (128)
                         metric type TE
         Request sequence number: 1
         Response sequence number: 1
         Number of times path updated: 1
         Last updated: 0:45:04 ago
         ID: 0x18
         Path: Path not found
      Path constraint: exclude node 0000.0000.0120
                       flex-algo algorithm MIN-LATENCY (128)
                         metric type TE
         Request sequence number: 1
         Response sequence number: 1
         Number of times path updated: 1
         Last updated: 0:45:04 ago
         ID: 0x19
         Path: Path not found
      Path constraint: exclude Ethernet3
                       flex-algo algorithm ADMIN (130)
                         metric type TE
         Request sequence number: 1
         Response sequence number: 1
         Number of times path updated: 1
         Last updated: 0:45:04 ago
         ID: 0x1a
         Path: Path not found
      Path constraint: exclude node 0000.0000.0120
                       flex-algo algorithm ADMIN (130)
                         metric type TE
         Request sequence number: 1
         Response sequence number: 1
         Number of times path updated: 1
         Last updated: 0:45:04 ago
         ID: 0x1b
         Path: Path not found

   Destination: Juniper-156-PTX10002-36QDD
      Path constraint: exclude Ethernet11
                       algorithm SPF (0)
         Request sequence number: 1
         Response sequence number: 1
         Number of times path updated: 3
         Last updated: 0:08:00 ago
         ID: 0x0
         Path:
            Juniper-175-ACX7100-48L [PQ-node]
      Path constraint: exclude node 0000.0000.0156
                       algorithm SPF (0)
         Request sequence number: 1
         Response sequence number: 1
         Number of times path updated: 1
         Last updated: 2:38:45 ago
         ID: 0x1
         Path: Path not found
      Path constraint: exclude Ethernet11
                       flex-algo algorithm MIN-TE (129)
                         metric type TE
         Request sequence number: 1
         Response sequence number: 1
         Number of times path updated: 5
         Last updated: 0:04:00 ago
         ID: 0x10
         Path:
            Arrcus-53 [PQ-node]
      Path constraint: exclude node 0000.0000.0156
                       flex-algo algorithm MIN-TE (129)
                         metric type TE
         Request sequence number: 1
         Response sequence number: 1
         Number of times path updated: 1
         Last updated: 2:38:45 ago
         ID: 0x11
         Path: Path not found
      Path constraint: exclude Ethernet11
                       flex-algo algorithm MIN-LATENCY (128)
                         metric type TE
         Request sequence number: 1
         Response sequence number: 1
         Number of times path updated: 7
         Last updated: 0:11:30 ago
         ID: 0x12
         Path:
            Juniper-175-ACX7100-48L [PQ-node]
      Path constraint: exclude node 0000.0000.0156
                       flex-algo algorithm MIN-LATENCY (128)
                         metric type TE
         Request sequence number: 1
         Response sequence number: 1
         Number of times path updated: 1
         Last updated: 2:38:45 ago
         ID: 0x13
         Path: Path not found
      Path constraint: exclude Ethernet11
                       flex-algo algorithm ADMIN (130)
                         metric type TE
         Request sequence number: 1
         Response sequence number: 1
         Number of times path updated: 1
         Last updated: 2:38:45 ago
         ID: 0x14
         Path: Path not found
      Path constraint: exclude node 0000.0000.0156
                       flex-algo algorithm ADMIN (130)
                         metric type TE
         Request sequence number: 1
         Response sequence number: 1
         Number of times path updated: 1
         Last updated: 2:38:45 ago
         ID: 0x15
         Path: Path not found

   Destination: Juniper-175-ACX7100-48L
      Path constraint: exclude Ethernet13
                       flex-algo algorithm MIN-LATENCY (128)
                         metric type TE
         Request sequence number: 1
         Response sequence number: 1
         Number of times path updated: 2
         Last updated: 0:08:00 ago
         ID: 0xe
         Path:
            Juniper-156-PTX10002-36QDD [P-node]
            Juniper-175-ACX7100-48L [Q-node]
      Path constraint: exclude node 0000.0000.0053
                       flex-algo algorithm MIN-LATENCY (128)
                         metric type TE
         Request sequence number: 1
         Response sequence number: 1
         Number of times path updated: 3
         Last updated: 0:04:00 ago
         ID: 0xf
         Path:
            Juniper-156-PTX10002-36QDD [P-node]
            Juniper-175-ACX7100-48L [Q-node]
      Path constraint: exclude Ethernet4
                       flex-algo algorithm ADMIN (130)
                         metric type TE
         Request sequence number: 1
         Response sequence number: 1
         Number of times path updated: 1
         Last updated: 0:10:42 ago
         ID: 0x1c
         Path: Path not found
      Path constraint: exclude node 0100.0000.0217
                       flex-algo algorithm ADMIN (130)
                         metric type TE
         Request sequence number: 1
         Response sequence number: 1
         Number of times path updated: 1
         Last updated: 0:10:42 ago
         ID: 0x1d
         Path: Path not found

```

## show isis ti-lfa tunnel

```text
Tunnel Index 0
   via 20.30.217.217, 'Ethernet4'
      label stack 3
   backup via 20.30.179.179, 'Ethernet40'
      label stack 3
Tunnel Index 1
   via fe80::5e07:58ff:fea3:aaa, 'Ethernet13'
      label stack 21703
   backup via fe80::d248:a1ff:feba:3c61, 'Ethernet11'
      label stack 19
Tunnel Index 2
   via 20.30.84.84, 'Ethernet12'
      label stack 3
   backup via 20.30.179.179, 'Ethernet40'
      label stack 3
Tunnel Index 3
   via 20.30.131.131, 'Ethernet35'
      label stack 3
   backup via 20.30.179.179, 'Ethernet40'
      label stack 20131
Tunnel Index 4
   via 20.30.72.72, 'Ethernet9'
      label stack 3
   backup via 20.30.179.179, 'Ethernet40'
      label stack 20072
Tunnel Index 5
   via fe80::d248:a1ff:feba:3c61, 'Ethernet11'
      label stack 3
   backup via fe80::5e07:58ff:fea3:aaa, 'Ethernet13'
      label stack 21685
Tunnel Index 6
   via 20.30.221.221, 'Ethernet15'
      label stack 3
   backup via 20.30.179.179, 'Ethernet40'
      label stack 20221
Tunnel Index 7
   via 20.30.72.72, 'Ethernet9'
      label stack 3
   backup via 21.30.156.156, 'Ethernet21'
      label stack 21201
Tunnel Index 8
   via fe80::d248:a1ff:feba:3c61, 'Ethernet11'
      label stack 3
   backup via fe80::5a70:7fff:fe9f:c403, 'Ethernet12'
      label stack 20575 20556
Tunnel Index 10
   via fe80::5e07:58ff:fea3:aaa, 'Ethernet13'
      label stack 2
   backup via fe80::5a70:7fff:fe9f:c403, 'Ethernet12'
      label stack 20575 20453
Tunnel Index 11
   via 20.30.32.32, 'Ethernet2'
      label stack 3
   backup via 20.30.179.179, 'Ethernet40'
      label stack 20032
Tunnel Index 12
   via fe80::d248:a1ff:feba:3c61, 'Ethernet11'
      label stack 3
   backup via fe80::5e07:58ff:fea3:aaa, 'Ethernet13'
      label stack 21703 21684
Tunnel Index 13
   via 20.30.32.32, 'Ethernet2'
      label stack 3
   backup via 20.30.221.221, 'Ethernet15'
      label stack 721303 20161
Tunnel Index 14
   via 20.30.221.221, 'Ethernet15'
      label stack 3
   backup via 20.30.53.53, 'Ethernet13'
      label stack 21303 21349
Tunnel Index 15
   via 20.30.221.221, 'Ethernet15'
      label stack 721248
   backup via 20.30.53.53, 'Ethernet13'
      label stack 21248
Tunnel Index 16
   via 20.30.221.221, 'Ethernet15'
      label stack 721303
   backup via 20.30.53.53, 'Ethernet13'
      label stack 21303
Tunnel Index 17
   via 20.30.53.53, 'Ethernet13'
      label stack 0
   backup via 20.30.179.179, 'Ethernet40'
      label stack 20053
Tunnel Index 18
   via 20.30.66.66, 'Ethernet31'
      label stack 3
   backup via 20.30.179.179, 'Ethernet40'
      label stack 20066
Tunnel Index 19
   via 20.30.217.217, 'Ethernet4'
      label stack 3
   backup via 20.30.221.221, 'Ethernet15'
      label stack 721303
Tunnel Index 20
   via 20.30.66.66, 'Ethernet31'
      label stack 3
   backup via 20.30.179.179, 'Ethernet40'
      label stack 21195
Tunnel Index 21
   via 20.30.179.179, 'Ethernet40'
      label stack 3
   backup via 21.30.156.156, 'Ethernet21'
      label stack 21308
Tunnel Index 22
   via 20.30.221.221, 'Ethernet15'
      label stack 3
   backup via 20.30.179.179, 'Ethernet40'
      label stack 21350
Tunnel Index 23
   via 20.30.53.53, 'Ethernet13'
      label stack 3
   backup via 20.30.221.221, 'Ethernet15'
      label stack 721182
Tunnel Index 24
   via 20.30.53.53, 'Ethernet13'
      label stack 3
   backup via 20.30.221.221, 'Ethernet15'
      label stack 721303 21181
Tunnel Index 25
   via 20.30.32.32, 'Ethernet2'
      label stack 3
   backup via 20.30.217.217, 'Ethernet4'
      label stack 20162
Tunnel Index 26
   via 20.30.179.179, 'Ethernet40'
      label stack 3
   backup via 20.30.221.221, 'Ethernet15'
      label stack 721303 21307
Tunnel Index 39
   via fe80::5e07:58ff:fea3:aaa, 'Ethernet13'
      label stack 3
   backup via fe80::d248:a1ff:feba:3c61, 'Ethernet11'
      label stack 21582
Tunnel Index 40
   via fe80::5e07:58ff:fea3:aaa, 'Ethernet13'
      label stack 3
   backup via fe80::d248:a1ff:feba:3c61, 'Ethernet11'
      label stack 19 21581
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
 I L2     10.0.0.32/32 [115/1]
           via 20.30.32.32, Ethernet2
 I L2     10.0.0.53/32 [115/1]
           via 20.30.53.53, Ethernet13
 I L2     10.0.0.66/32 [115/11]
           via 20.30.66.66, Ethernet31
 I L2     10.0.0.72/32 [115/11]
           via 20.30.72.72, Ethernet9
 I L2     10.0.0.84/32 [115/11]
           via 20.30.84.84, Ethernet12
 I L2     10.0.0.120/32 [115/1]
           via 20.30.120.120, Ethernet3
           via 21.30.120.120, Ethernet10
 I L2     10.0.0.124/32 [115/1]
           via 20.30.124.124, Ethernet17
           via 21.30.124.124, Ethernet18
 I L2     10.0.0.128/32 [115/1]
           via 21.30.128.128, Ethernet20
 I L2     10.0.0.131/32 [115/1]
           via 20.30.131.131, Ethernet35
 I L2     10.0.0.156/32 [115/1]
           via 20.30.156.156, Ethernet11
           via 21.30.156.156, Ethernet21
 I L2     10.0.0.175/32 [115/11]
           via 20.30.32.32, Ethernet2
           via 20.30.120.120, Ethernet3
           via 20.30.72.72, Ethernet9
           via 20.30.84.84, Ethernet12
           via 20.30.53.53, Ethernet13
           via 20.30.124.124, Ethernet17
           via 20.30.66.66, Ethernet31
           via 20.30.131.131, Ethernet35
 I L2     10.0.0.179/32 [115/1]
           via 20.30.179.179, Ethernet40
 I L2     10.0.0.214/32 [115/1]
           via 20.30.214.214, Ethernet5
           via 21.30.214.214, Ethernet6
 I L2     10.0.0.216/32 [115/11]
           via 20.30.214.214, Ethernet5
           via 21.30.214.214, Ethernet6
 I L2     10.0.0.217/32 [115/1]
           via 20.30.217.217, Ethernet4
 I L2     10.0.0.221/32 [115/1]
           via 20.30.221.221, Ethernet15
 I L2     10.0.1.179/32 [115/1]
           via 20.30.179.179, Ethernet40
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
 I L2     20.32.175.0/24 [115/11]
           via 20.30.32.32, Ethernet2
 I L2     20.53.175.0/24 [115/11]
           via 20.30.53.53, Ethernet13
 I L2     20.66.175.0/24 [115/11]
           via 20.30.66.66, Ethernet31
 I L2     20.72.175.0/24 [115/11]
           via 20.30.72.72, Ethernet9
 I L2     20.84.175.0/24 [115/21]
           via 20.30.32.32, Ethernet2
           via 20.30.120.120, Ethernet3
           via 20.30.72.72, Ethernet9
           via 20.30.84.84, Ethernet12
           via 20.30.53.53, Ethernet13
           via 20.30.124.124, Ethernet17
           via 20.30.66.66, Ethernet31
           via 20.30.131.131, Ethernet35
 I L2     20.120.175.0/24 [115/11]
           via 20.30.120.120, Ethernet3
           via 21.30.120.120, Ethernet10
 I L2     20.120.214.0/24 [115/11]
           via 20.30.120.120, Ethernet3
           via 21.30.120.120, Ethernet10
 I L2     20.120.217.0/24 [115/1]
           via 20.30.120.120, Ethernet3
           via 21.30.120.120, Ethernet10
 I L2     20.124.175.0/24 [115/11]
           via 20.30.124.124, Ethernet17
           via 21.30.124.124, Ethernet18
 I L2     20.128.175.0/24 [115/11]
           via 21.30.128.128, Ethernet20
 I L2     20.131.175.0/24 [115/11]
           via 20.30.131.131, Ethernet35
 I L2     20.156.175.0/24 [115/11]
           via 20.30.156.156, Ethernet11
           via 21.30.156.156, Ethernet21
 I L2     20.175.179.0/24 [115/11]
           via 20.30.179.179, Ethernet40
 I L2     20.175.184.0/24 [115/21]
           via 20.30.32.32, Ethernet2
           via 20.30.120.120, Ethernet3
           via 20.30.72.72, Ethernet9
           via 20.30.84.84, Ethernet12
           via 20.30.53.53, Ethernet13
           via 20.30.124.124, Ethernet17
           via 20.30.66.66, Ethernet31
           via 20.30.131.131, Ethernet35
 I L2     20.175.214.0/24 [115/21]
           via 20.30.32.32, Ethernet2
           via 20.30.120.120, Ethernet3
           via 20.30.72.72, Ethernet9
           via 20.30.84.84, Ethernet12
           via 20.30.53.53, Ethernet13
           via 20.30.124.124, Ethernet17
           via 20.30.66.66, Ethernet31
           via 20.30.131.131, Ethernet35
 I L2     20.175.217.0/24 [115/11]
           via 20.30.217.217, Ethernet4
 I L2     20.175.221.0/24 [115/11]
           via 20.30.221.221, Ethernet15
 I L2     20.214.216.0/24 [115/11]
           via 20.30.214.214, Ethernet5
           via 21.30.214.214, Ethernet6
 C        21.30.120.0/24
           directly connected, Ethernet10
 C        21.30.124.0/24
           directly connected, Ethernet18
 C        21.30.128.0/24
           directly connected, Ethernet20
 C        21.30.156.0/24
           directly connected, Ethernet21
 C        21.30.214.0/24
           directly connected, Ethernet6
 C        21.30.217.0/24
           directly connected, Ethernet8
 I L2     192.168.20.0/23 [115/1]
           via 20.30.120.120, Ethernet3
           via 21.30.120.120, Ethernet10

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
           via 10.0.0.32/32, IS-IS SR tunnel index 20, label 378528
              via TI-LFA tunnel index 11, label imp-null(3)
                 via 20.30.32.32, Ethernet2, label imp-null(3)
                 backup via 20.30.179.179, Ethernet40, label 20032
 B I      50.10.53.0/24 [200/0]
           via 10.0.0.53/32, IS-IS SR tunnel index 10, label 970000
              via TI-LFA tunnel index 17, label imp-null(3)
                 via 20.30.53.53, Ethernet13, label exp-null-v4(0)
                 backup via 20.30.179.179, Ethernet40, label 20053
 B I      50.10.66.0/24 [200/0]
           via 10.0.0.66/32, IS-IS SR tunnel index 13, label 62000
              via TI-LFA tunnel index 18, label imp-null(3)
                 via 20.30.66.66, Ethernet31, label imp-null(3)
                 backup via 20.30.179.179, Ethernet40, label 20066
 B I      50.10.72.0/24 [200/0]
           via 10.0.0.72/32, IS-IS SR tunnel index 14, label 62000
              via TI-LFA tunnel index 4, label imp-null(3)
                 via 20.30.72.72, Ethernet9, label imp-null(3)
                 backup via 20.30.179.179, Ethernet40, label 20072
 B I      50.10.84.0/24 [200/0]
           via 10.0.0.84/32, IS-IS SR tunnel index 8, label 720898
              via TI-LFA tunnel index 2, label 20084
                 via 20.30.84.84, Ethernet12, label imp-null(3)
                 backup via 20.30.179.179, Ethernet40, label imp-null(3)
 B I      50.10.120.0/24 [200/0]
           via 10.0.0.120/32, IS-IS SR tunnel index 17, label 1657
              via 20.30.120.120, Ethernet3, label imp-null(3)
              via 21.30.120.120, Ethernet10, label imp-null(3)
 B I      50.10.131.0/24 [200/0]
           via 10.0.0.131/32, IS-IS SR tunnel index 9, label 18
              via TI-LFA tunnel index 3, label imp-null(3)
                 via 20.30.131.131, Ethernet35, label imp-null(3)
                 backup via 20.30.179.179, Ethernet40, label 20131
 B I      50.10.156.0/24 [200/0]
           via 10.0.0.156/32, IS-IS SR tunnel index 11, label 16
              via 20.30.156.156, Ethernet11, label imp-null(3)
              via 21.30.156.156, Ethernet21, label imp-null(3)
 B I      50.10.179.0/24 [200/0]
           via 10.0.0.179/32, IS-IS SR tunnel index 12, label 16
              via 20.30.179.179, Ethernet40, label imp-null(3)
 B I      50.10.214.0/24 [200/0]
           via 10.0.0.214/32, IS-IS SR tunnel index 21, label 500000
              via 20.30.214.214, Ethernet5, label 20214
              via 21.30.214.214, Ethernet6, label 20214
 B I      50.10.217.0/24 [200/0]
           via 10.0.0.217/32, IS-IS SR tunnel index 16, label 524287
              via TI-LFA tunnel index 0, label 20217
                 via 20.30.217.217, Ethernet4, label imp-null(3)
                 backup via 20.30.179.179, Ethernet40, label imp-null(3)
 B I      50.10.221.0/24 [200/0]
           via 10.0.0.221/32, IS-IS SR tunnel index 15, label 524292
              via TI-LFA tunnel index 6, label imp-null(3)
                 via 20.30.221.221, Ethernet15, label imp-null(3)
                 backup via 20.30.179.179, Ethernet40, label 20221
 B I      50.129.66.0/24 [200/0]
           via 10.0.0.66/32, IS-IS SR tunnel index 13, label 62000
              via TI-LFA tunnel index 18, label imp-null(3)
                 via 20.30.66.66, Ethernet31, label imp-null(3)
                 backup via 20.30.179.179, Ethernet40, label 20066
 B I      50.129.72.0/24 [200/0]
           via 10.0.0.72/32, IS-IS SR tunnel index 14, label 62000
              via TI-LFA tunnel index 4, label imp-null(3)
                 via 20.30.72.72, Ethernet9, label imp-null(3)
                 backup via 20.30.179.179, Ethernet40, label 20072

```

## show mpls route

```text
MPLS forwarding table (Label [metric] Vias) - 77 routes 
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
                  via TI-LFA tunnel index 11
                    via 20.30.32.32, Ethernet2, label imp-null(3)
                    backup via 20.30.179.179, Ethernet40, label 20032
 20053   A[1]
                via M, ::, pop
                    EgressACL: apply
                  via TI-LFA tunnel index 17
                    via 20.30.53.53, Ethernet13, label exp-null-v4(0)
                    backup via 20.30.179.179, Ethernet40, label 20053
 20066   A[1]
                via M, ::, pop
                    EgressACL: apply
                  via TI-LFA tunnel index 18
                    via 20.30.66.66, Ethernet31, label imp-null(3)
                    backup via 20.30.179.179, Ethernet40, label 20066
 20072   A[1]
                via M, ::, pop
                    EgressACL: apply
                  via TI-LFA tunnel index 4
                    via 20.30.72.72, Ethernet9, label imp-null(3)
                    backup via 20.30.179.179, Ethernet40, label 20072
 20084   A[1]
                via M, ::, forward
                    EgressACL: apply
                  via TI-LFA tunnel index 2
                    via 20.30.84.84, Ethernet12, label imp-null(3)
                    backup via 20.30.179.179, Ethernet40, label imp-null(3)
 20120   A[1]
                via M, pop
                    EgressACL: apply
                    20.30.120.120 Ethernet3
                    21.30.120.120 Ethernet10
 20131   A[1]
                via M, ::, pop
                    EgressACL: apply
                  via TI-LFA tunnel index 3
                    via 20.30.131.131, Ethernet35, label imp-null(3)
                    backup via 20.30.179.179, Ethernet40, label 20131
 20156   A[1]
                via M, pop
                    EgressACL: apply
                    20.30.156.156 Ethernet11
                    21.30.156.156 Ethernet21
 20161   A[1]
                via M, ::, pop
                    EgressACL: apply
                  via TI-LFA tunnel index 13
                    via 20.30.32.32, Ethernet2, label imp-null(3)
                    backup via 20.30.221.221, Ethernet15, label 721303 20161
 20162   A[1]
                via M, ::, pop
                    EgressACL: apply
                  via TI-LFA tunnel index 25
                    via 20.30.32.32, Ethernet2, label imp-null(3)
                    backup via 20.30.217.217, Ethernet4, label 20162
 20163   A[1]
                via M, pop
                    EgressACL: apply
                    20.30.32.32 Ethernet2
 20175   A[1]
                via M, 20.30.32.32, swap 20175
                    EgressACL: apply
                    directly connected, Ethernet2
                    d4:af:f7:2f:13:96, vlan 1018
                via M, 20.30.53.53, swap 20175
                    EgressACL: apply
                    directly connected, Ethernet13
                    5c:07:58:a3:0a:aa, vlan 1026
                via M, 20.30.66.66, swap 20175
                    EgressACL: apply
                    directly connected, Ethernet31
                    e4:6d:7f:e3:c8:0a, vlan 1020
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
 20214   A[1]
                via M, forward
                    EgressACL: apply
                    20.30.214.214 Ethernet5
                    21.30.214.214 Ethernet6
 20217   A[1]
                via M, ::, forward
                    EgressACL: apply
                  via TI-LFA tunnel index 0
                    via 20.30.217.217, Ethernet4, label imp-null(3)
                    backup via 20.30.179.179, Ethernet40, label imp-null(3)
 20221   A[1]
                via M, ::, pop
                    EgressACL: apply
                  via TI-LFA tunnel index 6
                    via 20.30.221.221, Ethernet15, label imp-null(3)
                    backup via 20.30.179.179, Ethernet40, label 20221
 20453   A[1]
                via M, ::, pop
                    EgressACL: apply
                  via TI-LFA tunnel index 10
                    via fe80::5e07:58ff:fea3:aaa, Ethernet13, label exp-null-v6(2)
                    backup via fe80::5a70:7fff:fe9f:c403, Ethernet12, label 20575 20453
 20520   A[1]
                via M, pop
                    EgressACL: apply
                    fe80::be31:e2ff:fee1:ec2c Ethernet3
 20556   A[1]
                via M, ::, pop
                    EgressACL: apply
                  via TI-LFA tunnel index 8
                    via fe80::d248:a1ff:feba:3c61, Ethernet11, label imp-null(3)
                    backup via fe80::5a70:7fff:fe9f:c403, Ethernet12, label 20575 20556
 20575   A[1]
                via M, forward
                    EgressACL: apply
                    fe80::5e07:58ff:fea3:aaa Ethernet13
                    fe80::d248:a1ff:feba:3c61 Ethernet11
                    fe80::c214:b8ff:fe21:9790 Ethernet4
                    fe80::5a70:7fff:fe9f:c403 Ethernet12
                    fe80::d6af:f7ff:fe2f:1396 Ethernet2
                    fe80::be31:e2ff:fee1:ec2c Ethernet3
 21181   A[1]
                via M, ::, pop
                    EgressACL: apply
                  via TI-LFA tunnel index 24
                    via 20.30.53.53, Ethernet13, label imp-null(3)
                    backup via 20.30.221.221, Ethernet15, label 721303 21181
 21182   A[1]
                via M, ::, pop
                    EgressACL: apply
                  via TI-LFA tunnel index 23
                    via 20.30.53.53, Ethernet13, label imp-null(3)
                    backup via 20.30.221.221, Ethernet15, label 721182
 21183   A[1]
                via M, pop
                    EgressACL: apply
                    20.30.53.53 Ethernet13
 21195   A[1]
                via M, ::, pop
                    EgressACL: apply
                  via TI-LFA tunnel index 20
                    via 20.30.66.66, Ethernet31, label imp-null(3)
                    backup via 20.30.179.179, Ethernet40, label 21195
 21201   A[1]
                via M, ::, pop
                    EgressACL: apply
                  via TI-LFA tunnel index 7
                    via 20.30.72.72, Ethernet9, label imp-null(3)
                    backup via 21.30.156.156, Ethernet21, label 21201
 21248   A[1]
                via M, ::, pop
                    EgressACL: apply
                  via TI-LFA tunnel index 15
                    via 20.30.221.221, Ethernet15, label 721248
                    backup via 20.30.53.53, Ethernet13, label 21248
 21249   A[1]
                via M, 20.30.32.32, swap 21249
                    EgressACL: apply
                    directly connected, Ethernet2
                    d4:af:f7:2f:13:96, vlan 1018
                via M, 20.30.53.53, swap 21249
                    EgressACL: apply
                    directly connected, Ethernet13
                    5c:07:58:a3:0a:aa, vlan 1026
                via M, 20.30.156.156, swap 21249
                    EgressACL: apply
                    directly connected, Ethernet11
                    d0:48:a1:ba:3c:61, vlan 1019
                via M, 20.30.179.179, swap 21249
                    EgressACL: apply
                    directly connected, Ethernet40
                    e8:24:a6:96:05:48, vlan 1015
                via M, 20.30.217.217, swap 21249
                    EgressACL: apply
                    directly connected, Ethernet4
                    c0:14:b8:21:97:90, vlan 1007
                via M, 20.30.221.221, swap 721249
                    EgressACL: apply
                    directly connected, Ethernet15
                    30:c5:07:84:3e:79, vlan 1006
                via M, 21.30.156.156, swap 21249
                    EgressACL: apply
                    directly connected, Ethernet21
                    d0:48:a1:ba:3c:63, vlan 1027
 21284   A[1]
                via M, pop
                    EgressACL: apply
                    20.30.156.156 Ethernet11
                    21.30.156.156 Ethernet21
 21285   A[1]
                via M, pop
                    EgressACL: apply
                    20.30.156.156 Ethernet11
                    21.30.156.156 Ethernet21
 21286   A[1]
                via M, pop
                    EgressACL: apply
                    20.30.156.156 Ethernet11
                    21.30.156.156 Ethernet21
 21303   A[1]
                via M, ::, pop
                    EgressACL: apply
                  via TI-LFA tunnel index 16
                    via 20.30.221.221, Ethernet15, label 721303
                    backup via 20.30.53.53, Ethernet13, label 21303
 21304   A[1]
                via M, 20.30.32.32, swap 21304
                    EgressACL: apply
                    directly connected, Ethernet2
                    d4:af:f7:2f:13:96, vlan 1018
                via M, 20.30.53.53, swap 21304
                    EgressACL: apply
                    directly connected, Ethernet13
                    5c:07:58:a3:0a:aa, vlan 1026
                via M, 20.30.156.156, swap 21304
                    EgressACL: apply
                    directly connected, Ethernet11
                    d0:48:a1:ba:3c:61, vlan 1019
                via M, 20.30.179.179, swap 21304
                    EgressACL: apply
                    directly connected, Ethernet40
                    e8:24:a6:96:05:48, vlan 1015
                via M, 20.30.217.217, swap 21304
                    EgressACL: apply
                    directly connected, Ethernet4
                    c0:14:b8:21:97:90, vlan 1007
                via M, 20.30.221.221, swap 721304
                    EgressACL: apply
                    directly connected, Ethernet15
                    30:c5:07:84:3e:79, vlan 1006
                via M, 21.30.156.156, swap 21304
                    EgressACL: apply
                    directly connected, Ethernet21
                    d0:48:a1:ba:3c:63, vlan 1027
 21305   A[1]
                via M, forward
                    EgressACL: apply
                    20.30.131.131 Ethernet35
 21307   A[1]
                via M, ::, pop
                    EgressACL: apply
                  via TI-LFA tunnel index 26
                    via 20.30.179.179, Ethernet40, label imp-null(3)
                    backup via 20.30.221.221, Ethernet15, label 721303 21307
 21308   A[1]
                via M, ::, pop
                    EgressACL: apply
                  via TI-LFA tunnel index 21
                    via 20.30.179.179, Ethernet40, label imp-null(3)
                    backup via 21.30.156.156, Ethernet21, label 21308
 21309   A[1]
                via M, pop
                    EgressACL: apply
                    20.30.179.179 Ethernet40
 21345   A[1]
                via M, ::, forward
                    EgressACL: apply
                  via TI-LFA tunnel index 19
                    via 20.30.217.217, Ethernet4, label imp-null(3)
                    backup via 20.30.221.221, Ethernet15, label 721303
 21346   A[1]
                via M, ::, forward
                    EgressACL: apply
                  via TI-LFA tunnel index 0
                    via 20.30.217.217, Ethernet4, label imp-null(3)
                    backup via 20.30.179.179, Ethernet40, label imp-null(3)
 21347   A[1]
                via M, forward
                    EgressACL: apply
                    20.30.217.217 Ethernet4
 21349   A[1]
                via M, ::, pop
                    EgressACL: apply
                  via TI-LFA tunnel index 14
                    via 20.30.221.221, Ethernet15, label imp-null(3)
                    backup via 20.30.53.53, Ethernet13, label 21303 21349
 21350   A[1]
                via M, ::, pop
                    EgressACL: apply
                  via TI-LFA tunnel index 22
                    via 20.30.221.221, Ethernet15, label imp-null(3)
                    backup via 20.30.179.179, Ethernet40, label 21350
 21581   A[1]
                via M, ::, pop
                    EgressACL: apply
                  via TI-LFA tunnel index 40
                    via fe80::5e07:58ff:fea3:aaa, Ethernet13, label imp-null(3)
                    backup via fe80::d248:a1ff:feba:3c61, Ethernet11, label 19 21581
 21582   A[1]
                via M, ::, pop
                    EgressACL: apply
                  via TI-LFA tunnel index 39
                    via fe80::5e07:58ff:fea3:aaa, Ethernet13, label imp-null(3)
                    backup via fe80::d248:a1ff:feba:3c61, Ethernet11, label 21582
 21583   A[1]
                via M, pop
                    EgressACL: apply
                    fe80::5e07:58ff:fea3:aaa Ethernet13
 21648   A[1]
                via M, pop
                    EgressACL: apply
                    fe80::be31:e2ff:fee1:ec2c Ethernet3
 21649   A[1]
                via M, pop
                    EgressACL: apply
                    fe80::be31:e2ff:fee1:ec2c Ethernet3
 21650   A[1]
                via M, pop
                    EgressACL: apply
                    fe80::be31:e2ff:fee1:ec2c Ethernet3
 21684   A[1]
                via M, ::, pop
                    EgressACL: apply
                  via TI-LFA tunnel index 12
                    via fe80::d248:a1ff:feba:3c61, Ethernet11, label imp-null(3)
                    backup via fe80::5e07:58ff:fea3:aaa, Ethernet13, label 21703 21684
 21685   A[1]
                via M, ::, pop
                    EgressACL: apply
                  via TI-LFA tunnel index 5
                    via fe80::d248:a1ff:feba:3c61, Ethernet11, label imp-null(3)
                    backup via fe80::5e07:58ff:fea3:aaa, Ethernet13, label 21685
 21686   A[1]
                via M, pop
                    EgressACL: apply
                    fe80::d248:a1ff:feba:3c61 Ethernet11
 21703   A[1]
                via M, ::, pop
                    EgressACL: apply
                  via TI-LFA tunnel index 1
                    via fe80::5e07:58ff:fea3:aaa, Ethernet13, label 21703
                    backup via fe80::d248:a1ff:feba:3c61, Ethernet11, label 19
 21704   A[1]
                via M, forward
                    EgressACL: apply
                    fe80::5e07:58ff:fea3:aaa Ethernet13
                    fe80::d248:a1ff:feba:3c61 Ethernet11
                    fe80::d6af:f7ff:fe2f:1396 Ethernet2
 21705   A[1]
                via M, forward
                    EgressACL: apply
                    fe80::c214:b8ff:fe21:9790 Ethernet4
 362144   [0]
                via I, ipv4, vrf FLEXALGO
 362145   [0]
                via I, ipv4, vrf RED
 362146   [0]
                via I, ipv6, vrf RED
 378528  A[1]
                via M, 20.30.53.53, pop
                    EgressACL: apply
                    directly connected, Ethernet13
                    5c:07:58:a3:0a:aa, vlan 1026
 378529  A[1]
                via M, fe80::5e07:58ff:fea3:aaa, pop
                    EgressACL: apply
                    directly connected, Ethernet13
                    5c:07:58:a3:0a:aa, vlan 1026
 378533  A[1]
                via M, 20.30.131.131, pop
                    EgressACL: apply
                    directly connected, Ethernet35
                    40:a6:b7:94:34:cb, vlan 1012
 378538  A[1]
                via M, 20.30.179.179, pop
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
 378553  A[1]
                via M, 20.30.214.214, pop
                    EgressACL: apply
                    directly connected, Ethernet5
                    18:5b:00:61:ac:6f, vlan 1008
 378562  A[1]
                via M, 21.30.214.214, pop
                    EgressACL: apply
                    directly connected, Ethernet6
                    18:5b:00:61:ac:73, vlan 1022
 378574  A[1]
                via M, 21.30.156.156, pop
                    EgressACL: apply
                    directly connected, Ethernet21
                    d0:48:a1:ba:3c:63, vlan 1027
 378577  A[1]
                via M, 20.30.72.72, pop
                    EgressACL: apply
                    directly connected, Ethernet9
                    e0:9b:27:c4:c5:84, vlan 1009
 378578  A[1]
                via M, 20.30.66.66, pop
                    EgressACL: apply
                    directly connected, Ethernet31
                    e4:6d:7f:e3:c8:0a, vlan 1020
 378582  A[1]
                via M, 20.30.217.217, pop
                    EgressACL: apply
                    directly connected, Ethernet4
                    c0:14:b8:21:97:90, vlan 1007
 378583  A[1]
                via M, fe80::c214:b8ff:fe21:9790, pop
                    EgressACL: apply
                    directly connected, Ethernet4
                    c0:14:b8:21:97:90, vlan 1007
 378586  A[1]
                via M, 20.30.84.84, pop
                    EgressACL: apply
                    directly connected, Ethernet12
                    58:70:7f:9f:c4:03, vlan 1014
 378587  A[1]
                via M, fe80::5a70:7fff:fe9f:c403, pop
                    EgressACL: apply
                    directly connected, Ethernet12
                    58:70:7f:9f:c4:03, vlan 1014
 378588  A[1]
                via M, 20.30.32.32, pop
                    EgressACL: apply
                    directly connected, Ethernet2
                    d4:af:f7:2f:13:96, vlan 1018
 378589  A[1]
                via M, fe80::d6af:f7ff:fe2f:1396, pop
                    EgressACL: apply
                    directly connected, Ethernet2
                    d4:af:f7:2f:13:96, vlan 1018
 378590  A[1]
                via M, 21.30.120.120, pop
                    EgressACL: apply
                    directly connected, Ethernet10
                    bc:31:e2:e1:ec:32, vlan 1029
 378597  A[1]
                via M, 20.30.120.120, pop
                    EgressACL: apply
                    directly connected, Ethernet3
                    bc:31:e2:e1:ec:2c, vlan 1017
 378598  A[1]
                via M, fe80::be31:e2ff:fee1:ec2c, pop
                    EgressACL: apply
                    directly connected, Ethernet3
                    bc:31:e2:e1:ec:2c, vlan 1017
```

## show mpls lfib route

```text
MPLS forwarding table (Label [metric] Vias) - 77 routes 
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
                via TI-LFA tunnel index 11, pop
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                    via 20.30.32.32, Ethernet2, label imp-null(3)
                    backup via 20.30.179.179, Ethernet40, label 20032
 IP    20053    [1], 10.0.0.53/32
                via TI-LFA tunnel index 17, pop
                 payload autoDecide, ttlMode uniform, apply egress-acl
                    via 20.30.53.53, Ethernet13, label exp-null-v4(0)
                    backup via 20.30.179.179, Ethernet40, label 20053
 IP    20066    [1], 10.0.0.66/32
                via TI-LFA tunnel index 18, pop
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                    via 20.30.66.66, Ethernet31, label imp-null(3)
                    backup via 20.30.179.179, Ethernet40, label 20066
 IP    20072    [1], 10.0.0.72/32
                via TI-LFA tunnel index 4, pop
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                    via 20.30.72.72, Ethernet9, label imp-null(3)
                    backup via 20.30.179.179, Ethernet40, label 20072
 IP    20084    [1], 10.0.0.84/32
                via TI-LFA tunnel index 2, forward
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                    via 20.30.84.84, Ethernet12, label imp-null(3)
                    backup via 20.30.179.179, Ethernet40, label imp-null(3)
 IP    20120    [1], 10.0.0.120/32
                via M, 20.30.120.120, pop
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                 interface Ethernet3
                via M, 21.30.120.120, pop
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                 interface Ethernet10
 IP    20131    [1], 10.0.0.131/32
                via TI-LFA tunnel index 3, pop
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                    via 20.30.131.131, Ethernet35, label imp-null(3)
                    backup via 20.30.179.179, Ethernet40, label 20131
 IP    20156    [1], 10.0.0.156/32
                via M, 20.30.156.156, pop
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                 interface Ethernet11
                via M, 21.30.156.156, pop
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                 interface Ethernet21
 IP    20161    [1], 10.0.0.32/32, algorithm MIN-LATENCY
                via TI-LFA tunnel index 13, pop
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                    via 20.30.32.32, Ethernet2, label imp-null(3)
                    backup via 20.30.221.221, Ethernet15, label 721303 20161
 IP    20162    [1], 10.0.0.32/32, algorithm MIN-TE
                via TI-LFA tunnel index 25, pop
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                    via 20.30.32.32, Ethernet2, label imp-null(3)
                    backup via 20.30.217.217, Ethernet4, label 20162
 IP    20163    [1], 10.0.0.32/32, algorithm ADMIN
                via M, 20.30.32.32, pop
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                 interface Ethernet2
 IP    20175    [1], 10.0.0.175/32
                via M, 20.30.32.32, swap 20175
                 payload autoDecide, ttlMode uniform, apply egress-acl
                 interface Ethernet2
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
 IP    20214    [1], 10.0.0.214/32
                via M, 20.30.214.214, forward
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                 interface Ethernet5
                via M, 21.30.214.214, forward
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                 interface Ethernet6
 IP    20217    [1], 10.0.0.217/32
                via TI-LFA tunnel index 0, forward
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                    via 20.30.217.217, Ethernet4, label imp-null(3)
                    backup via 20.30.179.179, Ethernet40, label imp-null(3)
 IP    20221    [1], 10.0.0.221/32
                via TI-LFA tunnel index 6, pop
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                    via 20.30.221.221, Ethernet15, label imp-null(3)
                    backup via 20.30.179.179, Ethernet40, label 20221
 IP    20453    [1], 2002::53/128
                via TI-LFA tunnel index 10, pop
                 payload autoDecide, ttlMode uniform, apply egress-acl
                    via fe80::5e07:58ff:fea3:aaa, Ethernet13, label exp-null-v6(2)
                    backup via fe80::5a70:7fff:fe9f:c403, Ethernet12, label 20575 20453
 IP    20520    [1], 2002::120/128
                via M, fe80::be31:e2ff:fee1:ec2c, pop
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                 interface Ethernet3
 IP    20556    [1], 2002::156/128
                via TI-LFA tunnel index 8, pop
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                    via fe80::d248:a1ff:feba:3c61, Ethernet11, label imp-null(3)
                    backup via fe80::5a70:7fff:fe9f:c403, Ethernet12, label 20575 20556
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
                via M, fe80::d6af:f7ff:fe2f:1396, forward
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                 interface Ethernet2
 IP    21181    [1], 10.0.0.53/32, algorithm MIN-LATENCY
                via TI-LFA tunnel index 24, pop
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                    via 20.30.53.53, Ethernet13, label imp-null(3)
                    backup via 20.30.221.221, Ethernet15, label 721303 21181
 IP    21182    [1], 10.0.0.53/32, algorithm MIN-TE
                via TI-LFA tunnel index 23, pop
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                    via 20.30.53.53, Ethernet13, label imp-null(3)
                    backup via 20.30.221.221, Ethernet15, label 721182
 IP    21183    [1], 10.0.0.53/32, algorithm ADMIN
                via M, 20.30.53.53, pop
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                 interface Ethernet13
 IP    21195    [1], 10.0.0.66/32, algorithm MIN-TE
                via TI-LFA tunnel index 20, pop
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                    via 20.30.66.66, Ethernet31, label imp-null(3)
                    backup via 20.30.179.179, Ethernet40, label 21195
 IP    21201    [1], 10.0.0.72/32, algorithm MIN-TE
                via TI-LFA tunnel index 7, pop
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                    via 20.30.72.72, Ethernet9, label imp-null(3)
                    backup via 21.30.156.156, Ethernet21, label 21201
 IP    21248    [1], 10.0.0.120/32, algorithm MIN-LATENCY
                via TI-LFA tunnel index 15, pop
                 payload autoDecide, ttlMode uniform, apply egress-acl
                    via 20.30.221.221, Ethernet15, label 721248
                    backup via 20.30.53.53, Ethernet13, label 21248
 IP    21249    [1], 10.0.0.120/32, algorithm MIN-TE
                via M, 20.30.32.32, swap 21249
                 payload autoDecide, ttlMode uniform, apply egress-acl
                 interface Ethernet2
                via M, 20.30.53.53, swap 21249
                 payload autoDecide, ttlMode uniform, apply egress-acl
                 interface Ethernet13
                via M, 20.30.156.156, swap 21249
                 payload autoDecide, ttlMode uniform, apply egress-acl
                 interface Ethernet11
                via M, 20.30.179.179, swap 21249
                 payload autoDecide, ttlMode uniform, apply egress-acl
                 interface Ethernet40
                via M, 20.30.217.217, swap 21249
                 payload autoDecide, ttlMode uniform, apply egress-acl
                 interface Ethernet4
                via M, 20.30.221.221, swap 721249
                 payload autoDecide, ttlMode uniform, apply egress-acl
                 interface Ethernet15
                via M, 21.30.156.156, swap 21249
                 payload autoDecide, ttlMode uniform, apply egress-acl
                 interface Ethernet21
 IP    21284    [1], 10.0.0.156/32, algorithm MIN-LATENCY
                via M, 20.30.156.156, pop
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                 interface Ethernet11
                via M, 21.30.156.156, pop
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                 interface Ethernet21
 IP    21285    [1], 10.0.0.156/32, algorithm MIN-TE
                via M, 20.30.156.156, pop
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                 interface Ethernet11
                via M, 21.30.156.156, pop
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                 interface Ethernet21
 IP    21286    [1], 10.0.0.156/32, algorithm ADMIN
                via M, 20.30.156.156, pop
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                 interface Ethernet11
                via M, 21.30.156.156, pop
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                 interface Ethernet21
 IP    21303    [1], 10.0.0.175/32, algorithm MIN-LATENCY
                via TI-LFA tunnel index 16, pop
                 payload autoDecide, ttlMode uniform, apply egress-acl
                    via 20.30.221.221, Ethernet15, label 721303
                    backup via 20.30.53.53, Ethernet13, label 21303
 IP    21304    [1], 10.0.0.175/32, algorithm MIN-TE
                via M, 20.30.32.32, swap 21304
                 payload autoDecide, ttlMode uniform, apply egress-acl
                 interface Ethernet2
                via M, 20.30.53.53, swap 21304
                 payload autoDecide, ttlMode uniform, apply egress-acl
                 interface Ethernet13
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
                via M, 21.30.156.156, swap 21304
                 payload autoDecide, ttlMode uniform, apply egress-acl
                 interface Ethernet21
 IP    21305    [1], 10.0.0.175/32, algorithm ADMIN
                via M, 20.30.131.131, forward
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                 interface Ethernet35
 IP    21307    [1], 10.0.0.179/32, algorithm MIN-LATENCY
                via TI-LFA tunnel index 26, pop
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                    via 20.30.179.179, Ethernet40, label imp-null(3)
                    backup via 20.30.221.221, Ethernet15, label 721303 21307
 IP    21308    [1], 10.0.0.179/32, algorithm MIN-TE
                via TI-LFA tunnel index 21, pop
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                    via 20.30.179.179, Ethernet40, label imp-null(3)
                    backup via 21.30.156.156, Ethernet21, label 21308
 IP    21309    [1], 10.0.0.179/32, algorithm ADMIN
                via M, 20.30.179.179, pop
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                 interface Ethernet40
 IP    21345    [1], 10.0.0.217/32, algorithm MIN-LATENCY
                via TI-LFA tunnel index 19, forward
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                    via 20.30.217.217, Ethernet4, label imp-null(3)
                    backup via 20.30.221.221, Ethernet15, label 721303
 IP    21346    [1], 10.0.0.217/32, algorithm MIN-TE
                via TI-LFA tunnel index 0, forward
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                    via 20.30.217.217, Ethernet4, label imp-null(3)
                    backup via 20.30.179.179, Ethernet40, label imp-null(3)
 IP    21347    [1], 10.0.0.217/32, algorithm ADMIN
                via M, 20.30.217.217, forward
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                 interface Ethernet4
 IP    21349    [1], 10.0.0.221/32, algorithm MIN-LATENCY
                via TI-LFA tunnel index 14, pop
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                    via 20.30.221.221, Ethernet15, label imp-null(3)
                    backup via 20.30.53.53, Ethernet13, label 21303 21349
 IP    21350    [1], 10.0.0.221/32, algorithm MIN-TE
                via TI-LFA tunnel index 22, pop
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                    via 20.30.221.221, Ethernet15, label imp-null(3)
                    backup via 20.30.179.179, Ethernet40, label 21350
 IP    21581    [1], 2002::53/128, algorithm MIN-LATENCY
                via TI-LFA tunnel index 40, pop
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                    via fe80::5e07:58ff:fea3:aaa, Ethernet13, label imp-null(3)
                    backup via fe80::d248:a1ff:feba:3c61, Ethernet11, label 19 21581
 IP    21582    [1], 2002::53/128, algorithm MIN-TE
                via TI-LFA tunnel index 39, pop
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                    via fe80::5e07:58ff:fea3:aaa, Ethernet13, label imp-null(3)
                    backup via fe80::d248:a1ff:feba:3c61, Ethernet11, label 21582
 IP    21583    [1], 2002::53/128, algorithm ADMIN
                via M, fe80::5e07:58ff:fea3:aaa, pop
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                 interface Ethernet13
 IP    21648    [1], 2002::120/128, algorithm MIN-LATENCY
                via M, fe80::be31:e2ff:fee1:ec2c, pop
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                 interface Ethernet3
 IP    21649    [1], 2002::120/128, algorithm MIN-TE
                via M, fe80::be31:e2ff:fee1:ec2c, pop
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                 interface Ethernet3
 IP    21650    [1], 2002::120/128, algorithm ADMIN
                via M, fe80::be31:e2ff:fee1:ec2c, pop
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                 interface Ethernet3
 IP    21684    [1], 2002::156/128, algorithm MIN-LATENCY
                via TI-LFA tunnel index 12, pop
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                    via fe80::d248:a1ff:feba:3c61, Ethernet11, label imp-null(3)
                    backup via fe80::5e07:58ff:fea3:aaa, Ethernet13, label 21703 21684
 IP    21685    [1], 2002::156/128, algorithm MIN-TE
                via TI-LFA tunnel index 5, pop
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                    via fe80::d248:a1ff:feba:3c61, Ethernet11, label imp-null(3)
                    backup via fe80::5e07:58ff:fea3:aaa, Ethernet13, label 21685
 IP    21686    [1], 2002::156/128, algorithm ADMIN
                via M, fe80::d248:a1ff:feba:3c61, pop
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                 interface Ethernet11
 IP    21703    [1], 2002::175/128, algorithm MIN-LATENCY
                via TI-LFA tunnel index 1, pop
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                    via fe80::5e07:58ff:fea3:aaa, Ethernet13, label 21703
                    backup via fe80::d248:a1ff:feba:3c61, Ethernet11, label 19
 IP    21704    [1], 2002::175/128, algorithm MIN-TE
                via M, fe80::5e07:58ff:fea3:aaa, forward
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                 interface Ethernet13
                via M, fe80::d248:a1ff:feba:3c61, forward
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                 interface Ethernet11
                via M, fe80::d6af:f7ff:fe2f:1396, forward
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                 interface Ethernet2
 IP    21705    [1], 2002::175/128, algorithm ADMIN
                via M, fe80::c214:b8ff:fe21:9790, forward
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                 interface Ethernet4
 B3    362144   [0]
                via I, ipv4, vrf FLEXALGO
 B3    362145   [0]
                via I, ipv4, vrf RED
 B3    362146   [0]
                via I, ipv6, vrf RED
 IA    378528   [1]
                via M, 20.30.53.53, pop
                 payload autoDecide, ttlMode uniform, apply egress-acl
                 interface Ethernet13
 IA    378529   [1]
                via M, fe80::5e07:58ff:fea3:aaa, pop
                 payload autoDecide, ttlMode uniform, apply egress-acl
                 interface Ethernet13
 IA    378533   [1]
                via M, 20.30.131.131, pop
                 payload autoDecide, ttlMode uniform, apply egress-acl
                 interface Ethernet35
 IA    378538   [1]
                via M, 20.30.179.179, pop
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
 IA    378553   [1]
                via M, 20.30.214.214, pop
                 payload autoDecide, ttlMode uniform, apply egress-acl
                 interface Ethernet5
 IA    378562   [1]
                via M, 21.30.214.214, pop
                 payload autoDecide, ttlMode uniform, apply egress-acl
                 interface Ethernet6
 IA    378574   [1]
                via M, 21.30.156.156, pop
                 payload autoDecide, ttlMode uniform, apply egress-acl
                 interface Ethernet21
 IA    378577   [1]
                via M, 20.30.72.72, pop
                 payload autoDecide, ttlMode uniform, apply egress-acl
                 interface Ethernet9
 IA    378578   [1]
                via M, 20.30.66.66, pop
                 payload autoDecide, ttlMode uniform, apply egress-acl
                 interface Ethernet31
 IA    378582   [1]
                via M, 20.30.217.217, pop
                 payload autoDecide, ttlMode uniform, apply egress-acl
                 interface Ethernet4
 IA    378583   [1]
                via M, fe80::c214:b8ff:fe21:9790, pop
                 payload autoDecide, ttlMode uniform, apply egress-acl
                 interface Ethernet4
 IA    378586   [1]
                via M, 20.30.84.84, pop
                 payload autoDecide, ttlMode uniform, apply egress-acl
                 interface Ethernet12
 IA    378587   [1]
                via M, fe80::5a70:7fff:fe9f:c403, pop
                 payload autoDecide, ttlMode uniform, apply egress-acl
                 interface Ethernet12
 IA    378588   [1]
                via M, 20.30.32.32, pop
                 payload autoDecide, ttlMode uniform, apply egress-acl
                 interface Ethernet2
 IA    378589   [1]
                via M, fe80::d6af:f7ff:fe2f:1396, pop
                 payload autoDecide, ttlMode uniform, apply egress-acl
                 interface Ethernet2
 IA    378590   [1]
                via M, 21.30.120.120, pop
                 payload autoDecide, ttlMode uniform, apply egress-acl
                 interface Ethernet10
 IA    378597   [1]
                via M, 20.30.120.120, pop
                 payload autoDecide, ttlMode uniform, apply egress-acl
                 interface Ethernet3
 IA    378598   [1]
                via M, fe80::be31:e2ff:fee1:ec2c, pop
                 payload autoDecide, ttlMode uniform, apply egress-acl
                 interface Ethernet3
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
 * >      RD: 53:5001 IPv4 prefix 50.10.53.0/24
                                 10.0.0.53             -       100     0       ?
 * >      RD: 66:5001 IPv4 prefix 50.10.66.0/24
                                 10.0.0.66             -       100     0       ?
 * >      RD: 72:5001 IPv4 prefix 50.10.72.0/24
                                 10.0.0.72             -       100     0       ?
 * >      RD: 84:5001 IPv4 prefix 50.10.84.0/24
                                 10.0.0.84             0       100     0       ?
 * >      RD: 120:5001 IPv4 prefix 50.10.120.0/24
                                 10.0.0.120            0       100     0       ?
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
 * >      RD: 221:5001 IPv4 prefix 50.10.221.0/24
                                 10.0.0.221            -       100     0       i
 * >      RD: 10.0.0.30:5128 IPv4 prefix 50.128.32.0/24
                                 10.0.0.32             -       100     0       i
 * >      RD: 53:5128 IPv4 prefix 50.128.53.0/24
                                 10.0.0.53             -       100     0       ?
 * >      RD: 120:5128 IPv4 prefix 50.128.120.0/24
                                 10.0.0.120            0       100     0       ?
 * >      RD: 5128:5128 IPv4 prefix 50.128.156.0/24
                                 10.0.0.156            -       100     0       i
 * >      RD: 5128:5128 IPv4 prefix 50.128.179.0/24
                                 10.0.0.179            -       100     0       i
 * >      RD: 217:5128 IPv4 prefix 50.128.217.0/24
                                 10.0.0.217            -       100     0       i
 * >      RD: 10.0.0.30:5128 IPv4 prefix 50.129.32.0/24
                                 10.0.0.32             -       100     0       i
 * >      RD: 53:5128 IPv4 prefix 50.129.53.0/24
                                 10.0.0.53             -       100     0       ?
 * >      RD: 66:5001 IPv4 prefix 50.129.66.0/24
                                 10.0.0.66             -       100     0       ?
 * >      RD: 72:5001 IPv4 prefix 50.129.72.0/24
                                 10.0.0.72             -       100     0       ?
 * >      RD: 120:5129 IPv4 prefix 50.129.120.0/24
                                 10.0.0.120            0       100     0       ?
 * >      RD: 5128:5128 IPv4 prefix 50.129.156.0/24
                                 10.0.0.156            -       100     0       i
 * >      RD: 5128:5128 IPv4 prefix 50.129.179.0/24
                                 10.0.0.179            -       100     0       i
 * >      RD: 217:5128 IPv4 prefix 50.129.217.0/24
                                 10.0.0.217            -       100     0       i
 * >      RD: 221:5128 IPv4 prefix 50.129.221.0/24
                                 10.0.0.221            -       100     0       i
 * >      RD: 10.0.0.30:5128 IPv4 prefix 50.130.32.0/24
                                 10.0.0.32             -       100     0       i
 * >      RD: 53:5128 IPv4 prefix 50.130.53.0/24
                                 10.0.0.53             -       100     0       ?
 * >      RD: 120:5130 IPv4 prefix 50.130.120.0/24
                                 10.0.0.120            0       100     0       ?
 * >      RD: 5128:5128 IPv4 prefix 50.130.156.0/24
                                 10.0.0.156            -       100     0       i
 * >      RD: 5128:5128 IPv4 prefix 50.130.179.0/24
                                 10.0.0.179            -       100     0       i
 * >      RD: 217:5128 IPv4 prefix 50.130.217.0/24
                                 10.0.0.217            -       100     0       i
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
  Connect timer is active, time left: 00:02:15
  Connection interval is 148 seconds
  Failed connection attempts is 507
  Idle-restart timer is inactive
  BGP state is Active
  Number of transitions to established: 0
  Last state was Connect
  Last event was TransportError
  Last sent socket-error:Connect (Network is unreachable), Last time 00:00:14, First time 23:36:00, Repeats 506
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
  Last read 00:00:19, last write 00:00:40
  Hold time is 180, keepalive interval is 60 seconds
  Configured hold time is 180, keepalive interval is 60 seconds
  Effective minimum hold time is 3 seconds
  Send failure hold time is 0 seconds
  Hold timer is active, time left: 00:02:41
  Keepalive timer is active, time left: 00:00:14
  Connect timer is inactive
  Idle-restart timer is inactive
  BGP state is Established, up for 23:36:00
  Number of transitions to established: 1
  Last state was OpenConfirm
  Last event was RecvUpdate
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
      Restart-State bit: yes
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
      Received 23:35:59
      Number of stale paths removed after graceful restart: 0
      Number of paths received before End-of-RIB: 1
    VPN-IPv6 End-of-RIB received: Yes
      Received 23:35:59
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
    Updates:                       123         7
    Keepalives:                   1641      1662
    Enhanced Route Refresh:          0         0
    Begin of Route Refresh:          0         0
    End of Route Refresh:            0         0
    Total messages:               1765      1670
  Prefix Statistics:
                                   Sent      Rcvd     Best Paths     Best ECMP Paths
    IPv4 Unicast:                     0         0              0                   0
    VPN-IPv4:                        29         4              4                   0
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
Local TCP address is 10.0.0.30, local port is 39975
Remote TCP address is 10.0.0.32, remote port is 179
Local next hop for next hop self:
  VPN-IPv4: 10.0.0.30
  VPN-IPv6: ::ffff:10.0.0.30
TCP Socket Information:
  TCP state is ESTABLISHED
  Recv-Q: 0/32768
  Send-Q: 0/46080
  Outgoing Maximum Segment Size (MSS): 36
  Total Number of TCP retransmissions: 0
  Options:
    Timestamps enabled: yes
    Selective Acknowledgments enabled: yes
    Window Scale enabled: yes
    Explicit Congestion Notification (ECN) enabled: no
  Socket Statistics:
    Window Scale (wscale): 7,7
    Retransmission Timeout (rto): 204.0ms
    Round-trip Time (rtt/rtvar): 0.2ms/0.0ms
    Delayed Ack Timeout (ato): 40.0ms
    Congestion Window (cwnd): 10
    TCP Throughput: 11.76 Mbps
    Advertised Recv Window (rcv_space): 14480

BGP neighbor is 10.0.0.53, remote AS 64512, internal link
 Description: Arrcus-53
  BGP version 4, remote router ID 10.0.0.53, VRF default
  Inherits configuration from and member of peer-group IBGP_CLIENT_PEER
  Last read 00:00:02, last write 00:00:08
  Hold time is 180, keepalive interval is 60 seconds
  Configured hold time is 180, keepalive interval is 60 seconds
  Effective minimum hold time is 3 seconds
  Send failure hold time is 0 seconds
  Hold timer is active, time left: 00:02:58
  Keepalive timer is active, time left: 00:00:36
  Connect timer is inactive
  Idle-restart timer is inactive
  BGP state is Established, up for 23:36:01
  Number of transitions to established: 1
  Last state was OpenConfirm
  Last event was RecvRtRefresh
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
      Restart-State bit: yes
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
      Received 23:36:01
      Number of stale paths removed after graceful restart: 0
    VPN-IPv6 End-of-RIB received: Yes
      Received 23:36:01
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
    Updates:              160        10
    Keepalives:          1637      1417
    Route Refresh:          0         2
    Total messages:      1798      1430
  Prefix Statistics:
                                   Sent      Rcvd     Best Paths     Best ECMP Paths
    IPv4 Unicast:                     0         0              0                   0
    VPN-IPv4:                        29         4              4                   0
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
Remote TCP address is 10.0.0.53, remote port is 36759
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
    Round-trip Time (rtt/rtvar): 0.3ms/0.0ms
    Delayed Ack Timeout (ato): 40.0ms
    Congestion Window (cwnd): 10
    TCP Throughput: 443.55 Mbps
    Advertised Recv Window (rcv_space): 14600

BGP neighbor is 10.0.0.66, remote AS 64512, internal link
 Description: Ciena-8140-66
  BGP version 4, remote router ID 10.0.0.66, VRF default
  Inherits configuration from and member of peer-group IBGP_CLIENT_PEER
  Last read 00:00:54, last write 00:00:11
  Hold time is 180, keepalive interval is 60 seconds
  Configured hold time is 180, keepalive interval is 60 seconds
  Effective minimum hold time is 3 seconds
  Send failure hold time is 0 seconds
  Hold timer is active, time left: 00:02:06
  Keepalive timer is active, time left: 00:00:39
  Connect timer is inactive
  Idle-restart timer is inactive
  BGP state is Established, up for 01:36:54
  Number of transitions to established: 6
  Last state was OpenConfirm
  Last event was RecvUpdate
  Last sent notification:Hold Timer Expired Error/None, Last time 03:12:32, First time 07:18:20, Repeats 1
  Last rcvd notification:Cease/other configuration change, Last time 01:37:13, First time 23:25:36, Repeats 2
  Last sent socket-error:Connect (Connection refused), Last time 01:37:03, First time 03:06:09, Repeats 8
  Last rcvd socket-error:Connection reset by peer, Last time 01:36:54, First time 01:36:59, Repeats 1
  Types of communities advertised: standard extended large
  Neighbor is a route reflector client
  Neighbor is using global cluster ID 10.0.0.30
  Neighbor Capabilities:
    Multiprotocol IPv4 Unicast: received
    Multiprotocol VPN-IPv4: advertised and received and negotiated
    Multiprotocol VPN-IPv6: advertised
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
  Restart timer is inactive
  End of rib timer is inactive
    VPN-IPv4 End-of-RIB received: Yes
      Received 01:36:44
      Number of stale paths removed after graceful restart: 0
      Number of paths received before End-of-RIB: 2
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
    Opens:                  8         6
    Notifications:          2         3
    Updates:              250        20
    Keepalives:          1432      1231
    Route Refresh:          0         0
    Total messages:      1692      1260
  Prefix Statistics:
                                   Sent      Rcvd     Best Paths     Best ECMP Paths
    IPv4 Unicast:                     0         0              0                   0
    VPN-IPv4:                        31         2              2                   0
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
    VPN-IPv4 NLRIs dropped due to maximum route limit violation: 0
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
Local TCP address is 10.0.0.30, local port is 179
Remote TCP address is 10.0.0.66, remote port is 38163
Local next hop for next hop self:
  VPN-IPv4: 10.0.0.30
TCP Socket Information:
  TCP state is ESTABLISHED
  Recv-Q: 0/32768
  Send-Q: 0/46080
  Outgoing Maximum Segment Size (MSS): 1460
  Total Number of TCP retransmissions: 0
  Options:
    Timestamps enabled: no
    Selective Acknowledgments enabled: yes
    Window Scale enabled: yes
    Explicit Congestion Notification (ECN) enabled: no
  Socket Statistics:
    Window Scale (wscale): 7,7
    Retransmission Timeout (rto): 204.0ms
    Round-trip Time (rtt/rtvar): 0.5ms/0.0ms
    Delayed Ack Timeout (ato): 40.0ms
    Congestion Window (cwnd): 10
    TCP Throughput: 250.64 Mbps
    Advertised Recv Window (rcv_space): 14600

BGP neighbor is 10.0.0.72, remote AS 64512, internal link
 Description: Ciena-5134-72
  BGP version 4, remote router ID 10.0.0.72, VRF default
  Inherits configuration from and member of peer-group IBGP_CLIENT_PEER
  Last read 00:00:40, last write 00:00:07
  Hold time is 180, keepalive interval is 60 seconds
  Configured hold time is 180, keepalive interval is 60 seconds
  Effective minimum hold time is 3 seconds
  Send failure hold time is 0 seconds
  Hold timer is active, time left: 00:02:20
  Keepalive timer is active, time left: 00:00:50
  Connect timer is inactive
  Idle-restart timer is inactive
  BGP state is Established, up for 01:36:40
  Number of transitions to established: 7
  Last state was OpenConfirm
  Last event was RecvUpdate
  Last sent notification:Hold Timer Expired Error/None, Last time 03:11:47, First time 07:21:40, Repeats 1
  Last rcvd notification:Cease/other configuration change, Last time 01:37:09, First time 23:32:53, Repeats 3
  Last sent socket-error:Connect (Connection refused), Last time 01:36:50, First time 03:06:11, Repeats 7
  Last rcvd socket-error:Connection reset by peer, Last time 01:36:46, First time 04:16:53, Repeats 4
  Types of communities advertised: standard extended large
  Neighbor is a route reflector client
  Neighbor is using global cluster ID 10.0.0.30
  Neighbor Capabilities:
    Multiprotocol IPv4 Unicast: received
    Multiprotocol VPN-IPv4: advertised and received and negotiated
    Multiprotocol VPN-IPv6: advertised
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
  Restart timer is inactive
  End of rib timer is inactive
    VPN-IPv4 End-of-RIB received: Yes
      Received 01:36:30
      Number of stale paths removed after graceful restart: 0
      Number of paths received before End-of-RIB: 2
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
    Opens:                 12         7
    Notifications:          2         4
    Updates:              266        21
    Keepalives:          1438      1228
    Route Refresh:          0         0
    Total messages:      1718      1260
  Prefix Statistics:
                                   Sent      Rcvd     Best Paths     Best ECMP Paths
    IPv4 Unicast:                     0         0              0                   0
    VPN-IPv4:                        31         2              2                   0
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
    VPN-IPv4 NLRIs dropped due to maximum route limit violation: 0
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
Local TCP address is 10.0.0.30, local port is 179
Remote TCP address is 10.0.0.72, remote port is 37843
Local next hop for next hop self:
  VPN-IPv4: 10.0.0.30
TCP Socket Information:
  TCP state is ESTABLISHED
  Recv-Q: 0/32768
  Send-Q: 0/46080
  Outgoing Maximum Segment Size (MSS): 1460
  Total Number of TCP retransmissions: 0
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
    Congestion Window (cwnd): 10
    TCP Throughput: 182.79 Mbps
    Advertised Recv Window (rcv_space): 14600

BGP neighbor is 10.0.0.84, remote AS 64512, internal link
 Description: Ericsson_84
  BGP version 4, remote router ID 10.0.0.84, VRF default
  Inherits configuration from and member of peer-group IBGP_CLIENT_PEER
  Last read 00:00:57, last write 00:00:46
  Hold time is 180, keepalive interval is 60 seconds
  Configured hold time is 180, keepalive interval is 60 seconds
  Effective minimum hold time is 3 seconds
  Send failure hold time is 0 seconds
  Hold timer is active, time left: 00:02:03
  Keepalive timer is active, time left: 00:00:10
  Connect timer is inactive
  Idle-restart timer is inactive
  BGP state is Established, up for 23:36:00
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
      L2VPN EVPN is enabled, Forwarding State is preserved
  Restart timer is inactive
  End of rib timer is inactive
    VPN-IPv4 End-of-RIB received: Yes
      Received 23:36:00
      Number of stale paths removed after graceful restart: 0
      Number of paths received before End-of-RIB: 1
    VPN-IPv6 End-of-RIB received: Yes
      Received 23:36:00
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
    Updates:                       134         4
    Keepalives:                   1635      1415
    Enhanced Route Refresh:          0         0
    Begin of Route Refresh:          0         0
    End of Route Refresh:            0         0
    Total messages:               1770      1420
  Prefix Statistics:
                                   Sent      Rcvd     Best Paths     Best ECMP Paths
    IPv4 Unicast:                     0         0              0                   0
    VPN-IPv4:                        32         1              1                   0
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
Local TCP address is 10.0.0.30, local port is 35281
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
    Round-trip Time (rtt/rtvar): 232.0ms/0.1ms
    Delayed Ack Timeout (ato): 40.0ms
    Congestion Window (cwnd): 10
    TCP Throughput: 0.49 Mbps
    Advertised Recv Window (rcv_space): 14480

BGP neighbor is 10.0.0.120, remote AS 64512, internal link
 Description: Huawei_120
  BGP version 4, remote router ID 10.0.0.120, VRF default
  Inherits configuration from and member of peer-group IBGP_CLIENT_PEER
  Last read 00:00:22, last write 00:00:31
  Hold time is 180, keepalive interval is 60 seconds
  Configured hold time is 180, keepalive interval is 60 seconds
  Effective minimum hold time is 3 seconds
  Send failure hold time is 0 seconds
  Hold timer is active, time left: 00:02:38
  Keepalive timer is active, time left: 00:00:19
  Connect timer is inactive
  Idle-restart timer is inactive
  BGP state is Established, up for 01:13:21
  Number of transitions to established: 2
  Last state was OpenConfirm
  Last event was RecvKeepAlive
  Last sent notification:Hold Timer Expired Error/None, Last time 01:13:46
  Last sent socket-error:Connect (Connection refused), Last time 01:13:23, First time 01:13:45, Repeats 5
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
    Opens:                  2         3
    Notifications:          2         0
    Updates:              137        18
    Keepalives:           249       254
    Route Refresh:          0         2
    Total messages:       390       277
  Prefix Statistics:
                                   Sent      Rcvd     Best Paths     Best ECMP Paths
    IPv4 Unicast:                     0         0              0                   0
    VPN-IPv4:                        29         4              4                   0
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
Remote TCP address is 10.0.0.120, remote port is 55845
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
    Round-trip Time (rtt/rtvar): 0.3ms/0.0ms
    Delayed Ack Timeout (ato): 40.0ms
    Congestion Window (cwnd): 10
    TCP Throughput: 332.49 Mbps
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
  Connect timer is active, time left: 00:02:19
  Connection interval is 148 seconds
  Failed connection attempts is 14
  Idle-restart timer is inactive
  BGP state is Active
  Number of transitions to established: 0
  Last state was Connect
  Last event was TransportError
  Last sent socket-error:Connect (Connection refused), Last time 00:00:52, First time 06:23:13, Repeats 163
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

BGP neighbor is 10.0.0.128, remote AS 64512, internal link
 Description: Huawei_128
  BGP version 4, remote router ID 10.0.0.128, VRF default
  Inherits configuration from and member of peer-group IBGP_CLIENT_PEER
  Last read 05:37:47, last write 05:37:47
  Hold time is 180, keepalive interval is 60 seconds
  Configured hold time is 180, keepalive interval is 60 seconds
  Effective minimum hold time is 3 seconds
  Send failure hold time is 0 seconds
  Hold timer is inactive
  Keepalive timer is inactive
  Connect timer is active, time left: 00:00:15
  Connection interval is 148 seconds
  Failed connection attempts is 21
  Idle-restart timer is inactive
  BGP state is Active
  Number of transitions to established: 1
  Last state was Connect
  Last event was TransportError
  Last sent notification:Open Message Error/unsupported capability, Last time 05:37:47, First time 05:52:06, Repeats 38
    Sent data: 0x010400010080010400020080
  Last rcvd notification:Cease/peer de-configured, Last time 05:51:35
  Last sent socket-error:Connect (Connection refused), Last time 00:02:51, First time 00:42:11, Repeats 20
  Last rcvd socket-error:Connection reset by peer, Last time 05:51:01, First time 05:51:34, Repeats 5
  Types of communities advertised: standard extended large
  Neighbor is a route reflector client
  Neighbor is using global cluster ID 10.0.0.30
  Neighbor Capabilities:
    Multiprotocol IPv4 Unicast: received
    Multiprotocol VPN-IPv4: advertised
    Multiprotocol VPN-IPv6: advertised
    Four Octet ASN: advertised and received
    Route Refresh: advertised and received
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
    Opens:                 46        40
    Notifications:         39         1
    Updates:               25         2
    Keepalives:             2         1
    Route Refresh:          0         0
    Total messages:       112        44
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
Remote TCP address is 10.0.0.128, remote port is 179

BGP neighbor is 10.0.0.131, remote AS 64512, internal link
 Description: Juniper-131-JCNR
  BGP version 4, remote router ID 10.0.0.131, VRF default
  Inherits configuration from and member of peer-group IBGP_CLIENT_PEER
  Last read 00:00:26, last write 00:00:10
  Hold time is 90, keepalive interval is 30 seconds
  Configured hold time is 180, keepalive interval is 60 seconds
  Effective minimum hold time is 3 seconds
  Send failure hold time is 0 seconds
  Hold timer is active, time left: 00:01:04
  Keepalive timer is active, time left: 00:00:19
  Connect timer is inactive
  Idle-restart timer is inactive
  BGP state is Established, up for 23:36:00
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
      Received 23:35:59
      Number of stale paths removed after graceful restart: 0
      Number of paths received before End-of-RIB: 1
    VPN-IPv6 End-of-RIB received: Yes
      Received 23:35:59
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
    Updates:              134         4
    Keepalives:          3300      3137
    Route Refresh:          0         0
    Total messages:      3435      3142
  Prefix Statistics:
                                   Sent      Rcvd     Best Paths     Best ECMP Paths
    IPv4 Unicast:                     0         0              0                   0
    VPN-IPv4:                        32         1              1                   0
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
Local TCP address is 10.0.0.30, local port is 34875
Remote TCP address is 10.0.0.131, remote port is 179
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
    Window Scale (wscale): 1,7
    Retransmission Timeout (rto): 204.0ms
    Round-trip Time (rtt/rtvar): 0.4ms/0.1ms
    Delayed Ack Timeout (ato): 40.0ms
    Congestion Window (cwnd): 10
    TCP Throughput: 296.27 Mbps
    Advertised Recv Window (rcv_space): 14480

BGP neighbor is 10.0.0.156, remote AS 64512, internal link
 Description: Juniper-156
  BGP version 4, remote router ID 10.0.0.156, VRF default
  Inherits configuration from and member of peer-group IBGP_CLIENT_PEER
  Last read 00:00:01, last write 00:00:03
  Hold time is 90, keepalive interval is 30 seconds
  Configured hold time is 180, keepalive interval is 60 seconds
  Effective minimum hold time is 3 seconds
  Send failure hold time is 0 seconds
  Hold timer is active, time left: 00:01:29
  Keepalive timer is active, time left: 00:00:22
  Connect timer is inactive
  Idle-restart timer is inactive
  BGP state is Established, up for 23:36:00
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
      Received 23:35:59
      Number of stale paths removed after graceful restart: 0
      Number of paths received before End-of-RIB: 4
    VPN-IPv6 End-of-RIB received: Yes
      Received 23:35:59
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
    Updates:              131         7
    Keepalives:          3302      3126
    Route Refresh:          0         0
    Total messages:      3434      3134
  Prefix Statistics:
                                   Sent      Rcvd     Best Paths     Best ECMP Paths
    IPv4 Unicast:                     0         0              0                   0
    VPN-IPv4:                        29         4              4                   0
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
Local TCP address is 10.0.0.30, local port is 43549
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
    Round-trip Time (rtt/rtvar): 0.4ms/0.0ms
    Delayed Ack Timeout (ato): 40.0ms
    Congestion Window (cwnd): 10
    TCP Throughput: 304.04 Mbps
    Advertised Recv Window (rcv_space): 14480

BGP neighbor is 10.0.0.179, remote AS 64512, internal link
 Description: Juniper-179
  BGP version 4, remote router ID 10.0.0.179, VRF default
  Inherits configuration from and member of peer-group IBGP_CLIENT_PEER
  Last read 00:00:08, last write 00:00:04
  Hold time is 90, keepalive interval is 30 seconds
  Configured hold time is 180, keepalive interval is 60 seconds
  Effective minimum hold time is 3 seconds
  Send failure hold time is 0 seconds
  Hold timer is active, time left: 00:01:22
  Keepalive timer is active, time left: 00:00:18
  Connect timer is inactive
  Idle-restart timer is inactive
  BGP state is Established, up for 07:30:05
  Number of transitions to established: 1
  Last state was OpenConfirm
  Last event was RecvUpdate
  Last sent notification:Open Message Error/unsupported capability, Last time 07:32:01, First time 23:36:00, Repeats 333
    Sent data: 0x010400010080010400020080
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
      Received 07:30:04
      Number of stale paths removed after graceful restart: 0
      Number of paths received before End-of-RIB: 4
    VPN-IPv6 End-of-RIB received: Yes
      Received 07:30:04
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
    Opens:                335       335
    Notifications:        334         0
    Updates:              100         7
    Keepalives:          1041       999
    Route Refresh:          0         0
    Total messages:      1810      1341
  Prefix Statistics:
                                   Sent      Rcvd     Best Paths     Best ECMP Paths
    IPv4 Unicast:                     0         0              0                   0
    VPN-IPv4:                        29         4              4                   0
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
Local TCP address is 10.0.0.30, local port is 179
Remote TCP address is 10.0.0.179, remote port is 50428
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
    Round-trip Time (rtt/rtvar): 0.8ms/0.1ms
    Delayed Ack Timeout (ato): 40.0ms
    Congestion Window (cwnd): 10
    TCP Throughput: 141.61 Mbps
    Advertised Recv Window (rcv_space): 14600

BGP neighbor is 10.0.0.184, remote AS 64512, internal link
 Description: IXIA
  BGP version 4, remote router ID 0.0.0.0, VRF default
  Inherits configuration from and member of peer-group IBGP_CLIENT_PEER
  Last read never, last write never
  Hold time is 0, keepalive interval is 0 seconds
  Configured hold time is 180, keepalive interval is 60 seconds
  Effective minimum hold time is 3 seconds
  Send failure hold time is 0 seconds
  Hold timer is inactive
  Keepalive timer is inactive
  Connect timer is active, time left: 00:01:53
  Connection interval is 148 seconds
  Failed connection attempts is 505
  Idle-restart timer is inactive
  BGP state is Active
  Number of transitions to established: 0
  Last state was Connect
  Last event was TransportError
  Last sent socket-error:Connect (Network is unreachable), Last time 00:01:15, First time 23:36:00, Repeats 504
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
Remote TCP address is 10.0.0.184, remote port is 179

BGP neighbor is 10.0.0.214, remote AS 64512, internal link
 Description: Nokia-SXR-214
  BGP version 4, remote router ID 10.0.0.214, VRF default
  Inherits configuration from and member of peer-group IBGP_CLIENT_PEER
  Last read 00:00:16, last write 00:00:16
  Hold time is 90, keepalive interval is 30 seconds
  Configured hold time is 180, keepalive interval is 60 seconds
  Effective minimum hold time is 3 seconds
  Send failure hold time is 0 seconds
  Hold timer is active, time left: 00:01:14
  Keepalive timer is active, time left: 00:00:08
  Connect timer is inactive
  Idle-restart timer is inactive
  BGP state is Established, up for 23:27:17
  Number of transitions to established: 1
  Last state was OpenConfirm
  Last event was RecvUpdate
  Last sent socket-error:Connect (Network is unreachable), Last time 23:27:21, First time 23:36:00, Repeats 10
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
      Received 23:27:16
      Number of stale paths removed after graceful restart: 0
      Number of paths received before End-of-RIB: 1
    VPN-IPv6 End-of-RIB received: Yes
      Received 23:27:16
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
    Updates:              126         4
    Keepalives:          3289      2816
    Route Refresh:          0         0
    Total messages:      3416      2821
  Prefix Statistics:
                                   Sent      Rcvd     Best Paths     Best ECMP Paths
    IPv4 Unicast:                     0         0              0                   0
    VPN-IPv4:                        32         1              1                   0
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
Local TCP address is 10.0.0.30, local port is 45419
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
    TCP Throughput: 313.93 Mbps
    Advertised Recv Window (rcv_space): 14480

BGP neighbor is 10.0.0.217, remote AS 64512, internal link
 Description: Nokia
  BGP version 4, remote router ID 10.0.0.217, VRF default
  Inherits configuration from and member of peer-group IBGP_CLIENT_PEER
  Last read 00:00:30, last write 00:00:22
  Hold time is 90, keepalive interval is 30 seconds
  Configured hold time is 180, keepalive interval is 60 seconds
  Effective minimum hold time is 3 seconds
  Send failure hold time is 0 seconds
  Hold timer is active, time left: 00:01:00
  Keepalive timer is active, time left: 00:00:05
  Connect timer is inactive
  Idle-restart timer is inactive
  BGP state is Established, up for 23:36:00
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
      Received 23:36:00
      Number of stale paths removed after graceful restart: 0
      Number of paths received before End-of-RIB: 4
    VPN-IPv6 End-of-RIB received: Yes
      Received 23:36:00
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
    Updates:              131         7
    Keepalives:          3297      2833
    Route Refresh:          0         0
    Total messages:      3429      2841
  Prefix Statistics:
                                   Sent      Rcvd     Best Paths     Best ECMP Paths
    IPv4 Unicast:                     0         0              0                   0
    VPN-IPv4:                        29         4              4                   0
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
Local TCP address is 10.0.0.30, local port is 41903
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
    Round-trip Time (rtt/rtvar): 0.5ms/0.0ms
    Delayed Ack Timeout (ato): 40.0ms
    Congestion Window (cwnd): 10
    TCP Throughput: 169.37 Mbps
    Advertised Recv Window (rcv_space): 14480

BGP neighbor is 10.0.0.221, remote AS 64512, internal link
 Description: Ribbon-221
  BGP version 4, remote router ID 10.0.0.221, VRF default
  Inherits configuration from and member of peer-group IBGP_CLIENT_PEER
  Last read 00:00:20, last write 00:00:37
  Hold time is 180, keepalive interval is 60 seconds
  Configured hold time is 180, keepalive interval is 60 seconds
  Effective minimum hold time is 3 seconds
  Send failure hold time is 0 seconds
  Hold timer is active, time left: 00:02:40
  Keepalive timer is active, time left: 00:00:21
  Connect timer is inactive
  Idle-restart timer is inactive
  BGP state is Established, up for 00:33:05
  Number of transitions to established: 7
  Last state was OpenConfirm
  Last event was RecvKeepAlive
  Last sent notification:Hold Timer Expired Error/None, Last time 07:23:46
  Last sent socket-error:Connect (Network is unreachable), Last time 00:35:21, First time 08:10:42, Repeats 40
  Last rcvd socket-error:Connection reset by peer, Last time 00:42:10, First time 23:33:10, Repeats 4
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
    Opens:                           7         7
    Notifications:                   1         0
    Updates:                       401        22
    Keepalives:                   1594      3757
    Enhanced Route Refresh:          0        10
    Begin of Route Refresh:         10         0
    End of Route Refresh:           10         0
    Total messages:               2023      3796
  Prefix Statistics:
                                   Sent      Rcvd     Best Paths     Best ECMP Paths
    IPv4 Unicast:                     0         0              0                   0
    VPN-IPv4:                        31         2              2                   0
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
Local TCP address is 10.0.0.30, local port is 45883
Remote TCP address is 10.0.0.221, remote port is 179
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
    Window Scale (wscale): 9,7
    Retransmission Timeout (rto): 248.0ms
    Round-trip Time (rtt/rtvar): 12.7ms/24.9ms
    Delayed Ack Timeout (ato): 40.0ms
    Congestion Window (cwnd): 10
    TCP Throughput: 9.13 Mbps
    Advertised Recv Window (rcv_space): 14480

```

## show tunnel rib system-tunnel-rib brief

```text
Tunnel RIB: system-tunnel-rib
Endpoint        Tunnel Type     Index(es)   Tunnel Preference   IGP Preference 
-------------- --------------- ----------- ------------------- ----------------
10.0.0.32/32    IS-IS SR IPv4   20          65                  115            
10.0.0.53/32    IS-IS SR IPv4   10          65                  115            
10.0.0.66/32    IS-IS SR IPv4   13          65                  115            
10.0.0.72/32    IS-IS SR IPv4   14          65                  115            
10.0.0.84/32    IS-IS SR IPv4   8           65                  115            
10.0.0.120/32   IS-IS SR IPv4   17          65                  115            
10.0.0.131/32   IS-IS SR IPv4   9           65                  115            
10.0.0.156/32   IS-IS SR IPv4   11          65                  115            
10.0.0.175/32   IS-IS SR IPv4   7           65                  115            
10.0.0.179/32   IS-IS SR IPv4   12          65                  115            
10.0.0.214/32   IS-IS SR IPv4   21          65                  115            
10.0.0.217/32   IS-IS SR IPv4   16          65                  115            
10.0.0.221/32   IS-IS SR IPv4   15          65                  115            
2002::120/128   IS-IS SR IPv6   2           65                  115            
2002::175/128   IS-IS SR IPv6   3           65                  115            
2002::53/128    IS-IS SR IPv6   6           65                  115            
2002::156/128   IS-IS SR IPv6   5           65                  115            

   IGP Metric    Metric Type
---------------- -----------
   1             metric     
   1             metric     
   11            metric     
   11            metric     
   11            metric     
   1             metric     
   1             metric     
   1             metric     
   11            metric     
   1             metric     
   1             metric     
   1             metric     
   1             metric     
   10            metric     
   20            metric     
   10            metric     
   10            metric     

```

## show tunnel rib colored brief

```text
Tunnel RIB: system-colored-tunnel-rib
 Endpoint        Color   Tunnel Type       Index(es)    Tunnel Preference    IGP Preference    IGP Metric   Metric Type
--------------- ------- ----------------- ------------ -------------------- ----------------- ------------- -----------
 10.0.0.32/32    128     IS-IS FlexAlgo    46           65                   115               10000        metric     
 10.0.0.32/32    129     IS-IS FlexAlgo    47           65                   115               100          metric     
 10.0.0.32/32    130     IS-IS FlexAlgo    48           65                   115               1            metric     
 10.0.0.53/32    128     IS-IS FlexAlgo    8            65                   115               10000        metric     
 10.0.0.53/32    129     IS-IS FlexAlgo    3            65                   115               100          metric     
 10.0.0.53/32    130     IS-IS FlexAlgo    1            65                   115               1            metric     
 10.0.0.66/32    129     IS-IS FlexAlgo    13           65                   115               100          metric     
 10.0.0.72/32    129     IS-IS FlexAlgo    10           65                   115               100          metric     
 10.0.0.120/32   128     IS-IS FlexAlgo    51           65                   115               110010       metric     
 10.0.0.120/32   129     IS-IS FlexAlgo    52           65                   115               120          metric     
 10.0.0.156/32   128     IS-IS FlexAlgo    14           65                   115               10000        metric     
 10.0.0.156/32   129     IS-IS FlexAlgo    6            65                   115               100          metric     
 10.0.0.156/32   130     IS-IS FlexAlgo    37           65                   115               1            metric     
 10.0.0.175/32   128     IS-IS FlexAlgo    7            65                   115               10010        metric     
 10.0.0.175/32   129     IS-IS FlexAlgo    2            65                   115               110          metric     
 10.0.0.175/32   130     IS-IS FlexAlgo    28           65                   115               11           metric     
 10.0.0.179/32   128     IS-IS FlexAlgo    15           65                   115               10000        metric     
 10.0.0.179/32   129     IS-IS FlexAlgo    9            65                   115               100          metric     
 10.0.0.179/32   130     IS-IS FlexAlgo    34           65                   115               1            metric     
 10.0.0.217/32   128     IS-IS FlexAlgo    41           65                   115               10000        metric     
 10.0.0.217/32   129     IS-IS FlexAlgo    39           65                   115               100          metric     
 10.0.0.217/32   130     IS-IS FlexAlgo    40           65                   115               1            metric     
 10.0.0.221/32   128     IS-IS FlexAlgo    4            65                   115               10000        metric     
 10.0.0.221/32   129     IS-IS FlexAlgo    12           65                   115               100          metric     
 2002::120/128   128     IS-IS FlexAlgo    30           65                   115               10000        metric     
 2002::120/128   129     IS-IS FlexAlgo    31           65                   115               100          metric     
 2002::120/128   130     IS-IS FlexAlgo    29           65                   115               10           metric     
 2002::156/128   128     IS-IS FlexAlgo    21           65                   115               10000        metric     
 2002::156/128   129     IS-IS FlexAlgo    25           65                   115               100          metric     
 2002::156/128   130     IS-IS FlexAlgo    36           65                   115               10           metric     
 2002::53/128    128     IS-IS FlexAlgo    19           65                   115               10000        metric     
 2002::53/128    129     IS-IS FlexAlgo    17           65                   115               100          metric     
 2002::53/128    130     IS-IS FlexAlgo    20           65                   115               10           metric     
 2002::175/128   128     IS-IS FlexAlgo    26           65                   115               10100        metric     
 2002::175/128   129     IS-IS FlexAlgo    18           65                   115               110          metric     
 2002::175/128   130     IS-IS FlexAlgo    45           65                   115               20           metric     

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
>C    10.0.0.30/32 [0 pref/0 metric] updated 1d02h ago
         via Loopback0, directly connected
>C    20.30.32.0/24 [0 pref/0 metric] updated 00:00:27 ago
         via Ethernet2, directly connected
>C    20.30.53.0/24 [0 pref/0 metric] updated 00:11:33 ago
         via Ethernet13, directly connected
>C    20.30.66.0/24 [0 pref/0 metric] updated 02:10:35 ago
         via Ethernet31, directly connected
>C    20.30.72.0/24 [0 pref/0 metric] updated 02:10:35 ago
         via Ethernet9, directly connected
>C    20.30.84.0/24 [0 pref/0 metric] updated 01:25:41 ago
         via Ethernet12, directly connected
>C    20.30.120.0/24 [0 pref/0 metric] updated 00:45:14 ago
         via Ethernet3, directly connected
>C    20.30.124.0/24 [0 pref/0 metric] updated 00:19:01 ago
         via Ethernet17, directly connected
>C    20.30.131.0/24 [0 pref/0 metric] updated 1d02h ago
         via Ethernet35, directly connected
>C    20.30.156.0/24 [0 pref/0 metric] updated 02:39:29 ago
         via Ethernet11, directly connected
>C    20.30.179.0/24 [0 pref/0 metric] updated 02:44:27 ago
         via Ethernet40, directly connected
>C    20.30.184.0/24 [0 pref/0 metric] updated 1d02h ago
         via Ethernet7, directly connected
>C    20.30.214.0/24 [0 pref/0 metric] updated 07:12:29 ago
         via Ethernet5, directly connected
>C    20.30.217.0/24 [0 pref/0 metric] updated 00:10:52 ago
         via Ethernet4, directly connected
>C    20.30.221.0/24 [0 pref/0 metric] updated 00:33:30 ago
         via Ethernet15, directly connected
>C    21.30.120.0/24 [0 pref/0 metric] updated 01:10:49 ago
         via Ethernet10, directly connected
>C    21.30.124.0/24 [0 pref/0 metric] updated 00:19:01 ago
         via Ethernet18, directly connected
>C    21.30.128.0/24 [0 pref/0 metric] updated 01:26:43 ago
         via Ethernet20, directly connected
>C    21.30.156.0/24 [0 pref/0 metric] updated 02:39:25 ago
         via Ethernet21, directly connected
>C    21.30.214.0/24 [0 pref/0 metric] updated 06:05:33 ago
         via Ethernet6, directly connected
>C    21.30.217.0/24 [0 pref/0 metric] updated 06:04:06 ago
         via Ethernet8, directly connected
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
>P    0.0.0.0/8 [1 pref/0 metric] updated 1d02h ago
         via Null0, directly connected [NF]
>P    127.0.0.0/8 [1 pref/0 metric] updated 1d02h ago
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
>I    10.0.0.32/32 [115 pref/1 metric] updated 00:00:18 ago
         via 20.30.32.32, Ethernet2
>I    10.0.0.53/32 [115 pref/1 metric] updated 00:11:31 ago
         via 20.30.53.53, Ethernet13
>I    10.0.0.66/32 [115 pref/11 metric] updated 02:10:23 ago
         via 20.30.66.66, Ethernet31
>I    10.0.0.72/32 [115 pref/11 metric] updated 02:10:23 ago
         via 20.30.72.72, Ethernet9
>I    10.0.0.84/32 [115 pref/11 metric] updated 01:21:45 ago
         via 20.30.84.84, Ethernet12
>I    10.0.0.120/32 [115 pref/1 metric] updated 00:45:05 ago
         via 20.30.120.120, Ethernet3
         via 21.30.120.120, Ethernet10
>I    10.0.0.124/32 [115 pref/1 metric] updated 00:19:00 ago
         via 20.30.124.124, Ethernet17
         via 21.30.124.124, Ethernet18
>I    10.0.0.128/32 [115 pref/1 metric] updated 00:32:36 ago
         via 21.30.128.128, Ethernet20
>I    10.0.0.131/32 [115 pref/1 metric] updated 08:24:22 ago
         via 20.30.131.131, Ethernet35
>I    10.0.0.156/32 [115 pref/1 metric] updated 02:38:46 ago
         via 20.30.156.156, Ethernet11
         via 21.30.156.156, Ethernet21
>I    10.0.0.175/32 [115 pref/11 metric] updated 00:00:18 ago
         via 20.30.32.32, Ethernet2
         via 20.30.53.53, Ethernet13
         via 20.30.66.66, Ethernet31
         via 20.30.72.72, Ethernet9
         via 20.30.84.84, Ethernet12
         via 20.30.120.120, Ethernet3
         via 20.30.124.124, Ethernet17
         via 20.30.131.131, Ethernet35
>I    10.0.0.179/32 [115 pref/1 metric] updated 02:44:19 ago
         via 20.30.179.179, Ethernet40
>I    10.0.0.214/32 [115 pref/1 metric] updated 06:05:28 ago
         via 20.30.214.214, Ethernet5
         via 21.30.214.214, Ethernet6
>I    10.0.0.216/32 [115 pref/11 metric] updated 06:05:28 ago
         via 20.30.214.214, Ethernet5
         via 21.30.214.214, Ethernet6
>I    10.0.0.217/32 [115 pref/1 metric] updated 00:10:44 ago
         via 20.30.217.217, Ethernet4
>I    10.0.0.221/32 [115 pref/1 metric] updated 00:26:39 ago
         via 20.30.221.221, Ethernet15
>I    10.0.1.179/32 [115 pref/1 metric] updated 02:44:19 ago
         via 20.30.179.179, Ethernet40
>I    20.32.175.0/24 [115 pref/11 metric] updated 00:00:18 ago
         via 20.30.32.32, Ethernet2
>I    20.53.175.0/24 [115 pref/11 metric] updated 00:11:31 ago
         via 20.30.53.53, Ethernet13
>I    20.66.175.0/24 [115 pref/11 metric] updated 02:10:23 ago
         via 20.30.66.66, Ethernet31
>I    20.72.175.0/24 [115 pref/11 metric] updated 02:10:23 ago
         via 20.30.72.72, Ethernet9
>I    20.84.175.0/24 [115 pref/21 metric] updated 00:00:18 ago
         via 20.30.32.32, Ethernet2
         via 20.30.53.53, Ethernet13
         via 20.30.66.66, Ethernet31
         via 20.30.72.72, Ethernet9
         via 20.30.84.84, Ethernet12
         via 20.30.120.120, Ethernet3
         via 20.30.124.124, Ethernet17
         via 20.30.131.131, Ethernet35
>I    20.120.175.0/24 [115 pref/11 metric] updated 00:45:05 ago
         via 20.30.120.120, Ethernet3
         via 21.30.120.120, Ethernet10
>I    20.120.214.0/24 [115 pref/11 metric] updated 00:45:05 ago
         via 20.30.120.120, Ethernet3
         via 21.30.120.120, Ethernet10
>I    20.120.217.0/24 [115 pref/1 metric] updated 00:45:05 ago
         via 20.30.120.120, Ethernet3
         via 21.30.120.120, Ethernet10
>I    20.124.175.0/24 [115 pref/11 metric] updated 00:19:00 ago
         via 20.30.124.124, Ethernet17
         via 21.30.124.124, Ethernet18
>I    20.128.175.0/24 [115 pref/11 metric] updated 00:32:36 ago
         via 21.30.128.128, Ethernet20
>I    20.131.175.0/24 [115 pref/11 metric] updated 08:24:22 ago
         via 20.30.131.131, Ethernet35
>I    20.156.175.0/24 [115 pref/11 metric] updated 02:31:00 ago
         via 20.30.156.156, Ethernet11
         via 21.30.156.156, Ethernet21
>I    20.175.179.0/24 [115 pref/11 metric] updated 02:44:19 ago
         via 20.30.179.179, Ethernet40
>I    20.175.184.0/24 [115 pref/21 metric] updated 00:00:18 ago
         via 20.30.32.32, Ethernet2
         via 20.30.53.53, Ethernet13
         via 20.30.66.66, Ethernet31
         via 20.30.72.72, Ethernet9
         via 20.30.84.84, Ethernet12
         via 20.30.120.120, Ethernet3
         via 20.30.124.124, Ethernet17
         via 20.30.131.131, Ethernet35
>I    20.175.214.0/24 [115 pref/21 metric] updated 00:00:18 ago
         via 20.30.32.32, Ethernet2
         via 20.30.53.53, Ethernet13
         via 20.30.66.66, Ethernet31
         via 20.30.72.72, Ethernet9
         via 20.30.84.84, Ethernet12
         via 20.30.120.120, Ethernet3
         via 20.30.124.124, Ethernet17
         via 20.30.131.131, Ethernet35
>I    20.175.217.0/24 [115 pref/11 metric] updated 00:10:44 ago
         via 20.30.217.217, Ethernet4
>I    20.175.221.0/24 [115 pref/11 metric] updated 00:26:39 ago
         via 20.30.221.221, Ethernet15
>I    20.214.216.0/24 [115 pref/11 metric] updated 06:05:28 ago
         via 20.30.214.214, Ethernet5
         via 21.30.214.214, Ethernet6
>I    192.168.20.0/23 [115 pref/1 metric] updated 00:45:05 ago
         via 20.30.120.120, Ethernet3
         via 21.30.120.120, Ethernet10
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
>C    2001:0:30:32::/64 [0 pref/0 metric] updated 00:00:28 ago
         via Ethernet2, directly connected
>C    2001:0:30:53::/64 [0 pref/0 metric] updated 00:11:34 ago
         via Ethernet13, directly connected
>C    2001:0:30:66::/64 [0 pref/0 metric] updated 02:10:36 ago
         via Ethernet31, directly connected
>C    2001:0:30:72::/64 [0 pref/0 metric] updated 02:10:36 ago
         via Ethernet9, directly connected
>C    2001:0:30:84::/64 [0 pref/0 metric] updated 01:25:42 ago
         via Ethernet12, directly connected
>C    2001:0:30:120::/64 [0 pref/0 metric] updated 00:45:15 ago
         via Ethernet3, directly connected
>C    2001:0:30:124::/64 [0 pref/0 metric] updated 00:19:02 ago
         via Ethernet17, directly connected
>C    2001:0:30:131::/64 [0 pref/0 metric] updated 1d02h ago
         via Ethernet35, directly connected
>C    2001:0:30:156::/64 [0 pref/0 metric] updated 02:39:30 ago
         via Ethernet11, directly connected
>C    2001:0:30:179::/64 [0 pref/0 metric] updated 02:44:28 ago
         via Ethernet40, directly connected
>C    2001:0:30:184::/64 [0 pref/0 metric] updated 1d02h ago
         via Ethernet7, directly connected
>C    2001:0:30:214::/64 [0 pref/0 metric] updated 07:12:30 ago
         via Ethernet5, directly connected
>C    2001:0:30:217::/64 [0 pref/0 metric] updated 00:10:53 ago
         via Ethernet4, directly connected
>C    2001:0:30:221::/64 [0 pref/0 metric] updated 00:33:31 ago
         via Ethernet15, directly connected
>C    2002::30/128 [0 pref/0 metric] updated 1d02h ago
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
>P    ::/96 [1 pref/0 metric] updated 1d02h ago
         via Null0, directly connected [NF]
>P    ::ffff:127.0.0.0/104 [1 pref/0 metric] updated 1d02h ago
         via :: [1 pref/1 metric] type ipv6
            via , directly connected
>P    fe80::/10 [1 pref/0 metric] updated 1d02h ago
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
>I    2000::214/128 [115 pref/30 metric] updated 00:00:19 ago
         via fe80::5e07:58ff:fea3:aaa, Ethernet13
         via fe80::d248:a1ff:feba:3c61, Ethernet11
         via fe80::c214:b8ff:fe21:9790, Ethernet4
         via fe80::5a70:7fff:fe9f:c403, Ethernet12
         via fe80::d6af:f7ff:fe2f:1396, Ethernet2
         via fe80::be31:e2ff:fee1:ec2c, Ethernet3
>I    2001:0:32:175::/64 [115 pref/20 metric] updated 00:00:19 ago
         via fe80::d6af:f7ff:fe2f:1396, Ethernet2
>I    2001:0:53:175::/64 [115 pref/20 metric] updated 00:11:32 ago
         via fe80::5e07:58ff:fea3:aaa, Ethernet13
>I    2001:0:66:175::/64 [115 pref/30 metric] updated 00:00:19 ago
         via fe80::5e07:58ff:fea3:aaa, Ethernet13
         via fe80::d248:a1ff:feba:3c61, Ethernet11
         via fe80::c214:b8ff:fe21:9790, Ethernet4
         via fe80::5a70:7fff:fe9f:c403, Ethernet12
         via fe80::d6af:f7ff:fe2f:1396, Ethernet2
         via fe80::be31:e2ff:fee1:ec2c, Ethernet3
>I    2001:0:72:175::/64 [115 pref/30 metric] updated 00:00:19 ago
         via fe80::5e07:58ff:fea3:aaa, Ethernet13
         via fe80::d248:a1ff:feba:3c61, Ethernet11
         via fe80::c214:b8ff:fe21:9790, Ethernet4
         via fe80::5a70:7fff:fe9f:c403, Ethernet12
         via fe80::d6af:f7ff:fe2f:1396, Ethernet2
         via fe80::be31:e2ff:fee1:ec2c, Ethernet3
>I    2001:0:84:175::/64 [115 pref/20 metric] updated 01:25:40 ago
         via fe80::5a70:7fff:fe9f:c403, Ethernet12
>I    2001:0:120:175::/64 [115 pref/20 metric] updated 00:45:06 ago
         via fe80::be31:e2ff:fee1:ec2c, Ethernet3
>I    2001:0:120:214::/64 [115 pref/20 metric] updated 00:45:06 ago
         via fe80::be31:e2ff:fee1:ec2c, Ethernet3
>I    2001:0:120:217::/64 [115 pref/10 metric] updated 00:45:06 ago
         via fe80::be31:e2ff:fee1:ec2c, Ethernet3
>I    2001:0:128:175::/64 [115 pref/30 metric] updated 00:00:19 ago
         via fe80::5e07:58ff:fea3:aaa, Ethernet13
         via fe80::d248:a1ff:feba:3c61, Ethernet11
         via fe80::c214:b8ff:fe21:9790, Ethernet4
         via fe80::5a70:7fff:fe9f:c403, Ethernet12
         via fe80::d6af:f7ff:fe2f:1396, Ethernet2
         via fe80::be31:e2ff:fee1:ec2c, Ethernet3
>I    2001:0:131:175::/64 [115 pref/30 metric] updated 00:00:19 ago
         via fe80::5e07:58ff:fea3:aaa, Ethernet13
         via fe80::d248:a1ff:feba:3c61, Ethernet11
         via fe80::c214:b8ff:fe21:9790, Ethernet4
         via fe80::5a70:7fff:fe9f:c403, Ethernet12
         via fe80::d6af:f7ff:fe2f:1396, Ethernet2
         via fe80::be31:e2ff:fee1:ec2c, Ethernet3
>I    2001:0:156:175::/64 [115 pref/20 metric] updated 02:38:47 ago
         via fe80::d248:a1ff:feba:3c61, Ethernet11
>I    2001:0:175::/64 [115 pref/30 metric] updated 00:00:19 ago
         via fe80::5e07:58ff:fea3:aaa, Ethernet13
         via fe80::d248:a1ff:feba:3c61, Ethernet11
         via fe80::c214:b8ff:fe21:9790, Ethernet4
         via fe80::5a70:7fff:fe9f:c403, Ethernet12
         via fe80::d6af:f7ff:fe2f:1396, Ethernet2
         via fe80::be31:e2ff:fee1:ec2c, Ethernet3
>I    2001:0:175:184::/64 [115 pref/30 metric] updated 00:00:19 ago
         via fe80::5e07:58ff:fea3:aaa, Ethernet13
         via fe80::d248:a1ff:feba:3c61, Ethernet11
         via fe80::c214:b8ff:fe21:9790, Ethernet4
         via fe80::5a70:7fff:fe9f:c403, Ethernet12
         via fe80::d6af:f7ff:fe2f:1396, Ethernet2
         via fe80::be31:e2ff:fee1:ec2c, Ethernet3
>I    2001:0:175:214::/64 [115 pref/30 metric] updated 00:00:19 ago
         via fe80::5e07:58ff:fea3:aaa, Ethernet13
         via fe80::d248:a1ff:feba:3c61, Ethernet11
         via fe80::c214:b8ff:fe21:9790, Ethernet4
         via fe80::5a70:7fff:fe9f:c403, Ethernet12
         via fe80::d6af:f7ff:fe2f:1396, Ethernet2
         via fe80::be31:e2ff:fee1:ec2c, Ethernet3
>I    2001:0:175:217::/64 [115 pref/20 metric] updated 00:10:45 ago
         via fe80::c214:b8ff:fe21:9790, Ethernet4
>I    2001:0:175:221::/64 [115 pref/30 metric] updated 00:00:19 ago
         via fe80::5e07:58ff:fea3:aaa, Ethernet13
         via fe80::d248:a1ff:feba:3c61, Ethernet11
         via fe80::c214:b8ff:fe21:9790, Ethernet4
         via fe80::5a70:7fff:fe9f:c403, Ethernet12
         via fe80::d6af:f7ff:fe2f:1396, Ethernet2
         via fe80::be31:e2ff:fee1:ec2c, Ethernet3
>I    2001:0:214:216::/64 [115 pref/40 metric] updated 00:00:19 ago
         via fe80::5e07:58ff:fea3:aaa, Ethernet13
         via fe80::d248:a1ff:feba:3c61, Ethernet11
         via fe80::c214:b8ff:fe21:9790, Ethernet4
         via fe80::5a70:7fff:fe9f:c403, Ethernet12
         via fe80::d6af:f7ff:fe2f:1396, Ethernet2
         via fe80::be31:e2ff:fee1:ec2c, Ethernet3
>I    2001:1:30:120::/64 [115 pref/25 metric] updated 00:45:06 ago
         via fe80::be31:e2ff:fee1:ec2c, Ethernet3
>I    2002::32/128 [115 pref/20 metric] updated 00:00:19 ago
         via fe80::d6af:f7ff:fe2f:1396, Ethernet2
>I    2002::53/128 [115 pref/10 metric] updated 00:11:32 ago
         via fe80::5e07:58ff:fea3:aaa, Ethernet13
>I    2002::120/128 [115 pref/10 metric] updated 00:45:06 ago
         via fe80::be31:e2ff:fee1:ec2c, Ethernet3
>I    2002::156/128 [115 pref/10 metric] updated 02:38:47 ago
         via fe80::d248:a1ff:feba:3c61, Ethernet11
>I    2002::175/128 [115 pref/20 metric] updated 00:00:19 ago
         via fe80::5e07:58ff:fea3:aaa, Ethernet13
         via fe80::d248:a1ff:feba:3c61, Ethernet11
         via fe80::c214:b8ff:fe21:9790, Ethernet4
         via fe80::5a70:7fff:fe9f:c403, Ethernet12
         via fe80::d6af:f7ff:fe2f:1396, Ethernet2
         via fe80::be31:e2ff:fee1:ec2c, Ethernet3
>I    2002::216/128 [115 pref/40 metric] updated 00:00:19 ago
         via fe80::5e07:58ff:fea3:aaa, Ethernet13
         via fe80::d248:a1ff:feba:3c61, Ethernet11
         via fe80::c214:b8ff:fe21:9790, Ethernet4
         via fe80::5a70:7fff:fe9f:c403, Ethernet12
         via fe80::d6af:f7ff:fe2f:1396, Ethernet2
         via fe80::be31:e2ff:fee1:ec2c, Ethernet3
>I    2002::217/128 [115 pref/10 metric] updated 00:10:45 ago
         via fe80::c214:b8ff:fe21:9790, Ethernet4
```

## show platform sand l3 summary

```text
Number of vrfs: 4

Ipv4:
  Routes:       187  backlog:  0  unprogrammed:  0
  Adjacencies:  288  backlog:  0  unprogrammed:  0
Ipv6:
  Routes:       71   backlog:  0  unprogrammed:  0
  Adjacencies:  288  backlog:  0  unprogrammed:  0
Mpls:
  Routes:       74  backlog:  0  unprogrammed:  0
  Adjacencies:  24  backlog:  0  unprogrammed:  0

Jericho2 Ip Fecs:
  Non-ecmp fecs:  4219  ecmp fecs:  11  fec entries:  4257
Jericho2 Mpls Fecs:
  Non-ecmp fecs:  21  ecmp fecs:  3  fec entries:  42
Jericho2 Vxlan Tunnel Fecs:
  Non-ecmp fecs:  0  ecmp fecs:  0  fec entries:  0
  Number of vxlan tunnels configured: 0

Jericho2 Lpm Routes:
  Routes:   187  unprogrammed:   0   
  Routes6:  71   unprogrammed6:  0   
  Backlog:  0  

Jericho2 Lpm:
  TCAM entries used:   4   Percent free:  99  ADS2 entries used:   13  Percent free:  99
  Pivot buckets used:  6   Rows used:     2   Entries Per Bucket:  2   Percent free:  99
  Route buckets used:  44  Rows used:     6   Entries Per Bucket:  5   Percent free:  99

Lem:
  IPv4  Host in Lem:            disabled
  IPv4  Prefix-lengths in Lem:  None    
  IPv6  Host in Lem:            disabled
  IPv6  Prefix-lengths in Lem:  None    
  Number of downloads:        0
  Number of overflow events:  0

Egress Arp rewrite entries in use (in each fap):
  FixedSystem: 19
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
  FixedSystem: 4205

Jericho2 Fec:
  Maximum FEC hierarchy levels:  2
  ReusedEcmp:  248  allocs:  2211  frees:  2056  shuffles:  0  cmds:  0
  Zombies:     0    purges:    0
  Quarantine:  0/0  shuffles:  0  deletes:  0   
  Preserved FECs: 0
    First FEC preserved: never
    Last FEC preserved: never
  Fec insertion failures:  0
  Level1  Fecs:
    Non-ecmp fecs:            0    ecmp fecs:            1 
    Non-ecmp (Percent free):  100  ecmp (Percent free):  99
  Level2  Fecs:
    Non-ecmp fecs:            84  ecmp fecs:            0  
    Non-ecmp (Percent free):  99  ecmp (Percent free):  100
  Level3  Fecs:
    Non-ecmp fecs:            316  ecmp fecs:            14
    Non-ecmp (Percent free):  99   ecmp (Percent free):  99

Lpm Detail:
  Requests:  4244  cleanses:  682  batches:  682  avg batch size:  6

Jericho Arp:
  ArpTable writes:      45571   queued      0   
  IngressTable writes:  109379  queued      0   
  Coprocessors:         1       in CmdRing

Tunnel Counter Status
  Number of MPLS tunnels:                  90   
  Number of uncountable MPLS tunnels:      90   
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
|0  |0.0.0.0/8         |DROP | DROP               |0    |  -     |                   |  -  |318922|   -   
|0  |10.0.0.30/32      |TRAP | CoppSystemIpUcast  |0    |  -     | Receive           |  -  |314667|   -   
|0  |10.0.0.32/32      |ROUTE| Et2                |1018 |103425  | d4:af:f7:2f:13:96 |  -  |319054|   -   
|0  |10.0.0.53/32      |ROUTE| Et13               |1026 |103429  | 5c:07:58:a3:0a:aa |  -  |318988|   -   
|0  |10.0.0.66/32      |ROUTE| Et31               |1020 |103436  | e4:6d:7f:e3:c8:0a |  -  |318838|   -   
|0  |10.0.0.72/32      |ROUTE| Et9                |1009 |103421  | e0:9b:27:c4:c5:84 |  -  |318860|   -   
|0  |10.0.0.84/32      |ROUTE| Et12               |1014 |103430  | 58:70:7f:9f:c4:03 |  -  |319030|   -   
|0  |10.0.0.120/32     |ROUTE| Et3                |1017 |103431  | bc:31:e2:e1:ec:2c |24597|318798|   -   
|0  |10.0.0.120/32     |ROUTE| Et10               |1029 |103423  | bc:31:e2:e1:ec:32 |24597|318799|   -   
|0  |10.0.0.120/32     |ROUTE| Et10               |1029 |103423  | bc:31:e2:e1:ec:32 |24597|318800|   -   
|0  |10.0.0.120/32     |ROUTE| Et3                |1017 |103431  | bc:31:e2:e1:ec:2c |24597|318801|   -   
|0  |10.0.0.124/32     |ROUTE| Et18               |1013 |103450  | 64:6d:4e:32:e1:23 |24577|319158|   -   
|0  |10.0.0.124/32     |ROUTE| Et17               |1016 |103448  | 64:6d:4e:32:e1:22 |24577|319159|   -   
|0  |10.0.0.124/32     |ROUTE| Et17               |1016 |103448  | 64:6d:4e:32:e1:22 |24577|319160|   -   
|0  |10.0.0.124/32     |ROUTE| Et18               |1013 |103450  | 64:6d:4e:32:e1:23 |24577|319161|   -   
|0  |10.0.0.128/32     |ROUTE| Et20               |1025 |103475  | 60:53:75:13:ba:dd |  -  |318944|   -   
|0  |10.0.0.131/32     |ROUTE| Et35               |1012 |103426  | 40:a6:b7:94:34:cb |  -  |318868|   -   
|0  |10.0.0.156/32     |ROUTE| Et11               |1019 |103447  | d0:48:a1:ba:3c:61 |24582|318844|   -   
|0  |10.0.0.156/32     |ROUTE| Et21               |1027 |103453  | d0:48:a1:ba:3c:63 |24582|318845|   -   
|0  |10.0.0.156/32     |ROUTE| Et21               |1027 |103453  | d0:48:a1:ba:3c:63 |24582|318846|   -   
|0  |10.0.0.156/32     |ROUTE| Et11               |1019 |103447  | d0:48:a1:ba:3c:61 |24582|318847|   -   
|0  |10.0.0.175/32     |ROUTE| Et3                |1017 |103431  | bc:31:e2:e1:ec:2c |24591|319188|   -   
|0  |10.0.0.175/32     |ROUTE| Et35               |1012 |103426  | 40:a6:b7:94:34:cb |24591|319189|   -   
|0  |10.0.0.175/32     |ROUTE| Et35               |1012 |103426  | 40:a6:b7:94:34:cb |24591|319190|   -   
|0  |10.0.0.175/32     |ROUTE| Et31               |1020 |103436  | e4:6d:7f:e3:c8:0a |24591|319191|   -   
|0  |10.0.0.175/32     |ROUTE| Et31               |1020 |103436  | e4:6d:7f:e3:c8:0a |24591|319192|   -   
|0  |10.0.0.175/32     |ROUTE| Et12               |1014 |103430  | 58:70:7f:9f:c4:03 |24591|319193|   -   
|0  |10.0.0.175/32     |ROUTE| Et12               |1014 |103430  | 58:70:7f:9f:c4:03 |24591|319194|   -   
|0  |10.0.0.175/32     |ROUTE| Et9                |1009 |103421  | e0:9b:27:c4:c5:84 |24591|319195|   -   
|0  |10.0.0.175/32     |ROUTE| Et9                |1009 |103421  | e0:9b:27:c4:c5:84 |24591|319196|   -   
|0  |10.0.0.175/32     |ROUTE| Et2                |1018 |103425  | d4:af:f7:2f:13:96 |24591|319197|   -   
|0  |10.0.0.175/32     |ROUTE| Et2                |1018 |103425  | d4:af:f7:2f:13:96 |24591|319198|   -   
|0  |10.0.0.175/32     |ROUTE| Et17               |1016 |103448  | 64:6d:4e:32:e1:22 |24591|319199|   -   
|0  |10.0.0.175/32     |ROUTE| Et17               |1016 |103448  | 64:6d:4e:32:e1:22 |24591|319200|   -   
|0  |10.0.0.175/32     |ROUTE| Et13               |1026 |103429  | 5c:07:58:a3:0a:aa |24591|319201|   -   
|0  |10.0.0.175/32     |ROUTE| Et13               |1026 |103429  | 5c:07:58:a3:0a:aa |24591|319202|   -   
|0  |10.0.0.175/32     |ROUTE| Et3                |1017 |103431  | bc:31:e2:e1:ec:2c |24591|319203|   -   
|0  |10.0.0.179/32     |ROUTE| Et40               |1015 |103427  | e8:24:a6:96:05:48 |  -  |318910|   -   
|0  |10.0.0.214/32     |ROUTE| Et5                |1008 |103428  | 18:5b:00:61:ac:6f |24580|319014|   -   
|0  |10.0.0.214/32     |ROUTE| Et6                |1022 |103438  | 18:5b:00:61:ac:73 |24580|319015|   -   
|0  |10.0.0.214/32     |ROUTE| Et6                |1022 |103438  | 18:5b:00:61:ac:73 |24580|319016|   -   
|0  |10.0.0.214/32     |ROUTE| Et5                |1008 |103428  | 18:5b:00:61:ac:6f |24580|319017|   -   
|0  |10.0.0.216/32     |ROUTE| Et5                |1008 |103428  | 18:5b:00:61:ac:6f |24580|319014|   -   
|0  |10.0.0.216/32     |ROUTE| Et6                |1022 |103438  | 18:5b:00:61:ac:73 |24580|319015|   -   
|0  |10.0.0.216/32     |ROUTE| Et6                |1022 |103438  | 18:5b:00:61:ac:73 |24580|319016|   -   
|0  |10.0.0.216/32     |ROUTE| Et5                |1008 |103428  | 18:5b:00:61:ac:6f |24580|319017|   -   
|0  |10.0.0.217/32     |ROUTE| Et4                |1007 |103422  | c0:14:b8:21:97:90 |  -  |319066|   -   
|0  |10.0.0.221/32     |ROUTE| Et15               |1006 |103437  | 30:c5:07:84:3e:79 |  -  |318890|   -   
|0  |10.0.1.179/32     |ROUTE| Et40               |1015 |103427  | e8:24:a6:96:05:48 |  -  |318910|   -   
|0  |20.30.32.0/32     |TRAP | CoppSystemIpBcast  |0    |  -     | BcastReceive      |  -  |314666|   -   
|0  |20.30.32.30/32    |TRAP | CoppSystemIpUcast  |0    |  -     | Receive           |  -  |314667|   -   
|0  |20.30.32.32/32    |ROUTE| Et2                |1018 |103425  | d4:af:f7:2f:13:96 |  -  |318882|   -   
|0  |20.30.32.255/32   |TRAP | CoppSystemIpBcast  |0    |  -     | BcastReceive      |  -  |314666|   -   
|0  |20.30.32.0/24     |TRAP | CoppSystemL3DstMiss|1018 |1018    | ArpTrap           |  -  |315689|   -   
|0  |20.30.53.0/32     |TRAP | CoppSystemIpBcast  |0    |  -     | BcastReceive      |  -  |314666|   -   
|0  |20.30.53.30/32    |TRAP | CoppSystemIpUcast  |0    |  -     | Receive           |  -  |314667|   -   
|0  |20.30.53.53/32    |ROUTE| Et13               |1026 |103429  | 5c:07:58:a3:0a:aa |  -  |318884|   -   
|0  |20.30.53.255/32   |TRAP | CoppSystemIpBcast  |0    |  -     | BcastReceive      |  -  |314666|   -   
|0  |20.30.53.0/24     |TRAP | CoppSystemL3DstMiss|1026 |1026    | ArpTrap           |  -  |315697|   -   
|0  |20.30.66.0/32     |TRAP | CoppSystemIpBcast  |0    |  -     | BcastReceive      |  -  |314666|   -   
|0  |20.30.66.30/32    |TRAP | CoppSystemIpUcast  |0    |  -     | Receive           |  -  |314667|   -   
|0  |20.30.66.66/32    |ROUTE| Et31               |1020 |103436  | e4:6d:7f:e3:c8:0a |  -  |318908|   -   
|0  |20.30.66.255/32   |TRAP | CoppSystemIpBcast  |0    |  -     | BcastReceive      |  -  |314666|   -   
|0  |20.30.66.0/24     |TRAP | CoppSystemL3DstMiss|1020 |1020    | ArpTrap           |  -  |315691|   -   
|0  |20.30.72.0/32     |TRAP | CoppSystemIpBcast  |0    |  -     | BcastReceive      |  -  |314666|   -   
|0  |20.30.72.30/32    |TRAP | CoppSystemIpUcast  |0    |  -     | Receive           |  -  |314667|   -   
|0  |20.30.72.72/32    |ROUTE| Et9                |1009 |103421  | e0:9b:27:c4:c5:84 |  -  |318864|   -   
|0  |20.30.72.255/32   |TRAP | CoppSystemIpBcast  |0    |  -     | BcastReceive      |  -  |314666|   -   
|0  |20.30.72.0/24     |TRAP | CoppSystemL3DstMiss|1009 |1009    | ArpTrap           |  -  |315680|   -   
|0  |20.30.84.0/32     |TRAP | CoppSystemIpBcast  |0    |  -     | BcastReceive      |  -  |314666|   -   
|0  |20.30.84.30/32    |TRAP | CoppSystemIpUcast  |0    |  -     | Receive           |  -  |314667|   -   
|0  |20.30.84.84/32    |ROUTE| Et12               |1014 |103430  | 58:70:7f:9f:c4:03 |  -  |318776|   -   
|0  |20.30.84.255/32   |TRAP | CoppSystemIpBcast  |0    |  -     | BcastReceive      |  -  |314666|   -   
|0  |20.30.84.0/24     |TRAP | CoppSystemL3DstMiss|1014 |1014    | ArpTrap           |  -  |315685|   -   
|0  |20.30.120.0/32    |TRAP | CoppSystemIpBcast  |0    |  -     | BcastReceive      |  -  |314666|   -   
|0  |20.30.120.30/32   |TRAP | CoppSystemIpUcast  |0    |  -     | Receive           |  -  |314667|   -   
|0  |20.30.120.120/32  |ROUTE| Et3                |1017 |103431  | bc:31:e2:e1:ec:2c |  -  |319056|   -   
|0  |20.30.120.255/32  |TRAP | CoppSystemIpBcast  |0    |  -     | BcastReceive      |  -  |314666|   -   
|0  |20.30.120.0/24    |TRAP | CoppSystemL3DstMiss|1017 |1017    | ArpTrap           |  -  |315688|   -   
|0  |20.30.124.0/32    |TRAP | CoppSystemIpBcast  |0    |  -     | BcastReceive      |  -  |314666|   -   
|0  |20.30.124.30/32   |TRAP | CoppSystemIpUcast  |0    |  -     | Receive           |  -  |314667|   -   
|0  |20.30.124.124/32  |ROUTE| Et17               |1016 |103448  | 64:6d:4e:32:e1:22 |  -  |318936|   -   
|0  |20.30.124.255/32  |TRAP | CoppSystemIpBcast  |0    |  -     | BcastReceive      |  -  |314666|   -   
|0  |20.30.124.0/24    |TRAP | CoppSystemL3DstMiss|1016 |1016    | ArpTrap           |  -  |315687|   -   
|0  |20.30.131.0/32    |TRAP | CoppSystemIpBcast  |0    |  -     | BcastReceive      |  -  |314666|   -   
|0  |20.30.131.30/32   |TRAP | CoppSystemIpUcast  |0    |  -     | Receive           |  -  |314667|   -   
|0  |20.30.131.131/32  |ROUTE| Et35               |1012 |103426  | 40:a6:b7:94:34:cb |  -  |318928|   -   
|0  |20.30.131.255/32  |TRAP | CoppSystemIpBcast  |0    |  -     | BcastReceive      |  -  |314666|   -   
|0  |20.30.131.0/24    |TRAP | CoppSystemL3DstMiss|1012 |1012    | ArpTrap           |  -  |315683|   -   
|0  |20.30.156.0/32    |TRAP | CoppSystemIpBcast  |0    |  -     | BcastReceive      |  -  |314666|   -   
|0  |20.30.156.30/32   |TRAP | CoppSystemIpUcast  |0    |  -     | Receive           |  -  |314667|   -   
|0  |20.30.156.156/32  |ROUTE| Et11               |1019 |103447  | d0:48:a1:ba:3c:61 |  -  |318770|   -   
|0  |20.30.156.255/32  |TRAP | CoppSystemIpBcast  |0    |  -     | BcastReceive      |  -  |314666|   -   
|0  |20.30.156.0/24    |TRAP | CoppSystemL3DstMiss|1019 |1019    | ArpTrap           |  -  |315690|   -   
|0  |20.30.179.0/32    |TRAP | CoppSystemIpBcast  |0    |  -     | BcastReceive      |  -  |314666|   -   
|0  |20.30.179.30/32   |TRAP | CoppSystemIpUcast  |0    |  -     | Receive           |  -  |314667|   -   
|0  |20.30.179.179/32  |ROUTE| Et40               |1015 |103427  | e8:24:a6:96:05:48 |  -  |319072|   -   
|0  |20.30.179.255/32  |TRAP | CoppSystemIpBcast  |0    |  -     | BcastReceive      |  -  |314666|   -   
|0  |20.30.179.0/24    |TRAP | CoppSystemL3DstMiss|1015 |1015    | ArpTrap           |  -  |315686|   -   
|0  |20.30.184.0/32    |TRAP | CoppSystemIpBcast  |0    |  -     | BcastReceive      |  -  |314666|   -   
|0  |20.30.184.30/32   |TRAP | CoppSystemIpUcast  |0    |  -     | Receive           |  -  |314667|   -   
|0  |20.30.184.255/32  |TRAP | CoppSystemIpBcast  |0    |  -     | BcastReceive      |  -  |314666|   -   
|0  |20.30.184.0/24    |TRAP | CoppSystemL3DstMiss|1010 |1010    | ArpTrap           |  -  |315681|   -   
|0  |20.30.214.0/32    |TRAP | CoppSystemIpBcast  |0    |  -     | BcastReceive      |  -  |314666|   -   
|0  |20.30.214.30/32   |TRAP | CoppSystemIpUcast  |0    |  -     | Receive           |  -  |314667|   -   
|0  |20.30.214.214/32  |ROUTE| Et5                |1008 |103428  | 18:5b:00:61:ac:6f |  -  |318926|   -   
|0  |20.30.214.255/32  |TRAP | CoppSystemIpBcast  |0    |  -     | BcastReceive      |  -  |314666|   -   
|0  |20.30.214.0/24    |TRAP | CoppSystemL3DstMiss|1008 |1008    | ArpTrap           |  -  |315679|   -   
|0  |20.30.217.0/32    |TRAP | CoppSystemIpBcast  |0    |  -     | BcastReceive      |  -  |314666|   -   
|0  |20.30.217.30/32   |TRAP | CoppSystemIpUcast  |0    |  -     | Receive           |  -  |314667|   -   
|0  |20.30.217.217/32  |ROUTE| Et4                |1007 |103422  | c0:14:b8:21:97:90 |  -  |318962|   -   
|0  |20.30.217.255/32  |TRAP | CoppSystemIpBcast  |0    |  -     | BcastReceive      |  -  |314666|   -   
|0  |20.30.217.0/24    |TRAP | CoppSystemL3DstMiss|1007 |1007    | ArpTrap           |  -  |315678|   -   
|0  |20.30.221.0/32    |TRAP | CoppSystemIpBcast  |0    |  -     | BcastReceive      |  -  |314666|   -   
|0  |20.30.221.30/32   |TRAP | CoppSystemIpUcast  |0    |  -     | Receive           |  -  |314667|   -   
|0  |20.30.221.221/32  |ROUTE| Et15               |1006 |103437  | 30:c5:07:84:3e:79 |  -  |318888|   -   
|0  |20.30.221.255/32  |TRAP | CoppSystemIpBcast  |0    |  -     | BcastReceive      |  -  |314666|   -   
|0  |20.30.221.0/24    |TRAP | CoppSystemL3DstMiss|1006 |1006    | ArpTrap           |  -  |315677|   -   
|0  |20.32.175.0/24    |ROUTE| Et2                |1018 |103425  | d4:af:f7:2f:13:96 |  -  |319054|   -   
|0  |20.53.175.0/24    |ROUTE| Et13               |1026 |103429  | 5c:07:58:a3:0a:aa |  -  |318988|   -   
|0  |20.66.175.0/24    |ROUTE| Et31               |1020 |103436  | e4:6d:7f:e3:c8:0a |  -  |318838|   -   
|0  |20.72.175.0/24    |ROUTE| Et9                |1009 |103421  | e0:9b:27:c4:c5:84 |  -  |318860|   -   
|0  |20.84.175.0/24    |ROUTE| Et3                |1017 |103431  | bc:31:e2:e1:ec:2c |24591|319188|   -   
|0  |20.84.175.0/24    |ROUTE| Et35               |1012 |103426  | 40:a6:b7:94:34:cb |24591|319189|   -   
|0  |20.84.175.0/24    |ROUTE| Et35               |1012 |103426  | 40:a6:b7:94:34:cb |24591|319190|   -   
|0  |20.84.175.0/24    |ROUTE| Et31               |1020 |103436  | e4:6d:7f:e3:c8:0a |24591|319191|   -   
|0  |20.84.175.0/24    |ROUTE| Et31               |1020 |103436  | e4:6d:7f:e3:c8:0a |24591|319192|   -   
|0  |20.84.175.0/24    |ROUTE| Et12               |1014 |103430  | 58:70:7f:9f:c4:03 |24591|319193|   -   
|0  |20.84.175.0/24    |ROUTE| Et12               |1014 |103430  | 58:70:7f:9f:c4:03 |24591|319194|   -   
|0  |20.84.175.0/24    |ROUTE| Et9                |1009 |103421  | e0:9b:27:c4:c5:84 |24591|319195|   -   
|0  |20.84.175.0/24    |ROUTE| Et9                |1009 |103421  | e0:9b:27:c4:c5:84 |24591|319196|   -   
|0  |20.84.175.0/24    |ROUTE| Et2                |1018 |103425  | d4:af:f7:2f:13:96 |24591|319197|   -   
|0  |20.84.175.0/24    |ROUTE| Et2                |1018 |103425  | d4:af:f7:2f:13:96 |24591|319198|   -   
|0  |20.84.175.0/24    |ROUTE| Et17               |1016 |103448  | 64:6d:4e:32:e1:22 |24591|319199|   -   
|0  |20.84.175.0/24    |ROUTE| Et17               |1016 |103448  | 64:6d:4e:32:e1:22 |24591|319200|   -   
|0  |20.84.175.0/24    |ROUTE| Et13               |1026 |103429  | 5c:07:58:a3:0a:aa |24591|319201|   -   
|0  |20.84.175.0/24    |ROUTE| Et13               |1026 |103429  | 5c:07:58:a3:0a:aa |24591|319202|   -   
|0  |20.84.175.0/24    |ROUTE| Et3                |1017 |103431  | bc:31:e2:e1:ec:2c |24591|319203|   -   
|0  |20.120.175.0/24   |ROUTE| Et3                |1017 |103431  | bc:31:e2:e1:ec:2c |24597|318798|   -   
|0  |20.120.175.0/24   |ROUTE| Et10               |1029 |103423  | bc:31:e2:e1:ec:32 |24597|318799|   -   
|0  |20.120.175.0/24   |ROUTE| Et10               |1029 |103423  | bc:31:e2:e1:ec:32 |24597|318800|   -   
|0  |20.120.175.0/24   |ROUTE| Et3                |1017 |103431  | bc:31:e2:e1:ec:2c |24597|318801|   -   
|0  |20.120.214.0/24   |ROUTE| Et3                |1017 |103431  | bc:31:e2:e1:ec:2c |24597|318798|   -   
|0  |20.120.214.0/24   |ROUTE| Et10               |1029 |103423  | bc:31:e2:e1:ec:32 |24597|318799|   -   
|0  |20.120.214.0/24   |ROUTE| Et10               |1029 |103423  | bc:31:e2:e1:ec:32 |24597|318800|   -   
|0  |20.120.214.0/24   |ROUTE| Et3                |1017 |103431  | bc:31:e2:e1:ec:2c |24597|318801|   -   
|0  |20.120.217.0/24   |ROUTE| Et3                |1017 |103431  | bc:31:e2:e1:ec:2c |24597|318798|   -   
|0  |20.120.217.0/24   |ROUTE| Et10               |1029 |103423  | bc:31:e2:e1:ec:32 |24597|318799|   -   
|0  |20.120.217.0/24   |ROUTE| Et10               |1029 |103423  | bc:31:e2:e1:ec:32 |24597|318800|   -   
|0  |20.120.217.0/24   |ROUTE| Et3                |1017 |103431  | bc:31:e2:e1:ec:2c |24597|318801|   -   
|0  |20.124.175.0/24   |ROUTE| Et18               |1013 |103450  | 64:6d:4e:32:e1:23 |24577|319158|   -   
|0  |20.124.175.0/24   |ROUTE| Et17               |1016 |103448  | 64:6d:4e:32:e1:22 |24577|319159|   -   
|0  |20.124.175.0/24   |ROUTE| Et17               |1016 |103448  | 64:6d:4e:32:e1:22 |24577|319160|   -   
|0  |20.124.175.0/24   |ROUTE| Et18               |1013 |103450  | 64:6d:4e:32:e1:23 |24577|319161|   -   
|0  |20.128.175.0/24   |ROUTE| Et20               |1025 |103475  | 60:53:75:13:ba:dd |  -  |318944|   -   
|0  |20.131.175.0/24   |ROUTE| Et35               |1012 |103426  | 40:a6:b7:94:34:cb |  -  |318868|   -   
|0  |20.156.175.0/24   |ROUTE| Et11               |1019 |103447  | d0:48:a1:ba:3c:61 |24582|318844|   -   
|0  |20.156.175.0/24   |ROUTE| Et21               |1027 |103453  | d0:48:a1:ba:3c:63 |24582|318845|   -   
|0  |20.156.175.0/24   |ROUTE| Et21               |1027 |103453  | d0:48:a1:ba:3c:63 |24582|318846|   -   
|0  |20.156.175.0/24   |ROUTE| Et11               |1019 |103447  | d0:48:a1:ba:3c:61 |24582|318847|   -   
|0  |20.175.179.0/24   |ROUTE| Et40               |1015 |103427  | e8:24:a6:96:05:48 |  -  |318910|   -   
|0  |20.175.184.0/24   |ROUTE| Et3                |1017 |103431  | bc:31:e2:e1:ec:2c |24591|319188|   -   
|0  |20.175.184.0/24   |ROUTE| Et35               |1012 |103426  | 40:a6:b7:94:34:cb |24591|319189|   -   
|0  |20.175.184.0/24   |ROUTE| Et35               |1012 |103426  | 40:a6:b7:94:34:cb |24591|319190|   -   
|0  |20.175.184.0/24   |ROUTE| Et31               |1020 |103436  | e4:6d:7f:e3:c8:0a |24591|319191|   -   
|0  |20.175.184.0/24   |ROUTE| Et31               |1020 |103436  | e4:6d:7f:e3:c8:0a |24591|319192|   -   
|0  |20.175.184.0/24   |ROUTE| Et12               |1014 |103430  | 58:70:7f:9f:c4:03 |24591|319193|   -   
|0  |20.175.184.0/24   |ROUTE| Et12               |1014 |103430  | 58:70:7f:9f:c4:03 |24591|319194|   -   
|0  |20.175.184.0/24   |ROUTE| Et9                |1009 |103421  | e0:9b:27:c4:c5:84 |24591|319195|   -   
|0  |20.175.184.0/24   |ROUTE| Et9                |1009 |103421  | e0:9b:27:c4:c5:84 |24591|319196|   -   
|0  |20.175.184.0/24   |ROUTE| Et2                |1018 |103425  | d4:af:f7:2f:13:96 |24591|319197|   -   
|0  |20.175.184.0/24   |ROUTE| Et2                |1018 |103425  | d4:af:f7:2f:13:96 |24591|319198|   -   
|0  |20.175.184.0/24   |ROUTE| Et17               |1016 |103448  | 64:6d:4e:32:e1:22 |24591|319199|   -   
|0  |20.175.184.0/24   |ROUTE| Et17               |1016 |103448  | 64:6d:4e:32:e1:22 |24591|319200|   -   
|0  |20.175.184.0/24   |ROUTE| Et13               |1026 |103429  | 5c:07:58:a3:0a:aa |24591|319201|   -   
|0  |20.175.184.0/24   |ROUTE| Et13               |1026 |103429  | 5c:07:58:a3:0a:aa |24591|319202|   -   
|0  |20.175.184.0/24   |ROUTE| Et3                |1017 |103431  | bc:31:e2:e1:ec:2c |24591|319203|   -   
|0  |20.175.214.0/24   |ROUTE| Et3                |1017 |103431  | bc:31:e2:e1:ec:2c |24591|319188|   -   
|0  |20.175.214.0/24   |ROUTE| Et35               |1012 |103426  | 40:a6:b7:94:34:cb |24591|319189|   -   
|0  |20.175.214.0/24   |ROUTE| Et35               |1012 |103426  | 40:a6:b7:94:34:cb |24591|319190|   -   
|0  |20.175.214.0/24   |ROUTE| Et31               |1020 |103436  | e4:6d:7f:e3:c8:0a |24591|319191|   -   
|0  |20.175.214.0/24   |ROUTE| Et31               |1020 |103436  | e4:6d:7f:e3:c8:0a |24591|319192|   -   
|0  |20.175.214.0/24   |ROUTE| Et12               |1014 |103430  | 58:70:7f:9f:c4:03 |24591|319193|   -   
|0  |20.175.214.0/24   |ROUTE| Et12               |1014 |103430  | 58:70:7f:9f:c4:03 |24591|319194|   -   
|0  |20.175.214.0/24   |ROUTE| Et9                |1009 |103421  | e0:9b:27:c4:c5:84 |24591|319195|   -   
|0  |20.175.214.0/24   |ROUTE| Et9                |1009 |103421  | e0:9b:27:c4:c5:84 |24591|319196|   -   
|0  |20.175.214.0/24   |ROUTE| Et2                |1018 |103425  | d4:af:f7:2f:13:96 |24591|319197|   -   
|0  |20.175.214.0/24   |ROUTE| Et2                |1018 |103425  | d4:af:f7:2f:13:96 |24591|319198|   -   
|0  |20.175.214.0/24   |ROUTE| Et17               |1016 |103448  | 64:6d:4e:32:e1:22 |24591|319199|   -   
|0  |20.175.214.0/24   |ROUTE| Et17               |1016 |103448  | 64:6d:4e:32:e1:22 |24591|319200|   -   
|0  |20.175.214.0/24   |ROUTE| Et13               |1026 |103429  | 5c:07:58:a3:0a:aa |24591|319201|   -   
|0  |20.175.214.0/24   |ROUTE| Et13               |1026 |103429  | 5c:07:58:a3:0a:aa |24591|319202|   -   
|0  |20.175.214.0/24   |ROUTE| Et3                |1017 |103431  | bc:31:e2:e1:ec:2c |24591|319203|   -   
|0  |20.175.217.0/24   |ROUTE| Et4                |1007 |103422  | c0:14:b8:21:97:90 |  -  |319066|   -   
|0  |20.175.221.0/24   |ROUTE| Et15               |1006 |103437  | 30:c5:07:84:3e:79 |  -  |318890|   -   
|0  |20.214.216.0/24   |ROUTE| Et5                |1008 |103428  | 18:5b:00:61:ac:6f |24580|319014|   -   
|0  |20.214.216.0/24   |ROUTE| Et6                |1022 |103438  | 18:5b:00:61:ac:73 |24580|319015|   -   
|0  |20.214.216.0/24   |ROUTE| Et6                |1022 |103438  | 18:5b:00:61:ac:73 |24580|319016|   -   
|0  |20.214.216.0/24   |ROUTE| Et5                |1008 |103428  | 18:5b:00:61:ac:6f |24580|319017|   -   
|0  |21.30.120.0/32    |TRAP | CoppSystemIpBcast  |0    |  -     | BcastReceive      |  -  |314666|   -   
|0  |21.30.120.30/32   |TRAP | CoppSystemIpUcast  |0    |  -     | Receive           |  -  |314667|   -   
|0  |21.30.120.120/32  |ROUTE| Et10               |1029 |103423  | bc:31:e2:e1:ec:32 |  -  |318924|   -   
|0  |21.30.120.255/32  |TRAP | CoppSystemIpBcast  |0    |  -     | BcastReceive      |  -  |314666|   -   
|0  |21.30.120.0/24    |TRAP | CoppSystemL3DstMiss|1029 |1029    | ArpTrap           |  -  |315700|   -   
|0  |21.30.124.0/32    |TRAP | CoppSystemIpBcast  |0    |  -     | BcastReceive      |  -  |314666|   -   
|0  |21.30.124.30/32   |TRAP | CoppSystemIpUcast  |0    |  -     | Receive           |  -  |314667|   -   
|0  |21.30.124.124/32  |ROUTE| Et18               |1013 |103450  | 64:6d:4e:32:e1:23 |  -  |318938|   -   
|0  |21.30.124.255/32  |TRAP | CoppSystemIpBcast  |0    |  -     | BcastReceive      |  -  |314666|   -   
|0  |21.30.124.0/24    |TRAP | CoppSystemL3DstMiss|1013 |1013    | ArpTrap           |  -  |315684|   -   
|0  |21.30.128.0/32    |TRAP | CoppSystemIpBcast  |0    |  -     | BcastReceive      |  -  |314666|   -   
|0  |21.30.128.30/32   |TRAP | CoppSystemIpUcast  |0    |  -     | Receive           |  -  |314667|   -   
|0  |21.30.128.128/32  |ROUTE| Et20               |1025 |103475  | 60:53:75:13:ba:dd |  -  |319070|   -   
|0  |21.30.128.255/32  |TRAP | CoppSystemIpBcast  |0    |  -     | BcastReceive      |  -  |314666|   -   
|0  |21.30.128.0/24    |TRAP | CoppSystemL3DstMiss|1025 |1025    | ArpTrap           |  -  |315696|   -   
|0  |21.30.156.0/32    |TRAP | CoppSystemIpBcast  |0    |  -     | BcastReceive      |  -  |314666|   -   
|0  |21.30.156.30/32   |TRAP | CoppSystemIpUcast  |0    |  -     | Receive           |  -  |314667|   -   
|0  |21.30.156.156/32  |ROUTE| Et21               |1027 |103453  | d0:48:a1:ba:3c:63 |  -  |318954|   -   
|0  |21.30.156.255/32  |TRAP | CoppSystemIpBcast  |0    |  -     | BcastReceive      |  -  |314666|   -   
|0  |21.30.156.0/24    |TRAP | CoppSystemL3DstMiss|1027 |1027    | ArpTrap           |  -  |315698|   -   
|0  |21.30.214.0/32    |TRAP | CoppSystemIpBcast  |0    |  -     | BcastReceive      |  -  |314666|   -   
|0  |21.30.214.30/32   |TRAP | CoppSystemIpUcast  |0    |  -     | Receive           |  -  |314667|   -   
|0  |21.30.214.214/32  |ROUTE| Et6                |1022 |103438  | 18:5b:00:61:ac:73 |  -  |318810|   -   
|0  |21.30.214.255/32  |TRAP | CoppSystemIpBcast  |0    |  -     | BcastReceive      |  -  |314666|   -   
|0  |21.30.214.0/24    |TRAP | CoppSystemL3DstMiss|1022 |1022    | ArpTrap           |  -  |315693|   -   
|0  |21.30.217.0/32    |TRAP | CoppSystemIpBcast  |0    |  -     | BcastReceive      |  -  |314666|   -   
|0  |21.30.217.30/32   |TRAP | CoppSystemIpUcast  |0    |  -     | Receive           |  -  |314667|   -   
|0  |21.30.217.217/32  |ROUTE| Et8                |1023 |103432  | c0:14:b8:21:97:94 |  -  |318866|   -   
|0  |21.30.217.255/32  |TRAP | CoppSystemIpBcast  |0    |  -     | BcastReceive      |  -  |314666|   -   
|0  |21.30.217.0/24    |TRAP | CoppSystemL3DstMiss|1023 |1023    | ArpTrap           |  -  |315694|   -   
|0  |127.0.0.0/8       |TRAP | CoppSystemL3DstMiss|0    |  -     | ArpTrap           |  -  |314671|   -   
|0  |192.168.20.0/23   |ROUTE| Et3                |1017 |103431  | bc:31:e2:e1:ec:2c |24597|318798|   -   
|0  |192.168.20.0/23   |ROUTE| Et10               |1029 |103423  | bc:31:e2:e1:ec:32 |24597|318799|   -   
|0  |192.168.20.0/23   |ROUTE| Et10               |1029 |103423  | bc:31:e2:e1:ec:32 |24597|318800|   -   
|0  |192.168.20.0/23   |ROUTE| Et3                |1017 |103431  | bc:31:e2:e1:ec:2c |24597|318801|   -   
|0  |0.0.0.0/0         |TRAP | CoppSystemL3LpmOver|0    |  -     | SlowReceive       |  -  |314669|   -   
|1  |0.0.0.0/8         |DROP | DROP               |0    |  -     |                   |  -  |318968|   -   
|1  |10.0.0.30/32      |TRAP | CoppSystemIpUcast  |0    |  -     | Receive           |  -  |314667|   -   
|1  |50.10.32.0/24     |ROUTE| FEC 318794         |0    |2097128 | 00:00:00:00:00:00 |  -  |183506|M 378528
|1  |50.10.53.0/24     |ROUTE| FEC 319052         |0    |2097123 | 00:00:00:00:00:00 |  -  |183520|M 970000
|1  |50.10.66.0/24     |ROUTE| FEC 319068         |0    |2097149 | 00:00:00:00:00:00 |  -  |183556|M 62000
|1  |50.10.72.0/24     |ROUTE| FEC 318824         |0    |2097148 | 00:00:00:00:00:00 |  -  |183538|M 62000
|1  |50.10.84.0/24     |ROUTE| FEC 319050         |0    |2097122 | 00:00:00:00:00:00 |  -  |183518|M 20084 720898
|1  |50.10.120.0/24    |ROUTE| FEC 24598          |0    |2097139 | 00:00:00:00:00:00 |  -  |183578|M 1657
|1  |50.10.131.0/24    |ROUTE| FEC 318942         |0    |2097134 | 00:00:00:00:00:00 |  -  |183530|M 18
|1  |50.10.156.0/24    |ROUTE| FEC 24587          |0    |2097138 | 00:00:00:00:00:00 |  -  |183524|M 16
|1  |50.10.179.0/24    |ROUTE| FEC 318940         |0    |2097127 | 00:00:00:00:00:00 |  -  |183560|M 16
|1  |50.10.214.0/24    |ROUTE| FEC 24581          |0    |2097150 | 00:00:00:00:00:00 |  -  |183550|M 20214 500000
|1  |50.10.217.0/24    |ROUTE| FEC 319012         |0    |2097124 | 00:00:00:00:00:00 |  -  |183510|M 20217 524287
|1  |50.10.221.0/24    |ROUTE| FEC 318828         |0    |2097141 | 00:00:00:00:00:00 |  -  |183536|M 524292
|1  |50.129.66.0/24    |ROUTE| FEC 319068         |0    |2097149 | 00:00:00:00:00:00 |  -  |183556|M 62000
|1  |50.129.72.0/24    |ROUTE| FEC 318824         |0    |2097148 | 00:00:00:00:00:00 |  -  |183538|M 62000
|1  |127.0.0.0/8       |TRAP | CoppSystemL3DstMiss|0    |  -     | ArpTrap           |  -  |314671|   -   
|1  |0.0.0.0/0         |TRAP | CoppSystemL3LpmOver|0    |  -     | SlowReceive       |  -  |314669|   -   
|2  |0.0.0.0/8         |DROP | DROP               |0    |  -     |                   |  -  |318970|   -   
|2  |10.128.0.30/32    |TRAP | CoppSystemIpUcast  |0    |  -     | Receive           |  -  |314667|   -   
|2  |50.128.32.0/24    |ROUTE| FEC 318862         |0    |2097117 | 00:00:00:00:00:00 |  -  |183540|M 378530
|2  |50.128.53.0/24    |ROUTE| FEC 318998         |0    |2097118 | 00:00:00:00:00:00 |  -  |183570|M 970002
|2  |50.128.120.0/24   |ROUTE| FEC 318950         |0    |2097120 | 00:00:00:00:00:00 |  -  |183580|M 1660
|2  |50.128.156.0/24   |ROUTE| FEC 24587          |0    |2097130 | 00:00:00:00:00:00 |  -  |183526|M 17
|2  |50.128.179.0/24   |ROUTE| FEC 319026         |0    |2097140 | 00:00:00:00:00:00 |  -  |183562|M 21
|2  |50.128.217.0/24   |ROUTE| FEC 318796         |0    |2097115 | 00:00:00:00:00:00 |  -  |183512|M 21345 524284
|2  |50.129.32.0/24    |ROUTE| FEC 319048         |0    |2097114 | 00:00:00:00:00:00 |  -  |183532|M 378530
|2  |50.129.53.0/24    |ROUTE| FEC 318854         |0    |2097132 | 00:00:00:00:00:00 |  -  |183574|M 970002
|2  |50.129.120.0/24   |ROUTE| FEC 24595          |0    |2097133 | 00:00:00:00:00:00 |  -  |183542|M 1659
|2  |50.129.156.0/24   |ROUTE| FEC 24587          |0    |2097130 | 00:00:00:00:00:00 |  -  |183528|M 17
|2  |50.129.179.0/24   |ROUTE| FEC 318964         |0    |2097112 | 00:00:00:00:00:00 |  -  |183564|M 21
|2  |50.129.217.0/24   |ROUTE| FEC 319012         |0    |2097116 | 00:00:00:00:00:00 |  -  |183514|M 21346 524284
|2  |50.129.221.0/24   |ROUTE| FEC 318948         |0    |2097151 | 00:00:00:00:00:00 |  -  |183568|M 524293
|2  |50.130.32.0/24    |ROUTE| FEC 318986         |0    |2097135 | 00:00:00:00:00:00 |  -  |183554|M 378530
|2  |50.130.53.0/24    |ROUTE| FEC 318804         |0    |2097147 | 00:00:00:00:00:00 |  -  |183572|M 970002
|2  |50.130.120.0/24   |ROUTE| FEC 24598          |0    |2097137 | 00:00:00:00:00:00 |  -  |183582|M 1658
|2  |50.130.156.0/24   |ROUTE| FEC 24587          |0    |2097130 | 00:00:00:00:00:00 |  -  |183522|M 17
|2  |50.130.179.0/24   |ROUTE| FEC 318940         |0    |2097145 | 00:00:00:00:00:00 |  -  |183544|M 21
|2  |50.130.217.0/24   |ROUTE| FEC 319010         |0    |2097119 | 00:00:00:00:00:00 |  -  |183516|M 21347 524284
|2  |127.0.0.0/8       |TRAP | CoppSystemL3DstMiss|0    |  -     | ArpTrap           |  -  |314671|   -   
|2  |0.0.0.0/0         |TRAP | CoppSystemL3LpmOver|0    |  -     | SlowReceive       |  -  |314669|   -   
|3  |0.0.0.0/8         |DROP | DROP               |0    |  -     |                   |  -  |318966|   -   
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
|24577|319158|ROUTE| Et18               |1013 |103450  | 64:6d:4e:32:e1:23 |   -   
|24577|319159|ROUTE| Et17               |1016 |103448  | 64:6d:4e:32:e1:22 |   -   
|24577|319160|ROUTE| Et17               |1016 |103448  | 64:6d:4e:32:e1:22 |   -   
|24577|319161|ROUTE| Et18               |1013 |103450  | 64:6d:4e:32:e1:23 |   -   
|24578|319102|ROUTE| Et11               |1019 |103492  | d0:48:a1:ba:3c:61 |Mswap 21249
|24578|319103|ROUTE| Et40               |1015 |103494  | e8:24:a6:96:05:48 |Mswap 21249
|24578|319104|ROUTE| Et40               |1015 |103494  | e8:24:a6:96:05:48 |Mswap 21249
|24578|319105|ROUTE| Et4                |1007 |103424  | c0:14:b8:21:97:90 |Mswap 21249
|24578|319106|ROUTE| Et4                |1007 |103424  | c0:14:b8:21:97:90 |Mswap 21249
|24578|319107|ROUTE| Et13               |1026 |103485  | 5c:07:58:a3:0a:aa |Mswap 21249
|24578|319108|ROUTE| Et13               |1026 |103485  | 5c:07:58:a3:0a:aa |Mswap 21249
|24578|319109|ROUTE| Et15               |1006 |103496  | 30:c5:07:84:3e:79 |Mswap 721249
|24578|319110|ROUTE| Et15               |1006 |103496  | 30:c5:07:84:3e:79 |Mswap 721249
|24578|319111|ROUTE| Et2                |1018 |103459  | d4:af:f7:2f:13:96 |Mswap 21249
|24578|319112|ROUTE| Et2                |1018 |103459  | d4:af:f7:2f:13:96 |Mswap 21249
|24578|319113|ROUTE| Et21               |1027 |103498  | d0:48:a1:ba:3c:63 |Mswap 21249
|24578|319114|ROUTE| Et21               |1027 |103498  | d0:48:a1:ba:3c:63 |Mswap 21249
|24578|319115|ROUTE| Et11               |1019 |103492  | d0:48:a1:ba:3c:61 |Mswap 21249
|24579|318830|ROUTE| Et11               |1019 |103447  | d0:48:a1:ba:3c:61 |   -   
|24579|318831|ROUTE| Et2                |1018 |103425  | d4:af:f7:2f:13:96 |   -   
|24579|318832|ROUTE| Et2                |1018 |103425  | d4:af:f7:2f:13:96 |   -   
|24579|318833|ROUTE| Et13               |1026 |103429  | 5c:07:58:a3:0a:aa |   -   
|24579|318834|ROUTE| Et13               |1026 |103429  | 5c:07:58:a3:0a:aa |   -   
|24579|318835|ROUTE| Et11               |1019 |103447  | d0:48:a1:ba:3c:61 |   -   
|24580|319014|ROUTE| Et5                |1008 |103428  | 18:5b:00:61:ac:6f |   -   
|24580|319015|ROUTE| Et6                |1022 |103438  | 18:5b:00:61:ac:73 |   -   
|24580|319016|ROUTE| Et6                |1022 |103438  | 18:5b:00:61:ac:73 |   -   
|24580|319017|ROUTE| Et5                |1008 |103428  | 18:5b:00:61:ac:6f |   -   
|24581|318932|ROUTE| Et5                |1008 |103428  | 18:5b:00:61:ac:6f |   -   
|24581|318933|ROUTE| Et6                |1022 |103438  | 18:5b:00:61:ac:73 |   -   
|24581|318934|ROUTE| Et6                |1022 |103438  | 18:5b:00:61:ac:73 |   -   
|24581|318935|ROUTE| Et5                |1008 |103428  | 18:5b:00:61:ac:6f |   -   
|24582|318844|ROUTE| Et11               |1019 |103447  | d0:48:a1:ba:3c:61 |   -   
|24582|318845|ROUTE| Et21               |1027 |103453  | d0:48:a1:ba:3c:63 |   -   
|24582|318846|ROUTE| Et21               |1027 |103453  | d0:48:a1:ba:3c:63 |   -   
|24582|318847|ROUTE| Et11               |1019 |103447  | d0:48:a1:ba:3c:61 |   -   
|24584|319086|ROUTE| Et2                |1018 |103445  | d4:af:f7:2f:13:96 |Mswap 20175
|24584|319087|ROUTE| Et3                |1017 |103452  | bc:31:e2:e1:ec:2c |Mswap 20175
|24584|319088|ROUTE| Et3                |1017 |103452  | bc:31:e2:e1:ec:2c |Mswap 20175
|24584|319089|ROUTE| Et31               |1020 |103454  | e4:6d:7f:e3:c8:0a |Mswap 20175
|24584|319090|ROUTE| Et31               |1020 |103454  | e4:6d:7f:e3:c8:0a |Mswap 20175
|24584|319091|ROUTE| Et9                |1009 |103467  | e0:9b:27:c4:c5:84 |Mswap 20175
|24584|319092|ROUTE| Et9                |1009 |103467  | e0:9b:27:c4:c5:84 |Mswap 20175
|24584|319093|ROUTE| Et12               |1014 |103469  | 58:70:7f:9f:c4:03 |Mswap 20175
|24584|319094|ROUTE| Et12               |1014 |103469  | 58:70:7f:9f:c4:03 |Mswap 20175
|24584|319095|ROUTE| Et13               |1026 |103443  | 5c:07:58:a3:0a:aa |Mswap 20175
|24584|319096|ROUTE| Et13               |1026 |103443  | 5c:07:58:a3:0a:aa |Mswap 20175
|24584|319097|ROUTE| Et35               |1012 |103478  | 40:a6:b7:94:34:cb |Mswap 20175
|24584|319098|ROUTE| Et35               |1012 |103478  | 40:a6:b7:94:34:cb |Mswap 20175
|24584|319099|ROUTE| Et2                |1018 |103445  | d4:af:f7:2f:13:96 |Mswap 20175
|24587|319004|ROUTE| Et11               |1019 |103447  | d0:48:a1:ba:3c:61 |   -   
|24587|319005|ROUTE| Et21               |1027 |103453  | d0:48:a1:ba:3c:63 |   -   
|24587|319006|ROUTE| Et21               |1027 |103453  | d0:48:a1:ba:3c:63 |   -   
|24587|319007|ROUTE| Et11               |1019 |103447  | d0:48:a1:ba:3c:61 |   -   
|24590|319176|ROUTE| Et3                |1017 |103431  | bc:31:e2:e1:ec:2c |   -   
|24590|319177|ROUTE| Et11               |1019 |103447  | d0:48:a1:ba:3c:61 |   -   
|24590|319178|ROUTE| Et11               |1019 |103447  | d0:48:a1:ba:3c:61 |   -   
|24590|319179|ROUTE| Et12               |1014 |103430  | 58:70:7f:9f:c4:03 |   -   
|24590|319180|ROUTE| Et12               |1014 |103430  | 58:70:7f:9f:c4:03 |   -   
|24590|319181|ROUTE| Et2                |1018 |103425  | d4:af:f7:2f:13:96 |   -   
|24590|319182|ROUTE| Et2                |1018 |103425  | d4:af:f7:2f:13:96 |   -   
|24590|319183|ROUTE| Et4                |1007 |103422  | c0:14:b8:21:97:90 |   -   
|24590|319184|ROUTE| Et4                |1007 |103422  | c0:14:b8:21:97:90 |   -   
|24590|319185|ROUTE| Et13               |1026 |103429  | 5c:07:58:a3:0a:aa |   -   
|24590|319186|ROUTE| Et13               |1026 |103429  | 5c:07:58:a3:0a:aa |   -   
|24590|319187|ROUTE| Et3                |1017 |103431  | bc:31:e2:e1:ec:2c |   -   
|24591|319188|ROUTE| Et3                |1017 |103431  | bc:31:e2:e1:ec:2c |   -   
|24591|319189|ROUTE| Et35               |1012 |103426  | 40:a6:b7:94:34:cb |   -   
|24591|319190|ROUTE| Et35               |1012 |103426  | 40:a6:b7:94:34:cb |   -   
|24591|319191|ROUTE| Et31               |1020 |103436  | e4:6d:7f:e3:c8:0a |   -   
|24591|319192|ROUTE| Et31               |1020 |103436  | e4:6d:7f:e3:c8:0a |   -   
|24591|319193|ROUTE| Et12               |1014 |103430  | 58:70:7f:9f:c4:03 |   -   
|24591|319194|ROUTE| Et12               |1014 |103430  | 58:70:7f:9f:c4:03 |   -   
|24591|319195|ROUTE| Et9                |1009 |103421  | e0:9b:27:c4:c5:84 |   -   
|24591|319196|ROUTE| Et9                |1009 |103421  | e0:9b:27:c4:c5:84 |   -   
|24591|319197|ROUTE| Et2                |1018 |103425  | d4:af:f7:2f:13:96 |   -   
|24591|319198|ROUTE| Et2                |1018 |103425  | d4:af:f7:2f:13:96 |   -   
|24591|319199|ROUTE| Et17               |1016 |103448  | 64:6d:4e:32:e1:22 |   -   
|24591|319200|ROUTE| Et17               |1016 |103448  | 64:6d:4e:32:e1:22 |   -   
|24591|319201|ROUTE| Et13               |1026 |103429  | 5c:07:58:a3:0a:aa |   -   
|24591|319202|ROUTE| Et13               |1026 |103429  | 5c:07:58:a3:0a:aa |   -   
|24591|319203|ROUTE| Et3                |1017 |103431  | bc:31:e2:e1:ec:2c |   -   
|24595|319162|ROUTE| Et21               |1027 |103471  | d0:48:a1:ba:3c:63 |Mpush 21249
|24595|319163|ROUTE| Et11               |1019 |103472  | d0:48:a1:ba:3c:61 |Mpush 21249
|24595|319164|ROUTE| Et11               |1019 |103472  | d0:48:a1:ba:3c:61 |Mpush 21249
|24595|319165|ROUTE| Et2                |1018 |103456  | d4:af:f7:2f:13:96 |Mpush 21249
|24595|319166|ROUTE| Et2                |1018 |103456  | d4:af:f7:2f:13:96 |Mpush 21249
|24595|319167|ROUTE| Et40               |1015 |103476  | e8:24:a6:96:05:48 |Mpush 21249
|24595|319168|ROUTE| Et40               |1015 |103476  | e8:24:a6:96:05:48 |Mpush 21249
|24595|319169|ROUTE| Et13               |1026 |103486  | 5c:07:58:a3:0a:aa |Mpush 21249
|24595|319170|ROUTE| Et13               |1026 |103486  | 5c:07:58:a3:0a:aa |Mpush 21249
|24595|319171|ROUTE| Et4                |1007 |103439  | c0:14:b8:21:97:90 |Mpush 21249
|24595|319172|ROUTE| Et4                |1007 |103439  | c0:14:b8:21:97:90 |Mpush 21249
|24595|319173|ROUTE| Et15               |1006 |103479  | 30:c5:07:84:3e:79 |Mpush 721249
|24595|319174|ROUTE| Et15               |1006 |103479  | 30:c5:07:84:3e:79 |Mpush 721249
|24595|319175|ROUTE| Et21               |1027 |103471  | d0:48:a1:ba:3c:63 |Mpush 21249
|24597|318798|ROUTE| Et3                |1017 |103431  | bc:31:e2:e1:ec:2c |   -   
|24597|318799|ROUTE| Et10               |1029 |103423  | bc:31:e2:e1:ec:32 |   -   
|24597|318800|ROUTE| Et10               |1029 |103423  | bc:31:e2:e1:ec:32 |   -   
|24597|318801|ROUTE| Et3                |1017 |103431  | bc:31:e2:e1:ec:2c |   -   
|24598|318892|ROUTE| Et3                |1017 |103431  | bc:31:e2:e1:ec:2c |   -   
|24598|318893|ROUTE| Et10               |1029 |103423  | bc:31:e2:e1:ec:32 |   -   
|24598|318894|ROUTE| Et10               |1029 |103423  | bc:31:e2:e1:ec:32 |   -   
|24598|318895|ROUTE| Et3                |1017 |103431  | bc:31:e2:e1:ec:2c |   -   
|24601|319116|ROUTE| Et2                |1018 |103460  | d4:af:f7:2f:13:96 |Mswap 21304
|24601|319117|ROUTE| Et40               |1015 |103508  | e8:24:a6:96:05:48 |Mswap 21304
|24601|319118|ROUTE| Et40               |1015 |103508  | e8:24:a6:96:05:48 |Mswap 21304
|24601|319119|ROUTE| Et4                |1007 |103435  | c0:14:b8:21:97:90 |Mswap 21304
|24601|319120|ROUTE| Et4                |1007 |103435  | c0:14:b8:21:97:90 |Mswap 21304
|24601|319121|ROUTE| Et11               |1019 |103510  | d0:48:a1:ba:3c:61 |Mswap 21304
|24601|319122|ROUTE| Et11               |1019 |103510  | d0:48:a1:ba:3c:61 |Mswap 21304
|24601|319123|ROUTE| Et21               |1027 |103511  | d0:48:a1:ba:3c:63 |Mswap 21304
|24601|319124|ROUTE| Et21               |1027 |103511  | d0:48:a1:ba:3c:63 |Mswap 21304
|24601|319125|ROUTE| Et13               |1026 |103489  | 5c:07:58:a3:0a:aa |Mswap 21304
|24601|319126|ROUTE| Et13               |1026 |103489  | 5c:07:58:a3:0a:aa |Mswap 21304
|24601|319127|ROUTE| Et15               |1006 |103530  | 30:c5:07:84:3e:79 |Mswap 721304
|24601|319128|ROUTE| Et15               |1006 |103530  | 30:c5:07:84:3e:79 |Mswap 721304
|24601|319129|ROUTE| Et2                |1018 |103460  | d4:af:f7:2f:13:96 |Mswap 21304
|  -  |183502|ROUTE| FEC 318812         |   - |  -     |                   |   -   
|  -  |183504|ROUTE| FEC 319012         |   - |2097124 |                 - |Mpush 20217 524287
|  -  |183506|ROUTE| FEC 318794         |   - |2097128 |                 - |Mpush 378528
|  -  |183508|ROUTE| FEC 318942         |   - |2097134 |                 - |Mpush 18
|  -  |183510|ROUTE| FEC 319012         |   - |2097124 |                 - |Mpush 20217 524287
|  -  |183512|ROUTE| FEC 318796         |   - |2097115 |                 - |Mpush 21345 524284
|  -  |183514|ROUTE| FEC 319012         |   - |2097116 |                 - |Mpush 21346 524284
|  -  |183516|ROUTE| FEC 319010         |   - |2097119 |                 - |Mpush 21347 524284
|  -  |183518|ROUTE| FEC 319050         |   - |2097122 |                 - |Mpush 20084 720898
|  -  |183520|ROUTE| FEC 319052         |   - |2097123 |                 - |Mpush 970000
|  -  |183522|ROUTE| FEC 24587          |   - |2097130 |                 - |Mpush 17
|  -  |183524|ROUTE| FEC 24587          |   - |2097138 |                 - |Mpush 16
|  -  |183526|ROUTE| FEC 24587          |   - |2097130 |                 - |Mpush 17
|  -  |183528|ROUTE| FEC 24587          |   - |2097130 |                 - |Mpush 17
|  -  |183530|ROUTE| FEC 318942         |   - |2097134 |                 - |Mpush 18
|  -  |183532|ROUTE| FEC 319048         |   - |2097114 |                 - |Mpush 378530
|  -  |183534|ROUTE| FEC 319050         |   - |2097121 |                 - |Mpush 20084 720899
|  -  |183536|ROUTE| FEC 318828         |   - |2097141 |                 - |Mpush 524292
|  -  |183538|ROUTE| FEC 318824         |   - |2097148 |                 - |Mpush 62000
|  -  |183540|ROUTE| FEC 318862         |   - |2097117 |                 - |Mpush 378530
|  -  |183542|ROUTE| FEC 24595          |   - |2097133 |                 - |Mpush 1659
|  -  |183544|ROUTE| FEC 318940         |   - |2097145 |                 - |Mpush 21
|  -  |183546|ROUTE| FEC 24587          |   - |2097138 |                 - |Mpush 16
|  -  |183548|ROUTE| FEC 318842         |   - |  -     |                   |   -   
|  -  |183550|ROUTE| FEC 24581          |   - |2097150 |                 - |Mpush 20214 500000
|  -  |183552|ROUTE| FEC 24581          |   - |2097150 |                 - |Mpush 20214 500000
|  -  |183554|ROUTE| FEC 318986         |   - |2097135 |                 - |Mpush 378530
|  -  |183556|ROUTE| FEC 319068         |   - |2097149 |                 - |Mpush 62000
|  -  |183558|ROUTE| FEC 318950         |   - |  -     |                   |   -   
|  -  |183560|ROUTE| FEC 318940         |   - |2097127 |                 - |Mpush 16
|  -  |183562|ROUTE| FEC 319026         |   - |2097140 |                 - |Mpush 21
|  -  |183564|ROUTE| FEC 318964         |   - |2097112 |                 - |Mpush 21
|  -  |183566|ROUTE| FEC 318940         |   - |2097127 |                 - |Mpush 16
|  -  |183568|ROUTE| FEC 318948         |   - |2097151 |                 - |Mpush 524293
|  -  |183570|ROUTE| FEC 318998         |   - |2097118 |                 - |Mpush 970002
|  -  |183572|ROUTE| FEC 318804         |   - |2097147 |                 - |Mpush 970002
|  -  |183574|ROUTE| FEC 318854         |   - |2097132 |                 - |Mpush 970002
|  -  |183576|ROUTE| FEC 318794         |   - |2097125 |                 - |Mpush 378529
|  -  |183578|ROUTE| FEC 24598          |   - |2097139 |                 - |Mpush 1657
|  -  |183580|ROUTE| FEC 318950         |   - |2097120 |                 - |Mpush 1660
|  -  |183582|ROUTE| FEC 24598          |   - |2097137 |                 - |Mpush 1658
|  -  |183584|ROUTE| FEC 319052         |   - |  -     |                   |   -   
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
|  -  |315684|TRAP | CoppSystemL3DstMiss|1013 |1013    | ArpTrap           |   -   
|  -  |315685|TRAP | CoppSystemL3DstMiss|1014 |1014    | ArpTrap           |   -   
|  -  |315686|TRAP | CoppSystemL3DstMiss|1015 |1015    | ArpTrap           |   -   
|  -  |315687|TRAP | CoppSystemL3DstMiss|1016 |1016    | ArpTrap           |   -   
|  -  |315688|TRAP | CoppSystemL3DstMiss|1017 |1017    | ArpTrap           |   -   
|  -  |315689|TRAP | CoppSystemL3DstMiss|1018 |1018    | ArpTrap           |   -   
|  -  |315690|TRAP | CoppSystemL3DstMiss|1019 |1019    | ArpTrap           |   -   
|  -  |315691|TRAP | CoppSystemL3DstMiss|1020 |1020    | ArpTrap           |   -   
|  -  |315693|TRAP | CoppSystemL3DstMiss|1022 |1022    | ArpTrap           |   -   
|  -  |315694|TRAP | CoppSystemL3DstMiss|1023 |1023    | ArpTrap           |   -   
|  -  |315696|TRAP | CoppSystemL3DstMiss|1025 |1025    | ArpTrap           |   -   
|  -  |315697|TRAP | CoppSystemL3DstMiss|1026 |1026    | ArpTrap           |   -   
|  -  |315698|TRAP | CoppSystemL3DstMiss|1027 |1027    | ArpTrap           |   -   
|  -  |315700|TRAP | CoppSystemL3DstMiss|1029 |1029    | ArpTrap           |   -   
|  -  |318768|ROUTE| Et11               |1019 |103447  | d0:48:a1:ba:3c:61 |   -   
|  -  |318769|ROUTE| Et12               |1014 |103488  | 58:70:7f:9f:c4:03 |Mpush 20575 20556
|  -  |318770|ROUTE| Et11               |1019 |103447  | d0:48:a1:ba:3c:61 |   -   
|  -  |318772|DROP | DROP               |0    |  -     |                   |   -   
|  -  |318774|ROUTE| Et35               |1012 |103426  | 40:a6:b7:94:34:cb |   -   
|  -  |318776|ROUTE| Et12               |1014 |103430  | 58:70:7f:9f:c4:03 |   -   
|  -  |318778|ROUTE| Et31               |1020 |103436  | e4:6d:7f:e3:c8:0a |   -   
|  -  |318792|ROUTE| Et13               |1026 |103505  | 5c:07:58:a3:0a:aa |Mpush 21703
|  -  |318793|ROUTE| Et11               |1019 |103458  | d0:48:a1:ba:3c:61 |Mpush 19
|  -  |318794|ROUTE| Et2                |1018 |103425  | d4:af:f7:2f:13:96 |   -   
|  -  |318795|ROUTE| Et40               |1015 |103451  | e8:24:a6:96:05:48 |Mpush 20032
|  -  |318796|ROUTE| Et4                |1007 |103422  | c0:14:b8:21:97:90 |   -   
|  -  |318797|ROUTE| Et15               |1006 |103441  | 30:c5:07:84:3e:79 |Mpush 721303
|  -  |318802|ROUTE| Et13               |1026 |103429  | 5c:07:58:a3:0a:aa |   -   
|  -  |318804|ROUTE| Et13               |1026 |103429  | 5c:07:58:a3:0a:aa |   -   
|  -  |318806|ROUTE| Et4                |1007 |103422  | c0:14:b8:21:97:90 |   -   
|  -  |318810|ROUTE| Et6                |1022 |103438  | 18:5b:00:61:ac:73 |   -   
|  -  |318812|ROUTE| Et13               |1026 |103490  | 5c:07:58:a3:0a:aa |Mpush 2
|  -  |318813|ROUTE| Et12               |1014 |103495  | 58:70:7f:9f:c4:03 |Mpush 20575 20453
|  -  |318824|ROUTE| Et9                |1009 |103421  | e0:9b:27:c4:c5:84 |   -   
|  -  |318825|ROUTE| Et40               |1015 |103455  | e8:24:a6:96:05:48 |Mpush 20072
|  -  |318826|ROUTE| Et11               |1019 |103447  | d0:48:a1:ba:3c:61 |   -   
|  -  |318827|ROUTE| Et13               |1026 |103457  | 5c:07:58:a3:0a:aa |Mpush 21703 21684
|  -  |318828|ROUTE| Et15               |1006 |103437  | 30:c5:07:84:3e:79 |   -   
|  -  |318829|ROUTE| Et40               |1015 |103440  | e8:24:a6:96:05:48 |Mpush 20221
|  -  |318836|ROUTE| Et11               |1019 |103447  | d0:48:a1:ba:3c:61 |   -   
|  -  |318838|ROUTE| Et31               |1020 |103436  | e4:6d:7f:e3:c8:0a |   -   
|  -  |318840|ROUTE| Et15               |1006 |103437  | 30:c5:07:84:3e:79 |   -   
|  -  |318841|ROUTE| Et13               |1026 |103474  | 5c:07:58:a3:0a:aa |Mpush 21303 21349
|  -  |318842|ROUTE| Et15               |1006 |103483  | 30:c5:07:84:3e:79 |Mpush 721303
|  -  |318843|ROUTE| Et13               |1026 |103484  | 5c:07:58:a3:0a:aa |Mpush 21303
|  -  |318848|ROUTE| Et11               |1019 |103447  | d0:48:a1:ba:3c:61 |   -   
|  -  |318850|ROUTE| Et12               |1014 |103430  | 58:70:7f:9f:c4:03 |   -   
|  -  |318852|ROUTE| Et31               |1020 |103436  | e4:6d:7f:e3:c8:0a |   -   
|  -  |318853|ROUTE| Et40               |1015 |103433  | e8:24:a6:96:05:48 |Mpush 21195
|  -  |318854|ROUTE| Et13               |1026 |103429  | 5c:07:58:a3:0a:aa |   -   
|  -  |318855|ROUTE| Et15               |1006 |103524  | 30:c5:07:84:3e:79 |Mpush 721182
|  -  |318860|ROUTE| Et9                |1009 |103421  | e0:9b:27:c4:c5:84 |   -   
|  -  |318862|ROUTE| Et2                |1018 |103425  | d4:af:f7:2f:13:96 |   -   
|  -  |318863|ROUTE| Et15               |1006 |103463  | 30:c5:07:84:3e:79 |Mpush 721303 20161
|  -  |318864|ROUTE| Et9                |1009 |103421  | e0:9b:27:c4:c5:84 |   -   
|  -  |318866|ROUTE| Et8                |1023 |103432  | c0:14:b8:21:97:94 |   -   
|  -  |318868|ROUTE| Et35               |1012 |103426  | 40:a6:b7:94:34:cb |   -   
|  -  |318882|ROUTE| Et2                |1018 |103425  | d4:af:f7:2f:13:96 |   -   
|  -  |318884|ROUTE| Et13               |1026 |103429  | 5c:07:58:a3:0a:aa |   -   
|  -  |318886|ROUTE| Et13               |1026 |103429  | 5c:07:58:a3:0a:aa |   -   
|  -  |318888|ROUTE| Et15               |1006 |103437  | 30:c5:07:84:3e:79 |   -   
|  -  |318890|ROUTE| Et15               |1006 |103437  | 30:c5:07:84:3e:79 |   -   
|  -  |318896|ROUTE| Et3                |1017 |103431  | bc:31:e2:e1:ec:2c |   -   
|  -  |318898|ROUTE| Et13               |1026 |103429  | 5c:07:58:a3:0a:aa |   -   
|  -  |318899|ROUTE| Et11               |1019 |103514  | d0:48:a1:ba:3c:61 |Mpush 19 21581
|  -  |318908|ROUTE| Et31               |1020 |103436  | e4:6d:7f:e3:c8:0a |   -   
|  -  |318910|ROUTE| Et40               |1015 |103427  | e8:24:a6:96:05:48 |   -   
|  -  |318922|DROP | DROP               |0    |  -     |                   |   -   
|  -  |318924|ROUTE| Et10               |1029 |103423  | bc:31:e2:e1:ec:32 |   -   
|  -  |318926|ROUTE| Et5                |1008 |103428  | 18:5b:00:61:ac:6f |   -   
|  -  |318928|ROUTE| Et35               |1012 |103426  | 40:a6:b7:94:34:cb |   -   
|  -  |318930|ROUTE| Et4                |1007 |103422  | c0:14:b8:21:97:90 |   -   
|  -  |318936|ROUTE| Et17               |1016 |103448  | 64:6d:4e:32:e1:22 |   -   
|  -  |318938|ROUTE| Et18               |1013 |103450  | 64:6d:4e:32:e1:23 |   -   
|  -  |318940|ROUTE| Et40               |1015 |103427  | e8:24:a6:96:05:48 |   -   
|  -  |318942|ROUTE| Et35               |1012 |103426  | 40:a6:b7:94:34:cb |   -   
|  -  |318943|ROUTE| Et40               |1015 |103442  | e8:24:a6:96:05:48 |Mpush 20131
|  -  |318944|ROUTE| Et20               |1025 |103475  | 60:53:75:13:ba:dd |   -   
|  -  |318946|ROUTE| Et11               |1019 |103447  | d0:48:a1:ba:3c:61 |   -   
|  -  |318947|ROUTE| Et13               |1026 |103477  | 5c:07:58:a3:0a:aa |Mpush 21685
|  -  |318948|ROUTE| Et15               |1006 |103437  | 30:c5:07:84:3e:79 |   -   
|  -  |318949|ROUTE| Et40               |1015 |103434  | e8:24:a6:96:05:48 |Mpush 21350
|  -  |318950|ROUTE| Et15               |1006 |103466  | 30:c5:07:84:3e:79 |Mpush 721248
|  -  |318951|ROUTE| Et13               |1026 |103468  | 5c:07:58:a3:0a:aa |Mpush 21248
|  -  |318952|ROUTE| Et2                |1018 |103425  | d4:af:f7:2f:13:96 |   -   
|  -  |318954|ROUTE| Et21               |1027 |103453  | d0:48:a1:ba:3c:63 |   -   
|  -  |318956|DROP | DROP               |0    |  -     |                   |   -   
|  -  |318958|ROUTE| Et3                |1017 |103431  | bc:31:e2:e1:ec:2c |   -   
|  -  |318960|ROUTE| Et12               |1014 |103430  | 58:70:7f:9f:c4:03 |   -   
|  -  |318962|ROUTE| Et4                |1007 |103422  | c0:14:b8:21:97:90 |   -   
|  -  |318964|ROUTE| Et40               |1015 |103427  | e8:24:a6:96:05:48 |   -   
|  -  |318965|ROUTE| Et21               |1027 |103575  | d0:48:a1:ba:3c:63 |Mpush 21308
|  -  |318966|DROP | DROP               |0    |  -     |                   |   -   
|  -  |318968|DROP | DROP               |0    |  -     |                   |   -   
|  -  |318970|DROP | DROP               |0    |  -     |                   |   -   
|  -  |318972|ROUTE| Et6                |1022 |103438  | 18:5b:00:61:ac:73 |   -   
|  -  |318986|ROUTE| Et2                |1018 |103425  | d4:af:f7:2f:13:96 |   -   
|  -  |318988|ROUTE| Et13               |1026 |103429  | 5c:07:58:a3:0a:aa |   -   
|  -  |318994|ROUTE| Et12               |1014 |103430  | 58:70:7f:9f:c4:03 |   -   
|  -  |318996|ROUTE| Et4                |1007 |103422  | c0:14:b8:21:97:90 |   -   
|  -  |318998|ROUTE| Et13               |1026 |103429  | 5c:07:58:a3:0a:aa |   -   
|  -  |318999|ROUTE| Et15               |1006 |103491  | 30:c5:07:84:3e:79 |Mpush 721303 21181
|  -  |319000|ROUTE| Et40               |1015 |103427  | e8:24:a6:96:05:48 |   -   
|  -  |319002|ROUTE| Et13               |1026 |103429  | 5c:07:58:a3:0a:aa |   -   
|  -  |319008|ROUTE| Et9                |1009 |103421  | e0:9b:27:c4:c5:84 |   -   
|  -  |319010|ROUTE| Et4                |1007 |103422  | c0:14:b8:21:97:90 |   -   
|  -  |319012|ROUTE| Et4                |1007 |103422  | c0:14:b8:21:97:90 |   -   
|  -  |319013|ROUTE| Et40               |1015 |103427  | e8:24:a6:96:05:48 |   -   
|  -  |319018|ROUTE| Et21               |1027 |103453  | d0:48:a1:ba:3c:63 |   -   
|  -  |319020|ROUTE| Et4                |1007 |103422  | c0:14:b8:21:97:90 |   -   
|  -  |319022|ROUTE| Et9                |1009 |103421  | e0:9b:27:c4:c5:84 |   -   
|  -  |319023|ROUTE| Et21               |1027 |103480  | d0:48:a1:ba:3c:63 |Mpush 21201
|  -  |319024|ROUTE| Et13               |1026 |103429  | 5c:07:58:a3:0a:aa |   -   
|  -  |319025|ROUTE| Et11               |1019 |103513  | d0:48:a1:ba:3c:61 |Mpush 21582
|  -  |319026|ROUTE| Et40               |1015 |103427  | e8:24:a6:96:05:48 |   -   
|  -  |319027|ROUTE| Et15               |1006 |103446  | 30:c5:07:84:3e:79 |Mpush 721303 21307
|  -  |319028|ROUTE| Et12               |1014 |103430  | 58:70:7f:9f:c4:03 |   -   
|  -  |319030|ROUTE| Et12               |1014 |103430  | 58:70:7f:9f:c4:03 |   -   
|  -  |319032|ROUTE| Et5                |1008 |103428  | 18:5b:00:61:ac:6f |   -   
|  -  |319034|ROUTE| Et15               |1006 |103437  | 30:c5:07:84:3e:79 |   -   
|  -  |319036|ROUTE| Et13               |1026 |103429  | 5c:07:58:a3:0a:aa |   -   
|  -  |319038|ROUTE| Et3                |1017 |103431  | bc:31:e2:e1:ec:2c |   -   
|  -  |319040|ROUTE| Et3                |1017 |103431  | bc:31:e2:e1:ec:2c |   -   
|  -  |319042|ROUTE| Et2                |1018 |103425  | d4:af:f7:2f:13:96 |   -   
|  -  |319044|ROUTE| Et11               |1019 |103447  | d0:48:a1:ba:3c:61 |   -   
|  -  |319046|ROUTE| Et11               |1019 |103447  | d0:48:a1:ba:3c:61 |   -   
|  -  |319048|ROUTE| Et2                |1018 |103425  | d4:af:f7:2f:13:96 |   -   
|  -  |319049|ROUTE| Et4                |1007 |103473  | c0:14:b8:21:97:90 |Mpush 20162
|  -  |319050|ROUTE| Et12               |1014 |103430  | 58:70:7f:9f:c4:03 |   -   
|  -  |319051|ROUTE| Et40               |1015 |103427  | e8:24:a6:96:05:48 |   -   
|  -  |319052|ROUTE| Et13               |1026 |103464  | 5c:07:58:a3:0a:aa |Mpush 0
|  -  |319053|ROUTE| Et40               |1015 |103465  | e8:24:a6:96:05:48 |Mpush 20053
|  -  |319054|ROUTE| Et2                |1018 |103425  | d4:af:f7:2f:13:96 |   -   
|  -  |319056|ROUTE| Et3                |1017 |103431  | bc:31:e2:e1:ec:2c |   -   
|  -  |319064|ROUTE| Et10               |1029 |103423  | bc:31:e2:e1:ec:32 |   -   
|  -  |319066|ROUTE| Et4                |1007 |103422  | c0:14:b8:21:97:90 |   -   
|  -  |319068|ROUTE| Et31               |1020 |103436  | e4:6d:7f:e3:c8:0a |   -   
|  -  |319069|ROUTE| Et40               |1015 |103444  | e8:24:a6:96:05:48 |Mpush 20066
|  -  |319070|ROUTE| Et20               |1025 |103475  | 60:53:75:13:ba:dd |   -   
|  -  |319072|ROUTE| Et40               |1015 |103427  | e8:24:a6:96:05:48 |   -   
|  -  |319100|ROUTE| Et2                |1018 |103425  | d4:af:f7:2f:13:96 |   -   

```

