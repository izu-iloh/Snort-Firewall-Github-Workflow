# Command Reference

Commands below are drawn from the source lab. Run them only at the indicated prompt and in the provided authorized lab environment. Paths may depend on the course VM setup.

## CyberOps Workstation terminal

```bash
sudo ./lab.support.files/scripts/configure_as_dhcp.sh
ifconfig
ping www.cisco.com
sudo ./lab.support.files/scripts/cyberops_extended_topo_no_fw.py
```

Stop the ping with `Ctrl+C`. At the Mininet prompt, open terminals as directed by the course instructions:

```text
mininet> xterm R1
mininet> xterm H5
mininet> xterm H10
```

## R1 / IDS monitoring

```bash
./lab.support.files/scripts/start_snort.sh
tail -f /var/log/snort/alert
iptables -L -v
```

The Snort process and the `tail -f` monitor are intended to run in separate R1 terminals, as described in the source lab.

## H10 / simulated web server

```bash
./lab.support.files/scripts/mal_server_start.sh
netstat -tunpa
```

The course example shows a listener on TCP port `6666`. Confirm your own output.

## H5 / traffic generation and capture

The source lab uses the following course-lab request:

```bash
wget 209.165.202.133:6666/W32.Nimda.Amm.exe
```

It also demonstrates a packet capture on H5's `H5-eth0` interface:

```bash
tcpdump -i H5-eth0 -w nimda.download.pcap &
```

After reproducing the request in the isolated lab, bring the background capture to the foreground and stop it with `Ctrl+C`:

```bash
fg
ls -l nimda.download.pcap
```

Do not open or execute the downloaded file. Avoid moving the sample or PCAP to your everyday host. Follow instructor safety rules.

## R1 / firewall rule

The course lab inserts a rule into the `FORWARD` chain to drop TCP traffic destined for the server IP and port:

```bash
iptables -I FORWARD -p tcp -d 209.165.202.133 --dport 6666 -j DROP
iptables -L -v
```

Then the source lab asks you to retry the request from H5 and record the observed result. Do not assume it timed out; document your own result.

## Cleanup

At the Mininet prompt:

```text
quit
```

Then, in the CyberOps Workstation terminal, the source lab uses:

```bash
sudo mn -c
```

## Command safety

These commands can change firewall behavior or start background processes. Use them only in the course's isolated, authorized topology. Confirm the target host and interface before running capture or firewall commands.
