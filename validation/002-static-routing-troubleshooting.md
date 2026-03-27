# Lab 17: Routing Protocol Behavior & Failover Analysis

## 🎯 Objective
- Compare routing protocol behavior (RIP, OSPF, EIGRP)
- Observe route selection and failover
- Validate loopback advertisement and adjacency behavior

---

## 🧠 Scenario
A multi-router topology is configured using multiple routing protocols.
The lab evaluates:
- Protocol route selection (AD, metric)
- Failover behavior when links go down
- Loopback reachability and advertisement
- Effect of passive interfaces on adjacency

---

## 🏗️ Topology Overview
Devices:
- R1–R5
- PC1–PC3
![Topology](../diagrams/002-static-routing-topology.jpg)

Networks:
- 10.0.0.0/24 – 10.0.3.0/24
- 10.1.0.0/24 – 10.1.3.0/24
- Loopbacks: 192.168.0.1-5/32

---

# =========================
# 🔹 PHASE 1 – RIP BASELINE
# =========================

## Configuration
- RIP enabled on all routers

## Verification
```bash
show ip route


