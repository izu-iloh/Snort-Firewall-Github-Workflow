# Evidence Checklist

Mark an item complete only after capturing or recording your own result.

## Environment preparation
- [ ] VirtualBox network adapter setting documented (bridged, or NAT if required by the lab setup).
- [ ] DHCP configuration command result recorded.
- [ ] Network interface and assigned IP address shown.
- [ ] Connectivity test result recorded.

## Snort and simulated traffic
- [ ] Mininet startup and ready prompt captured.
- [ ] R1 shell identity and indicator recorded.
- [ ] Snort startup captured or summarized.
- [ ] H10 server listener verified; port recorded from actual output.
- [ ] Snort alert monitor shown.
- [ ] H5 request result documented, including whether the transfer completed.
- [ ] Snort alert captured with timestamp, signature message, source/destination IPs, and ports.
- [ ] PCAP creation verified by file listing and non-zero size.
- [ ] Brief note explains how a PCAP can support analyst investigation.

## Firewall tuning
- [ ] Initial `iptables -L -v` output captured; active chains and policies recorded.
- [ ] Rule insertion command recorded.
- [ ] Updated FORWARD-chain rule shown.
- [ ] Retry result recorded and explained based on observed output.
- [ ] Response to the source lab's final blocking question documented.

## Cleanup and GitHub review
- [ ] Mininet quit and cleanup command recorded.
- [ ] Screenshots have clear names and captions.
- [ ] No passwords, tokens, personal data, or unsafe captures are included.
- [ ] README and findings contain no unverified claims.
- [ ] `git status` reviewed before commit.
