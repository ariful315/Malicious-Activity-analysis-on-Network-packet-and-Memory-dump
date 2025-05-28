

## Key Findings
- **Processes**: Suspicious `xfce4-terminal` process found in the infected memory sample.
- **Hidden Modules**: The `lilyofthevalley` rootkit was identified, indicating sophisticated malware activity.
- **Network Connections**: Unauthorized connections to public IPs via `wget` revealed potential data leaks.
- **Function Hooking**: Hooked system calls and file operations were detected, showing malware evasion techniques.

## Tools Used
- **Volatility Framework**: For memory analysis.
- **LiME (Linux Memory Extractor)**: For memory dumping.
- **Kali Linux**: Analysis platform.
- **Debian Virtual Machine**: Clean baseline creation.

## Conclusion
This project demonstrates the importance of memory forensics in identifying and mitigating cyber threats. The structured approach, from creating a clean memory baseline to analyzing infected samples, provides valuable insights into malware behavior and system compromises.

## References
- Volatility Framework Documentation: [Volatility Labs](https://volatility-labs.blogspot.com/2017/04/volatility-26.html)
- LiME: Linux Memory Extractor Tool
- National Institute of Standards and Technology (NIST) Special Publication 800-86: [Guide to Forensic Techniques](https://nvlpubs.nist.gov/nistpubs/Legacy/SP/nistspecialpublication800-86.pdf)
