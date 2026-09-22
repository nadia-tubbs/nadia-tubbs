# Target Footprint Results: Username Enumeration Log

This log documents discoveries during automated Sherlock username scans, tool errors, and platform limitations.
* *Note: All target usernames and generated URLs in this audit have been changed to placeholders to protect personal privacy and maintain OPSEC rules.*

## 🔍 Raw Terminal Outputs

### Scan 1: Username (Target_A_Redacted)
```text
> sherlock Target_A_Redacted
[*] Checking username Target_A_Redacted on:

[+] Discord: https://discord.com
[+] F3.cool: https://f3.cool
[+] Xbox Gamertag: https://xboxgamertag.com

[*] Search completed with 3 results
```

### Scan 2: Username (Target_B_Redacted)
```text
> sherlock Target_B_Redacted
[*] Checking username Target_B_Redacted on:

[+] F3.cool: https://f3.cool
[+] Pinterest: https://www.pinterest.com

[*] Search completed with 2 results
```

## ⚠️ Tool Errors

* **Discovered Issue:** During both scans, the Sherlock tool reported active account status on the platform `F3.cool` (Links generated: `https://f3.cool` and `https://f3.cool`).
* **Verification Process:** Conducted manual URL validation by attempting to navigate directly to the generated profile links in a web browser.
* **Finding:** Both links returned a `https://f3.cool/lander` GoDaddy page. 
* **Conclusion:** Identified a tool-specific false positive error regarding F3.cool.

## ⚙️ Platform Limitations
* **Instagram Coverage Note:** Target tracking on Instagram could not be executed via this tool. 
* **Analysis:** The Sherlock open-source project officially removed Instagram coverage from its standard target data due to frequent changes on the platform that resulted in high rates of false positives. 


