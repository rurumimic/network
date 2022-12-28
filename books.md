# Books

### Computer Networking: A Top-Down Approach, 7th Edition

[Computer Networking: A Top-Down Approach](https://gaia.cs.umass.edu/kurose_ross/index.php), by James Kurose & Keith Ross.

- [Online lectures](https://gaia.cs.umass.edu/kurose_ross/lectures.php)

1. Computer Networks and the Internet
1. Application Layer
1. Transport Layer
1. The Network Layer: Data Plane
1. The Network Layer: Control Plane
1. The Link Layer: Links, Access Networks, and LANs
1. Wireless and Mobile Networks
1. Security in Computer Networks
1. Multimedia Networking

### Understanding Linux Network Internals

[Understanding Linux Network Internals](https://www.oreilly.com/library/view/understanding-linux-network/0596002556/), by Christian Benvenuti. Copyright 2006 O’Reilly Media, Inc., 0-596-00255-6.

#### I. General Background

1. Introduction
   1. Basic Terminology
   2. Common Coding Patterns
   3. User-Space Tools
   4. Browsing the Source Code
   5. When a Feature Is Offered as a Patch
2. Critical Data Structures
   1. The Socket Buffer: sk_buff Structure
   2. net_device Structure
   3. Files Mentioned in This Chapter
1. User-Space-to-Kernel Interface
   1. Overview
   2. procfs Versus sysctl
   3. ioctl
   4. Netlink
   5. Serializing Configuration Changes

#### II. System Initialization

1. Notification Chains
   1. Reasons for Notification Chains
   2. Overview
   3. Defining a Chain
   4. Registering with a Chain
   5. Notifying Events on a Chain
   6. Notification Chains for the Networking Subsystems
   7. Tuning viaChapter /proc Filesystem
   8. Functions and Variables Featured in This Chapter
   9. Files and Directories Featured in This Chapter
1. Network Device Initialization
   1. System Initialization Overview
   2. Device Registration and Initialization
   3. Basic Goals of NIC Initialization
   4. Interaction Between Devices and Kernel
   5. Initialization Options
   6. Module Options
   7. Initializing the Device Handling Layer: net_dev_init
   8. User-Space Helpers
   9. Virtual Devices
   10. Tuning via /proc Filesystem
   11. Functions and Variables Featured in This Chapter
   12. Files and Directories Featured in This Chapter
1. The PCI Layer and Network Interface Cards
   1. Data Structures Featured in This Chapter
   2. Registering a PCI NIC Device Driver
   3. Power Management and Wake-on-LAN
   4. Example of PCI NIC Driver Registration
   5. The Big Picture
   6. Tuning via /proc Filesystem
   7. Functions and Variables Featured in This Chapter
   8. Files and Directories Featured in This Chapter
1. Kernel Infrastructure for Component Initialization
   1. Boot-Time Kernel Options
   2. Module Initialization Code
   3. Optimized Macro-Based Tagging
   4. Boot-Time Initialization Routines
   5. Memory Optimizations
   6. Tuning via /proc Filesystem
   7. Functions and Variables Featured in This Chapter
   8. Files and Directories Featured in This Chapter
1. Device Registration and Initialization
   1. When a Device Is Registered
   2. When a Device Is Unregistered
   3. Allocating net_device Structures
   4. Skeleton of NIC Registration and Unregistration
   5. Device Initialization
   6. Organization of net_device Structures
   7. Device State
   8. Registering and Unregistering Devices
   9. Device Registration
   10. Device Unregistration
   11. Enabling and Disabling a Network Device
   12. Updating the Device Queuing Discipline State
   13. Configuring Device-Related Information from User Space
   14. Virtual Devices
   15. Locking
   16. Tuning via /proc Filesystem
   17. Functions and Variables Featured in This Chapter
   18. Files and Directories Featured in This Chapter

#### III. Transmission and Reception

1. Interrupts and Network Drivers
   1. Decisions and Traffic Direction
   2. Notifying Drivers When Frames Are Received
   3. Interrupt Handlers
   4. softnet_data Structure
1. Frame Reception
   1. Interactions with Other Features
   2. Enabling and Disabling a Device
   3. Queues
   4. Notifying the Kernel of Frame Reception: NAPI and netif_rx
   5. Old Interface Between Device Drivers and Kernel: First Part of netif_rx
   6. Congestion Management
   7. Processing the NET_RX_SOFTIRQ: net_rx_action
1. Frame Transmission
   1. Enabling and Disabling Transmissions
1. General and Reference Material About Interrupts
   1. Statistics
   2. Tuning via /proc and sysfs Filesystems
   3. Functions and Variables Featured in This Part of the Book
   4. Files and Directories Featured in This Part of the Book
1. Protocol Handlers
   1. Overview of Network Stack
   2. Executing the Right Protocol Handler
   3. Protocol Handler Organization
   4. Protocol Handler Registration
   5. Ethernet Versus IEEE
   6. Tuning via /proc Filesystem
   7. Functions and Variables Featured in This Chapter
   8. Files and Directories Featured in This Chapter

#### IV. Bridging

1. Bridging: Concepts
   1. Repeaters, Bridges, and Routers
   2. Bridges Versus Switches
   3. Hosts
   4. Merging LANs with Bridges
   5. Bridging Different LAN Technologies
   6. Address Learning
   7. Multiple Bridges
1. Bridging: The Spanning Tree Protocol
   1. Basic Terminology
   2. Example of Hierarchical Switched L2 Topology
   3. Basic Elements of the Spanning Tree Protocol
   4. Bridge and Port IDs
   5. Bridge Protocol Data Units (BPDUs)
   6. Defining the Active Topology
   7. Timers
   8. Topology Changes
   9. BPDU Encapsulation
   10. Transmitting Configuration BPDUs
   11. Processing Ingress Frames
   12. Convergence Time
   13. Overview of Newer Spanning Tree Protocols
1. Bridging: Linux Implementation
   1. Bridge Device Abstraction
   2. Important Data Structures
   3. Initialization of Bridging Code
   4. Creating Bridge Devices and Bridge Ports
   5. Creating a New Bridge Device
   6. Bridge Device Setup Routine
   7. Deleting a Bridge
   8. Adding Ports to a Bridge
   9. Enabling and Disabling a Bridge Device
   10. Enabling and Disabling a Bridge Port
   11. Changing State on a Bridge Port
   12. The Big Picture
   13. Forwarding Database
   14. Handling Ingress Traffic
   15. Transmitting on a Bridge Device
   16. Spanning Tree Protocol (STP)
   17. netdevice Notification Chain
1. Bridging: Miscellaneous Topics
   1. User-Space Configuration Tools
   2. Tuning via /proc Filesystem
   3. Tuning via /sys Filesystem
   4. Statistics
   5. Data Structures Featured in This Part of the Book
   6. Functions and Variables Featured in This Part of the Book
   7. Files and Directories Featured in This Part of the Book

#### V. Internet Protocol Version 4 (IPv4)

1. Internet Protocol Version 4 (IPv4): Concepts
   1. IP Protocol: The Big Picture
   2. IP Header
   3. IP Options
   4. Packet Fragmentation/Defragmentation
   5. Checksums
1. Internet Protocol Version 4 (IPv4): Linux Foundations and Features
   1. Main IPv4 Data Structures
   2. General Packet Handling
   3. IP Options
1. Internet Protocol Version 4 (IPv4): Forwarding and Local Delivery
   1. Forwarding
   2. Local Delivery
1. Internet Protocol Version 4 (IPv4): Transmission
   1. Key Functions That Perform Transmission
   2. Interface to the Neighboring Subsystem
1. Internet Protocol Version 4 (IPv4): Handling Fragmentation
   1. IP Fragmentation
   2. IP Defragmentation
1. Internet Protocol Version 4 (IPv4): Miscellaneous Topics
   1. Long-Living IP Peer Information
   2. Selecting the IP Header’s ID Field
   3. IP Statistics
   4. IP Configuration
   5. IP-over-IP
   6. IPv4: What’s Wrong with It?
   7. Tuning via /proc Filesystem
   8. Data Structures Featured in This Part of the Book
   9. Functions and Variables Featured in This Part of the Book
   10. Files and Directories Featured in This Part of the Book
1. Layer Four Protocol and Raw IP Handling
   1. Available L4 Protocols
   2. L4 Protocol Registration
   3. L3 to L4 Delivery: ip_local_deliver_finish
   4. IPv4 Versus IPv6
   5. Tuning via /proc Filesystem
   6. Functions and Variables Featured in This Chapter
   7. Files and Directories Featured in This Chapter
1. Internet Control Message Protocol (ICMPv4)
   1. ICMP Header
   2. ICMP Payload
   3. ICMP Types
   4. Applications of the ICMP Protocol
   5. The Big Picture
   6. Protocol Initialization
   7. Data Structures Featured in This Chapter
   8. Transmitting ICMP Messages
   9. ICMP Statistics
   10. Passing Error Notifications to the Transport Layer
   11. Tuning via /proc Filesystem
   12. Functions and Variables Featured in This Chapter
   13. Files and Directories Featured in This Chapter

#### VI. Neighboring Subsystem

1. Neighboring Subsystem: Concepts
   1. What Is a Neighbor?
   2. Reasons That Neighboring Protocols Are Needed
   3. Linux Implementation
   4. Proxying the Neighboring Protocol
   5. When Solicitation Requests Are Transmitted and Processed
   6. Neighbor States and Network Unreachability Detection (NUD)
1. Neighboring Subsystem: Infrastructure
   1. Main Data Structures
   2. Common Interface Between L3 Protocols and Neighboring Protocols
   3. General Tasks of the Neighboring Infrastructure
   4. Reference Counts on neighbour Structures
   5. Creating a neighbour Entry
   6. Neighbor Deletion
   7. Acting As a Proxy
   8. L2 Header Caching
   9. Protocol Initialization and Cleanup
   10. Interaction with Other Subsystems
   11. Interaction Between Neighboring Protocols and L3 Transmission Functions
   12. Queuing
1. Neighboring Subsystem: Address Resolution Protocol (ARP)
   1. ARP Packet Format
   2. Example of an ARP Transaction
   3. Gratuitous ARP
   4. Responding from Multiple Interfaces
   5. Tunable ARP Options
   6. ARP Protocol Initialization
   7. Initialization of a neighbour Structure
   8. Transmitting and Receiving ARP Packets
   9. Processing Ingress ARP Packets
   10. Proxy ARP
   11. Examples
   12. External Events
   13. ARPD
   14. Reverse Address Resolution Protocol (RARP)
   15. Improvements in ND (IPv6) over ARP (IPv4)
1. Neighboring Subsystem: Miscellaneous Topics
   1. System Administration of Neighbors
   2. Tuning via /proc Filesystem
   3. Data Structures Featured in This Part of the Book
   4. Files and Directories Featured in This Part of the Book

#### VII. Routing

1. Routing: Concepts
   1. Routers, Routes, and Routing Tables
   2. Essential Elements of Routing
   3. Routing Table
   4. Lookups
   5. Packet Reception Versus Packet Transmission
1. Routing: Advanced
   1. Concepts Behind Policy Routing
   2. Concepts Behind Multipath Routing
   3. Interactions with Other Kernel Subsystems
   4. Routing Protocol Daemons
   5. Verbose Monitoring
   6. ICMP_REDIRECT Messages
   7. Reverse Path Filtering
1. Routing: Li nux Implementation
   1. Kernel Options
   2. Main Data Structures
   3. Route and Address Scopes
   4. Primary and Secondary IP Addresses
   5. Generic Helper Routines and Macros
   6. Global Locks
   7. Routing Subsystem Initialization
   8. External Events
   9. Interactions with Other Subsystems
1. Routing: The Routing Cache
   1. Routing Cache Initialization
   2. Hash Table Organization
   3. Major Cache Operations
   4. Multipath Caching
   5. Interface Between the DST and Calling Protocols
   6. Flushing the Routing Cache
   7. Garbage Collection
   8. Egress ICMP REDIRECT Rate Limiting
1. Routing: Routing Tables
   1. Organization of Routing Hash Tables
   2. Routing Table Initialization
   3. Adding and Removing Routes
   4. Policy Routing and Its Effects on Routing Table Definitions
1. Routing: Lookups
   1. High-Level View of Lookup Functions
   2. Helper Routines
   3. The Table Lookup: fn_hash_lookup
   4. fib_lookup Function
   5. Setting Functions for Reception and Transmission
   6. General Structure of the Input and Output Routing Routines
   7. Input Routing
   8. Output Routing
   9. Effects of Multipath on Next Hop Selection
   10. Policy Routing
   11. Source Routing
   12. Policy Routing and Routing Table Based Classifier
1. Routing: Miscellaneous Topics
   1. User-Space Configuration Tools
   2. Statistics
   3. Tuning via /proc Filesystem
   4. Enabling and Disabling Forwarding
   5. Data Structures Featured in This Part of the Book
   6. Functions and Variables Featured in This Part of the Book
   7. Files and Directories Featured in This Part of the Book
