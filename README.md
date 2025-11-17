Here is a clean, professional **README.md** you can directly upload to GitHub for your GNS3 topology project.
I tailored it based on your screenshots, ping tests, and VPCS configuration steps.

---

# 🖧 GNS3 LAN Topology Project

This project contains a simple **Local Area Network (LAN)** simulation built using **GNS3**.
It demonstrates how multiple PCs connected through a switch can communicate with each other using basic **IP addressing** and **ICMP (ping)** verification.

---

## 📌 **Project Overview**

The topology includes:

* **4 VPCS hosts**

  * PC1 – `10.1.1.1`
  * PC2 – `10.1.1.2`
  * PC3 – `10.1.1.3`
  * PC4 – `10.1.1.4`
* **1 unmanaged switch (Ethernet switch)**
  Used to interconnect all PCs in a single broadcast domain.

This setup is ideal for:

* Testing basic connectivity
* Understanding how switches forward frames
* Observing ping/ICMP behavior
* Practicing GNS3 topologies

---

## 🧩 **Topology Diagram**

Screenshots of the topology are included in the repository:

* `Screenshot 1` – 2-PC test
* `Screenshot 2` – 4-PC topology
* `Screenshot 3` – Console outputs
* `Screenshot 4` – Ping test results
* `Screenshot 5` – Multi-switch test (optional)

---

## ⚙️ **IP Configuration**

Each PC uses VPCS with manual IP assignment:

### **Example (PC1):**

```
ip 10.1.1.1 255.255.255.0
```

### **All PCs:**

| PC  | IP Address | Subnet Mask   |
| --- | ---------- | ------------- |
| PC1 | 10.1.1.1   | 255.255.255.0 |
| PC2 | 10.1.1.2   | 255.255.255.0 |
| PC3 | 10.1.1.3   | 255.255.255.0 |
| PC4 | 10.1.1.4   | 255.255.255.0 |

No gateway is required since all devices are on the **same network**.

---

## 🖥️ **Ping Test Results**

Connectivity was tested using `ping` between all PCs.

### ✔️ Successful Pings

* PC1 ↔ PC2
* PC1 ↔ PC4
* PC3 ↔ PC1
* PC3 ↔ PC4
* PC2 ↔ PC4

These tests confirm that the switch is forwarding frames correctly.

### ⚠️ Observed Timeouts

During experiments with additional switches, some links showed:

* ICMP timeout
* Partial packet loss

This helps visualize how switching loops or mis-cabling can affect connectivity.

---

## 📁 Files Included

| File                     | Description                         |
| ------------------------ | ----------------------------------- |
| `topology-1.gns3project` | Basic 2-PC topology                 |
| `topology-2.gns3project` | 4-PC + 1 Switch topology            |
| `topology-3.gns3project` | Multi-switch testing topology       |
| `/screenshots/`          | Images of the topology & ping tests |

---

## ▶️ How to Use

1. Install **GNS3** and **GNS3 VM**
2. Import `.gns3project` files into GNS3
3. Start all nodes
4. Open each PC console
5. Assign IP addresses
6. Test connectivity using `ping`

---

## 📘 **Commands Used**

### Assign IP:

```
ip <address> <subnet>
```

### Ping:

```
ping <destination-ip>
```

---

## 🎯 Learning Outcomes

Through this project, you will understand:

* Basic LAN design
* Switch behavior (Layer 2 forwarding)
* IP addressing within a subnet
* Connectivity troubleshooting
* GNS3 project workflow

---

## 📬 Contact / Support

If you have questions, contributions, or improvements, feel free to open an issue or pull request on the repository.

---

If you want, I can also generate:

✅ A professional **GitHub description**
✅ A **short version of README**
✅ A **nice banner / badge section**
✅ Auto-formatted markdown with emojis

Just tell me!
