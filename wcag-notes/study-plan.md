# Study Plan

Map out the topics and how you will study.

# WAS Exam Content Outline
## Legend

### Heading Color Coding
- <span style="color:#2E8B57">**Green (#2E8B57)**</span> → Section mastered or confident  
- <span style="color:#FF8C00">**Orange (#FF8C00)**</span> → In progress  
- <span style="color:#B22222">**Red (#B22222)**</span> → Needs major study  

### Emoji Meaning
**Knowledge level**
- 🟥 = new / no knowledge  
- 🟨 = some understanding  
- 🟩 = solid / confident  

**Study need**
- 📚 = need to study more  
- ⚖️ = ok for now  
- 💤 = low priority / can postpone  

### Progress Calculation
I calculated progress like this:
- 🟩 = **1.0**  
- 🟨 = **0.5**  
- 🟥 = **0.0**  
- 📚 / ⚖️ / 💤 have **no effect** on knowledge score  
- **Percent = (sum of leaf-item scores) ÷ (number of leaf items)**  

---

<h2 style="color:#FF8C00">1 Creating Accessible Web Solutions (40%) — Progress: 43%  
<br>██████░░░░░░░</h2>

- [ ] Guidelines, principles and techniques for meeting success criteria 🟥 📚  
  - [ ] WCAG 2.2 🟨 📚  
  - [ ] WAI-ARIA 🟨 📚  
  - [ ] ATAG 🟥 📚  
  - [ ] basic concepts 🟨 📚  
  - [ ] limitations of the guidelines/techniques 🟥 📚  
  - [ ] normative vs. non-normative 🟥 📚  
  - [ ] conformance levels (A, AA, AAA) 🟨 📚

- [ ] Basic knowledge of programming 🟩 ⚖️  
  - [ ] at a conceptual level 🟩 💤  
  - [ ] principles and concepts related to programming 🟨 📚  
  - [ ] impact of coding practices on accessibility 🟨 📚  

- [ ] Accessibility quality assurance 🟥 📚  
  - [ ] accessibility throughout development lifecycle 🟨 📚  
  - [ ] overlap of UX and accessibility 🟨 📚  

- [ ] Accessibility supported technologies 🟥 📚  
  - [ ] assistive technologies & accessibility features 🟨 📚  
  - [ ] combining AT and user agents 🟨 📚  
  - [ ] choosing accessible-supportive technologies 🟨 📚  
  - [ ] avoiding inaccessible tech (e.g., Flash) 🟨 💤  
  - [ ] differences in AT behavior 🟨 📚  
  - [ ] touch support when screen reader is on/off 🟥 📚  

- [ ] Standard controls vs. custom controls 🟨 📚  
  - [ ] using standard controls when possible 🟩 💤  
  - [ ] WAI-ARIA best practices for custom controls 🟨 📚  

- [ ] Single page applications 🟥 📚  
  - [ ] focus control 🟥 📚  
  - [ ] AJAX + screen reader timing issues 🟥 📚  
  - [ ] live announcements 🟨 📚  

- [ ] Strategies of persons with disabilities 🟨 📚  
  - [ ] screen reader navigation 🟨 📚  
  - [ ] headings and landmarks 🟩 💤  
  - [ ] coping strategies 🟥 📚  
  - [ ] preferred vs. website-specific methods 🟥 📚  
  - [ ] using keyboard vs. mouse 🟩 💤  

---

<h2 style="color:#B22222">2 Identify Accessibility Issues in Web Solutions (40%) — Progress: 27%  
<br>████░░░░░░░░░</h2>

- [ ] Interoperability and compatibility issues 🟥 📚  

- [ ] Identifying guidelines/principles for issues 🟨 📚  
  - [ ] WCAG 2.2 🟨 📚  
  - [ ] WAI-ARIA 🟨 📚  
  - [ ] ATAG 🟥 📚  
  - [ ] basic concepts 🟨 📚  
  - [ ] limitations of guidelines/techniques 🟥 📚  
  - [ ] normative vs. non-normative 🟥 📚  
  - [ ] conformance levels (A, AA, AAA) 🟥 📚  

- [ ] Testing with assistive technologies 🟥 📚  
  - [ ] screen reader navigation 🟨 📚  
  - [ ] headings and landmarks 🟨 📚  
  - [ ] screen magnifiers 🟥 📚  
  - [ ] high contrast 🟥 📚  
  - [ ] keyboard vs. mouse testing 🟩 ⚖️  

- [ ] Testing for end-user impact 🟥 📚  
  - [ ] low vision 🟨 📚  
  - [ ] cognitive 🟨 📚  
  - [ ] mobile/touch 🟨 📚  

- [ ] Testing tools for the web 🟨 📚  
  - [ ] automated tools 🟨 ⚖️  
  - [ ] manual tools 🟨 📚  
  - [ ] unit testing 🟥 📚  
  - [ ] browser-based tools 🟨 📚  
  - [ ] spider tools 🟥 📚  
  - [ ] bookmarklets 🟥 📚  
  - [ ] automated site monitoring tools 🟥 📚  
  - [ ] external accessibility test tools 🟥 📚  

---

<h2 style="color:#B22222">3 Remediating Issues in Web Solutions (20%) — Progress: 0%  
<br>░░░░░░░░░░░░░</h2>

- [ ] Severity & prioritization of issues 🟥 📚  
  - [ ] cost–benefit considerations 🟥 📚  
  - [ ] legal risk 🟥 📚  
  - [ ] user impact 🟥 📚  
  - [ ] identifying root problems 🟥 📚  
  - [ ] determining what to fix first 🟥 📚  

- [ ] Recommending strategies/techniques for fixing issues 🟥 📚  
  - [ ] selecting best solution 🟥 📚  
  - [ ] most widely useful solution 🟥 📚  
  - [ ] feasibility of solution 🟥 📚  
  - [ ] fixing vs. redesign 🟥 📚  
  - [ ] how to fix specific issues 🟥 📚
     
## Prompts
```
I will paste my full checklist below. Each line contains:
- Knowledge emoji: 🟥 = 0, 🟨 = 0.5, 🟩 = 1
- Study emoji: 📚 / ⚖️ / 💤 (ignore for scoring)

Your task:
1. Parse the entire checklist.  
2. Count only *leaf* items (no category headers).
3. Calculate the progress for each major section using:
   Percent = (sum of item scores) ÷ (number of items)
4. Generate a 15-character progress bar using:
   █ = filled, ░ = empty
5. Update each section header with the new progress % and bar.
6. Do NOT change anything else in my checklist except updating numbers + bars.

I will paste my checklist below. Recalculate everything.
```

```
I will paste my full checklist below.

Your task:
Convert it into a standalone HTML dashboard with the following features:
- Use my color-coded section headers.
- Convert each checklist item into an HTML checkbox.
- Preserve my emojis.
- For each section, include:
  - a large progress bar (filled/unfilled)
  - the % number
- Make each section collapsible (details/summary HTML element).
- Use simple, readable CSS (no frameworks).
- Include a light background, rounded boxes, and spacing.
- Make sure the output is valid HTML I can save as "accessibility-dashboard.html" and open in a browser.

After generating the dashboard:
- Do NOT include explanations.
- Only output the final HTML file content.

I will paste my checklist below. Convert it.

```
