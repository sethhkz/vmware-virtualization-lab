# 💻 VMware Virtualization Lab — Multi-OS Testing Environment

A virtualization project focused on running multiple operating systems safely on a single physical machine, with hands-on configuration of virtual hardware, networking, and isolated test environments.

---

## 🎯 Project Goals

- Build a working virtual lab to run multiple OSes from one host machine
- Understand how virtual hardware (CPU, RAM, storage) is allocated
- Explore how virtual networking modes affect connectivity
- Create safe, isolated environments for technical experimentation
- Develop confidence with both Windows and Linux command-line workflows

---

## 🛠️ Tools & Technologies

| Tool | Purpose |
|------|---------|
| VMware Workstation | Hypervisor for creating and managing VMs |
| Windows host system | Physical machine running the hypervisor |
| Windows VM | Guest OS for testing Windows configuration |
| Kali Linux VM | Linux-based environment for technical practice |
| NAT networking | VM internet access via host |
| Bridged networking | VMs as standalone LAN devices |
| Command Prompt / Terminal | Connectivity testing and diagnostics |

---

## 📋 What I Did

### 1. VM Creation & Configuration
Built two virtual machines from scratch in VMware Workstation:
- **Windows VM** — 8 GB RAM, 4 vCPUs, 64 GB virtual NVMe disk
- **Kali Linux VM** — 8 GB RAM, 4 vCPUs, 40 GB virtual disk

Each VM was configured with its own isolated virtual hardware profile, allowing experimentation without touching the host system.

### 2. Resource Allocation
Hands-on practice with allocating CPU cores, RAM, and storage between VMs while keeping the host system stable. This involved understanding the trade-offs between guest performance and host resources — VMware's recommended memory range guided this directly.

### 3. Virtual Networking
Tested two networking modes:
- **NAT mode** — VMs share the host's network connection but are isolated behind a virtual NAT
- **Bridged mode** — VMs behave like real devices on the LAN with their own IPs

This gave me a clear understanding of how virtualised networks behave differently from physical ones, and when each mode is appropriate.

### 4. Connectivity Testing Inside VMs
Ran ping and IP configuration tests from inside each VM (`ping 1.1.1.1`, `ipconfig`) to verify:
- DNS resolution worked
- Internet access was functional
- Virtual network adapters were configured correctly

### 5. Cross-Platform Practice
- **Windows VM** — used for testing Windows-specific configurations and behaviour
- **Kali Linux VM** — used for command-line practice, terminal navigation, and Linux fundamentals

---

## 🧠 Key Skills Demonstrated

- VMware Workstation administration
- Virtual machine creation and configuration
- Virtual hardware resource allocation
- NAT vs bridged networking concepts
- Operating system installation and setup
- Cross-platform OS management (Windows + Linux)
- Virtual network troubleshooting
- Safe, isolated testing methodologies

---

## 💡 What I Took Away

Virtualization fundamentally changes how you can learn and experiment. Instead of being scared of breaking something, I could spin up a VM, try anything, break it, and start over. This project built genuine confidence with Linux command-line work and Windows configuration in a way that just reading guides never could.

The networking side was particularly valuable — actually seeing the difference between NAT and bridged behaviour made concepts click that had been abstract before.
