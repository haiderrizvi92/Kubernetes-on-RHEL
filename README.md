This Git repository contains supporting files for the "Certified Kubernetes Administrator (CKA)" video course. See https://sandervanvugt.com for more details. It is also used in the "CKA Crash Course" available at https://learning.oreilly.com.

## Lab Environment Requirements (RHEL Version)

In this course, you need to build your own lab environment. The lab environment should consist of **3 virtual machines**, running **Red Hat Enterprise Linux (RHEL) 9.5 or later**.

Ensure that each virtual machine meets the following requirements:

- 2 GB RAM
- 2 vCPUs
- 20 GB disk space
- Swap disabled

> Note: Kubernetes requires swap to be disabled for proper operation.

---

## RHEL Installation

Install **RHEL 9.5 Minimal** on all nodes. Ensure:

- Network connectivity between nodes
- Hostnames are properly configured
- Time synchronization is enabled

---

## Kubernetes Setup (RHEL)

To configure Kubernetes on RHEL nodes, use the scripts provided in the `rhel/` directory:

### 1. Install Container Runtime

```bash
./rhel/install-containerd.sh

