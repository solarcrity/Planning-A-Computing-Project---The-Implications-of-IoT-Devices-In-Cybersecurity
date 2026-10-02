# Planning a Computing Project — The Impact of Weak Authentication on IoT Device Security

A cybersecurity research and project-planning assignment for the **Pearson HND in Computing: Planning a Computing
Project** unit at GUSTO College, May–June 2026.

I investigated why IoT devices stay vulnerable through weak authentication: default passwords, password reuse and
patchy MFA. I combined a **primary survey of 46 users in Myanmar** with **secondary research on peer-reviewed
studies**, then planned the full research project with a WBS, Gantt chart, project charter and budget, and
presented recommendations.

📄 **[Full report (PDF)](report/IoT-Weak-Authentication-Project-Report.pdf)** ·
📋 **[Project charter (PDF)](planning/Project-Charter.pdf)** ·
📅 **[Gantt chart (PDF)](planning/Gantt-Chart.pdf)** ·
🎤 **[Presentation (PPTX)](presentation/IoT-Weak-Authentication-Presentation.pptx)**

---

## What I did

- **Primary research:** designed a mixed-methods survey (quantitative and open-ended questions), got it approved, ran it for 6 days and analysed **46 responses**
- **Secondary research:** reviewed academic work on IoT authentication techniques and an empirical security study of 52 IoT management platforms
- **Analysis:** combined both sources, identified key challenges, and evaluated the reliability and limitations of my own research
- **Project planning:** built a 5-phase **Work Breakdown Structure**, a 12-week **Gantt chart**, and a **project charter** with scope, milestones, stakeholders, constraints, risks and a costed budget
- **Recommendations:** presented technical and non-technical recommendations, assessed against the client organisation's needs

## Key findings from the survey

| Area | Finding |
|---|---|
| IoT adoption | **95.7%** use smart/IoT devices; 58.7% have more than 5 devices on their main network |
| Most-used devices | Routers, wearables, smart cameras, smart speakers |
| Password policy awareness | **93.5%** say they understand strong-password policy |
| Default passwords | 63.0% always change them; 28.3% sometimes; 8.7% rarely or never |
| Password reuse | **43.5%** reuse credentials most of the time, 32.6% sometimes; only 23.9% always use unique ones |
| MFA / 2FA | 80.4% are aware of MFA/2FA and use it |
| Threat perception | 58.7% are very concerned about unauthorised access; 73.9% know IoT devices can be recruited into botnets |
| Suspicious activity | **58.7%** have seen suspicious activity on their IoT devices |
| Local infrastructure | **63.0%** say power and internet outages make it hard to keep devices secure |

**The awareness–action gap.** Users know the rules, but convenience, "password fatigue" and complicated setup
lead to heavy credential reuse.

**Myanmar-specific risks.** Respondents reported:
- firmware updates interrupted by power cuts, which "bricked" routers or reset them to insecure factory defaults
- patches skipped because mobile data is too expensive for large firmware downloads
- cheap, unbranded or outdated devices bought because of budget limits

## Recommendations

| Technical | Non-technical |
|---|---|
| **Passkeys / phone-linked biometrics** in place of password-only login, to reduce reuse and credential stuffing | **Community training** to close local skills gaps |
| **Offline-first updates** over USB or local LAN to avoid bricking during outages | **Security blueprints**: step-by-step playbooks for isolating IoT devices on a separate Wi-Fi network |
| **Dual firmware banks** so a failed over-the-air update can roll back | **Post-outage audits**: teach users to re-check settings after a power failure |

## Project plan

![Work Breakdown Structure](planning/Work-Breakdown-Structure.png)

- **5 phases:** Preparation → Planning → Development → Testing → Release
- **12-week Gantt chart** ([PDF](planning/Gantt-Chart.pdf) / [Excel](planning/Gantt-Chart.xlsx)) with task owners, durations and dependencies; this charter covers phases 1–2
- **Budget:** £372 one-off (IoT testbed with Raspberry Pi 4s, routers and smart devices; open-source scanners such as OpenVAS, Nmap and OWASP ZAP) plus £59/month (AWS sandbox and hosted vulnerability scanning)
- **Risks identified:** small survey sample, fast-changing threats, limited access to live systems for testing, scope creep, and stakeholder or budget constraints

### Timeline (2026)

| Date | Milestone |
|---|---|
| 8 May | Research topic chosen; secondary sources gathered |
| 21 May | Survey questions approved |
| 22–27 May | Survey live: 46 responses |
| 29 May | Survey data analysed |
| 11–12 June | WBS and Gantt chart |
| 18 June | Project charter |
| 19–23 June | Final report and presentation |

## Skills demonstrated

`IoT security` · `Authentication & MFA` · `Threat awareness` · `Survey design & data analysis` ·
`Literature review` · `Work Breakdown Structure` · `Gantt charts` · `Project charter & budgeting` ·
`Risk assessment` · `Stakeholder analysis` · `Presenting recommendations`

## Repository contents

```
.
├── README.md
├── report/
│   └── IoT-Weak-Authentication-Project-Report.pdf   # Final report
├── planning/
│   ├── Project-Charter.pdf
│   ├── Gantt-Chart.pdf
│   ├── Gantt-Chart.xlsx
│   └── Work-Breakdown-Structure.png
├── research/
│   └── Survey-Data-Analysis.docx                    # Analysis of the 46 survey responses
└── presentation/
    └── IoT-Weak-Authentication-Presentation.pptx
```

Raw survey responses are not published, to protect respondents' privacy.

## References

- Alotaibi, A., Aldawghan, H. and Aljughaiman, A. (2025). *A Review of the Authentication Techniques for Internet of Things Devices in Smart Cities: Opportunities, Challenges, and Future Directions.* Sensors, 25(6), 1649. https://doi.org/10.3390/s25061649
- Tejaswi, B., Mannan, M. and Youssef, A. (2023). *Security Weaknesses in IoT Management Platforms.* IEEE Internet of Things Journal.
- NIST. *SP 800-213 series: IoT device cybersecurity guidance for the federal government.* https://www.nist.gov/itl/applied-cybersecurity/nist-cybersecurity-iot-program/sp-800-213-series

---

**Author:** Thet Htoo Zin · HND in Computing, GUSTO College · June 2026

*Other networking projects:* [BlueWave network & subnetting design](https://github.com/solarcrity/bluewave-network-subnetting-design) ·
[Summit Ridge secure LAN (Packet Tracer)](https://github.com/solarcrity/Summit-Ridge-Institute-Simulation)
