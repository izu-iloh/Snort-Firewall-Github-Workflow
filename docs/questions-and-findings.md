# Lab Questions and Findings

Answer using your own terminal output and screenshots. Do not copy example timestamps or packet counts from the course PDF as if they were your own.

## Part 2, Step 1 — Real-Time IDS Log Monitoring

1. **R1 shell identity:** What user is logged into the R1 shell? What indicates this?
   - Answer:
   - Evidence:

2. **Server port:** What port is used to communicate with the simulated malware web server? What indicates it?
   - Answer:
   - Evidence:

3. **Download status:** Was the file completely downloaded?
   - Answer:
   - Evidence:

4. **IDS alert:** Did the IDS generate an alert related to the file download?
   - Answer:
   - Evidence:

5. **Addresses:** What source and destination IPv4 addresses appear in the alert?
   - Source:
   - Destination:
   - Evidence:

6. **Ports:** What source and destination ports appear in the alert?
   - Source port:
   - Destination port:
   - Evidence:

7. **Time:** Based on your alert, when did the request/download take place?
   - Answer:
   - Evidence:

8. **Signature message:** What message did the IDS signature record?
   - Answer:
   - Evidence:

9. **PCAP usefulness:** How can the PCAP file be useful to a security analyst?
   - Answer:

## Part 2, Step 2 — Tuning Firewall Rules Based on IDS Alerts

10. **Initial chains:** What chains are currently in use by R1?
    - Answer:
    - Evidence:

11. **Retry after rule insertion:** Was the download successful after the blocking rule was added? Explain using your observed output.
    - Answer:
    - Evidence:

12. **Alternative blocking approach:** What would be a more aggressive but also valid approach when blocking the offending server?
    - Answer:
    - Reasoning:

## Summary of findings

- Main observation:
- What the Snort alert revealed:
- What changed after the firewall rule:
- What evidence supports the conclusion:
- Limitations or unexpected results:
