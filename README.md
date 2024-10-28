# 🌐 CyberPanel v2.3.6 Pre-Auth RCE Exploit Tool

CyberPanel v2.3.6 Pre-Auth RCE Exploit leverages a critical Remote Code Execution vulnerability in CyberPanel version 2.3.6. Thanks to [DreyAnd’s exceptional work](https://dreyand.rs/code/review/2024/10/27/what-are-my-options-cyberpanel-v236-pre-auth-rce), this vulnerability is well-documented and thoroughly explained.

> ⭐ **Don’t forget to [follow DreyAnd on GitHub](https://github.com/DreyAnd) for more security insights and tools.** His contributions are invaluable to the security community!

---

### 🔍 Overview

The exploit targets the **`/dataBases/upgrademysqlstatus`** endpoint, which mishandles the `statusfile` parameter, allowing unauthorized command execution on the target server.  

- 📢 Check out [LeakIX’s latest update on exploitable CyberPanel instances](https://x.com/leak_ix/status/1850949064826745202).
- 🔗 **See over [22,000 results on LeakIX](https://leakix.net/) related to CyberPanel**.

---

### ⚙️ Features

- 💻 **Interactive Shell** for on-the-fly command execution on a target server.
- 📂 **Bulk Exploitation** with multithreading for multiple targets.
- 📝 **Output File Support** for saving results during bulk operations.

---

### 🛠️ Installation

1. **Clone this repository**:
   ```bash
   git clone https://github.com/Chocapikk/CyberPanel
   cd CyberPanel
   ```

2. **Install dependencies**:
   ```bash
   pip install -r requirements.txt
   ```

---

### 🚀 Usage

Run the tool with the options provided below.

**Basic Commands**:

- **Single target in interactive mode**  
  ```bash
  python exploit.py -u http://example.org
  ```

- **Multiple targets from a file with output**  
  ```bash
  python exploit.py -f targets.txt -o results.txt -t 10 "uname -a"
  ```

### ⚠️ Disclaimer

This tool is intended solely for educational purposes and authorized security testing. **Unauthorized use of this tool on systems without explicit permission from the owner is illegal and unethical.** The developer assumes no liability or responsibility for misuse or damage caused by this tool.

**Use responsibly and only on systems you own or have explicit permission to test.**