# Incident Response: Security Incident Report – YummyRecipesForMe.com

## 📝 Scenario Summary
This report documents a simulated security incident involving a brute force attack and malware injection on the website `yummyrecipesforme.com`. The incident was part of a cybersecurity analyst exercise focused on identifying threats using tcpdump logs and proposing effective countermeasures.

## 🔍 Investigation Details
- **Attack Type**: Brute force attack on admin panel
- **Threat Actor**: Disgruntled former employee
- **Payload**: Malicious JavaScript embedded into source code
- **Effect**: Users were prompted to download malware and redirected to `greatrecipesforme.com`

## 🧪 Tools Used
- `tcpdump` for packet capture and traffic analysis
- Network protocol analysis of DNS and HTTP activity
- Word processor for formal incident documentation

## 📄 Files Included
- `security-incident-report-yummyrecipesforme.docx` – Formal documentation of the incident
- `tcpdump traffic log.docx` – Captured packet log showing DNS and HTTP activity
- `how-to-read-tcpdump-log.docx` – Reference guide for interpreting tcpdump entries

## 🛡️ Key Findings
- DNS and HTTP traffic were used to redirect users to a malicious site
- The website used a default admin password, which enabled the brute force attack
- No controls were in place to limit login attempts or monitor for unauthorized access

## ✅ Recommendation
Implement account lockout policies and two-factor authentication (2FA) to prevent brute force attacks. Regularly audit and enforce strong password policies.

## 📚 Learning Outcomes
- Performed hands-on tcpdump log analysis
- Applied incident response documentation practices
- Recommended actionable cybersecurity controls

---

*This folder is part of my Cybersecurity Portfolio demonstrating real-world incident response skills.*
"""

# Save the README.md to the appropriate folder
readme_path = "/mnt/data/incident-response-README.md"
with open(readme_path, "w") as file:
    file.write(readme_content)

readme_path
