# Test results for PE31-Q2C-31

## show version

```text
Arista DCS-7280SR3-48YC8-F
Hardware version: 12.12
Serial number: HBG243203DT
Hardware MAC address: 68bf.6c35.1e31
System MAC address: 68bf.6c35.1e31

Software image version: 4.33.1.1F
Architecture: x86_64
Internal build version: 4.33.1.1F-40155285.43311F
Internal build ID: 2170da2c-90c5-421e-adc1-86266708cffc
Image format version: 3.0
Image optimization: Default

Uptime: 1 day, 2 hours and 9 minutes
Total memory: 8099700 kB
Free memory: 5045368 kB

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
Ethernet1        20.30.31.31/24       down       down            1500          
Ethernet5        20.31.175.31/24      up         up              1500          
Ethernet40.4     50.10.31.1/24        up         up              1500          
Loopback0        10.0.0.31/32         up         up             65535          
Management1      192.168.20.31/23     up         up              1500          

```

## show interfaces counters rates | nz

```text
Port      Name                Intvl  In Mbps      %  In Kpps Out Mbps      %

Port      Out Kpps
```

## show ip ospf neighbor detail

```text
Neighbor 10.0.0.175, instance 1, VRF default, interface address 20.31.175.175
  In area 0.0.0.0 interface Ethernet5
  Neighbor priority is 128, State is FULL, 6 state changes
  Adjacency was established 00:37:23 ago
  Current state was established 00:37:23 ago
  DR IP Address 0.0.0.0 BDR IP Address 0.0.0.0
  Options is E
  Dead timer is due in 00:00:34
  Inactivity timer deferred 0 times
  LSAs retransmitted 0 times to this neighbor
  Graceful-restart-helper mode is Inactive
  Graceful-restart attempts: 0
  Segment Routing enabled
    SRGB Base: 20000 Range: 2000
```

## show ip ospf database detail

```text

            OSPF Router with ID(10.0.0.31) (Instance ID 1) (VRF default)


                 Router Link States (Area 0.0.0.0)

  LS Age: 1513
  Options: (E)
  LS Type: Router Links
  Link State ID: 192.168.20.128
  Advertising Router: 192.168.20.128
  LS Seq Number: 0x80000006
  Checksum: 0xd80c
  Length: 60
  Number of Links: 3

    Link connected to: a Point-to-point Network
     (Link ID) Neighboring Router ID: 10.0.0.175
     (Link Data)  20.128.175.128
      Number of TOS metrics: 0
       TOS 0 Metrics: 1


    Link connected to: a Stub Network
     (Link ID) Network/subnet number: 20.128.175.0
     (Link Data) Network Mask: 255.255.255.0
      Number of TOS metrics: 0
       TOS 0 Metrics: 1


    Link connected to: a Stub Network
     (Link ID) Network/subnet number: 10.0.0.128
     (Link Data) Network Mask: 255.255.255.255
      Number of TOS metrics: 0
       TOS 0 Metrics: 0

  LS Age: 1634
  Options: ((null))
  LS Type: Router Links
  Link State ID: 100.0.0.184
  Advertising Router: 100.0.0.184
  LS Seq Number: 0x80000003
  Checksum: 0x289
  Length: 48
  Number of Links: 2

    Link connected to: a Point-to-point Network
     (Link ID) Neighboring Router ID: 10.0.0.175
     (Link Data)  20.175.184.184
      Number of TOS metrics: 0
       TOS 0 Metrics: 10


    Link connected to: a Stub Network
     (Link ID) Network/subnet number: 20.175.184.0
     (Link Data) Network Mask: 255.255.255.0
      Number of TOS metrics: 0
       TOS 0 Metrics: 10

  LS Age: 133
  Options: (E O)
  LS Type: Router Links
  Link State ID: 192.168.20.120
  Advertising Router: 192.168.20.120
  LS Seq Number: 0x8000000a
  Checksum: 0xce01
  Length: 60
  Number of Links: 3

    Link connected to: a Point-to-point Network
     (Link ID) Neighboring Router ID: 10.0.0.175
     (Link Data)  20.120.175.120
      Number of TOS metrics: 0
       TOS 0 Metrics: 1


    Link connected to: a Stub Network
     (Link ID) Network/subnet number: 10.0.0.120
     (Link Data) Network Mask: 255.255.255.255
      Number of TOS metrics: 0
       TOS 0 Metrics: 0


    Link connected to: a Stub Network
     (Link ID) Network/subnet number: 20.120.175.0
     (Link Data) Network Mask: 255.255.255.0
      Number of TOS metrics: 0
       TOS 0 Metrics: 1

  LS Age: 175
  Options: ((null))
  LS Type: Router Links
  Link State ID: 10.0.0.184
  Advertising Router: 10.0.0.184
  LS Seq Number: 0x8000000b
  Checksum: 0x95c
  Length: 60
  Number of Links: 3

    Link connected to: a Point-to-point Network
     (Link ID) Neighboring Router ID: 10.0.0.175
     (Link Data)  20.175.184.184
      Number of TOS metrics: 0
       TOS 0 Metrics: 10


    Link connected to: a Stub Network
     (Link ID) Network/subnet number: 20.175.184.0
     (Link Data) Network Mask: 255.255.255.0
      Number of TOS metrics: 0
       TOS 0 Metrics: 10


    Link connected to: a Stub Network
     (Link ID) Network/subnet number: 10.0.0.184
     (Link Data) Network Mask: 255.255.255.255
      Number of TOS metrics: 0
       TOS 0 Metrics: 0

  LS Age: 318
  Options: (E DC)
  LS Type: Router Links
  Link State ID: 10.0.0.66
  Advertising Router: 10.0.0.66
  LS Seq Number: 0x80000005
  Checksum: 0x2cd9
  Length: 60
  Number of Links: 3

    Link connected to: a Stub Network
     (Link ID) Network/subnet number: 10.0.0.66
     (Link Data) Network Mask: 255.255.255.255
      Number of TOS metrics: 0
       TOS 0 Metrics: 10


    Link connected to: a Point-to-point Network
     (Link ID) Neighboring Router ID: 10.0.0.175
     (Link Data)  20.66.175.66
      Number of TOS metrics: 0
       TOS 0 Metrics: 10


    Link connected to: a Stub Network
     (Link ID) Network/subnet number: 20.66.175.0
     (Link Data) Network Mask: 255.255.255.0
      Number of TOS metrics: 0
       TOS 0 Metrics: 10

  LS Age: 1500
  Options: (E)
  LS Type: Router Links
  Link State ID: 10.0.0.124
  Advertising Router: 10.0.0.124
  LS Seq Number: 0x80000006
  Checksum: 0x22c1
  Length: 60
  Number of Links: 3

    Link connected to: a Point-to-point Network
     (Link ID) Neighboring Router ID: 10.0.0.175
     (Link Data)  20.124.175.124
      Number of TOS metrics: 0
       TOS 0 Metrics: 1


    Link connected to: a Stub Network
     (Link ID) Network/subnet number: 20.124.175.0
     (Link Data) Network Mask: 255.255.255.0
      Number of TOS metrics: 0
       TOS 0 Metrics: 1


    Link connected to: a Stub Network
     (Link ID) Network/subnet number: 10.0.0.124
     (Link Data) Network Mask: 255.255.255.255
      Number of TOS metrics: 0
       TOS 0 Metrics: 0

  LS Age: 368
  Options: (E DC)
  LS Type: Router Links
  Link State ID: 10.0.0.32
  Advertising Router: 10.0.0.32
  LS Seq Number: 0x80000006
  Checksum: 0x8c9
  Length: 60
  Number of Links: 3

    Link connected to: a Stub Network
     (Link ID) Network/subnet number: 10.0.0.32
     (Link Data) Network Mask: 255.255.255.255
      Number of TOS metrics: 0
       TOS 0 Metrics: 10


    Link connected to: a Point-to-point Network
     (Link ID) Neighboring Router ID: 10.0.0.175
     (Link Data)  20.32.175.32
      Number of TOS metrics: 0
       TOS 0 Metrics: 10


    Link connected to: a Stub Network
     (Link ID) Network/subnet number: 20.32.175.0
     (Link Data) Network Mask: 255.255.255.0
      Number of TOS metrics: 0
       TOS 0 Metrics: 10

  LS Age: 365
  Options: (E DC)
  LS Type: Router Links
  Link State ID: 10.0.0.72
  Advertising Router: 10.0.0.72
  LS Seq Number: 0x80000005
  Checksum: 0xf5eb
  Length: 60
  Number of Links: 3

    Link connected to: a Stub Network
     (Link ID) Network/subnet number: 10.0.0.72
     (Link Data) Network Mask: 255.255.255.255
      Number of TOS metrics: 0
       TOS 0 Metrics: 10


    Link connected to: a Point-to-point Network
     (Link ID) Neighboring Router ID: 10.0.0.175
     (Link Data)  20.72.175.72
      Number of TOS metrics: 0
       TOS 0 Metrics: 10


    Link connected to: a Stub Network
     (Link ID) Network/subnet number: 20.72.175.0
     (Link Data) Network Mask: 255.255.255.0
      Number of TOS metrics: 0
       TOS 0 Metrics: 10

  LS Age: 196
  Options: (E DC)
  LS Type: Router Links
  Link State ID: 10.0.0.84
  Advertising Router: 10.0.0.84
  LS Seq Number: 0x80000006
  Checksum: 0x8dd1
  Length: 60
  Number of Links: 3

    Link connected to: a Stub Network
     (Link ID) Network/subnet number: 10.0.0.84
     (Link Data) Network Mask: 255.255.255.255
      Number of TOS metrics: 0
       TOS 0 Metrics: 1


    Link connected to: a Point-to-point Network
     (Link ID) Neighboring Router ID: 10.0.0.175
     (Link Data)  20.84.175.84
      Number of TOS metrics: 0
       TOS 0 Metrics: 1


    Link connected to: a Stub Network
     (Link ID) Network/subnet number: 20.84.175.84
     (Link Data) Network Mask: 255.255.255.0
      Number of TOS metrics: 0
       TOS 0 Metrics: 1

  LS Age: 1819
  Options: (E)
  LS Type: Router Links
  Link State ID: 10.0.0.214
  Advertising Router: 10.0.0.214
  LS Seq Number: 0x80000004
  Checksum: 0x4433
  Length: 60
  Number of Links: 3

    Link connected to: a Stub Network
     (Link ID) Network/subnet number: 10.0.0.214
     (Link Data) Network Mask: 255.255.255.255
      Number of TOS metrics: 0
       TOS 0 Metrics: 0


    Link connected to: a Point-to-point Network
     (Link ID) Neighboring Router ID: 10.0.0.175
     (Link Data)  20.175.214.214
      Number of TOS metrics: 0
       TOS 0 Metrics: 40


    Link connected to: a Stub Network
     (Link ID) Network/subnet number: 20.175.214.0
     (Link Data) Network Mask: 255.255.255.0
      Number of TOS metrics: 0
       TOS 0 Metrics: 40

  LS Age: 476
  Options: (E)
  LS Type: Router Links
  Link State ID: 10.0.0.221
  Advertising Router: 10.0.0.221
  LS Seq Number: 0x80000003
  Checksum: 0xeba0
  Length: 60
  Number of Links: 3

    Link connected to: a Stub Network
     (Link ID) Network/subnet number: 10.0.0.221
     (Link Data) Network Mask: 255.255.255.255
      Number of TOS metrics: 0
       TOS 0 Metrics: 0


    Link connected to: a Point-to-point Network
     (Link ID) Neighboring Router ID: 10.0.0.175
     (Link Data)  20.175.221.221
      Number of TOS metrics: 0
       TOS 0 Metrics: 10


    Link connected to: a Stub Network
     (Link ID) Network/subnet number: 20.175.221.0
     (Link Data) Network Mask: 255.255.255.0
      Number of TOS metrics: 0
       TOS 0 Metrics: 10

  LS Age: 577
  Options: (E)
  LS Type: Router Links
  Link State ID: 10.0.0.217
  Advertising Router: 10.0.0.217
  LS Seq Number: 0x80000006
  Checksum: 0xb2ec
  Length: 60
  Number of Links: 3

    Link connected to: a Stub Network
     (Link ID) Network/subnet number: 10.0.0.217
     (Link Data) Network Mask: 255.255.255.255
      Number of TOS metrics: 0
       TOS 0 Metrics: 0


    Link connected to: a Point-to-point Network
     (Link ID) Neighboring Router ID: 10.0.0.175
     (Link Data)  20.175.217.217
      Number of TOS metrics: 0
       TOS 0 Metrics: 10


    Link connected to: a Stub Network
     (Link ID) Network/subnet number: 20.175.217.0
     (Link Data) Network Mask: 255.255.255.0
      Number of TOS metrics: 0
       TOS 0 Metrics: 10

  LS Age: 495
  Options: (E DC)
  LS Type: Router Links
  Link State ID: 10.0.0.179
  Advertising Router: 10.0.0.179
  LS Seq Number: 0x80000004
  Checksum: 0x1a60
  Length: 60
  Number of Links: 3

    Link connected to: a Point-to-point Network
     (Link ID) Neighboring Router ID: 10.0.0.175
     (Link Data)  20.175.179.179
      Number of TOS metrics: 0
       TOS 0 Metrics: 1


    Link connected to: a Stub Network
     (Link ID) Network/subnet number: 20.175.179.0
     (Link Data) Network Mask: 255.255.255.0
      Number of TOS metrics: 0
       TOS 0 Metrics: 1


    Link connected to: a Stub Network
     (Link ID) Network/subnet number: 10.0.0.179
     (Link Data) Network Mask: 255.255.255.255
      Number of TOS metrics: 0
       TOS 0 Metrics: 0

  LS Age: 2023
  Options: (E DC)
  LS Type: Router Links
  Link State ID: 10.0.0.131
  Advertising Router: 10.0.0.131
  LS Seq Number: 0x80000002
  Checksum: 0xa93
  Length: 60
  Number of Links: 3

    Link connected to: a Point-to-point Network
     (Link ID) Neighboring Router ID: 10.0.0.175
     (Link Data)  20.131.175.131
      Number of TOS metrics: 0
       TOS 0 Metrics: 1


    Link connected to: a Stub Network
     (Link ID) Network/subnet number: 20.131.175.0
     (Link Data) Network Mask: 255.255.255.0
      Number of TOS metrics: 0
       TOS 0 Metrics: 1


    Link connected to: a Stub Network
     (Link ID) Network/subnet number: 10.0.0.131
     (Link Data) Network Mask: 255.255.255.255
      Number of TOS metrics: 0
       TOS 0 Metrics: 0

  LS Age: 174
  Options: (E DC)
  LS Type: Router Links
  Link State ID: 10.0.0.175
  Advertising Router: 10.0.0.175
  LS Seq Number: 0x80000029
  Checksum: 0x293a
  Length: 384
  Number of Links: 30

    Link connected to: a Point-to-point Network
     (Link ID) Neighboring Router ID: 10.0.0.131
     (Link Data)  20.131.175.175
      Number of TOS metrics: 0
       TOS 0 Metrics: 1


    Link connected to: a Stub Network
     (Link ID) Network/subnet number: 20.131.175.0
     (Link Data) Network Mask: 255.255.255.0
      Number of TOS metrics: 0
       TOS 0 Metrics: 1


    Link connected to: a Point-to-point Network
     (Link ID) Neighboring Router ID: 10.0.0.217
     (Link Data)  20.175.217.175
      Number of TOS metrics: 0
       TOS 0 Metrics: 1


    Link connected to: a Stub Network
     (Link ID) Network/subnet number: 20.175.217.0
     (Link Data) Network Mask: 255.255.255.0
      Number of TOS metrics: 0
       TOS 0 Metrics: 1


    Link connected to: a Point-to-point Network
     (Link ID) Neighboring Router ID: 10.0.0.221
     (Link Data)  20.175.221.175
      Number of TOS metrics: 0
       TOS 0 Metrics: 1


    Link connected to: a Stub Network
     (Link ID) Network/subnet number: 20.175.221.0
     (Link Data) Network Mask: 255.255.255.0
      Number of TOS metrics: 0
       TOS 0 Metrics: 1


    Link connected to: a Point-to-point Network
     (Link ID) Neighboring Router ID: 10.0.0.84
     (Link Data)  20.84.175.175
      Number of TOS metrics: 0
       TOS 0 Metrics: 1


    Link connected to: a Stub Network
     (Link ID) Network/subnet number: 20.84.175.0
     (Link Data) Network Mask: 255.255.255.0
      Number of TOS metrics: 0
       TOS 0 Metrics: 1


    Link connected to: a Point-to-point Network
     (Link ID) Neighboring Router ID: 192.168.20.128
     (Link Data)  20.128.175.175
      Number of TOS metrics: 0
       TOS 0 Metrics: 1


    Link connected to: a Stub Network
     (Link ID) Network/subnet number: 20.128.175.0
     (Link Data) Network Mask: 255.255.255.0
      Number of TOS metrics: 0
       TOS 0 Metrics: 1


    Link connected to: a Point-to-point Network
     (Link ID) Neighboring Router ID: 10.0.0.184
     (Link Data)  20.175.184.175
      Number of TOS metrics: 0
       TOS 0 Metrics: 1


    Link connected to: a Stub Network
     (Link ID) Network/subnet number: 20.175.184.0
     (Link Data) Network Mask: 255.255.255.0
      Number of TOS metrics: 0
       TOS 0 Metrics: 1


    Link connected to: a Point-to-point Network
     (Link ID) Neighboring Router ID: 10.0.0.124
     (Link Data)  20.124.175.175
      Number of TOS metrics: 0
       TOS 0 Metrics: 1


    Link connected to: a Stub Network
     (Link ID) Network/subnet number: 20.124.175.0
     (Link Data) Network Mask: 255.255.255.0
      Number of TOS metrics: 0
       TOS 0 Metrics: 1


    Link connected to: a Point-to-point Network
     (Link ID) Neighboring Router ID: 10.0.0.214
     (Link Data)  20.175.214.175
      Number of TOS metrics: 0
       TOS 0 Metrics: 1


    Link connected to: a Stub Network
     (Link ID) Network/subnet number: 20.175.214.0
     (Link Data) Network Mask: 255.255.255.0
      Number of TOS metrics: 0
       TOS 0 Metrics: 1


    Link connected to: a Point-to-point Network
     (Link ID) Neighboring Router ID: 10.0.0.32
     (Link Data)  20.32.175.175
      Number of TOS metrics: 0
       TOS 0 Metrics: 1


    Link connected to: a Stub Network
     (Link ID) Network/subnet number: 20.32.175.0
     (Link Data) Network Mask: 255.255.255.0
      Number of TOS metrics: 0
       TOS 0 Metrics: 1


    Link connected to: a Point-to-point Network
     (Link ID) Neighboring Router ID: 10.0.0.72
     (Link Data)  20.72.175.175
      Number of TOS metrics: 0
       TOS 0 Metrics: 1


    Link connected to: a Stub Network
     (Link ID) Network/subnet number: 20.72.175.0
     (Link Data) Network Mask: 255.255.255.0
      Number of TOS metrics: 0
       TOS 0 Metrics: 1


    Link connected to: a Point-to-point Network
     (Link ID) Neighboring Router ID: 10.0.0.66
     (Link Data)  20.66.175.175
      Number of TOS metrics: 0
       TOS 0 Metrics: 1


    Link connected to: a Stub Network
     (Link ID) Network/subnet number: 20.66.175.0
     (Link Data) Network Mask: 255.255.255.0
      Number of TOS metrics: 0
       TOS 0 Metrics: 1


    Link connected to: a Point-to-point Network
     (Link ID) Neighboring Router ID: 10.0.0.179
     (Link Data)  20.175.179.175
      Number of TOS metrics: 0
       TOS 0 Metrics: 1


    Link connected to: a Stub Network
     (Link ID) Network/subnet number: 20.175.179.0
     (Link Data) Network Mask: 255.255.255.0
      Number of TOS metrics: 0
       TOS 0 Metrics: 1


    Link connected to: a Point-to-point Network
     (Link ID) Neighboring Router ID: 10.0.0.31
     (Link Data)  20.31.175.175
      Number of TOS metrics: 0
       TOS 0 Metrics: 1


    Link connected to: a Stub Network
     (Link ID) Network/subnet number: 20.31.175.0
     (Link Data) Network Mask: 255.255.255.0
      Number of TOS metrics: 0
       TOS 0 Metrics: 1


    Link connected to: a Point-to-point Network
     (Link ID) Neighboring Router ID: 192.168.20.120
     (Link Data)  20.120.175.175
      Number of TOS metrics: 0
       TOS 0 Metrics: 1


    Link connected to: a Stub Network
     (Link ID) Network/subnet number: 20.120.175.0
     (Link Data) Network Mask: 255.255.255.0
      Number of TOS metrics: 0
       TOS 0 Metrics: 1


    Link connected to: a Stub Network
     (Link ID) Network/subnet number: 20.53.175.0
     (Link Data) Network Mask: 255.255.255.0
      Number of TOS metrics: 0
       TOS 0 Metrics: 1


    Link connected to: a Stub Network
     (Link ID) Network/subnet number: 10.0.0.175
     (Link Data) Network Mask: 255.255.255.255
      Number of TOS metrics: 0
       TOS 0 Metrics: 0

  LS Age: 436
  Options: (E DC)
  LS Type: Router Links
  Link State ID: 10.0.0.31
  Advertising Router: 10.0.0.31
  LS Seq Number: 0x80000006
  Checksum: 0xbb1c
  Length: 60
  Number of Links: 3

    Link connected to: a Stub Network
     (Link ID) Network/subnet number: 10.0.0.31
     (Link Data) Network Mask: 255.255.255.255
      Number of TOS metrics: 0
       TOS 0 Metrics: 10


    Link connected to: a Point-to-point Network
     (Link ID) Neighboring Router ID: 10.0.0.175
     (Link Data)  20.31.175.31
      Number of TOS metrics: 0
       TOS 0 Metrics: 10


    Link connected to: a Stub Network
     (Link ID) Network/subnet number: 20.31.175.0
     (Link Data) Network Mask: 255.255.255.0
      Number of TOS metrics: 0
       TOS 0 Metrics: 10


                 Opaque Type 10 Link States (Area 0.0.0.0)

  LS Age: 436
  Options: (DC O)
  LS Type: Opaque Type 10 Links
  Link State ID: 7.0.0.0
  Advertising Router: 10.0.0.31
  LS Seq Number: 0x80000002
  Checksum: 0x32bb
  Length: 44
  Segment Routing Extended Prefix TLV
    Route Type: Intra-Area, Prefix: 10.0.0.31/32, AF: IPv4 unicast
    Flags:  [N]
    Prefix-SID Sub-TLV
      Algorithm: Shortest Path First
      Flags:  []
      MT-ID: 0, SID: 31

  LS Age: 1358
  Options: (E DC)
  LS Type: Opaque Type 10 Links
  Link State ID: 8.0.0.1
  Advertising Router: 10.0.0.175
  LS Seq Number: 0x80000002
  Checksum: 0xa8d1
  Length: 48
  Segment Routing Extended Link TLV
    Link Type: 1 (Point-to-point)
    Reserved: 0
    Link Id: 10.0.0.221
    Link Data: 20.175.221.175
    Adj-SID Sub-TLV
      Flags: [V, L]
      Reserved: 0
      Multi-Topology ID: 0
      SID: 38

  LS Age: 225
  Options: (E DC)
  LS Type: Opaque Type 10 Links
  Link State ID: 8.255.216.246
  Advertising Router: 10.0.0.72
  LS Seq Number: 0x80000002
  Checksum: 0x51a
  Length: 48
  Segment Routing Extended Link TLV
    Link Type: 1 (Point-to-point)
    Reserved: 0
    Link Id: 10.0.0.175
    Link Data: 20.72.175.72
    Adj-SID Sub-TLV
      Flags: [V, L]
      Reserved: 0
      Multi-Topology ID: 0
      SID: 22000

  LS Age: 648
  Options: (E DC)
  LS Type: Opaque Type 10 Links
  Link State ID: 8.0.0.10
  Advertising Router: 10.0.0.175
  LS Seq Number: 0x80000002
  Checksum: 0x474f
  Length: 48
  Segment Routing Extended Link TLV
    Link Type: 1 (Point-to-point)
    Reserved: 0
    Link Id: 10.0.0.72
    Link Data: 20.72.175.175
    Adj-SID Sub-TLV
      Flags: [V, L]
      Reserved: 0
      Multi-Topology ID: 0
      SID: 44

  LS Age: 436
  Options: (DC O)
  LS Type: Opaque Type 10 Links
  Link State ID: 8.0.0.0
  Advertising Router: 10.0.0.31
  LS Seq Number: 0x80000002
  Checksum: 0xb9cb
  Length: 48
  Segment Routing Extended Link TLV
    Link Type: 1 (Point-to-point)
    Reserved: 0
    Link Id: 10.0.0.175
    Link Data: 20.31.175.31
    Adj-SID Sub-TLV
      Flags: [V, L]
      Reserved: 0
      Multi-Topology ID: 0
      SID: 411296

  LS Age: 1179
  Options: (E DC)
  LS Type: Opaque Type 10 Links
  Link State ID: 8.0.0.4
  Advertising Router: 10.0.0.175
  LS Seq Number: 0x80000002
  Checksum: 0x3cb6
  Length: 48
  Segment Routing Extended Link TLV
    Link Type: 1 (Point-to-point)
    Reserved: 0
    Link Id: 10.0.0.31
    Link Data: 20.31.175.175
    Adj-SID Sub-TLV
      Flags: [V, L]
      Reserved: 0
      Multi-Topology ID: 0
      SID: 40

  LS Age: 500
  Options: (E DC)
  LS Type: Opaque Type 10 Links
  Link State ID: 8.0.0.24
  Advertising Router: 10.0.0.175
  LS Seq Number: 0x80000001
  Checksum: 0x911f
  Length: 48
  Segment Routing Extended Link TLV
    Link Type: 1 (Point-to-point)
    Reserved: 0
    Link Id: 10.0.0.179
    Link Data: 20.175.179.175
    Adj-SID Sub-TLV
      Flags: [V, L]
      Reserved: 0
      Multi-Topology ID: 0
      SID: 46

  LS Age: 368
  Options: (DC O)
  LS Type: Opaque Type 10 Links
  Link State ID: 8.0.0.0
  Advertising Router: 10.0.0.32
  LS Seq Number: 0x80000002
  Checksum: 0xd5ac
  Length: 48
  Segment Routing Extended Link TLV
    Link Type: 1 (Point-to-point)
    Reserved: 0
    Link Id: 10.0.0.175
    Link Data: 20.32.175.32
    Adj-SID Sub-TLV
      Flags: [V, L]
      Reserved: 0
      Multi-Topology ID: 0
      SID: 411296

  LS Age: 1001
  Options: (E DC)
  LS Type: Opaque Type 10 Links
  Link State ID: 8.0.0.6
  Advertising Router: 10.0.0.175
  LS Seq Number: 0x80000002
  Checksum: 0x6e0b
  Length: 48
  Segment Routing Extended Link TLV
    Link Type: 1 (Point-to-point)
    Reserved: 0
    Link Id: 10.0.0.217
    Link Data: 20.175.217.175
    Adj-SID Sub-TLV
      Flags: [V, L]
      Reserved: 0
      Multi-Topology ID: 0
      SID: 42

  LS Age: 1817
  Options: (E DC)
  LS Type: Opaque Type 10 Links
  Link State ID: 8.0.0.18
  Advertising Router: 10.0.0.175
  LS Seq Number: 0x80000001
  Checksum: 0xa0ca
  Length: 48
  Segment Routing Extended Link TLV
    Link Type: 1 (Point-to-point)
    Reserved: 0
    Link Id: 10.0.0.214
    Link Data: 20.175.214.175
    Adj-SID Sub-TLV
      Flags: [V, L]
      Reserved: 0
      Multi-Topology ID: 0
      SID: 51

  LS Age: 1500
  Options: (E DC)
  LS Type: Opaque Type 10 Links
  Link State ID: 8.0.0.22
  Advertising Router: 10.0.0.175
  LS Seq Number: 0x80000001
  Checksum: 0xf425
  Length: 48
  Segment Routing Extended Link TLV
    Link Type: 1 (Point-to-point)
    Reserved: 0
    Link Id: 10.0.0.124
    Link Data: 20.124.175.175
    Adj-SID Sub-TLV
      Flags: [V, L]
      Reserved: 0
      Multi-Topology ID: 0
      SID: 53

  LS Age: 493
  Options: (E)
  LS Type: Opaque Type 10 Links
  Link State ID: 8.0.0.3
  Advertising Router: 10.0.0.217
  LS Seq Number: 0x80000002
  Checksum: 0xb8df
  Length: 48
  Segment Routing Extended Link TLV
    Link Type: 1 (Point-to-point)
    Reserved: 0
    Link Id: 10.0.0.175
    Link Data: 20.175.217.217
    Adj-SID Sub-TLV
      Flags: [V, L]
      Reserved: 0
      Multi-Topology ID: 0
      SID: 524285

  LS Age: 286
  Options: (E DC)
  LS Type: Opaque Type 10 Links
  Link State ID: 8.0.0.13
  Advertising Router: 10.0.0.175
  LS Seq Number: 0x80000003
  Checksum: 0x2253
  Length: 48
  Segment Routing Extended Link TLV
    Link Type: 1 (Point-to-point)
    Reserved: 0
    Link Id: 10.0.0.84
    Link Data: 20.84.175.175
    Adj-SID Sub-TLV
      Flags: [V, L]
      Reserved: 0
      Multi-Topology ID: 0
      SID: 49

  LS Age: 824
  Options: (E DC)
  LS Type: Opaque Type 10 Links
  Link State ID: 8.0.0.9
  Advertising Router: 10.0.0.175
  LS Seq Number: 0x80000002
  Checksum: 0x45a5
  Length: 48
  Segment Routing Extended Link TLV
    Link Type: 1 (Point-to-point)
    Reserved: 0
    Link Id: 10.0.0.32
    Link Data: 20.32.175.175
    Adj-SID Sub-TLV
      Flags: [V, L]
      Reserved: 0
      Multi-Topology ID: 0
      SID: 41

  LS Age: 1831
  Options: (E DC)
  LS Type: Opaque Type 10 Links
  Link State ID: 8.0.0.17
  Advertising Router: 10.0.0.175
  LS Seq Number: 0x80000001
  Checksum: 0xc6f2
  Length: 48
  Segment Routing Extended Link TLV
    Link Type: 1 (Point-to-point)
    Reserved: 0
    Link Id: 192.168.20.120
    Link Data: 20.120.175.175
    Adj-SID Sub-TLV
      Flags: [V, L]
      Reserved: 0
      Multi-Topology ID: 0
      SID: 47

  LS Age: 1514
  Options: (E)
  LS Type: Opaque Type 10 Links
  Link State ID: 8.0.0.1
  Advertising Router: 192.168.20.128
  LS Seq Number: 0x80000001
  Checksum: 0x5e5f
  Length: 48
  Segment Routing Extended Link TLV
    Link Type: 1 (Point-to-point)
    Reserved: 0
    Link Id: 10.0.0.175
    Link Data: 20.128.175.128
    Adj-SID Sub-TLV
      Flags: [V, L]
      Reserved: 0
      Multi-Topology ID: 0
      SID: 48063

  LS Age: 1501
  Options: (E)
  LS Type: Opaque Type 10 Links
  Link State ID: 8.0.0.1
  Advertising Router: 10.0.0.124
  LS Seq Number: 0x80000001
  Checksum: 0x365
  Length: 48
  Segment Routing Extended Link TLV
    Link Type: 1 (Point-to-point)
    Reserved: 0
    Link Id: 10.0.0.175
    Link Data: 20.124.175.124
    Adj-SID Sub-TLV
      Flags: [V, L]
      Reserved: 0
      Multi-Topology ID: 0
      SID: 335

  LS Age: 476
  Options: (E)
  LS Type: Opaque Type 10 Links
  Link State ID: 8.0.0.1
  Advertising Router: 10.0.0.221
  LS Seq Number: 0x80000003
  Checksum: 0x193b
  Length: 96
  Segment Routing Extended Link TLV
    Link Type: 1 (Point-to-point)
    Reserved: 0
    Link Id: 10.0.0.175
    Link Data: 20.175.221.221
    Adj-SID Sub-TLV
      Flags: [V, L]
      Reserved: 0
      Multi-Topology ID: 0
      SID: 524298
    Adj-SID Sub-TLV
      Flags: [B, V, L]
      Reserved: 0
      Multi-Topology ID: 0
      SID: 524299
    Unsupported sub-TLV: Type 10, Length 24
    Unsupported sub-TLV: Type 8, Length 4

  LS Age: 2023
  Options: (E DC)
  LS Type: Opaque Type 10 Links
  Link State ID: 8.0.0.1
  Advertising Router: 10.0.0.131
  LS Seq Number: 0x80000001
  Checksum: 0xf679
  Length: 48
  Segment Routing Extended Link TLV
    Link Type: 1 (Point-to-point)
    Reserved: 0
    Link Id: 10.0.0.175
    Link Data: 20.131.175.131
    Adj-SID Sub-TLV
      Flags: [V, L]
      Reserved: 0
      Multi-Topology ID: 0
      SID: 19

  LS Age: 496
  Options: (E DC)
  LS Type: Opaque Type 10 Links
  Link State ID: 8.0.0.1
  Advertising Router: 10.0.0.179
  LS Seq Number: 0x80000003
  Checksum: 0x2dd
  Length: 48
  Segment Routing Extended Link TLV
    Link Type: 1 (Point-to-point)
    Reserved: 0
    Link Id: 10.0.0.175
    Link Data: 20.175.179.179
    Adj-SID Sub-TLV
      Flags: [V, L]
      Reserved: 0
      Multi-Topology ID: 0
      SID: 17

  LS Age: 184
  Options: (E DC)
  LS Type: Opaque Type 10 Links
  Link State ID: 8.0.0.25
  Advertising Router: 10.0.0.175
  LS Seq Number: 0x80000001
  Checksum: 0x5755
  Length: 48
  Segment Routing Extended Link TLV
    Link Type: 1 (Point-to-point)
    Reserved: 0
    Link Id: 10.0.0.184
    Link Data: 20.175.184.175
    Adj-SID Sub-TLV
      Flags: [V, L]
      Reserved: 0
      Multi-Topology ID: 0
      SID: 39

  LS Age: 1513
  Options: (E DC)
  LS Type: Opaque Type 10 Links
  Link State ID: 8.0.0.21
  Advertising Router: 10.0.0.175
  LS Seq Number: 0x80000001
  Checksum: 0x217f
  Length: 48
  Segment Routing Extended Link TLV
    Link Type: 1 (Point-to-point)
    Reserved: 0
    Link Id: 192.168.20.128
    Link Data: 20.128.175.175
    Adj-SID Sub-TLV
      Flags: [V, L]
      Reserved: 0
      Multi-Topology ID: 0
      SID: 52

  LS Age: 100
  Options: (E DC)
  LS Type: Opaque Type 10 Links
  Link State ID: 8.0.0.15
  Advertising Router: 10.0.0.175
  LS Seq Number: 0x80000002
  Checksum: 0xb460
  Length: 48
  Segment Routing Extended Link TLV
    Link Type: 1 (Point-to-point)
    Reserved: 0
    Link Id: 10.0.0.131
    Link Data: 20.131.175.175
    Adj-SID Sub-TLV
      Flags: [V, L]
      Reserved: 0
      Multi-Topology ID: 0
      SID: 50

  LS Age: 472
  Options: (E DC)
  LS Type: Opaque Type 10 Links
  Link State ID: 8.0.0.11
  Advertising Router: 10.0.0.175
  LS Seq Number: 0x80000002
  Checksum: 0xa5fa
  Length: 48
  Segment Routing Extended Link TLV
    Link Type: 1 (Point-to-point)
    Reserved: 0
    Link Id: 10.0.0.66
    Link Data: 20.66.175.175
    Adj-SID Sub-TLV
      Flags: [V, L]
      Reserved: 0
      Multi-Topology ID: 0
      SID: 45

  LS Age: 388
  Options: (E DC)
  LS Type: Opaque Type 10 Links
  Link State ID: 8.255.216.243
  Advertising Router: 10.0.0.66
  LS Seq Number: 0x80000003
  Checksum: 0x78ba
  Length: 48
  Segment Routing Extended Link TLV
    Link Type: 1 (Point-to-point)
    Reserved: 0
    Link Id: 10.0.0.175
    Link Data: 20.66.175.66
    Adj-SID Sub-TLV
      Flags: [V, L]
      Reserved: 0
      Multi-Topology ID: 0
      SID: 22000

  LS Age: 555
  Options: (E)
  LS Type: Opaque Type 10 Links
  Link State ID: 4.0.0.0
  Advertising Router: 192.168.20.128
  LS Seq Number: 0x80000004
  Checksum: 0xab0c
  Length: 52
  Segment Routing Router Information TLV
    Supported Algorithm: Shortest Path First
    Label Range
      SRGB Base: 20000, Size: 2000
  Unsupported TLV: Type 12, Length 2

  LS Age: 251
  Options: (E O)
  LS Type: Opaque Type 10 Links
  Link State ID: 4.0.0.0
  Advertising Router: 192.168.20.120
  LS Seq Number: 0x80000002
  Checksum: 0x1721
  Length: 60
  Segment Routing Router Information TLV
    Supported Algorithm: Shortest Path First
    Label Range
      SRGB Base: 16000, Size: 8001
  Unsupported TLV: Type 12, Length 2
  Unsupported TLV: Type 1, Length 4

  LS Age: 428
  Options: (DC O)
  LS Type: Opaque Type 10 Links
  Link State ID: 4.0.0.0
  Advertising Router: 10.0.0.32
  LS Seq Number: 0x80000002
  Checksum: 0xaaa5
  Length: 44
  Segment Routing Router Information TLV
    Supported Algorithm: Shortest Path First
    Label Range
      SRGB Base: 20000, Size: 2000

  LS Age: 208
  Options: (E DC)
  LS Type: Opaque Type 10 Links
  Link State ID: 4.0.0.0
  Advertising Router: 10.0.0.66
  LS Seq Number: 0x80000002
  Checksum: 0x1953
  Length: 44
  Segment Routing Router Information TLV
    Supported Algorithm: Shortest Path First
    Label Range
      SRGB Base: 20000, Size: 2000

  LS Age: 347
  Options: (E)
  LS Type: Opaque Type 10 Links
  Link State ID: 4.0.0.0
  Advertising Router: 10.0.0.124
  LS Seq Number: 0x80000004
  Checksum: 0xa51f
  Length: 52
  Segment Routing Router Information TLV
    Supported Algorithm: Shortest Path First
    Label Range
      SRGB Base: 2000, Size: 2001
  Unsupported TLV: Type 12, Length 2

  LS Age: 985
  Options: (E DC)
  LS Type: Opaque Type 10 Links
  Link State ID: 4.0.0.0
  Advertising Router: 10.0.0.72
  LS Seq Number: 0x80000002
  Checksum: 0xf471
  Length: 44
  Segment Routing Router Information TLV
    Supported Algorithm: Shortest Path First
    Label Range
      SRGB Base: 20000, Size: 2000

  LS Age: 106
  Options: (E DC)
  LS Type: Opaque Type 10 Links
  Link State ID: 4.0.0.0
  Advertising Router: 10.0.0.84
  LS Seq Number: 0x80000002
  Checksum: 0x8065
  Length: 60
  Segment Routing Router Information TLV
    Supported Algorithm: Shortest Path First
    Label Range
      SRGB Base: 20000, Size: 2000
  Unsupported TLV: Type 12, Length 2
  Unsupported TLV: Type 1, Length 4

  LS Age: 1812
  Options: (E)
  LS Type: Opaque Type 10 Links
  Link State ID: 4.0.0.0
  Advertising Router: 10.0.0.214
  LS Seq Number: 0x80000002
  Checksum: 0x290e
  Length: 48
  Segment Routing Router Information TLV
  Unsupported TLV: Type 7, Length 13
  Unsupported TLV: Type 1, Length 4

  LS Age: 476
  Options: (E)
  LS Type: Opaque Type 10 Links
  Link State ID: 4.0.0.0
  Advertising Router: 10.0.0.221
  LS Seq Number: 0x80000003
  Checksum: 0xa510
  Length: 68
  Segment Routing Router Information TLV
    Supported Algorithm: Shortest Path First
    Label Range
      SRGB Base: 720000, Size: 2000
  Unsupported TLV: Type 12, Length 2
  Unsupported TLV: Type 14, Length 12

  LS Age: 322
  Options: (E)
  LS Type: Opaque Type 10 Links
  Link State ID: 4.0.0.0
  Advertising Router: 10.0.0.217
  LS Seq Number: 0x80000002
  Checksum: 0x820c
  Length: 80
  Segment Routing Router Information TLV
    Supported Algorithm: Shortest Path First
    Label Range
      SRGB Base: 20000, Size: 2000
  Unsupported TLV: Type 12, Length 4
  Unsupported TLV: Type 7, Length 13
  Unsupported TLV: Type 1, Length 4

  LS Age: 501
  Options: (E DC)
  LS Type: Opaque Type 10 Links
  Link State ID: 4.0.0.0
  Advertising Router: 10.0.0.179
  LS Seq Number: 0x80000003
  Checksum: 0xd821
  Length: 44
  Segment Routing Router Information TLV
    Supported Algorithm: Shortest Path First
    Label Range
      SRGB Base: 20000, Size: 2000

  LS Age: 1085
  Options: (E DC)
  LS Type: Opaque Type 10 Links
  Link State ID: 4.0.0.0
  Advertising Router: 10.0.0.131
  LS Seq Number: 0x80000002
  Checksum: 0xfb2f
  Length: 44
  Segment Routing Router Information TLV
    Supported Algorithm: Shortest Path First
    Label Range
      SRGB Base: 20000, Size: 2000

  LS Age: 1557
  Options: (E DC)
  LS Type: Opaque Type 10 Links
  Link State ID: 4.0.0.0
  Advertising Router: 10.0.0.175
  LS Seq Number: 0x80000002
  Checksum: 0xf20c
  Length: 44
  Segment Routing Router Information TLV
    Supported Algorithm: Shortest Path First
    Label Range
      SRGB Base: 20000, Size: 2000

  LS Age: 436
  Options: (DC O)
  LS Type: Opaque Type 10 Links
  Link State ID: 4.0.0.0
  Advertising Router: 10.0.0.31
  LS Seq Number: 0x80000002
  Checksum: 0xb0a0
  Length: 44
  Segment Routing Router Information TLV
    Supported Algorithm: Shortest Path First
    Label Range
      SRGB Base: 20000, Size: 2000

  LS Age: 476
  Options: (E)
  LS Type: Opaque Type 10 Links
  Link State ID: 1.0.0.1
  Advertising Router: 10.0.0.221
  LS Seq Number: 0x80000002
  Checksum: 0xc5f3
  Length: 156
   Link Type: Point-to-point
   Link Id: 10.0.0.175
   Interface Address: 20.175.221.221
   Neighbor Address: 20.175.221.175
   TE default metric: 10
   Maximum link BW: 0.00 bps
   Maximum reservable link BW: 0.00 bps
   Administrative group (Color): 0x0
   Unreserved BW:
    TE class 0: 0.00 bps	    TE class 1: 0.00 bps	    TE class 2: 0.00 bps
    TE class 3: 0.00 bps	    TE class 4: 0.00 bps	    TE class 5: 0.00 bps
    TE class 6: 0.00 bps	    TE class 7: 0.00 bps
   Unsupported sub-TLV: Type: 11 Length: 8
   Unsupported sub-TLV: Type: 14 Length: 4
   Unsupported sub-TLV: Type: 0 Length: 0
   Unsupported sub-TLV: Type: 0 Length: 0
   Unsupported sub-TLV: Type: 0 Length: 0

  LS Age: 496
  Options: (E)
  LS Type: Opaque Type 10 Links
  Link State ID: 1.0.0.0
  Advertising Router: 10.0.0.221
  LS Seq Number: 0x80000002
  Checksum: 0x7906
  Length: 28
   TE router ID: 10.0.0.221

  LS Age: 350
  Options: (E)
  LS Type: Opaque Type 10 Links
  Link State ID: 1.0.0.1
  Advertising Router: 10.0.0.217
  LS Seq Number: 0x80000003
  Checksum: 0x5d28
  Length: 28
   TE router ID: 10.0.0.217

  LS Age: 2280
  Options: (E DC)
  LS Type: Opaque Type 10 Links
  Link State ID: 7.0.0.1
  Advertising Router: 10.0.0.175
  LS Seq Number: 0x80000001
  Checksum: 0x377
  Length: 44
  Segment Routing Extended Prefix TLV
    Route Type: Intra-Area, Prefix: 10.0.0.175/32, AF: IPv4 unicast
    Flags:  [N]
    Prefix-SID Sub-TLV
      Algorithm: Shortest Path First
      Flags:  []
      MT-ID: 0, SID: 175

  LS Age: 253
  Options: (E)
  LS Type: Opaque Type 10 Links
  Link State ID: 7.0.0.2
  Advertising Router: 10.0.0.217
  LS Seq Number: 0x80000002
  Checksum: 0x7841
  Length: 44
  Segment Routing Extended Prefix TLV
    Route Type: Intra-Area, Prefix: 10.0.0.217/32, AF: IPv4 unicast
    Flags:  [N]
    Prefix-SID Sub-TLV
      Algorithm: Shortest Path First
      Flags:  [NP]
      MT-ID: 0, SID: 217

  LS Age: 521
  Options: (E)
  LS Type: Opaque Type 10 Links
  Link State ID: 7.0.0.0
  Advertising Router: 192.168.20.128
  LS Seq Number: 0x80000002
  Checksum: 0x6a4a
  Length: 44
  Segment Routing Extended Prefix TLV
    Route Type: Intra-Area, Prefix: 10.0.0.128/32, AF: IPv4 unicast
    Flags:  [N]
    Prefix-SID Sub-TLV
      Algorithm: Shortest Path First
      Flags:  []
      MT-ID: 0, SID: 128

  LS Age: 251
  Options: (E O)
  LS Type: Opaque Type 10 Links
  Link State ID: 7.0.0.0
  Advertising Router: 192.168.20.120
  LS Seq Number: 0x80000002
  Checksum: 0x95f6
  Length: 44
  Segment Routing Extended Prefix TLV
    Route Type: Intra-Area, Prefix: 10.0.0.120/32, AF: IPv4 unicast
    Flags:  [N]
    Prefix-SID Sub-TLV
      Algorithm: Shortest Path First
      Flags:  []
      MT-ID: 0, SID: 120

  LS Age: 428
  Options: (DC O)
  LS Type: Opaque Type 10 Links
  Link State ID: 7.0.0.0
  Advertising Router: 10.0.0.32
  LS Seq Number: 0x80000002
  Checksum: 0x5496
  Length: 44
  Segment Routing Extended Prefix TLV
    Route Type: Intra-Area, Prefix: 10.0.0.32/32, AF: IPv4 unicast
    Flags:  [N]
    Prefix-SID Sub-TLV
      Algorithm: Shortest Path First
      Flags:  []
      MT-ID: 0, SID: 32

  LS Age: 2168
  Options: (E DC)
  LS Type: Opaque Type 10 Links
  Link State ID: 7.0.0.0
  Advertising Router: 10.0.0.66
  LS Seq Number: 0x80000001
  Checksum: 0x843f
  Length: 44
  Segment Routing Extended Prefix TLV
    Route Type: Intra-Area, Prefix: 10.0.0.66/32, AF: IPv4 unicast
    Flags:  [N]
    Prefix-SID Sub-TLV
      Algorithm: Shortest Path First
      Flags:  []
      MT-ID: 0, SID: 66

  LS Age: 197
  Options: (E)
  LS Type: Opaque Type 10 Links
  Link State ID: 7.0.0.0
  Advertising Router: 10.0.0.124
  LS Seq Number: 0x80000002
  Checksum: 0xe40f
  Length: 44
  Segment Routing Extended Prefix TLV
    Route Type: Intra-Area, Prefix: 10.0.0.124/32, AF: IPv4 unicast
    Flags:  [N]
    Prefix-SID Sub-TLV
      Algorithm: Shortest Path First
      Flags:  [NP]
      MT-ID: 0, SID: 124

  LS Age: 905
  Options: (E DC)
  LS Type: Opaque Type 10 Links
  Link State ID: 7.0.0.0
  Advertising Router: 10.0.0.72
  LS Seq Number: 0x80000002
  Checksum: 0x4f61
  Length: 44
  Segment Routing Extended Prefix TLV
    Route Type: Intra-Area, Prefix: 10.0.0.72/32, AF: IPv4 unicast
    Flags:  [N]
    Prefix-SID Sub-TLV
      Algorithm: Shortest Path First
      Flags:  []
      MT-ID: 0, SID: 72

  LS Age: 476
  Options: (E)
  LS Type: Opaque Type 10 Links
  Link State ID: 7.0.0.0
  Advertising Router: 10.0.0.221
  LS Seq Number: 0x80000005
  Checksum: 0xfa26
  Length: 44
  Segment Routing Extended Prefix TLV
    Route Type: Intra-Area, Prefix: 10.0.0.221/32, AF: IPv4 unicast
    Flags:  [N]
    Prefix-SID Sub-TLV
      Algorithm: Shortest Path First
      Flags:  []
      MT-ID: 0, SID: 1221

  LS Age: 201
  Options: (E DC)
  LS Type: Opaque Type 10 Links
  Link State ID: 7.0.0.1
  Advertising Router: 10.0.0.84
  LS Seq Number: 0x80000002
  Checksum: 0xa3a7
  Length: 44
  Segment Routing Extended Prefix TLV
    Route Type: Intra-Area, Prefix: 10.0.0.84/32, AF: IPv4 unicast
    Flags:  [N]
    Prefix-SID Sub-TLV
      Algorithm: Shortest Path First
      Flags:  [NP]
      MT-ID: 0, SID: 84

  LS Age: 501
  Options: (E DC)
  LS Type: Opaque Type 10 Links
  Link State ID: 7.0.0.1
  Advertising Router: 10.0.0.179
  LS Seq Number: 0x80000003
  Checksum: 0x87e4
  Length: 44
  Segment Routing Extended Prefix TLV
    Route Type: Intra-Area, Prefix: 10.0.0.179/32, AF: IPv4 unicast
    Flags:  [N]
    Prefix-SID Sub-TLV
      Algorithm: Shortest Path First
      Flags:  []
      MT-ID: 0, SID: 179

  LS Age: 398
  Options: (E DC)
  LS Type: Opaque Type 10 Links
  Link State ID: 7.0.0.1
  Advertising Router: 10.0.0.131
  LS Seq Number: 0x80000002
  Checksum: 0x23da
  Length: 44
  Segment Routing Extended Prefix TLV
    Route Type: Intra-Area, Prefix: 10.0.0.131/32, AF: IPv4 unicast
    Flags:  [N]
    Prefix-SID Sub-TLV
      Algorithm: Shortest Path First
      Flags:  []
      MT-ID: 0, SID: 131

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

 C        10.0.0.31/32
           directly connected, Loopback0
 O        10.0.0.32/32 [110/21]
           via 20.31.175.175, Ethernet5
 O        10.0.0.66/32 [110/21]
           via 20.31.175.175, Ethernet5
 O        10.0.0.72/32 [110/21]
           via 20.31.175.175, Ethernet5
 O        10.0.0.84/32 [110/12]
           via 20.31.175.175, Ethernet5
 O        10.0.0.120/32 [110/11]
           via 20.31.175.175, Ethernet5
 O        10.0.0.124/32 [110/11]
           via 20.31.175.175, Ethernet5
 O        10.0.0.128/32 [110/11]
           via 20.31.175.175, Ethernet5
 O        10.0.0.131/32 [110/11]
           via 20.31.175.175, Ethernet5
 O        10.0.0.175/32 [110/10]
           via 20.31.175.175, Ethernet5
 O        10.0.0.179/32 [110/11]
           via 20.31.175.175, Ethernet5
 O        10.0.0.184/32 [110/11]
           via 20.31.175.175, Ethernet5
 O        10.0.0.214/32 [110/11]
           via 20.31.175.175, Ethernet5
 O        10.0.0.217/32 [110/11]
           via 20.31.175.175, Ethernet5
 O        10.0.0.221/32 [110/11]
           via 20.31.175.175, Ethernet5
 C        20.31.175.0/24
           directly connected, Ethernet5
 O        20.32.175.0/24 [110/11]
           via 20.31.175.175, Ethernet5
 O        20.53.175.0/24 [110/11]
           via 20.31.175.175, Ethernet5
 O        20.66.175.0/24 [110/11]
           via 20.31.175.175, Ethernet5
 O        20.72.175.0/24 [110/11]
           via 20.31.175.175, Ethernet5
 O        20.84.175.0/24 [110/11]
           via 20.31.175.175, Ethernet5
 O        20.120.175.0/24 [110/11]
           via 20.31.175.175, Ethernet5
 O        20.124.175.0/24 [110/11]
           via 20.31.175.175, Ethernet5
 O        20.128.175.0/24 [110/11]
           via 20.31.175.175, Ethernet5
 O        20.131.175.0/24 [110/11]
           via 20.31.175.175, Ethernet5
 O        20.175.179.0/24 [110/11]
           via 20.31.175.175, Ethernet5
 O        20.175.184.0/24 [110/11]
           via 20.31.175.175, Ethernet5
 O        20.175.214.0/24 [110/11]
           via 20.31.175.175, Ethernet5
 O        20.175.217.0/24 [110/11]
           via 20.31.175.175, Ethernet5
 O        20.175.221.0/24 [110/11]
           via 20.31.175.175, Ethernet5

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

 C        50.10.31.0/24
           directly connected, Ethernet40.4
 B I      50.10.32.0/24 [200/0]
           via 10.0.0.32/32, OSPF SR tunnel index 4, label 378528
              via 20.31.175.175, Ethernet5, label 20032
 B I      50.10.66.0/24 [200/0]
           via 10.0.0.66/32, OSPF SR tunnel index 6, label 62000
              via 20.31.175.175, Ethernet5, label 20066
 B I      50.10.72.0/24 [200/0]
           via 10.0.0.72/32, OSPF SR tunnel index 5, label 62002
              via 20.31.175.175, Ethernet5, label 20072
 B I      50.10.84.0/24 [200/0]
           via 10.0.0.84/32, OSPF SR tunnel index 7, label 720896
              via 20.31.175.175, Ethernet5, label 20084
 B I      50.10.120.0/24 [200/0]
           via 10.0.0.120/32, OSPF SR tunnel index 8, label 1277
              via 20.31.175.175, Ethernet5, label 20120
 B I      50.10.124.0/24 [200/0]
           via 10.0.0.124/32, OSPF SR tunnel index 11, label 332
              via 20.31.175.175, Ethernet5, label 20124
 B I      50.10.128.0/24 [200/0]
           via 10.0.0.128/32, OSPF SR tunnel index 10, label 48060
              via 20.31.175.175, Ethernet5, label 20128
 B I      50.10.131.0/24 [200/0]
           via 10.0.0.131/32, OSPF SR tunnel index 9, label 18
              via 20.31.175.175, Ethernet5, label 20131
 B I      50.10.179.0/24 [200/0]
           via 10.0.0.179/32, OSPF SR tunnel index 12, label 16
              via 20.31.175.175, Ethernet5, label 20179
 B I      50.10.217.0/24 [200/0]
           via 10.0.0.217/32, OSPF SR tunnel index 3, label 524287
              via 20.31.175.175, Ethernet5, label 20217
 B I      50.10.221.0/24 [200/0]
           via 10.0.0.221/32, OSPF SR tunnel index 2, label 524289
              via 20.31.175.175, Ethernet5, label 21221
 B I      51.10.120.0/24 [200/0]
           via 10.0.0.120/32, OSPF SR tunnel index 8, label 1277
              via 20.31.175.175, Ethernet5, label 20120

```

## show ipv6 route

```text

VRF: default
Displaying 0 of 3 IPv6 routing table entries
Source Codes:
       C - connected, S - static, K - kernel, O3 - OSPFv3,
       B - Other BGP Routes, A B - BGP Aggregate, R - RIP,
       I L1 - IS-IS level 1, I L2 - IS-IS level 2, DH - DHCP,
       NG - Nexthop Group Static Route, M - Martian,
       DP - Dynamic Policy Route, L - VRF Leaked,
       G  - gRIBI, RC - Route Cache Route,
       CL - CBF Leaked Route


```

## show ipv6 route vrf RED

```text

VRF: RED
Displaying 13 of 17 IPv6 routing table entries
Source Codes:
       C - connected, S - static, K - kernel, O3 - OSPFv3,
       B - Other BGP Routes, A B - BGP Aggregate, R - RIP,
       I L1 - IS-IS level 1, I L2 - IS-IS level 2, DH - DHCP,
       NG - Nexthop Group Static Route, M - Martian,
       DP - Dynamic Policy Route, L - VRF Leaked,
       G  - gRIBI, RC - Route Cache Route,
       CL - CBF Leaked Route

 C        2600:50:10:31::/64 [0/0]
           via Ethernet40.6, directly connected
 B I      2600:50:10:32::/64 [200/0]
           via 10.0.0.32/32, OSPF SR tunnel index 4, label 378529
              via 20.31.175.175, Ethernet5, label 20032
 B I      2600:50:10:66::/64 [200/0]
           via 10.0.0.66/32, OSPF SR tunnel index 6, label 62001
              via 20.31.175.175, Ethernet5, label 20066
 B I      2600:50:10:72::/64 [200/0]
           via 10.0.0.72/32, OSPF SR tunnel index 5, label 62003
              via 20.31.175.175, Ethernet5, label 20072
 B I      2600:50:10:84::/64 [200/0]
           via 10.0.0.84/32, OSPF SR tunnel index 7, label 720897
              via 20.31.175.175, Ethernet5, label 20084
 B I      2600:50:10:120::/64 [200/0]
           via 10.0.0.120/32, OSPF SR tunnel index 8, label 1276
              via 20.31.175.175, Ethernet5, label 20120
 B I      2600:50:10:124::/64 [200/0]
           via 10.0.0.124/32, OSPF SR tunnel index 11, label 333
              via 20.31.175.175, Ethernet5, label 20124
 B I      2600:50:10:128::/64 [200/0]
           via 10.0.0.128/32, OSPF SR tunnel index 10, label 48061
              via 20.31.175.175, Ethernet5, label 20128
 B I      2600:50:10:131::/64 [200/0]
           via 10.0.0.131/32, OSPF SR tunnel index 9, label 18
              via 20.31.175.175, Ethernet5, label 20131
 B I      2600:50:10:179::/64 [200/0]
           via 10.0.0.179/32, OSPF SR tunnel index 12, label 16
              via 20.31.175.175, Ethernet5, label 20179
 B I      2600:50:10:217::/64 [200/0]
           via 10.0.0.217/32, OSPF SR tunnel index 3, label 524287
              via 20.31.175.175, Ethernet5, label 20217
 B I      2600:50:10:221::/64 [200/0]
           via 10.0.0.221/32, OSPF SR tunnel index 2, label 524289
              via 20.31.175.175, Ethernet5, label 21221
 B I      2600:51:10:120::/64 [200/0]
           via 10.0.0.120/32, OSPF SR tunnel index 8, label 1276
              via 20.31.175.175, Ethernet5, label 20120

```

## show mpls route

```text
MPLS forwarding table (Label [metric] Vias) - 15 routes 
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
                via M, forward
                    EgressACL: apply
                    20.31.175.175 Ethernet5
 20066   A[1]
                via M, forward
                    EgressACL: apply
                    20.31.175.175 Ethernet5
 20072   A[1]
                via M, forward
                    EgressACL: apply
                    20.31.175.175 Ethernet5
 20084   A[1]
                via M, forward
                    EgressACL: apply
                    20.31.175.175 Ethernet5
 20120   A[1]
                via M, forward
                    EgressACL: apply
                    20.31.175.175 Ethernet5
 20124   A[1]
                via M, forward
                    EgressACL: apply
                    20.31.175.175 Ethernet5
 20128   A[1]
                via M, forward
                    EgressACL: apply
                    20.31.175.175 Ethernet5
 20131   A[1]
                via M, forward
                    EgressACL: apply
                    20.31.175.175 Ethernet5
 20175   A[1]
                via M, pop
                    EgressACL: apply
                    20.31.175.175 Ethernet5
 20179   A[1]
                via M, forward
                    EgressACL: apply
                    20.31.175.175 Ethernet5
 20217   A[1]
                via M, forward
                    EgressACL: apply
                    20.31.175.175 Ethernet5
 21221   A[1]
                via M, forward
                    EgressACL: apply
                    20.31.175.175 Ethernet5
 362144   [0]
                via I, ipv6, vrf RED
 362145   [0]
                via I, ipv4, vrf RED
 411296  A[1]
                via M, 20.31.175.175, pop
                    EgressACL: apply
                    directly connected, Ethernet5
                    3c:08:cd:8d:ba:f4, vlan 1010
```

## show mpls lfib route

```text
MPLS forwarding table (Label [metric] Vias) - 15 routes 
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

 OP    20032    [1], 10.0.0.32/32
                via M, 20.31.175.175, forward
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                 interface Ethernet5
 OP    20066    [1], 10.0.0.66/32
                via M, 20.31.175.175, forward
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                 interface Ethernet5
 OP    20072    [1], 10.0.0.72/32
                via M, 20.31.175.175, forward
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                 interface Ethernet5
 OP    20084    [1], 10.0.0.84/32
                via M, 20.31.175.175, forward
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                 interface Ethernet5
 OP    20120    [1], 10.0.0.120/32
                via M, 20.31.175.175, forward
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                 interface Ethernet5
 OP    20124    [1], 10.0.0.124/32
                via M, 20.31.175.175, forward
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                 interface Ethernet5
 OP    20128    [1], 10.0.0.128/32
                via M, 20.31.175.175, forward
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                 interface Ethernet5
 OP    20131    [1], 10.0.0.131/32
                via M, 20.31.175.175, forward
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                 interface Ethernet5
 OP    20175    [1], 10.0.0.175/32
                via M, 20.31.175.175, pop
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                 interface Ethernet5
 OP    20179    [1], 10.0.0.179/32
                via M, 20.31.175.175, forward
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                 interface Ethernet5
 OP    20217    [1], 10.0.0.217/32
                via M, 20.31.175.175, forward
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                 interface Ethernet5
 OP    21221    [1], 10.0.0.221/32
                via M, 20.31.175.175, forward
                 payload autoDecide, ttlMode uniform, dscpMode uniform, apply egress-acl
                 interface Ethernet5
 B3    362144   [0]
                via I, ipv6, vrf RED
 B3    362145   [0]
                via I, ipv4, vrf RED
 OA    411296   [1]
                via M, 20.31.175.175, pop
                 payload autoDecide, ttlMode uniform, apply egress-acl
                 interface Ethernet5
```

## show ip ospf segment-routing

```text
OSPF Instance ID: 1
SR supported Data-plane: MPLS			SR Router ID: 10.0.0.31
SR Global Block( SRGB ): Base: 20000           	Size: 2000            

OSPF Reachability Algorithm : SPF (0)

Number of OSPF segment routing capable nodes excluding self: 12

Self-Originated Segment Statistics:
Node-Segments       : 1
Prefix-Segments     : 0
Proxy-Node-Segments : 0
Adjacency Segments  : 1

```

## show ip ospf segment-routing global-blocks

```text
OSPF Instance ID: 1
SR supported Data-plane: MPLS			SR Router ID: 10.0.0.31
Number of OSPF segment routing capable nodes excluding self: 12

        Router ID         Base    Size
-------------------- ------------ ----
        10.0.0.31        20000    2000
        10.0.0.32        20000    2000
        10.0.0.66        20000    2000
        10.0.0.72        20000    2000
        10.0.0.84        20000    2000
       10.0.0.124         2000    2001
       10.0.0.131        20000    2000
       10.0.0.175        20000    2000
       10.0.0.179        20000    2000
       10.0.0.217        20000    2000
       10.0.0.221       720000    2000
   192.168.20.120        16000    8001
   192.168.20.128        20000    2000

```

## show ip ospf segment-routing bindings

```text
10.0.0.31/32
   Local binding:  Label: imp-null
   Remote binding: Peer ID: 10.0.0.175, Label: 20031
10.0.0.32/32
   Local binding:  Label: 20032
   Remote binding: Peer ID: 10.0.0.175, Label: 20032
10.0.0.66/32
   Local binding:  Label: 20066
   Remote binding: Peer ID: 10.0.0.175, Label: 20066
10.0.0.72/32
   Local binding:  Label: 20072
   Remote binding: Peer ID: 10.0.0.175, Label: 20072
10.0.0.84/32
   Local binding:  Label: 20084
   Remote binding: Peer ID: 10.0.0.175, Label: 20084
10.0.0.120/32
   Local binding:  Label: 20120
   Remote binding: Peer ID: 10.0.0.175, Label: 20120
10.0.0.124/32
   Local binding:  Label: 20124
   Remote binding: Peer ID: 10.0.0.175, Label: 20124
10.0.0.128/32
   Local binding:  Label: 20128
   Remote binding: Peer ID: 10.0.0.175, Label: 20128
10.0.0.131/32
   Local binding:  Label: 20131
   Remote binding: Peer ID: 10.0.0.175, Label: 20131
10.0.0.175/32
   Local binding:  Label: 20175
   Remote binding: Peer ID: 10.0.0.175, Label: imp-null
10.0.0.179/32
   Local binding:  Label: 20179
   Remote binding: Peer ID: 10.0.0.175, Label: 20179
10.0.0.217/32
   Local binding:  Label: 20217
   Remote binding: Peer ID: 10.0.0.175, Label: 20217
10.0.0.221/32
   Local binding:  Label: 21221
   Remote binding: Peer ID: 10.0.0.175, Label: 21221
```

## show ip ospf segment-routing adjacency-segments

```text
OSPF Instance ID: 1
SR supported Data-plane: MPLS			SR Router ID: 10.0.0.31
Adj-SID allocation mode: SR-adjacencies
Adj-SID allocation pool: Base: 411296     Size: 16384
Adjacency Segment Count: 1
Flag Descriptions: B: Backup, V: Value, L: Local,
                   G: Group, P: Persistent

Segment Status codes: P2P - Point-to-Point adjacency, LAN - Broadcast adjacency

Adj IP Address Local Intf    SID SID Source               Flags Type  Protection
-------------- ---------- ------ ---------- ------------------- ---- -----------
 20.31.175.175        Et5 411296    Dynamic B:0 V:1 L:1 G:0 P:0  P2P unprotected

```

## show bgp evpn

```text
BGP routing table information for VRF default
Router identifier 10.0.0.31, local AS number 64512
Route status codes: * - valid, > - active, S - Stale, E - ECMP head, e - ECMP
                    c - Contributing to ECMP, % - Pending best path selection
Origin codes: i - IGP, e - EGP, ? - incomplete
AS Path Attributes: Or-ID - Originator ID, C-LST - Cluster List, LL Nexthop - Link Local Nexthop

          Network                Next Hop              Metric  LocPref Weight  Path
```

## show bgp vpn-ipv4

```text
BGP routing table information for VRF default
Router identifier 10.0.0.31, local AS number 64512
Route status codes: s - suppressed contributor, * - valid, > - active, E - ECMP head, e - ECMP
                    S - Stale, c - Contributing to ECMP, b - backup, L - labeled-unicast
                    % - Pending best path selection
Origin codes: i - IGP, e - EGP, ? - incomplete
AS Path Attributes: Or-ID - Originator ID, C-LST - Cluster List, LL Nexthop - Link Local Nexthop

          Network                Next Hop              Metric  LocPref Weight  Path
          RD: 184:5001 IPv4 prefix 20.184.184.0/24
                                 10.0.0.184            -       0       0       i Or-ID: 100.0.0.184 C-LST: 10.0.0.175 
 * >      RD: 10.0.0.31:5001 IPv4 prefix 50.10.31.0/24
                                 -                     -       -       0       i
 * >      RD: 10.0.0.32:5001 IPv4 prefix 50.10.32.0/24
                                 10.0.0.32             -       100     0       i Or-ID: 10.0.0.32 C-LST: 10.0.0.175 
 * >      RD: 66:5001 IPv4 prefix 50.10.66.0/24
                                 10.0.0.66             -       100     0       ? Or-ID: 10.0.0.66 C-LST: 10.0.0.175 
 * >      RD: 72:5001 IPv4 prefix 50.10.72.0/24
                                 10.0.0.72             -       100     0       ? Or-ID: 10.0.0.72 C-LST: 10.0.0.175 
 * >      RD: 84:5001 IPv4 prefix 50.10.84.0/24
                                 10.0.0.84             0       100     0       ? Or-ID: 10.0.0.84 C-LST: 10.0.0.175 
 * >      RD: 120:5001 IPv4 prefix 50.10.120.0/24
                                 10.0.0.120            0       100     0       ? Or-ID: 10.0.0.120 C-LST: 10.0.0.175 
 * >      RD: 124:5001 IPv4 prefix 50.10.124.0/24
                                 10.0.0.124            0       100     0       ? Or-ID: 10.0.0.124 C-LST: 10.0.0.175 
 * >      RD: 128:5001 IPv4 prefix 50.10.128.0/24
                                 10.0.0.128            0       100     0       ? Or-ID: 10.0.0.128 C-LST: 10.0.0.175 
 * >      RD: 131:5001 IPv4 prefix 50.10.131.0/24
                                 10.0.0.131            -       100     0       i Or-ID: 10.0.0.131 C-LST: 10.0.0.175 
 * >      RD: 179:5001 IPv4 prefix 50.10.179.0/24
                                 10.0.0.179            -       100     0       i Or-ID: 10.0.0.179 C-LST: 10.0.0.175 
          RD: 214:5001 IPv4 prefix 50.10.214.0/24
                                 10.0.0.214            -       100     0       i Or-ID: 10.0.0.214 C-LST: 10.0.0.175 
 * >      RD: 217:5001 IPv4 prefix 50.10.217.0/24
                                 10.0.0.217            -       100     0       i Or-ID: 10.0.0.217 C-LST: 10.0.0.175 
 * >      RD: 210:5001 IPv4 prefix 50.10.221.0/24
                                 10.0.0.221            -       100     0       i Or-ID: 10.0.0.221 C-LST: 10.0.0.175 
 * >      RD: 120:5001 IPv4 prefix 51.10.120.0/24
                                 10.0.0.120            0       100     0       ? Or-ID: 10.0.0.120 C-LST: 10.0.0.175 
```

## show bgp vpn-ipv6

```text
BGP routing table information for VRF default
Router identifier 10.0.0.31, local AS number 64512
Route status codes: s - suppressed contributor, * - valid, > - active, E - ECMP head, e - ECMP
                    S - Stale, c - Contributing to ECMP, b - backup, L - labeled-unicast
                    % - Pending best path selection
Origin codes: i - IGP, e - EGP, ? - incomplete
AS Path Attributes: Or-ID - Originator ID, C-LST - Cluster List, LL Nexthop - Link Local Nexthop

          Network                Next Hop              Metric  LocPref Weight  Path
          RD: 184:5001 IPv6 prefix 2001:0:184:184::/64
                                 ::ffff:10.0.0.184     -       0       0       i Or-ID: 100.0.0.184 C-LST: 10.0.0.175 
 * >      RD: 10.0.0.31:5001 IPv6 prefix 2600:50:10:31::/64
                                 -                     -       -       0       i
 * >      RD: 10.0.0.32:5001 IPv6 prefix 2600:50:10:32::/64
                                 ::ffff:10.0.0.32      -       100     0       i Or-ID: 10.0.0.32 C-LST: 10.0.0.175 
 * >      RD: 66:5001 IPv6 prefix 2600:50:10:66::/64
                                 ::ffff:10.0.0.66      -       100     0       ? Or-ID: 10.0.0.66 C-LST: 10.0.0.175 
 * >      RD: 72:5001 IPv6 prefix 2600:50:10:72::/64
                                 ::ffff:10.0.0.72      -       100     0       ? Or-ID: 10.0.0.72 C-LST: 10.0.0.175 
 * >      RD: 84:5001 IPv6 prefix 2600:50:10:84::/64
                                 ::ffff:10.0.0.84      0       100     0       ? Or-ID: 10.0.0.84 C-LST: 10.0.0.175 
 * >      RD: 120:5001 IPv6 prefix 2600:50:10:120::/64
                                 ::ffff:10.0.0.120     0       100     0       ? Or-ID: 10.0.0.120 C-LST: 10.0.0.175 
 * >      RD: 124:5001 IPv6 prefix 2600:50:10:124::/64
                                 ::ffff:10.0.0.124     0       100     0       ? Or-ID: 10.0.0.124 C-LST: 10.0.0.175 
 * >      RD: 128:5001 IPv6 prefix 2600:50:10:128::/64
                                 ::ffff:10.0.0.128     0       100     0       ? Or-ID: 10.0.0.128 C-LST: 10.0.0.175 
 * >      RD: 131:5001 IPv6 prefix 2600:50:10:131::/64
                                 ::ffff:10.0.0.131     -       100     0       i Or-ID: 10.0.0.131 C-LST: 10.0.0.175 
 * >      RD: 179:5001 IPv6 prefix 2600:50:10:179::/64
                                 ::ffff:10.0.0.179     -       100     0       i Or-ID: 10.0.0.179 C-LST: 10.0.0.175 
          RD: 214:5001 IPv6 prefix 2600:50:10:214::/64
                                 ::ffff:10.0.0.214     -       100     0       i Or-ID: 10.0.0.214 C-LST: 10.0.0.175 
 * >      RD: 217:5001 IPv6 prefix 2600:50:10:217::/64
                                 ::ffff:10.0.0.217     -       100     0       i Or-ID: 10.0.0.217 C-LST: 10.0.0.175 
 * >      RD: 210:5001 IPv6 prefix 2600:50:10:221::/64
                                 ::ffff:10.0.0.221     -       100     0       i Or-ID: 10.0.0.221 C-LST: 10.0.0.175 
 * >      RD: 120:5001 IPv6 prefix 2600:51:10:120::/64
                                 ::ffff:10.0.0.120     0       100     0       ? Or-ID: 10.0.0.120 C-LST: 10.0.0.175 
```

## show bgp ipv4 labeled-unicast

```text
BGP routing table information for VRF default
Router identifier 10.0.0.31, local AS number 64512
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
  Last read 00:39:44, last write 00:36:44
  Hold time is 180, keepalive interval is 60 seconds
  Configured hold time is 180, keepalive interval is 60 seconds
  Effective minimum hold time is 3 seconds
  Send failure hold time is 0 seconds
  Hold timer is inactive
  Keepalive timer is inactive
  Connect timer is active, time left: 00:00:05
  Connection interval is 148 seconds
  Failed connection attempts is 20
  Idle-restart timer is inactive
  BGP state is Active
  Number of transitions to established: 1
  Last state was Connect
  Last event was TransportError
  Last sent notification:Hold Timer Expired Error/None, Last time 00:36:44
  Last sent socket-error:Connect (Network is unreachable), Last time 00:02:23, First time 00:36:43, Repeats 19
  Types of communities advertised: standard extended large
  Neighbor Capabilities:
    Multiprotocol VPN-IPv4: advertised and received
    Multiprotocol VPN-IPv6: advertised and received
    Four Octet ASN: advertised and received
    Route Refresh: advertised and received
    Enhanced route refresh: advertised and received
    Send End-of-RIB messages: advertised and received
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
    Updates:               14       439
    Keepalives:          1346      1318
    Route Refresh:          0         0
    Total messages:      1362      1758
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
Local AS is 64512, local router ID 10.0.0.31
TTL is 255
Local TCP address is 10.0.0.31
Remote TCP address is 10.0.0.30, remote port is 179

BGP neighbor is 10.0.0.175, remote AS 64512, internal link
 Description: Juniper_175
  BGP version 4, remote router ID 10.0.0.175, VRF default
  Inherits configuration from and member of peer-group IBGP_CLIENT_PEER
  Last read 00:00:25, last write 00:00:24
  Hold time is 90, keepalive interval is 30 seconds
  Configured hold time is 180, keepalive interval is 60 seconds
  Effective minimum hold time is 3 seconds
  Send failure hold time is 0 seconds
  Hold timer is active, time left: 00:01:05
  Keepalive timer is active, time left: 00:00:02
  Connect timer is inactive
  Idle-restart timer is inactive
  BGP state is Established, up for 01:00:20
  Number of transitions to established: 3
  Last state was OpenConfirm
  Last event was ReapplyInboundPolicy
  Last sent notification:Hold Timer Expired Error/None, Last time 01:02:41, First time 12:26:52, Repeats 1
  Last sent socket-error:Connect (Network is unreachable), Last time 01:00:25, First time 12:26:51, Repeats 15
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
      Received 01:00:20
      Number of stale paths removed after graceful restart: 0
    VPN-IPv6 End-of-RIB received: Yes
      Received 01:00:20
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
    Notifications:          2         0
    Updates:               12       236
    Keepalives:          2582      2341
    Route Refresh:          0         0
    Total messages:      2599      2580
  Prefix Statistics:
                                   Sent      Rcvd     Best Paths     Best ECMP Paths
    IPv4 Unicast:                     0         0              0                   0
    VPN-IPv4:                         1        14             12                   0
    IPv6 Unicast:                     0         0              0                   0
    VPN-IPv6:                         1        14             12                   0
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
Local AS is 64512, local router ID 10.0.0.31
TTL is 255
Local TCP address is 10.0.0.31, local port is 43111
Remote TCP address is 10.0.0.175, remote port is 179
Local next hop for next hop self:
  VPN-IPv4: 10.0.0.31
  VPN-IPv6: ::ffff:10.0.0.31
TCP Socket Information:
  TCP state is ESTABLISHED
  Recv-Q: 0/32768
  Send-Q: 0/46080
  Outgoing Maximum Segment Size (MSS): 1448
  Total Number of TCP retransmissions: 7
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
    Congestion Window (cwnd): 2
    Slow-start Threshold (ssthresh): 7
    TCP Throughput: 45.43 Mbps
    Advertised Recv Window (rcv_space): 14480

```

## show tunnel rib system-tunnel-rib brief

```text
Tunnel RIB: system-tunnel-rib
Endpoint      Tunnel Type Index(es) Tunnel Preference IGP Preference IGP Metric
------------- ----------- --------- ----------------- -------------- ----------
10.0.0.32/32  OSPF SR     4         60                110            21        
10.0.0.66/32  OSPF SR     6         60                110            21        
10.0.0.72/32  OSPF SR     5         60                110            21        
10.0.0.84/32  OSPF SR     7         60                110            12        
10.0.0.120/32 OSPF SR     8         60                110            11        
10.0.0.124/32 OSPF SR     11        60                110            11        
10.0.0.128/32 OSPF SR     10        60                110            11        
10.0.0.131/32 OSPF SR     9         60                110            11        
10.0.0.175/32 OSPF SR     1         60                110            10        
10.0.0.179/32 OSPF SR     12        60                110            11        
10.0.0.217/32 OSPF SR     3         60                110            11        
10.0.0.221/32 OSPF SR     2         60                110            11        

Metric Type
-----------
metric     
metric     
metric     
metric     
metric     
metric     
metric     
metric     
metric     
metric     
metric     
metric     

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
>C    10.0.0.31/32 [0 pref/0 metric] updated 19:41:03 ago
         via Loopback0, directly connected
>C    20.31.175.0/24 [0 pref/0 metric] updated 01:00:36 ago
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
>P    0.0.0.0/8 [1 pref/0 metric] updated 1d02h ago
         via Null0, directly connected [NF]
>P    127.0.0.0/8 [1 pref/0 metric] updated 1d02h ago
         via :: [1 pref/1 metric] type ipv4
            via , directly connected
VRF: default, Protocol: ospf
Codes: C - Connected, S - Static, P - Route Input, G - Gribi
       B - BGP, O - Ospf, O3 - Ospf3, I - Isis, R - Rip, VL - VRF Leak
       > - Best Route, * - Unresolved Next hop
       EM - Exact match of the SR-TE Policy
       NM - Null endpoint match of the SR-TE Policy
       AM - Any endpoint match of the SR-TE Policy
       L - Part of a recursive route resolution loop
       A - Next hop not resolved in ARP/ND
       NF - Not in FEC
>O    10.0.0.32/32 [110 pref/21 metric] updated 00:36:59 ago
         via 20.31.175.175, Ethernet5
>O    10.0.0.66/32 [110 pref/21 metric] updated 00:36:06 ago
         via 20.31.175.175, Ethernet5
>O    10.0.0.72/32 [110 pref/21 metric] updated 00:36:43 ago
         via 20.31.175.175, Ethernet5
>O    10.0.0.84/32 [110 pref/12 metric] updated 00:34:13 ago
         via 20.31.175.175, Ethernet5
>O    10.0.0.120/32 [110 pref/11 metric] updated 00:30:27 ago
         via 20.31.175.175, Ethernet5
>O    10.0.0.124/32 [110 pref/11 metric] updated 00:24:51 ago
         via 20.31.175.175, Ethernet5
>O    10.0.0.128/32 [110 pref/11 metric] updated 00:25:08 ago
         via 20.31.175.175, Ethernet5
>O    10.0.0.131/32 [110 pref/11 metric] updated 00:33:37 ago
         via 20.31.175.175, Ethernet5
>O    10.0.0.175/32 [110 pref/10 metric] updated 00:37:23 ago
         via 20.31.175.175, Ethernet5
>O    10.0.0.179/32 [110 pref/11 metric] updated 00:08:13 ago
         via 20.31.175.175, Ethernet5
>O    10.0.0.184/32 [110 pref/11 metric] updated 00:02:55 ago
         via 20.31.175.175, Ethernet5
>O    10.0.0.214/32 [110 pref/11 metric] updated 00:30:14 ago
         via 20.31.175.175, Ethernet5
>O    10.0.0.217/32 [110 pref/11 metric] updated 00:37:13 ago
         via 20.31.175.175, Ethernet5
>O    10.0.0.221/32 [110 pref/11 metric] updated 00:37:23 ago
         via 20.31.175.175, Ethernet5
>O    20.32.175.0/24 [110 pref/11 metric] updated 00:37:23 ago
         via 20.31.175.175, Ethernet5
>O    20.53.175.0/24 [110 pref/11 metric] updated 00:37:23 ago
         via 20.31.175.175, Ethernet5
>O    20.66.175.0/24 [110 pref/11 metric] updated 00:37:23 ago
         via 20.31.175.175, Ethernet5
>O    20.72.175.0/24 [110 pref/11 metric] updated 00:37:23 ago
         via 20.31.175.175, Ethernet5
>O    20.84.175.0/24 [110 pref/11 metric] updated 00:37:23 ago
         via 20.31.175.175, Ethernet5
>O    20.120.175.0/24 [110 pref/11 metric] updated 00:37:23 ago
         via 20.31.175.175, Ethernet5
>O    20.124.175.0/24 [110 pref/11 metric] updated 00:37:23 ago
         via 20.31.175.175, Ethernet5
>O    20.128.175.0/24 [110 pref/11 metric] updated 00:37:23 ago
         via 20.31.175.175, Ethernet5
>O    20.131.175.0/24 [110 pref/11 metric] updated 00:37:23 ago
         via 20.31.175.175, Ethernet5
>O    20.175.179.0/24 [110 pref/11 metric] updated 00:37:23 ago
         via 20.31.175.175, Ethernet5
>O    20.175.184.0/24 [110 pref/11 metric] updated 00:37:23 ago
         via 20.31.175.175, Ethernet5
>O    20.175.214.0/24 [110 pref/11 metric] updated 00:37:23 ago
         via 20.31.175.175, Ethernet5
>O    20.175.217.0/24 [110 pref/11 metric] updated 00:37:23 ago
         via 20.31.175.175, Ethernet5
>O    20.175.221.0/24 [110 pref/11 metric] updated 00:37:23 ago
         via 20.31.175.175, Ethernet5
```

## show rib route ipv6

```text
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
>P    ::/96 [1 pref/0 metric] updated 00:39:01 ago
         via Null0, directly connected [NF]
>P    ::ffff:127.0.0.0/104 [1 pref/0 metric] updated 00:39:01 ago
         via :: [1 pref/1 metric] type ipv6
            via , directly connected
>P    fe80::/10 [1 pref/0 metric] updated 00:39:01 ago
```

## show platform sand l3 summary

```text
Number of vrfs: 3

Ipv4:
  Routes:       64  backlog:  0  unprogrammed:  0
  Adjacencies:  64  backlog:  0  unprogrammed:  0
Ipv6:
  Routes:       23  backlog:  0  unprogrammed:  0
  Adjacencies:  64  backlog:  0  unprogrammed:  0
Mpls:
  Routes:       13  backlog:  0  unprogrammed:  0
  Adjacencies:  1   backlog:  0  unprogrammed:  0

Jericho2 Ip Fecs:
  Non-ecmp fecs:  4131  ecmp fecs:  0  fec entries:  4131
Jericho2 Mpls Fecs:
  Non-ecmp fecs:  1  ecmp fecs:  0  fec entries:  1
Jericho2 Vxlan Tunnel Fecs:
  Non-ecmp fecs:  0  ecmp fecs:  0  fec entries:  0
  Number of vxlan tunnels configured: 0

Jericho2 Lpm Routes:
  Routes:   64  unprogrammed:   0   
  Routes6:  23  unprogrammed6:  0   
  Backlog:  0 

Jericho2 Lpm:
  TCAM entries used:   4   Percent free:  99  ADS2 entries used:   5  Percent free:  99
  Pivot buckets used:  5   Rows used:     2   Entries Per Bucket:  1  Percent free:  99
  Route buckets used:  18  Rows used:     4   Entries Per Bucket:  4  Percent free:  99

Lem:
  IPv4  Host in Lem:            disabled
  IPv4  Prefix-lengths in Lem:  None    
  IPv6  Host in Lem:            disabled
  IPv6  Prefix-lengths in Lem:  None    
  Number of downloads:        0
  Number of overflow events:  0

Egress Arp rewrite entries in use (in each fap):
  FixedSystem: 3
Egress Arp remote rewrite entries in use (in each fap):
  FixedSystem: 0
Egress Ip tunnel rewrite entries in use (in each fap):
  FixedSystem: 0
Egress Mpls (for outer 2 labels) rewrite entries in use (in each fap):
  FixedSystem: 0
Egress Mpls (for inner 2 labels) rewrite entries in use (in each fap):
  FixedSystem: 18
Egress Sflow rewrite entries in use (in each fap):
  FixedSystem: 0

Egress rewrite chains in backlog: resource-full 0, no-interface 0

Glem entries used per fap :
  FixedSystem: 4117

Jericho2 Fec:
  Maximum FEC hierarchy levels:  2
  ReusedEcmp:  0  allocs:  292  frees:  259  shuffles:  0  cmds:  0
  Zombies:     0    purges:    0
  Quarantine:  0/0  shuffles:  0  deletes:  0   
  Preserved FECs: 0
    First FEC preserved: never
    Last FEC preserved: never
  Fec insertion failures:  0
  Level1  Fecs:
    Non-ecmp fecs:            22  ecmp fecs:            1 
    Non-ecmp (Percent free):  99  ecmp (Percent free):  99
  Level2  Fecs:
    Non-ecmp fecs:            11  ecmp fecs:            0  
    Non-ecmp (Percent free):  99  ecmp (Percent free):  100
  Level3  Fecs:
    Non-ecmp fecs:            0    ecmp fecs:            0  
    Non-ecmp (Percent free):  100  ecmp (Percent free):  100

Lpm Detail:
  Requests:  1441  cleanses:  463  batches:  463  avg batch size:  3

Jericho Arp:
  ArpTable writes:      27738  queued      0   
  IngressTable writes:  78101  queued      0   
  Coprocessors:         1      in CmdRing

Tunnel Counter Status
  Number of MPLS tunnels:                  18   
  Number of uncountable MPLS tunnels:      18   
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
|0  |10.0.0.31/32      |TRAP | CoppSystemIpUcast  |0    |  -     | Receive           |  -  |524291|   -   
|0  |10.0.0.32/32      |ROUTE| Et5                |1010 |107518  | 3c:08:cd:8d:ba:f4 |  -  |288371|   -   
|0  |10.0.0.66/32      |ROUTE| Et5                |1010 |107518  | 3c:08:cd:8d:ba:f4 |  -  |288371|   -   
|0  |10.0.0.72/32      |ROUTE| Et5                |1010 |107518  | 3c:08:cd:8d:ba:f4 |  -  |288371|   -   
|0  |10.0.0.84/32      |ROUTE| Et5                |1010 |107518  | 3c:08:cd:8d:ba:f4 |  -  |288371|   -   
|0  |10.0.0.120/32     |ROUTE| Et5                |1010 |107518  | 3c:08:cd:8d:ba:f4 |  -  |288371|   -   
|0  |10.0.0.124/32     |ROUTE| Et5                |1010 |107518  | 3c:08:cd:8d:ba:f4 |  -  |288371|   -   
|0  |10.0.0.128/32     |ROUTE| Et5                |1010 |107518  | 3c:08:cd:8d:ba:f4 |  -  |288371|   -   
|0  |10.0.0.131/32     |ROUTE| Et5                |1010 |107518  | 3c:08:cd:8d:ba:f4 |  -  |288371|   -   
|0  |10.0.0.175/32     |ROUTE| Et5                |1010 |107518  | 3c:08:cd:8d:ba:f4 |  -  |288371|   -   
|0  |10.0.0.179/32     |ROUTE| Et5                |1010 |107518  | 3c:08:cd:8d:ba:f4 |  -  |288371|   -   
|0  |10.0.0.184/32     |ROUTE| Et5                |1010 |107518  | 3c:08:cd:8d:ba:f4 |  -  |288371|   -   
|0  |10.0.0.214/32     |ROUTE| Et5                |1010 |107518  | 3c:08:cd:8d:ba:f4 |  -  |288371|   -   
|0  |10.0.0.217/32     |ROUTE| Et5                |1010 |107518  | 3c:08:cd:8d:ba:f4 |  -  |288371|   -   
|0  |10.0.0.221/32     |ROUTE| Et5                |1010 |107518  | 3c:08:cd:8d:ba:f4 |  -  |288371|   -   
|0  |20.31.175.0/32    |TRAP | CoppSystemIpBcast  |0    |  -     | BcastReceive      |  -  |524290|   -   
|0  |20.31.175.31/32   |TRAP | CoppSystemIpUcast  |0    |  -     | Receive           |  -  |524291|   -   
|0  |20.31.175.175/32  |ROUTE| Et5                |1010 |107518  | 3c:08:cd:8d:ba:f4 |  -  |288373|   -   
|0  |20.31.175.255/32  |TRAP | CoppSystemIpBcast  |0    |  -     | BcastReceive      |  -  |524290|   -   
|0  |20.31.175.0/24    |TRAP | CoppSystemL3DstMiss|1010 |1010    | ArpTrap           |  -  |525305|   -   
|0  |20.32.175.0/24    |ROUTE| Et5                |1010 |107518  | 3c:08:cd:8d:ba:f4 |  -  |288371|   -   
|0  |20.53.175.0/24    |ROUTE| Et5                |1010 |107518  | 3c:08:cd:8d:ba:f4 |  -  |288371|   -   
|0  |20.66.175.0/24    |ROUTE| Et5                |1010 |107518  | 3c:08:cd:8d:ba:f4 |  -  |288371|   -   
|0  |20.72.175.0/24    |ROUTE| Et5                |1010 |107518  | 3c:08:cd:8d:ba:f4 |  -  |288371|   -   
|0  |20.84.175.0/24    |ROUTE| Et5                |1010 |107518  | 3c:08:cd:8d:ba:f4 |  -  |288371|   -   
|0  |20.120.175.0/24   |ROUTE| Et5                |1010 |107518  | 3c:08:cd:8d:ba:f4 |  -  |288371|   -   
|0  |20.124.175.0/24   |ROUTE| Et5                |1010 |107518  | 3c:08:cd:8d:ba:f4 |  -  |288371|   -   
|0  |20.128.175.0/24   |ROUTE| Et5                |1010 |107518  | 3c:08:cd:8d:ba:f4 |  -  |288371|   -   
|0  |20.131.175.0/24   |ROUTE| Et5                |1010 |107518  | 3c:08:cd:8d:ba:f4 |  -  |288371|   -   
|0  |20.175.179.0/24   |ROUTE| Et5                |1010 |107518  | 3c:08:cd:8d:ba:f4 |  -  |288371|   -   
|0  |20.175.184.0/24   |ROUTE| Et5                |1010 |107518  | 3c:08:cd:8d:ba:f4 |  -  |288371|   -   
|0  |20.175.214.0/24   |ROUTE| Et5                |1010 |107518  | 3c:08:cd:8d:ba:f4 |  -  |288371|   -   
|0  |20.175.217.0/24   |ROUTE| Et5                |1010 |107518  | 3c:08:cd:8d:ba:f4 |  -  |288371|   -   
|0  |20.175.221.0/24   |ROUTE| Et5                |1010 |107518  | 3c:08:cd:8d:ba:f4 |  -  |288371|   -   
|0  |127.0.0.0/8       |TRAP | CoppSystemL3DstMiss|0    |  -     | ArpTrap           |  -  |524295|   -   
|0  |0.0.0.0/0         |TRAP | CoppSystemL3LpmOver|0    |  -     | SlowReceive       |  -  |524293|   -   
|1  |0.0.0.0/8         |DROP | DROP               |0    |  -     |                   |  -  |288361|   -   
|1  |127.0.0.0/8       |TRAP | CoppSystemL3DstMiss|0    |  -     | ArpTrap           |  -  |524295|   -   
|1  |192.168.20.0/32   |TRAP | CoppSystemIpBcast  |0    |  -     | BcastReceive      |  -  |524290|   -   
|1  |192.168.20.31/32  |TRAP | CoppSystemIpUcast  |0    |  -     | Receive           |  -  |524291|   -   
|1  |192.168.21.255/32 |TRAP | CoppSystemIpBcast  |0    |  -     | BcastReceive      |  -  |524290|   -   
|1  |192.168.20.0/23   |TRAP | CoppSystemL3DstMiss|0    |  -     | ArpTrap           |  -  |524295|   -   
|1  |0.0.0.0/0         |TRAP | CoppSystemL3DstMiss|0    |  -     | ArpTrap           |  -  |524295|   -   
|2  |0.0.0.0/8         |DROP | DROP               |0    |  -     |                   |  -  |288365|   -   
|2  |50.10.31.0/32     |TRAP | CoppSystemIpBcast  |0    |  -     | BcastReceive      |  -  |524290|   -   
|2  |50.10.31.1/32     |TRAP | CoppSystemIpUcast  |0    |  -     | Receive           |  -  |524291|   -   
|2  |50.10.31.2/32     |ROUTE| Et40               |1008 |107520  | 00:14:01:00:00:01 |  -  |288369|   -   
|2  |50.10.31.255/32   |TRAP | CoppSystemIpBcast  |0    |  -     | BcastReceive      |  -  |524290|   -   
|2  |50.10.31.0/24     |TRAP | CoppSystemL3DstMiss|1008 |1008    | ArpTrap           |  -  |525303|   -   
|2  |50.10.32.0/24     |ROUTE| FEC 288372         |0    |2097149 | 00:00:00:00:00:00 |  -  |91754 |M 20032 378528
|2  |50.10.66.0/24     |ROUTE| FEC 288372         |0    |2097147 | 00:00:00:00:00:00 |  -  |91756 |M 20066 62000
|2  |50.10.72.0/24     |ROUTE| FEC 288372         |0    |2097150 | 00:00:00:00:00:00 |  -  |91755 |M 20072 62002
|2  |50.10.84.0/24     |ROUTE| FEC 288372         |0    |2097146 | 00:00:00:00:00:00 |  -  |91757 |M 20084 720896
|2  |50.10.120.0/24    |ROUTE| FEC 288372         |0    |2097145 | 00:00:00:00:00:00 |  -  |91758 |M 20120 1277
|2  |50.10.124.0/24    |ROUTE| FEC 288372         |0    |2097142 | 00:00:00:00:00:00 |  -  |91761 |M 20124 332
|2  |50.10.128.0/24    |ROUTE| FEC 288372         |0    |2097143 | 00:00:00:00:00:00 |  -  |91760 |M 20128 48060
|2  |50.10.131.0/24    |ROUTE| FEC 288372         |0    |2097144 | 00:00:00:00:00:00 |  -  |91759 |M 20131 18
|2  |50.10.179.0/24    |ROUTE| FEC 288372         |0    |2097141 | 00:00:00:00:00:00 |  -  |91762 |M 20179 16
|2  |50.10.217.0/24    |ROUTE| FEC 288372         |0    |2097148 | 00:00:00:00:00:00 |  -  |91753 |M 20217 524287
|2  |50.10.221.0/24    |ROUTE| FEC 288372         |0    |2097151 | 00:00:00:00:00:00 |  -  |91752 |M 21221 524289
|2  |51.10.120.0/24    |ROUTE| FEC 288372         |0    |2097145 | 00:00:00:00:00:00 |  -  |91758 |M 20120 1277
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
|  -  |91752 |ROUTE| FEC 288372         |   - |2097151 |                 - |Mpush 21221 524289
|  -  |91753 |ROUTE| FEC 288372         |   - |2097148 |                 - |Mpush 20217 524287
|  -  |91754 |ROUTE| FEC 288372         |   - |2097149 |                 - |Mpush 20032 378528
|  -  |91755 |ROUTE| FEC 288372         |   - |2097150 |                 - |Mpush 20072 62002
|  -  |91756 |ROUTE| FEC 288372         |   - |2097147 |                 - |Mpush 20066 62000
|  -  |91757 |ROUTE| FEC 288372         |   - |2097146 |                 - |Mpush 20084 720896
|  -  |91758 |ROUTE| FEC 288372         |   - |2097145 |                 - |Mpush 20120 1277
|  -  |91759 |ROUTE| FEC 288372         |   - |2097144 |                 - |Mpush 20131 18
|  -  |91760 |ROUTE| FEC 288372         |   - |2097143 |                 - |Mpush 20128 48060
|  -  |91761 |ROUTE| FEC 288372         |   - |2097142 |                 - |Mpush 20124 332
|  -  |91762 |ROUTE| FEC 288372         |   - |2097141 |                 - |Mpush 20179 16
|  -  |91763 |ROUTE| FEC 288372         |   - |2097141 |                 - |Mpush 20179 16
|  -  |91764 |ROUTE| FEC 288372         |   - |2097151 |                 - |Mpush 21221 524289
|  -  |91765 |ROUTE| FEC 288372         |   - |2097140 |                 - |Mpush 20120 1276
|  -  |91766 |ROUTE| FEC 288372         |   - |2097139 |                 - |Mpush 20084 720897
|  -  |91767 |ROUTE| FEC 288372         |   - |2097138 |                 - |Mpush 20128 48061
|  -  |91768 |ROUTE| FEC 288372         |   - |2097144 |                 - |Mpush 20131 18
|  -  |91769 |ROUTE| FEC 288372         |   - |2097137 |                 - |Mpush 20072 62003
|  -  |91770 |ROUTE| FEC 288372         |   - |2097148 |                 - |Mpush 20217 524287
|  -  |91771 |ROUTE| FEC 288372         |   - |2097136 |                 - |Mpush 20032 378529
|  -  |91772 |ROUTE| FEC 288372         |   - |2097135 |                 - |Mpush 20066 62001
|  -  |91773 |ROUTE| FEC 288372         |   - |2097134 |                 - |Mpush 20124 333
|  -  |288360|DROP | DROP               |0    |  -     |                   |   -   
|  -  |288361|DROP | DROP               |0    |  -     |                   |   -   
|  -  |288365|DROP | DROP               |0    |  -     |                   |   -   
|  -  |288369|ROUTE| Et40               |1008 |107520  | 00:14:01:00:00:01 |   -   
|  -  |288370|ROUTE| Et40               |1009 |107521  | 00:27:01:00:00:01 |   -   
|  -  |288371|ROUTE| Et5                |1010 |107518  | 3c:08:cd:8d:ba:f4 |   -   
|  -  |288372|ROUTE| Et5                |1010 |107518  | 3c:08:cd:8d:ba:f4 |   -   
|  -  |288373|ROUTE| Et5                |1010 |107518  | 3c:08:cd:8d:ba:f4 |   -   
|  -  |288374|ROUTE| Et5                |1010 |107518  | 3c:08:cd:8d:ba:f4 |   -   
|  -  |288375|DROP | DROP               |0    |  -     |                   |   -   
|  -  |288379|DROP | DROP               |0    |  -     |                   |   -   
|  -  |524290|TRAP | CoppSystemIpBcast  |0    |  -     | BcastReceive      |   -   
|  -  |524291|TRAP | CoppSystemIpUcast  |0    |  -     | Receive           |   -   
|  -  |524293|TRAP | CoppSystemL3LpmOver|0    |  -     | SlowReceive       |   -   
|  -  |524295|TRAP | CoppSystemL3DstMiss|0    |  -     | ArpTrap           |   -   
|  -  |525303|TRAP | CoppSystemL3DstMiss|1008 |1008    | ArpTrap           |   -   
|  -  |525304|TRAP | CoppSystemL3DstMiss|1009 |1009    | ArpTrap           |   -   
|  -  |525305|TRAP | CoppSystemL3DstMiss|1010 |1010    | ArpTrap           |   -   

```

