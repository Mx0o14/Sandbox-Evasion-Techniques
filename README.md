# Sandbox Evasion Techniques – TryHackMe Room Implementation

This repository contains the full code implementation of sandbox evasion techniques discussed in my [Medium article](https://medium.com/@Mx0o14/tryhackme-sandbox-evasion-0a5150be7f1e), based on the [TryHackMe: Sandbox Evasion](https://tryhackme.com/room/sandboxevasion) room.

---

## Summary

Malware often uses sandbox evasion techniques to detect whether it's being analyzed in a controlled or virtualized environment before executing its actual payload.

This project showcases multiple evasion strategies implemented in C++, including:

- Analysis tool detection  
- Geo-filtering  
- Memory checks  
- Sleep timing tricks  
- Combined evasion dropper  

---

## Included Files

| File Name            | Description                                                         |
|----------------------|---------------------------------------------------------------------|
| `dropper.cpp`        | Simulates basic dropper behavior                                    |
| `ad-check.cpp`       | Detects analysis tools (Wireshark, ProcMon, etc.)                   |
| `geofiltering.cpp`   | Restricts execution based on IP geolocation                         |
| `memory-check.cpp`   | Checks for unrealistic memory values common in sandbox VMs          |
| `sleep-check.cpp`    | Detects sleep-skipping used by dynamic analysis environments        |
| `Final Dropper.cpp`  | Combines all evasion techniques into a single executable            |
| `SandboxChecker.exe` | Sample sandbox environment used for testing evasion techniques      |

---

## Getting Started

To compile the source files on Windows (using g++):

`g++ dropper.cpp -o dropper.exe`
`g++ "Final Dropper.cpp" -o FinalDropper.exe`

> **Note:** Test responsibly in isolated environments (e.g., VMs or labs).  
> Use the appropriate flags if you’re working with specific Windows APIs.

---

##  Disclaimer

This repository is for **educational and ethical research purposes only**.  
Do **not** use any part of this code on systems you do not own or have explicit permission to test.

---

## Author

**Mohamed Ashraf (Mx0o14)**  
Red Team Operator | Malware Developer | Cybersecurity Enthusiast

- Medium: [https://medium.com/@Mx0o14](https://medium.com/@Mx0o14)  
- LinkedIn: [https://linkedin.com/in/mx0o14](https://linkedin.com/in/mx0o14)

---

## ⭐️ Show Your Support

If you found this project helpful, feel free to ⭐️ the repo and share the [Medium article](https://medium.com/@Mx0o14/tryhackme-sandbox-evasion-0a5150be7f1e).  
Ideas, feedback, and contributions are always welcome!

