# Lab Overview: Snort and Firewall Rules

## Purpose

The course lab introduces firewall rules and IDS signatures. It demonstrates monitoring Snort alerts, examining traffic associated with a simulated server, capturing packets, and adding an `iptables` rule to block traffic through the firewall.

## Objectives from the source lab

1. Preparing the virtual environment.
2. Firewall and IDS logs.
3. Terminate and clear the Mininet process.

## Required resources listed in the source

- CyberOps Workstation virtual machine.
- Internet connection.

The source also describes Oracle VirtualBox, a Mininet topology, Snort, `iptables`, and provided lab support scripts.

## Concepts to observe

- Firewall and IDS rules have matching components and action components.
- Firewalls commonly inspect packet headers; IDS rules may inspect payload content.
- `iptables` uses INPUT, FORWARD, and OUTPUT chains.
- Snort writes alert events to the configured alert log.
- `tcpdump` can capture packets to a PCAP file for later analysis.
- A firewall rule can drop traffic matching a specified protocol, destination, and destination port.

## Lab metadata

- Learner: [Add your name if you want it public]
- Date performed: [YYYY-MM-DD]
- Course/module: [Fill in]
- Environment/VM version: [Fill in]
- Result: [In progress / Completed / Partially completed]
