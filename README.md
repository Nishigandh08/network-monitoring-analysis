# network-monitoring-analysis
Network Monitoring and Performance Analysis using Cisco Packet Tracer
# 🌐 Network Monitoring and Performance Analysis

![Cisco Packet Tracer](https://img.shields.io/badge/Tool-Cisco%20Packet%20Tracer-blue)
![Course](https://img.shields.io/badge/Course-Computer%20Networking-green)
![Status](https://img.shields.io/badge/Status-Completed-success)

---

## 📋 Project Description

This project demonstrates **Network Monitoring and Performance Analysis** using Cisco Packet Tracer. It involves monitoring network traffic, analyzing performance metrics, identifying bottlenecks, detecting faults, and ensuring optimal network availability and efficiency in a simulated environment.

---

## 🛠️ Tools Used

- **Cisco Packet Tracer** — Network Simulation
- **Ping Command** — Connectivity Testing
- **Traceroute Command** — Performance Analysis
- **Simulation Mode** — Packet Capture & Traffic Analysis

---

## 🖥️ Network Topology

```
Network 1 (192.168.1.0/24)        WAN (10.0.0.0/30)        Network 2 (192.168.2.0/24)

  [PC1] [PC2] [PC3]                                        [PC4] [PC5] [PC6] [PC7]
        |                                                          |
    [Switch1]                                                  [Switch2]
        |                                                          |
    [Router1] ──────────── Gig Link ──────────── [Router2]
   192.168.1.1   10.0.0.1              10.0.0.2   192.168.2.1
```

---

## 📡 IP Address Plan

### Network 1 — 192.168.1.0/24
| Device  | IP Address    | Gateway     |
|---------|--------------|-------------|
| Router1 | 192.168.1.1  | —           |
| PC1     | 192.168.1.10 | 192.168.1.1 |
| PC2     | 192.168.1.11 | 192.168.1.1 |
| PC3     | 192.168.1.12 | 192.168.1.1 |

### WAN Link — 10.0.0.0/30
| Device  | IP Address | 
|---------|-----------|
| Router1 | 10.0.0.1  |
| Router2 | 10.0.0.2  |

### Network 2 — 192.168.2.0/24
| Device  | IP Address    | Gateway     |
|---------|--------------|-------------|
| Router2 | 192.168.2.1  | —           |
| PC4     | 192.168.2.10 | 192.168.2.1 |
| PC5     | 192.168.2.11 | 192.168.2.1 |
| PC6     | 192.168.2.12 | 192.168.2.1 |
| PC7     | 192.168.2.13 | 192.168.2.1 |

---

## 📝 Project Steps

| Step | Description | Status |
|------|-------------|--------|
| Step 1 | Build Network Topology | ✅ Done |
| Step 2 | Assign IP Addresses | ✅ Done |
| Step 3 | Configure Routers | ✅ Done |
| Step 4 | Configure Servers | ✅ Done |
| Step 5 | Test Basic Connectivity (Ping) | ✅ Done |
| Step 6 | Analyze Traffic — Simulation Mode | ✅ Done |
| Step 7 | Performance Analysis — Traceroute | ✅ Done |
| Step 8 | Fault Simulation & Detection | ✅ Done |
| Step 9 | Project Report | ✅ Done |

---

## 📊 Key Results

### Ping Test Results
| Source | Destination | Packet Loss | Status |
|--------|------------|-------------|--------|
| PC1 | PC4 (192.168.2.10) | 0% | ✅ Success |
| PC1 | PC5 (192.168.2.11) | 0% | ✅ Success |
| PC1 | PC6 (192.168.2.12) | 0% | ✅ Success |
| PC1 | PC7 (192.168.2.13) | 0% | ✅ Success |

### Traceroute Results (PC1 → PC7)
| Hop | IP Address   | Latency | Device  |
|-----|-------------|---------|---------|
| 1   | 192.168.1.1 | 1ms     | Router1 |
| 2   | 10.0.0.2    | 0ms     | Router2 |
| 3   | 192.168.2.13| 6ms     | PC7     |

### TTL Analysis
| Device  | TTL Value |
|---------|-----------|
| PC1     | 128       |
| Router1 | 127       |
| Router2 | 126       |
| PC7     | 126       |

---

## 🔴 Fault Simulation Results

| Fault | Cause | Symptom | Resolution |
|-------|-------|---------|------------|
| Fault 1 | Interface Shutdown | Destination host unreachable | no shutdown |
| Fault 2 | Wrong Default Gateway | Request timed out | Correct gateway |
| Fault 3 | Wrong IP Address | Request timed out | Correct IP |

---

## 📁 Repository Structure

```
📁 Network-Monitoring-and-Performance-Analysis
   📄 README.md
   📄 Network_Monitoring_Report.pdf
   📄 Network_Monitoring.pkt
   📁 screenshots
      🖼️ topology.png
      🖼️ ping_results.png
      🖼️ simulation_mode.png
      🖼️ traceroute.png
      🖼️ fault1.png
      🖼️ fault2.png
      🖼️ fault3.png
```

---

## 🚀 How to Open the Project

1. Download and install **Cisco Packet Tracer**
2. Clone this repository:
```bash
git clone https://github.com/Nishigandh/Network-Monitoring-and-Performance-Analysis.git
```
3. Open the `.pkt` file in Cisco Packet Tracer
4. Explore the network topology and configurations!

---

## 👤 Author

**Nishigandh**
📚 Course: Computer Networking

---

## 📄 License

This project is for educational purposes only.
