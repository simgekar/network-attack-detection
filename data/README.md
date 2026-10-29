# Data

The raw captures and generated datasets are **not committed** to this repository. The captures contain IP and MAC addresses from the lab network, and some files are large (up to ~45 MB).

Expected layout if you reproduce the pipeline with your own captures:

```
pcap_verileri/
├── normal/
│   ├── normal_trafik.pcapng
│   ├── normal_trafik2.pcapng
│   ├── normal_trafik3.pcapng
│   └── normal_trafik4.pcapng
└── zararli/
    ├── arp_saldiri_trafigi.pcapng
    ├── arp_ve_dns_saldirisi.pcapng
    ├── dhcp_poisoning_trafigi.pcapng
    └── nmap_tarama.pcapng
```

Generated files:

| File | Created by | Content |
|---|---|---|
| `normal_dataset.csv` / `.txt` | notebook 01 | 117 normal 5-second windows |
| `zararli_dataset.csv` / `.txt` | notebook 01 | 872 malicious 5-second windows |
| `dataset.json` | notebook 03 | 167 windows with packet-level text logs, used for the LLM experiments |
