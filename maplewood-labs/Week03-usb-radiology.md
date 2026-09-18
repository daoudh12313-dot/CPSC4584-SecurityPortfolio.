# Week 3: Unauthorized USB Drive in Radiology
**Course:** CPSC 4584 | Special Topics in Information Security
**Date:** September 14, 2026
**Analyst:** [Hani Daoud]
**Incident ID:** INC-2026-0914-001

---

## Incident Summary

[An unknown USB drive was detected in the Radiology imaging suite. What tools are needed to safely decode the text?]

---

## Chain of Custody

[Chain of custody exists to maintain the integrity of the evidence found in an investigation. All evidence should be kept intact, and fully documented to prevent evidence from being thrown out in court.]

---

## Key Encoding Finding

**String Found:** Y3VybCAtcyAtbyAvZGV2L251bGw=
**Encoding Type:** [Base64]
**Decoded Content:** [curl -s /dev/nullhdaoud-academy@webshell:~$]
**Significance:** [This finding is important, because the command sends a silent message to a server. This can be a breach of confidentiality.]

---

## Terminal Commands Used

| Command | Purpose |
|---------|---------|
|  echo "unauthorized access" | base64 | [Base64 is represented by characters such as: A-Z, a-z, 0-9, plus, and an equal sign.]|
| echo "Y3VybCAtcyAvZGV2L251bGw="| base64 -d| [The decoded revealed the following: curl -s /dev/nullhdaoud-academy@webshell:~$. Which was silently sending the user's dev folder information to a server.]|
| xxd .bashrc | head -6| [The hex dump showed the file signature, which allowed the evidence to be compared to the file name to reach a consensus. ]|
| strings .bashrc | grep -i "path\|export\|alias" | [Pattern filtering assisted by comparing the same context of the file. The title/description should be the same; if not, then it would raise suspicion.]|

---

## Escalation Recommendation

[I would escalate the incident further to a Tier 2 Analyst. Mainly for the discovery of the unknown USB drive, being found in a restricted area. A question that requires more investigation is the following: whether there was a security breach, and whether data was exfiltrated, via an unknown source/destination.]

---
*CPSC 4584 | Governors State University | Fall 2026*
    
