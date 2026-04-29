# Enterprise EIGRP Dual-AS Lab with Mutual Redistribution

## 📌 Project Overview
This project demonstrates a complex enterprise network architecture using **Cisco EIGRP**. The lab features a dual Autonomous System (AS) design, focusing on high availability, traffic engineering, and route propagation between different routing domains.



## 🛠️ Network Architecture & Features
- **Dual Autonomous Systems:** Split into `AS 1` and `AS 2` to simulate separate corporate departments or geographical locations.
- **Mutual Redistribution:** Configured on **R5** and **R6** (ASBRs) to ensure full reachability between both domains.
- **Redundancy & High Availability:** Dual boundary routers (R5/R6) and multiple paths between distribution layers to prevent single points of failure.
- **Traffic Engineering:** Manual metric manipulation using `Bandwidth` and `Delay` to influence EIGRP Successor and Feasible Successor selection.
- **Infrastructure Services:** Integrated **DHCP Pools** for end-user networks (Net50, Net60, Net70, Net80).
- **Security Best Practices:** Use of `passive-interface` on LAN-facing interfaces to optimize performance and security.

## 📂 Repository Structure
- **/configs:** Contains the running configurations for all 10 routers (`R1.cfg` to `R10.cfg`).
- **topology.png:** High-resolution diagram of the network lab.

## 🚀 Key Technologies Used
- Cisco IOS (EIGRP Routing)
- Route Redistribution
- DHCP (Dynamic Host Configuration Protocol)
- Metric Weights & Vector Metrics
- HSRP/VRRP (Conceptualized in the 3-Tier design)

## 📝 How to Use
1. Clone the repository.
2. Load the `.cfg` files into your terminal or network simulator (GNS3/CML/EVE-NG).
3. Verify adjacency using `show ip eigrp neighbors`.
4. Test end-to-end connectivity using `ping` and `traceroute`.

---
**Designed by: [ضع اسمك هنا]** *IT Professional | Network Engineering Enthusiast*
