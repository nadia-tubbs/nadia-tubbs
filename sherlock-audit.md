# Target Footprint Results: Username Enumeration Log

This log documents the active web nodes discovered during automated Sherlock username scans, including the manual verification of tool errors and platform limitations.

## 🔍 Raw Terminal Outputs

### Scan 1: Username (stellaax182)
```text
 sherlock stellaax182
[*] Checking username stellaax182 on:

[+] Discord: https://discord.com
[+] F3.cool: https://f3.cool/stellaax182/
[+] Xbox Gamertag: https://xboxgamertag.com

[*] Search completed with 3 results
```

### Scan 2: Username (thekaffeebear)
```text
> sherlock thekaffeebear
[*] Checking username thekaffeebear on:

[+] F3.cool: https://f3.cool/thekaffeebear/
[+] Pinterest: https://www.pinterest.com/thekaffeebear/

[*] Search completed with 2 results
```

## ⚠️ Tool Error & Data Verification Log

* **Discovered Issue:** During both scans, the Sherlock tool reported active account status on the platform `F3.cool` (Links generated: `https://f3.cool/stellaax182/` and `https://f3.cool/thekaffeebear/`).
* **Verification Process:** Conducted manual URL validation by attempting to navigate directly to the generated profile links in a secure web browser.
* **Finding:** Both links returned a `https://f3.cool/lander` GoDaddy page. 
* **Conclusion:** Identified a tool-specific false positive error regarding F3.cool. Automated tool outputs must always be manually verified and cross-referenced before being trusted in an investigation.

## ⚙️ Scope Limitations & Platform Updates
* **Instagram Coverage Note:** It was noted during tool assessment that target tracking on Instagram could not be executed via this tool. 
* **Analysis:** The core Sherlock open-source project officially removed Instagram coverage from its standard target data arrays due to frequent structural changes on the platform that resulted in high rates of false positives. 


