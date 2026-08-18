# 🔓 Identity & Access Management | Red Team Session

```assembly
global _start

section .text
_start:
    ; Bypass IAM restrictions & spawn root shell
    mov rax, 59         ; sys_execve
    lea rdi, [binary]   ; "/bin/sh"
    xor rsi, rsi        ; NULL
    xor rdx, rdx        ; NULL
    syscall
```

```bash
\$ whoami
root@totvs-iam-operator

\$ ./identity_audit.sh --target=infrastructure
[+] Corporate Domain: TOTVS S.A. 🏢
[+] Active Role: Information Security / Identity & Access Management (IAM)
[+] Mission: Securing identity perimeters while mastering offensive security.

\$ cat /root/intel/tactics.txt
- Identity Governance & Administration (IGA) / PAM / SSO
- Low-Level Exploit Development (x86_64 Assembly / C)
- Pentesting & CTFs (Red Team)
- Web & AV/EDR Evasion
```

### 📡 Social Connections & Targets

[![LinkedIn](https://shields.io)]([https://linkedin.com](https://www.linkedin.com/in/rian-marques/))
[![Hack The Box](https://shields.io)]([https://hackthebox.com](https://profile.hackthebox.com/profile/019c7098-f21b-700d-9ea7-cc75c3c53c65?utm_medium=copy_url))
[![TryHackMe](https://shields.io)]([https://tryhackme.com](https://tryhackme.com/p/rianmarquesmateus))

---

### 🧰 The Security Ecosystem

| Domain | Technologies & Toolset |
| :--- | :--- |
| **Identity & IAM** | **`IAM/IGA`** **`PAM`** **`OAuth2`** **`SAML`** **`Active Directory`** |
| **Red Team & Web Pentest** | ![Burp Suite](https://shields.io) ![Nmap](https://shields.io) ![Metasploit](https://shields.io) ![OWASP](https://shields.io) |
| **Offensive Tools** | ![GDB](https://shields.io) ![Kali Linux](https://shields.io) **`Ghidra`** **`Mimikatz`** |

---

### 📊 Compromised Metrics & Contributions
<p align="left">
  <img src="https://vercel.app" alt="GitHub Stats" height="160" />
</p>
