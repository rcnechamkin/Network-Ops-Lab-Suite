# NetworkOps Lab Suite

A portfolio of hands-on labs showcasing enterprise-grade networking skills in automation, auditing, and routing. Built using Cisco IOSv on EVE-NG and open-source tooling to reflect real-world NOC/MSP environments.

---

## 🔧 Lab 1: Network Automation with Ansible

Automate switch and router configurations using Ansible. This lab demonstrates how to:

- Push VLAN, interface, and routing configs using playbooks
- Backup and verify configurations
- Use Jinja2 templates for repeatable deployments

**Tools:** Ansible, Cisco IOSv, EVE-NG  
**Folder:** `/1-automation-lab`

**Folder Structure:**
```
1-automation-lab/
├── README.md
├── playbooks/
│   └── base_config.yml
├── templates/
│   └── base_config.j2
├── inventory/
│   └── hosts.ini
```

---

## 🧾 Lab 2: NetBox + Python Inventory Audit

Compare live router configurations against NetBox documentation using Python scripts. This simulates a real-world source-of-truth audit system.

- Pull device inventory via API from NetBox
- SSH into Cisco devices (via Netmiko)
- Compare config state and log mismatches

**Tools:** NetBox, Python (Netmiko, Requests), Docker  
**Folder:** `/2-netbox-audit-tool`

**Folder Structure:**
```
2-netbox-audit-tool/
├── README.md
├── scripts/
│   ├── netbox_pull.py
│   ├── config_compare.py
│   └── audit_report.json
```

---

## 🌐 Lab 3: Multi-Site BGP Redundancy & Failover

Simulates a multi-site WAN with redundant ISP links. Includes:

- eBGP + iBGP peering
- AS path manipulation, local preference, route-maps
- Interface shutdowns to simulate failover
- Wireshark captures and convergence time tests

**Tools:** Cisco IOSv, EVE-NG, Wireshark, Python  
**Folder:** `/3-bgp-failover-lab`

**Folder Structure:**
```
3-bgp-failover-lab/
├── README.md
├── router-configs/
│   ├── site-a-r1.cfg
│   ├── site-b-r1.cfg
│   └── isp-core.cfg
├── failover-tests/
│   └── convergence_log.txt
├── captures/
│   └── bgp_failover.pcap
```

---

## 📂 Repo Structure
```
networkops-lab-suite/
├── README.md
├── diagrams/
│   └── full-suite-topology.png
├── 1-automation-lab/
│   ├── playbooks/
│   ├── templates/
│   ├── inventory/
│   └── README.md
├── 2-netbox-audit-tool/
│   ├── scripts/
│   └── README.md
├── 3-bgp-failover-lab/
│   ├── router-configs/
│   ├── failover-tests/
│   ├── captures/
│   └── README.md
└── docs/
    └── resume_snippet.md
```

---

## 📝 About This Project

This project was built to demonstrate core competencies in networking, troubleshooting, and infrastructure automation while transitioning from helpdesk roles to full-time network engineering.

To learn more about my background, visit:  
🔗 [https://github.com/rcnechamkin](https://github.com/rcnechamkin)  
📧 cnechamkin@gmail.com
