# Omegle IP Logger

A Proof-of-Concept Educational Tool for Demonstrating Web Privacy Vulnerabilities

---

## Disclaimer and Legal Notice

This tool and its source code are provided STRICTLY FOR EDUCATIONAL AND RESEARCH PURPOSES ONLY.

The primary goal of this project is to demonstrate how real-time web connections can potentially leak sensitive information, such as IP addresses, even in services marketed as "anonymous." It is intended for security professionals, students, and developers to understand these vulnerabilities and to promote the adoption of better security practices, such as using a reliable VPN.

You must only use this tool on systems you own or have explicit, written permission to test. Unauthorised use of this tool to gather information from individuals without their consent is illegal and unethical. The developer, @xelor7, is not responsible for any misuse or damage caused by this software.

By using this repository, you agree to use it responsibly and legally.

## Purpose

This script serves as a Proof-of-Concept (PoC) to illustrate a specific information disclosure vulnerability. It is a practical demonstration for:

- Security Researchers: To analyze and understand client-side data leakage.
- Educators and Students: To learn about web security, WebRTC, and privacy in a controlled environment.
- Privacy-Conscious Users: To see firsthand why tools like VPNs are critical for online anonymity.

## Installation and Usage

Follow these steps precisely to execute the script in your browser's development console.

### Prerequisites:
- A modern web browser (Chrome, Firefox, Edge, etc.).
- Basic knowledge of how to open the browser's developer console.

### Step-by-Step Guide:

1.  Navigate to Omegle: Open your web browser and go to the Omegle website.
2.  Open Developer Tools: Once on the site, press the F12 key on your keyboard. Alternatively, you can right-click on the page and select "Inspect".
3.  Select the Console Tab: Inside the Developer Tools window, click on the "Console" tab. This is where you will paste and run the JavaScript code.
4.  Paste the Code: Copy the entire script from the script.js file in this repository. Return to the Console tab and paste the code.
    - Note: If the browser prevents you from pasting, simply type "allow pasting" in the console and press Enter. You should then be able to paste the script successfully.
5.  Execute the Script: Press Enter to run the code. The script will now be active.

The script will attempt to log connection details to the console. Observe the output to see the demonstrated vulnerability.

## How It Works (Technical Overview)

This script exploits the way peer-to-peer (P2P) connections are established in some web applications. It attempts to intercept and log the Session Description Protocol (SDP) offers, which can contain candidate IP addresses (including your local and public IP) necessary for establishing a direct connection via WebRTC. This demonstrates a potential privacy leak inherent in the platform's design.

## License

This project is licensed for educational use. Refer to the LICENSE file for more details.

---

## Developed by @xelor7

Remember: With great power comes great responsibility. Use your knowledge to improve security, not to exploit it.
