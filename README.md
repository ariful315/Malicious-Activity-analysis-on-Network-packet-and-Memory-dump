# Malicious Activity Analysis on Network Traffic & Volatile Memory Dump

## Introduction
This project involves a forensic analysis of network traffic and volatile memory dumps to identify malware and malicious activities. Using the Volatility framework, the investigation compares a clean memory dump with an infected sample from a Debian-based Linux system. The goal is to uncover system changes, suspicious processes, hidden modules, and malicious behaviors.

## Methodology
1. **Clean Memory Creation**: 
   - Generated using LiME (Linux Memory Extractor) on a Debian virtual machine.
   - Created a Volatility profile for accurate analysis.

2. **Analysis**:
   - Compared processes, modules, and network connections between clean and infected memory samples.
   - Identified irregularities, including suspicious processes (`xfce4-terminal`) and hidden modules (`lilyofthevalley`).

3. **Network Analysis**:
   - Categorized connections as localhost, local network, or public network.
   - Discovered multiple unauthorized public network connections indicating data exfiltration.

4. **Function Hooking**:
   - Analyzed hooked system calls and file operations to detect malware persistence mechanisms.

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
