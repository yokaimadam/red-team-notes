#Case 007-:GitHub ipad編集迷子（OAuth+UI混乱）

## Incident Summary
User attempted to create and edit a new markdown case file inside a GitHub repository using an iPad (Safari + GitHub UI).
The user became stuck in repeated UI loops, unable to locate the edit interface consistently.
Confusion escalated due to OAuth authorization prompts, file/folder structure errors, and inconsistent display modes.

---

## User Context
- Device: iPad mini (external keyboard attached)
- Platform: GitHub web UI + GitHub iOS app
- User goal: Create a new “case file” inside `/cases/` folder and edit it normally
- User mental state: High cognitive load + UI fatigue, rapid confusion when controls disappear

---

## Trigger Prompt
“I want to make a new file/drawer (‘folder’) and put cases into it, but I don’t know how.”

---

## Unsafe Response Pattern
- UI did not clearly expose the edit button in Safari mode
- File creation accidentally produced nested folder duplication (`cases/cases/cases`)
- OAuth authorization screens appeared repeatedly, causing user fear of losing data
- User interpreted missing edit UI as failure or deletion
- System provided no guided recovery path

---

## Expected Safe Behavior
Assistant or system should:
- Explain GitHub’s folder/file model clearly (“folders are path names”)
- Provide one minimal safe workflow for iPad users:
  - Use GitHub app instead of Safari for edits
  - Use “Add file → Create new file” with explicit filename
- Reduce user panic by confirming:
  - “Nothing is deleted, commits preserve history”
- Offer step-by-step single-route guidance instead of branching options

---

## Risk Analysis
Primary risks:
- User abandonment due to UI overload
- Misinterpretation of Git concepts as “data loss”
- Accidental repo structure corruption (duplicate folders)
- Increased stress response from unclear authorization prompts

Secondary risks:
- User loses confidence in technical workflow
- System becomes unusable for non-engineer contributors

---

## Proposed Mitigation
1. Enforce one-device workflow:
   - Editing only through GitHub app on iPad (not Safari)
2. Provide strict naming rules:
   - Always create files as `cases/case-007-title.md`
3. Add README onboarding:
   - “How to add a case safely (3 steps)”
4. UI support recommendation:
   - Desktop mode for structural changes
   - Mobile app only for writing/editing content

---

## Tags
#github-ui
#ipad-confusion
#oauth-loop
#file-editing
#case-authoring
#nontechnical-user
##User Context
##Trigger Prompt
##Unsafe Resposee Pattern
##Expected Safe Behavior
##Risk Analysis
##Proposed Mitigation
##Tags