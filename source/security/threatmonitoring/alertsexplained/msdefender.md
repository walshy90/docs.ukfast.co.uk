```eval_rst
.. meta::
     :title: MS Defender Rules Explained | UKFast Documentation
     :description: Our Threat Monitoring ruleset explained
     :keywords: threat monitoring, alerts, security, compliance, rules, rulesets, ukfast, hosting, file integrity monitoring, rootkit, detection, vulnerability scan, scans, hids, intrustion detection, set up
```
# MS Defender

## Windows Defender detected potentially unwanted software.

### What does this rule mean?


Defending your server from viruses and malware, this rule triggers when Windows Defender (Microsofts Anti Virus and Malware Solution) detects a suspicious PUP (Potentially Unwanted Program) program. As stated, this is flagged as a potentially unwanted program or software.

Many attackers follow an attack with malware. Installing a trojan, backdoor or, rootkit or RAT on your server is high on an attackers priority list. Should they be discovered, and the exploits patched, this malware could allow the attacker to regain access to your server, potentially bypassing authentication and auditing techniques.

### What triggers this rule?


One of the most common triggers for this rule is unwanted software that is installed along with third-party applications, ranging Tool Bars to viruses like the infamous PCOptimiserPro Trojan. This rule can also trigger when legitimate software is triggered. This can happen when Windows doesn't recognise an application.

### What action do I need to take?


As a first responder, you should log into the server in question to determine whether the PUP (Potentially Unwanted Program) was deleted by the anti-virus software. If the action was taken, we recommend manually running another system scan to check for any remnants of the malware. Should the malware be present on the system still, it should be removed, either through the anti-virus program or manually? Then, a manual anti-virus scan should be run. 