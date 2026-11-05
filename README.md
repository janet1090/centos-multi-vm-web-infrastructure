# CentOS Multi VM Web Infrastructure Lab

A documented CentOS systems lab built in Oracle VirtualBox. I configured a virtual load-balancer host and three web-server virtual machines, then documented the networking, web-server setup, load-balancing configuration, and service checks.

## Architecture

```text
Browser
  |
  v
CentOS_HA — NGINX front end
  |
  +--> CentOS_WS1 — Apache
  +--> CentOS_WS2 — Apache
  +--> CentOS_WS3 — Apache
```

## Work documented

- Created and configured the virtual machines in VirtualBox, including bridged networking.
- Checked interface addresses, assigned hostnames, edited `/etc/hosts`, and tested VM connectivity.
- Set up Apache on the web-server VMs, configured firewall access, and created distinct test pages.
- Prepared NGINX on the front-end VM, adjusted firewall and SELinux settings, and backed up the configuration before editing it.
- Documented least-connections and round-robin load-balancing configurations, including a test with one backend unavailable.
- Checked service status and logs and viewed the web-server responses in a browser.

## Evidence

See [the portfolio case study](./CentOS_Multi_VM_Web_Infrastructure_Portfolio.docx) for the VM inventory and selected browser screenshots, plus a summary of the configuration workflow and skills demonstrated.

## Reproducibility

This repository contains portfolio documentation only. The original VM disks and configuration files are not available after a computer change, so the lab cannot be recreated from this repository as-is. The screenshots and written lab record document the work completed; they are not presented as source code or automated deployment scripts.
