# Task-2-Elevate-Labs

Objective: Identify phishing characteristics in a suspicious email sample.

1. Sample Email Overview
Subject: Urgent Account Verification Required
Sender Address: account-security@micr0soft-support.com
Received Date: June 22, 2025
Attachments: None
Email Body :
  “Your account will be suspended in 24 hours unless you verify your login credentials immediately. Click the link below to secure your account.”

2.  Spoofed Sender Address
Real Company Name (Microsoft) is spoofed as “micr0soft-support.com”.
The domain has a zero (“0”) instead of the letter “o”.      
Domain is not an official Microsoft domain.

3.  Header Discrepancies (using MxToolbox or Google Header Analyzer)
SPF Check: Failed
DKIM Check: Failed
DMARC Check: Failed

4. Suspicious Links
Hyperlink text: https://microsoft.com/login
Actual link (on hover): http://security-update-login.micr0soft-verify.co.vu
Redirects to a phishing page mimicking Microsoft login

5.  Threatening Language
Phrases like:
“Your account will be suspended in 24 hours”
“Immediate action required”
“Failure to comply will result in account termination”

6. Mismatched URLs
The visible text looks legitimate, but the actual hyperlink leads to a non-Microsoft phishing domain.
Misleading formatting used to disguise the real destination.

7. Spelling & Grammar Errors
"Your acount will be termnated if you do not responce immediately."
Errors Found: "acount", "termnated", "responce"

8. | Indicator           | Description                            |
| ------------------- | -------------------------------------- |
| 🚨 Spoofed Email    | Fake domain resembling Microsoft       |
| 📛 Header Failures  | SPF, DKIM, DMARC all failed            |
| 🔗 Suspicious Links | Mismatched, redirects to fake login    |
| ⏳ Urgent Language   | Pressure to act quickly                |
| ❌ Grammar Mistakes  | Multiple typos and errors              |
| 🎭 Visual Deception | Link text disguised to look legitimate |
