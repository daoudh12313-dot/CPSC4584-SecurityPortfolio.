# Week 2: Suspicious File on a Nurse's Workstation
**Course:** CPSC 4584 | Special Topics in Information Security
**Date:** September 11, 2026
**Analyst:** [Hani Daoud]
**Incident ID:** INC-2026-0907-001

---

## Incident Summary

A unknown text file was found was found on the home directory, of the clinics workstation. This file itself, contained things that were concerning. It needed to be analyzed, to protect from a possible incident from occurring, within the clinic. 

---

## Key Findings

**Permission Finding:** [The file contained permissions that allowed the account, to have executable privileges on top of the already, read, and write permissions. The executable permissions for a text file raised suspicion. Which warranted for analysis, and possible escalation s. ]
**File Type Finding:** [The command allowed comparison of the description of the file, to the actual file type of said document. This helped verify the document was what it claimed to be.]
**Timestamp Finding:** [The Timestamp Finding uncovered another possible reason for escalation. The Timestamp, showed that the file was accessed outside the, timeline/schedule of the health clinic team.]
**Strings Finding:** [This command help identify the contents of the file, without execution of the file.]

---


## Terminal Commands Used

| Command | Purpose |
|---------|---------|
| pwd && ls -la | [This helped me verify the contents within the directory. The command printed, and listed the all contents(both hidden as well) found in the current directory.] 
| file [patient_notes.txt] | [This allowed me to compare the description against the file type.] |
| stat [patient_notes.txt] | [This command help verify the following, of the file. The Access Date, the last modified date, the change date, and lastly, the Birth date of the file.] |
| strings [patient_notes.txt] | [This command helped simplify/shortens the contents of the said file, which also easier analysis. This command also you read said file, without running/opening its contents.] |
| find . -mtime -1 -type f | [This command helped me identify the contents of the directory tree.] |

---

## Escalation Recommendation

 [I would escalate the incident further, to a Tier 2 Analyst. The strongest evidence that I would present would be, the Timestamp Finding, and the Permission Findings. The Timestamp Finding, began the overall incident response. Which may have, helped protect against further incidents. Lastly, I would go with the Permissions Finding. This is, because the file shows that it has an executable permission, which is odd for a "text file". 

---
*CPSC 4584 | Governors State University | Fall 2026*
