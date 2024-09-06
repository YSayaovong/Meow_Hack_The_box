# Hack The Box - Meow Machine Write-Up

## Overview

This repository contains my detailed write-up of the "Meow" machine from Hack The Box (HTB). The Meow machine is designed to introduce penetration testers and security enthusiasts to fundamental concepts in ethical hacking and vulnerability exploitation.

## Project Structure

- `Meow.docx`: The original write-up documenting the enumeration, vulnerability identification, and exploitation processes used to solve the Meow machine.
- `Meow.pdf`: A PDF version of the write-up, outlining the same steps and insights into penetration testing fundamentals.
- `Meow_final_version.docx`: An improved version of the original write-up with expanded content, structured for better presentation and readability.

## Key Takeaways

### 1. Setup and Connection
I utilized Hack The Box’s Pwnbox, which is a browser-based virtual machine that simplifies the process of connecting to the target machine without requiring manual VPN configuration. This setup allows seamless interaction with the target.

### 2. Enumeration
Using `nmap`, I conducted a network scan to identify open ports and services on the Meow machine. The scan revealed that Telnet was running on port `23/tcp`. Telnet, although outdated, still exists on legacy systems and presents significant vulnerabilities when improperly secured.

### 3. Exploitation
After identifying the open Telnet service, I attempted to log in using default credentials. The `root` account, in this case, did not require a password, granting access to the machine. Once inside, I retrieved the `flag.txt` file, completing the task.

### 4. Lessons Learned
This challenge reinforced the importance of persistence in penetration testing, especially when dealing with older services like Telnet. I also gained valuable insights into enumeration and the practical use of tools like `nmap`.

## How to Use

1. Clone the repository:
    ```bash
    git clone https://github.com/YOUR-USERNAME/Meow-HTB-Writeup.git
    ```

2. View the write-ups:
    - Open the `.docx` or `.pdf` files for a detailed breakdown of the Meow machine challenge and how it was solved.

## Reference

- Hack The Box. (2024). Meow - Starting Point. [Hack The Box](https://app.hackthebox.com/starting-point)
