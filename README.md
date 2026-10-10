# Snort and Firewall Rules Lab

A GitHub-ready documentation workflow for the **Cisco Networking Academy: Lab - Snort and Firewall Rules** activity.

> **Important:** This repository is a documentation template, not proof that the lab has been completed. Add your own screenshots, observations, answers, and results as you perform the lab. Do not claim a step succeeded unless you observed and verified it.

## Lab objectives

The source lab is organized into three parts:

1. Prepare the virtual environment.
2. Inspect firewall and IDS logs, generate and capture simulated traffic, and add an `iptables` blocking rule.
3. Terminate and clear the Mininet process.

## Lab environment from the source document

- CyberOps Workstation virtual machine
- Oracle VirtualBox
- Internet connection
- Mininet topology and provided lab support scripts
- Snort IDS, `iptables`, `wget`, `tcpdump`, and `netstat`

Refer to the original course PDF for the exact topology and step-by-step instructions. This repository organizes evidence and notes; it does not replace the course instructions.

## Repository map

```text
snort-firewall-rules-github-workflow/
├── README.md
├── .gitignore
├── LICENSE
├── COMMANDS.md
├── EVIDENCE_CHECKLIST.md
├── docs/
│   ├── README.md
│   ├── lab-overview.md
│   ├── procedure-and-observations.md
│   └── questions-and-findings.md
├── screenshots/
│   └── README.md
├── evidence/
│   └── README.md
├── commands/
│   └── README.md
└── notes/
    └── README.md
```

## Suggested workflow

1. Read the source lab and `docs/lab-overview.md`.
2. Complete the lab in the assigned CyberOps Workstation environment.
3. Record only your actual results in `docs/procedure-and-observations.md`.
4. Answer the source lab questions in `docs/questions-and-findings.md`.
5. Save screenshots using the naming convention in `screenshots/README.md`.
6. Use `EVIDENCE_CHECKLIST.md` to check your documentation before publishing.
7. Review the repository for credentials, personal information, and unsafe or unnecessary files.
8. Commit and push using Git Bash (commands below).

## Git Bash: publish to your GitHub repository

Open Git Bash in the extracted folder:

```bash
cd /path/to/snort-firewall-rules-github-workflow
git init
git add .
git commit -m "Add Snort and firewall rules lab documentation workflow"
git branch -M main
git remote add origin https://github.com/YOUR-USERNAME/YOUR-REPOSITORY.git
git push -u origin main
```

Replace the example remote with your own repository URL. If the GitHub repository already contains commits or files, check its contents and follow the appropriate pull/merge workflow instead of blindly overwriting it.

For later updates:

```bash
git status
git add .
git commit -m "Document Snort and firewall lab results"
git push
```

## Safety and documentation notes

- Run this exercise only in the authorized course lab or an isolated environment you are permitted to use.
- The course scenario describes a simulated malicious web server and a file named `W32.Nimda.Amm.exe`. Do not download or execute real malware on your normal computer. Use only the instructor-provided isolated lab environment and follow your institution's safety procedures.
- PCAP files can contain sensitive network information. Review them before publishing; do not commit captures that expose credentials, personal data, or unrelated traffic.
- Do not commit passwords, tokens, private keys, or sensitive VM configuration.
- Use screenshots of your own terminal output and label them accurately.
