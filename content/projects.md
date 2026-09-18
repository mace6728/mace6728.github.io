+++
draft = false
date = 2026-02-23T18:45:00+08:00
title = "Projects"
slug = "projects"
+++

Here's a collection of my technical projects spanning hardware acceleration, networking systems, and deep learning applications.

---

## Networking & Systems

### DPU-Accelerated Scitags Marking System

High-energy physics experiments like the Large Hadron Collider generate massive amounts of data that need to be transferred across global research networks. Traditional approaches using CPU-based software marking struggle to keep up with modern 400Gbps networks, creating a significant bottleneck.

I developed a hardware-accelerated solution using **NVIDIA BlueField-3 DPU** to offload packet marking entirely from the host CPU. By leveraging **DOCA Flow**, the system performs IPv6 Flow Label modifications directly in hardware at line rate.

**Key Results:**
- Achieved full **400Gbps line-rate processing** (compared to ~300Gbps with traditional eBPF)
- Reduced host CPU overhead to essentially zero
- Implemented dynamic flow rule management and real-time traffic visualization

**Tech Stack:** `C`, `DOCA`, `DPDK`, `eBPF/XDP`, `Prometheus`, `Grafana`
    

> **Open to collaborating on networking, systems performance, or ML infrastructure projects. Feel free to reach out!**