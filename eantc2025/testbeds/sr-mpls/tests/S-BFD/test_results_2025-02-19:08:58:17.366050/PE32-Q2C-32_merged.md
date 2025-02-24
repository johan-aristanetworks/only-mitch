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

Uptime: 2 days, 2 hours and 5 minutes
Total memory: 65734472 kB
Free memory: 61802944 kB

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
Et1       Arista_Spine30_Eth2  0:01      0.1   0.0%        0      0.1   0.0%
Et5       Juniper-175_509      0:01      0.0   0.0%        0      0.1   0.0%

Port      Out Kpps
```

## show isis neighbors

```text
 
Instance  VRF      System Id        Type Interface          SNPA              State Hold time   Circuit Id          
IGP       default  Arista-Spine3-Q2A-30 L2   Ethernet1          P2P               UP    25          2C                  
IGP       default  Juniper-175-ACX7100-48L L2   Ethernet5          P2P               UP    24          01                  
```

## show isis database detail

```text
Legend:
H - hostname conflict
U - node unreachable

IS-IS Instance: IGP VRF: default
  IS-IS Level 2 Link State Database
    LSPID                   Seq Num  Cksum  Life Length IS  Received LSPID        Flags
    Arista-Spine3-Q2A-30.00-00       550  29371   995   1180 L2  0000.0000.0030.00-00  <>
      Remaining lifetime received: 1199 s Modified to: 1200 s
      NLPID: 0xCC(IPv4) 0x8E(IPv6)
      Hostname: Arista-Spine3-Q2A-30
      Area addresses: 49.0001
      Topology: 2 (IPv6)
      Topology: 0 (IPv4)
      Interface address: 20.30.184.30
      Interface address: 20.30.156.30
      Interface address: 20.30.53.30
      Interface address: 20.30.66.30
      Interface address: 20.30.128.30
      Interface address: 20.30.179.30
      Interface address: 20.30.124.30
      Interface address: 20.30.217.30
      Interface address: 20.30.221.30
      Interface address: 20.30.72.30
      Interface address: 20.30.84.30
      Interface address: 20.30.214.30
      Interface address: 20.30.120.30
      Interface address: 20.30.32.30
      Interface address: 10.0.0.30
      Interface address: 2001:0:30:184::30
      Interface address: 2001:0:30:156::30
      Interface address: 2001:0:53:120::30
      Interface address: 2001:0:30:66::30
      Interface address: 2001:0:30:128::30
      Interface address: 2001:0:30:179::30
      Interface address: 2001:0:30:124::30
      Interface address: 2001:0:30:217::30
      Interface address: 2001:0:30:221::30
      Interface address: 2001:0:30:72::30
      Interface address: 2001:0:30:84::30
      Interface address: 2001:0:30:214::30
      Interface address: 2001:0:30:120::30
      Interface address: 2001:0:30:32::30
      IS Neighbor          : Juniper-156-PTX10002-36QDD.00 Metric: 10
        IPv4 Neighbor Address: 20.30.156.156
        IPv4 Interface Address: 20.30.156.30
        Adj-sid: 362202 flags: [L V] weight: 0x0
      IS Neighbor          : Arrcus-53.00        Metric: 10
        IPv4 Neighbor Address: 20.30.53.53
        IPv4 Interface Address: 20.30.53.30
        Adj-sid: 362193 flags: [L V] weight: 0x0
      IS Neighbor          : Ciena-8140-66.00    Metric: 10
        IPv4 Neighbor Address: 20.30.66.66
        IPv4 Interface Address: 20.30.66.30
        Adj-sid: 362207 flags: [L V] weight: 0x0
      IS Neighbor          : Ciena-5134-72.00    Metric: 10
        IPv4 Neighbor Address: 20.30.72.72
        IPv4 Interface Address: 20.30.72.30
        Adj-sid: 362206 flags: [L V] weight: 0x0
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
      IS Neighbor          : 0000.0000.0128.00   Metric: 10
        IPv4 Neighbor Address: 20.30.128.128
        IPv4 Interface Address: 20.30.128.30
        Adj-sid: 362194 flags: [L V] weight: 0x0
      IS Neighbor          : 221.00              Metric: 10
        IPv4 Neighbor Address: 20.30.221.221
        IPv4 Interface Address: 20.30.221.30
        Adj-sid: 362197 flags: [L V] weight: 0x0
      IS Neighbor          : Nokia-SR1-217.00    Metric: 10
        IPv4 Neighbor Address: 20.30.217.217
        IPv4 Interface Address: 20.30.217.30
        Adj-sid: 362196 flags: [L V] weight: 0x0
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
      Reachability         : 20.30.184.0/24 Metric: 10 Type: 1 Up
      Reachability         : 20.30.156.0/24 Metric: 10 Type: 1 Up
      Reachability         : 20.30.53.0/24 Metric: 10 Type: 1 Up
      Reachability         : 20.30.66.0/24 Metric: 10 Type: 1 Up
      Reachability         : 20.30.128.0/24 Metric: 10 Type: 1 Up
      Reachability         : 20.30.179.0/24 Metric: 10 Type: 1 Up
      Reachability         : 20.30.124.0/24 Metric: 10 Type: 1 Up
      Reachability         : 20.30.217.0/24 Metric: 10 Type: 1 Up
      Reachability         : 20.30.221.0/24 Metric: 10 Type: 1 Up
      Reachability         : 20.30.72.0/24 Metric: 10 Type: 1 Up
      Reachability         : 20.30.84.0/24 Metric: 10 Type: 1 Up
      Reachability         : 20.30.214.0/24 Metric: 10 Type: 1 Up
      Reachability         : 20.30.120.0/24 Metric: 10 Type: 1 Up
      Reachability         : 20.30.32.0/24 Metric: 10 Type: 1 Up
      Reachability         : 10.0.0.30/32 Metric: 0 Type: 1 Up
        SR Prefix-SID: 30 Flags: [N] Algorithm: 0
      Reachability (MT-IPv6): 2001:0:30:184::/64 Metric: 10 Type: 1 Up
      Reachability (MT-IPv6): 2001:0:30:156::/64 Metric: 10 Type: 1 Up
      Reachability (MT-IPv6): 2001:0:53:120::/64 Metric: 10 Type: 1 Up
      Reachability (MT-IPv6): 2001:0:30:66::/64 Metric: 10 Type: 1 Up
      Reachability (MT-IPv6): 2001:0:30:128::/64 Metric: 10 Type: 1 Up
      Reachability (MT-IPv6): 2001:0:30:179::/64 Metric: 10 Type: 1 Up
      Reachability (MT-IPv6): 2001:0:30:124::/64 Metric: 10 Type: 1 Up
      Reachability (MT-IPv6): 2001:0:30:217::/64 Metric: 10 Type: 1 Up
      Reachability (MT-IPv6): 2001:0:30:221::/64 Metric: 10 Type: 1 Up
      Reachability (MT-IPv6): 2001:0:30:72::/64 Metric: 10 Type: 1 Up
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
    Arista-Spine3-Q2A-30.00-01         2   6996  1113     59 L2  0000.0000.0030.00-01  <>
      Remaining lifetime received: 1199 s Modified to: 1200 s
      IS Neighbor          : Keysight-184.00     Metric: 10
        IPv4 Neighbor Address: 20.30.184.184
        IPv4 Interface Address: 20.30.184.30
        Adj-sid: 362208 flags: [L V] weight: 0x0
    Arista-PE32-Q2C-32.00-00       129  18470  1177    306 L2  0000.0000.0032.00-00  <>
      LSP generation remaining wait time: 0 ms
      Time remaining until refresh: 877 s
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
    Arrcus-53.00-00             338  57618  1046    210 L2  0000.0000.0053.00-00  <>
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
    Ciena-8140-66.00-00          91  19411   445    314 L2  0000.0000.0066.00-00  <>
      Remaining lifetime received: 1199 s Modified to: 1200 s
      NLPID: 0xCC(IPv4)
      Hostname: Ciena-8140-66
      Area addresses: 49.0001
      Topology: 0 (IPv4)
      Interface address: 10.0.0.66
      IS Neighbor          : Arista-Spine3-Q2A-30.00 Metric: 10
        IPv4 Neighbor Address: 20.30.66.30
        IPv4 Interface Address: 20.30.66.66
        Adj-sid: 16007 flags: [L V] weight: 0x0
      IS Neighbor          : Juniper-175-ACX7100-48L.00 Metric: 10
        IPv4 Neighbor Address: 20.66.175.175
        IPv4 Interface Address: 20.66.175.66
        Adj-sid: 16006 flags: [L V] weight: 0x0
      Reachability         : 20.66.175.0/24 Metric: 10 Type: 1 Up
      Reachability         : 20.30.66.0/24 Metric: 10 Type: 1 Up
      Reachability         : 10.0.0.66/32 Metric: 10 Type: 1 Up
        SR Prefix-SID: 66 Flags: [N] Algorithm: 0
      Router Capabilities: Router Id: 10.0.0.66 Flags: []
        SR Capability: Flags: [I]
          SRGB Base: 20000 Range: 2000
        Algorithms:  0
    Ciena-5134-72.00-00         444  42962   515    314 L2  0000.0000.0072.00-00  <>
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
    Ericsson_84_R6678.00-00       237  24395   662    277 L2  0000.0000.0084.00-00  <>
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
    H3C_M1A_120.00-00           336  22280  1066    555 L2  0000.0000.0120.00-00  <>
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
    0000.0000.0124.00-00        113  29438   486    297 L2  0000.0000.0124.00-00  <>
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
    0000.0000.0128.00-00        117  59729   659    297 L2  0000.0000.0128.00-00  <>
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
      Reachability         : 20.128.175.0/24 Metric: 10 Type: 1 Up
      Reachability         : 20.30.128.0/24 Metric: 10 Type: 1 Up
      Router Capabilities: Router Id: 10.0.0.128 Flags: []
        Maximum SID depth:
          Base MPLS imposition (MSD type 1):  10
        SR Capability: Flags: [I]
          SRGB Base: 20000 Range: 2000
    Juniper-156-PTX10002-36QDD.00-00        23  63988  1041    408 L2  0000.0000.0156.00-00  <>
      Remaining lifetime received: 1199 s Modified to: 1200 s
      NLPID: 0xCC(IPv4) 0x8E(IPv6)
      Hostname: Juniper-156-PTX10002-36QDD
      Area addresses: 49.0001
      Interface address: 10.0.0.156
      Interface address: 127.0.0.1
      IS Neighbor          : Arista-Spine3-Q2A-30.00 Metric: 10
        IPv4 Neighbor Address: 20.30.156.30
        IPv4 Interface Address: 20.30.156.156
        Global IPv6 Interface Address: 2001:0:30:156::156
        Adj-sid: 20 flags: [L V F] weight: 0x0
        Adj-sid: 19 flags: [L V] weight: 0x0
      IS Neighbor          : Juniper-175-ACX7100-48L.00 Metric: 10
        IPv4 Neighbor Address: 20.156.175.175
        IPv4 Interface Address: 20.156.175.156
        IPv6 Neighbor Address: 2001:0:156:175::175
        Global IPv6 Interface Address: 2001:0:156:175::156
        Adj-sid: 18 flags: [L V F] weight: 0x0
        Adj-sid: 17 flags: [L V] weight: 0x0
      Reachability         : 10.0.0.156/32 Metric: 0 Type: 1 Up
        SR Prefix-SID: 156 Flags: [N] Algorithm: 0
      Reachability         : 20.156.175.0/24 Metric: 10 Type: 1 Up
      Reachability         : 20.30.156.0/24 Metric: 10 Type: 1 Up
      Reachability         : 127.0.0.1/32 Metric: 0 Type: 1 Up
      Reachability          : 2001:0:156:175::/64 Metric: 10 Type: 1 Up
      Reachability          : 2001:0:30:156::/64 Metric: 10 Type: 1 Up
      Router Capabilities: Router Id: 10.0.0.156 Flags: []
        Maximum SID depth:
          Base MPLS imposition (MSD type 1):  0
        SR Capability: Flags: [I V]
          SRGB Base: 20000 Range: 2000
        Algorithms:  0, 1
      Unsupported TLV: Type: 14 Length: 2
    Juniper-175-ACX7100-48L.00-00       173  50236   822   1247 L2  0000.0000.0175.00-00  <>
      Remaining lifetime received: 1199 s Modified to: 1200 s
      NLPID: 0xCC(IPv4) 0x8E(IPv6)
      Hostname: Juniper-175-ACX7100-48L
      Area addresses: 49.0001
      Interface address: 10.0.0.175
      Interface address: 2001:0:32:175::175
      IS Neighbor          : Nokia-SR1-217.00    Metric: 15
        IPv4 Neighbor Address: 20.175.217.217
        IPv4 Interface Address: 20.175.217.175
        IPv6 Neighbor Address: 2001:0:175:217::217
        Global IPv6 Interface Address: 2001:0:175:217::175
        Adj-sid: 62 flags: [L V F] weight: 0x0
        Adj-sid: 61 flags: [L V] weight: 0x0
      IS Neighbor          : 221.00              Metric: 15
        IPv4 Neighbor Address: 20.175.221.221
        IPv4 Interface Address: 20.175.221.175
        Global IPv6 Interface Address: 2001:0:175:221::175
        Adj-sid: 68 flags: [L V F] weight: 0x0
        Adj-sid: 67 flags: [L V] weight: 0x0
      IS Neighbor          : Ericsson_84_R6678.00 Metric: 15
        IPv4 Neighbor Address: 20.84.175.84
        IPv4 Interface Address: 20.84.175.175
        IPv6 Neighbor Address: 2001:0:84:175::175
        Global IPv6 Interface Address: 2001:0:84:175::175
        Adj-sid: 60 flags: [L V F] weight: 0x0
        Adj-sid: 59 flags: [L V] weight: 0x0
      IS Neighbor          : 0000.0000.0128.00   Metric: 15
        IPv4 Neighbor Address: 20.128.175.128
        IPv4 Interface Address: 20.128.175.175
        Global IPv6 Interface Address: 2001:0:128:175::175
        Adj-sid: 72 flags: [L V] weight: 0x0
      IS Neighbor          : 0000.0000.0124.00   Metric: 15
        IPv4 Neighbor Address: 20.124.175.124
        IPv4 Interface Address: 20.124.175.175
        Adj-sid: 71 flags: [L V] weight: 0x0
      IS Neighbor          : Nokia-SXR-214.00    Metric: 15
        IPv4 Neighbor Address: 20.175.214.214
        IPv4 Interface Address: 20.175.214.175
        IPv6 Neighbor Address: 2001:0:175:214::214
        Global IPv6 Interface Address: 2001:0:175:214::175
        Adj-sid: 66 flags: [L V F] weight: 0x0
        Adj-sid: 65 flags: [L V] weight: 0x0
      IS Neighbor          : Arista-PE32-Q2C-32.00 Metric: 15
        IPv4 Neighbor Address: 20.32.175.32
        IPv4 Interface Address: 20.32.175.175
        Global IPv6 Interface Address: 2001:0:32:175::175
        Adj-sid: 74 flags: [L V F] weight: 0x0
        Adj-sid: 73 flags: [L V] weight: 0x0
      IS Neighbor          : Ciena-5134-72.00    Metric: 15
        IPv4 Neighbor Address: 20.72.175.72
        IPv4 Interface Address: 20.72.175.175
        Global IPv6 Interface Address: 2001:0:72:175::175
        Adj-sid: 70 flags: [L V] weight: 0x0
      IS Neighbor          : Juniper-179-ACX7024.00 Metric: 15
        IPv4 Neighbor Address: 20.175.179.179
        IPv4 Interface Address: 20.175.179.175
        IPv6 Neighbor Address: 2001:0:175::179:179
        Global IPv6 Interface Address: 2001:0:175::179:175
        Adj-sid: 82 flags: [L V F] weight: 0x0
        Adj-sid: 81 flags: [L V] weight: 0x0
      IS Neighbor          : H3C_M1A_120.00      Metric: 15
        IPv4 Neighbor Address: 20.120.175.120
        IPv4 Interface Address: 20.120.175.175
        IPv6 Neighbor Address: 2001:0:120:175::120
        Global IPv6 Interface Address: 2001:0:120:175::175
        Adj-sid: 78 flags: [L V F] weight: 0x0
        Adj-sid: 77 flags: [L V] weight: 0x0
      Reachability         : 10.0.0.175/32 Metric: 0 Type: 1 Up
        SR Prefix-SID: 175 Flags: [N] Algorithm: 0
      Reachability         : 20.72.175.0/24 Metric: 15 Type: 1 Up
      Reachability         : 20.175.214.0/24 Metric: 15 Type: 1 Up
      Reachability         : 20.124.175.0/24 Metric: 15 Type: 1 Up
      Reachability         : 20.128.175.0/24 Metric: 15 Type: 1 Up
      Reachability         : 20.84.175.0/24 Metric: 15 Type: 1 Up
      Reachability         : 20.175.221.0/24 Metric: 15 Type: 1 Up
      Reachability         : 20.120.175.0/24 Metric: 15 Type: 1 Up
      Reachability         : 20.175.179.0/24 Metric: 15 Type: 1 Up
      Reachability         : 20.32.175.0/24 Metric: 15 Type: 1 Up
      Reachability         : 20.175.217.0/24 Metric: 15 Type: 1 Up
      Reachability         : 20.131.175.0/24 Metric: 15 Type: 1 Up
      Reachability         : 20.66.175.0/24 Metric: 15 Type: 1 Up
      Reachability         : 20.53.175.0/24 Metric: 15 Type: 1 Up
      Reachability         : 20.156.175.0/24 Metric: 10 Type: 1 Up
      Reachability         : 20.175.184.0/24 Metric: 15 Type: 1 Up
      Reachability          : 2001:0:72:175::/64 Metric: 15 Type: 1 Up
      Reachability          : 2001:0:175:214::/64 Metric: 15 Type: 1 Up
      Reachability          : 2001:0:128:175::/64 Metric: 15 Type: 1 Up
      Reachability          : 2001:0:84:175::/64 Metric: 15 Type: 1 Up
      Reachability          : 2001:0:175:221::/64 Metric: 15 Type: 1 Up
      Reachability          : 2001:0:120:175::/64 Metric: 15 Type: 1 Up
      Reachability          : 2001:0:175::/64 Metric: 15 Type: 1 Up
      Reachability          : 2001:0:32:175::/64 Metric: 15 Type: 1 Up
      Reachability          : 2001:0:175:217::/64 Metric: 15 Type: 1 Up
      Reachability          : 2001:0:131:175::/64 Metric: 15 Type: 1 Up
      Reachability          : 2001:0:66:175::/64 Metric: 15 Type: 1 Up
      Reachability          : 2001:0:53:175::/64 Metric: 15 Type: 1 Up
      Reachability          : 2001:0:156:175::/64 Metric: 10 Type: 1 Up
      Reachability          : 2001:0:175:184::/64 Metric: 15 Type: 1 Up
      Router Capabilities: Router Id: 10.0.0.175 Flags: []
        Maximum SID depth:
          Base MPLS imposition (MSD type 1):  3
        SR Capability: Flags: [I V]
          SRGB Base: 20000 Range: 2000
        Algorithms:  0, 1
      Unsupported TLV: Type: 14 Length: 2
    Juniper-175-ACX7100-48L.00-01       113   7001  1116    304 L2  0000.0000.0175.00-01  <>
      Remaining lifetime received: 1199 s Modified to: 1200 s
      IS Neighbor          : Ciena-8140-66.00    Metric: 15
        IPv4 Neighbor Address: 20.66.175.66
        IPv4 Interface Address: 20.66.175.175
        Global IPv6 Interface Address: 2001:0:66:175::175
        Adj-sid: 84 flags: [L V] weight: 0x0
      IS Neighbor          : Arrcus-53.00        Metric: 15
        IPv4 Neighbor Address: 20.53.175.53
        IPv4 Interface Address: 20.53.175.175
        Global IPv6 Interface Address: 2001:0:53:175::175
        Adj-sid: 91 flags: [L V] weight: 0x0
      IS Neighbor          : Juniper-156-PTX10002-36QDD.00 Metric: 10
        IPv4 Neighbor Address: 20.156.175.156
        IPv4 Interface Address: 20.156.175.175
        IPv6 Neighbor Address: 2001:0:156:175::156
        Global IPv6 Interface Address: 2001:0:156:175::175
        Adj-sid: 93 flags: [L V F] weight: 0x0
        Adj-sid: 92 flags: [L V] weight: 0x0
      IS Neighbor          : Keysight-184.00     Metric: 15
        IPv4 Neighbor Address: 20.175.184.184
        IPv4 Interface Address: 20.175.184.175
        Global IPv6 Interface Address: 2001:0:175:184::175
        Adj-sid: 94 flags: [L V] weight: 0x0
    Juniper-179-ACX7024.00-00       128  63266   946    401 L2  0000.0000.0179.00-00  <>
      Remaining lifetime received: 1199 s Modified to: 1200 s
      NLPID: 0xCC(IPv4) 0x8E(IPv6)
      Hostname: Juniper-179-ACX7024
      Area addresses: 49.0001
      Interface address: 10.0.0.179
      Interface address: 127.0.0.1
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
      Reachability         : 127.0.0.1/32 Metric: 0 Type: 1 Up
      Reachability          : 2001:0:175::/64 Metric: 10 Type: 1 Up
      Reachability          : 2001:0:30:179::/64 Metric: 10 Type: 1 Up
      Router Capabilities: Router Id: 10.0.0.179 Flags: []
        Maximum SID depth:
          Base MPLS imposition (MSD type 1):  8
        SR Capability: Flags: [I V]
          SRGB Base: 20000 Range: 2000
        Algorithms:  0, 1
      Unsupported TLV: Type: 14 Length: 2
    Keysight-184.00-00          373  34085  1197    132 L2  0000.0000.0184.00-00  <DefaultAtt>
      Remaining lifetime received: 1199 s Modified to: 1200 s
      NLPID: 0xCC(IPv4) 0x8E(IPv6) 0x81(CLNP)
      Hostname: Keysight-184
      Area addresses: 49.0001
      Interface address: 20.30.184.184
      IS Neighbor          : Arista-Spine3-Q2A-30.00 Metric: 10
        Adj-sid: 9001 flags: [L V] weight: 0x0
      Reachability         : 10.0.0.184/32 Metric: 10 Type: 1 Up
        SR Prefix-SID: 484 Flags: [N] Algorithm: 0
      Reachability         : 20.30.184.0/24 Metric: 10 Type: 1 Up
      Router Capabilities: Router Id: 10.0.0.184 Flags: []
        SR Capability: Flags: [I V]
          SRGB Base: 20000 Range: 2000
        Algorithms:  0
    Nokia-SXR-214.00-00        8767  20135   712    413 L2  0000.0000.0214.00-00  <>
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
    Nokia-SR1-217.00-00         291  52715   904    435 L2  0100.0000.0217.00-00  <>
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
    221.00-00                   105   9971  1017     80 L2  0221.0221.0221.00-00  <>
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
    221.00-01                   106   3066   738     32 L2  0221.0221.0221.00-01  <>
      Remaining lifetime received: 1199 s Modified to: 1200 s
      Hostname: 221
    221.00-02                   110  64118   534    273 L2  0221.0221.0221.00-02  <>
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

## show isis database traffic-engineering

```text
Legend:
H - hostname conflict
U - node unreachable

IS-IS Instance: IGP VRF: default
  IS-IS Level 2 Link State Database
    LSPID                   Seq Num  Cksum  Life Length IS  Received LSPID        Flags
    Arista-Spine3-Q2A-30.00-00       550  29371   995   1180 L2  0000.0000.0030.00-00  <>
      Remaining lifetime received: 1199 s Modified to: 1200 s
      NLPID: 0xCC(IPv4) 0x8E(IPv6)
      Hostname: Arista-Spine3-Q2A-30
      TE IPv4 router ID: 10.0.0.30
      Area addresses: 49.0001
      Topology: 2 (IPv6)
      Topology: 0 (IPv4)
      Interface address: 20.30.184.30
      Interface address: 20.30.156.30
      Interface address: 20.30.53.30
      Interface address: 20.30.66.30
      Interface address: 20.30.128.30
      Interface address: 20.30.179.30
      Interface address: 20.30.124.30
      Interface address: 20.30.217.30
      Interface address: 20.30.221.30
      Interface address: 20.30.72.30
      Interface address: 20.30.84.30
      Interface address: 20.30.214.30
      Interface address: 20.30.120.30
      Interface address: 20.30.32.30
      Interface address: 10.0.0.30
      Interface address: 2001:0:30:184::30
      Interface address: 2001:0:30:156::30
      Interface address: 2001:0:53:120::30
      Interface address: 2001:0:30:66::30
      Interface address: 2001:0:30:128::30
      Interface address: 2001:0:30:179::30
      Interface address: 2001:0:30:124::30
      Interface address: 2001:0:30:217::30
      Interface address: 2001:0:30:221::30
      Interface address: 2001:0:30:72::30
      Interface address: 2001:0:30:84::30
      Interface address: 2001:0:30:214::30
      Interface address: 2001:0:30:120::30
      Interface address: 2001:0:30:32::30
      IS Neighbor          : Juniper-156-PTX10002-36QDD.00 Metric: 10
        IPv4 Neighbor Address: 20.30.156.156
        IPv4 Interface Address: 20.30.156.30
        Adj-sid: 362202 flags: [L V] weight: 0x0
      IS Neighbor          : Arrcus-53.00        Metric: 10
        IPv4 Neighbor Address: 20.30.53.53
        IPv4 Interface Address: 20.30.53.30
        Adj-sid: 362193 flags: [L V] weight: 0x0
      IS Neighbor          : Ciena-8140-66.00    Metric: 10
        IPv4 Neighbor Address: 20.30.66.66
        IPv4 Interface Address: 20.30.66.30
        Adj-sid: 362207 flags: [L V] weight: 0x0
      IS Neighbor          : Ciena-5134-72.00    Metric: 10
        IPv4 Neighbor Address: 20.30.72.72
        IPv4 Interface Address: 20.30.72.30
        Adj-sid: 362206 flags: [L V] weight: 0x0
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
      IS Neighbor          : 0000.0000.0128.00   Metric: 10
        IPv4 Neighbor Address: 20.30.128.128
        IPv4 Interface Address: 20.30.128.30
        Adj-sid: 362194 flags: [L V] weight: 0x0
      IS Neighbor          : 221.00              Metric: 10
        IPv4 Neighbor Address: 20.30.221.221
        IPv4 Interface Address: 20.30.221.30
        Adj-sid: 362197 flags: [L V] weight: 0x0
      IS Neighbor          : Nokia-SR1-217.00    Metric: 10
        IPv4 Neighbor Address: 20.30.217.217
        IPv4 Interface Address: 20.30.217.30
        Adj-sid: 362196 flags: [L V] weight: 0x0
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
      Reachability         : 20.30.184.0/24 Metric: 10 Type: 1 Up
      Reachability         : 20.30.156.0/24 Metric: 10 Type: 1 Up
      Reachability         : 20.30.53.0/24 Metric: 10 Type: 1 Up
      Reachability         : 20.30.66.0/24 Metric: 10 Type: 1 Up
      Reachability         : 20.30.128.0/24 Metric: 10 Type: 1 Up
      Reachability         : 20.30.179.0/24 Metric: 10 Type: 1 Up
      Reachability         : 20.30.124.0/24 Metric: 10 Type: 1 Up
      Reachability         : 20.30.217.0/24 Metric: 10 Type: 1 Up
      Reachability         : 20.30.221.0/24 Metric: 10 Type: 1 Up
      Reachability         : 20.30.72.0/24 Metric: 10 Type: 1 Up
      Reachability         : 20.30.84.0/24 Metric: 10 Type: 1 Up
      Reachability         : 20.30.214.0/24 Metric: 10 Type: 1 Up
      Reachability         : 20.30.120.0/24 Metric: 10 Type: 1 Up
      Reachability         : 20.30.32.0/24 Metric: 10 Type: 1 Up
      Reachability         : 10.0.0.30/32 Metric: 0 Type: 1 Up
        SR Prefix-SID: 30 Flags: [N] Algorithm: 0
      Reachability (MT-IPv6): 2001:0:30:184::/64 Metric: 10 Type: 1 Up
      Reachability (MT-IPv6): 2001:0:30:156::/64 Metric: 10 Type: 1 Up
      Reachability (MT-IPv6): 2001:0:53:120::/64 Metric: 10 Type: 1 Up
      Reachability (MT-IPv6): 2001:0:30:66::/64 Metric: 10 Type: 1 Up
      Reachability (MT-IPv6): 2001:0:30:128::/64 Metric: 10 Type: 1 Up
      Reachability (MT-IPv6): 2001:0:30:179::/64 Metric: 10 Type: 1 Up
      Reachability (MT-IPv6): 2001:0:30:124::/64 Metric: 10 Type: 1 Up
      Reachability (MT-IPv6): 2001:0:30:217::/64 Metric: 10 Type: 1 Up
      Reachability (MT-IPv6): 2001:0:30:221::/64 Metric: 10 Type: 1 Up
      Reachability (MT-IPv6): 2001:0:30:72::/64 Metric: 10 Type: 1 Up
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
    Arista-Spine3-Q2A-30.00-01         2   6996  1113     59 L2  0000.0000.0030.00-01  <>
      Remaining lifetime received: 1199 s Modified to: 1200 s
      IS Neighbor          : Keysight-184.00     Metric: 10
        IPv4 Neighbor Address: 20.30.184.184
        IPv4 Interface Address: 20.30.184.30
        Adj-sid: 362208 flags: [L V] weight: 0x0
    Arista-PE32-Q2C-32.00-00       129  18470  1176    306 L2  0000.0000.0032.00-00  <>
      LSP generation remaining wait time: 0 ms
      Time remaining until refresh: 876 s
      NLPID: 0xCC(IPv4) 0x8E(IPv6)
      Hostname: Arista-PE32-Q2C-32
      TE IPv4 router ID: 10.0.0.32
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
    Arrcus-53.00-00             338  57618  1045    210 L2  0000.0000.0053.00-00  <>
      Remaining lifetime received: 1199 s Modified to: 1200 s
      NLPID: 0xCC(IPv4)
      Hostname: Arrcus-53
      TE IPv4 router ID: 10.0.0.53
      Area addresses: 49.0001
      Interface address: 10.0.0.53
      IS Neighbor          : Arista-Spine3-Q2A-30.00 Metric: 10
        IPv4 Neighbor Address: 20.30.53.30
        IPv4 Interface Address: 20.30.53.53
        Adj-sid: 30000 flags: [L V] weight: 0x0
      IS Neighbor          : Juniper-175-ACX7100-48L.00 Metric: 10
        IPv4 Neighbor Address: 20.53.175.175
        IPv4 Interface Address: 20.53.175.53
        Application Specific Link Attributes:
          Standard applications: SR-TE
            Administrative group (Color): 20
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
    Ciena-8140-66.00-00          91  19411   445    314 L2  0000.0000.0066.00-00  <>
      Remaining lifetime received: 1199 s Modified to: 1200 s
      NLPID: 0xCC(IPv4)
      Hostname: Ciena-8140-66
      TE IPv4 router ID: 10.0.0.66
      Area addresses: 49.0001
      Topology: 0 (IPv4)
      Interface address: 10.0.0.66
      IS Neighbor          : Arista-Spine3-Q2A-30.00 Metric: 10
        IPv4 Neighbor Address: 20.30.66.30
        IPv4 Interface Address: 20.30.66.66
        Adj-sid: 16007 flags: [L V] weight: 0x0
        Maximum link BW: 10.00 Gbps
        Maximum reservable link BW: 10.00 Gbps
        Unreserved BW:
            TE class 0: 10.00 Gbps	TE class 1: 10.00 Gbps	TE class 2: 10.00 Gbps
            TE class 3: 10.00 Gbps	TE class 4: 10.00 Gbps	TE class 5: 10.00 Gbps
            TE class 6: 10.00 Gbps	TE class 7: 10.00 Gbps
        Local link ID: 1073731827
        Remote link ID: 113
        Application Specific Link Attributes:
          Standard applications: [L] RSVP-TE SR-TE LFA Flex-Algo
      IS Neighbor          : Juniper-175-ACX7100-48L.00 Metric: 10
        IPv4 Neighbor Address: 20.66.175.175
        IPv4 Interface Address: 20.66.175.66
        Adj-sid: 16006 flags: [L V] weight: 0x0
        Maximum link BW: 10.00 Gbps
        Maximum reservable link BW: 10.00 Gbps
        Unreserved BW:
            TE class 0: 10.00 Gbps	TE class 1: 10.00 Gbps	TE class 2: 10.00 Gbps
            TE class 3: 10.00 Gbps	TE class 4: 10.00 Gbps	TE class 5: 10.00 Gbps
            TE class 6: 10.00 Gbps	TE class 7: 10.00 Gbps
        Local link ID: 1073731826
        Remote link ID: 1016
        Application Specific Link Attributes:
          Standard applications: [L] RSVP-TE SR-TE LFA Flex-Algo
      Reachability         : 20.66.175.0/24 Metric: 10 Type: 1 Up
      Reachability         : 20.30.66.0/24 Metric: 10 Type: 1 Up
      Reachability         : 10.0.0.66/32 Metric: 10 Type: 1 Up
        SR Prefix-SID: 66 Flags: [N] Algorithm: 0
      Router Capabilities: Router Id: 10.0.0.66 Flags: []
        SR Capability: Flags: [I]
          SRGB Base: 20000 Range: 2000
        Algorithms:  0
    Ciena-5134-72.00-00         444  42962   514    314 L2  0000.0000.0072.00-00  <>
      Remaining lifetime received: 1199 s Modified to: 1200 s
      NLPID: 0xCC(IPv4)
      Hostname: Ciena-5134-72
      TE IPv4 router ID: 10.0.0.72
      Area addresses: 49.0001
      Topology: 0 (IPv4)
      Interface address: 10.0.0.72
      IS Neighbor          : Juniper-175-ACX7100-48L.00 Metric: 10
        IPv4 Neighbor Address: 20.72.175.175
        IPv4 Interface Address: 20.72.175.72
        Adj-sid: 16002 flags: [L V] weight: 0x0
        Maximum link BW: 10.00 Gbps
        Maximum reservable link BW: 10.00 Gbps
        Unreserved BW:
            TE class 0: 10.00 Gbps	TE class 1: 10.00 Gbps	TE class 2: 10.00 Gbps
            TE class 3: 10.00 Gbps	TE class 4: 10.00 Gbps	TE class 5: 10.00 Gbps
            TE class 6: 10.00 Gbps	TE class 7: 10.00 Gbps
        Local link ID: 1073731829
        Remote link ID: 1015
        Application Specific Link Attributes:
          Standard applications: [L] RSVP-TE SR-TE LFA Flex-Algo
      IS Neighbor          : Arista-Spine3-Q2A-30.00 Metric: 10
        IPv4 Neighbor Address: 20.30.72.30
        IPv4 Interface Address: 20.30.72.72
        Adj-sid: 16003 flags: [L V] weight: 0x0
        Maximum link BW: 10.00 Gbps
        Maximum reservable link BW: 10.00 Gbps
        Unreserved BW:
            TE class 0: 10.00 Gbps	TE class 1: 10.00 Gbps	TE class 2: 10.00 Gbps
            TE class 3: 10.00 Gbps	TE class 4: 10.00 Gbps	TE class 5: 10.00 Gbps
            TE class 6: 10.00 Gbps	TE class 7: 10.00 Gbps
        Local link ID: 1073731830
        Remote link ID: 89
        Application Specific Link Attributes:
          Standard applications: [L] RSVP-TE SR-TE LFA Flex-Algo
      Reachability         : 20.72.175.0/24 Metric: 10 Type: 1 Up
      Reachability         : 20.30.72.0/24 Metric: 10 Type: 1 Up
      Reachability         : 10.0.0.72/32 Metric: 10 Type: 1 Up
        SR Prefix-SID: 72 Flags: [N] Algorithm: 0
      Router Capabilities: Router Id: 10.0.0.72 Flags: []
        SR Capability: Flags: [I]
          SRGB Base: 20000 Range: 2000
        Algorithms:  0
    Ericsson_84_R6678.00-00       237  24395   662    277 L2  0000.0000.0084.00-00  <>
      Remaining lifetime received: 1199 s Modified to: 1200 s
      NLPID: 0xCC(IPv4) 0x8E(IPv6)
      Hostname: Ericsson_84_R6678
      TE IPv4 router ID: 10.0.0.84
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
    H3C_M1A_120.00-00           336  22280  1066    555 L2  0000.0000.0120.00-00  <>
      Remaining lifetime received: 1199 s Modified to: 1200 s
      NLPID: 0xCC(IPv4) 0x8E(IPv6)
      Hostname: H3C_M1A_120
      TE IPv4 router ID: 10.0.0.120
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
        TE default metric: 10
        Maximum link BW: 0.00 bps
        Maximum reservable link BW: 0.00 bps
        Unreserved BW:
            TE class 0: 0.00 bps	TE class 1: 0.00 bps	TE class 2: 0.00 bps
            TE class 3: 0.00 bps	TE class 4: 0.00 bps	TE class 5: 0.00 bps
            TE class 6: 0.00 bps	TE class 7: 0.00 bps
        Local link ID: 1
        Remote link ID: 76
      IS Neighbor          : Juniper-175-ACX7100-48L.00 Metric: 10
        IPv4 Neighbor Address: 20.120.175.175
        IPv4 Interface Address: 20.120.175.120
        Adj-sid: 1141 flags: [L V] weight: 0x0
        TE default metric: 10
        Maximum link BW: 0.00 bps
        Maximum reservable link BW: 0.00 bps
        Unreserved BW:
            TE class 0: 0.00 bps	TE class 1: 0.00 bps	TE class 2: 0.00 bps
            TE class 3: 0.00 bps	TE class 4: 0.00 bps	TE class 5: 0.00 bps
            TE class 6: 0.00 bps	TE class 7: 0.00 bps
        Local link ID: 4
        Remote link ID: 1007
      IS Neighbor (MT-IPv6): Arista-Spine3-Q2A-30.00 Metric: 10
        Local link ID: 1
        Remote link ID: 76
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
    0000.0000.0124.00-00        113  29438   486    297 L2  0000.0000.0124.00-00  <>
      Remaining lifetime received: 1199 s Modified to: 1200 s
      NLPID: 0xCC(IPv4) 0x8E(IPv6)
      TE IPv4 router ID: 10.0.0.124
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
        TE default metric: 10
        Maximum link BW: 1.00 Gbps
        Maximum reservable link BW: 0.00 bps
        Unreserved BW:
            TE class 0: 0.00 bps	TE class 1: 0.00 bps	TE class 2: 0.00 bps
            TE class 3: 0.00 bps	TE class 4: 0.00 bps	TE class 5: 0.00 bps
            TE class 6: 0.00 bps	TE class 7: 0.00 bps
      IS Neighbor          : Arista-Spine3-Q2A-30.00 Metric: 10
        IPv4 Neighbor Address: 20.30.124.30
        IPv4 Interface Address: 20.30.124.124
        Adj-sid: 397 flags: [L V] weight: 0x0
        TE default metric: 10
        Maximum link BW: 1.00 Gbps
        Maximum reservable link BW: 0.00 bps
        Unreserved BW:
            TE class 0: 0.00 bps	TE class 1: 0.00 bps	TE class 2: 0.00 bps
            TE class 3: 0.00 bps	TE class 4: 0.00 bps	TE class 5: 0.00 bps
            TE class 6: 0.00 bps	TE class 7: 0.00 bps
      Reachability         : 20.30.124.0/24 Metric: 10 Type: 1 Up
      Reachability         : 20.124.175.0/24 Metric: 10 Type: 1 Up
      Reachability         : 10.0.0.124/32 Metric: 0 Type: 1 Up
        SR Prefix-SID: 124 Flags: [N P] Algorithm: 0
      Router Capabilities: Router Id: 10.0.0.124 Flags: []
        Maximum SID depth:
          Base MPLS imposition (MSD type 1):  10
        SR Capability: Flags: [I]
          SRGB Base: 2000 Range: 2001
    0000.0000.0128.00-00        117  59729   659    297 L2  0000.0000.0128.00-00  <>
      Remaining lifetime received: 1199 s Modified to: 1200 s
      NLPID: 0xCC(IPv4) 0x8E(IPv6)
      TE IPv4 router ID: 10.0.0.128
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
        TE default metric: 10
        Maximum link BW: 10.00 Gbps
        Maximum reservable link BW: 0.00 bps
        Unreserved BW:
            TE class 0: 0.00 bps	TE class 1: 0.00 bps	TE class 2: 0.00 bps
            TE class 3: 0.00 bps	TE class 4: 0.00 bps	TE class 5: 0.00 bps
            TE class 6: 0.00 bps	TE class 7: 0.00 bps
      IS Neighbor          : Arista-Spine3-Q2A-30.00 Metric: 10
        IPv4 Neighbor Address: 20.30.128.30
        IPv4 Interface Address: 20.30.128.128
        Adj-sid: 48122 flags: [L V] weight: 0x0
        TE default metric: 10
        Maximum link BW: 10.00 Gbps
        Maximum reservable link BW: 0.00 bps
        Unreserved BW:
            TE class 0: 0.00 bps	TE class 1: 0.00 bps	TE class 2: 0.00 bps
            TE class 3: 0.00 bps	TE class 4: 0.00 bps	TE class 5: 0.00 bps
            TE class 6: 0.00 bps	TE class 7: 0.00 bps
      Reachability         : 10.0.0.128/32 Metric: 0 Type: 1 Up
        SR Prefix-SID: 128 Flags: [N] Algorithm: 0
      Reachability         : 20.128.175.0/24 Metric: 10 Type: 1 Up
      Reachability         : 20.30.128.0/24 Metric: 10 Type: 1 Up
      Router Capabilities: Router Id: 10.0.0.128 Flags: []
        Maximum SID depth:
          Base MPLS imposition (MSD type 1):  10
        SR Capability: Flags: [I]
          SRGB Base: 20000 Range: 2000
    Juniper-156-PTX10002-36QDD.00-00        23  63988  1041    408 L2  0000.0000.0156.00-00  <>
      Remaining lifetime received: 1199 s Modified to: 1200 s
      NLPID: 0xCC(IPv4) 0x8E(IPv6)
      Hostname: Juniper-156-PTX10002-36QDD
      TE IPv4 router ID: 10.0.0.156
      TE IPv6 router ID: 2001:0:30:156::156
      Area addresses: 49.0001
      Interface address: 10.0.0.156
      Interface address: 127.0.0.1
      IS Neighbor          : Arista-Spine3-Q2A-30.00 Metric: 10
        IPv4 Neighbor Address: 20.30.156.30
        IPv4 Interface Address: 20.30.156.156
        Global IPv6 Interface Address: 2001:0:30:156::156
        Adj-sid: 20 flags: [L V F] weight: 0x0
        Adj-sid: 19 flags: [L V] weight: 0x0
        Administrative group (Color): 8
        Maximum link BW: 10.00 Gbps
        Local link ID: 1006
        Remote link ID: 123
      IS Neighbor          : Juniper-175-ACX7100-48L.00 Metric: 10
        IPv4 Neighbor Address: 20.156.175.175
        IPv4 Interface Address: 20.156.175.156
        IPv6 Neighbor Address: 2001:0:156:175::175
        Global IPv6 Interface Address: 2001:0:156:175::156
        Adj-sid: 18 flags: [L V F] weight: 0x0
        Adj-sid: 17 flags: [L V] weight: 0x0
        Administrative group (Color): 7
        Maximum link BW: 10.00 Gbps
        Local link ID: 1007
        Remote link ID: 1056
      Reachability         : 10.0.0.156/32 Metric: 0 Type: 1 Up
        SR Prefix-SID: 156 Flags: [N] Algorithm: 0
      Reachability         : 20.156.175.0/24 Metric: 10 Type: 1 Up
      Reachability         : 20.30.156.0/24 Metric: 10 Type: 1 Up
      Reachability         : 127.0.0.1/32 Metric: 0 Type: 1 Up
      Reachability          : 2001:0:156:175::/64 Metric: 10 Type: 1 Up
      Reachability          : 2001:0:30:156::/64 Metric: 10 Type: 1 Up
      Router Capabilities: Router Id: 10.0.0.156 Flags: []
        Maximum SID depth:
          Base MPLS imposition (MSD type 1):  0
        SR Capability: Flags: [I V]
          SRGB Base: 20000 Range: 2000
        Algorithms:  0, 1
      Unsupported TLV: Type: 14 Length: 2
    Juniper-175-ACX7100-48L.00-00       173  50236   822   1247 L2  0000.0000.0175.00-00  <>
      Remaining lifetime received: 1199 s Modified to: 1200 s
      NLPID: 0xCC(IPv4) 0x8E(IPv6)
      Hostname: Juniper-175-ACX7100-48L
      TE IPv4 router ID: 10.0.0.175
      TE IPv6 router ID: 2001:0:32:175::175
      Area addresses: 49.0001
      Interface address: 10.0.0.175
      Interface address: 2001:0:32:175::175
      IS Neighbor          : Nokia-SR1-217.00    Metric: 15
        IPv4 Neighbor Address: 20.175.217.217
        IPv4 Interface Address: 20.175.217.175
        IPv6 Neighbor Address: 2001:0:175:217::217
        Global IPv6 Interface Address: 2001:0:175:217::175
        Adj-sid: 62 flags: [L V F] weight: 0x0
        Adj-sid: 61 flags: [L V] weight: 0x0
        Local link ID: 1003
        Remote link ID: 10
      IS Neighbor          : 221.00              Metric: 15
        IPv4 Neighbor Address: 20.175.221.221
        IPv4 Interface Address: 20.175.221.175
        Global IPv6 Interface Address: 2001:0:175:221::175
        Adj-sid: 68 flags: [L V F] weight: 0x0
        Adj-sid: 67 flags: [L V] weight: 0x0
        Local link ID: 1009
        Remote link ID: 8388613
      IS Neighbor          : Ericsson_84_R6678.00 Metric: 15
        IPv4 Neighbor Address: 20.84.175.84
        IPv4 Interface Address: 20.84.175.175
        IPv6 Neighbor Address: 2001:0:84:175::175
        Global IPv6 Interface Address: 2001:0:84:175::175
        Adj-sid: 60 flags: [L V F] weight: 0x0
        Adj-sid: 59 flags: [L V] weight: 0x0
        Local link ID: 1010
        Remote link ID: 528
      IS Neighbor          : 0000.0000.0128.00   Metric: 15
        IPv4 Neighbor Address: 20.128.175.128
        IPv4 Interface Address: 20.128.175.175
        Global IPv6 Interface Address: 2001:0:128:175::175
        Adj-sid: 72 flags: [L V] weight: 0x0
        Local link ID: 1011
        Remote link ID: 9
      IS Neighbor          : 0000.0000.0124.00   Metric: 15
        IPv4 Neighbor Address: 20.124.175.124
        IPv4 Interface Address: 20.124.175.175
        Adj-sid: 71 flags: [L V] weight: 0x0
        Local link ID: 1013
        Remote link ID: 11
      IS Neighbor          : Nokia-SXR-214.00    Metric: 15
        IPv4 Neighbor Address: 20.175.214.214
        IPv4 Interface Address: 20.175.214.175
        IPv6 Neighbor Address: 2001:0:175:214::214
        Global IPv6 Interface Address: 2001:0:175:214::175
        Adj-sid: 66 flags: [L V F] weight: 0x0
        Adj-sid: 65 flags: [L V] weight: 0x0
        Local link ID: 1014
        Remote link ID: 11
      IS Neighbor          : Arista-PE32-Q2C-32.00 Metric: 15
        IPv4 Neighbor Address: 20.32.175.32
        IPv4 Interface Address: 20.32.175.175
        Global IPv6 Interface Address: 2001:0:32:175::175
        Adj-sid: 74 flags: [L V F] weight: 0x0
        Adj-sid: 73 flags: [L V] weight: 0x0
        Local link ID: 1004
        Remote link ID: 88
      IS Neighbor          : Ciena-5134-72.00    Metric: 15
        IPv4 Neighbor Address: 20.72.175.72
        IPv4 Interface Address: 20.72.175.175
        Global IPv6 Interface Address: 2001:0:72:175::175
        Adj-sid: 70 flags: [L V] weight: 0x0
        Local link ID: 1015
        Remote link ID: 1073731829
      IS Neighbor          : Juniper-179-ACX7024.00 Metric: 15
        IPv4 Neighbor Address: 20.175.179.179
        IPv4 Interface Address: 20.175.179.175
        IPv6 Neighbor Address: 2001:0:175::179:179
        Global IPv6 Interface Address: 2001:0:175::179:175
        Adj-sid: 82 flags: [L V F] weight: 0x0
        Adj-sid: 81 flags: [L V] weight: 0x0
        Local link ID: 1005
        Remote link ID: 1010
      IS Neighbor          : H3C_M1A_120.00      Metric: 15
        IPv4 Neighbor Address: 20.120.175.120
        IPv4 Interface Address: 20.120.175.175
        IPv6 Neighbor Address: 2001:0:120:175::120
        Global IPv6 Interface Address: 2001:0:120:175::175
        Adj-sid: 78 flags: [L V F] weight: 0x0
        Adj-sid: 77 flags: [L V] weight: 0x0
        Local link ID: 1007
        Remote link ID: 4
      Reachability         : 10.0.0.175/32 Metric: 0 Type: 1 Up
        SR Prefix-SID: 175 Flags: [N] Algorithm: 0
      Reachability         : 20.72.175.0/24 Metric: 15 Type: 1 Up
      Reachability         : 20.175.214.0/24 Metric: 15 Type: 1 Up
      Reachability         : 20.124.175.0/24 Metric: 15 Type: 1 Up
      Reachability         : 20.128.175.0/24 Metric: 15 Type: 1 Up
      Reachability         : 20.84.175.0/24 Metric: 15 Type: 1 Up
      Reachability         : 20.175.221.0/24 Metric: 15 Type: 1 Up
      Reachability         : 20.120.175.0/24 Metric: 15 Type: 1 Up
      Reachability         : 20.175.179.0/24 Metric: 15 Type: 1 Up
      Reachability         : 20.32.175.0/24 Metric: 15 Type: 1 Up
      Reachability         : 20.175.217.0/24 Metric: 15 Type: 1 Up
      Reachability         : 20.131.175.0/24 Metric: 15 Type: 1 Up
      Reachability         : 20.66.175.0/24 Metric: 15 Type: 1 Up
      Reachability         : 20.53.175.0/24 Metric: 15 Type: 1 Up
      Reachability         : 20.156.175.0/24 Metric: 10 Type: 1 Up
      Reachability         : 20.175.184.0/24 Metric: 15 Type: 1 Up
      Reachability          : 2001:0:72:175::/64 Metric: 15 Type: 1 Up
      Reachability          : 2001:0:175:214::/64 Metric: 15 Type: 1 Up
      Reachability          : 2001:0:128:175::/64 Metric: 15 Type: 1 Up
      Reachability          : 2001:0:84:175::/64 Metric: 15 Type: 1 Up
      Reachability          : 2001:0:175:221::/64 Metric: 15 Type: 1 Up
      Reachability          : 2001:0:120:175::/64 Metric: 15 Type: 1 Up
      Reachability          : 2001:0:175::/64 Metric: 15 Type: 1 Up
      Reachability          : 2001:0:32:175::/64 Metric: 15 Type: 1 Up
      Reachability          : 2001:0:175:217::/64 Metric: 15 Type: 1 Up
      Reachability          : 2001:0:131:175::/64 Metric: 15 Type: 1 Up
      Reachability          : 2001:0:66:175::/64 Metric: 15 Type: 1 Up
      Reachability          : 2001:0:53:175::/64 Metric: 15 Type: 1 Up
      Reachability          : 2001:0:156:175::/64 Metric: 10 Type: 1 Up
      Reachability          : 2001:0:175:184::/64 Metric: 15 Type: 1 Up
      Router Capabilities: Router Id: 10.0.0.175 Flags: []
        Maximum SID depth:
          Base MPLS imposition (MSD type 1):  3
        SR Capability: Flags: [I V]
          SRGB Base: 20000 Range: 2000
        Algorithms:  0, 1
      Unsupported TLV: Type: 14 Length: 2
    Juniper-175-ACX7100-48L.00-01       113   7001  1116    304 L2  0000.0000.0175.00-01  <>
      Remaining lifetime received: 1199 s Modified to: 1200 s
      IS Neighbor          : Ciena-8140-66.00    Metric: 15
        IPv4 Neighbor Address: 20.66.175.66
        IPv4 Interface Address: 20.66.175.175
        Global IPv6 Interface Address: 2001:0:66:175::175
        Adj-sid: 84 flags: [L V] weight: 0x0
        Local link ID: 1016
        Remote link ID: 1073731826
      IS Neighbor          : Arrcus-53.00        Metric: 15
        IPv4 Neighbor Address: 20.53.175.53
        IPv4 Interface Address: 20.53.175.175
        Global IPv6 Interface Address: 2001:0:53:175::175
        Adj-sid: 91 flags: [L V] weight: 0x0
        Local link ID: 1008
        Remote link ID: 1002
      IS Neighbor          : Juniper-156-PTX10002-36QDD.00 Metric: 10
        IPv4 Neighbor Address: 20.156.175.156
        IPv4 Interface Address: 20.156.175.175
        IPv6 Neighbor Address: 2001:0:156:175::156
        Global IPv6 Interface Address: 2001:0:156:175::175
        Adj-sid: 93 flags: [L V F] weight: 0x0
        Adj-sid: 92 flags: [L V] weight: 0x0
        Local link ID: 1056
        Remote link ID: 1007
      IS Neighbor          : Keysight-184.00     Metric: 15
        IPv4 Neighbor Address: 20.175.184.184
        IPv4 Interface Address: 20.175.184.175
        Global IPv6 Interface Address: 2001:0:175:184::175
        Adj-sid: 94 flags: [L V] weight: 0x0
        Local link ID: 1012
        Remote link ID: 1
    Juniper-179-ACX7024.00-00       128  63266   946    401 L2  0000.0000.0179.00-00  <>
      Remaining lifetime received: 1199 s Modified to: 1200 s
      NLPID: 0xCC(IPv4) 0x8E(IPv6)
      Hostname: Juniper-179-ACX7024
      TE IPv4 router ID: 10.0.0.179
      TE IPv6 router ID: 2001:0:30:179::179
      Area addresses: 49.0001
      Interface address: 10.0.0.179
      Interface address: 127.0.0.1
      IS Neighbor          : Juniper-175-ACX7100-48L.00 Metric: 10
        IPv4 Neighbor Address: 20.175.179.175
        IPv4 Interface Address: 20.175.179.179
        IPv6 Neighbor Address: 2001:0:175::179:175
        Global IPv6 Interface Address: 2001:0:175::179:179
        Adj-sid: 20 flags: [L V F] weight: 0x0
        Adj-sid: 19 flags: [L V] weight: 0x0
        Administrative group (Color): 7
        Maximum link BW: 10.00 Gbps
        Local link ID: 1010
        Remote link ID: 1005
      IS Neighbor          : Arista-Spine3-Q2A-30.00 Metric: 10
        IPv4 Neighbor Address: 20.30.179.30
        IPv4 Interface Address: 20.30.179.179
        Global IPv6 Interface Address: 2001:0:30:179::179
        Adj-sid: 18 flags: [L V F] weight: 0x0
        Adj-sid: 17 flags: [L V] weight: 0x0
        Administrative group (Color): 8
        Maximum link BW: 10.00 Gbps
        Local link ID: 1014
        Remote link ID: 82
      Reachability         : 10.0.0.179/32 Metric: 0 Type: 1 Up
        SR Prefix-SID: 179 Flags: [N] Algorithm: 0
      Reachability         : 20.175.179.0/24 Metric: 10 Type: 1 Up
      Reachability         : 20.30.179.0/24 Metric: 10 Type: 1 Up
      Reachability         : 127.0.0.1/32 Metric: 0 Type: 1 Up
      Reachability          : 2001:0:175::/64 Metric: 10 Type: 1 Up
      Reachability          : 2001:0:30:179::/64 Metric: 10 Type: 1 Up
      Router Capabilities: Router Id: 10.0.0.179 Flags: []
        Maximum SID depth:
          Base MPLS imposition (MSD type 1):  8
        SR Capability: Flags: [I V]
          SRGB Base: 20000 Range: 2000
        Algorithms:  0, 1
      Unsupported TLV: Type: 14 Length: 2
    Keysight-184.00-00          373  34085  1197    132 L2  0000.0000.0184.00-00  <DefaultAtt>
      Remaining lifetime received: 1199 s Modified to: 1200 s
      NLPID: 0xCC(IPv4) 0x8E(IPv6) 0x81(CLNP)
      Hostname: Keysight-184
      Area addresses: 49.0001
      Interface address: 20.30.184.184
      IS Neighbor          : Arista-Spine3-Q2A-30.00 Metric: 10
        Adj-sid: 9001 flags: [L V] weight: 0x0
      Reachability         : 10.0.0.184/32 Metric: 10 Type: 1 Up
        SR Prefix-SID: 484 Flags: [N] Algorithm: 0
      Reachability         : 20.30.184.0/24 Metric: 10 Type: 1 Up
      Router Capabilities: Router Id: 10.0.0.184 Flags: []
        SR Capability: Flags: [I V]
          SRGB Base: 20000 Range: 2000
        Algorithms:  0
    Nokia-SXR-214.00-00        8767  20135   712    413 L2  0000.0000.0214.00-00  <>
      Remaining lifetime received: 1199 s Modified to: 1200 s
      NLPID: 0xCC(IPv4) 0x8E(IPv6)
      Hostname: Nokia-SXR-214
      TE IPv4 router ID: 10.0.0.214
      TE IPv6 router ID: 2000::214
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
        IPv6 Neighbor Address: 2001:0:175:214::175
        Global IPv6 Interface Address: 2001:0:175:214::214
        Adj-sid: 30016 flags: [L V B] weight: 0x0
        Adj-sid: 30017 flags: [L V B F] weight: 0x0
        Application Specific Link Attributes:
          Standard applications: SR-TE
            Maximum link BW: 80.00 Mbps
      IS Neighbor          : Arista-Spine3-Q2A-30.00 Metric: 10
        IPv4 Neighbor Address: 20.30.214.30
        IPv4 Interface Address: 20.30.214.214
        Adj-sid: 30018 flags: [L V B] weight: 0x0
        Adj-sid: 30019 flags: [L V B F] weight: 0x0
        Application Specific Link Attributes:
          Standard applications: SR-TE
            Maximum link BW: 80.00 Mbps
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
    Nokia-SR1-217.00-00         291  52715   904    435 L2  0100.0000.0217.00-00  <>
      Remaining lifetime received: 1199 s Modified to: 1200 s
      NLPID: 0xCC(IPv4) 0x8E(IPv6)
      Hostname: Nokia-SR1-217
      TE IPv4 router ID: 10.0.0.217
      TE IPv6 router ID: 2002::217
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
        Application Specific Link Attributes:
          Standard applications: SR-TE
            Administrative group (Color): 2
            Maximum link BW: 10.00 Gbps
      IS Neighbor          : Arista-Spine3-Q2A-30.00 Metric: 10
        IPv4 Neighbor Address: 20.30.217.30
        IPv4 Interface Address: 20.30.217.217
        Adj-sid: 524282 flags: [L V B] weight: 0x0
        Adj-sid: 524281 flags: [L V B F] weight: 0x0
        Application Specific Link Attributes:
          Standard applications: SR-TE
            Administrative group (Color): 1
            Maximum link BW: 10.00 Gbps
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
    221.00-00                   105   9971  1017     80 L2  0221.0221.0221.00-00  <>
      Remaining lifetime received: 1199 s Modified to: 1200 s
      NLPID: 0xCC(IPv4) 0x8E(IPv6)
      TE IPv4 router ID: 10.0.0.221
      Area addresses: 49.0001
      Router Capabilities: Router Id: 10.0.0.221 Flags: []
        SR Local Block:
          SRLB Base: 626688 Range: 14336
        Maximum SID depth:
          Base MPLS imposition (MSD type 1):  10
        SR Capability: Flags: [I]
          SRGB Base: 720000 Range: 2000
      Unsupported TLV: Type: 14 Length: 2
    221.00-01                   106   3066   738     32 L2  0221.0221.0221.00-01  <>
      Remaining lifetime received: 1199 s Modified to: 1200 s
      Hostname: 221
    221.00-02                   110  64118   533    273 L2  0221.0221.0221.00-02  <>
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
  2         10.0.0.84/32      TI-LFA (1)                 -            [ 20084 ]
  5         10.0.0.30/32      TI-LFA (3)                 -            [ 3 ]    
  6         10.0.0.53/32      TI-LFA (1)                 -            [ 20053 ]
  7         10.0.0.179/32     TI-LFA (1)                 -            [ 20179 ]
  8         10.0.0.120/32     TI-LFA (1)                 -            [ 20120 ]
  9         10.0.0.72/32      TI-LFA (1)                 -            [ 20072 ]
  10        10.0.0.214/32     TI-LFA (1)                 -            [ 20214 ]
  11        10.0.0.128/32     TI-LFA (1)                 -            [ 20128 ]
  13        10.0.0.221/32     TI-LFA (1)                 -            [ 21221 ]
  14        10.0.0.124/32     TI-LFA (1)                 -            [ 20124 ]
  15        10.0.0.184/32     TI-LFA (1)                 -            [ 20484 ]
  16        10.0.0.217/32     TI-LFA (1)                 -            [ 20217 ]
  17        10.0.0.66/32      TI-LFA (1)                 -            [ 20066 ]
  18        10.0.0.156/32     20.30.32.30                Ethernet1    [ 20156 ]
                              20.32.175.175              Ethernet5    [ 20156 ]

```

## show isis segment-routing prefix-segments

```text

System ID: Arista-PE32-Q2C-32			Instance: 'IGP'
SR supported Data-plane: MPLS			SR Router ID: 10.0.0.32

Node: 16     Proxy-Node: 0      Prefix: 0       Total Segments: 16

Flag Descriptions: R: Re-advertised, N: Node Segment, P: no-PHP
                   E: Explicit-NULL, V: Value, L: Local
Segment status codes: * - Self originated Prefix, L1 - level 1, L2 - level 2, ! - SR-unreachable,
                      # - Some IS-IS next-hops are SR-unreachable
   Prefix                      SID   Label Type       Flags                        System ID       Level Protection  Algorithm   
   ------------------------- ----- ------- ---------- ---------------------------- --------------- ----- ----------- -------------
   10.0.0.30/32                 30   20030 Node       R:0 N:1 P:0 E:0 V:0 L:0      Arista-Spine3-Q2A-30 L2    node        SPF         
*  10.0.0.32/32                 32   20032 Node       R:0 N:1 P:0 E:0 V:0 L:0      Arista-PE32-Q2C-32 L2    unprotected SPF         
   10.0.0.53/32                 53   20053 Node       R:0 N:1 P:1 E:1 V:0 L:0      Arrcus-53       L2    node        SPF         
   10.0.0.66/32                 66   20066 Node       R:0 N:1 P:0 E:0 V:0 L:0      Ciena-8140-66   L2    node        SPF         
   10.0.0.72/32                 72   20072 Node       R:0 N:1 P:0 E:0 V:0 L:0      Ciena-5134-72   L2    node        SPF         
   10.0.0.84/32                 84   20084 Node       R:0 N:1 P:1 E:0 V:0 L:0      Ericsson_84_R6678 L2    node        SPF         
   10.0.0.120/32               120   20120 Node       R:0 N:1 P:0 E:0 V:0 L:0      H3C_M1A_120     L2    node        SPF         
   10.0.0.124/32               124    2124 Node       R:0 N:1 P:1 E:0 V:0 L:0      0000.0000.0124  L2    node        SPF         
   10.0.0.128/32               128   20128 Node       R:0 N:1 P:0 E:0 V:0 L:0      0000.0000.0128  L2    node        SPF         
   10.0.0.156/32               156   20156 Node       R:0 N:1 P:0 E:0 V:0 L:0      Juniper-156-PTX10002-36QDD L2    unprotected SPF         
   10.0.0.175/32               175   20175 Node       R:0 N:1 P:0 E:0 V:0 L:0      Juniper-175-ACX7100-48L L2    node        SPF         
   10.0.0.179/32               179   20179 Node       R:0 N:1 P:0 E:0 V:0 L:0      Juniper-179-ACX7024 L2    node        SPF         
   10.0.0.184/32               484   20484 Node       R:0 N:1 P:0 E:0 V:0 L:0      Keysight-184    L2    node        SPF         
   10.0.0.214/32               214   20214 Node       R:0 N:1 P:1 E:0 V:0 L:0      Nokia-SXR-214   L2    node        SPF         
   10.0.0.217/32               217   20217 Node       R:0 N:1 P:1 E:0 V:0 L:0      Nokia-SR1-217   L2    node        SPF         
   10.0.0.221/32              1221  721221 Node       R:0 N:1 P:0 E:0 V:0 L:0      221             L2    node        SPF         
```

## show traffic-engineering segment-routing policy

```text
Endpoint 10.0.0.66 Color 100, Counters: 0 packets, 0 bytes
	Path group: State: active (for 00:01:34), modified: 15:33:20 ago
		Protocol: Static
		Endpoint provisioning: Static
		Originator: 0.0.0.0(AS0)
		Discriminator: 32769
		Preference: 2
		IGP metric: 0 (static)
		Binding SID: 1004066
		Path computation: Configured
		Explicit null label policy: IPv6 (system default)
		Segment List: State: Valid, SBFD State: Up, ID: 10, Counters: 0 packets, 0 bytes
		Protected: Yes
			Label Stack: [20030 20066], Weight: 1
			Resolved Label Stack: [20066], Next hop: 20.30.32.30, Interface: Ethernet1
			Backup Resolved Label Stack: [20030 20066], Next hop: 20.32.175.175, Interface: Ethernet5
	Path group: State: valid, modified: 15:33:20 ago
		Protocol: Static
		Endpoint provisioning: Static
		Originator: 0.0.0.0(AS0)
		Discriminator: 32770
		Preference: 1
		Binding SID: 1004066
		Path computation: Configured
		Explicit null label policy: IPv6 (system default)
		Segment List: State: Valid, SBFD State: Up, ID: 4, Counters: 0 packets, 0 bytes (counter not in use)
		Protected: Yes
			Label Stack: [20175 20066], Weight: 1
			Resolved Label Stack: [20066], Next hop: 20.32.175.175, Interface: Ethernet5
			Backup Resolved Label Stack: [20124 2175 20066], Next hop: 20.30.32.30, Interface: Ethernet1
Endpoint 10.0.0.72 Color 100, Counters: 0 packets, 0 bytes
	Path group: State: active (for 00:01:34), modified: 15:33:20 ago
		Protocol: Static
		Endpoint provisioning: Static
		Originator: 0.0.0.0(AS0)
		Discriminator: 32769
		Preference: 2
		IGP metric: 0 (static)
		Binding SID: 1004072
		Path computation: Configured
		Explicit null label policy: IPv6 (system default)
		Segment List: State: Valid, SBFD State: Up, ID: 1, Counters: 0 packets, 0 bytes
		Protected: Yes
			Label Stack: [20030 20072], Weight: 1
			Resolved Label Stack: [20072], Next hop: 20.30.32.30, Interface: Ethernet1
			Backup Resolved Label Stack: [20030 20072], Next hop: 20.32.175.175, Interface: Ethernet5
	Path group: State: valid, modified: 15:33:20 ago
		Protocol: Static
		Endpoint provisioning: Static
		Originator: 0.0.0.0(AS0)
		Discriminator: 32770
		Preference: 1
		Binding SID: 1004072
		Path computation: Configured
		Explicit null label policy: IPv6 (system default)
		Segment List: State: Valid, SBFD State: Up, ID: 15, Counters: 0 packets, 0 bytes (counter not in use)
		Protected: Yes
			Label Stack: [20175 20072], Weight: 1
			Resolved Label Stack: [20072], Next hop: 20.32.175.175, Interface: Ethernet5
			Backup Resolved Label Stack: [20124 2175 20072], Next hop: 20.30.32.30, Interface: Ethernet1
Endpoint 10.0.0.120 Color 100, Counters: 0 packets, 0 bytes
	Path group: State: active (for 00:01:34), modified: 15:32:12 ago
		Protocol: Static
		Endpoint provisioning: Static
		Originator: 0.0.0.0(AS0)
		Discriminator: 32769
		Preference: 2
		IGP metric: 0 (static)
		Binding SID: 1004120
		Path computation: Configured
		Explicit null label policy: IPv6 (system default)
		Segment List: State: Valid, SBFD State: Up, ID: 6, Counters: 0 packets, 0 bytes
		Protected: Yes
			Label Stack: [20030 20120], Weight: 1
			Resolved Label Stack: [20120], Next hop: 20.30.32.30, Interface: Ethernet1
			Backup Resolved Label Stack: [20030 20120], Next hop: 20.32.175.175, Interface: Ethernet5
	Path group: State: valid, modified: 15:32:12 ago
		Protocol: Static
		Endpoint provisioning: Static
		Originator: 0.0.0.0(AS0)
		Discriminator: 32770
		Preference: 1
		Binding SID: 1004120
		Path computation: Configured
		Explicit null label policy: IPv6 (system default)
		Segment List: State: Valid, SBFD State: Up, ID: 11, Counters: 0 packets, 0 bytes (counter not in use)
		Protected: Yes
			Label Stack: [20175 20120], Weight: 1
			Resolved Label Stack: [20120], Next hop: 20.32.175.175, Interface: Ethernet5
			Backup Resolved Label Stack: [20124 2175 20120], Next hop: 20.30.32.30, Interface: Ethernet1
Endpoint 10.0.0.124 Color 100, Counters: 0 packets, 0 bytes
	Path group: State: active (for 00:01:34), modified: 15:33:20 ago
		Protocol: Static
		Endpoint provisioning: Static
		Originator: 0.0.0.0(AS0)
		Discriminator: 32770
		Preference: 2
		IGP metric: 0 (static)
		Binding SID: 1004124
		Path computation: Configured
		Explicit null label policy: IPv6 (system default)
		Segment List: State: Valid, SBFD State: Up, ID: 5, Counters: 0 packets, 0 bytes
		Protected: Yes
			Label Stack: [20030 20124], Weight: 1
			Resolved Label Stack: [20124], Next hop: 20.30.32.30, Interface: Ethernet1
			Backup Resolved Label Stack: [20030 20124], Next hop: 20.32.175.175, Interface: Ethernet5
	Path group: State: valid, modified: 15:33:20 ago
		Protocol: Static
		Endpoint provisioning: Static
		Originator: 0.0.0.0(AS0)
		Discriminator: 32769
		Preference: 1
		Binding SID: 1004124
		Path computation: Configured
		Explicit null label policy: IPv6 (system default)
		Segment List: State: Valid, SBFD State: Up, ID: 8, Counters: 0 packets, 0 bytes (counter not in use)
		Protected: Yes
			Label Stack: [20175 20124], Weight: 1
			Resolved Label Stack: [20124], Next hop: 20.32.175.175, Interface: Ethernet5
			Backup Resolved Label Stack: [20124 2175 20124], Next hop: 20.30.32.30, Interface: Ethernet1
Endpoint 10.0.0.128 Color 100, Counters: 0 packets, 0 bytes
	Path group: State: active (for 00:01:34), modified: 15:33:20 ago
		Protocol: Static
		Endpoint provisioning: Static
		Originator: 0.0.0.0(AS0)
		Discriminator: 32770
		Preference: 2
		IGP metric: 0 (static)
		Binding SID: 1004128
		Path computation: Configured
		Explicit null label policy: IPv6 (system default)
		Segment List: State: Valid, SBFD State: Up, ID: 16, Counters: 0 packets, 0 bytes
		Protected: Yes
			Label Stack: [20030 20128], Weight: 1
			Resolved Label Stack: [20128], Next hop: 20.30.32.30, Interface: Ethernet1
			Backup Resolved Label Stack: [20030 20128], Next hop: 20.32.175.175, Interface: Ethernet5
	Path group: State: valid, modified: 15:33:20 ago
		Protocol: Static
		Endpoint provisioning: Static
		Originator: 0.0.0.0(AS0)
		Discriminator: 32769
		Preference: 1
		Binding SID: 1004128
		Path computation: Configured
		Explicit null label policy: IPv6 (system default)
		Segment List: State: Valid, SBFD State: Up, ID: 2, Counters: 0 packets, 0 bytes (counter not in use)
		Protected: Yes
			Label Stack: [20175 20128], Weight: 1
			Resolved Label Stack: [20128], Next hop: 20.32.175.175, Interface: Ethernet5
			Backup Resolved Label Stack: [20124 2175 20128], Next hop: 20.30.32.30, Interface: Ethernet1
Endpoint 10.0.0.156 Color 100, Counters: 0 packets, 0 bytes
	Path group: State: active (for 00:01:12), modified: 00:01:12 ago
		Protocol: Static
		Endpoint provisioning: Static
		Originator: 0.0.0.0(AS0)
		Discriminator: 32770
		Preference: 2
		IGP metric: 0 (static)
		Binding SID: 1004156
		Path computation: Configured
		Explicit null label policy: IPv6 (system default)
		Segment List: State: Valid, SBFD State: Up, ID: 18, Counters: 0 packets, 0 bytes
		Protected: Yes
			Label Stack: [20030 20156], Weight: 1
			Resolved Label Stack: [20156], Next hop: 20.30.32.30, Interface: Ethernet1
			Backup Resolved Label Stack: [20030 20156], Next hop: 20.32.175.175, Interface: Ethernet5
	Path group: State: valid, modified: 00:01:12 ago
		Protocol: Static
		Endpoint provisioning: Static
		Originator: 0.0.0.0(AS0)
		Discriminator: 32769
		Preference: 1
		Binding SID: 1004156
		Path computation: Configured
		Explicit null label policy: IPv6 (system default)
		Segment List: State: Valid, SBFD State: Up, ID: 17, Counters: 0 packets, 0 bytes (counter not in use)
		Protected: Yes
			Label Stack: [20175 20156], Weight: 1
			Resolved Label Stack: [20156], Next hop: 20.32.175.175, Interface: Ethernet5
			Backup Resolved Label Stack: [20124 2175 20156], Next hop: 20.30.32.30, Interface: Ethernet1
Endpoint 10.0.0.179 Color 100, Counters: 0 packets, 0 bytes
	Path group: State: active (for 00:01:34), modified: 15:33:20 ago
		Protocol: Static
		Endpoint provisioning: Static
		Originator: 0.0.0.0(AS0)
		Discriminator: 32770
		Preference: 2
		IGP metric: 0 (static)
		Binding SID: 1004179
		Path computation: Configured
		Explicit null label policy: IPv6 (system default)
		Segment List: State: Valid, SBFD State: Up, ID: 7, Counters: 0 packets, 0 bytes
		Protected: Yes
			Label Stack: [20030 20179], Weight: 1
			Resolved Label Stack: [20179], Next hop: 20.30.32.30, Interface: Ethernet1
			Backup Resolved Label Stack: [20030 20179], Next hop: 20.32.175.175, Interface: Ethernet5
	Path group: State: valid, modified: 15:33:20 ago
		Protocol: Static
		Endpoint provisioning: Static
		Originator: 0.0.0.0(AS0)
		Discriminator: 32769
		Preference: 1
		Binding SID: 1004179
		Path computation: Configured
		Explicit null label policy: IPv6 (system default)
		Segment List: State: Valid, SBFD State: Up, ID: 12, Counters: 0 packets, 0 bytes (counter not in use)
		Protected: Yes
			Label Stack: [20175 20179], Weight: 1
			Resolved Label Stack: [20179], Next hop: 20.32.175.175, Interface: Ethernet5
			Backup Resolved Label Stack: [20124 2175 20179], Next hop: 20.30.32.30, Interface: Ethernet1
Endpoint 10.0.0.217 Color 100, Counters: 451177380 packets, 45117738000 bytes
	Path group: State: active (for 00:01:34), modified: 15:33:20 ago
		Protocol: Static
		Endpoint provisioning: Static
		Originator: 0.0.0.0(AS0)
		Discriminator: 32769
		Preference: 2
		IGP metric: 0 (static)
		Binding SID: 1004217
		Path computation: Configured
		Explicit null label policy: IPv6 (system default)
		Segment List: State: Valid, SBFD State: Up, ID: 13, Counters: 55419130 packets, 5541913000 bytes
		Protected: Yes
			Label Stack: [20030 20217], Weight: 1
			Resolved Label Stack: [20217], Next hop: 20.30.32.30, Interface: Ethernet1
			Backup Resolved Label Stack: [20030 20217], Next hop: 20.32.175.175, Interface: Ethernet5
	Path group: State: valid, modified: 15:33:20 ago
		Protocol: Static
		Endpoint provisioning: Static
		Originator: 0.0.0.0(AS0)
		Discriminator: 32770
		Preference: 1
		Binding SID: 1004217
		Path computation: Configured
		Explicit null label policy: IPv6 (system default)
		Segment List: State: Valid, SBFD State: Up, ID: 9, Counters: 395758250 packets, 39575825000 bytes (counter not in use)
		Protected: Yes
			Label Stack: [20175 20217], Weight: 1
			Resolved Label Stack: [20217], Next hop: 20.32.175.175, Interface: Ethernet5
			Backup Resolved Label Stack: [20124 2175 20217], Next hop: 20.30.32.30, Interface: Ethernet1
Endpoint 10.0.0.221 Color 100, Counters: 0 packets, 0 bytes
	Path group: State: active (for 00:01:33), modified: 15:33:20 ago
		Protocol: Static
		Endpoint provisioning: Static
		Originator: 0.0.0.0(AS0)
		Discriminator: 32770
		Preference: 2
		IGP metric: 0 (static)
		Binding SID: 1004221
		Path computation: Configured
		Explicit null label policy: IPv6 (system default)
		Segment List: State: Valid, SBFD State: Up, ID: 14, Counters: 0 packets, 0 bytes
		Protected: Yes
			Label Stack: [20030 21221], Weight: 1
			Resolved Label Stack: [21221], Next hop: 20.30.32.30, Interface: Ethernet1
			Backup Resolved Label Stack: [20030 21221], Next hop: 20.32.175.175, Interface: Ethernet5
	Path group: State: valid, modified: 15:33:21 ago
		Protocol: Static
		Endpoint provisioning: Static
		Originator: 0.0.0.0(AS0)
		Discriminator: 32769
		Preference: 1
		Binding SID: 1004221
		Path computation: Configured
		Explicit null label policy: IPv6 (system default)
		Segment List: State: Valid, SBFD State: Up, ID: 3, Counters: 0 packets, 0 bytes (counter not in use)
		Protected: Yes
			Label Stack: [20175 21221], Weight: 1
			Resolved Label Stack: [21221], Next hop: 20.32.175.175, Interface: Ethernet5
			Backup Resolved Label Stack: [20124 2175 21221], Next hop: 20.30.32.30, Interface: Ethernet1
```

## show bfd peers detail

```text
VRF name: default
-----------------
Peer Addr 0.8.0.0, Tunnel ID 140737488355337(SR), Segment list ID 9, Type SBFD(initiator), State Up
VRF default, LAddr 10.0.0.32, LD/RD 764890487/524288
Session state is Up and not using echo function
Hardware Acceleration: Async Off, Echo Off
Last Up 02/18/25 17:10:06.742
Last Down NA
Last Diag: No Diagnostic
Authentication mode: None
Shared-secret profile: None
TxInt: 100 ms, RxInt: 100 ms, Multiplier: 3
Received RxInt: 3 ms, Received Multiplier: 3
Rx Count: 605896, Rx Interval (ms) min/max/avg: 75/108/92 last: -598 ms ago
Tx Count: 605896, Tx Interval (ms) min/max/avg: 80/108/92 last: -598 ms ago
Detect Time: 300 ms
Sched Delay: 1*TxInt: 534404, 2*TxInt: 71491, 3*TxInt: 0, GT 3*TxInt: 0
RTT (us) min/max/avg: 54/4110/110 last: 155 us
Registered protocols: sr-te policy
Uptime: 15:48:13.36
Tunnel Info:  MPLS label stack: [20175 20217]
              MPLS EXP: 7                    
              IP DSCP: 192                   
Last packet:  Version: 1           - Diagnostic: 0         
              State bit: Up        - Demand bit: 0         
              Poll bit: 0          - Final bit: 0          
              Multiplier: 3        - Length: 30            
              My Discr.: 524288    - Your Discr.: 764890487
              Min tx interval: 100 - Min rx interval: 3    
              Min Echo interval: 0                         

Peer Addr 0.8.0.0, Tunnel ID 140737488355341(SR), Segment list ID 13, Type SBFD(initiator), State Up
VRF default, LAddr 10.0.0.32, LD/RD 3200281249/524288
Session state is Up and not using echo function
Hardware Acceleration: Async Off, Echo Off
Last Up 02/19/25 08:56:45.561
Last Down 02/19/25 08:48:41.886
Last Diag: No Diagnostic
Authentication mode: None
Shared-secret profile: None
TxInt: 100 ms, RxInt: 100 ms, Multiplier: 3
Received RxInt: 3 ms, Received Multiplier: 3
Rx Count: 1024, Rx Interval (ms) min/max/avg: 79/108/92 last: -550 ms ago
Tx Count: 1023, Tx Interval (ms) min/max/avg: 80/108/92 last: -550 ms ago
Detect Time: 300 ms
Sched Delay: 1*TxInt: 915, 2*TxInt: 107, 3*TxInt: 0, GT 3*TxInt: 0
RTT (us) min/max/avg: 56/276/120 last: 116 us
Registered protocols: sr-te policy
Uptime: 01:34.55
Tunnel Info:  MPLS label stack: [20030 20217]
              MPLS EXP: 7                    
              IP DSCP: 192                   
Last packet:  Version: 1           - Diagnostic: 0          
              State bit: Up        - Demand bit: 0          
              Poll bit: 0          - Final bit: 0           
              Multiplier: 3        - Length: 30             
              My Discr.: 524288    - Your Discr.: 3200281249
              Min tx interval: 100 - Min rx interval: 3     
              Min Echo interval: 0                          

Peer Addr 10.0.0.124, Tunnel ID 140737488355333(SR), Segment list ID 5, Type SBFD(initiator), State Up
VRF default, LAddr 10.0.0.32, LD/RD 2626331766/167772284
Session state is Up and not using echo function
Hardware Acceleration: Async Off, Echo Off
Last Up 02/19/25 08:56:45.785
Last Down 02/19/25 08:48:41.945
Last Diag: No Diagnostic
Authentication mode: None
Shared-secret profile: None
TxInt: 100 ms, RxInt: 100 ms, Multiplier: 3
Received RxInt: 0 ms, Received Multiplier: 3
Rx Count: 1026, Rx Interval (ms) min/max/avg: 76/108/91 last: -562 ms ago
Tx Count: 1024, Tx Interval (ms) min/max/avg: 80/108/91 last: -562 ms ago
Detect Time: 300 ms
Sched Delay: 1*TxInt: 921, 2*TxInt: 102, 3*TxInt: 0, GT 3*TxInt: 0
RTT (us) min/max/avg: 80/276/136 last: 141 us
Registered protocols: sr-te policy
Uptime: 01:34.33
Tunnel Info:  MPLS label stack: [20030 20124]
              MPLS EXP: 7                    
              IP DSCP: 192                   
Last packet:  Version: 1           - Diagnostic: 0          
              State bit: Up        - Demand bit: 0          
              Poll bit: 0          - Final bit: 0           
              Multiplier: 3        - Length: 30             
              My Discr.: 167772284 - Your Discr.: 2626331766
              Min tx interval: 100 - Min rx interval: 0     
              Min Echo interval: 0                          

Peer Addr 10.0.0.124, Tunnel ID 140737488355336(SR), Segment list ID 8, Type SBFD(initiator), State Up
VRF default, LAddr 10.0.0.32, LD/RD 252341208/167772284
Session state is Up and not using echo function
Hardware Acceleration: Async Off, Echo Off
Last Up 02/18/25 17:10:06.743
Last Down NA
Last Diag: No Diagnostic
Authentication mode: None
Shared-secret profile: None
TxInt: 100 ms, RxInt: 100 ms, Multiplier: 3
Received RxInt: 0 ms, Received Multiplier: 3
Rx Count: 605754, Rx Interval (ms) min/max/avg: 75/108/92 last: -570 ms ago
Tx Count: 605753, Tx Interval (ms) min/max/avg: 80/108/92 last: -570 ms ago
Detect Time: 300 ms
Sched Delay: 1*TxInt: 533706, 2*TxInt: 72046, 3*TxInt: 0, GT 3*TxInt: 0
RTT (us) min/max/avg: 83/819/133 last: 113 us
Registered protocols: sr-te policy
Uptime: 15:48:13.37
Tunnel Info:  MPLS label stack: [20175 20124]
              MPLS EXP: 7                    
              IP DSCP: 192                   
Last packet:  Version: 1           - Diagnostic: 0         
              State bit: Up        - Demand bit: 0         
              Poll bit: 0          - Final bit: 0          
              Multiplier: 3        - Length: 30            
              My Discr.: 167772284 - Your Discr.: 252341208
              Min tx interval: 100 - Min rx interval: 0    
              Min Echo interval: 0                         

Peer Addr 10.0.0.128, Tunnel ID 140737488355330(SR), Segment list ID 2, Type SBFD(initiator), State Up
VRF default, LAddr 10.0.0.32, LD/RD 677506679/167772288
Session state is Up and not using echo function
Hardware Acceleration: Async Off, Echo Off
Last Up 02/18/25 17:10:06.737
Last Down NA
Last Diag: No Diagnostic
Authentication mode: None
Shared-secret profile: None
TxInt: 100 ms, RxInt: 100 ms, Multiplier: 3
Received RxInt: 0 ms, Received Multiplier: 3
Rx Count: 606003, Rx Interval (ms) min/max/avg: 75/108/92 last: -586 ms ago
Tx Count: 606002, Tx Interval (ms) min/max/avg: 80/108/92 last: -586 ms ago
Detect Time: 300 ms
Sched Delay: 1*TxInt: 534594, 2*TxInt: 71407, 3*TxInt: 0, GT 3*TxInt: 0
RTT (us) min/max/avg: 52/1671/108 last: 138 us
Registered protocols: sr-te policy
Uptime: 15:48:13.38
Tunnel Info:  MPLS label stack: [20175 20128]
              MPLS EXP: 7                    
              IP DSCP: 192                   
Last packet:  Version: 1           - Diagnostic: 0         
              State bit: Up        - Demand bit: 0         
              Poll bit: 0          - Final bit: 0          
              Multiplier: 3        - Length: 30            
              My Discr.: 167772288 - Your Discr.: 677506679
              Min tx interval: 100 - Min rx interval: 0    
              Min Echo interval: 0                         

Peer Addr 10.0.0.128, Tunnel ID 140737488355344(SR), Segment list ID 16, Type SBFD(initiator), State Up
VRF default, LAddr 10.0.0.32, LD/RD 2025507954/167772288
Session state is Up and not using echo function
Hardware Acceleration: Async Off, Echo Off
Last Up 02/19/25 08:56:45.753
Last Down 02/19/25 08:48:41.886
Last Diag: No Diagnostic
Authentication mode: None
Shared-secret profile: None
TxInt: 100 ms, RxInt: 100 ms, Multiplier: 3
Received RxInt: 0 ms, Received Multiplier: 3
Rx Count: 1022, Rx Interval (ms) min/max/avg: 76/108/92 last: -578 ms ago
Tx Count: 1020, Tx Interval (ms) min/max/avg: 80/108/92 last: -578 ms ago
Detect Time: 300 ms
Sched Delay: 1*TxInt: 899, 2*TxInt: 120, 3*TxInt: 0, GT 3*TxInt: 0
RTT (us) min/max/avg: 55/269/115 last: 73 us
Registered protocols: sr-te policy
Uptime: 01:34.36
Tunnel Info:  MPLS label stack: [20030 20128]
              MPLS EXP: 7                    
              IP DSCP: 192                   
Last packet:  Version: 1           - Diagnostic: 0          
              State bit: Up        - Demand bit: 0          
              Poll bit: 0          - Final bit: 0           
              Multiplier: 3        - Length: 30             
              My Discr.: 167772288 - Your Discr.: 2025507954
              Min tx interval: 100 - Min rx interval: 0     
              Min Echo interval: 0                          

Peer Addr 10.0.0.156, Tunnel ID 140737488355345(SR), Segment list ID 17, Type SBFD(initiator), State Up
VRF default, LAddr 10.0.0.32, LD/RD 238718245/167772316
Session state is Up and not using echo function
Hardware Acceleration: Async Off, Echo Off
Last Up 02/19/25 08:29:37.757
Last Down 02/19/25 08:18:35.641
Last Diag: No Diagnostic
Authentication mode: None
Shared-secret profile: None
TxInt: 100 ms, RxInt: 100 ms, Multiplier: 3
Received RxInt: 0 ms, Received Multiplier: 3
Rx Count: 18570, Rx Interval (ms) min/max/avg: 75/108/92 last: -578 ms ago
Tx Count: 18569, Tx Interval (ms) min/max/avg: 80/108/92 last: -578 ms ago
Detect Time: 300 ms
Sched Delay: 1*TxInt: 16131, 2*TxInt: 2437, 3*TxInt: 0, GT 3*TxInt: 0
RTT (us) min/max/avg: 90/955/200 last: 113 us
Registered protocols: sr-te policy
Uptime: 28:42.36
Tunnel Info:  MPLS label stack: [20175 20156]
              MPLS EXP: 7                    
              IP DSCP: 192                   
Last packet:  Version: 1           - Diagnostic: 0         
              State bit: Up        - Demand bit: 0         
              Poll bit: 0          - Final bit: 0          
              Multiplier: 3        - Length: 30            
              My Discr.: 167772316 - Your Discr.: 238718245
              Min tx interval: 100 - Min rx interval: 0    
              Min Echo interval: 0                         

Peer Addr 10.0.0.156, Tunnel ID 140737488355346(SR), Segment list ID 18, Type SBFD(initiator), State Up
VRF default, LAddr 10.0.0.32, LD/RD 1046734703/167772316
Session state is Up and not using echo function
Hardware Acceleration: Async Off, Echo Off
Last Up 02/19/25 08:56:45.501
Last Down 02/19/25 08:48:41.977
Last Diag: No Diagnostic
Authentication mode: None
Shared-secret profile: None
TxInt: 100 ms, RxInt: 100 ms, Multiplier: 3
Received RxInt: 0 ms, Received Multiplier: 3
Rx Count: 1027, Rx Interval (ms) min/max/avg: 76/108/92 last: -562 ms ago
Tx Count: 1026, Tx Interval (ms) min/max/avg: 80/108/92 last: -562 ms ago
Detect Time: 300 ms
Sched Delay: 1*TxInt: 908, 2*TxInt: 117, 3*TxInt: 0, GT 3*TxInt: 0
RTT (us) min/max/avg: 93/322/154 last: 104 us
Registered protocols: sr-te policy
Uptime: 01:34.62
Tunnel Info:  MPLS label stack: [20030 20156]
              MPLS EXP: 7                    
              IP DSCP: 192                   
Last packet:  Version: 1           - Diagnostic: 0          
              State bit: Up        - Demand bit: 0          
              Poll bit: 0          - Final bit: 0           
              Multiplier: 3        - Length: 30             
              My Discr.: 167772316 - Your Discr.: 1046734703
              Min tx interval: 100 - Min rx interval: 0     
              Min Echo interval: 0                          

Peer Addr 10.0.0.179, Tunnel ID 140737488355335(SR), Segment list ID 7, Type SBFD(initiator), State Up
VRF default, LAddr 10.0.0.32, LD/RD 1270332993/167772339
Session state is Up and not using echo function
Hardware Acceleration: Async Off, Echo Off
Last Up 02/19/25 08:56:45.562
Last Down 02/19/25 08:48:41.920
Last Diag: No Diagnostic
Authentication mode: None
Shared-secret profile: None
TxInt: 100 ms, RxInt: 100 ms, Multiplier: 3
Received RxInt: 0 ms, Received Multiplier: 3
Rx Count: 1025, Rx Interval (ms) min/max/avg: 75/109/92 last: -530 ms ago
Tx Count: 1024, Tx Interval (ms) min/max/avg: 80/108/92 last: -530 ms ago
Detect Time: 300 ms
Sched Delay: 1*TxInt: 913, 2*TxInt: 110, 3*TxInt: 0, GT 3*TxInt: 0
RTT (us) min/max/avg: 376/14078/692 last: 448 us
Registered protocols: sr-te policy
Uptime: 01:34.56
Tunnel Info:  MPLS label stack: [20030 20179]
              MPLS EXP: 7                    
              IP DSCP: 192                   
Last packet:  Version: 1           - Diagnostic: 0          
              State bit: Up        - Demand bit: 0          
              Poll bit: 0          - Final bit: 0           
              Multiplier: 3        - Length: 30             
              My Discr.: 167772339 - Your Discr.: 1270332993
              Min tx interval: 100 - Min rx interval: 0     
              Min Echo interval: 0                          

Peer Addr 10.0.0.179, Tunnel ID 140737488355340(SR), Segment list ID 12, Type SBFD(initiator), State Up
VRF default, LAddr 10.0.0.32, LD/RD 35964480/167772339
Session state is Up and not using echo function
Hardware Acceleration: Async Off, Echo Off
Last Up 02/19/25 02:47:32.674
Last Down 02/19/25 02:47:32.601
Last Diag: No Diagnostic
Authentication mode: None
Shared-secret profile: None
TxInt: 100 ms, RxInt: 100 ms, Multiplier: 3
Received RxInt: 0 ms, Received Multiplier: 3
Rx Count: 240533, Rx Interval (ms) min/max/avg: 16/179/92 last: -510 ms ago
Tx Count: 240533, Tx Interval (ms) min/max/avg: 80/108/92 last: -510 ms ago
Detect Time: 300 ms
Sched Delay: 1*TxInt: 211450, 2*TxInt: 29082, 3*TxInt: 0, GT 3*TxInt: 0
RTT (us) min/max/avg: 343/72441/705 last: 476 us
Registered protocols: sr-te policy
Uptime: 06:10:47.45
Tunnel Info:  MPLS label stack: [20175 20179]
              MPLS EXP: 7                    
              IP DSCP: 192                   
Last packet:  Version: 1           - Diagnostic: 0        
              State bit: Up        - Demand bit: 0        
              Poll bit: 0          - Final bit: 0         
              Multiplier: 3        - Length: 30           
              My Discr.: 167772339 - Your Discr.: 35964480
              Min tx interval: 100 - Min rx interval: 0   
              Min Echo interval: 0                        

Peer Addr 255.255.255.255, Tunnel ID 140737488355329(SR), Segment list ID 1, Type SBFD(initiator), State Up
VRF default, LAddr 10.0.0.32, LD/RD 1863129822/1863129822
Session state is Up and not using echo function
Hardware Acceleration: Async Off, Echo Off
Last Up 02/19/25 08:56:45.561
Last Down 02/19/25 08:48:41.917
Last Diag: No Diagnostic
Authentication mode: None
Shared-secret profile: None
TxInt: 100 ms, RxInt: 100 ms, Multiplier: 3
Received RxInt: 0 ms, Received Multiplier: 3
Rx Count: 1026, Rx Interval (ms) min/max/avg: 76/108/92 last: -590 ms ago
Tx Count: 1027, Tx Interval (ms) min/max/avg: 80/108/92 last: -590 ms ago
Detect Time: 300 ms
Sched Delay: 1*TxInt: 910, 2*TxInt: 116, 3*TxInt: 0, GT 3*TxInt: 0
RTT (us) min/max/avg: 45/261/109 last: 115 us
Registered protocols: sr-te policy
Uptime: 01:34.56
Tunnel Info:  MPLS label stack: [20030 20072]
              MPLS EXP: 7                    
              IP DSCP: 192                   
Last packet:  Version: 1            - Diagnostic: 0          
              State bit: Up         - Demand bit: 0          
              Poll bit: 0           - Final bit: 0           
              Multiplier: 3         - Length: 30             
              My Discr.: 1863129822 - Your Discr.: 1863129822
              Min tx interval: 100  - Min rx interval: 0     
              Min Echo interval: 0                           

Peer Addr 255.255.255.255, Tunnel ID 140737488355331(SR), Segment list ID 3, Type SBFD(initiator), State Up
VRF default, LAddr 10.0.0.32, LD/RD 1584396073/1584396073
Session state is Up and not using echo function
Hardware Acceleration: Async Off, Echo Off
Last Up 02/18/25 17:10:06.737
Last Down NA
Last Diag: No Diagnostic
Authentication mode: None
Shared-secret profile: None
TxInt: 100 ms, RxInt: 100 ms, Multiplier: 3
Received RxInt: 0 ms, Received Multiplier: 3
Rx Count: 605901, Rx Interval (ms) min/max/avg: 75/108/92 last: -598 ms ago
Tx Count: 605901, Tx Interval (ms) min/max/avg: 80/108/92 last: -598 ms ago
Detect Time: 300 ms
Sched Delay: 1*TxInt: 534319, 2*TxInt: 71581, 3*TxInt: 0, GT 3*TxInt: 0
RTT (us) min/max/avg: 40/782/100 last: 119 us
Registered protocols: sr-te policy
Uptime: 15:48:13.39
Tunnel Info:  MPLS label stack: [20175 21221]
              MPLS EXP: 7                    
              IP DSCP: 192                   
Last packet:  Version: 1            - Diagnostic: 0          
              State bit: Up         - Demand bit: 0          
              Poll bit: 0           - Final bit: 0           
              Multiplier: 3         - Length: 30             
              My Discr.: 1584396073 - Your Discr.: 1584396073
              Min tx interval: 100  - Min rx interval: 0     
              Min Echo interval: 0                           

Peer Addr 255.255.255.255, Tunnel ID 140737488355332(SR), Segment list ID 4, Type SBFD(initiator), State Up
VRF default, LAddr 10.0.0.32, LD/RD 1600151469/1600151469
Session state is Up and not using echo function
Hardware Acceleration: Async Off, Echo Off
Last Up 02/18/25 17:21:42.977
Last Down NA
Last Diag: No Diagnostic
Authentication mode: None
Shared-secret profile: None
TxInt: 100 ms, RxInt: 100 ms, Multiplier: 3
Received RxInt: 0 ms, Received Multiplier: 3
Rx Count: 605910, Rx Interval (ms) min/max/avg: 75/108/92 last: -598 ms ago
Tx Count: 605910, Tx Interval (ms) min/max/avg: 80/108/92 last: -598 ms ago
Detect Time: 300 ms
Sched Delay: 1*TxInt: 534029, 2*TxInt: 71880, 3*TxInt: 0, GT 3*TxInt: 0
RTT (us) min/max/avg: 38/1660/100 last: 104 us
Registered protocols: sr-te policy
Uptime: 15:36:37.15
Tunnel Info:  MPLS label stack: [20175 20066]
              MPLS EXP: 7                    
              IP DSCP: 192                   
Last packet:  Version: 1            - Diagnostic: 0          
              State bit: Up         - Demand bit: 0          
              Poll bit: 0           - Final bit: 0           
              Multiplier: 3         - Length: 30             
              My Discr.: 1600151469 - Your Discr.: 1600151469
              Min tx interval: 100  - Min rx interval: 0     
              Min Echo interval: 0                           

Peer Addr 255.255.255.255, Tunnel ID 140737488355334(SR), Segment list ID 6, Type SBFD(initiator), State Up
VRF default, LAddr 10.0.0.32, LD/RD 4168450569/4168450569
Session state is Up and not using echo function
Hardware Acceleration: Async Off, Echo Off
Last Up 02/19/25 08:56:45.337
Last Down 02/19/25 08:48:41.885
Last Diag: No Diagnostic
Authentication mode: None
Shared-secret profile: None
TxInt: 100 ms, RxInt: 100 ms, Multiplier: 3
Received RxInt: 0 ms, Received Multiplier: 3
Rx Count: 1027, Rx Interval (ms) min/max/avg: 76/108/92 last: -510 ms ago
Tx Count: 1028, Tx Interval (ms) min/max/avg: 80/108/92 last: -510 ms ago
Detect Time: 300 ms
Sched Delay: 1*TxInt: 924, 2*TxInt: 103, 3*TxInt: 0, GT 3*TxInt: 0
RTT (us) min/max/avg: 69/320/128 last: 166 us
Registered protocols: sr-te policy
Uptime: 01:34.79
Tunnel Info:  MPLS label stack: [20030 20120]
              MPLS EXP: 7                    
              IP DSCP: 192                   
Last packet:  Version: 1            - Diagnostic: 0          
              State bit: Up         - Demand bit: 0          
              Poll bit: 0           - Final bit: 0           
              Multiplier: 3         - Length: 30             
              My Discr.: 4168450569 - Your Discr.: 4168450569
              Min tx interval: 100  - Min rx interval: 0     
              Min Echo interval: 0                           

Peer Addr 255.255.255.255, Tunnel ID 140737488355338(SR), Segment list ID 10, Type SBFD(initiator), State Up
VRF default, LAddr 10.0.0.32, LD/RD 866680721/866680721
Session state is Up and not using echo function
Hardware Acceleration: Async Off, Echo Off
Last Up 02/19/25 08:56:45.241
Last Down 02/19/25 08:48:41.917
Last Diag: No Diagnostic
Authentication mode: None
Shared-secret profile: None
TxInt: 100 ms, RxInt: 100 ms, Multiplier: 3
Received RxInt: 0 ms, Received Multiplier: 3
Rx Count: 1032, Rx Interval (ms) min/max/avg: 79/108/91 last: -530 ms ago
Tx Count: 1033, Tx Interval (ms) min/max/avg: 80/108/91 last: -530 ms ago
Detect Time: 300 ms
Sched Delay: 1*TxInt: 939, 2*TxInt: 93, 3*TxInt: 0, GT 3*TxInt: 0
RTT (us) min/max/avg: 44/546/109 last: 71 us
Registered protocols: sr-te policy
Uptime: 01:34.89
Tunnel Info:  MPLS label stack: [20030 20066]
              MPLS EXP: 7                    
              IP DSCP: 192                   
Last packet:  Version: 1           - Diagnostic: 0         
              State bit: Up        - Demand bit: 0         
              Poll bit: 0          - Final bit: 0          
              Multiplier: 3        - Length: 30            
              My Discr.: 866680721 - Your Discr.: 866680721
              Min tx interval: 100 - Min rx interval: 0    
              Min Echo interval: 0                         

Peer Addr 255.255.255.255, Tunnel ID 140737488355339(SR), Segment list ID 11, Type SBFD(initiator), State Up
VRF default, LAddr 10.0.0.32, LD/RD 3690177226/3690177226
Session state is Up and not using echo function
Hardware Acceleration: Async Off, Echo Off
Last Up 02/18/25 17:26:07.041
Last Down NA
Last Diag: No Diagnostic
Authentication mode: None
Shared-secret profile: None
TxInt: 100 ms, RxInt: 100 ms, Multiplier: 3
Received RxInt: 0 ms, Received Multiplier: 3
Rx Count: 605109, Rx Interval (ms) min/max/avg: 75/108/92 last: -598 ms ago
Tx Count: 605110, Tx Interval (ms) min/max/avg: 80/108/92 last: -598 ms ago
Detect Time: 300 ms
Sched Delay: 1*TxInt: 533090, 2*TxInt: 72019, 3*TxInt: 0, GT 3*TxInt: 0
RTT (us) min/max/avg: 66/1940/121 last: 143 us
Registered protocols: sr-te policy
Uptime: 15:32:13.09
Tunnel Info:  MPLS label stack: [20175 20120]
              MPLS EXP: 7                    
              IP DSCP: 192                   
Last packet:  Version: 1            - Diagnostic: 0          
              State bit: Up         - Demand bit: 0          
              Poll bit: 0           - Final bit: 0           
              Multiplier: 3         - Length: 30             
              My Discr.: 3690177226 - Your Discr.: 3690177226
              Min tx interval: 100  - Min rx interval: 0     
              Min Echo interval: 0                           

Peer Addr 255.255.255.255, Tunnel ID 140737488355342(SR), Segment list ID 14, Type SBFD(initiator), State Up
VRF default, LAddr 10.0.0.32, LD/RD 2613258878/2613258878
Session state is Up and not using echo function
Hardware Acceleration: Async Off, Echo Off
Last Up 02/19/25 08:56:46.041
Last Down 02/19/25 08:48:41.919
Last Diag: No Diagnostic
Authentication mode: None
Shared-secret profile: None
TxInt: 100 ms, RxInt: 100 ms, Multiplier: 3
Received RxInt: 0 ms, Received Multiplier: 3
Rx Count: 1017, Rx Interval (ms) min/max/avg: 79/108/92 last: -550 ms ago
Tx Count: 1018, Tx Interval (ms) min/max/avg: 80/108/92 last: -550 ms ago
Detect Time: 300 ms
Sched Delay: 1*TxInt: 907, 2*TxInt: 110, 3*TxInt: 0, GT 3*TxInt: 0
RTT (us) min/max/avg: 45/260/108 last: 61 us
Registered protocols: sr-te policy
Uptime: 01:34.10
Tunnel Info:  MPLS label stack: [20030 21221]
              MPLS EXP: 7                    
              IP DSCP: 192                   
Last packet:  Version: 1            - Diagnostic: 0          
              State bit: Up         - Demand bit: 0          
              Poll bit: 0           - Final bit: 0           
              Multiplier: 3         - Length: 30             
              My Discr.: 2613258878 - Your Discr.: 2613258878
              Min tx interval: 100  - Min rx interval: 0     
              Min Echo interval: 0                           

Peer Addr 255.255.255.255, Tunnel ID 140737488355343(SR), Segment list ID 15, Type SBFD(initiator), State Up
VRF default, LAddr 10.0.0.32, LD/RD 3974681151/3974681151
Session state is Up and not using echo function
Hardware Acceleration: Async Off, Echo Off
Last Up 02/18/25 17:23:04.857
Last Down NA
Last Diag: No Diagnostic
Authentication mode: None
Shared-secret profile: None
TxInt: 100 ms, RxInt: 100 ms, Multiplier: 3
Received RxInt: 0 ms, Received Multiplier: 3
Rx Count: 605960, Rx Interval (ms) min/max/avg: 75/108/92 last: -534 ms ago
Tx Count: 605960, Tx Interval (ms) min/max/avg: 80/108/92 last: -534 ms ago
Detect Time: 300 ms
Sched Delay: 1*TxInt: 534205, 2*TxInt: 71754, 3*TxInt: 0, GT 3*TxInt: 0
RTT (us) min/max/avg: 40/4072/101 last: 54 us
Registered protocols: sr-te policy
Uptime: 15:35:15.28
Tunnel Info:  MPLS label stack: [20175 20072]
              MPLS EXP: 7                    
              IP DSCP: 192                   
Last packet:  Version: 1            - Diagnostic: 0          
              State bit: Up         - Demand bit: 0          
              Poll bit: 0           - Final bit: 0           
              Multiplier: 3         - Length: 30             
              My Discr.: 3974681151 - Your Discr.: 3974681151
              Min tx interval: 100  - Min rx interval: 0     
              Min Echo interval: 0                           

Peer Addr 10.0.0.120, Dest Port 42781, Type SBFD(reflector), State Up
VRF default, LAddr 10.0.0.32, LD/RD 167772192/32782
Session state is Up
Last Up 02/18/25 17:02:22.685
Last Down NA
Last Diag: No Diagnostic
Last Rx state change: 02/18/25 17:02:22.685, old Rx state is Down
RxInt: 300 ms
Received TxInt: 100 ms, Received RxInt: 0 ms, Received Multiplier: 3
Rx Count: 195129, Rx Interval (ms) min/max/avg: 99/303/293 last: 213 ms ago
Tx Count: 195129, last: 213 ms ago
Last packet:  Version: 1           - Diagnostic: 0         
              State bit: Up        - Demand bit: 1         
              Poll bit: 0          - Final bit: 0          
              Multiplier: 3        - Length: 24            
              My Discr.: 32782     - Your Discr.: 167772192
              Min tx interval: 100 - Min rx interval: 0    
              Min Echo interval: 0                         

Peer Addr 10.0.0.124, Dest Port 4784, Type SBFD(reflector), State Up
VRF default, LAddr 10.0.0.32, LD/RD 167772192/16385
Session state is Up
Last Up 02/18/25 16:29:08.630
Last Down NA
Last Diag: No Diagnostic
Last Rx state change: 02/18/25 16:29:08.630, old Rx state is Down
RxInt: 300 ms
Received TxInt: 10 ms, Received RxInt: 0 ms, Received Multiplier: 3
Rx Count: 197833, Rx Interval (ms) min/max/avg: 1/300/300 last: 35 ms ago
Tx Count: 197833, last: 35 ms ago
Last packet:  Version: 1           - Diagnostic: 0         
              State bit: Up        - Demand bit: 1         
              Poll bit: 0          - Final bit: 0          
              Multiplier: 3        - Length: 24            
              My Discr.: 16385     - Your Discr.: 167772192
              Min tx interval: 10  - Min rx interval: 0    
              Min Echo interval: 0                         

Peer Addr 10.0.0.124, Dest Port 4784, Type SBFD(reflector), State Up
VRF default, LAddr 10.0.0.32, LD/RD 167772192/16386
Session state is Up
Last Up 02/18/25 16:29:04.230
Last Down NA
Last Diag: No Diagnostic
Last Rx state change: 02/18/25 16:33:36.331, old Rx state is Down
RxInt: 300 ms
Received TxInt: 10 ms, Received RxInt: 0 ms, Received Multiplier: 3
Rx Count: 197784, Rx Interval (ms) min/max/avg: 1/12191/300 last: 49 ms ago
Tx Count: 197784, last: 49 ms ago
Last packet:  Version: 1           - Diagnostic: 3         
              State bit: Up        - Demand bit: 1         
              Poll bit: 0          - Final bit: 0          
              Multiplier: 3        - Length: 24            
              My Discr.: 16386     - Your Discr.: 167772192
              Min tx interval: 10  - Min rx interval: 0    
              Min Echo interval: 0                         

Peer Addr 10.0.0.128, Dest Port 4784, Type SBFD(reflector), State Up
VRF default, LAddr 10.0.0.32, LD/RD 167772192/16385
Session state is Up
Last Up 02/18/25 16:29:04.729
Last Down NA
Last Diag: No Diagnostic
Last Rx state change: 02/18/25 17:05:48.952, old Rx state is Down
RxInt: 300 ms
Received TxInt: 10 ms, Received RxInt: 0 ms, Received Multiplier: 3
Rx Count: 197852, Rx Interval (ms) min/max/avg: 0/5371/299 last: 308 ms ago
Tx Count: 197852, last: 308 ms ago
Last packet:  Version: 1           - Diagnostic: 1         
              State bit: Up        - Demand bit: 1         
              Poll bit: 0          - Final bit: 0          
              Multiplier: 3        - Length: 24            
              My Discr.: 16385     - Your Discr.: 167772192
              Min tx interval: 10  - Min rx interval: 0    
              Min Echo interval: 0                         

Peer Addr 10.0.0.128, Dest Port 4784, Type SBFD(reflector), State Up
VRF default, LAddr 10.0.0.32, LD/RD 167772192/16386
Session state is Up
Last Up 02/18/25 16:28:58.529
Last Down NA
Last Diag: No Diagnostic
Last Rx state change: 02/18/25 16:28:58.529, old Rx state is Down
RxInt: 300 ms
Received TxInt: 10 ms, Received RxInt: 0 ms, Received Multiplier: 3
Rx Count: 197887, Rx Interval (ms) min/max/avg: 0/300/299 last: 181 ms ago
Tx Count: 197887, last: 181 ms ago
Last packet:  Version: 1           - Diagnostic: 0         
              State bit: Up        - Demand bit: 1         
              Poll bit: 0          - Final bit: 0          
              Multiplier: 3        - Length: 24            
              My Discr.: 16386     - Your Discr.: 167772192
              Min tx interval: 10  - Min rx interval: 0    
              Min Echo interval: 0                         

Peer Addr 10.0.0.156, Dest Port 4784, Type SBFD(reflector), State Up
VRF default, LAddr 10.0.0.32, LD/RD 167772192/22
Session state is Up
Last Up 02/19/25 07:50:14.436
Last Down NA
Last Diag: No Diagnostic
Last Rx state change: 02/19/25 08:21:31.416, old Rx state is Down
RxInt: 300 ms
Received TxInt: 300 ms, Received RxInt: 0 ms, Received Multiplier: 3
Rx Count: 8523, Rx Interval (ms) min/max/avg: 224/1803825/479 last: 234 ms ago
Tx Count: 8523, last: 234 ms ago
Last packet:  Version: 1           - Diagnostic: 0         
              State bit: Up        - Demand bit: 1         
              Poll bit: 0          - Final bit: 0          
              Multiplier: 3        - Length: 24            
              My Discr.: 22        - Your Discr.: 167772192
              Min tx interval: 300 - Min rx interval: 0    
              Min Echo interval: 0                         

Peer Addr 10.0.0.179, Dest Port 4784, Type SBFD(reflector), State Up
VRF default, LAddr 10.0.0.32, LD/RD 167772192/18
Session state is Up
Last Up 02/18/25 16:24:10.654
Last Down NA
Last Diag: No Diagnostic
Last Rx state change: 02/18/25 16:25:09.932, old Rx state is Down
RxInt: 300 ms
Received TxInt: 10 ms, Received RxInt: 0 ms, Received Multiplier: 3
Rx Count: 3382, Rx Interval (ms) min/max/avg: 222/1990/276 last: 58716318 ms ago
Tx Count: 3382, last: 58716318 ms ago
Last packet:  Version: 1           - Diagnostic: 0         
              State bit: Up        - Demand bit: 1         
              Poll bit: 0          - Final bit: 0          
              Multiplier: 3        - Length: 24            
              My Discr.: 18        - Your Discr.: 167772192
              Min tx interval: 10  - Min rx interval: 0    
              Min Echo interval: 0                         

Peer Addr 10.0.0.179, Dest Port 4784, Type SBFD(reflector), State Up
VRF default, LAddr 10.0.0.32, LD/RD 167772192/24
Session state is Up
Last Up 02/18/25 16:39:50.443
Last Down NA
Last Diag: No Diagnostic
Last Rx state change: 02/18/25 16:44:45.360, old Rx state is Down
RxInt: 300 ms
Received TxInt: 10 ms, Received RxInt: 0 ms, Received Multiplier: 3
Rx Count: 3166, Rx Interval (ms) min/max/avg: 216/169656/332 last: 57658658 ms ago
Tx Count: 3166, last: 57658658 ms ago
Last packet:  Version: 1           - Diagnostic: 0         
              State bit: Up        - Demand bit: 1         
              Poll bit: 0          - Final bit: 0          
              Multiplier: 3        - Length: 24            
              My Discr.: 24        - Your Discr.: 167772192
              Min tx interval: 10  - Min rx interval: 0    
              Min Echo interval: 0                         

Peer Addr 10.0.0.179, Dest Port 4784, Type SBFD(reflector), State Up
VRF default, LAddr 10.0.0.32, LD/RD 167772192/26
Session state is Up
Last Up 02/18/25 16:57:28.366
Last Down NA
Last Diag: No Diagnostic
Last Rx state change: 02/18/25 16:58:27.221, old Rx state is Down
RxInt: 300 ms
Received TxInt: 10 ms, Received RxInt: 0 ms, Received Multiplier: 3
Rx Count: 417, Rx Interval (ms) min/max/avg: 224/1987/371 last: 57499231 ms ago
Tx Count: 417, last: 57499231 ms ago
Last packet:  Version: 1           - Diagnostic: 0         
              State bit: Up        - Demand bit: 1         
              Poll bit: 0          - Final bit: 0          
              Multiplier: 3        - Length: 24            
              My Discr.: 26        - Your Discr.: 167772192
              Min tx interval: 10  - Min rx interval: 0    
              Min Echo interval: 0                         

Peer Addr 10.0.0.179, Dest Port 4784, Type SBFD(reflector), State Up
VRF default, LAddr 10.0.0.32, LD/RD 167772192/29
Session state is Up
Last Up 02/18/25 17:00:07.899
Last Down NA
Last Diag: No Diagnostic
Last Rx state change: 02/18/25 17:27:18.350, old Rx state is Down
RxInt: 300 ms
Received TxInt: 100 ms, Received RxInt: 0 ms, Received Multiplier: 3
Rx Count: 218374, Rx Interval (ms) min/max/avg: 191/1987/263 last: 95 ms ago
Tx Count: 218374, last: 95 ms ago
Last packet:  Version: 1           - Diagnostic: 0         
              State bit: Up        - Demand bit: 1         
              Poll bit: 0          - Final bit: 0          
              Multiplier: 3        - Length: 24            
              My Discr.: 29        - Your Discr.: 167772192
              Min tx interval: 100 - Min rx interval: 0    
              Min Echo interval: 0                         

Peer Addr 10.0.0.217, Dest Port 49152, Type SBFD(reflector), State Up
VRF default, LAddr 10.0.0.32, LD/RD 167772192/1
Session state is Up
Last Up 02/18/25 16:31:02.031
Last Down NA
Last Diag: No Diagnostic
Last Rx state change: 02/18/25 16:31:02.031, old Rx state is Down
RxInt: 300 ms
Received TxInt: 100 ms, Received RxInt: 0 ms, Received Multiplier: 3
Rx Count: 3397, Rx Interval (ms) min/max/avg: 101/262/262 last: 58348177 ms ago
Tx Count: 3397, last: 58348177 ms ago
Last packet:  Version: 1           - Diagnostic: 0         
              State bit: Up        - Demand bit: 1         
              Poll bit: 0          - Final bit: 0          
              Multiplier: 3        - Length: 24            
              My Discr.: 1         - Your Discr.: 167772192
              Min tx interval: 100 - Min rx interval: 0    
              Min Echo interval: 0                         

Peer Addr 10.0.0.217, Dest Port 49152, Type SBFD(reflector), State Up
VRF default, LAddr 10.0.0.32, LD/RD 167772192/77
Session state is Up
Last Up 02/18/25 16:41:18.315
Last Down NA
Last Diag: No Diagnostic
Last Rx state change: 02/18/25 16:41:18.315, old Rx state is Down
RxInt: 300 ms
Received TxInt: 100 ms, Received RxInt: 0 ms, Received Multiplier: 3
Rx Count: 1046, Rx Interval (ms) min/max/avg: 6/262/261 last: 58348177 ms ago
Tx Count: 1046, last: 58348177 ms ago
Last packet:  Version: 1           - Diagnostic: 0         
              State bit: Up        - Demand bit: 1         
              Poll bit: 0          - Final bit: 0          
              Multiplier: 3        - Length: 24            
              My Discr.: 77        - Your Discr.: 167772192
              Min tx interval: 100 - Min rx interval: 0    
              Min Echo interval: 0                         

Peer Addr 10.0.0.217, Dest Port 49152, Type SBFD(reflector), State Up
VRF default, LAddr 10.0.0.32, LD/RD 167772192/140
Session state is Up
Last Up 02/18/25 16:45:56.810
Last Down NA
Last Diag: No Diagnostic
Last Rx state change: 02/18/25 16:45:56.810, old Rx state is Down
RxInt: 300 ms
Received TxInt: 100 ms, Received RxInt: 0 ms, Received Multiplier: 3
Rx Count: 269, Rx Interval (ms) min/max/avg: 4/262/260 last: 58273463 ms ago
Tx Count: 269, last: 58273463 ms ago
Last packet:  Version: 1           - Diagnostic: 0         
              State bit: Up        - Demand bit: 1         
              Poll bit: 0          - Final bit: 0          
              Multiplier: 3        - Length: 24            
              My Discr.: 140       - Your Discr.: 167772192
              Min tx interval: 100 - Min rx interval: 0    
              Min Echo interval: 0                         

Peer Addr 10.0.0.217, Dest Port 49152, Type SBFD(reflector), State Up
VRF default, LAddr 10.0.0.32, LD/RD 167772192/141
Session state is Up
Last Up 02/18/25 16:45:56.804
Last Down NA
Last Diag: No Diagnostic
Last Rx state change: 02/18/25 16:45:56.804, old Rx state is Down
RxInt: 300 ms
Received TxInt: 100 ms, Received RxInt: 0 ms, Received Multiplier: 3
Rx Count: 225, Rx Interval (ms) min/max/avg: 2/262/260 last: 58284926 ms ago
Tx Count: 225, last: 58284926 ms ago
Last packet:  Version: 1           - Diagnostic: 0         
              State bit: Up        - Demand bit: 1         
              Poll bit: 0          - Final bit: 0          
              Multiplier: 3        - Length: 24            
              My Discr.: 141       - Your Discr.: 167772192
              Min tx interval: 100 - Min rx interval: 0    
              Min Echo interval: 0                         

Peer Addr 10.0.0.217, Dest Port 49152, Type SBFD(reflector), State Up
VRF default, LAddr 10.0.0.32, LD/RD 167772192/168
Session state is Up
Last Up 02/18/25 16:47:00.981
Last Down NA
Last Diag: No Diagnostic
Last Rx state change: 02/18/25 16:47:00.981, old Rx state is Down
RxInt: 300 ms
Received TxInt: 100 ms, Received RxInt: 0 ms, Received Multiplier: 3
Rx Count: 24, Rx Interval (ms) min/max/avg: 10/262/246 last: 58273463 ms ago
Tx Count: 24, last: 58273463 ms ago
Last packet:  Version: 1           - Diagnostic: 0         
              State bit: Up        - Demand bit: 1         
              Poll bit: 0          - Final bit: 0          
              Multiplier: 3        - Length: 24            
              My Discr.: 168       - Your Discr.: 167772192
              Min tx interval: 100 - Min rx interval: 0    
              Min Echo interval: 0                         

Peer Addr 10.0.0.217, Dest Port 49152, Type SBFD(reflector), State Up
VRF default, LAddr 10.0.0.32, LD/RD 167772192/178
Session state is Up
Last Up 02/18/25 16:47:09.461
Last Down NA
Last Diag: No Diagnostic
Last Rx state change: 02/18/25 16:47:09.461, old Rx state is Down
RxInt: 300 ms
Received TxInt: 100 ms, Received RxInt: 0 ms, Received Multiplier: 3
Rx Count: 2696, Rx Interval (ms) min/max/avg: 10/262/262 last: 57564398 ms ago
Tx Count: 2696, last: 57564398 ms ago
Last packet:  Version: 1           - Diagnostic: 0         
              State bit: Up        - Demand bit: 1         
              Poll bit: 0          - Final bit: 0          
              Multiplier: 3        - Length: 24            
              My Discr.: 178       - Your Discr.: 167772192
              Min tx interval: 100 - Min rx interval: 0    
              Min Echo interval: 0                         

Peer Addr 10.0.0.217, Dest Port 49152, Type SBFD(reflector), State Up
VRF default, LAddr 10.0.0.32, LD/RD 167772192/179
Session state is Up
Last Up 02/18/25 16:47:09.453
Last Down NA
Last Diag: No Diagnostic
Last Rx state change: 02/18/25 16:47:09.453, old Rx state is Down
RxInt: 300 ms
Received TxInt: 100 ms, Received RxInt: 0 ms, Received Multiplier: 3
Rx Count: 2696, Rx Interval (ms) min/max/avg: 1/262/262 last: 57564398 ms ago
Tx Count: 2696, last: 57564398 ms ago
Last packet:  Version: 1           - Diagnostic: 0         
              State bit: Up        - Demand bit: 1         
              Poll bit: 0          - Final bit: 0          
              Multiplier: 3        - Length: 24            
              My Discr.: 179       - Your Discr.: 167772192
              Min tx interval: 100 - Min rx interval: 0    
              Min Echo interval: 0                         

Peer Addr 10.0.0.217, Dest Port 49152, Type SBFD(reflector), State Up
VRF default, LAddr 10.0.0.32, LD/RD 167772192/332
Session state is Up
Last Up 02/18/25 16:58:55.819
Last Down NA
Last Diag: No Diagnostic
Last Rx state change: 02/18/25 16:58:55.819, old Rx state is Down
RxInt: 300 ms
Received TxInt: 100 ms, Received RxInt: 0 ms, Received Multiplier: 3
Rx Count: 38, Rx Interval (ms) min/max/avg: 4/262/250 last: 57555029 ms ago
Tx Count: 38, last: 57555029 ms ago
Last packet:  Version: 1           - Diagnostic: 0         
              State bit: Up        - Demand bit: 1         
              Poll bit: 0          - Final bit: 0          
              Multiplier: 3        - Length: 24            
              My Discr.: 332       - Your Discr.: 167772192
              Min tx interval: 100 - Min rx interval: 0    
              Min Echo interval: 0                         

Peer Addr 10.0.0.217, Dest Port 49152, Type SBFD(reflector), State Up
VRF default, LAddr 10.0.0.32, LD/RD 167772192/333
Session state is Up
Last Up 02/18/25 16:58:55.827
Last Down NA
Last Diag: No Diagnostic
Last Rx state change: 02/18/25 16:58:55.827, old Rx state is Down
RxInt: 300 ms
Received TxInt: 100 ms, Received RxInt: 0 ms, Received Multiplier: 3
Rx Count: 79, Rx Interval (ms) min/max/avg: 4/262/255 last: 57544329 ms ago
Tx Count: 79, last: 57544329 ms ago
Last packet:  Version: 1           - Diagnostic: 0         
              State bit: Up        - Demand bit: 1         
              Poll bit: 0          - Final bit: 0          
              Multiplier: 3        - Length: 24            
              My Discr.: 333       - Your Discr.: 167772192
              Min tx interval: 100 - Min rx interval: 0    
              Min Echo interval: 0                         

Peer Addr 10.0.0.217, Dest Port 49152, Type SBFD(reflector), State Up
VRF default, LAddr 10.0.0.32, LD/RD 167772192/336
Session state is Up
Last Up 02/18/25 16:59:05.131
Last Down NA
Last Diag: No Diagnostic
Last Rx state change: 02/18/25 16:59:05.131, old Rx state is Down
RxInt: 300 ms
Received TxInt: 100 ms, Received RxInt: 0 ms, Received Multiplier: 3
Rx Count: 219519, Rx Interval (ms) min/max/avg: 8/262/262 last: 78 ms ago
Tx Count: 219519, last: 78 ms ago
Last packet:  Version: 1           - Diagnostic: 0         
              State bit: Up        - Demand bit: 1         
              Poll bit: 0          - Final bit: 0          
              Multiplier: 3        - Length: 24            
              My Discr.: 336       - Your Discr.: 167772192
              Min tx interval: 100 - Min rx interval: 0    
              Min Echo interval: 0                         

Peer Addr 10.0.0.217, Dest Port 49152, Type SBFD(reflector), State Up
VRF default, LAddr 10.0.0.32, LD/RD 167772192/338
Session state is Up
Last Up 02/18/25 16:59:15.940
Last Down NA
Last Diag: No Diagnostic
Last Rx state change: 02/18/25 16:59:15.940, old Rx state is Down
RxInt: 300 ms
Received TxInt: 100 ms, Received RxInt: 0 ms, Received Multiplier: 3
Rx Count: 219477, Rx Interval (ms) min/max/avg: 10/268/262 last: 281 ms ago
Tx Count: 219477, last: 281 ms ago
Last packet:  Version: 1           - Diagnostic: 0         
              State bit: Up        - Demand bit: 1         
              Poll bit: 0          - Final bit: 0          
              Multiplier: 3        - Length: 24            
              My Discr.: 338       - Your Discr.: 167772192
              Min tx interval: 100 - Min rx interval: 0    
              Min Echo interval: 0                         

Peer Addr 10.0.0.221, Dest Port 49153, Type SBFD(reflector), State Up
VRF default, LAddr 10.0.0.32, LD/RD 167772192/167780343
Session state is Up
Last Up 02/18/25 17:00:53.784
Last Down NA
Last Diag: No Diagnostic
Last Rx state change: 02/18/25 17:00:53.784, old Rx state is Down
RxInt: 300 ms
Received TxInt: 100 ms, Received RxInt: 0 ms, Received Multiplier: 3
Rx Count: 58895, Rx Interval (ms) min/max/avg: 100/1001/975 last: 99 ms ago
Tx Count: 58895, last: 99 ms ago
Last packet:  Version: 1           - Diagnostic: 0         
              State bit: Up        - Demand bit: 1         
              Poll bit: 0          - Final bit: 0          
              Multiplier: 3        - Length: 24            
              My Discr.: 167780343 - Your Discr.: 167772192
              Min tx interval: 100 - Min rx interval: 0    
              Min Echo interval: 0                         

Peer Addr 10.0.0.221, Dest Port 49153, Type SBFD(reflector), State Up
VRF default, LAddr 10.0.0.32, LD/RD 167772192/167780351
Session state is Up
Last Up 02/18/25 16:38:52.367
Last Down NA
Last Diag: No Diagnostic
Last Rx state change: 02/18/25 16:38:52.367, old Rx state is Down
RxInt: 300 ms
Received TxInt: 100 ms, Received RxInt: 0 ms, Received Multiplier: 3
Rx Count: 60216, Rx Interval (ms) min/max/avg: 99/1001/975 last: 99 ms ago
Tx Count: 60216, last: 99 ms ago
Last packet:  Version: 1           - Diagnostic: 0         
              State bit: Up        - Demand bit: 1         
              Poll bit: 0          - Final bit: 0          
              Multiplier: 3        - Length: 24            
              My Discr.: 167780351 - Your Discr.: 167772192
              Min tx interval: 100 - Min rx interval: 0    
              Min Echo interval: 0                         

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
 I L2     10.0.0.66/32 [115/30]
           via 20.30.32.30, Ethernet1
 I L2     10.0.0.72/32 [115/30]
           via 20.30.32.30, Ethernet1
 I L2     10.0.0.84/32 [115/30]
           via 20.30.32.30, Ethernet1
 I L2     10.0.0.120/32 [115/20]
           via 20.30.32.30, Ethernet1
 I L2     10.0.0.124/32 [115/20]
           via 20.30.32.30, Ethernet1
 I L2     10.0.0.128/32 [115/20]
           via 20.30.32.30, Ethernet1
 I L2     10.0.0.156/32 [115/20]
           via 20.30.32.30, Ethernet1
           via 20.32.175.175, Ethernet5
 I L2     10.0.0.175/32 [115/10]
           via 20.32.175.175, Ethernet5
 I L2     10.0.0.179/32 [115/20]
           via 20.30.32.30, Ethernet1
 I L2     10.0.0.184/32 [115/35]
           via 20.32.175.175, Ethernet5
 I L2     10.0.0.214/32 [115/20]
           via 20.30.32.30, Ethernet1
 I L2     10.0.0.217/32 [115/20]
           via 20.30.32.30, Ethernet1
 I L2     10.0.0.221/32 [115/20]
           via 20.30.32.30, Ethernet1
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
 I L2     20.66.175.0/24 [115/25]
           via 20.32.175.175, Ethernet5
 I L2     20.72.175.0/24 [115/25]
           via 20.32.175.175, Ethernet5
 I L2     20.84.175.0/24 [115/25]
           via 20.32.175.175, Ethernet5
 I L2     20.120.175.0/24 [115/25]
           via 20.32.175.175, Ethernet5
 I L2     20.120.214.0/24 [115/30]
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

```

## show ip route vrf all

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
 I L2     10.0.0.66/32 [115/30]
           via 20.30.32.30, Ethernet1
 I L2     10.0.0.72/32 [115/30]
           via 20.30.32.30, Ethernet1
 I L2     10.0.0.84/32 [115/30]
           via 20.30.32.30, Ethernet1
 I L2     10.0.0.120/32 [115/20]
           via 20.30.32.30, Ethernet1
 I L2     10.0.0.124/32 [115/20]
           via 20.30.32.30, Ethernet1
 I L2     10.0.0.128/32 [115/20]
           via 20.30.32.30, Ethernet1
 I L2     10.0.0.156/32 [115/20]
           via 20.30.32.30, Ethernet1
           via 20.32.175.175, Ethernet5
 I L2     10.0.0.175/32 [115/10]
           via 20.32.175.175, Ethernet5
 I L2     10.0.0.179/32 [115/20]
           via 20.30.32.30, Ethernet1
 I L2     10.0.0.184/32 [115/35]
           via 20.32.175.175, Ethernet5
 I L2     10.0.0.214/32 [115/20]
           via 20.30.32.30, Ethernet1
 I L2     10.0.0.217/32 [115/20]
           via 20.30.32.30, Ethernet1
 I L2     10.0.0.221/32 [115/20]
           via 20.30.32.30, Ethernet1
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
 I L2     20.66.175.0/24 [115/25]
           via 20.32.175.175, Ethernet5
 I L2     20.72.175.0/24 [115/25]
           via 20.32.175.175, Ethernet5
 I L2     20.84.175.0/24 [115/25]
           via 20.32.175.175, Ethernet5
 I L2     20.120.175.0/24 [115/25]
           via 20.32.175.175, Ethernet5
 I L2     20.120.214.0/24 [115/30]
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

 B I      20.184.184.0/24 [200/0]
           via 10.0.0.184/32, IS-IS SR tunnel index 15, label 16
              via TI-LFA tunnel index 5, label 20484
                 via 20.32.175.175, Ethernet5, label imp-null(3)
                 backup via 20.30.32.30, Ethernet1, label 20217
 C        50.10.32.0/24
           directly connected, Ethernet40.4
 B I      50.10.53.0/24 [200/0]
           via 10.0.0.53/32, IS-IS SR tunnel index 6, label 970000
              via TI-LFA tunnel index 1, label 20053
                 via 20.30.32.30, Ethernet1, label imp-null(3)
                 backup via 20.32.175.175, Ethernet5, label imp-null(3)
 B I      50.10.66.0/24 [200/0]
           via SR-TE Policy 10.0.0.66, color 100, label 62000
              via SR-TE tunnel index 10, weight 1
                 via TI-LFA tunnel index 3, label 20066
                    via 20.30.32.30, Ethernet1, label imp-null(3)
                    backup via 20.32.175.175, Ethernet5, label 20030
 B I      50.10.72.0/24 [200/0]
           via SR-TE Policy 10.0.0.72, color 100, label 62002
              via SR-TE tunnel index 1, weight 1
                 via TI-LFA tunnel index 3, label 20072
                    via 20.30.32.30, Ethernet1, label imp-null(3)
                    backup via 20.32.175.175, Ethernet5, label 20030
 B I      50.10.84.0/24 [200/0]
           via 10.0.0.84/32, IS-IS SR tunnel index 2, label 720896
              via TI-LFA tunnel index 1, label 20084
                 via 20.30.32.30, Ethernet1, label imp-null(3)
                 backup via 20.32.175.175, Ethernet5, label imp-null(3)
 B I      50.10.120.0/24 [200/0]
           via SR-TE Policy 10.0.0.120, color 100, label 1277
              via SR-TE tunnel index 6, weight 1
                 via TI-LFA tunnel index 3, label 20120
                    via 20.30.32.30, Ethernet1, label imp-null(3)
                    backup via 20.32.175.175, Ethernet5, label 20030
 B I      50.10.124.0/24 [200/0]
           via SR-TE Policy 10.0.0.124, color 100, label 332
              via SR-TE tunnel index 5, weight 1
                 via TI-LFA tunnel index 3, label 20124
                    via 20.30.32.30, Ethernet1, label imp-null(3)
                    backup via 20.32.175.175, Ethernet5, label 20030
 B I      50.10.128.0/24 [200/0]
           via SR-TE Policy 10.0.0.128, color 100, label 48060
              via SR-TE tunnel index 16, weight 1
                 via TI-LFA tunnel index 3, label 20128
                    via 20.30.32.30, Ethernet1, label imp-null(3)
                    backup via 20.32.175.175, Ethernet5, label 20030
 B I      50.10.156.0/24 [200/0]
           via 10.0.0.156/32, IS-IS SR tunnel index 18, label 16
              via 20.30.32.30, Ethernet1, label 20156
              via 20.32.175.175, Ethernet5, label 20156
 B I      50.10.179.0/24 [200/0]
           via SR-TE Policy 10.0.0.179, color 100, label 16
              via SR-TE tunnel index 7, weight 1
                 via TI-LFA tunnel index 3, label 20179
                    via 20.30.32.30, Ethernet1, label imp-null(3)
                    backup via 20.32.175.175, Ethernet5, label 20030
 B I      50.10.214.0/24 [200/0]
           via 10.0.0.214/32, IS-IS SR tunnel index 10, label 500000
              via TI-LFA tunnel index 1, label 20214
                 via 20.30.32.30, Ethernet1, label imp-null(3)
                 backup via 20.32.175.175, Ethernet5, label imp-null(3)
 B I      50.10.217.0/24 [200/0]
           via SR-TE Policy 10.0.0.217, color 100, label 524287
              via SR-TE tunnel index 13, weight 1
                 via TI-LFA tunnel index 3, label 20217
                    via 20.30.32.30, Ethernet1, label imp-null(3)
                    backup via 20.32.175.175, Ethernet5, label 20030
 B I      50.10.221.0/24 [200/0]
           via SR-TE Policy 10.0.0.221, color 100, label 524305
              via SR-TE tunnel index 14, weight 1
                 via TI-LFA tunnel index 3, label 21221
                    via 20.30.32.30, Ethernet1, label imp-null(3)
                    backup via 20.32.175.175, Ethernet5, label 20030
 B I      51.10.120.0/24 [200/0]
           via SR-TE Policy 10.0.0.120, color 100, label 1277
              via SR-TE tunnel index 6, weight 1
                 via TI-LFA tunnel index 3, label 20120
                    via 20.30.32.30, Ethernet1, label imp-null(3)
                    backup via 20.32.175.175, Ethernet5, label 20030


VRF: mgmt
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

Gateway of last resort:
 S        0.0.0.0/0 [1/0]
           via 192.168.20.1, Management1

 C        192.168.20.0/23
           directly connected, Management1

```

## show ipv6 route

```text

VRF: default
Displaying 18 of 23 IPv6 routing table entries
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
 I L2     2001:0:30:156::/64 [115/20]
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

## show mpls route

```text
MPLS forwarding table (Label [metric] Vias) - 29 routes 
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
                  via TI-LFA tunnel index 3
                    via 20.30.32.30, Ethernet1, label imp-null(3)
                    backup via 20.32.175.175, Ethernet5, label 20030
 20053   A[1]
                via M, ::, forward
                    EgressACL: apply
                  via TI-LFA tunnel index 1
                    via 20.30.32.30, Ethernet1, label imp-null(3)
                    backup via 20.32.175.175, Ethernet5, label imp-null(3)
 20066   A[1]
                via M, ::, forward
                    EgressACL: apply
                  via TI-LFA tunnel index 1
                    via 20.30.32.30, Ethernet1, label imp-null(3)
                    backup via 20.32.175.175, Ethernet5, label imp-null(3)
 20072   A[1]
                via M, ::, forward
                    EgressACL: apply
                  via TI-LFA tunnel index 1
                    via 20.30.32.30, Ethernet1, label imp-null(3)
                    backup via 20.32.175.175, Ethernet5, label imp-null(3)
 20084   A[1]
                via M, ::, forward
                    EgressACL: apply
                  via TI-LFA tunnel index 1
                    via 20.30.32.30, Ethernet1, label imp-null(3)
                    backup via 20.32.175.175, Ethernet5, label imp-null(3)
 20120   A[1]
                via M, ::, forward
                    EgressACL: apply
                  via TI-LFA tunnel index 1
                    via 20.30.32.30, Ethernet1, label imp-null(3)
                    backup via 20.32.175.175, Ethernet5, label imp-null(3)
 20124   A[1]
                via M, ::, forward
                    EgressACL: apply
                  via TI-LFA tunnel index 1
                    via 20.30.32.30, Ethernet1, label imp-null(3)
                    backup via 20.32.175.175, Ethernet5, label imp-null(3)
 20128   A[1]
                via M, ::, forward
                    EgressACL: apply
                  via TI-LFA tunnel index 1
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
                  via TI-LFA tunnel index 18
                    via 20.32.175.175, Ethernet5, label imp-null(3)
                    backup via 20.30.32.30, Ethernet1, label 20124 2175
 20179   A[1]
                via M, ::, forward
                    EgressACL: apply
                  via TI-LFA tunnel index 1
                    via 20.30.32.30, Ethernet1, label imp-null(3)
                    backup via 20.32.175.175, Ethernet5, label imp-null(3)
 20214   A[1]
                via M, ::, forward
                    EgressACL: apply
                  via TI-LFA tunnel index 1
                    via 20.30.32.30, Ethernet1, label imp-null(3)
                    backup via 20.32.175.175, Ethernet5, label imp-null(3)
 20217   A[1]
                via M, ::, forward
                    EgressACL: apply
                  via TI-LFA tunnel index 1
                    via 20.30.32.30, Ethernet1, label imp-null(3)
                    backup via 20.32.175.175, Ethernet5, label imp-null(3)
 20484   A[1]
                via M, ::, forward
                    EgressACL: apply
                  via TI-LFA tunnel index 5
                    via 20.32.175.175, Ethernet5, label imp-null(3)
                    backup via 20.30.32.30, Ethernet1, label 20217
 21221   A[1]
                via M, ::, forward
                    EgressACL: apply
                  via TI-LFA tunnel index 1
                    via 20.30.32.30, Ethernet1, label imp-null(3)
                    backup via 20.32.175.175, Ethernet5, label imp-null(3)
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
 1004066 A[1]
                SR-TE Policy 10.0.0.66, color 100, pop
                    EgressACL: apply
                  via SR-TE tunnel index 10
                    via TI-LFA tunnel index 3, label 20066
                       via 20.30.32.30, Ethernet1, label imp-null(3)
                       backup via 20.32.175.175, Ethernet5, label 20030
 1004072 A[1]
                SR-TE Policy 10.0.0.72, color 100, pop
                    EgressACL: apply
                  via SR-TE tunnel index 1
                    via TI-LFA tunnel index 3, label 20072
                       via 20.30.32.30, Ethernet1, label imp-null(3)
                       backup via 20.32.175.175, Ethernet5, label 20030
 1004120 A[1]
                SR-TE Policy 10.0.0.120, color 100, pop
                    EgressACL: apply
                  via SR-TE tunnel index 6
                    via TI-LFA tunnel index 3, label 20120
                       via 20.30.32.30, Ethernet1, label imp-null(3)
                       backup via 20.32.175.175, Ethernet5, label 20030
 1004124 A[1]
                SR-TE Policy 10.0.0.124, color 100, pop
                    EgressACL: apply
                  via SR-TE tunnel index 5
                    via TI-LFA tunnel index 3, label 20124
                       via 20.30.32.30, Ethernet1, label imp-null(3)
                       backup via 20.32.175.175, Ethernet5, label 20030
 1004128 A[1]
                SR-TE Policy 10.0.0.128, color 100, pop
                    EgressACL: apply
                  via SR-TE tunnel index 16
                    via TI-LFA tunnel index 3, label 20128
                       via 20.30.32.30, Ethernet1, label imp-null(3)
                       backup via 20.32.175.175, Ethernet5, label 20030
 1004156 A[1]
                SR-TE Policy 10.0.0.156, color 100, pop
                    EgressACL: apply
                  via SR-TE tunnel index 18
                    via TI-LFA tunnel index 3, label 20156
                       via 20.30.32.30, Ethernet1, label imp-null(3)
                       backup via 20.32.175.175, Ethernet5, label 20030
 1004179 A[1]
                SR-TE Policy 10.0.0.179, color 100, pop
                    EgressACL: apply
                  via SR-TE tunnel index 7
                    via TI-LFA tunnel index 3, label 20179
                       via 20.30.32.30, Ethernet1, label imp-null(3)
                       backup via 20.32.175.175, Ethernet5, label 20030
 1004217 A[1]
                SR-TE Policy 10.0.0.217, color 100, pop
                    EgressACL: apply
                  via SR-TE tunnel index 13
                    via TI-LFA tunnel index 3, label 20217
                       via 20.30.32.30, Ethernet1, label imp-null(3)
                       backup via 20.32.175.175, Ethernet5, label 20030
 1004221 A[1]
                SR-TE Policy 10.0.0.221, color 100, pop
                    EgressACL: apply
                  via SR-TE tunnel index 14
                    via TI-LFA tunnel index 3, label 21221
                       via 20.30.32.30, Ethernet1, label imp-null(3)
                       backup via 20.32.175.175, Ethernet5, label 20030
```

## show mpls lfib route

```text
MPLS forwarding table (Label [metric] Vias) - 29 routes 
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
                via TI-LFA tunnel index 3, pop
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                    via 20.30.32.30, Ethernet1, label imp-null(3)
                    backup via 20.32.175.175, Ethernet5, label 20030
 IP    20053    [1], 10.0.0.53/32
                via TI-LFA tunnel index 1, forward
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                    via 20.30.32.30, Ethernet1, label imp-null(3)
                    backup via 20.32.175.175, Ethernet5, label imp-null(3)
 IP    20066    [1], 10.0.0.66/32
                via TI-LFA tunnel index 1, forward
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                    via 20.30.32.30, Ethernet1, label imp-null(3)
                    backup via 20.32.175.175, Ethernet5, label imp-null(3)
 IP    20072    [1], 10.0.0.72/32
                via TI-LFA tunnel index 1, forward
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                    via 20.30.32.30, Ethernet1, label imp-null(3)
                    backup via 20.32.175.175, Ethernet5, label imp-null(3)
 IP    20084    [1], 10.0.0.84/32
                via TI-LFA tunnel index 1, forward
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                    via 20.30.32.30, Ethernet1, label imp-null(3)
                    backup via 20.32.175.175, Ethernet5, label imp-null(3)
 IP    20120    [1], 10.0.0.120/32
                via TI-LFA tunnel index 1, forward
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                    via 20.30.32.30, Ethernet1, label imp-null(3)
                    backup via 20.32.175.175, Ethernet5, label imp-null(3)
 IP    20124    [1], 10.0.0.124/32
                via TI-LFA tunnel index 1, forward
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                    via 20.30.32.30, Ethernet1, label imp-null(3)
                    backup via 20.32.175.175, Ethernet5, label imp-null(3)
 IP    20128    [1], 10.0.0.128/32
                via TI-LFA tunnel index 1, forward
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
                via TI-LFA tunnel index 18, pop
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                    via 20.32.175.175, Ethernet5, label imp-null(3)
                    backup via 20.30.32.30, Ethernet1, label 20124 2175
 IP    20179    [1], 10.0.0.179/32
                via TI-LFA tunnel index 1, forward
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                    via 20.30.32.30, Ethernet1, label imp-null(3)
                    backup via 20.32.175.175, Ethernet5, label imp-null(3)
 IP    20214    [1], 10.0.0.214/32
                via TI-LFA tunnel index 1, forward
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                    via 20.30.32.30, Ethernet1, label imp-null(3)
                    backup via 20.32.175.175, Ethernet5, label imp-null(3)
 IP    20217    [1], 10.0.0.217/32
                via TI-LFA tunnel index 1, forward
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                    via 20.30.32.30, Ethernet1, label imp-null(3)
                    backup via 20.32.175.175, Ethernet5, label imp-null(3)
 IP    20484    [1], 10.0.0.184/32
                via TI-LFA tunnel index 5, forward
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                    via 20.32.175.175, Ethernet5, label imp-null(3)
                    backup via 20.30.32.30, Ethernet1, label 20217
 IP    21221    [1], 10.0.0.221/32
                via TI-LFA tunnel index 1, forward
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                    via 20.30.32.30, Ethernet1, label imp-null(3)
                    backup via 20.32.175.175, Ethernet5, label imp-null(3)
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
 ST    1004066  [1], SR-TE Policy 10.0.0.66, color 100
                via SR-TE tunnel index 10, pop
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                    via TI-LFA tunnel index 3, label 20066
                       via 20.30.32.30, Ethernet1, label imp-null(3)
                       backup via 20.32.175.175, Ethernet5, label 20030
 ST    1004072  [1], SR-TE Policy 10.0.0.72, color 100
                via SR-TE tunnel index 1, pop
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                    via TI-LFA tunnel index 3, label 20072
                       via 20.30.32.30, Ethernet1, label imp-null(3)
                       backup via 20.32.175.175, Ethernet5, label 20030
 ST    1004120  [1], SR-TE Policy 10.0.0.120, color 100
                via SR-TE tunnel index 6, pop
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                    via TI-LFA tunnel index 3, label 20120
                       via 20.30.32.30, Ethernet1, label imp-null(3)
                       backup via 20.32.175.175, Ethernet5, label 20030
 ST    1004124  [1], SR-TE Policy 10.0.0.124, color 100
                via SR-TE tunnel index 5, pop
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                    via TI-LFA tunnel index 3, label 20124
                       via 20.30.32.30, Ethernet1, label imp-null(3)
                       backup via 20.32.175.175, Ethernet5, label 20030
 ST    1004128  [1], SR-TE Policy 10.0.0.128, color 100
                via SR-TE tunnel index 16, pop
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                    via TI-LFA tunnel index 3, label 20128
                       via 20.30.32.30, Ethernet1, label imp-null(3)
                       backup via 20.32.175.175, Ethernet5, label 20030
 ST    1004156  [1], SR-TE Policy 10.0.0.156, color 100
                via SR-TE tunnel index 18, pop
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                    via TI-LFA tunnel index 3, label 20156
                       via 20.30.32.30, Ethernet1, label imp-null(3)
                       backup via 20.32.175.175, Ethernet5, label 20030
 ST    1004179  [1], SR-TE Policy 10.0.0.179, color 100
                via SR-TE tunnel index 7, pop
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                    via TI-LFA tunnel index 3, label 20179
                       via 20.30.32.30, Ethernet1, label imp-null(3)
                       backup via 20.32.175.175, Ethernet5, label 20030
 ST    1004217  [1], SR-TE Policy 10.0.0.217, color 100
                via SR-TE tunnel index 13, pop
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                    via TI-LFA tunnel index 3, label 20217
                       via 20.30.32.30, Ethernet1, label imp-null(3)
                       backup via 20.32.175.175, Ethernet5, label 20030
 ST    1004221  [1], SR-TE Policy 10.0.0.221, color 100
                via SR-TE tunnel index 14, pop
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                    via TI-LFA tunnel index 3, label 21221
                       via 20.30.32.30, Ethernet1, label imp-null(3)
                       backup via 20.32.175.175, Ethernet5, label 20030
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
 * >      RD: 184:5001 IPv4 prefix 20.184.184.0/24
                                 10.0.0.184            -       0       0       i Or-ID: 194.0.0.1 C-LST: 10.0.0.30 
 * >      RD: 10.0.0.32:5001 IPv4 prefix 50.10.32.0/24
                                 -                     -       -       0       i
 * >Ec    RD: 53:5001 IPv4 prefix 50.10.53.0/24
                                 10.0.0.53             -       100     0       ? Or-ID: 10.0.0.53 C-LST: 10.0.0.30 
 *  ec    RD: 53:5001 IPv4 prefix 50.10.53.0/24
                                 10.0.0.53             -       100     0       ? Or-ID: 10.0.0.53 C-LST: 10.0.0.175 
 * >Ec    RD: 66:5001 IPv4 prefix 50.10.66.0/24
                                 10.0.0.66             -       100     0       ? Or-ID: 10.0.0.66 C-LST: 10.0.0.30 
 *  ec    RD: 66:5001 IPv4 prefix 50.10.66.0/24
                                 10.0.0.66             -       100     0       ? Or-ID: 10.0.0.66 C-LST: 10.0.0.175 
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
 * >      RD: 124:5001 IPv4 prefix 50.10.124.0/24
                                 10.0.0.124            0       100     0       ? Or-ID: 10.0.0.124 C-LST: 10.0.0.175 
 * >      RD: 128:5001 IPv4 prefix 50.10.128.0/24
                                 10.0.0.128            0       100     0       ? Or-ID: 10.0.0.128 C-LST: 10.0.0.175 
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
 * >      RD: 184:5001 IPv6 prefix 2001:0:184:184::/64
                                 ::ffff:10.0.0.184     -       0       0       i Or-ID: 194.0.0.1 C-LST: 10.0.0.30 
 * >      RD: 10.0.0.32:5001 IPv6 prefix 2600:50:10:32::/64
                                 -                     -       -       0       i
 * >Ec    RD: 53:5001 IPv6 prefix 2600:50:10:53::/64
                                 ::ffff:10.0.0.53      -       100     0       ? Or-ID: 10.0.0.53 C-LST: 10.0.0.30 
 *  ec    RD: 53:5001 IPv6 prefix 2600:50:10:53::/64
                                 ::ffff:10.0.0.53      -       100     0       ? Or-ID: 10.0.0.53 C-LST: 10.0.0.175 
 * >Ec    RD: 66:5001 IPv6 prefix 2600:50:10:66::/64
                                 ::ffff:10.0.0.66      -       100     0       ? Or-ID: 10.0.0.66 C-LST: 10.0.0.30 
 *  ec    RD: 66:5001 IPv6 prefix 2600:50:10:66::/64
                                 ::ffff:10.0.0.66      -       100     0       ? Or-ID: 10.0.0.66 C-LST: 10.0.0.175 
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
 * >      RD: 124:5001 IPv6 prefix 2600:50:10:124::/64
                                 ::ffff:10.0.0.124     0       100     0       ? Or-ID: 10.0.0.124 C-LST: 10.0.0.175 
 * >      RD: 128:5001 IPv6 prefix 2600:50:10:128::/64
                                 ::ffff:10.0.0.128     0       100     0       ? Or-ID: 10.0.0.128 C-LST: 10.0.0.175 
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
  Last read 00:00:41, last write 00:00:16
  Hold time is 180, keepalive interval is 60 seconds
  Configured hold time is 180, keepalive interval is 60 seconds
  Effective minimum hold time is 3 seconds
  Send failure hold time is 0 seconds
  Hold timer is active, time left: 00:02:19
  Keepalive timer is active, time left: 00:00:34
  Connect timer is inactive
  Idle-restart timer is inactive
  BGP state is Established, up for 22:51:34
  Number of transitions to established: 3
  Last state was OpenConfirm
  Last event was ReapplyOutboundPolicy
  Last sent notification:Hold Timer Expired Error/None, Last time 23:30:53, First time 1d00h, Repeats 1
  Last sent socket-error:Connect (Network is unreachable), Last time 23:18:38, First time 1d00h, Repeats 38
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
      Received 22:51:33
      Number of stale paths removed after graceful restart: 0
      Number of paths received before End-of-RIB: 9
    VPN-IPv6 End-of-RIB received: Yes
      Received 22:51:33
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
    Updates:                        44       725
    Keepalives:                   2960      2892
    Enhanced Route Refresh:          0         0
    Begin of Route Refresh:          0         0
    End of Route Refresh:            0         0
    Total messages:               3009      3620
  Prefix Statistics:
                                   Sent      Rcvd     Best Paths     Best ECMP Paths
    IPv4 Unicast:                     0         0              0                   0
    VPN-IPv4:                         1        12             12                  11
    IPv6 Unicast:                     0         0              0                   0
    VPN-IPv6:                         1        12             12                  11
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
    Round-trip Time (rtt/rtvar): 0.3ms/0.2ms
    Delayed Ack Timeout (ato): 40.0ms
    Congestion Window (cwnd): 2
    Slow-start Threshold (ssthresh): 7
    TCP Throughput: 67.15 Mbps
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
  Keepalive timer is active, time left: 00:00:04
  Connect timer is inactive
  Idle-restart timer is inactive
  BGP state is Established, up for 22:51:20
  Number of transitions to established: 11
  Last state was OpenConfirm
  Last event was ReapplyOutboundPolicy
  Last sent notification:Hold Timer Expired Error/None, Last time 23:02:12, First time 1d12h, Repeats 9
  Last sent socket-error:Connect (Network is unreachable), Last time 23:19:50, First time 1d12h, Repeats 25
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
      Received 22:51:19
      Number of stale paths removed after graceful restart: 0
      Number of paths received before End-of-RIB: 9
    VPN-IPv6 End-of-RIB received: Yes
      Received 22:51:19
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
    Updates:               66       677
    Keepalives:          5885      5286
    Route Refresh:          0         0
    Total messages:      5972      5974
  Prefix Statistics:
                                   Sent      Rcvd     Best Paths     Best ECMP Paths
    IPv4 Unicast:                     0         0              0                   0
    VPN-IPv4:                         1        13             13                   0
    IPv6 Unicast:                     0         0              0                   0
    VPN-IPv6:                         1        13             13                   0
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
    TCP Throughput: 245.94 Mbps
    Recv Round-trip Time (rcv_rtt): 384980.4ms
    Advertised Recv Window (rcv_space): 64345

```

## show tunnel rib system-tunnel-rib brief

```text
Tunnel RIB: system-tunnel-rib
Endpoint        Tunnel Type     Index(es)   Tunnel Preference   IGP Preference 
-------------- --------------- ----------- ------------------- ----------------
10.0.0.30/32    IS-IS SR IPv4   5           65                  115            
10.0.0.53/32    IS-IS SR IPv4   6           65                  115            
10.0.0.66/32    IS-IS SR IPv4   17          65                  115            
10.0.0.72/32    IS-IS SR IPv4   9           65                  115            
10.0.0.84/32    IS-IS SR IPv4   2           65                  115            
10.0.0.120/32   IS-IS SR IPv4   8           65                  115            
10.0.0.124/32   IS-IS SR IPv4   14          65                  115            
10.0.0.128/32   IS-IS SR IPv4   11          65                  115            
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
   30            metric     
   30            metric     
   20            metric     
   20            metric     
   20            metric     
   20            metric     
   10            metric     
   20            metric     
   35            metric     
   20            metric     
   20            metric     
   20            metric     

```

## show tunnel rib colored brief

```text
Tunnel RIB: system-colored-tunnel-rib
 Endpoint         Color    Tunnel Type     Index(es)    Tunnel Preference    IGP Preference    IGP Metric   Metric Type
---------------- -------- --------------- ------------ -------------------- ----------------- ------------- -----------
 10.0.0.66/32     100      SR-TE Policy    10           35                   3                 0            metric     
 10.0.0.72/32     100      SR-TE Policy    12           35                   3                 0            metric     
 10.0.0.120/32    100      SR-TE Policy    14           35                   3                 0            metric     
 10.0.0.124/32    100      SR-TE Policy    0            35                   3                 0            metric     
 10.0.0.128/32    100      SR-TE Policy    4            35                   3                 0            metric     
 10.0.0.156/32    100      SR-TE Policy    6            35                   3                 0            metric     
 10.0.0.179/32    100      SR-TE Policy    16           35                   3                 0            metric     
 10.0.0.217/32    100      SR-TE Policy    8            35                   3                 0            metric     
 10.0.0.221/32    100      SR-TE Policy    2            35                   3                 0            metric     

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
>C    10.0.0.32/32 [0 pref/0 metric] updated 1d19h ago
         via Loopback0, directly connected
>C    20.30.32.0/24 [0 pref/0 metric] updated 23:18:49 ago
         via Ethernet1, directly connected
>C    20.32.175.0/24 [0 pref/0 metric] updated 1d00h ago
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
>P    0.0.0.0/8 [1 pref/0 metric] updated 2d02h ago
         via Null0, directly connected [NF]
>P    127.0.0.0/8 [1 pref/0 metric] updated 2d02h ago
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
>I    10.0.0.30/32 [115 pref/10 metric] updated 19:54:30 ago
         via 20.30.32.30, Ethernet1
>I    10.0.0.53/32 [115 pref/20 metric] updated 00:58:00 ago
         via 20.30.32.30, Ethernet1
>I    10.0.0.66/32 [115 pref/30 metric] updated 15:42:40 ago
         via 20.30.32.30, Ethernet1
>I    10.0.0.72/32 [115 pref/30 metric] updated 17:51:46 ago
         via 20.30.32.30, Ethernet1
>I    10.0.0.84/32 [115 pref/30 metric] updated 18:20:13 ago
         via 20.30.32.30, Ethernet1
>I    10.0.0.120/32 [115 pref/20 metric] updated 18:20:13 ago
         via 20.30.32.30, Ethernet1
>I    10.0.0.124/32 [115 pref/20 metric] updated 18:20:13 ago
         via 20.30.32.30, Ethernet1
>I    10.0.0.128/32 [115 pref/20 metric] updated 15:52:21 ago
         via 20.30.32.30, Ethernet1
>I    10.0.0.156/32 [115 pref/20 metric] updated 00:39:34 ago
         via 20.30.32.30, Ethernet1
         via 20.32.175.175, Ethernet5
>I    10.0.0.175/32 [115 pref/10 metric] updated 19:54:23 ago
         via 20.32.175.175, Ethernet5
>I    10.0.0.179/32 [115 pref/20 metric] updated 18:20:13 ago
         via 20.30.32.30, Ethernet1
>I    10.0.0.184/32 [115 pref/35 metric] updated 00:00:02 ago
         via 20.32.175.175, Ethernet5
>I    10.0.0.214/32 [115 pref/20 metric] updated 18:20:13 ago
         via 20.30.32.30, Ethernet1
>I    10.0.0.217/32 [115 pref/20 metric] updated 18:20:13 ago
         via 20.30.32.30, Ethernet1
>I    10.0.0.221/32 [115 pref/20 metric] updated 18:20:13 ago
         via 20.30.32.30, Ethernet1
>I    20.30.53.0/24 [115 pref/20 metric] updated 00:58:01 ago
         via 20.30.32.30, Ethernet1
>I    20.30.66.0/24 [115 pref/20 metric] updated 15:42:52 ago
         via 20.30.32.30, Ethernet1
>I    20.30.72.0/24 [115 pref/20 metric] updated 19:54:30 ago
         via 20.30.32.30, Ethernet1
>I    20.30.84.0/24 [115 pref/20 metric] updated 19:54:30 ago
         via 20.30.32.30, Ethernet1
>I    20.30.120.0/24 [115 pref/20 metric] updated 19:54:30 ago
         via 20.30.32.30, Ethernet1
>I    20.30.124.0/24 [115 pref/20 metric] updated 19:54:30 ago
         via 20.30.32.30, Ethernet1
>I    20.30.128.0/24 [115 pref/20 metric] updated 15:52:23 ago
         via 20.30.32.30, Ethernet1
>I    20.30.156.0/24 [115 pref/20 metric] updated 00:40:07 ago
         via 20.30.32.30, Ethernet1
>I    20.30.179.0/24 [115 pref/20 metric] updated 19:47:17 ago
         via 20.30.32.30, Ethernet1
>I    20.30.184.0/24 [115 pref/20 metric] updated 00:06:19 ago
         via 20.30.32.30, Ethernet1
>I    20.30.214.0/24 [115 pref/20 metric] updated 19:54:30 ago
         via 20.30.32.30, Ethernet1
>I    20.30.217.0/24 [115 pref/20 metric] updated 19:54:30 ago
         via 20.30.32.30, Ethernet1
>I    20.30.221.0/24 [115 pref/20 metric] updated 19:54:30 ago
         via 20.30.32.30, Ethernet1
>I    20.53.175.0/24 [115 pref/25 metric] updated 00:58:06 ago
         via 20.32.175.175, Ethernet5
>I    20.66.175.0/24 [115 pref/25 metric] updated 15:42:57 ago
         via 20.32.175.175, Ethernet5
>I    20.72.175.0/24 [115 pref/25 metric] updated 17:26:11 ago
         via 20.32.175.175, Ethernet5
>I    20.84.175.0/24 [115 pref/25 metric] updated 17:26:11 ago
         via 20.32.175.175, Ethernet5
>I    20.120.175.0/24 [115 pref/25 metric] updated 17:26:11 ago
         via 20.32.175.175, Ethernet5
>I    20.120.214.0/24 [115 pref/30 metric] updated 18:20:13 ago
         via 20.30.32.30, Ethernet1
>I    20.124.175.0/24 [115 pref/25 metric] updated 17:26:11 ago
         via 20.32.175.175, Ethernet5
>I    20.128.175.0/24 [115 pref/25 metric] updated 17:26:11 ago
         via 20.32.175.175, Ethernet5
>I    20.131.175.0/24 [115 pref/25 metric] updated 17:26:11 ago
         via 20.32.175.175, Ethernet5
>I    20.156.175.0/24 [115 pref/20 metric] updated 00:40:12 ago
         via 20.32.175.175, Ethernet5
>I    20.175.179.0/24 [115 pref/25 metric] updated 17:26:11 ago
         via 20.32.175.175, Ethernet5
>I    20.175.184.0/24 [115 pref/25 metric] updated 00:06:31 ago
         via 20.32.175.175, Ethernet5
>I    20.175.214.0/24 [115 pref/25 metric] updated 17:26:11 ago
         via 20.32.175.175, Ethernet5
>I    20.175.217.0/24 [115 pref/25 metric] updated 17:26:11 ago
         via 20.32.175.175, Ethernet5
>I    20.175.221.0/24 [115 pref/25 metric] updated 17:26:11 ago
         via 20.32.175.175, Ethernet5
>I    20.214.216.0/24 [115 pref/30 metric] updated 18:20:13 ago
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
>C    2001:0:30:32::/64 [0 pref/0 metric] updated 23:18:49 ago
         via Ethernet1, directly connected
>C    2001:0:32:175::/64 [0 pref/0 metric] updated 22:24:27 ago
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
>P    ::/96 [1 pref/0 metric] updated 23:18:49 ago
         via Null0, directly connected [NF]
>P    ::ffff:127.0.0.0/104 [1 pref/0 metric] updated 23:18:49 ago
         via :: [1 pref/1 metric] type ipv6
            via , directly connected
>P    fe80::/10 [1 pref/0 metric] updated 23:18:49 ago
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
>I    2001:0:30:66::/64 [115 pref/20 metric] updated 15:42:52 ago
         via fe80::c6ca:2bff:fe45:a215, Ethernet1
>I    2001:0:30:72::/64 [115 pref/20 metric] updated 19:54:30 ago
         via fe80::c6ca:2bff:fe45:a215, Ethernet1
>I    2001:0:30:84::/64 [115 pref/20 metric] updated 19:54:30 ago
         via fe80::c6ca:2bff:fe45:a215, Ethernet1
>I    2001:0:30:120::/64 [115 pref/20 metric] updated 19:54:30 ago
         via fe80::c6ca:2bff:fe45:a215, Ethernet1
>I    2001:0:30:124::/64 [115 pref/20 metric] updated 19:54:30 ago
         via fe80::c6ca:2bff:fe45:a215, Ethernet1
>I    2001:0:30:128::/64 [115 pref/20 metric] updated 15:52:23 ago
         via fe80::c6ca:2bff:fe45:a215, Ethernet1
>I    2001:0:30:156::/64 [115 pref/20 metric] updated 00:40:07 ago
         via fe80::c6ca:2bff:fe45:a215, Ethernet1
>I    2001:0:30:179::/64 [115 pref/20 metric] updated 19:47:17 ago
         via fe80::c6ca:2bff:fe45:a215, Ethernet1
>I    2001:0:30:184::/64 [115 pref/20 metric] updated 00:06:19 ago
         via fe80::c6ca:2bff:fe45:a215, Ethernet1
>I    2001:0:30:214::/64 [115 pref/20 metric] updated 19:54:30 ago
         via fe80::c6ca:2bff:fe45:a215, Ethernet1
>I    2001:0:30:217::/64 [115 pref/20 metric] updated 19:54:30 ago
         via fe80::c6ca:2bff:fe45:a215, Ethernet1
>I    2001:0:30:221::/64 [115 pref/20 metric] updated 19:54:30 ago
         via fe80::c6ca:2bff:fe45:a215, Ethernet1
>I    2001:0:53:120::/64 [115 pref/20 metric] updated 00:58:01 ago
         via fe80::c6ca:2bff:fe45:a215, Ethernet1
>I    2001:0:84:175::/64 [115 pref/30 metric] updated 19:54:30 ago
         via fe80::c6ca:2bff:fe45:a215, Ethernet1
>I    2001:0:120:175::/64 [115 pref/30 metric] updated 18:43:53 ago
         via fe80::c6ca:2bff:fe45:a215, Ethernet1
>I    2001:0:120:214::/64 [115 pref/30 metric] updated 18:43:53 ago
         via fe80::c6ca:2bff:fe45:a215, Ethernet1
```

## show platform sand l3 summary

```text
Number of vrfs: 3

Ipv4:
  Routes:       87   backlog:  0  unprogrammed:  0
  Adjacencies:  105  backlog:  0  unprogrammed:  0
Ipv6:
  Routes:       45   backlog:  0  unprogrammed:  0
  Adjacencies:  105  backlog:  0  unprogrammed:  0
Mpls:
  Routes:       27  backlog:  0  unprogrammed:  0
  Adjacencies:  3   backlog:  0  unprogrammed:  0

Jericho2 Ip Fecs:
  Non-ecmp fecs:  4171  ecmp fecs:  2  fec entries:  4175
Jericho2 Mpls Fecs:
  Non-ecmp fecs:  3  ecmp fecs:  0  fec entries:  3
Jericho2 Vxlan Tunnel Fecs:
  Non-ecmp fecs:  0  ecmp fecs:  0  fec entries:  0
  Number of vxlan tunnels configured: 0

Jericho2 Lpm Routes:
  Routes:   87  unprogrammed:   0   
  Routes6:  45  unprogrammed6:  0   
  Backlog:  0 

Jericho2 Lpm:
  TCAM entries used:   4   Percent free:  99  ADS2 entries used:   5  Percent free:  99
  Pivot buckets used:  6   Rows used:     2   Entries Per Bucket:  0  Percent free:  99
  Route buckets used:  27  Rows used:     3   Entries Per Bucket:  4  Percent free:  99

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
  FixedSystem: 28
Egress Sflow rewrite entries in use (in each fap):
  FixedSystem: 0

Egress rewrite chains in backlog: resource-full 0, no-interface 0

Glem entries used per fap :
  FixedSystem: 4148

Jericho2 Fec:
  Maximum FEC hierarchy levels:  2
  ReusedEcmp:  0  allocs:  2592  frees:  2515  shuffles:  0  cmds:  0
  Zombies:     0    purges:    0
  Quarantine:  0/0  shuffles:  0  deletes:  0   
  Preserved FECs: 0
    First FEC preserved: never
    Last FEC preserved: never
  Fec insertion failures:  0
  Level1  Fecs:
    Non-ecmp fecs:            35  ecmp fecs:            1 
    Non-ecmp (Percent free):  99  ecmp (Percent free):  99
  Level2  Fecs:
    Non-ecmp fecs:            44  ecmp fecs:            2 
    Non-ecmp (Percent free):  99  ecmp (Percent free):  99
  Level3  Fecs:
    Non-ecmp fecs:            0    ecmp fecs:            0  
    Non-ecmp (Percent free):  100  ecmp (Percent free):  100

Lpm Detail:
  Requests:  4272  cleanses:  1972  batches:  1972  avg batch size:  2

Jericho Arp:
  ArpTable writes:      50741  queued      0   
  IngressTable writes:  94174  queued      0   
  Coprocessors:         1      in CmdRing

Tunnel Counter Status
  Number of MPLS tunnels:                  48   
  Number of uncountable MPLS tunnels:      22   
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
|0  |10.0.0.66/32      |ROUTE| Et1                |1006 |107517  | c4:ca:2b:45:a2:15 |  -  |288369|   -   
|0  |10.0.0.72/32      |ROUTE| Et1                |1006 |107517  | c4:ca:2b:45:a2:15 |  -  |288369|   -   
|0  |10.0.0.84/32      |ROUTE| Et1                |1006 |107517  | c4:ca:2b:45:a2:15 |  -  |288369|   -   
|0  |10.0.0.120/32     |ROUTE| Et1                |1006 |107517  | c4:ca:2b:45:a2:15 |  -  |288369|   -   
|0  |10.0.0.124/32     |ROUTE| Et1                |1006 |107517  | c4:ca:2b:45:a2:15 |  -  |288369|   -   
|0  |10.0.0.128/32     |ROUTE| Et1                |1006 |107517  | c4:ca:2b:45:a2:15 |  -  |288369|   -   
|0  |10.0.0.156/32     |ROUTE| Et5                |1010 |107518  | 3c:08:cd:8d:ba:dc |16384|288383|   -   
|0  |10.0.0.156/32     |ROUTE| Et1                |1006 |107517  | c4:ca:2b:45:a2:15 |16384|288384|   -   
|0  |10.0.0.175/32     |ROUTE| Et5                |1010 |107518  | 3c:08:cd:8d:ba:dc |  -  |288374|   -   
|0  |10.0.0.179/32     |ROUTE| Et1                |1006 |107517  | c4:ca:2b:45:a2:15 |  -  |288369|   -   
|0  |10.0.0.184/32     |ROUTE| Et5                |1010 |107518  | 3c:08:cd:8d:ba:dc |  -  |288374|   -   
|0  |10.0.0.214/32     |ROUTE| Et1                |1006 |107517  | c4:ca:2b:45:a2:15 |  -  |288369|   -   
|0  |10.0.0.217/32     |ROUTE| Et1                |1006 |107517  | c4:ca:2b:45:a2:15 |  -  |288369|   -   
|0  |10.0.0.221/32     |ROUTE| Et1                |1006 |107517  | c4:ca:2b:45:a2:15 |  -  |288369|   -   
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
|0  |20.53.175.0/24    |ROUTE| Et5                |1010 |107518  | 3c:08:cd:8d:ba:dc |  -  |288374|   -   
|0  |20.66.175.0/24    |ROUTE| Et5                |1010 |107518  | 3c:08:cd:8d:ba:dc |  -  |288374|   -   
|0  |20.72.175.0/24    |ROUTE| Et5                |1010 |107518  | 3c:08:cd:8d:ba:dc |  -  |288374|   -   
|0  |20.84.175.0/24    |ROUTE| Et5                |1010 |107518  | 3c:08:cd:8d:ba:dc |  -  |288374|   -   
|0  |20.120.175.0/24   |ROUTE| Et5                |1010 |107518  | 3c:08:cd:8d:ba:dc |  -  |288374|   -   
|0  |20.120.214.0/24   |ROUTE| Et1                |1006 |107517  | c4:ca:2b:45:a2:15 |  -  |288369|   -   
|0  |20.124.175.0/24   |ROUTE| Et5                |1010 |107518  | 3c:08:cd:8d:ba:dc |  -  |288374|   -   
|0  |20.128.175.0/24   |ROUTE| Et5                |1010 |107518  | 3c:08:cd:8d:ba:dc |  -  |288374|   -   
|0  |20.131.175.0/24   |ROUTE| Et5                |1010 |107518  | 3c:08:cd:8d:ba:dc |  -  |288374|   -   
|0  |20.156.175.0/24   |ROUTE| Et5                |1010 |107518  | 3c:08:cd:8d:ba:dc |  -  |288374|   -   
|0  |20.175.179.0/24   |ROUTE| Et5                |1010 |107518  | 3c:08:cd:8d:ba:dc |  -  |288374|   -   
|0  |20.175.184.0/24   |ROUTE| Et5                |1010 |107518  | 3c:08:cd:8d:ba:dc |  -  |288374|   -   
|0  |20.175.214.0/24   |ROUTE| Et5                |1010 |107518  | 3c:08:cd:8d:ba:dc |  -  |288374|   -   
|0  |20.175.217.0/24   |ROUTE| Et5                |1010 |107518  | 3c:08:cd:8d:ba:dc |  -  |288374|   -   
|0  |20.175.221.0/24   |ROUTE| Et5                |1010 |107518  | 3c:08:cd:8d:ba:dc |  -  |288374|   -   
|0  |20.214.216.0/24   |ROUTE| Et1                |1006 |107517  | c4:ca:2b:45:a2:15 |  -  |288369|   -   
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
|2  |50.10.32.2/32     |ROUTE| Et40               |1008 |107520  | 00:28:01:00:00:01 |  -  |288388|   -   
|2  |50.10.32.255/32   |TRAP | CoppSystemIpBcast  |0    |  -     | BcastReceive      |  -  |524290|   -   
|2  |50.10.32.0/24     |TRAP | CoppSystemL3DstMiss|1008 |1008    | ArpTrap           |  -  |525303|   -   
|2  |50.10.53.0/24     |ROUTE| FEC 288380         |0    |2097151 | 00:00:00:00:00:00 |  -  |157300|M 970000
|2  |50.10.66.0/24     |ROUTE| FEC 288381         |0    |2097141 | 00:00:00:00:00:00 |  -  |157311|M 62000
|2  |50.10.72.0/24     |ROUTE| FEC 288379         |0    |2097139 | 00:00:00:00:00:00 |  -  |157310|M 62002
|2  |50.10.84.0/24     |ROUTE| FEC 288371         |0    |2097142 | 00:00:00:00:00:00 |  -  |157319|M 720896
|2  |50.10.120.0/24    |ROUTE| FEC 288396         |0    |2097140 | 00:00:00:00:00:00 |  -  |157302|M 1277
|2  |50.10.124.0/24    |ROUTE| FEC 288382         |0    |2097125 | 00:00:00:00:00:00 |  -  |157301|M 332
|2  |50.10.128.0/24    |ROUTE| FEC 288397         |0    |2097126 | 00:00:00:00:00:00 |  -  |157303|M 48060
|2  |50.10.156.0/24    |ROUTE| FEC 16385          |0    |2097147 | 00:00:00:00:00:00 |  -  |157315|M 20156 16
|2  |50.10.179.0/24    |ROUTE| FEC 288373         |0    |2097127 | 00:00:00:00:00:00 |  -  |157294|M 16
|2  |50.10.214.0/24    |ROUTE| FEC 288401         |0    |2097149 | 00:00:00:00:00:00 |  -  |157305|M 500000
|2  |50.10.217.0/24    |ROUTE| FEC 288403         |0    |2097129 | 00:00:00:00:00:00 |  -  |157306|M 524287
|2  |50.10.221.0/24    |ROUTE| FEC 288392         |0    |2097124 | 00:00:00:00:00:00 |  -  |157304|M 524305
|2  |51.10.120.0/24    |ROUTE| FEC 288396         |0    |2097140 | 00:00:00:00:00:00 |  -  |157302|M 1277
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
|16384|288383|ROUTE| Et5                |1010 |107518  | 3c:08:cd:8d:ba:dc |   -   
|16384|288384|ROUTE| Et1                |1006 |107517  | c4:ca:2b:45:a2:15 |   -   
|16385|288394|ROUTE| Et5                |1010 |107518  | 3c:08:cd:8d:ba:dc |   -   
|16385|288395|ROUTE| Et1                |1006 |107517  | c4:ca:2b:45:a2:15 |   -   
|  -  |157288|ROUTE| FEC 288381         |   - |  -     |                   |   -   
|  -  |157289|ROUTE| FEC 288379         |   - |  -     |                   |   -   
|  -  |157290|ROUTE| FEC 288396         |   - |  -     |                   |   -   
|  -  |157291|ROUTE| FEC 288405         |   - |2097133 |                 - |Mpush 16
|  -  |157292|ROUTE| FEC 288405         |   - |2097133 |                 - |Mpush 16
|  -  |157293|ROUTE| FEC 288400         |   - |  -     |                   |   -   
|  -  |157294|ROUTE| FEC 288373         |   - |2097127 |                 - |Mpush 16
|  -  |157295|ROUTE| FEC 288378         |   - |2097138 |                 - |Mpush 16
|  -  |157299|ROUTE| FEC 288382         |   - |  -     |                   |   -   
|  -  |157300|ROUTE| FEC 288380         |   - |2097151 |                 - |Mpush 970000
|  -  |157301|ROUTE| FEC 288382         |   - |2097125 |                 - |Mpush 332
|  -  |157302|ROUTE| FEC 288396         |   - |2097140 |                 - |Mpush 1277
|  -  |157303|ROUTE| FEC 288397         |   - |2097126 |                 - |Mpush 48060
|  -  |157304|ROUTE| FEC 288392         |   - |2097124 |                 - |Mpush 524305
|  -  |157305|ROUTE| FEC 288401         |   - |2097149 |                 - |Mpush 500000
|  -  |157306|ROUTE| FEC 288403         |   - |2097129 |                 - |Mpush 524287
|  -  |157307|ROUTE| FEC 288370         |   - |2097134 |                 - |Mpush 62001
|  -  |157308|ROUTE| FEC 288397         |   - |  -     |                   |   -   
|  -  |157309|ROUTE| FEC 288377         |   - |2097146 |                 - |Mpush 62003
|  -  |157310|ROUTE| FEC 288379         |   - |2097139 |                 - |Mpush 62002
|  -  |157311|ROUTE| FEC 288381         |   - |2097141 |                 - |Mpush 62000
|  -  |157312|ROUTE| FEC 288380         |   - |2097150 |                 - |Mpush 970001
|  -  |157313|ROUTE| FEC 288373         |   - |  -     |                   |   -   
|  -  |157314|ROUTE| FEC 288403         |   - |  -     |                   |   -   
|  -  |157315|ROUTE| FEC 16385          |   - |2097147 |                 - |Mpush 20156 16
|  -  |157316|ROUTE| FEC 16385          |   - |2097147 |                 - |Mpush 20156 16
|  -  |157317|ROUTE| FEC 288392         |   - |  -     |                   |   -   
|  -  |157318|ROUTE| FEC 288371         |   - |2097143 |                 - |Mpush 720897
|  -  |157319|ROUTE| FEC 288371         |   - |2097142 |                 - |Mpush 720896
|  -  |157320|ROUTE| FEC 288398         |   - |2097135 |                 - |Mpush 48061
|  -  |157321|ROUTE| FEC 288401         |   - |2097149 |                 - |Mpush 500000
|  -  |157322|ROUTE| FEC 288389         |   - |2097145 |                 - |Mpush 333
|  -  |157323|ROUTE| FEC 288391         |   - |2097132 |                 - |Mpush 524287
|  -  |157324|ROUTE| FEC 288386         |   - |2097137 |                 - |Mpush 524305
|  -  |157325|ROUTE| FEC 288387         |   - |2097144 |                 - |Mpush 1276
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
|  -  |288370|ROUTE| Et1                |1006 |107524  | c4:ca:2b:45:a2:15 |Mpush 20066
|  -  |288371|ROUTE| Et1                |1006 |107531  | c4:ca:2b:45:a2:15 |Mpush 20084
|  -  |288372|ROUTE| Et1                |1006 |107529  | c4:ca:2b:45:a2:15 |   -   
|  -  |288373|ROUTE| Et1                |1006 |107546  | c4:ca:2b:45:a2:15 |Mpush 20179
|  -  |288374|ROUTE| Et5                |1010 |107518  | 3c:08:cd:8d:ba:dc |   -   
|  -  |288375|ROUTE| Et5                |1010 |107518  | 3c:08:cd:8d:ba:dc |   -   
|  -  |288376|DROP | DROP               |0    |  -     |                   |   -   
|  -  |288377|ROUTE| Et1                |1006 |107523  | c4:ca:2b:45:a2:15 |Mpush 20072
|  -  |288378|ROUTE| Et1                |1006 |107521  | c4:ca:2b:45:a2:15 |Mpush 20179
|  -  |288379|ROUTE| Et1                |1006 |107543  | c4:ca:2b:45:a2:15 |Mpush 20072
|  -  |288380|ROUTE| Et1                |1006 |107525  | c4:ca:2b:45:a2:15 |Mpush 20053
|  -  |288381|ROUTE| Et1                |1006 |107530  | c4:ca:2b:45:a2:15 |Mpush 20066
|  -  |288382|ROUTE| Et1                |1006 |107551  | c4:ca:2b:45:a2:15 |Mpush 20124
|  -  |288385|ROUTE| Et40               |1009 |107522  | 00:29:01:00:00:01 |   -   
|  -  |288386|ROUTE| Et1                |1006 |107534  | c4:ca:2b:45:a2:15 |Mpush 21221
|  -  |288387|ROUTE| Et1                |1006 |107528  | c4:ca:2b:45:a2:15 |Mpush 20120
|  -  |288388|ROUTE| Et40               |1008 |107520  | 00:28:01:00:00:01 |   -   
|  -  |288389|ROUTE| Et1                |1006 |107535  | c4:ca:2b:45:a2:15 |Mpush 20124
|  -  |288391|ROUTE| Et1                |1006 |107538  | c4:ca:2b:45:a2:15 |Mpush 20217
|  -  |288392|ROUTE| Et1                |1006 |107556  | c4:ca:2b:45:a2:15 |Mpush 21221
|  -  |288393|ROUTE| Et5                |1010 |107540  | 3c:08:cd:8d:ba:dc |   -   
|  -  |288396|ROUTE| Et1                |1006 |107536  | c4:ca:2b:45:a2:15 |Mpush 20120
|  -  |288397|ROUTE| Et1                |1006 |107549  | c4:ca:2b:45:a2:15 |Mpush 20128
|  -  |288398|ROUTE| Et1                |1006 |107519  | c4:ca:2b:45:a2:15 |Mpush 20128
|  -  |288400|ROUTE| Et1                |1006 |107539  | c4:ca:2b:45:a2:15 |Mpush 20156
|  -  |288401|ROUTE| Et1                |1006 |107533  | c4:ca:2b:45:a2:15 |Mpush 20214
|  -  |288402|ROUTE| Et1                |1006 |107526  | c4:ca:2b:45:a2:15 |   -   
|  -  |288403|ROUTE| Et1                |1006 |107544  | c4:ca:2b:45:a2:15 |Mpush 20217
|  -  |288405|ROUTE| Et1                |1006 |107537  | c4:ca:2b:45:a2:15 |Mpush 20484
|  -  |524290|TRAP | CoppSystemIpBcast  |0    |  -     | BcastReceive      |   -   
|  -  |524291|TRAP | CoppSystemIpUcast  |0    |  -     | Receive           |   -   
|  -  |524293|TRAP | CoppSystemL3LpmOver|0    |  -     | SlowReceive       |   -   
|  -  |524295|TRAP | CoppSystemL3DstMiss|0    |  -     | ArpTrap           |   -   
|  -  |525301|TRAP | CoppSystemL3DstMiss|1006 |1006    | ArpTrap           |   -   
|  -  |525303|TRAP | CoppSystemL3DstMiss|1008 |1008    | ArpTrap           |   -   
|  -  |525304|TRAP | CoppSystemL3DstMiss|1009 |1009    | ArpTrap           |   -   
|  -  |525305|TRAP | CoppSystemL3DstMiss|1010 |1010    | ArpTrap           |   -   

```

