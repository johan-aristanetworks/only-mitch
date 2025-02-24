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

Uptime: 1 day, 7 hours and 43 minutes
Total memory: 65734472 kB
Free memory: 61871552 kB

```

## show lldp neighbors

```text
Last table change time   : 4:56:47 ago
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
Et1       Arista_Spine30_Eth2  0:01    521.3   6.3%      678    528.0   6.3%
Et40                           0:01    524.6   6.3%      682    538.5   6.5%

Port      Out Kpps
Et1            660
Et40           701
```

## show isis neighbors

```text
 
Instance  VRF      System Id        Type Interface          SNPA              State Hold time   Circuit Id          
IGP       default  Arista-Spine3-Q2A-30 L2   Ethernet1          P2P               UP    27          2C                  
IGP       default  Juniper-175-ACX7100-48L L2   Ethernet5          P2P               UP    19          01                  
```

## show isis database detail

```text
Legend:
H - hostname conflict
U - node unreachable

IS-IS Instance: IGP VRF: default
  IS-IS Level 2 Link State Database
    LSPID                   Seq Num  Cksum  Life Length IS  Received LSPID        Flags
    Arista-Spine3-Q2A-30.00-00       422  55345   501   1078 L2  0000.0000.0030.00-00  <>
      Remaining lifetime received: 1199 s Modified to: 1200 s
      NLPID: 0xCC(IPv4) 0x8E(IPv6)
      Hostname: Arista-Spine3-Q2A-30
      Area addresses: 49.0001
      Topology: 2 (IPv6)
      Topology: 0 (IPv4)
      Interface address: 20.30.179.30
      Interface address: 20.30.66.30
      Interface address: 20.30.124.30
      Interface address: 20.30.128.30
      Interface address: 20.30.217.30
      Interface address: 20.30.184.30
      Interface address: 20.30.221.30
      Interface address: 20.30.72.30
      Interface address: 20.30.53.30
      Interface address: 20.30.84.30
      Interface address: 20.30.214.30
      Interface address: 20.30.120.30
      Interface address: 20.30.32.30
      Interface address: 10.0.0.30
      Interface address: 2001:0:30:179::30
      Interface address: 2001:0:30:66::30
      Interface address: 2001:0:30:124::30
      Interface address: 2001:0:30:128::30
      Interface address: 2001:0:30:217::30
      Interface address: 2001:0:30:184::30
      Interface address: 2001:0:30:221::30
      Interface address: 2001:0:30:72::30
      Interface address: 2001:0:53:120::30
      Interface address: 2001:0:30:84::30
      Interface address: 2001:0:30:214::30
      Interface address: 2001:0:30:120::30
      Interface address: 2001:0:30:32::30
      IS Neighbor          : H3C_M1A_120.00      Metric: 10
        IPv4 Neighbor Address: 20.30.120.120
        IPv4 Interface Address: 20.30.120.30
        Adj-sid: 362188 flags: [L V] weight: 0x0
      IS Neighbor          : Juniper-179-ACX7024.00 Metric: 10
        IPv4 Neighbor Address: 20.30.179.179
        IPv4 Interface Address: 20.30.179.30
        Adj-sid: 362201 flags: [L V] weight: 0x0
      IS Neighbor          : Ericsson_84_R6678.00 Metric: 10
        IPv4 Neighbor Address: 20.30.84.84
        IPv4 Interface Address: 20.30.84.30
        Adj-sid: 362199 flags: [L V] weight: 0x0
      IS Neighbor          : Arista-PE32-Q2C-32.00 Metric: 10
        IPv4 Neighbor Address: 20.30.32.32
        IPv4 Interface Address: 20.30.32.30
        Adj-sid: 362190 flags: [L V] weight: 0x0
      IS Neighbor          : 221.00              Metric: 10
        IPv4 Neighbor Address: 20.30.221.221
        IPv4 Interface Address: 20.30.221.30
        Adj-sid: 362197 flags: [L V] weight: 0x0
      IS Neighbor          : Nokia-SR1-217.00    Metric: 10
        IPv4 Neighbor Address: 20.30.217.217
        IPv4 Interface Address: 20.30.217.30
        Adj-sid: 362196 flags: [L V] weight: 0x0
      IS Neighbor          : Ciena-5134-72.00    Metric: 10
        IPv4 Neighbor Address: 20.30.72.72
        IPv4 Interface Address: 20.30.72.30
        Adj-sid: 362195 flags: [L V] weight: 0x0
      IS Neighbor          : 0000.0000.0128.00   Metric: 10
        IPv4 Neighbor Address: 20.30.128.128
        IPv4 Interface Address: 20.30.128.30
        Adj-sid: 362194 flags: [L V] weight: 0x0
      IS Neighbor          : Arrcus-53.00        Metric: 10
        IPv4 Neighbor Address: 20.30.53.53
        IPv4 Interface Address: 20.30.53.30
        Adj-sid: 362193 flags: [L V] weight: 0x0
      IS Neighbor          : 0000.0000.0124.00   Metric: 10
        IPv4 Neighbor Address: 20.30.124.124
        IPv4 Interface Address: 20.30.124.30
        Adj-sid: 362192 flags: [L V] weight: 0x0
      IS Neighbor          : Nokia-SXR-214.00    Metric: 10
        IPv4 Neighbor Address: 20.30.214.214
        IPv4 Interface Address: 20.30.214.30
        Adj-sid: 362191 flags: [L V] weight: 0x0
      IS Neighbor (MT-IPv6): H3C_M1A_120.00      Metric: 10
        Adj-sid: 362189 flags: [L V F] weight: 0x0
      IS Neighbor (MT-IPv6): Ericsson_84_R6678.00 Metric: 10
        Adj-sid: 362200 flags: [L V F] weight: 0x0
      IS Neighbor (MT-IPv6): Arista-PE32-Q2C-32.00 Metric: 10
        Adj-sid: 362198 flags: [L V F] weight: 0x0
      Reachability         : 20.30.179.0/24 Metric: 10 Type: 1 Up
      Reachability         : 20.30.66.0/24 Metric: 10 Type: 1 Up
      Reachability         : 20.30.124.0/24 Metric: 10 Type: 1 Up
      Reachability         : 20.30.128.0/24 Metric: 10 Type: 1 Up
      Reachability         : 20.30.217.0/24 Metric: 10 Type: 1 Up
      Reachability         : 20.30.184.0/24 Metric: 10 Type: 1 Up
      Reachability         : 20.30.221.0/24 Metric: 10 Type: 1 Up
      Reachability         : 20.30.72.0/24 Metric: 10 Type: 1 Up
      Reachability         : 20.30.53.0/24 Metric: 10 Type: 1 Up
      Reachability         : 20.30.84.0/24 Metric: 10 Type: 1 Up
      Reachability         : 20.30.214.0/24 Metric: 10 Type: 1 Up
      Reachability         : 20.30.120.0/24 Metric: 10 Type: 1 Up
      Reachability         : 20.30.32.0/24 Metric: 10 Type: 1 Up
      Reachability         : 10.0.0.30/32 Metric: 0 Type: 1 Up
        SR Prefix-SID: 30 Flags: [N] Algorithm: 0
      Reachability (MT-IPv6): 2001:0:30:179::/64 Metric: 10 Type: 1 Up
      Reachability (MT-IPv6): 2001:0:30:66::/64 Metric: 10 Type: 1 Up
      Reachability (MT-IPv6): 2001:0:30:124::/64 Metric: 10 Type: 1 Up
      Reachability (MT-IPv6): 2001:0:30:128::/64 Metric: 10 Type: 1 Up
      Reachability (MT-IPv6): 2001:0:30:217::/64 Metric: 10 Type: 1 Up
      Reachability (MT-IPv6): 2001:0:30:184::/64 Metric: 10 Type: 1 Up
      Reachability (MT-IPv6): 2001:0:30:221::/64 Metric: 10 Type: 1 Up
      Reachability (MT-IPv6): 2001:0:30:72::/64 Metric: 10 Type: 1 Up
      Reachability (MT-IPv6): 2001:0:53:120::/64 Metric: 10 Type: 1 Up
      Reachability (MT-IPv6): 2001:0:30:84::/64 Metric: 10 Type: 1 Up
      Reachability (MT-IPv6): 2001:0:30:214::/64 Metric: 10 Type: 1 Up
      Reachability (MT-IPv6): 2001:0:30:120::/64 Metric: 10 Type: 1 Up
      Reachability (MT-IPv6): 2001:0:30:32::/64 Metric: 10 Type: 1 Up
      Router Capabilities: Router Id: 10.0.0.30 Flags: []
        SR Local Block:
          SRLB Base: 965536 Range: 65536
        Area leader priority: 250 algorithm: 0
        Maximum SID depth:
          Base MPLS imposition (MSD type 1):  12
        SR Capability: Flags: [I V]
          SRGB Base: 20000 Range: 2000
    Arista-PE32-Q2C-32.00-00        46  61138   643    306 L2  0000.0000.0032.00-00  <>
      LSP generation remaining wait time: 0 ms
      Time remaining until refresh: 343 s
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
        Adj-sid: 362158 flags: [L V] weight: 0x0
      IS Neighbor          : Arista-Spine3-Q2A-30.00 Metric: 10
        IPv4 Neighbor Address: 20.30.32.30
        IPv4 Interface Address: 20.30.32.32
        Adj-sid: 362156 flags: [L V] weight: 0x0
      IS Neighbor (MT-IPv6): Arista-Spine3-Q2A-30.00 Metric: 10
        Adj-sid: 362157 flags: [L V F] weight: 0x0
      Reachability         : 20.32.175.0/24 Metric: 10 Type: 1 Up
      Reachability         : 20.30.32.0/24 Metric: 10 Type: 1 Up
      Reachability         : 10.0.0.32/32 Metric: 0 Type: 1 Up
        SR Prefix-SID: 32 Flags: [N] Algorithm: 0
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
    Arrcus-53.00-00             205  60811   958    210 L2  0000.0000.0053.00-00  <>
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
      Router Capabilities: Router Id: 10.0.0.53 Flags: []
        SR Local Block:
          SRLB Base: 30000 Range: 2001
        SR Capability: Flags: [I V]
          SRGB Base: 20000 Range: 2000
        Algorithms:  0
    Ciena-5134-72.00-00         118  20450  1044    308 L2  0000.0000.0072.00-00  <>
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
    Ericsson_84_R6678.00-00       162  62975   855    277 L2  0000.0000.0084.00-00  <>
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
      IS Neighbor (MT-IPv6): Arista-Spine3-Q2A-30.00 Metric: 10
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
    H3C_M1A_120.00-00           239   7077   575    555 L2  0000.0000.0120.00-00  <>
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
        Adj-sid: 1140 flags: [L V] weight: 0x0
      IS Neighbor          : Juniper-175-ACX7100-48L.00 Metric: 10
        IPv4 Neighbor Address: 20.120.175.175
        IPv4 Interface Address: 20.120.175.120
        Adj-sid: 1141 flags: [L V] weight: 0x0
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
    0000.0000.0124.00-00         40   1461   903    297 L2  0000.0000.0124.00-00  <>
      Remaining lifetime received: 1199 s Modified to: 1200 s
      NLPID: 0xCC(IPv4) 0x8E(IPv6)
      Area addresses: 49.0001
      Topology: 0 (IPv4)
      Topology: 2 (IPv6)
      Interface address: 20.124.175.124
      Interface address: 20.30.124.124
      Interface address: 10.0.0.124
      IS Neighbor          : Juniper-175-ACX7100-48L.00 Metric: 10
        IPv4 Neighbor Address: 20.124.175.175
        IPv4 Interface Address: 20.124.175.124
        Adj-sid: 396 flags: [L V] weight: 0x0
      IS Neighbor          : Arista-Spine3-Q2A-30.00 Metric: 10
        IPv4 Neighbor Address: 20.30.124.30
        IPv4 Interface Address: 20.30.124.124
        Adj-sid: 397 flags: [L V] weight: 0x0
      Reachability         : 20.30.124.0/24 Metric: 10 Type: 1 Up
      Reachability         : 20.124.175.0/24 Metric: 10 Type: 1 Up
      Reachability         : 10.0.0.124/32 Metric: 0 Type: 1 Up
        SR Prefix-SID: 124 Flags: [N P] Algorithm: 0
      Router Capabilities: Router Id: 10.0.0.124 Flags: []
        Maximum SID depth:
          Base MPLS imposition (MSD type 1):  10
        SR Capability: Flags: [I]
          SRGB Base: 2000 Range: 2001
    0000.0000.0128.00-00         40  22321  1075    297 L2  0000.0000.0128.00-00  <>
      Remaining lifetime received: 1199 s Modified to: 1200 s
      NLPID: 0xCC(IPv4) 0x8E(IPv6)
      Area addresses: 49.0001
      Topology: 0 (IPv4)
      Topology: 2 (IPv6)
      Interface address: 10.0.0.128
      Interface address: 20.30.128.128
      Interface address: 20.128.175.128
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
      Reachability         : 20.30.128.0/24 Metric: 10 Type: 1 Up
      Reachability         : 20.128.175.0/24 Metric: 10 Type: 1 Up
      Router Capabilities: Router Id: 10.0.0.128 Flags: []
        Maximum SID depth:
          Base MPLS imposition (MSD type 1):  10
        SR Capability: Flags: [I]
          SRGB Base: 20000 Range: 2000
    Juniper-175-ACX7100-48L.00-00        71  36311   958   1287 L2  0000.0000.0175.00-00  <>
      Remaining lifetime received: 1199 s Modified to: 1200 s
      NLPID: 0xCC(IPv4) 0x8E(IPv6)
      Hostname: Juniper-175-ACX7100-48L
      Area addresses: 49.0001
      Interface address: 10.0.0.175
      Interface address: 2001:0:32:175::175
      IS Neighbor          : Nokia-SR1-217.00    Metric: 1
        IPv4 Neighbor Address: 20.175.217.217
        IPv4 Interface Address: 20.175.217.175
        IPv6 Neighbor Address: 2001:0:175:217::217
        Global IPv6 Interface Address: 2001:0:175:217::175
        Adj-sid: 62 flags: [L V F] weight: 0x0
        Adj-sid: 61 flags: [L V] weight: 0x0
      IS Neighbor          : 221.00              Metric: 1
        IPv4 Neighbor Address: 20.175.221.221
        IPv4 Interface Address: 20.175.221.175
        Global IPv6 Interface Address: 2001:0:175:221::175
        Adj-sid: 68 flags: [L V F] weight: 0x0
        Adj-sid: 67 flags: [L V] weight: 0x0
      IS Neighbor          : Ericsson_84_R6678.00 Metric: 1
        IPv4 Neighbor Address: 20.84.175.84
        IPv4 Interface Address: 20.84.175.175
        IPv6 Neighbor Address: 2001:0:84:175::175
        Global IPv6 Interface Address: 2001:0:84:175::175
        Adj-sid: 60 flags: [L V F] weight: 0x0
        Adj-sid: 59 flags: [L V] weight: 0x0
      IS Neighbor          : 0000.0000.0128.00   Metric: 1
        IPv4 Neighbor Address: 20.128.175.128
        IPv4 Interface Address: 20.128.175.175
        Global IPv6 Interface Address: 2001:0:128:175::175
        Adj-sid: 72 flags: [L V] weight: 0x0
      IS Neighbor          : 0000.0000.0124.00   Metric: 1
        IPv4 Neighbor Address: 20.124.175.124
        IPv4 Interface Address: 20.124.175.175
        Adj-sid: 71 flags: [L V] weight: 0x0
      IS Neighbor          : Nokia-SXR-214.00    Metric: 1
        IPv4 Neighbor Address: 20.175.214.214
        IPv4 Interface Address: 20.175.214.175
        IPv6 Neighbor Address: 2001:0:175:214::214
        Global IPv6 Interface Address: 2001:0:175:214::175
        Adj-sid: 66 flags: [L V F] weight: 0x0
        Adj-sid: 65 flags: [L V] weight: 0x0
      IS Neighbor          : Arista-PE32-Q2C-32.00 Metric: 1
        IPv4 Neighbor Address: 20.32.175.32
        IPv4 Interface Address: 20.32.175.175
        Global IPv6 Interface Address: 2001:0:32:175::175
        Adj-sid: 74 flags: [L V F] weight: 0x0
        Adj-sid: 73 flags: [L V] weight: 0x0
      IS Neighbor          : Ciena-5134-72.00    Metric: 1
        IPv4 Neighbor Address: 20.72.175.72
        IPv4 Interface Address: 20.72.175.175
        Global IPv6 Interface Address: 2001:0:72:175::175
        Adj-sid: 70 flags: [L V] weight: 0x0
      IS Neighbor          : Juniper-179-ACX7024.00 Metric: 1
        IPv4 Neighbor Address: 20.175.179.179
        IPv4 Interface Address: 20.175.179.175
        IPv6 Neighbor Address: 2001:0:175::179:179
        Global IPv6 Interface Address: 2001:0:175::179:175
        Adj-sid: 82 flags: [L V F] weight: 0x0
        Adj-sid: 81 flags: [L V] weight: 0x0
      IS Neighbor          : H3C_M1A_120.00      Metric: 1
        IPv4 Neighbor Address: 20.120.175.120
        IPv4 Interface Address: 20.120.175.175
        IPv6 Neighbor Address: 2001:0:120:175::120
        Global IPv6 Interface Address: 2001:0:120:175::175
        Adj-sid: 78 flags: [L V F] weight: 0x0
        Adj-sid: 77 flags: [L V] weight: 0x0
      IS Neighbor          : Arrcus-53.00        Metric: 1
        IPv4 Neighbor Address: 20.53.175.53
        IPv4 Interface Address: 20.53.175.175
        Global IPv6 Interface Address: 2001:0:53:175::175
        Adj-sid: 83 flags: [L V] weight: 0x0
      Reachability         : 10.0.0.175/32 Metric: 0 Type: 1 Up
        SR Prefix-SID: 175 Flags: [N] Algorithm: 0
      Reachability         : 20.66.175.0/24 Metric: 1 Type: 1 Up
      Reachability         : 20.72.175.0/24 Metric: 1 Type: 1 Up
      Reachability         : 20.175.214.0/24 Metric: 1 Type: 1 Up
      Reachability         : 20.124.175.0/24 Metric: 1 Type: 1 Up
      Reachability         : 20.175.184.0/24 Metric: 1 Type: 1 Up
      Reachability         : 20.128.175.0/24 Metric: 1 Type: 1 Up
      Reachability         : 20.84.175.0/24 Metric: 1 Type: 1 Up
      Reachability         : 20.175.221.0/24 Metric: 1 Type: 1 Up
      Reachability         : 20.120.175.0/24 Metric: 1 Type: 1 Up
      Reachability         : 20.175.179.0/24 Metric: 1 Type: 1 Up
      Reachability         : 20.32.175.0/24 Metric: 1 Type: 1 Up
      Reachability         : 20.175.217.0/24 Metric: 1 Type: 1 Up
      Reachability         : 20.131.175.0/24 Metric: 1 Type: 1 Up
      Reachability         : 20.53.175.0/24 Metric: 1 Type: 1 Up
      Reachability          : 2001:0:66:175::/64 Metric: 1 Type: 1 Up
      Reachability          : 2001:0:72:175::/64 Metric: 1 Type: 1 Up
      Reachability          : 2001:0:175:214::/64 Metric: 1 Type: 1 Up
      Reachability          : 2001:0:175:184::/64 Metric: 1 Type: 1 Up
      Reachability          : 2001:0:128:175::/64 Metric: 1 Type: 1 Up
      Reachability          : 2001:0:84:175::/64 Metric: 1 Type: 1 Up
      Reachability          : 2001:0:175:221::/64 Metric: 1 Type: 1 Up
      Reachability          : 2001:0:120:175::/64 Metric: 1 Type: 1 Up
      Reachability          : 2001:0:175::/64 Metric: 1 Type: 1 Up
      Reachability          : 2001:0:32:175::/64 Metric: 1 Type: 1 Up
      Reachability          : 2001:0:175:217::/64 Metric: 1 Type: 1 Up
      Reachability          : 2001:0:131:175::/64 Metric: 1 Type: 1 Up
      Reachability          : 2001:0:53:175::/64 Metric: 1 Type: 1 Up
      Router Capabilities: Router Id: 10.0.0.175 Flags: []
        Maximum SID depth:
          Base MPLS imposition (MSD type 1):  3
        SR Capability: Flags: [I V]
          SRGB Base: 20000 Range: 2000
        Algorithms:  0, 1
      Unsupported TLV: Type: 14 Length: 2
    Juniper-179-ACX7024.00-00        38  12279   752    386 L2  0000.0000.0179.00-00  <>
      Remaining lifetime received: 1199 s Modified to: 1200 s
      NLPID: 0xCC(IPv4) 0x8E(IPv6)
      Hostname: Juniper-179-ACX7024
      Area addresses: 49.0001
      Interface address: 10.0.0.179
      IS Neighbor          : Juniper-175-ACX7100-48L.00 Metric: 10
        IPv4 Neighbor Address: 20.175.179.175
        IPv4 Interface Address: 20.175.179.179
        IPv6 Neighbor Address: 2001:0:175::179:175
        Global IPv6 Interface Address: 2001:0:175::179:179
        Adj-sid: 20 flags: [L V F] weight: 0x0
        Adj-sid: 19 flags: [L V] weight: 0x0
      IS Neighbor          : Arista-Spine3-Q2A-30.00 Metric: 10
        IPv4 Neighbor Address: 20.30.179.30
        IPv4 Interface Address: 20.30.179.179
        Global IPv6 Interface Address: 2001:0:30:179::179
        Adj-sid: 18 flags: [L V F] weight: 0x0
        Adj-sid: 17 flags: [L V] weight: 0x0
      Reachability         : 10.0.0.179/32 Metric: 0 Type: 1 Up
        SR Prefix-SID: 179 Flags: [N] Algorithm: 0
      Reachability         : 20.175.179.0/24 Metric: 10 Type: 1 Up
      Reachability         : 20.30.179.0/24 Metric: 10 Type: 1 Up
      Reachability          : 2001:0:175::/64 Metric: 10 Type: 1 Up
      Reachability          : 2001:0:30:179::/64 Metric: 10 Type: 1 Up
      Router Capabilities: Router Id: 10.0.0.179 Flags: []
        Maximum SID depth:
          Base MPLS imposition (MSD type 1):  8
        SR Capability: Flags: [I V]
          SRGB Base: 20000 Range: 2000
        Algorithms:  0, 1
      Unsupported TLV: Type: 14 Length: 2
    Nokia-SXR-214.00-00        8656  51872  1197    482 L2  0000.0000.0214.00-00  <>
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
        IPv6 Neighbor Address: 2001:0:214:216::216
        Global IPv6 Interface Address: 2001:0:214:216::214
        Adj-sid: 30003 flags: [L V B] weight: 0x0
        Adj-sid: 30020 flags: [L V B F] weight: 0x0
      IS Neighbor          : Juniper-175-ACX7100-48L.00 Metric: 10
        IPv4 Neighbor Address: 20.175.214.175
        IPv4 Interface Address: 20.175.214.214
        IPv6 Neighbor Address: 2001:0:175:214::175
        Global IPv6 Interface Address: 2001:0:175:214::214
        Adj-sid: 30016 flags: [L V B] weight: 0x0
        Adj-sid: 30017 flags: [L V B F] weight: 0x0
      IS Neighbor          : Arista-Spine3-Q2A-30.00 Metric: 10
        IPv4 Neighbor Address: 20.30.214.30
        IPv4 Interface Address: 20.30.214.214
        Adj-sid: 30018 flags: [L V B] weight: 0x0
        Adj-sid: 30019 flags: [L V B F] weight: 0x0
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
    Nokia-IXRe2-216.00-00       165  15341   653    335 L2  0100.0000.0216.00-00  <>
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
        Adj-sid: 1048575 flags: [L V] weight: 0x0
        Adj-sid: 1048574 flags: [L V F] weight: 0x0
      Reachability         : 20.214.216.0/24 Metric: 10 Type: 1 Up
      Reachability         : 10.0.0.216/32 Metric: 0 Type: 1 Up
      Reachability          : 2001:0:214:216::/64 Metric: 10 Type: 1 Up
      Reachability          : 2002::216/128 Metric: 0 Type: 1 Up
      Reachability (MT-IPv6): 2001:0:214:216::/64 Metric: 10 Type: 1 Up
      Reachability (MT-IPv6): 2002::216/128 Metric: 0 Type: 1 Up
      Router Capabilities: Router Id: 10.0.0.216 Flags: []
        Maximum SID depth:
          Base MPLS imposition (MSD type 1):  11
        SR Capability: Flags: [I V]
          SRGB Base: 20000 Range: 2000
        Algorithms:  0
    Nokia-SR1-217.00-00         171  58228   710    429 L2  0100.0000.0217.00-00  <>
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
      IS Neighbor          : Juniper-175-ACX7100-48L.00 Metric: 10
        IPv4 Neighbor Address: 20.175.217.175
        IPv4 Interface Address: 20.175.217.217
        IPv6 Neighbor Address: 2001:0:175:217::175
        Global IPv6 Interface Address: 2001:0:175:217::217
        Adj-sid: 524280 flags: [L V B] weight: 0x0
        Adj-sid: 524279 flags: [L V B F] weight: 0x0
      IS Neighbor          : Arista-Spine3-Q2A-30.00 Metric: 10
        IPv4 Neighbor Address: 20.30.217.30
        IPv4 Interface Address: 20.30.217.217
        Adj-sid: 524282 flags: [L V B] weight: 0x0
        Adj-sid: 524281 flags: [L V B F] weight: 0x0
      Reachability         : 10.0.0.217/32 Metric: 0 Type: 1 Up
        SR Prefix-SID: 217 Flags: [N P] Algorithm: 0
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
        Algorithms:  0
    221.00-00                    22  52384   512     80 L2  0221.0221.0221.00-00  <>
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
    221.00-01                    22  45990  1011     32 L2  0221.0221.0221.00-01  <>
      Remaining lifetime received: 1199 s Modified to: 1200 s
      Hostname: 221
    221.00-02                    27  41251   888    273 L2  0221.0221.0221.00-02  <>
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
        Adj-sid: 524307 flags: [L V B] weight: 0x0
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
  1         10.0.0.175/32     TI-LFA (18)                -            [ 3 ]    
  2         10.0.0.84/32      TI-LFA (0)                 -            [ 20084 ]
  5         10.0.0.30/32      TI-LFA (16)                -            [ 3 ]    
  6         10.0.0.53/32      TI-LFA (0)                 -            [ 20053 ]
  7         10.0.0.179/32     TI-LFA (0)                 -            [ 20179 ]
  8         10.0.0.120/32     TI-LFA (0)                 -            [ 20120 ]
  9         10.0.0.72/32      TI-LFA (0)                 -            [ 20072 ]
  10        10.0.0.214/32     TI-LFA (0)                 -            [ 20214 ]
  11        10.0.0.128/32     TI-LFA (0)                 -            [ 20128 ]
  13        10.0.0.221/32     TI-LFA (0)                 -            [ 21221 ]
  14        10.0.0.124/32     TI-LFA (0)                 -            [ 20124 ]
  16        10.0.0.217/32     TI-LFA (0)                 -            [ 20217 ]

```

## show isis segment-routing prefix-segments

```text

System ID: Arista-PE32-Q2C-32			Instance: 'IGP'
SR supported Data-plane: MPLS			SR Router ID: 10.0.0.32

Node: 13     Proxy-Node: 0      Prefix: 0       Total Segments: 13

Flag Descriptions: R: Re-advertised, N: Node Segment, P: no-PHP
                   E: Explicit-NULL, V: Value, L: Local
Segment status codes: * - Self originated Prefix, L1 - level 1, L2 - level 2, ! - SR-unreachable,
                      # - Some IS-IS next-hops are SR-unreachable
   Prefix                      SID   Label Type       Flags                        System ID       Level Protection  Algorithm   
   ------------------------- ----- ------- ---------- ---------------------------- --------------- ----- ----------- -------------
   10.0.0.30/32                 30   20030 Node       R:0 N:1 P:0 E:0 V:0 L:0      Arista-Spine3-Q2A-30 L2    node        SPF         
*  10.0.0.32/32                 32   20032 Node       R:0 N:1 P:0 E:0 V:0 L:0      Arista-PE32-Q2C-32 L2    unprotected SPF         
   10.0.0.53/32                 53   20053 Node       R:0 N:1 P:1 E:1 V:0 L:0      Arrcus-53       L2    node        SPF         
   10.0.0.72/32                 72   20072 Node       R:0 N:1 P:0 E:0 V:0 L:0      Ciena-5134-72   L2    node        SPF         
   10.0.0.84/32                 84   20084 Node       R:0 N:1 P:1 E:0 V:0 L:0      Ericsson_84_R6678 L2    node        SPF         
   10.0.0.120/32               120   20120 Node       R:0 N:1 P:0 E:0 V:0 L:0      H3C_M1A_120     L2    node        SPF         
   10.0.0.124/32               124    2124 Node       R:0 N:1 P:1 E:0 V:0 L:0      0000.0000.0124  L2    node        SPF         
   10.0.0.128/32               128   20128 Node       R:0 N:1 P:0 E:0 V:0 L:0      0000.0000.0128  L2    node        SPF         
   10.0.0.175/32               175   20175 Node       R:0 N:1 P:0 E:0 V:0 L:0      Juniper-175-ACX7100-48L L2    node        SPF         
   10.0.0.179/32               179   20179 Node       R:0 N:1 P:0 E:0 V:0 L:0      Juniper-179-ACX7024 L2    node        SPF         
   10.0.0.214/32               214   20214 Node       R:0 N:1 P:1 E:0 V:0 L:0      Nokia-SXR-214   L2    node        SPF         
   10.0.0.217/32               217   20217 Node       R:0 N:1 P:1 E:0 V:0 L:0      Nokia-SR1-217   L2    node        SPF         
   10.0.0.221/32              1221  721221 Node       R:0 N:1 P:0 E:0 V:0 L:0      221             L2    node        SPF         
```

## show traffic-engineering segment-routing policy

```text
Endpoint 10.0.0.53 Color 100, Counters: 171533894 packets, 12767512502 bytes
	Path group: State: active (for 01:32:31), modified: 03:04:25 ago
		Protocol: Static
		Endpoint provisioning: Static
		Originator: 0.0.0.0(AS0)
		Discriminator: 32769
		Preference: 10
		IGP metric: 0 (static)
		Binding SID: 1004053
		Path computation: Configured
		Explicit null label policy: IPv6 (system default)
		Segment List: State: Valid, ID: 1, Counters: 171533894 packets, 12767512502 bytes
		Protected: Yes
			Label Stack: [20030 20053], Weight: 1
			Resolved Label Stack: [20053], Next hop: 20.30.32.30, Interface: Ethernet1
			Backup Resolved Label Stack: [20124 2030 20053], Next hop: 20.32.175.175, Interface: Ethernet5
Endpoint 10.0.0.53 Color 101, Counters: 6245634 packets, 587089756 bytes
	Path group: State: active (for 01:32:24), modified: 03:04:25 ago
		Protocol: Static
		Endpoint provisioning: Static
		Originator: 0.0.0.0(AS0)
		Discriminator: 32769
		Preference: 10
		IGP metric: 0 (static)
		Binding SID: 1006053
		Path computation: Configured
		Explicit null label policy: IPv6 (system default)
		Segment List: State: Valid, ID: 2, Counters: 6245629 packets, 587089126 bytes
		Protected: Yes
			Label Stack: [20175 20053], Weight: 1
			Resolved Label Stack: [20053], Next hop: 20.32.175.175, Interface: Ethernet5
			Backup Resolved Label Stack: [20124 2175 20053], Next hop: 20.30.32.30, Interface: Ethernet1
Endpoint 10.0.0.66 Color 100, Counters: 0 packets, 0 bytes
	Path group: State: active (for 01:32:31), modified: 03:04:25 ago
		Protocol: Static
		Endpoint provisioning: Static
		Originator: 0.0.0.0(AS0)
		Discriminator: 32769
		Preference: 10
		IGP metric: 0 (static)
		Binding SID: 1004066
		Path computation: Configured
		Explicit null label policy: IPv6 (system default)
		Segment List: State: Valid, ID: 3, Counters: 0 packets, 0 bytes (counter not in use)
		Protected: Yes
			Label Stack: [20030 20066], Weight: 1
			Resolved Label Stack: [20066], Next hop: 20.30.32.30, Interface: Ethernet1
			Backup Resolved Label Stack: [20124 2030 20066], Next hop: 20.32.175.175, Interface: Ethernet5
Endpoint 10.0.0.66 Color 101, Counters: 0 packets, 0 bytes
	Path group: State: active (for 01:32:24), modified: 03:04:25 ago
		Protocol: Static
		Endpoint provisioning: Static
		Originator: 0.0.0.0(AS0)
		Discriminator: 32769
		Preference: 10
		IGP metric: 0 (static)
		Binding SID: 1006066
		Path computation: Configured
		Explicit null label policy: IPv6 (system default)
		Segment List: State: Valid, ID: 4, Counters: 0 packets, 0 bytes
		Protected: Yes
			Label Stack: [20175 20066], Weight: 1
			Resolved Label Stack: [20066], Next hop: 20.32.175.175, Interface: Ethernet5
			Backup Resolved Label Stack: [20124 2175 20066], Next hop: 20.30.32.30, Interface: Ethernet1
Endpoint 10.0.0.72 Color 100, Counters: 171990714 packets, 12801371880 bytes
	Path group: State: active (for 01:32:31), modified: 03:04:25 ago
		Protocol: Static
		Endpoint provisioning: Static
		Originator: 0.0.0.0(AS0)
		Discriminator: 32769
		Preference: 10
		IGP metric: 0 (static)
		Binding SID: 1004072
		Path computation: Configured
		Explicit null label policy: IPv6 (system default)
		Segment List: State: Valid, ID: 5, Counters: 171990714 packets, 12801371880 bytes (counter not in use)
		Protected: Yes
			Label Stack: [20030 20072], Weight: 1
			Resolved Label Stack: [20072], Next hop: 20.30.32.30, Interface: Ethernet1
			Backup Resolved Label Stack: [20124 2030 20072], Next hop: 20.32.175.175, Interface: Ethernet5
Endpoint 10.0.0.72 Color 101, Counters: 6245626 packets, 587088844 bytes
	Path group: State: active (for 01:32:24), modified: 03:04:25 ago
		Protocol: Static
		Endpoint provisioning: Static
		Originator: 0.0.0.0(AS0)
		Discriminator: 32769
		Preference: 10
		IGP metric: 0 (static)
		Binding SID: 1006072
		Path computation: Configured
		Explicit null label policy: IPv6 (system default)
		Segment List: State: Valid, ID: 6, Counters: 6245626 packets, 587088844 bytes
		Protected: Yes
			Label Stack: [20175 20072], Weight: 1
			Resolved Label Stack: [20072], Next hop: 20.32.175.175, Interface: Ethernet5
			Backup Resolved Label Stack: [20124 2175 20072], Next hop: 20.30.32.30, Interface: Ethernet1
Endpoint 10.0.0.84 Color 100, Counters: 0 packets, 0 bytes
	Path group: State: active (for 01:32:31), modified: 03:04:25 ago
		Protocol: Static
		Endpoint provisioning: Static
		Originator: 0.0.0.0(AS0)
		Discriminator: 32769
		Preference: 10
		IGP metric: 0 (static)
		Binding SID: 1004084
		Path computation: Configured
		Explicit null label policy: IPv6 (system default)
		Segment List: State: Valid, ID: 7, Counters: 0 packets, 0 bytes (counter not in use)
		Protected: Yes
			Label Stack: [20030 20084], Weight: 1
			Resolved Label Stack: [20084], Next hop: 20.30.32.30, Interface: Ethernet1
			Backup Resolved Label Stack: [20124 2030 20084], Next hop: 20.32.175.175, Interface: Ethernet5
Endpoint 10.0.0.84 Color 101, Counters: 0 packets, 0 bytes
	Path group: State: active (for 01:32:24), modified: 03:04:25 ago
		Protocol: Static
		Endpoint provisioning: Static
		Originator: 0.0.0.0(AS0)
		Discriminator: 32769
		Preference: 10
		IGP metric: 0 (static)
		Binding SID: 1006084
		Path computation: Configured
		Explicit null label policy: IPv6 (system default)
		Segment List: State: Valid, ID: 8, Counters: 0 packets, 0 bytes
		Protected: Yes
			Label Stack: [20175 20084], Weight: 1
			Resolved Label Stack: [20084], Next hop: 20.32.175.175, Interface: Ethernet5
			Backup Resolved Label Stack: [20124 2175 20084], Next hop: 20.30.32.30, Interface: Ethernet1
Endpoint 10.0.0.120 Color 100, Counters: 171992778 packets, 12801578234 bytes
	Path group: State: active (for 01:32:31), modified: 03:04:25 ago
		Protocol: Static
		Endpoint provisioning: Static
		Originator: 0.0.0.0(AS0)
		Discriminator: 32769
		Preference: 10
		IGP metric: 0 (static)
		Binding SID: 1004120
		Path computation: Configured
		Explicit null label policy: IPv6 (system default)
		Segment List: State: Valid, ID: 9, Counters: 171992778 packets, 12801578234 bytes (counter not in use)
		Protected: Yes
			Label Stack: [20030 20120], Weight: 1
			Resolved Label Stack: [20120], Next hop: 20.30.32.30, Interface: Ethernet1
			Backup Resolved Label Stack: [20124 2030 20120], Next hop: 20.32.175.175, Interface: Ethernet5
Endpoint 10.0.0.120 Color 101, Counters: 6245636 packets, 587089784 bytes
	Path group: State: active (for 01:32:24), modified: 03:04:25 ago
		Protocol: Static
		Endpoint provisioning: Static
		Originator: 0.0.0.0(AS0)
		Discriminator: 32769
		Preference: 10
		IGP metric: 0 (static)
		Binding SID: 1006120
		Path computation: Configured
		Explicit null label policy: IPv6 (system default)
		Segment List: State: Valid, ID: 10, Counters: 6245636 packets, 587089784 bytes
		Protected: Yes
			Label Stack: [20175 20120], Weight: 1
			Resolved Label Stack: [20120], Next hop: 20.32.175.175, Interface: Ethernet5
			Backup Resolved Label Stack: [20124 2175 20120], Next hop: 20.30.32.30, Interface: Ethernet1
Endpoint 10.0.0.124 Color 100, Counters: 177284874 packets, 13193247738 bytes
	Path group: State: active (for 01:32:31), modified: 03:04:25 ago
		Protocol: Static
		Endpoint provisioning: Static
		Originator: 0.0.0.0(AS0)
		Discriminator: 32769
		Preference: 10
		IGP metric: 0 (static)
		Binding SID: 1004124
		Path computation: Configured
		Explicit null label policy: IPv6 (system default)
		Segment List: State: Valid, ID: 11, Counters: 177284874 packets, 13193247738 bytes
		Protected: Yes
			Label Stack: [20030 20124], Weight: 1
			Resolved Label Stack: [20124], Next hop: 20.30.32.30, Interface: Ethernet1
			Backup Resolved Label Stack: [20124 2030 20124], Next hop: 20.32.175.175, Interface: Ethernet5
Endpoint 10.0.0.124 Color 101, Counters: 6245644 packets, 587090896 bytes
	Path group: State: active (for 01:32:24), modified: 03:04:25 ago
		Protocol: Static
		Endpoint provisioning: Static
		Originator: 0.0.0.0(AS0)
		Discriminator: 32769
		Preference: 10
		IGP metric: 0 (static)
		Binding SID: 1006124
		Path computation: Configured
		Explicit null label policy: IPv6 (system default)
		Segment List: State: Valid, ID: 12, Counters: 6245644 packets, 587090896 bytes
		Protected: Yes
			Label Stack: [20175 20124], Weight: 1
			Resolved Label Stack: [20124], Next hop: 20.32.175.175, Interface: Ethernet5
			Backup Resolved Label Stack: [20124 2175 20124], Next hop: 20.30.32.30, Interface: Ethernet1
Endpoint 10.0.0.128 Color 100, Counters: 177286958 packets, 13193456184 bytes
	Path group: State: active (for 01:32:31), modified: 03:04:24 ago
		Protocol: Static
		Endpoint provisioning: Static
		Originator: 0.0.0.0(AS0)
		Discriminator: 32769
		Preference: 10
		IGP metric: 0 (static)
		Binding SID: 1004128
		Path computation: Configured
		Explicit null label policy: IPv6 (system default)
		Segment List: State: Valid, ID: 13, Counters: 177286958 packets, 13193456184 bytes
		Protected: Yes
			Label Stack: [20030 20128], Weight: 1
			Resolved Label Stack: [20128], Next hop: 20.30.32.30, Interface: Ethernet1
			Backup Resolved Label Stack: [20124 2030 20128], Next hop: 20.32.175.175, Interface: Ethernet5
Endpoint 10.0.0.128 Color 101, Counters: 6245639 packets, 587090354 bytes
	Path group: State: active (for 01:32:24), modified: 03:04:24 ago
		Protocol: Static
		Endpoint provisioning: Static
		Originator: 0.0.0.0(AS0)
		Discriminator: 32769
		Preference: 10
		IGP metric: 0 (static)
		Binding SID: 1006128
		Path computation: Configured
		Explicit null label policy: IPv6 (system default)
		Segment List: State: Valid, ID: 14, Counters: 6245639 packets, 587090354 bytes
		Protected: Yes
			Label Stack: [20175 20128], Weight: 1
			Resolved Label Stack: [20128], Next hop: 20.32.175.175, Interface: Ethernet5
			Backup Resolved Label Stack: [20124 2175 20128], Next hop: 20.30.32.30, Interface: Ethernet1
Endpoint 10.0.0.179 Color 100, Counters: 3136614334 packets, 236411291994 bytes
	Path group: State: active (for 01:32:31), modified: 03:04:24 ago
		Protocol: Static
		Endpoint provisioning: Static
		Originator: 0.0.0.0(AS0)
		Discriminator: 32769
		Preference: 10
		IGP metric: 0 (static)
		Binding SID: 1004179
		Path computation: Configured
		Explicit null label policy: IPv6 (system default)
		Segment List: State: Valid, ID: 15, Counters: 3136614334 packets, 236411291994 bytes (counter not in use)
		Protected: Yes
			Label Stack: [20030 20179], Weight: 1
			Resolved Label Stack: [20179], Next hop: 20.30.32.30, Interface: Ethernet1
			Backup Resolved Label Stack: [20124 2030 20179], Next hop: 20.32.175.175, Interface: Ethernet5
Endpoint 10.0.0.179 Color 101, Counters: 5959878049 packets, 560300722290 bytes
	Path group: State: active (for 01:32:24), modified: 03:04:24 ago
		Protocol: Static
		Endpoint provisioning: Static
		Originator: 0.0.0.0(AS0)
		Discriminator: 32769
		Preference: 10
		IGP metric: 0 (static)
		Binding SID: 1006179
		Path computation: Configured
		Explicit null label policy: IPv6 (system default)
		Segment List: State: Valid, ID: 16, Counters: 8256759 packets, 735912946 bytes
		Protected: Yes
			Label Stack: [20175 20179], Weight: 1
			Resolved Label Stack: [20179], Next hop: 20.32.175.175, Interface: Ethernet5
			Backup Resolved Label Stack: [20124 2175 20179], Next hop: 20.30.32.30, Interface: Ethernet1
Endpoint 10.0.0.214 Color 100, Counters: 171982384 packets, 12800539484 bytes
	Path group: State: active (for 01:32:31), modified: 03:04:24 ago
		Protocol: Static
		Endpoint provisioning: Static
		Originator: 0.0.0.0(AS0)
		Discriminator: 32769
		Preference: 10
		IGP metric: 0 (static)
		Binding SID: 1004214
		Path computation: Configured
		Explicit null label policy: IPv6 (system default)
		Segment List: State: Valid, ID: 17, Counters: 171982384 packets, 12800539484 bytes (counter not in use)
		Protected: Yes
			Label Stack: [20030 20214], Weight: 1
			Resolved Label Stack: [20214], Next hop: 20.30.32.30, Interface: Ethernet1
			Backup Resolved Label Stack: [20124 2030 20214], Next hop: 20.32.175.175, Interface: Ethernet5
Endpoint 10.0.0.214 Color 101, Counters: 6245642 packets, 587090348 bytes
	Path group: State: active (for 01:32:24), modified: 03:04:24 ago
		Protocol: Static
		Endpoint provisioning: Static
		Originator: 0.0.0.0(AS0)
		Discriminator: 32769
		Preference: 10
		IGP metric: 0 (static)
		Binding SID: 1006214
		Path computation: Configured
		Explicit null label policy: IPv6 (system default)
		Segment List: State: Valid, ID: 18, Counters: 6245642 packets, 587090348 bytes
		Protected: Yes
			Label Stack: [20175 20214], Weight: 1
			Resolved Label Stack: [20214], Next hop: 20.32.175.175, Interface: Ethernet5
			Backup Resolved Label Stack: [20124 2175 20214], Next hop: 20.30.32.30, Interface: Ethernet1
Endpoint 10.0.0.217 Color 100, Counters: 171984532 packets, 12800756182 bytes
	Path group: State: active (for 01:32:31), modified: 03:04:24 ago
		Protocol: Static
		Endpoint provisioning: Static
		Originator: 0.0.0.0(AS0)
		Discriminator: 32769
		Preference: 10
		IGP metric: 0 (static)
		Binding SID: 1004217
		Path computation: Configured
		Explicit null label policy: IPv6 (system default)
		Segment List: State: Valid, ID: 19, Counters: 171984532 packets, 12800756182 bytes
		Protected: Yes
			Label Stack: [20030 20217], Weight: 1
			Resolved Label Stack: [20217], Next hop: 20.30.32.30, Interface: Ethernet1
			Backup Resolved Label Stack: [20124 2030 20217], Next hop: 20.32.175.175, Interface: Ethernet5
Endpoint 10.0.0.217 Color 101, Counters: 6245746 packets, 587103164 bytes
	Path group: State: active (for 01:32:24), modified: 03:04:24 ago
		Protocol: Static
		Endpoint provisioning: Static
		Originator: 0.0.0.0(AS0)
		Discriminator: 32769
		Preference: 10
		IGP metric: 0 (static)
		Binding SID: 1006217
		Path computation: Configured
		Explicit null label policy: IPv6 (system default)
		Segment List: State: Valid, ID: 20, Counters: 6245651 packets, 587091194 bytes
		Protected: Yes
			Label Stack: [20175 20217], Weight: 1
			Resolved Label Stack: [20217], Next hop: 20.32.175.175, Interface: Ethernet5
			Backup Resolved Label Stack: [20124 2175 20217], Next hop: 20.30.32.30, Interface: Ethernet1
Endpoint 10.0.0.221 Color 100, Counters: 171986542 packets, 12800954958 bytes
	Path group: State: active (for 01:32:31), modified: 03:04:24 ago
		Protocol: Static
		Endpoint provisioning: Static
		Originator: 0.0.0.0(AS0)
		Discriminator: 32769
		Preference: 10
		IGP metric: 0 (static)
		Binding SID: 1004221
		Path computation: Configured
		Explicit null label policy: IPv6 (system default)
		Segment List: State: Valid, ID: 21, Counters: 171986542 packets, 12800954958 bytes
		Protected: Yes
			Label Stack: [20030 21221], Weight: 1
			Resolved Label Stack: [21221], Next hop: 20.30.32.30, Interface: Ethernet1
			Backup Resolved Label Stack: [20124 2030 21221], Next hop: 20.32.175.175, Interface: Ethernet5
Endpoint 10.0.0.221 Color 101, Counters: 6245651 packets, 587091410 bytes
	Path group: State: active (for 01:32:24), modified: 03:04:24 ago
		Protocol: Static
		Endpoint provisioning: Static
		Originator: 0.0.0.0(AS0)
		Discriminator: 32769
		Preference: 10
		IGP metric: 0 (static)
		Binding SID: 1006221
		Path computation: Configured
		Explicit null label policy: IPv6 (system default)
		Segment List: State: Valid, ID: 22, Counters: 6245651 packets, 587091410 bytes
		Protected: Yes
			Label Stack: [20175 21221], Weight: 1
			Resolved Label Stack: [21221], Next hop: 20.32.175.175, Interface: Ethernet5
			Backup Resolved Label Stack: [20124 2175 21221], Next hop: 20.30.32.30, Interface: Ethernet1
```

## show mpls segment-routing bindings detail

```text
10.0.0.30/32
   Local binding:  Label: 20030
      Uptime: 1:32:31
   Remote binding: Peer ID: Arista-Spine3-Q2A-30, Label: imp-null
      Uptime: 1:32:31
   Remote binding: Peer ID: 0000.0000.0124, Label: 2030
      Uptime: 1:32:23
   Remote binding: Peer ID: Juniper-175-ACX7100-48L, Label: 20030
      Uptime: 1:32:23
10.0.0.32/32
   Local binding:  Label: imp-null
      Uptime: 1:32:33
   Remote binding: Peer ID: Arista-Spine3-Q2A-30, Label: 20032
      Uptime: 1:32:31
   Remote binding: Peer ID: 0000.0000.0124, Label: 2032
      Uptime: 1:32:23
   Remote binding: Peer ID: Juniper-175-ACX7100-48L, Label: 20032
      Uptime: 1:32:23
10.0.0.53/32
   Local binding:  Label: 20053
      Uptime: 1:32:31
   Remote binding: Peer ID: Arista-Spine3-Q2A-30, Label: 20053
      Uptime: 1:32:31
   Remote binding: Peer ID: 0000.0000.0124, Label: 2053
      Uptime: 1:32:23
   Remote binding: Peer ID: Juniper-175-ACX7100-48L, Label: 20053
      Uptime: 1:32:23
10.0.0.72/32
   Local binding:  Label: 20072
      Uptime: 1:32:31
   Remote binding: Peer ID: Arista-Spine3-Q2A-30, Label: 20072
      Uptime: 1:32:31
   Remote binding: Peer ID: 0000.0000.0124, Label: 2072
      Uptime: 1:32:23
   Remote binding: Peer ID: Juniper-175-ACX7100-48L, Label: 20072
      Uptime: 1:32:23
10.0.0.84/32
   Local binding:  Label: 20084
      Uptime: 1:32:31
   Remote binding: Peer ID: Arista-Spine3-Q2A-30, Label: 20084
      Uptime: 1:32:31
   Remote binding: Peer ID: 0000.0000.0124, Label: 2084
      Uptime: 1:32:23
   Remote binding: Peer ID: Juniper-175-ACX7100-48L, Label: 20084
      Uptime: 1:32:23
10.0.0.120/32
   Local binding:  Label: 20120
      Uptime: 0:21:54
   Remote binding: Peer ID: Arista-Spine3-Q2A-30, Label: 20120
      Uptime: 0:21:54
   Remote binding: Peer ID: 0000.0000.0124, Label: 2120
      Uptime: 0:21:54
   Remote binding: Peer ID: Juniper-175-ACX7100-48L, Label: 20120
      Uptime: 0:21:54
10.0.0.124/32
   Local binding:  Label: 20124
      Uptime: 1:32:31
   Remote binding: Peer ID: Arista-Spine3-Q2A-30, Label: 20124
      Uptime: 1:32:31
   Remote binding: Peer ID: 0000.0000.0124, Label: 2124
      Uptime: 1:32:23
   Remote binding: Peer ID: Juniper-175-ACX7100-48L, Label: 20124
      Uptime: 1:32:23
10.0.0.128/32
   Local binding:  Label: 20128
      Uptime: 1:32:31
   Remote binding: Peer ID: Arista-Spine3-Q2A-30, Label: 20128
      Uptime: 1:32:31
   Remote binding: Peer ID: 0000.0000.0124, Label: 2128
      Uptime: 1:32:23
   Remote binding: Peer ID: Juniper-175-ACX7100-48L, Label: 20128
      Uptime: 1:32:23
10.0.0.175/32
   Local binding:  Label: 20175
      Uptime: 1:32:31
   Remote binding: Peer ID: Arista-Spine3-Q2A-30, Label: 20175
      Uptime: 1:32:31
   Remote binding: Peer ID: 0000.0000.0124, Label: 2175
      Uptime: 1:32:23
   Remote binding: Peer ID: Juniper-175-ACX7100-48L, Label: imp-null
      Uptime: 1:32:23
10.0.0.179/32
   Local binding:  Label: 20179
      Uptime: 1:25:03
   Remote binding: Peer ID: Arista-Spine3-Q2A-30, Label: 20179
      Uptime: 1:25:03
   Remote binding: Peer ID: 0000.0000.0124, Label: 2179
      Uptime: 1:25:03
   Remote binding: Peer ID: Juniper-175-ACX7100-48L, Label: 20179
      Uptime: 1:25:03
10.0.0.214/32
   Local binding:  Label: 20214
      Uptime: 1:32:30
   Remote binding: Peer ID: Arista-Spine3-Q2A-30, Label: 20214
      Uptime: 1:32:30
   Remote binding: Peer ID: 0000.0000.0124, Label: 2214
      Uptime: 1:32:23
   Remote binding: Peer ID: Juniper-175-ACX7100-48L, Label: 20214
      Uptime: 1:32:23
10.0.0.217/32
   Local binding:  Label: 20217
      Uptime: 1:32:30
   Remote binding: Peer ID: Arista-Spine3-Q2A-30, Label: 20217
      Uptime: 1:32:30
   Remote binding: Peer ID: 0000.0000.0124, Label: 2217
      Uptime: 1:32:23
   Remote binding: Peer ID: Juniper-175-ACX7100-48L, Label: 20217
      Uptime: 1:32:23
10.0.0.221/32
   Local binding:  Label: 21221
      Uptime: 1:32:30
   Remote binding: Peer ID: Arista-Spine3-Q2A-30, Label: 21221
      Uptime: 1:32:30
   Remote binding: Peer ID: 0000.0000.0124, Label: 3221
      Uptime: 1:32:23
   Remote binding: Peer ID: Juniper-175-ACX7100-48L, Label: 21221
      Uptime: 1:32:23
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
 I L2     10.0.0.53/32 [115/11]
           via 20.32.175.175, Ethernet5
 I L2     10.0.0.72/32 [115/21]
           via 20.32.175.175, Ethernet5
 I L2     10.0.0.84/32 [115/21]
           via 20.32.175.175, Ethernet5
 I L2     10.0.0.120/32 [115/11]
           via 20.32.175.175, Ethernet5
 I L2     10.0.0.124/32 [115/11]
           via 20.32.175.175, Ethernet5
 I L2     10.0.0.128/32 [115/11]
           via 20.32.175.175, Ethernet5
 I L2     10.0.0.175/32 [115/10]
           via 20.32.175.175, Ethernet5
 I L2     10.0.0.179/32 [115/11]
           via 20.32.175.175, Ethernet5
 I L2     10.0.0.214/32 [115/11]
           via 20.32.175.175, Ethernet5
 I L2     10.0.0.216/32 [115/21]
           via 20.32.175.175, Ethernet5
 I L2     10.0.0.217/32 [115/11]
           via 20.32.175.175, Ethernet5
 I L2     10.0.0.221/32 [115/11]
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
 I L2     20.53.175.0/24 [115/11]
           via 20.32.175.175, Ethernet5
 I L2     20.66.175.0/24 [115/11]
           via 20.32.175.175, Ethernet5
 I L2     20.72.175.0/24 [115/11]
           via 20.32.175.175, Ethernet5
 I L2     20.84.175.0/24 [115/11]
           via 20.32.175.175, Ethernet5
 I L2     20.120.175.0/24 [115/11]
           via 20.32.175.175, Ethernet5
 I L2     20.120.214.0/24 [115/21]
           via 20.32.175.175, Ethernet5
 I L2     20.124.175.0/24 [115/11]
           via 20.32.175.175, Ethernet5
 I L2     20.128.175.0/24 [115/11]
           via 20.32.175.175, Ethernet5
 I L2     20.131.175.0/24 [115/11]
           via 20.32.175.175, Ethernet5
 I L2     20.175.179.0/24 [115/11]
           via 20.32.175.175, Ethernet5
 I L2     20.175.184.0/24 [115/11]
           via 20.32.175.175, Ethernet5
 I L2     20.175.214.0/24 [115/11]
           via 20.32.175.175, Ethernet5
 I L2     20.175.217.0/24 [115/11]
           via 20.32.175.175, Ethernet5
 I L2     20.175.221.0/24 [115/11]
           via 20.32.175.175, Ethernet5
 I L2     20.214.216.0/24 [115/21]
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
 B I      50.10.53.0/24 [200/0]
           via SR-TE Policy 10.0.0.53, color 100, label 970000
              via SR-TE tunnel index 1, weight 1
                 via TI-LFA tunnel index 16, label 20053
                    via 20.30.32.30, Ethernet1, label imp-null(3)
                    backup via 20.32.175.175, Ethernet5, label 20124 2030
 B I      50.10.72.0/24 [200/0]
           via SR-TE Policy 10.0.0.72, color 100, label 62002
              via SR-TE tunnel index 5, weight 1
                 via TI-LFA tunnel index 16, label 20072
                    via 20.30.32.30, Ethernet1, label imp-null(3)
                    backup via 20.32.175.175, Ethernet5, label 20124 2030
 B I      50.10.84.0/24 [200/0]
           via 10.0.0.84/32, IS-IS SR tunnel index 2, label 720896
              via TI-LFA tunnel index 0, label 20084
                 via 20.32.175.175, Ethernet5, label imp-null(3)
                 backup via 20.30.32.30, Ethernet1, label imp-null(3)
 B I      50.10.120.0/24 [200/0]
           via SR-TE Policy 10.0.0.120, color 100, label 1277
              via SR-TE tunnel index 9, weight 1
                 via TI-LFA tunnel index 16, label 20120
                    via 20.30.32.30, Ethernet1, label imp-null(3)
                    backup via 20.32.175.175, Ethernet5, label 20124 2030
 B I      50.10.124.0/24 [200/0]
           via SR-TE Policy 10.0.0.124, color 100, label 332
              via SR-TE tunnel index 11, weight 1
                 via TI-LFA tunnel index 16, label 20124
                    via 20.30.32.30, Ethernet1, label imp-null(3)
                    backup via 20.32.175.175, Ethernet5, label 20124 2030
 B I      50.10.128.0/24 [200/0]
           via SR-TE Policy 10.0.0.128, color 100, label 48060
              via SR-TE tunnel index 13, weight 1
                 via TI-LFA tunnel index 16, label 20128
                    via 20.30.32.30, Ethernet1, label imp-null(3)
                    backup via 20.32.175.175, Ethernet5, label 20124 2030
 B I      50.10.179.0/24 [200/0]
           via SR-TE Policy 10.0.0.179, color 100, label 16
              via SR-TE tunnel index 15, weight 1
                 via TI-LFA tunnel index 16, label 20179
                    via 20.30.32.30, Ethernet1, label imp-null(3)
                    backup via 20.32.175.175, Ethernet5, label 20124 2030
 B I      50.10.214.0/24 [200/0]
           via SR-TE Policy 10.0.0.214, color 100, label 500000
              via SR-TE tunnel index 17, weight 1
                 via TI-LFA tunnel index 16, label 20214
                    via 20.30.32.30, Ethernet1, label imp-null(3)
                    backup via 20.32.175.175, Ethernet5, label 20124 2030
 B I      50.10.217.0/24 [200/0]
           via SR-TE Policy 10.0.0.217, color 100, label 524287
              via SR-TE tunnel index 19, weight 1
                 via TI-LFA tunnel index 16, label 20217
                    via 20.30.32.30, Ethernet1, label imp-null(3)
                    backup via 20.32.175.175, Ethernet5, label 20124 2030
 B I      50.10.221.0/24 [200/0]
           via SR-TE Policy 10.0.0.221, color 100, label 524305
              via SR-TE tunnel index 21, weight 1
                 via TI-LFA tunnel index 16, label 21221
                    via 20.30.32.30, Ethernet1, label imp-null(3)
                    backup via 20.32.175.175, Ethernet5, label 20124 2030
 B I      51.10.120.0/24 [200/0]
           via SR-TE Policy 10.0.0.120, color 100, label 1277
              via SR-TE tunnel index 9, weight 1
                 via TI-LFA tunnel index 16, label 20120
                    via 20.30.32.30, Ethernet1, label imp-null(3)
                    backup via 20.32.175.175, Ethernet5, label 20124 2030

```

## show ipv6 route

```text

VRF: default
Displaying 17 of 22 IPv6 routing table entries
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
 I L2     2001:0:84:175::/64 [115/30]
           via fe80::c6ca:2bff:fe45:a215, Ethernet1
 I L2     2001:0:120:175::/64 [115/30]
           via fe80::c6ca:2bff:fe45:a215, Ethernet1
 I L2     2001:0:120:214::/64 [115/30]
           via fe80::c6ca:2bff:fe45:a215, Ethernet1

```

## show ipv6 route vrf RED

```text

VRF: RED
Displaying 12 of 16 IPv6 routing table entries
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
 B I      2600:50:10:53::/64 [200/0]
           via SR-TE Policy 10.0.0.53, color 101, label 970001
              via SR-TE tunnel index 2, weight 1
                 via TI-LFA tunnel index 18, label 20053
                    via 20.32.175.175, Ethernet5, label imp-null(3)
                    backup via 20.30.32.30, Ethernet1, label 20124 2175
 B I      2600:50:10:72::/64 [200/0]
           via SR-TE Policy 10.0.0.72, color 101, label 62003
              via SR-TE tunnel index 6, weight 1
                 via TI-LFA tunnel index 18, label 20072
                    via 20.32.175.175, Ethernet5, label imp-null(3)
                    backup via 20.30.32.30, Ethernet1, label 20124 2175
 B I      2600:50:10:84::/64 [200/0]
           via 10.0.0.84/32, IS-IS SR tunnel index 2, label 720897
              via TI-LFA tunnel index 0, label 20084
                 via 20.32.175.175, Ethernet5, label imp-null(3)
                 backup via 20.30.32.30, Ethernet1, label imp-null(3)
 B I      2600:50:10:120::/64 [200/0]
           via SR-TE Policy 10.0.0.120, color 101, label 1276
              via SR-TE tunnel index 10, weight 1
                 via TI-LFA tunnel index 18, label 20120
                    via 20.32.175.175, Ethernet5, label imp-null(3)
                    backup via 20.30.32.30, Ethernet1, label 20124 2175
 B I      2600:50:10:124::/64 [200/0]
           via SR-TE Policy 10.0.0.124, color 101, label 333
              via SR-TE tunnel index 12, weight 1
                 via TI-LFA tunnel index 18, label 20124
                    via 20.32.175.175, Ethernet5, label imp-null(3)
                    backup via 20.30.32.30, Ethernet1, label 20124 2175
 B I      2600:50:10:128::/64 [200/0]
           via SR-TE Policy 10.0.0.128, color 101, label 48061
              via SR-TE tunnel index 14, weight 1
                 via TI-LFA tunnel index 18, label 20128
                    via 20.32.175.175, Ethernet5, label imp-null(3)
                    backup via 20.30.32.30, Ethernet1, label 20124 2175
 B I      2600:50:10:179::/64 [200/0]
           via SR-TE Policy 10.0.0.179, color 101, label 16
              via SR-TE tunnel index 16, weight 1
                 via TI-LFA tunnel index 18, label 20179
                    via 20.32.175.175, Ethernet5, label imp-null(3)
                    backup via 20.30.32.30, Ethernet1, label 20124 2175
 B I      2600:50:10:214::/64 [200/0]
           via SR-TE Policy 10.0.0.214, color 101, label 500000
              via SR-TE tunnel index 18, weight 1
                 via TI-LFA tunnel index 18, label 20214
                    via 20.32.175.175, Ethernet5, label imp-null(3)
                    backup via 20.30.32.30, Ethernet1, label 20124 2175
 B I      2600:50:10:217::/64 [200/0]
           via SR-TE Policy 10.0.0.217, color 101, label 524287
              via SR-TE tunnel index 20, weight 1
                 via TI-LFA tunnel index 18, label 20217
                    via 20.32.175.175, Ethernet5, label imp-null(3)
                    backup via 20.30.32.30, Ethernet1, label 20124 2175
 B I      2600:50:10:221::/64 [200/0]
           via SR-TE Policy 10.0.0.221, color 101, label 524305
              via SR-TE tunnel index 22, weight 1
                 via TI-LFA tunnel index 18, label 21221
                    via 20.32.175.175, Ethernet5, label imp-null(3)
                    backup via 20.30.32.30, Ethernet1, label 20124 2175
 B I      2600:51:10:120::/64 [200/0]
           via SR-TE Policy 10.0.0.120, color 101, label 1276
              via SR-TE tunnel index 10, weight 1
                 via TI-LFA tunnel index 18, label 20120
                    via 20.32.175.175, Ethernet5, label imp-null(3)
                    backup via 20.30.32.30, Ethernet1, label 20124 2175

```

## show mpls route

```text
MPLS forwarding table (Label [metric] Vias) - 39 routes 
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
                  via TI-LFA tunnel index 16
                    via 20.30.32.30, Ethernet1, label imp-null(3)
                    backup via 20.32.175.175, Ethernet5, label 20124 2030
 20053   A[1]
                via M, ::, forward
                    EgressACL: apply
                  via TI-LFA tunnel index 0
                    via 20.32.175.175, Ethernet5, label imp-null(3)
                    backup via 20.30.32.30, Ethernet1, label imp-null(3)
 20072   A[1]
                via M, ::, forward
                    EgressACL: apply
                  via TI-LFA tunnel index 0
                    via 20.32.175.175, Ethernet5, label imp-null(3)
                    backup via 20.30.32.30, Ethernet1, label imp-null(3)
 20084   A[1]
                via M, ::, forward
                    EgressACL: apply
                  via TI-LFA tunnel index 0
                    via 20.32.175.175, Ethernet5, label imp-null(3)
                    backup via 20.30.32.30, Ethernet1, label imp-null(3)
 20120   A[1]
                via M, ::, forward
                    EgressACL: apply
                  via TI-LFA tunnel index 0
                    via 20.32.175.175, Ethernet5, label imp-null(3)
                    backup via 20.30.32.30, Ethernet1, label imp-null(3)
 20124   A[1]
                via M, ::, forward
                    EgressACL: apply
                  via TI-LFA tunnel index 0
                    via 20.32.175.175, Ethernet5, label imp-null(3)
                    backup via 20.30.32.30, Ethernet1, label imp-null(3)
 20128   A[1]
                via M, ::, forward
                    EgressACL: apply
                  via TI-LFA tunnel index 0
                    via 20.32.175.175, Ethernet5, label imp-null(3)
                    backup via 20.30.32.30, Ethernet1, label imp-null(3)
 20175   A[1]
                via M, ::, pop
                    EgressACL: apply
                  via TI-LFA tunnel index 18
                    via 20.32.175.175, Ethernet5, label imp-null(3)
                    backup via 20.30.32.30, Ethernet1, label 20124 2175
 20179   A[1]
                via M, ::, forward
                    EgressACL: apply
                  via TI-LFA tunnel index 0
                    via 20.32.175.175, Ethernet5, label imp-null(3)
                    backup via 20.30.32.30, Ethernet1, label imp-null(3)
 20214   A[1]
                via M, ::, forward
                    EgressACL: apply
                  via TI-LFA tunnel index 0
                    via 20.32.175.175, Ethernet5, label imp-null(3)
                    backup via 20.30.32.30, Ethernet1, label imp-null(3)
 20217   A[1]
                via M, ::, forward
                    EgressACL: apply
                  via TI-LFA tunnel index 0
                    via 20.32.175.175, Ethernet5, label imp-null(3)
                    backup via 20.30.32.30, Ethernet1, label imp-null(3)
 21221   A[1]
                via M, ::, forward
                    EgressACL: apply
                  via TI-LFA tunnel index 0
                    via 20.32.175.175, Ethernet5, label imp-null(3)
                    backup via 20.30.32.30, Ethernet1, label imp-null(3)
 362156  A[1]
                via M, 20.30.32.30, pop
                    EgressACL: apply
                    directly connected, Ethernet1
                    c4:ca:2b:45:a2:15, vlan 1006
 362157  A[1]
                via M, fe80::c6ca:2bff:fe45:a215, pop
                    EgressACL: apply
                    directly connected, Ethernet1
                    c4:ca:2b:45:a2:15, vlan 1006
 362158  A[1]
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
                  via SR-TE tunnel index 1
                    via TI-LFA tunnel index 16, label 20053
                       via 20.30.32.30, Ethernet1, label imp-null(3)
                       backup via 20.32.175.175, Ethernet5, label 20124 2030
 1004066 A[1]
                SR-TE Policy 10.0.0.66, color 100, pop
                    EgressACL: apply
                  via SR-TE tunnel index 3
                    via TI-LFA tunnel index 16, label 20066
                       via 20.30.32.30, Ethernet1, label imp-null(3)
                       backup via 20.32.175.175, Ethernet5, label 20124 2030
 1004072 A[1]
                SR-TE Policy 10.0.0.72, color 100, pop
                    EgressACL: apply
                  via SR-TE tunnel index 5
                    via TI-LFA tunnel index 16, label 20072
                       via 20.30.32.30, Ethernet1, label imp-null(3)
                       backup via 20.32.175.175, Ethernet5, label 20124 2030
 1004084 A[1]
                SR-TE Policy 10.0.0.84, color 100, pop
                    EgressACL: apply
                  via SR-TE tunnel index 7
                    via TI-LFA tunnel index 16, label 20084
                       via 20.30.32.30, Ethernet1, label imp-null(3)
                       backup via 20.32.175.175, Ethernet5, label 20124 2030
 1004120 A[1]
                SR-TE Policy 10.0.0.120, color 100, pop
                    EgressACL: apply
                  via SR-TE tunnel index 9
                    via TI-LFA tunnel index 16, label 20120
                       via 20.30.32.30, Ethernet1, label imp-null(3)
                       backup via 20.32.175.175, Ethernet5, label 20124 2030
 1004124 A[1]
                SR-TE Policy 10.0.0.124, color 100, pop
                    EgressACL: apply
                  via SR-TE tunnel index 11
                    via TI-LFA tunnel index 16, label 20124
                       via 20.30.32.30, Ethernet1, label imp-null(3)
                       backup via 20.32.175.175, Ethernet5, label 20124 2030
 1004128 A[1]
                SR-TE Policy 10.0.0.128, color 100, pop
                    EgressACL: apply
                  via SR-TE tunnel index 13
                    via TI-LFA tunnel index 16, label 20128
                       via 20.30.32.30, Ethernet1, label imp-null(3)
                       backup via 20.32.175.175, Ethernet5, label 20124 2030
 1004179 A[1]
                SR-TE Policy 10.0.0.179, color 100, pop
                    EgressACL: apply
                  via SR-TE tunnel index 15
                    via TI-LFA tunnel index 16, label 20179
                       via 20.30.32.30, Ethernet1, label imp-null(3)
                       backup via 20.32.175.175, Ethernet5, label 20124 2030
 1004214 A[1]
                SR-TE Policy 10.0.0.214, color 100, pop
                    EgressACL: apply
                  via SR-TE tunnel index 17
                    via TI-LFA tunnel index 16, label 20214
                       via 20.30.32.30, Ethernet1, label imp-null(3)
                       backup via 20.32.175.175, Ethernet5, label 20124 2030
 1004217 A[1]
                SR-TE Policy 10.0.0.217, color 100, pop
                    EgressACL: apply
                  via SR-TE tunnel index 19
                    via TI-LFA tunnel index 16, label 20217
                       via 20.30.32.30, Ethernet1, label imp-null(3)
                       backup via 20.32.175.175, Ethernet5, label 20124 2030
 1004221 A[1]
                SR-TE Policy 10.0.0.221, color 100, pop
                    EgressACL: apply
                  via SR-TE tunnel index 21
                    via TI-LFA tunnel index 16, label 21221
                       via 20.30.32.30, Ethernet1, label imp-null(3)
                       backup via 20.32.175.175, Ethernet5, label 20124 2030
 1006053 A[1]
                SR-TE Policy 10.0.0.53, color 101, pop
                    EgressACL: apply
                  via SR-TE tunnel index 2
                    via TI-LFA tunnel index 18, label 20053
                       via 20.32.175.175, Ethernet5, label imp-null(3)
                       backup via 20.30.32.30, Ethernet1, label 20124 2175
 1006066 A[1]
                SR-TE Policy 10.0.0.66, color 101, pop
                    EgressACL: apply
                  via SR-TE tunnel index 4
                    via TI-LFA tunnel index 18, label 20066
                       via 20.32.175.175, Ethernet5, label imp-null(3)
                       backup via 20.30.32.30, Ethernet1, label 20124 2175
 1006072 A[1]
                SR-TE Policy 10.0.0.72, color 101, pop
                    EgressACL: apply
                  via SR-TE tunnel index 6
                    via TI-LFA tunnel index 18, label 20072
                       via 20.32.175.175, Ethernet5, label imp-null(3)
                       backup via 20.30.32.30, Ethernet1, label 20124 2175
 1006084 A[1]
                SR-TE Policy 10.0.0.84, color 101, pop
                    EgressACL: apply
                  via SR-TE tunnel index 8
                    via TI-LFA tunnel index 18, label 20084
                       via 20.32.175.175, Ethernet5, label imp-null(3)
                       backup via 20.30.32.30, Ethernet1, label 20124 2175
 1006120 A[1]
                SR-TE Policy 10.0.0.120, color 101, pop
                    EgressACL: apply
                  via SR-TE tunnel index 10
                    via TI-LFA tunnel index 18, label 20120
                       via 20.32.175.175, Ethernet5, label imp-null(3)
                       backup via 20.30.32.30, Ethernet1, label 20124 2175
 1006124 A[1]
                SR-TE Policy 10.0.0.124, color 101, pop
                    EgressACL: apply
                  via SR-TE tunnel index 12
                    via TI-LFA tunnel index 18, label 20124
                       via 20.32.175.175, Ethernet5, label imp-null(3)
                       backup via 20.30.32.30, Ethernet1, label 20124 2175
 1006128 A[1]
                SR-TE Policy 10.0.0.128, color 101, pop
                    EgressACL: apply
                  via SR-TE tunnel index 14
                    via TI-LFA tunnel index 18, label 20128
                       via 20.32.175.175, Ethernet5, label imp-null(3)
                       backup via 20.30.32.30, Ethernet1, label 20124 2175
 1006179 A[1]
                SR-TE Policy 10.0.0.179, color 101, pop
                    EgressACL: apply
                  via SR-TE tunnel index 16
                    via TI-LFA tunnel index 18, label 20179
                       via 20.32.175.175, Ethernet5, label imp-null(3)
                       backup via 20.30.32.30, Ethernet1, label 20124 2175
 1006214 A[1]
                SR-TE Policy 10.0.0.214, color 101, pop
                    EgressACL: apply
                  via SR-TE tunnel index 18
                    via TI-LFA tunnel index 18, label 20214
                       via 20.32.175.175, Ethernet5, label imp-null(3)
                       backup via 20.30.32.30, Ethernet1, label 20124 2175
 1006217 A[1]
                SR-TE Policy 10.0.0.217, color 101, pop
                    EgressACL: apply
                  via SR-TE tunnel index 20
                    via TI-LFA tunnel index 18, label 20217
                       via 20.32.175.175, Ethernet5, label imp-null(3)
                       backup via 20.30.32.30, Ethernet1, label 20124 2175
 1006221 A[1]
                SR-TE Policy 10.0.0.221, color 101, pop
                    EgressACL: apply
                  via SR-TE tunnel index 22
                    via TI-LFA tunnel index 18, label 21221
                       via 20.32.175.175, Ethernet5, label imp-null(3)
                       backup via 20.30.32.30, Ethernet1, label 20124 2175
```

## show mpls lfib route

```text
MPLS forwarding table (Label [metric] Vias) - 39 routes 
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
                via TI-LFA tunnel index 16, pop
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                    via 20.30.32.30, Ethernet1, label imp-null(3)
                    backup via 20.32.175.175, Ethernet5, label 20124 2030
 IP    20053    [1], 10.0.0.53/32
                via TI-LFA tunnel index 0, forward
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                    via 20.32.175.175, Ethernet5, label imp-null(3)
                    backup via 20.30.32.30, Ethernet1, label imp-null(3)
 IP    20072    [1], 10.0.0.72/32
                via TI-LFA tunnel index 0, forward
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                    via 20.32.175.175, Ethernet5, label imp-null(3)
                    backup via 20.30.32.30, Ethernet1, label imp-null(3)
 IP    20084    [1], 10.0.0.84/32
                via TI-LFA tunnel index 0, forward
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                    via 20.32.175.175, Ethernet5, label imp-null(3)
                    backup via 20.30.32.30, Ethernet1, label imp-null(3)
 IP    20120    [1], 10.0.0.120/32
                via TI-LFA tunnel index 0, forward
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                    via 20.32.175.175, Ethernet5, label imp-null(3)
                    backup via 20.30.32.30, Ethernet1, label imp-null(3)
 IP    20124    [1], 10.0.0.124/32
                via TI-LFA tunnel index 0, forward
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                    via 20.32.175.175, Ethernet5, label imp-null(3)
                    backup via 20.30.32.30, Ethernet1, label imp-null(3)
 IP    20128    [1], 10.0.0.128/32
                via TI-LFA tunnel index 0, forward
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                    via 20.32.175.175, Ethernet5, label imp-null(3)
                    backup via 20.30.32.30, Ethernet1, label imp-null(3)
 IP    20175    [1], 10.0.0.175/32
                via TI-LFA tunnel index 18, pop
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                    via 20.32.175.175, Ethernet5, label imp-null(3)
                    backup via 20.30.32.30, Ethernet1, label 20124 2175
 IP    20179    [1], 10.0.0.179/32
                via TI-LFA tunnel index 0, forward
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                    via 20.32.175.175, Ethernet5, label imp-null(3)
                    backup via 20.30.32.30, Ethernet1, label imp-null(3)
 IP    20214    [1], 10.0.0.214/32
                via TI-LFA tunnel index 0, forward
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                    via 20.32.175.175, Ethernet5, label imp-null(3)
                    backup via 20.30.32.30, Ethernet1, label imp-null(3)
 IP    20217    [1], 10.0.0.217/32
                via TI-LFA tunnel index 0, forward
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                    via 20.32.175.175, Ethernet5, label imp-null(3)
                    backup via 20.30.32.30, Ethernet1, label imp-null(3)
 IP    21221    [1], 10.0.0.221/32
                via TI-LFA tunnel index 0, forward
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                    via 20.32.175.175, Ethernet5, label imp-null(3)
                    backup via 20.30.32.30, Ethernet1, label imp-null(3)
 IA    362156   [1]
                via M, 20.30.32.30, pop
                 payload autoDecide, ttlMode uniform, apply egress-acl
                 interface Ethernet1
 IA    362157   [1]
                via M, fe80::c6ca:2bff:fe45:a215, pop
                 payload autoDecide, ttlMode uniform, apply egress-acl
                 interface Ethernet1
 IA    362158   [1]
                via M, 20.32.175.175, pop
                 payload autoDecide, ttlMode uniform, apply egress-acl
                 interface Ethernet5
 B3    378528   [0]
                via I, ipv4, vrf RED
 B3    378529   [0]
                via I, ipv6, vrf RED
 ST    1004053  [1], SR-TE Policy 10.0.0.53, color 100
                via SR-TE tunnel index 1, pop
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                    via TI-LFA tunnel index 16, label 20053
                       via 20.30.32.30, Ethernet1, label imp-null(3)
                       backup via 20.32.175.175, Ethernet5, label 20124 2030
 ST    1004066  [1], SR-TE Policy 10.0.0.66, color 100
                via SR-TE tunnel index 3, pop
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                    via TI-LFA tunnel index 16, label 20066
                       via 20.30.32.30, Ethernet1, label imp-null(3)
                       backup via 20.32.175.175, Ethernet5, label 20124 2030
 ST    1004072  [1], SR-TE Policy 10.0.0.72, color 100
                via SR-TE tunnel index 5, pop
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                    via TI-LFA tunnel index 16, label 20072
                       via 20.30.32.30, Ethernet1, label imp-null(3)
                       backup via 20.32.175.175, Ethernet5, label 20124 2030
 ST    1004084  [1], SR-TE Policy 10.0.0.84, color 100
                via SR-TE tunnel index 7, pop
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                    via TI-LFA tunnel index 16, label 20084
                       via 20.30.32.30, Ethernet1, label imp-null(3)
                       backup via 20.32.175.175, Ethernet5, label 20124 2030
 ST    1004120  [1], SR-TE Policy 10.0.0.120, color 100
                via SR-TE tunnel index 9, pop
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                    via TI-LFA tunnel index 16, label 20120
                       via 20.30.32.30, Ethernet1, label imp-null(3)
                       backup via 20.32.175.175, Ethernet5, label 20124 2030
 ST    1004124  [1], SR-TE Policy 10.0.0.124, color 100
                via SR-TE tunnel index 11, pop
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                    via TI-LFA tunnel index 16, label 20124
                       via 20.30.32.30, Ethernet1, label imp-null(3)
                       backup via 20.32.175.175, Ethernet5, label 20124 2030
 ST    1004128  [1], SR-TE Policy 10.0.0.128, color 100
                via SR-TE tunnel index 13, pop
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                    via TI-LFA tunnel index 16, label 20128
                       via 20.30.32.30, Ethernet1, label imp-null(3)
                       backup via 20.32.175.175, Ethernet5, label 20124 2030
 ST    1004179  [1], SR-TE Policy 10.0.0.179, color 100
                via SR-TE tunnel index 15, pop
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                    via TI-LFA tunnel index 16, label 20179
                       via 20.30.32.30, Ethernet1, label imp-null(3)
                       backup via 20.32.175.175, Ethernet5, label 20124 2030
 ST    1004214  [1], SR-TE Policy 10.0.0.214, color 100
                via SR-TE tunnel index 17, pop
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                    via TI-LFA tunnel index 16, label 20214
                       via 20.30.32.30, Ethernet1, label imp-null(3)
                       backup via 20.32.175.175, Ethernet5, label 20124 2030
 ST    1004217  [1], SR-TE Policy 10.0.0.217, color 100
                via SR-TE tunnel index 19, pop
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                    via TI-LFA tunnel index 16, label 20217
                       via 20.30.32.30, Ethernet1, label imp-null(3)
                       backup via 20.32.175.175, Ethernet5, label 20124 2030
 ST    1004221  [1], SR-TE Policy 10.0.0.221, color 100
                via SR-TE tunnel index 21, pop
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                    via TI-LFA tunnel index 16, label 21221
                       via 20.30.32.30, Ethernet1, label imp-null(3)
                       backup via 20.32.175.175, Ethernet5, label 20124 2030
 ST    1006053  [1], SR-TE Policy 10.0.0.53, color 101
                via SR-TE tunnel index 2, pop
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                    via TI-LFA tunnel index 18, label 20053
                       via 20.32.175.175, Ethernet5, label imp-null(3)
                       backup via 20.30.32.30, Ethernet1, label 20124 2175
 ST    1006066  [1], SR-TE Policy 10.0.0.66, color 101
                via SR-TE tunnel index 4, pop
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                    via TI-LFA tunnel index 18, label 20066
                       via 20.32.175.175, Ethernet5, label imp-null(3)
                       backup via 20.30.32.30, Ethernet1, label 20124 2175
 ST    1006072  [1], SR-TE Policy 10.0.0.72, color 101
                via SR-TE tunnel index 6, pop
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                    via TI-LFA tunnel index 18, label 20072
                       via 20.32.175.175, Ethernet5, label imp-null(3)
                       backup via 20.30.32.30, Ethernet1, label 20124 2175
 ST    1006084  [1], SR-TE Policy 10.0.0.84, color 101
                via SR-TE tunnel index 8, pop
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                    via TI-LFA tunnel index 18, label 20084
                       via 20.32.175.175, Ethernet5, label imp-null(3)
                       backup via 20.30.32.30, Ethernet1, label 20124 2175
 ST    1006120  [1], SR-TE Policy 10.0.0.120, color 101
                via SR-TE tunnel index 10, pop
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                    via TI-LFA tunnel index 18, label 20120
                       via 20.32.175.175, Ethernet5, label imp-null(3)
                       backup via 20.30.32.30, Ethernet1, label 20124 2175
 ST    1006124  [1], SR-TE Policy 10.0.0.124, color 101
                via SR-TE tunnel index 12, pop
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                    via TI-LFA tunnel index 18, label 20124
                       via 20.32.175.175, Ethernet5, label imp-null(3)
                       backup via 20.30.32.30, Ethernet1, label 20124 2175
 ST    1006128  [1], SR-TE Policy 10.0.0.128, color 101
                via SR-TE tunnel index 14, pop
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                    via TI-LFA tunnel index 18, label 20128
                       via 20.32.175.175, Ethernet5, label imp-null(3)
                       backup via 20.30.32.30, Ethernet1, label 20124 2175
 ST    1006179  [1], SR-TE Policy 10.0.0.179, color 101
                via SR-TE tunnel index 16, pop
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                    via TI-LFA tunnel index 18, label 20179
                       via 20.32.175.175, Ethernet5, label imp-null(3)
                       backup via 20.30.32.30, Ethernet1, label 20124 2175
 ST    1006214  [1], SR-TE Policy 10.0.0.214, color 101
                via SR-TE tunnel index 18, pop
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                    via TI-LFA tunnel index 18, label 20214
                       via 20.32.175.175, Ethernet5, label imp-null(3)
                       backup via 20.30.32.30, Ethernet1, label 20124 2175
 ST    1006217  [1], SR-TE Policy 10.0.0.217, color 101
                via SR-TE tunnel index 20, pop
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                    via TI-LFA tunnel index 18, label 20217
                       via 20.32.175.175, Ethernet5, label imp-null(3)
                       backup via 20.30.32.30, Ethernet1, label 20124 2175
 ST    1006221  [1], SR-TE Policy 10.0.0.221, color 101
                via SR-TE tunnel index 22, pop
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                    via TI-LFA tunnel index 18, label 21221
                       via 20.32.175.175, Ethernet5, label imp-null(3)
                       backup via 20.30.32.30, Ethernet1, label 20124 2175
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

## show bgp vpn-ipv4 detail

```text
BGP routing table information for VRF default
Router identifier 10.0.0.32, local AS number 64512
BGP routing table entry for IPv4 prefix 50.10.32.0/24, Route Distinguisher: 10.0.0.32:5001
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best, redistributed (Connected)
      Extended Community: Route-Target-AS:5001:5001
      Local MPLS label (VRF label): 378528
BGP routing table entry for IPv4 prefix 50.10.53.0/24, Route Distinguisher: 53:5001
 Paths: 2 available
  Local
    10.0.0.53 from 10.0.0.30 (10.0.0.30)
      Origin INCOMPLETE, metric -, localpref 100, weight 0, tag 0, valid, internal, ECMP head, ECMP, best, ECMP contributor
      Originator: 10.0.0.53, Cluster list: 10.0.0.30 
      Extended Community: Route-Target-AS:5001:5001 Color:CO(00):100
      Remote MPLS label: 970000
  Local
    10.0.0.53 from 10.0.0.175 (10.0.0.175)
      Origin INCOMPLETE, metric -, localpref 100, weight 0, tag 0, valid, internal, ECMP, ECMP contributor
      Originator: 10.0.0.53, Cluster list: 10.0.0.175 
      Extended Community: Route-Target-AS:5001:5001 Color:CO(00):100
      Remote MPLS label: 970000
BGP routing table entry for IPv4 prefix 50.10.72.0/24, Route Distinguisher: 72:5001
 Paths: 2 available
  Local
    10.0.0.72 from 10.0.0.30 (10.0.0.30)
      Origin INCOMPLETE, metric -, localpref 100, weight 0, tag 0, valid, internal, ECMP head, ECMP, best, ECMP contributor
      Originator: 10.0.0.72, Cluster list: 10.0.0.30 
      Extended Community: Route-Target-AS:5001:5001 Color:CO(00):100
      Remote MPLS label: 62002
  Local
    10.0.0.72 from 10.0.0.175 (10.0.0.175)
      Origin INCOMPLETE, metric -, localpref 100, weight 0, tag 0, valid, internal, ECMP, ECMP contributor
      Originator: 10.0.0.72, Cluster list: 10.0.0.175 
      Extended Community: Route-Target-AS:5001:5001 Color:CO(00):100
      Remote MPLS label: 62002
BGP routing table entry for IPv4 prefix 50.10.84.0/24, Route Distinguisher: 84:5001
 Paths: 2 available
  Local
    10.0.0.84 from 10.0.0.30 (10.0.0.30)
      Origin INCOMPLETE, metric 0, localpref 100, weight 0, tag 0, valid, internal, ECMP head, ECMP, best, ECMP contributor
      Originator: 10.0.0.84, Cluster list: 10.0.0.30 
      Extended Community: Route-Target-AS:5001:5001
      Remote MPLS label: 720896
  Local
    10.0.0.84 from 10.0.0.175 (10.0.0.175)
      Origin INCOMPLETE, metric 0, localpref 100, weight 0, tag 0, valid, internal, ECMP, ECMP contributor
      Originator: 10.0.0.84, Cluster list: 10.0.0.175 
      Extended Community: Route-Target-AS:5001:5001
      Remote MPLS label: 720896
BGP routing table entry for IPv4 prefix 50.10.120.0/24, Route Distinguisher: 120:5001
 Paths: 2 available
  Local
    10.0.0.120 from 10.0.0.30 (10.0.0.30)
      Origin INCOMPLETE, metric 0, localpref 100, weight 0, tag 0, valid, internal, ECMP head, ECMP, best, ECMP contributor
      Originator: 10.0.0.120, Cluster list: 10.0.0.30 
      Extended Community: Route-Target-AS:5001:5001 Color:CO(00):100
      Remote MPLS label: 1277
  Local
    10.0.0.120 from 10.0.0.175 (10.0.0.175)
      Origin INCOMPLETE, metric 0, localpref 100, weight 0, tag 0, valid, internal, ECMP, ECMP contributor
      Originator: 10.0.0.120, Cluster list: 10.0.0.175 
      Extended Community: Route-Target-AS:5001:5001 Color:CO(00):100
      Remote MPLS label: 1277
BGP routing table entry for IPv4 prefix 50.10.124.0/24, Route Distinguisher: 124:5001
 Paths: 1 available
  Local
    10.0.0.124 from 10.0.0.175 (10.0.0.175)
      Origin INCOMPLETE, metric 0, localpref 100, weight 0, tag 0, valid, internal, best
      Originator: 10.0.0.124, Cluster list: 10.0.0.175 
      Extended Community: Route-Target-AS:5001:5001 Color:CO(00):100
      Remote MPLS label: 332
BGP routing table entry for IPv4 prefix 50.10.128.0/24, Route Distinguisher: 128:5001
 Paths: 1 available
  Local
    10.0.0.128 from 10.0.0.175 (10.0.0.175)
      Origin INCOMPLETE, metric 0, localpref 100, weight 0, tag 0, valid, internal, best
      Originator: 10.0.0.128, Cluster list: 10.0.0.175 
      Extended Community: Route-Target-AS:5001:5001 Color:CO(00):100
      Remote MPLS label: 48060
BGP routing table entry for IPv4 prefix 50.10.179.0/24, Route Distinguisher: 179:5001
 Paths: 2 available
  Local
    10.0.0.179 from 10.0.0.30 (10.0.0.30)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, ECMP head, ECMP, best, ECMP contributor
      Originator: 10.0.0.179, Cluster list: 10.0.0.30 
      Extended Community: Route-Target-AS:5001:5001 Color:CO(00):100
      Remote MPLS label: 16
  Local
    10.0.0.179 from 10.0.0.175 (10.0.0.175)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, ECMP, ECMP contributor
      Originator: 10.0.0.179, Cluster list: 10.0.0.175 
      Extended Community: Route-Target-AS:5001:5001 Color:CO(00):100
      Remote MPLS label: 16
BGP routing table entry for IPv4 prefix 50.10.214.0/24, Route Distinguisher: 214:5001
 Paths: 2 available
  Local
    10.0.0.214 from 10.0.0.30 (10.0.0.30)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, ECMP head, ECMP, best, ECMP contributor
      Originator: 10.0.0.214, Cluster list: 10.0.0.30 
      Extended Community: Route-Target-AS:5001:5001 Color:CO(00):100
      Remote MPLS label: 500000
  Local
    10.0.0.214 from 10.0.0.175 (10.0.0.175)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, ECMP, ECMP contributor
      Originator: 10.0.0.214, Cluster list: 10.0.0.175 
      Extended Community: Route-Target-AS:5001:5001 Color:CO(00):100
      Remote MPLS label: 500000
BGP routing table entry for IPv4 prefix 50.10.217.0/24, Route Distinguisher: 217:5001
 Paths: 2 available
  Local
    10.0.0.217 from 10.0.0.30 (10.0.0.30)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, ECMP head, ECMP, best, ECMP contributor
      Originator: 10.0.0.217, Cluster list: 10.0.0.30 
      Extended Community: Route-Target-AS:5001:5001 Color:CO(00):100
      Remote MPLS label: 524287
  Local
    10.0.0.217 from 10.0.0.175 (10.0.0.175)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, ECMP, ECMP contributor
      Originator: 10.0.0.217, Cluster list: 10.0.0.175 
      Extended Community: Route-Target-AS:5001:5001 Color:CO(00):100
      Remote MPLS label: 524287
BGP routing table entry for IPv4 prefix 50.10.221.0/24, Route Distinguisher: 210:5001
 Paths: 2 available
  Local
    10.0.0.221 from 10.0.0.30 (10.0.0.30)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, ECMP head, ECMP, best, ECMP contributor
      Originator: 10.0.0.221, Cluster list: 10.0.0.30 
      Extended Community: Route-Target-AS:5001:5001 Color:CO(00):100
      Remote MPLS label: 524305
  Local
    10.0.0.221 from 10.0.0.175 (10.0.0.175)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, ECMP, ECMP contributor
      Originator: 10.0.0.221, Cluster list: 10.0.0.175 
      Extended Community: Route-Target-AS:5001:5001 Color:CO(00):100
      Remote MPLS label: 524305
BGP routing table entry for IPv4 prefix 51.10.120.0/24, Route Distinguisher: 120:5001
 Paths: 2 available
  Local
    10.0.0.120 from 10.0.0.30 (10.0.0.30)
      Origin INCOMPLETE, metric 0, localpref 100, weight 0, tag 0, valid, internal, ECMP head, ECMP, best, ECMP contributor
      Originator: 10.0.0.120, Cluster list: 10.0.0.30 
      Extended Community: Route-Target-AS:5001:5001 Color:CO(00):100
      Remote MPLS label: 1277
  Local
    10.0.0.120 from 10.0.0.175 (10.0.0.175)
      Origin INCOMPLETE, metric 0, localpref 100, weight 0, tag 0, valid, internal, ECMP, ECMP contributor
      Originator: 10.0.0.120, Cluster list: 10.0.0.175 
      Extended Community: Route-Target-AS:5001:5001 Color:CO(00):100
      Remote MPLS label: 1277
```

## show bgp vpn-ipv6 detail

```text
BGP routing table information for VRF default
Router identifier 10.0.0.32, local AS number 64512
BGP routing table entry for IPv6 prefix 2600:50:10:32::/64, Route Distinguisher: 10.0.0.32:5001
 Paths: 1 available
  Local
    - from - (0.0.0.0)
      Origin IGP, metric -, localpref -, weight 0, tag 0, valid, local, best, redistributed (Connected)
      Extended Community: Route-Target-AS:5001:5001
      Local MPLS label (VRF label): 378529
BGP routing table entry for IPv6 prefix 2600:50:10:53::/64, Route Distinguisher: 53:5001
 Paths: 2 available
  Local
    ::ffff:10.0.0.53 from 10.0.0.30 (10.0.0.30)
      Origin INCOMPLETE, metric -, localpref 100, weight 0, tag 0, valid, internal, ECMP head, ECMP, best, ECMP contributor
      Originator: 10.0.0.53, Cluster list: 10.0.0.30 
      Extended Community: Route-Target-AS:5001:5001 Color:CO(00):101
      Remote MPLS label: 970001
  Local
    ::ffff:10.0.0.53 from 10.0.0.175 (10.0.0.175)
      Origin INCOMPLETE, metric -, localpref 100, weight 0, tag 0, valid, internal, ECMP, ECMP contributor
      Originator: 10.0.0.53, Cluster list: 10.0.0.175 
      Extended Community: Route-Target-AS:5001:5001 Color:CO(00):101
      Remote MPLS label: 970001
BGP routing table entry for IPv6 prefix 2600:50:10:72::/64, Route Distinguisher: 72:5001
 Paths: 2 available
  Local
    ::ffff:10.0.0.72 from 10.0.0.30 (10.0.0.30)
      Origin INCOMPLETE, metric -, localpref 100, weight 0, tag 0, valid, internal, ECMP head, ECMP, best, ECMP contributor
      Originator: 10.0.0.72, Cluster list: 10.0.0.30 
      Extended Community: Route-Target-AS:5001:5001 Color:CO(00):101
      Remote MPLS label: 62003
  Local
    ::ffff:10.0.0.72 from 10.0.0.175 (10.0.0.175)
      Origin INCOMPLETE, metric -, localpref 100, weight 0, tag 0, valid, internal, ECMP, ECMP contributor
      Originator: 10.0.0.72, Cluster list: 10.0.0.175 
      Extended Community: Route-Target-AS:5001:5001 Color:CO(00):101
      Remote MPLS label: 62003
BGP routing table entry for IPv6 prefix 2600:50:10:84::/64, Route Distinguisher: 84:5001
 Paths: 2 available
  Local
    ::ffff:10.0.0.84 from 10.0.0.30 (10.0.0.30)
      Origin INCOMPLETE, metric 0, localpref 100, weight 0, tag 0, valid, internal, ECMP head, ECMP, best, ECMP contributor
      Originator: 10.0.0.84, Cluster list: 10.0.0.30 
      Extended Community: Route-Target-AS:5001:5001
      Remote MPLS label: 720897
  Local
    ::ffff:10.0.0.84 from 10.0.0.175 (10.0.0.175)
      Origin INCOMPLETE, metric 0, localpref 100, weight 0, tag 0, valid, internal, ECMP, ECMP contributor
      Originator: 10.0.0.84, Cluster list: 10.0.0.175 
      Extended Community: Route-Target-AS:5001:5001
      Remote MPLS label: 720897
BGP routing table entry for IPv6 prefix 2600:50:10:120::/64, Route Distinguisher: 120:5001
 Paths: 2 available
  Local
    ::ffff:10.0.0.120 from 10.0.0.30 (10.0.0.30)
      Origin INCOMPLETE, metric 0, localpref 100, weight 0, tag 0, valid, internal, ECMP head, ECMP, best, ECMP contributor
      Originator: 10.0.0.120, Cluster list: 10.0.0.30 
      Extended Community: Route-Target-AS:5001:5001 Color:CO(00):101
      Remote MPLS label: 1276
  Local
    ::ffff:10.0.0.120 from 10.0.0.175 (10.0.0.175)
      Origin INCOMPLETE, metric 0, localpref 100, weight 0, tag 0, valid, internal, ECMP, ECMP contributor
      Originator: 10.0.0.120, Cluster list: 10.0.0.175 
      Extended Community: Route-Target-AS:5001:5001 Color:CO(00):101
      Remote MPLS label: 1276
BGP routing table entry for IPv6 prefix 2600:50:10:124::/64, Route Distinguisher: 124:5001
 Paths: 1 available
  Local
    ::ffff:10.0.0.124 from 10.0.0.175 (10.0.0.175)
      Origin INCOMPLETE, metric 0, localpref 100, weight 0, tag 0, valid, internal, best
      Originator: 10.0.0.124, Cluster list: 10.0.0.175 
      Extended Community: Route-Target-AS:5001:5001 Color:CO(00):101
      Remote MPLS label: 333
BGP routing table entry for IPv6 prefix 2600:50:10:128::/64, Route Distinguisher: 128:5001
 Paths: 1 available
  Local
    ::ffff:10.0.0.128 from 10.0.0.175 (10.0.0.175)
      Origin INCOMPLETE, metric 0, localpref 100, weight 0, tag 0, valid, internal, best
      Originator: 10.0.0.128, Cluster list: 10.0.0.175 
      Extended Community: Route-Target-AS:5001:5001 Color:CO(00):101
      Remote MPLS label: 48061
BGP routing table entry for IPv6 prefix 2600:50:10:179::/64, Route Distinguisher: 179:5001
 Paths: 2 available
  Local
    ::ffff:10.0.0.179 from 10.0.0.30 (10.0.0.30)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, ECMP head, ECMP, best, ECMP contributor
      Originator: 10.0.0.179, Cluster list: 10.0.0.30 
      Extended Community: Route-Target-AS:5001:5001 Color:CO(00):101
      Remote MPLS label: 16
  Local
    ::ffff:10.0.0.179 from 10.0.0.175 (10.0.0.175)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, ECMP, ECMP contributor
      Originator: 10.0.0.179, Cluster list: 10.0.0.175 
      Extended Community: Route-Target-AS:5001:5001 Color:CO(00):101
      Remote MPLS label: 16
BGP routing table entry for IPv6 prefix 2600:50:10:214::/64, Route Distinguisher: 214:5001
 Paths: 2 available
  Local
    ::ffff:10.0.0.214 from 10.0.0.30 (10.0.0.30)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, ECMP head, ECMP, best, ECMP contributor
      Originator: 10.0.0.214, Cluster list: 10.0.0.30 
      Extended Community: Route-Target-AS:5001:5001 Color:CO(00):101
      Remote MPLS label: 500000
  Local
    ::ffff:10.0.0.214 from 10.0.0.175 (10.0.0.175)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, ECMP, ECMP contributor
      Originator: 10.0.0.214, Cluster list: 10.0.0.175 
      Extended Community: Route-Target-AS:5001:5001 Color:CO(00):101
      Remote MPLS label: 500000
BGP routing table entry for IPv6 prefix 2600:50:10:217::/64, Route Distinguisher: 217:5001
 Paths: 2 available
  Local
    ::ffff:10.0.0.217 from 10.0.0.30 (10.0.0.30)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, ECMP head, ECMP, best, ECMP contributor
      Originator: 10.0.0.217, Cluster list: 10.0.0.30 
      Extended Community: Route-Target-AS:5001:5001 Color:CO(00):101
      Remote MPLS label: 524287
  Local
    ::ffff:10.0.0.217 from 10.0.0.175 (10.0.0.175)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, ECMP, ECMP contributor
      Originator: 10.0.0.217, Cluster list: 10.0.0.175 
      Extended Community: Route-Target-AS:5001:5001 Color:CO(00):101
      Remote MPLS label: 524287
BGP routing table entry for IPv6 prefix 2600:50:10:221::/64, Route Distinguisher: 210:5001
 Paths: 2 available
  Local
    ::ffff:10.0.0.221 from 10.0.0.30 (10.0.0.30)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, ECMP head, ECMP, best, ECMP contributor
      Originator: 10.0.0.221, Cluster list: 10.0.0.30 
      Extended Community: Route-Target-AS:5001:5001 Color:CO(00):101
      Remote MPLS label: 524305
  Local
    ::ffff:10.0.0.221 from 10.0.0.175 (10.0.0.175)
      Origin IGP, metric -, localpref 100, weight 0, tag 0, valid, internal, ECMP, ECMP contributor
      Originator: 10.0.0.221, Cluster list: 10.0.0.175 
      Extended Community: Route-Target-AS:5001:5001 Color:CO(00):101
      Remote MPLS label: 524305
BGP routing table entry for IPv6 prefix 2600:51:10:120::/64, Route Distinguisher: 120:5001
 Paths: 2 available
  Local
    ::ffff:10.0.0.120 from 10.0.0.30 (10.0.0.30)
      Origin INCOMPLETE, metric 0, localpref 100, weight 0, tag 0, valid, internal, ECMP head, ECMP, best, ECMP contributor
      Originator: 10.0.0.120, Cluster list: 10.0.0.30 
      Extended Community: Route-Target-AS:5001:5001 Color:CO(00):101
      Remote MPLS label: 1276
  Local
    ::ffff:10.0.0.120 from 10.0.0.175 (10.0.0.175)
      Origin INCOMPLETE, metric 0, localpref 100, weight 0, tag 0, valid, internal, ECMP, ECMP contributor
      Originator: 10.0.0.120, Cluster list: 10.0.0.175 
      Extended Community: Route-Target-AS:5001:5001 Color:CO(00):101
      Remote MPLS label: 1276
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
  Last read 00:00:03, last write 00:00:03
  Hold time is 180, keepalive interval is 60 seconds
  Configured hold time is 180, keepalive interval is 60 seconds
  Effective minimum hold time is 3 seconds
  Send failure hold time is 0 seconds
  Hold timer is active, time left: 00:02:57
  Keepalive timer is active, time left: 00:00:49
  Connect timer is inactive
  Idle-restart timer is inactive
  BGP state is Established, up for 04:29:37
  Number of transitions to established: 3
  Last state was OpenConfirm
  Last event was ReapplyOutboundPolicy
  Last sent notification:Hold Timer Expired Error/None, Last time 05:08:55, First time 06:10:48, Repeats 1
  Last sent socket-error:Connect (Network is unreachable), Last time 04:56:40, First time 06:10:46, Repeats 38
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
      Received 04:29:36
      Number of stale paths removed after graceful restart: 0
      Number of paths received before End-of-RIB: 9
    VPN-IPv6 End-of-RIB received: Yes
      Received 04:29:36
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
    Updates:                        44       653
    Keepalives:                   1666      1603
    Enhanced Route Refresh:          0         0
    Begin of Route Refresh:          0         0
    End of Route Refresh:            0         0
    Total messages:               1715      2259
  Prefix Statistics:
                                   Sent      Rcvd     Best Paths     Best ECMP Paths
    IPv4 Unicast:                     0         0              0                   0
    VPN-IPv4:                         1         9              9                   9
    IPv6 Unicast:                     0         0              0                   0
    VPN-IPv6:                         1         9              9                   9
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
  Total Number of TCP retransmissions: 2
  Options:
    Timestamps enabled: yes
    Selective Acknowledgments enabled: yes
    Window Scale enabled: yes
    Explicit Congestion Notification (ECN) enabled: no
  Socket Statistics:
    Window Scale (wscale): 7,7
    Retransmission Timeout (rto): 204.0ms
    Round-trip Time (rtt/rtvar): 1.0ms/1.2ms
    Delayed Ack Timeout (ato): 40.0ms
    Congestion Window (cwnd): 2
    Slow-start Threshold (ssthresh): 7
    TCP Throughput: 22.49 Mbps
    Advertised Recv Window (rcv_space): 14600

BGP neighbor is 10.0.0.175, remote AS 64512, internal link
 Description: Juniper_175
  BGP version 4, remote router ID 10.0.0.175, VRF default
  Inherits configuration from and member of peer-group IBGP_CLIENT_PEER
  Last read 00:00:19, last write 00:00:21
  Hold time is 90, keepalive interval is 30 seconds
  Configured hold time is 180, keepalive interval is 60 seconds
  Effective minimum hold time is 3 seconds
  Send failure hold time is 0 seconds
  Hold timer is active, time left: 00:01:11
  Keepalive timer is active, time left: 00:00:00
  Connect timer is inactive
  Idle-restart timer is inactive
  BGP state is Established, up for 04:29:22
  Number of transitions to established: 11
  Last state was OpenConfirm
  Last event was ReapplyOutboundPolicy
  Last sent notification:Hold Timer Expired Error/None, Last time 04:40:14, First time 18:01:20, Repeats 9
  Last sent socket-error:Connect (Network is unreachable), Last time 04:57:52, First time 18:01:19, Repeats 25
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
      Received 04:29:21
      Number of stale paths removed after graceful restart: 0
      Number of paths received before End-of-RIB: 9
    VPN-IPv6 End-of-RIB received: Yes
      Received 04:29:21
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
    Updates:               66       545
    Keepalives:          3295      2935
    Route Refresh:          0         0
    Total messages:      3382      3491
  Prefix Statistics:
                                   Sent      Rcvd     Best Paths     Best ECMP Paths
    IPv4 Unicast:                     0         0              0                   0
    VPN-IPv4:                         1        11             11                   0
    IPv6 Unicast:                     0         0              0                   0
    VPN-IPv6:                         1        11             11                   0
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
    TCP Throughput: 247.52 Mbps
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
10.0.0.124/32   IS-IS SR IPv4   14          65                  115            
10.0.0.128/32   IS-IS SR IPv4   11          65                  115            
10.0.0.175/32   IS-IS SR IPv4   1           65                  115            
10.0.0.179/32   IS-IS SR IPv4   7           65                  115            
10.0.0.214/32   IS-IS SR IPv4   10          65                  115            
10.0.0.217/32   IS-IS SR IPv4   16          65                  115            
10.0.0.221/32   IS-IS SR IPv4   13          65                  115            

   IGP Metric    Metric Type
---------------- -----------
   10            metric     
   11            metric     
   21            metric     
   21            metric     
   11            metric     
   11            metric     
   11            metric     
   10            metric     
   11            metric     
   11            metric     
   11            metric     
   11            metric     

```

## show tunnel rib colored brief

```text
Tunnel RIB: system-colored-tunnel-rib
 Endpoint         Color    Tunnel Type     Index(es)    Tunnel Preference    IGP Preference    IGP Metric   Metric Type
---------------- -------- --------------- ------------ -------------------- ----------------- ------------- -----------
 10.0.0.53/32     100      SR-TE Policy    170          35                   3                 0            metric     
 10.0.0.53/32     101      SR-TE Policy    218          35                   3                 0            metric     
 10.0.0.66/32     100      SR-TE Policy    164          35                   3                 0            metric     
 10.0.0.66/32     101      SR-TE Policy    212          35                   3                 0            metric     
 10.0.0.72/32     100      SR-TE Policy    156          35                   3                 0            metric     
 10.0.0.72/32     101      SR-TE Policy    200          35                   3                 0            metric     
 10.0.0.84/32     100      SR-TE Policy    154          35                   3                 0            metric     
 10.0.0.84/32     101      SR-TE Policy    216          35                   3                 0            metric     
 10.0.0.120/32    100      SR-TE Policy    158          35                   3                 0            metric     
 10.0.0.120/32    101      SR-TE Policy    204          35                   3                 0            metric     
 10.0.0.124/32    100      SR-TE Policy    172          35                   3                 0            metric     
 10.0.0.124/32    101      SR-TE Policy    198          35                   3                 0            metric     
 10.0.0.128/32    100      SR-TE Policy    166          35                   3                 0            metric     
 10.0.0.128/32    101      SR-TE Policy    214          35                   3                 0            metric     
 10.0.0.179/32    100      SR-TE Policy    162          35                   3                 0            metric     
 10.0.0.179/32    101      SR-TE Policy    202          35                   3                 0            metric     
 10.0.0.214/32    100      SR-TE Policy    174          35                   3                 0            metric     
 10.0.0.214/32    101      SR-TE Policy    210          35                   3                 0            metric     
 10.0.0.217/32    100      SR-TE Policy    160          35                   3                 0            metric     
 10.0.0.217/32    101      SR-TE Policy    206          35                   3                 0            metric     
 10.0.0.221/32    100      SR-TE Policy    168          35                   3                 0            metric     
 10.0.0.221/32    101      SR-TE Policy    208          35                   3                 0            metric     

```

## show tunnel rib colored system-colored-tunnel-rib brief

```text
Tunnel RIB: system-colored-tunnel-rib
 Endpoint         Color    Tunnel Type     Index(es)    Tunnel Preference    IGP Preference    IGP Metric   Metric Type
---------------- -------- --------------- ------------ -------------------- ----------------- ------------- -----------
 10.0.0.53/32     100      SR-TE Policy    170          35                   3                 0            metric     
 10.0.0.53/32     101      SR-TE Policy    218          35                   3                 0            metric     
 10.0.0.66/32     100      SR-TE Policy    164          35                   3                 0            metric     
 10.0.0.66/32     101      SR-TE Policy    212          35                   3                 0            metric     
 10.0.0.72/32     100      SR-TE Policy    156          35                   3                 0            metric     
 10.0.0.72/32     101      SR-TE Policy    200          35                   3                 0            metric     
 10.0.0.84/32     100      SR-TE Policy    154          35                   3                 0            metric     
 10.0.0.84/32     101      SR-TE Policy    216          35                   3                 0            metric     
 10.0.0.120/32    100      SR-TE Policy    158          35                   3                 0            metric     
 10.0.0.120/32    101      SR-TE Policy    204          35                   3                 0            metric     
 10.0.0.124/32    100      SR-TE Policy    172          35                   3                 0            metric     
 10.0.0.124/32    101      SR-TE Policy    198          35                   3                 0            metric     
 10.0.0.128/32    100      SR-TE Policy    166          35                   3                 0            metric     
 10.0.0.128/32    101      SR-TE Policy    214          35                   3                 0            metric     
 10.0.0.179/32    100      SR-TE Policy    162          35                   3                 0            metric     
 10.0.0.179/32    101      SR-TE Policy    202          35                   3                 0            metric     
 10.0.0.214/32    100      SR-TE Policy    174          35                   3                 0            metric     
 10.0.0.214/32    101      SR-TE Policy    210          35                   3                 0            metric     
 10.0.0.217/32    100      SR-TE Policy    160          35                   3                 0            metric     
 10.0.0.217/32    101      SR-TE Policy    206          35                   3                 0            metric     
 10.0.0.221/32    100      SR-TE Policy    168          35                   3                 0            metric     
 10.0.0.221/32    101      SR-TE Policy    208          35                   3                 0            metric     

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
>C    10.0.0.32/32 [0 pref/0 metric] updated 1d01h ago
         via Loopback0, directly connected
>C    20.30.32.0/24 [0 pref/0 metric] updated 04:56:51 ago
         via Ethernet1, directly connected
>C    20.32.175.0/24 [0 pref/0 metric] updated 06:34:51 ago
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
>P    0.0.0.0/8 [1 pref/0 metric] updated 1d07h ago
         via Null0, directly connected [NF]
>P    127.0.0.0/8 [1 pref/0 metric] updated 1d07h ago
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
>I    10.0.0.30/32 [115 pref/10 metric] updated 01:32:32 ago
         via 20.30.32.30, Ethernet1
>I    10.0.0.53/32 [115 pref/11 metric] updated 00:04:03 ago
         via 20.32.175.175, Ethernet5
>I    10.0.0.72/32 [115 pref/21 metric] updated 00:26:46 ago
         via 20.32.175.175, Ethernet5
>I    10.0.0.84/32 [115 pref/21 metric] updated 00:26:46 ago
         via 20.32.175.175, Ethernet5
>I    10.0.0.120/32 [115 pref/11 metric] updated 00:21:55 ago
         via 20.32.175.175, Ethernet5
>I    10.0.0.124/32 [115 pref/11 metric] updated 00:26:46 ago
         via 20.32.175.175, Ethernet5
>I    10.0.0.128/32 [115 pref/11 metric] updated 00:26:46 ago
         via 20.32.175.175, Ethernet5
>I    10.0.0.175/32 [115 pref/10 metric] updated 01:32:25 ago
         via 20.32.175.175, Ethernet5
>I    10.0.0.179/32 [115 pref/11 metric] updated 00:26:46 ago
         via 20.32.175.175, Ethernet5
>I    10.0.0.214/32 [115 pref/11 metric] updated 00:26:46 ago
         via 20.32.175.175, Ethernet5
>I    10.0.0.216/32 [115 pref/21 metric] updated 00:26:46 ago
         via 20.32.175.175, Ethernet5
>I    10.0.0.217/32 [115 pref/11 metric] updated 00:26:46 ago
         via 20.32.175.175, Ethernet5
>I    10.0.0.221/32 [115 pref/11 metric] updated 00:26:46 ago
         via 20.32.175.175, Ethernet5
>I    20.30.53.0/24 [115 pref/20 metric] updated 01:32:32 ago
         via 20.30.32.30, Ethernet1
>I    20.30.66.0/24 [115 pref/20 metric] updated 01:32:32 ago
         via 20.30.32.30, Ethernet1
>I    20.30.72.0/24 [115 pref/20 metric] updated 01:32:32 ago
         via 20.30.32.30, Ethernet1
>I    20.30.84.0/24 [115 pref/20 metric] updated 01:32:32 ago
         via 20.30.32.30, Ethernet1
>I    20.30.120.0/24 [115 pref/20 metric] updated 01:32:32 ago
         via 20.30.32.30, Ethernet1
>I    20.30.124.0/24 [115 pref/20 metric] updated 01:32:32 ago
         via 20.30.32.30, Ethernet1
>I    20.30.128.0/24 [115 pref/20 metric] updated 01:32:32 ago
         via 20.30.32.30, Ethernet1
>I    20.30.179.0/24 [115 pref/20 metric] updated 01:25:19 ago
         via 20.30.32.30, Ethernet1
>I    20.30.184.0/24 [115 pref/20 metric] updated 01:32:32 ago
         via 20.30.32.30, Ethernet1
>I    20.30.214.0/24 [115 pref/20 metric] updated 01:32:32 ago
         via 20.30.32.30, Ethernet1
>I    20.30.217.0/24 [115 pref/20 metric] updated 01:32:32 ago
         via 20.30.32.30, Ethernet1
>I    20.30.221.0/24 [115 pref/20 metric] updated 01:32:32 ago
         via 20.30.32.30, Ethernet1
>I    20.53.175.0/24 [115 pref/11 metric] updated 00:04:14 ago
         via 20.32.175.175, Ethernet5
>I    20.66.175.0/24 [115 pref/11 metric] updated 00:26:46 ago
         via 20.32.175.175, Ethernet5
>I    20.72.175.0/24 [115 pref/11 metric] updated 00:26:46 ago
         via 20.32.175.175, Ethernet5
>I    20.84.175.0/24 [115 pref/11 metric] updated 00:26:46 ago
         via 20.32.175.175, Ethernet5
>I    20.120.175.0/24 [115 pref/11 metric] updated 00:26:46 ago
         via 20.32.175.175, Ethernet5
>I    20.120.214.0/24 [115 pref/21 metric] updated 00:21:55 ago
         via 20.32.175.175, Ethernet5
>I    20.124.175.0/24 [115 pref/11 metric] updated 00:26:46 ago
         via 20.32.175.175, Ethernet5
>I    20.128.175.0/24 [115 pref/11 metric] updated 00:26:46 ago
         via 20.32.175.175, Ethernet5
>I    20.131.175.0/24 [115 pref/11 metric] updated 00:26:46 ago
         via 20.32.175.175, Ethernet5
>I    20.175.179.0/24 [115 pref/11 metric] updated 00:26:46 ago
         via 20.32.175.175, Ethernet5
>I    20.175.184.0/24 [115 pref/11 metric] updated 00:26:46 ago
         via 20.32.175.175, Ethernet5
>I    20.175.214.0/24 [115 pref/11 metric] updated 00:26:46 ago
         via 20.32.175.175, Ethernet5
>I    20.175.217.0/24 [115 pref/11 metric] updated 00:26:46 ago
         via 20.32.175.175, Ethernet5
>I    20.175.221.0/24 [115 pref/11 metric] updated 00:26:46 ago
         via 20.32.175.175, Ethernet5
>I    20.214.216.0/24 [115 pref/21 metric] updated 00:26:46 ago
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
>C    2001:0:30:32::/64 [0 pref/0 metric] updated 04:56:51 ago
         via Ethernet1, directly connected
>C    2001:0:32:175::/64 [0 pref/0 metric] updated 04:02:29 ago
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
>P    ::/96 [1 pref/0 metric] updated 04:56:51 ago
         via Null0, directly connected [NF]
>P    ::ffff:127.0.0.0/104 [1 pref/0 metric] updated 04:56:51 ago
         via :: [1 pref/1 metric] type ipv6
            via , directly connected
>P    fe80::/10 [1 pref/0 metric] updated 04:56:51 ago
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
>I    2001:0:30:66::/64 [115 pref/20 metric] updated 01:32:32 ago
         via fe80::c6ca:2bff:fe45:a215, Ethernet1
>I    2001:0:30:72::/64 [115 pref/20 metric] updated 01:32:32 ago
         via fe80::c6ca:2bff:fe45:a215, Ethernet1
>I    2001:0:30:84::/64 [115 pref/20 metric] updated 01:32:32 ago
         via fe80::c6ca:2bff:fe45:a215, Ethernet1
>I    2001:0:30:120::/64 [115 pref/20 metric] updated 01:32:32 ago
         via fe80::c6ca:2bff:fe45:a215, Ethernet1
>I    2001:0:30:124::/64 [115 pref/20 metric] updated 01:32:32 ago
         via fe80::c6ca:2bff:fe45:a215, Ethernet1
>I    2001:0:30:128::/64 [115 pref/20 metric] updated 01:32:32 ago
         via fe80::c6ca:2bff:fe45:a215, Ethernet1
>I    2001:0:30:179::/64 [115 pref/20 metric] updated 01:25:19 ago
         via fe80::c6ca:2bff:fe45:a215, Ethernet1
>I    2001:0:30:184::/64 [115 pref/20 metric] updated 01:32:32 ago
         via fe80::c6ca:2bff:fe45:a215, Ethernet1
>I    2001:0:30:214::/64 [115 pref/20 metric] updated 01:32:32 ago
         via fe80::c6ca:2bff:fe45:a215, Ethernet1
>I    2001:0:30:217::/64 [115 pref/20 metric] updated 01:32:32 ago
         via fe80::c6ca:2bff:fe45:a215, Ethernet1
>I    2001:0:30:221::/64 [115 pref/20 metric] updated 01:32:32 ago
         via fe80::c6ca:2bff:fe45:a215, Ethernet1
>I    2001:0:53:120::/64 [115 pref/20 metric] updated 01:32:32 ago
         via fe80::c6ca:2bff:fe45:a215, Ethernet1
>I    2001:0:84:175::/64 [115 pref/30 metric] updated 01:32:32 ago
         via fe80::c6ca:2bff:fe45:a215, Ethernet1
>I    2001:0:120:175::/64 [115 pref/30 metric] updated 00:21:55 ago
         via fe80::c6ca:2bff:fe45:a215, Ethernet1
>I    2001:0:120:214::/64 [115 pref/30 metric] updated 00:21:55 ago
         via fe80::c6ca:2bff:fe45:a215, Ethernet1
```

## show platform sand l3 summary

```text
Number of vrfs: 3

Ipv4:
  Routes:       80   backlog:  0  unprogrammed:  0
  Adjacencies:  110  backlog:  0  unprogrammed:  0
Ipv6:
  Routes:       41   backlog:  0  unprogrammed:  0
  Adjacencies:  110  backlog:  0  unprogrammed:  0
Mpls:
  Routes:       37  backlog:  0  unprogrammed:  0
  Adjacencies:  3   backlog:  0  unprogrammed:  0

Jericho2 Ip Fecs:
  Non-ecmp fecs:  4179  ecmp fecs:  0  fec entries:  4179
Jericho2 Mpls Fecs:
  Non-ecmp fecs:  3  ecmp fecs:  0  fec entries:  3
Jericho2 Vxlan Tunnel Fecs:
  Non-ecmp fecs:  0  ecmp fecs:  0  fec entries:  0
  Number of vxlan tunnels configured: 0

Jericho2 Lpm Routes:
  Routes:   80  unprogrammed:   0   
  Routes6:  41  unprogrammed6:  0   
  Backlog:  0 

Jericho2 Lpm:
  TCAM entries used:   4   Percent free:  99  ADS2 entries used:   5  Percent free:  99
  Pivot buckets used:  6   Rows used:     2   Entries Per Bucket:  0  Percent free:  99
  Route buckets used:  25  Rows used:     3   Entries Per Bucket:  4  Percent free:  99

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
  FixedSystem: 27
Egress Sflow rewrite entries in use (in each fap):
  FixedSystem: 0

Egress rewrite chains in backlog: resource-full 0, no-interface 0

Glem entries used per fap :
  FixedSystem: 4146

Jericho2 Fec:
  Maximum FEC hierarchy levels:  2
  ReusedEcmp:  0  allocs:  1230  frees:  1147  shuffles:  0  cmds:  0
  Zombies:     0    purges:    0
  Quarantine:  0/0  shuffles:  0  deletes:  0   
  Preserved FECs: 0
    First FEC preserved: never
    Last FEC preserved: never
  Fec insertion failures:  0
  Level1  Fecs:
    Non-ecmp fecs:            42  ecmp fecs:            1 
    Non-ecmp (Percent free):  99  ecmp (Percent free):  99
  Level2  Fecs:
    Non-ecmp fecs:            41  ecmp fecs:            0  
    Non-ecmp (Percent free):  99  ecmp (Percent free):  100
  Level3  Fecs:
    Non-ecmp fecs:            0    ecmp fecs:            0  
    Non-ecmp (Percent free):  100  ecmp (Percent free):  100

Lpm Detail:
  Requests:  2839  cleanses:  692  batches:  692  avg batch size:  4

Jericho Arp:
  ArpTable writes:      33702  queued      0   
  IngressTable writes:  83436  queued      0   
  Coprocessors:         1      in CmdRing

Tunnel Counter Status
  Number of MPLS tunnels:                  46   
  Number of uncountable MPLS tunnels:      20   
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
|0  |10.0.0.53/32      |ROUTE| Et5                |1010 |107518  | 3c:08:cd:8d:ba:dc |  -  |288374|   -   
|0  |10.0.0.72/32      |ROUTE| Et5                |1010 |107518  | 3c:08:cd:8d:ba:dc |  -  |288374|   -   
|0  |10.0.0.84/32      |ROUTE| Et5                |1010 |107518  | 3c:08:cd:8d:ba:dc |  -  |288374|   -   
|0  |10.0.0.120/32     |ROUTE| Et5                |1010 |107518  | 3c:08:cd:8d:ba:dc |  -  |288374|   -   
|0  |10.0.0.124/32     |ROUTE| Et5                |1010 |107518  | 3c:08:cd:8d:ba:dc |  -  |288374|   -   
|0  |10.0.0.128/32     |ROUTE| Et5                |1010 |107518  | 3c:08:cd:8d:ba:dc |  -  |288374|   -   
|0  |10.0.0.175/32     |ROUTE| Et5                |1010 |107518  | 3c:08:cd:8d:ba:dc |  -  |288374|   -   
|0  |10.0.0.179/32     |ROUTE| Et5                |1010 |107518  | 3c:08:cd:8d:ba:dc |  -  |288374|   -   
|0  |10.0.0.214/32     |ROUTE| Et5                |1010 |107518  | 3c:08:cd:8d:ba:dc |  -  |288374|   -   
|0  |10.0.0.216/32     |ROUTE| Et5                |1010 |107518  | 3c:08:cd:8d:ba:dc |  -  |288374|   -   
|0  |10.0.0.217/32     |ROUTE| Et5                |1010 |107518  | 3c:08:cd:8d:ba:dc |  -  |288374|   -   
|0  |10.0.0.221/32     |ROUTE| Et5                |1010 |107518  | 3c:08:cd:8d:ba:dc |  -  |288374|   -   
|0  |20.30.32.0/32     |TRAP | CoppSystemIpBcast  |0    |  -     | BcastReceive      |  -  |524290|   -   
|0  |20.30.32.30/32    |ROUTE| Et1                |1006 |107517  | c4:ca:2b:45:a2:15 |  -  |288368|   -   
|0  |20.30.32.32/32    |TRAP | CoppSystemIpUcast  |0    |  -     | Receive           |  -  |524291|   -   
|0  |20.30.32.255/32   |TRAP | CoppSystemIpBcast  |0    |  -     | BcastReceive      |  -  |524290|   -   
|0  |20.30.32.0/24     |TRAP | CoppSystemL3DstMiss|1006 |1006    | ArpTrap           |  -  |525301|   -   
|0  |20.30.53.0/24     |ROUTE| Et1                |1006 |107517  | c4:ca:2b:45:a2:15 |  -  |288369|   -   
|0  |20.30.66.0/24     |ROUTE| Et1                |1006 |107517  | c4:ca:2b:45:a2:15 |  -  |288369|   -   
|0  |20.30.72.0/24     |ROUTE| Et1                |1006 |107517  | c4:ca:2b:45:a2:15 |  -  |288369|   -   
|0  |20.30.84.0/24     |ROUTE| Et1                |1006 |107517  | c4:ca:2b:45:a2:15 |  -  |288369|   -   
|0  |20.30.120.0/24    |ROUTE| Et1                |1006 |107517  | c4:ca:2b:45:a2:15 |  -  |288369|   -   
|0  |20.30.124.0/24    |ROUTE| Et1                |1006 |107517  | c4:ca:2b:45:a2:15 |  -  |288369|   -   
|0  |20.30.128.0/24    |ROUTE| Et1                |1006 |107517  | c4:ca:2b:45:a2:15 |  -  |288369|   -   
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
|0  |20.53.175.0/24    |ROUTE| Et5                |1010 |107518  | 3c:08:cd:8d:ba:dc |  -  |288374|   -   
|0  |20.66.175.0/24    |ROUTE| Et5                |1010 |107518  | 3c:08:cd:8d:ba:dc |  -  |288374|   -   
|0  |20.72.175.0/24    |ROUTE| Et5                |1010 |107518  | 3c:08:cd:8d:ba:dc |  -  |288374|   -   
|0  |20.84.175.0/24    |ROUTE| Et5                |1010 |107518  | 3c:08:cd:8d:ba:dc |  -  |288374|   -   
|0  |20.120.175.0/24   |ROUTE| Et5                |1010 |107518  | 3c:08:cd:8d:ba:dc |  -  |288374|   -   
|0  |20.120.214.0/24   |ROUTE| Et5                |1010 |107518  | 3c:08:cd:8d:ba:dc |  -  |288374|   -   
|0  |20.124.175.0/24   |ROUTE| Et5                |1010 |107518  | 3c:08:cd:8d:ba:dc |  -  |288374|   -   
|0  |20.128.175.0/24   |ROUTE| Et5                |1010 |107518  | 3c:08:cd:8d:ba:dc |  -  |288374|   -   
|0  |20.131.175.0/24   |ROUTE| Et5                |1010 |107518  | 3c:08:cd:8d:ba:dc |  -  |288374|   -   
|0  |20.175.179.0/24   |ROUTE| Et5                |1010 |107518  | 3c:08:cd:8d:ba:dc |  -  |288374|   -   
|0  |20.175.184.0/24   |ROUTE| Et5                |1010 |107518  | 3c:08:cd:8d:ba:dc |  -  |288374|   -   
|0  |20.175.214.0/24   |ROUTE| Et5                |1010 |107518  | 3c:08:cd:8d:ba:dc |  -  |288374|   -   
|0  |20.175.217.0/24   |ROUTE| Et5                |1010 |107518  | 3c:08:cd:8d:ba:dc |  -  |288374|   -   
|0  |20.175.221.0/24   |ROUTE| Et5                |1010 |107518  | 3c:08:cd:8d:ba:dc |  -  |288374|   -   
|0  |20.214.216.0/24   |ROUTE| Et5                |1010 |107518  | 3c:08:cd:8d:ba:dc |  -  |288374|   -   
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
|2  |50.10.32.2/32     |ROUTE| Et40               |1008 |107520  | 00:28:01:00:00:01 |  -  |288383|   -   
|2  |50.10.32.255/32   |TRAP | CoppSystemIpBcast  |0    |  -     | BcastReceive      |  -  |524290|   -   
|2  |50.10.32.0/24     |TRAP | CoppSystemL3DstMiss|1008 |1008    | ArpTrap           |  -  |525303|   -   
|2  |50.10.53.0/24     |ROUTE| FEC 288378         |0    |2097147 | 00:00:00:00:00:00 |  -  |157300|M 970000
|2  |50.10.72.0/24     |ROUTE| FEC 288386         |0    |2097148 | 00:00:00:00:00:00 |  -  |157310|M 62002
|2  |50.10.84.0/24     |ROUTE| FEC 288371         |0    |2097142 | 00:00:00:00:00:00 |  -  |157319|M 720896
|2  |50.10.120.0/24    |ROUTE| FEC 288387         |0    |2097146 | 00:00:00:00:00:00 |  -  |157302|M 1277
|2  |50.10.124.0/24    |ROUTE| FEC 288388         |0    |2097109 | 00:00:00:00:00:00 |  -  |157301|M 332
|2  |50.10.128.0/24    |ROUTE| FEC 288389         |0    |2097108 | 00:00:00:00:00:00 |  -  |157303|M 48060
|2  |50.10.179.0/24    |ROUTE| FEC 288379         |0    |2097151 | 00:00:00:00:00:00 |  -  |157313|M 16
|2  |50.10.214.0/24    |ROUTE| FEC 288380         |0    |2097112 | 00:00:00:00:00:00 |  -  |157305|M 500000
|2  |50.10.217.0/24    |ROUTE| FEC 288381         |0    |2097111 | 00:00:00:00:00:00 |  -  |157306|M 524287
|2  |50.10.221.0/24    |ROUTE| FEC 288382         |0    |2097110 | 00:00:00:00:00:00 |  -  |157304|M 524305
|2  |51.10.120.0/24    |ROUTE| FEC 288387         |0    |2097146 | 00:00:00:00:00:00 |  -  |157302|M 1277
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
|  -  |157288|ROUTE| FEC 288394         |   - |2097144 |                 - |Mpush 970001
|  -  |157289|ROUTE| FEC 288378         |   - |  -     |                   |   -   
|  -  |157290|ROUTE| FEC 288384         |   - |  -     |                   |   -   
|  -  |157291|ROUTE| FEC 288386         |   - |  -     |                   |   -   
|  -  |157292|ROUTE| FEC 288385         |   - |  -     |                   |   -   
|  -  |157293|ROUTE| FEC 288387         |   - |  -     |                   |   -   
|  -  |157294|ROUTE| FEC 288388         |   - |  -     |                   |   -   
|  -  |157295|ROUTE| FEC 288389         |   - |  -     |                   |   -   
|  -  |157296|ROUTE| FEC 288379         |   - |  -     |                   |   -   
|  -  |157297|ROUTE| FEC 288380         |   - |  -     |                   |   -   
|  -  |157298|ROUTE| FEC 288381         |   - |  -     |                   |   -   
|  -  |157299|ROUTE| FEC 288382         |   - |  -     |                   |   -   
|  -  |157300|ROUTE| FEC 288378         |   - |2097147 |                 - |Mpush 970000
|  -  |157301|ROUTE| FEC 288388         |   - |2097109 |                 - |Mpush 332
|  -  |157302|ROUTE| FEC 288387         |   - |2097146 |                 - |Mpush 1277
|  -  |157303|ROUTE| FEC 288389         |   - |2097108 |                 - |Mpush 48060
|  -  |157304|ROUTE| FEC 288382         |   - |2097110 |                 - |Mpush 524305
|  -  |157305|ROUTE| FEC 288380         |   - |2097112 |                 - |Mpush 500000
|  -  |157306|ROUTE| FEC 288381         |   - |2097111 |                 - |Mpush 524287
|  -  |157308|ROUTE| FEC 288401         |   - |2097150 |                 - |Mpush 16
|  -  |157309|ROUTE| FEC 288396         |   - |2097149 |                 - |Mpush 62003
|  -  |157310|ROUTE| FEC 288386         |   - |2097148 |                 - |Mpush 62002
|  -  |157313|ROUTE| FEC 288379         |   - |2097151 |                 - |Mpush 16
|  -  |157318|ROUTE| FEC 288371         |   - |2097143 |                 - |Mpush 720897
|  -  |157319|ROUTE| FEC 288371         |   - |2097142 |                 - |Mpush 720896
|  -  |157320|ROUTE| FEC 288400         |   - |2097101 |                 - |Mpush 48061
|  -  |157321|ROUTE| FEC 288402         |   - |2097100 |                 - |Mpush 500000
|  -  |157322|ROUTE| FEC 288399         |   - |2097102 |                 - |Mpush 333
|  -  |157323|ROUTE| FEC 288403         |   - |2097099 |                 - |Mpush 524287
|  -  |157324|ROUTE| FEC 288404         |   - |2097098 |                 - |Mpush 524305
|  -  |157325|ROUTE| FEC 288398         |   - |2097145 |                 - |Mpush 1276
|  -  |157326|ROUTE| FEC 288394         |   - |  -     |                   |   -   
|  -  |157327|ROUTE| FEC 288398         |   - |  -     |                   |   -   
|  -  |157328|ROUTE| FEC 288399         |   - |  -     |                   |   -   
|  -  |157329|ROUTE| FEC 288400         |   - |  -     |                   |   -   
|  -  |157330|ROUTE| FEC 288402         |   - |  -     |                   |   -   
|  -  |157331|ROUTE| FEC 288403         |   - |  -     |                   |   -   
|  -  |157332|ROUTE| FEC 288404         |   - |  -     |                   |   -   
|  -  |157333|ROUTE| FEC 288395         |   - |  -     |                   |   -   
|  -  |157334|ROUTE| FEC 288396         |   - |  -     |                   |   -   
|  -  |157335|ROUTE| FEC 288397         |   - |  -     |                   |   -   
|  -  |157336|ROUTE| FEC 288401         |   - |  -     |                   |   -   
|  -  |288360|DROP | DROP               |0    |  -     |                   |   -   
|  -  |288361|DROP | DROP               |0    |  -     |                   |   -   
|  -  |288362|ROUTE| Et1                |1006 |107517  | c4:ca:2b:45:a2:15 |   -   
|  -  |288363|ROUTE| Et1                |1006 |107517  | c4:ca:2b:45:a2:15 |   -   
|  -  |288364|DROP | DROP               |0    |  -     |                   |   -   
|  -  |288365|ROUTE| Et1                |1006 |107517  | c4:ca:2b:45:a2:15 |   -   
|  -  |288366|DROP | DROP               |0    |  -     |                   |   -   
|  -  |288367|ROUTE| Et5                |1010 |107518  | 3c:08:cd:8d:ba:dc |   -   
|  -  |288368|ROUTE| Et1                |1006 |107517  | c4:ca:2b:45:a2:15 |   -   
|  -  |288369|ROUTE| Et1                |1006 |107517  | c4:ca:2b:45:a2:15 |   -   
|  -  |288370|ROUTE| Et40               |1009 |107532  | 00:29:01:00:00:01 |   -   
|  -  |288371|ROUTE| Et5                |1010 |107530  | 3c:08:cd:8d:ba:dc |Mpush 20084
|  -  |288374|ROUTE| Et5                |1010 |107518  | 3c:08:cd:8d:ba:dc |   -   
|  -  |288375|ROUTE| Et5                |1010 |107518  | 3c:08:cd:8d:ba:dc |   -   
|  -  |288376|DROP | DROP               |0    |  -     |                   |   -   
|  -  |288377|ROUTE| Et1                |1006 |107519  | c4:ca:2b:45:a2:15 |   -   
|  -  |288378|ROUTE| Et1                |1006 |107528  | c4:ca:2b:45:a2:15 |Mpush 20053
|  -  |288379|ROUTE| Et1                |1006 |107524  | c4:ca:2b:45:a2:15 |Mpush 20179
|  -  |288380|ROUTE| Et1                |1006 |107534  | c4:ca:2b:45:a2:15 |Mpush 20214
|  -  |288381|ROUTE| Et1                |1006 |107535  | c4:ca:2b:45:a2:15 |Mpush 20217
|  -  |288382|ROUTE| Et1                |1006 |107536  | c4:ca:2b:45:a2:15 |Mpush 21221
|  -  |288383|ROUTE| Et40               |1008 |107520  | 00:28:01:00:00:01 |   -   
|  -  |288384|ROUTE| Et1                |1006 |107526  | c4:ca:2b:45:a2:15 |Mpush 20066
|  -  |288385|ROUTE| Et1                |1006 |107527  | c4:ca:2b:45:a2:15 |Mpush 20084
|  -  |288386|ROUTE| Et1                |1006 |107523  | c4:ca:2b:45:a2:15 |Mpush 20072
|  -  |288387|ROUTE| Et1                |1006 |107533  | c4:ca:2b:45:a2:15 |Mpush 20120
|  -  |288388|ROUTE| Et1                |1006 |107537  | c4:ca:2b:45:a2:15 |Mpush 20124
|  -  |288389|ROUTE| Et1                |1006 |107538  | c4:ca:2b:45:a2:15 |Mpush 20128
|  -  |288392|ROUTE| Et5                |1010 |107521  | 3c:08:cd:8d:ba:dc |   -   
|  -  |288393|ROUTE| Et5                |1010 |107540  | 3c:08:cd:8d:ba:dc |   -   
|  -  |288394|ROUTE| Et5                |1010 |107553  | 3c:08:cd:8d:ba:dc |Mpush 20053
|  -  |288395|ROUTE| Et5                |1010 |107542  | 3c:08:cd:8d:ba:dc |Mpush 20066
|  -  |288396|ROUTE| Et5                |1010 |107522  | 3c:08:cd:8d:ba:dc |Mpush 20072
|  -  |288397|ROUTE| Et5                |1010 |107544  | 3c:08:cd:8d:ba:dc |Mpush 20084
|  -  |288398|ROUTE| Et5                |1010 |107552  | 3c:08:cd:8d:ba:dc |Mpush 20120
|  -  |288399|ROUTE| Et5                |1010 |107554  | 3c:08:cd:8d:ba:dc |Mpush 20124
|  -  |288400|ROUTE| Et5                |1010 |107555  | 3c:08:cd:8d:ba:dc |Mpush 20128
|  -  |288401|ROUTE| Et5                |1010 |107525  | 3c:08:cd:8d:ba:dc |Mpush 20179
|  -  |288402|ROUTE| Et5                |1010 |107556  | 3c:08:cd:8d:ba:dc |Mpush 20214
|  -  |288403|ROUTE| Et5                |1010 |107557  | 3c:08:cd:8d:ba:dc |Mpush 20217
|  -  |288404|ROUTE| Et5                |1010 |107558  | 3c:08:cd:8d:ba:dc |Mpush 21221
|  -  |524290|TRAP | CoppSystemIpBcast  |0    |  -     | BcastReceive      |   -   
|  -  |524291|TRAP | CoppSystemIpUcast  |0    |  -     | Receive           |   -   
|  -  |524293|TRAP | CoppSystemL3LpmOver|0    |  -     | SlowReceive       |   -   
|  -  |524295|TRAP | CoppSystemL3DstMiss|0    |  -     | ArpTrap           |   -   
|  -  |525301|TRAP | CoppSystemL3DstMiss|1006 |1006    | ArpTrap           |   -   
|  -  |525303|TRAP | CoppSystemL3DstMiss|1008 |1008    | ArpTrap           |   -   
|  -  |525304|TRAP | CoppSystemL3DstMiss|1009 |1009    | ArpTrap           |   -   
|  -  |525305|TRAP | CoppSystemL3DstMiss|1010 |1010    | ArpTrap           |   -   

```

