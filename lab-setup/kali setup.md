# Kali setup
# Network Configuration

The Kali Linux virtual machine operates within the isolated SOC homelab subnet:

```text
192.168.56.103
```

The environment includes:

* Kali Linux attacker workstation
* DVWA vulnerable web server
* Wazuh SIEM platform
* Windows 10 monitored endpoint

All systems are configured on the same internal VirtualBox network to allow:

* internal host communication
* attack simulation
* telemetry generation
* SIEM monitoring
* log correlation



---

# Internet Connectivity

The virtual machine retains outbound internet access through a secondary VirtualBox NAT adapter.

This enables:

* package installation
* system updates
* tool downloads
* repository cloning
* vulnerability database updates

while still maintaining an isolated internal lab environment for attack simulation activities.

---

# Connectivity Verification

Internal communication validated using:

```bash
ping 192.168.56.102 (Ubuntu Dvwa)
```


