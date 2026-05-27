# Sub-GHz Rolling Code Analyzer for Flipper Zero

A passive, receive-only (RX) diagnostic application for the Flipper Zero designed to analyze Sub-GHz radio signals and determine if a transmitting device uses static or rolling code security.

## ⚠️ Important Disclaimer & Educational Purpose
**This software is provided for educational, informational, and personal diagnostic purposes only.** 

By downloading, installing, or using this application, you agree to the following terms:
1. **Strictly Passive (RX-Only):** This application only listens to radio frequencies. It does not possess any transmission (TX), emulation, or replay capabilities. It cannot be used to bypass security systems, clone remotes, or interact maliciously with physical infrastructure.
2. **As-Is Provision:** This software is provided "as is" and "with all faults," without warranty of any kind, express or implied, including but not limited to the warranties of merchantability, fitness for a particular purpose, or non-infringement.
3. **Limitation of Liability:** In no event shall the author(s) or copyright holders be liable for any claim, damages, data loss, device malfunction ("bricking"), or other liability, whether in an action of contract, tort, or otherwise, arising from, out of, or in connection with the software or the use or other dealings in the software.
4. **Legal Compliance:** It is the sole responsibility of the end-user to ensure that using this application complies with all local, state, federal, and international laws regarding radio frequency monitoring.

Use entirely at your own risk.

---

## 🔍 How It Works
This tool operates as a digital magnifying glass for radio data:
1. **First Capture:** The app passively listens to a designated frequency and records the incoming data payload from a remote button press.
2. **Second Capture:** The app listens for a second consecutive press from the same remote.
3. **Analysis:** The tool compares the two data packets:
   * **Static Code:** If the payloads are identical, the system uses static coding (vulnerable to replay).
   * **Rolling Code:** If the payloads differ, the system utilizes rolling/dynamic security mechanisms.

---



---

## 📜 License
This project is licensed under the **GNU General Public License v3.0 (GPL-3.0)**. 

Under this license, anyone is free to fork, modify, and distribute this software, provided that:
* All derivative works and forks **must remain 100% open-source**.
* The code cannot be repackaged into proprietary, closed-source software.
* Any modified versions must be distributed under the exact same GPL-3.0 license terms.

See the `LICENSE` file in this repository for the full legal text.
