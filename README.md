# Advanced Computer Forensics: Reverse Engineering Tool Comparison

## Overview
The goal of this project was to evaluate and compare four reverse engineering tools — IDA Free, Ghidra, Binary Ninja Free, and DnSpy with Radare2 — applied to LokiBot, a real-world credential-stealing infostealer. LokiBot's multi-layer obfuscation and packing made it an ideal test case for comparing how each tool handles a challenging binary. Each team member worked with an assigned tool, following established forensics procedures within isolated virtual machine environments, and results were synthesized into a comparative evaluation of each tool's strengths and limitations.

---

## My Role
- Performed static analysis on LokiBot using IDA Free, including triage of the packed binary and post-unpacking deep analysis
- Used x32dbg to dynamically unpack LokiBot by pausing execution at the Original Entry Point and dumping the payload to disk
- Leveraged IDA's Strings, Imports, Cross References, and Graph View windows to identify malicious behavior indicators
- Identified runtime artifacts in the packed binary including networking libraries, cryptographic operations, and credential decryption functions
- Confirmed browser credential theft post-unpacking, including SQLite queries against login stores, Firefox NSS library references, and Windows Credential Manager targeting
- Documented LokiBot's exfiltration pipeline: credentials compressed with aPLib, encrypted with Triple-DES, and sent via HTTP POST to a C2 server
- Contributed findings to the group's comparative analysis and final report

---

## Skills Learned
- Performing static and dynamic analysis on packed malware executables using IDA Free and x32dbg
- Identifying obfuscation techniques, runtime unpacking behavior, and credential theft mechanisms in real-world infostealer samples
- Evaluating the capabilities and limitations of professional reverse engineering tools in a forensic investigation context

---

 > **Note:** The full group report and final presentation can be found in this repository.
