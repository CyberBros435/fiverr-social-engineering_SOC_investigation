# Fiverr Social Engineering: SOC Investigation

I treated a suspicious Fiverr "order" like a SOC alert: collected evidence, analysed the file, extracted IOCs, mapped to MITRE ATT&CK, and reported it.

## Cases

| Case | Scam type | Report | PDF |
|---|---|---|---|
| 01 | Fake order + HTML file + card-harvesting page | [report/report.md](fiverr-social-engineering_SOC_investigation/fiverr-social-engineering_SOC_investigation/report/report.md) | [report.pdf](fiverr-social-engineering_SOC_investigation/fiverr-social-engineering_SOC_investigation/report.pdf) |

## Case 01 in one line
A new account sent an HTML "project". It showed a fake Fiverr page, redirected to a fake payment site and asked for bank card details. Two scanners showed 0 detections, so the proof is in the source code and behaviour.

## Folder structure
```
fiverr-social-engineering_SOC_investigation/
├── README.md
├── report.pdf                  # same report, easy to read, with screenshots
└── report/
    ├── report.md               # full report with screenshots in place
    └── screenshots/            # 16 evidence images
```

## Safety note
All IOCs are defanged (`hxxp`, `[.]`). Do not visit them. The malicious file itself is not included in this repository.
