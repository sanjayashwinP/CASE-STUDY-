# CASE-STUDY-

Case Study Title: Resource Allocation and Cost Optimization in an OpenStack Private Cloud

Case Overview:

ABC Cloud Services runs a private cloud using OpenStack to host virtual machines (VMs) for internal development, testing, and production workloads. Their cloud infrastructure comprises:

5 Compute Nodes, each with:
64 vCPUs
256 GB RAM
2 TB SSD storage
OpenStack Services Deployed:
Nova (Compute)
Neutron (Networking)
Cinder (Block Storage)
Glance (Image Management)
Keystone (Identity)
Horizon (Dashboard)
Heat (Orchestration)

They are considering expanding their cloud but want to first evaluate current capacity usage, VM density, and cost efficiency. The goal is to calculate whether their resource usage aligns with business needs and how to optimize it.

Case Study Questions – OpenStack Calculation in Cloud Computing

1. Resource Utilization:

Based on the current infrastructure, what is the total available compute capacity in terms of:
Total vCPUs
Total RAM
Total storage

2.Storage Allocation:

Given 10 TB of total block storage across the cloud, how many VMs can be supported if:
a) Each VM is allocated 100 GB block storage
b) Snapshot storage consumes 20% extra on average

**SOLUTIONS:**
### Problem 1: Encryption Time Calculation
AES 256 encryption is used to secure data before uploading it to the cloud. The encryption speed is 0.05 seconds per MB. To convert 2 TB into MB, we use binary units: 2 TB = 2 × 1024 × 1024 MB
= 2,097,152 MB. Multiplying the total size by the encryption time per MB: 2,097,152 × 0.05 = 104,857.6 seconds. This equals approximately 29 hours, 7 minutes, and 38 seconds. This shows that large scale data encryption can add significant preprocessing time in cloud environments.

### Problem 2: CPU Utilization Efficiency
The VM is allocated 8 vCPUs but on average uses only 5.5 vCPUs. CPU utilization efficiency indicates how effectively the allocated compute resources are used. Efficiency = (Used / Allocated)
× 100 = (5.5 / 8) × 100 = 68.75%. This means the VM underutilizes around 31% of its assigned computing capacity, which may suggest over provisioning.

### Problem 3: Network Throughput Efficiency
The maximum available network bandwidth is 1 Gbps, but only 600 Mbps is utilized during peak activity. Throughput efficiency measures how much of the available network capacity is actually being used. Efficiency = (600 / 1000) × 100 = 60%. This indicates the network has unused capacity and may support additional workloads without congestion.

### Problem 4: Energy Efficiency
To process the same workload, Setup A consumes 500W for 2 hours, whereas Setup B uses 300W for 3.5 hours. Energy = Power × Time. Setup A: 500W × 2h = 1.00 kWh. Setup B: 300W × 3.5h =
1.05 kWh. Since Setup A consumes less energy for the same work, it is more energy efficient. Energy efficiency is critical in cloud infrastructures to reduce operational costs and environmental impact.

### Problem 5: Maximum Efficient VM Hosting
The physical server contains 16 CPU cores. Each VM requires 2 cores. However, for optimal performance and to avoid CPU contention, the system must operate at 75% utilization. Usable cores = 16 × 0.75 = 12 cores. Maximum efficiently hosted VMs = 12 / 2 = 6 VMs. This ensures balanced resource sharing without overloading the server, maintaining stability and performance in multi VM environments.
