# Procedure and Observations

> Fill this in while performing the course lab. These are prompts, not claims that the steps have already been completed.

## Part 1 — Preparing the Virtual Environment

### VirtualBox networking
- Adapter mode selected:
- Reason for selection:
- Evidence screenshot: `screenshots/01-virtualbox-network.png`

### DHCP configuration and connectivity
- Command used:
- Interface/IP observed:
- Connectivity test and result:
- Any error and troubleshooting:
- Evidence screenshot: `screenshots/02-network-check.png`

## Part 2 — Firewall and IDS Logs

### Start Mininet and open R1
- Mininet startup result:
- Was the `mininet>` prompt displayed?
- User shown in R1 shell and indicator:
- Evidence screenshot: `screenshots/03-mininet-r1.png`

### Start Snort
- Startup result:
- Any errors:
- Evidence screenshot: `screenshots/04-snort-start.png`

### Start the simulated server on H10
- Server startup result:
- Listener shown by `netstat -tunpa`:
- Evidence screenshot: `screenshots/05-h10-listener.png`

### Monitor alerts and request the file from H5
- Alert-monitor command:
- Request command/result:
- Was the transfer complete? What output supports your answer?
- Evidence screenshot: `screenshots/06-h5-request.png`

### Snort alert details
- Timestamp:
- Signature ID/revision:
- Alert message:
- Source IPv4 address and port:
- Destination IPv4 address and port:
- Evidence screenshot: `screenshots/07-snort-alert.png`

### Capture traffic with tcpdump
- Interface captured:
- Capture filename:
- Packets captured / dropped, as reported:
- File size:
- Evidence screenshot: `screenshots/08-pcap-created.png`
- PCAP stored locally for analysis? [Do not commit it unless reviewed and intentionally approved.]

### Add the firewall rule
- Initial chains/policies observed:
- Rule inserted:
- Updated FORWARD-chain output:
- Retry result from H5:
- Evidence screenshot: `screenshots/09-firewall-rule.png`
- Evidence screenshot: `screenshots/10-blocked-request.png`

## Part 3 — Terminate and Clear Mininet Process
- How Mininet was stopped:
- Cleanup command/result:
- Evidence screenshot: `screenshots/11-cleanup.png`

## Troubleshooting log

| Time/date | Step | Symptom/error | Action taken | Outcome |
|---|---|---|---|---|
| | | | | |

## Final reflection
- What did you learn about the relationship between IDS alerts and firewall rules?
- What evidence was most useful?
- What would you investigate further?
