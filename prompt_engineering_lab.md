# 🧪 Hands-On Lab: Prompt Engineering for Law Enforcement
### Module 2 | GenAI Training Programme for IPS Officers
**Duration:** 60 Minutes | **Format:** Individual + Group Exercise  
**Tools Required:** ChatGPT (chat.openai.com) or Claude (claude.ai) — browser access needed

---

> **Facilitator Note:** Walk participants through the TODO section of each exercise first. Give them time to attempt it independently. Only reveal the Solution section after the group has tried. Encourage participants to compare their outputs with the model solution — differences are learning opportunities, not mistakes.

---

## 🗺️ Lab Structure at a Glance

| # | Exercise | Type | Time |
|---|----------|------|------|
| 1 | Bad Prompt vs Good Prompt | Individual | 10 min |
| 2 | Drafting an Official Government Letter | Individual | 15 min |
| 3 | Summarising a Case Document | Individual | 10 min |
| 4 | Preparing a Briefing Note | Pair Work | 10 min |
| 5 | Refining AI Output for Government Standards | Group | 10 min |
| — | Debrief & Discussion | Group | 5 min |

---

## 📋 The C-T-F-E-C Framework (Keep This Open)

Every good prompt must have:

| Component | What it means | Example |
|-----------|--------------|---------|
| **C** — Context | Who you are, your role, the situation | *"You are an SSP in Punjab..."* |
| **T** — Task | Exactly what you want the AI to do | *"Draft a letter to..."* |
| **F** — Format | How the output should be structured | *"Use GoI letter format..."* |
| **E** — Examples | A sample tone or style to follow | *"Formal, third-person, official..."* |
| **C** — Constraints | Word limits, things to avoid, compliance rules | *"Under 300 words, no jargon..."* |

---

---

# ✅ EXERCISE 1: Bad Prompt vs Good Prompt
**Time: 10 minutes**

---

## 📝 TODO LIST

### Task 1.1 — Identify What's Wrong
Read the following prompt carefully. List **at least 4 things** that are wrong or missing from it:

```
Write something about a missing child case.
```

Write your observations here:
1. _______________________________________________
2. _______________________________________________
3. _______________________________________________
4. _______________________________________________

---

### Task 1.2 — Rewrite the Prompt
Using the **C-T-F-E-C Framework**, rewrite the above bad prompt into a good prompt for drafting a formal police communication about a missing child case. Use the space below:

```
YOUR REWRITTEN PROMPT:

[Write here]
```

---

### Task 1.3 — Test It
Paste your rewritten prompt into ChatGPT or Claude. Note:
- Did the output look like an official government document?
- What would you change in a second attempt?

---

## ✅ SOLUTION — Exercise 1

### Task 1.1 — What's Wrong with the Bad Prompt

| # | Problem | Why It Matters |
|---|---------|----------------|
| 1 | No role context | AI defaults to civilian tone, not police/official voice |
| 2 | No recipient defined | AI doesn't know who this is addressed to |
| 3 | No format specified | Output arrives as unstructured prose |
| 4 | No case details provided | Output is generic and unusable |
| 5 | No constraints | No word limit, language standard, or compliance requirement |
| 6 | No purpose stated | Unclear if this is an FIR, a letter, a notice, or a press release |

---

### Task 1.2 — Model Good Prompt

```
You are a Superintendent of Police (SP) in a district in India. A 9-year-old child named
Riya Sharma went missing from the Sadar Bazaar area on the evening of 14 May 2025.
The child was last seen wearing a blue school uniform. A formal complaint has been 
registered as FIR No. 112/2025.

Draft a formal government letter to the District Magistrate requesting inter-district 
coordination and activation of the Missing Child Alert protocol. 

The letter must:
- Follow standard Government of India correspondence format
- Include: Subject line, Reference number placeholder, Salutation, Body (3 paragraphs), 
  Closing, and Signature block with designation
- Be written in formal English, third-person voice
- Be under 350 words
- Avoid casual language, abbreviations, or vague statements
- End with a clear action request and timeline

Use the tone of an official police communication intended for a senior district authority.
```

---

### Task 1.3 — What to Look For in the Output
A good output should include:
- `From:`, `To:`, `Subject:`, `Ref No.:`, `Date:` in header
- Formal salutation: *"Respected Sir/Madam"*
- Body: Situation summary → Action requested → Urgency/timeline
- Closing: *"Yours faithfully"* with name, designation, and district

---

---

# ✅ EXERCISE 2: Drafting an Official Government Letter
**Time: 15 minutes**

---

## 📝 TODO LIST

### Scenario
You are the **Deputy Commissioner of Police (DCP), Cyber Crime, Mumbai**. A series of coordinated UPI fraud cases have been reported across Maharashtra, Gujarat, and Rajasthan, targeting senior citizens. Your investigation has traced one key suspect to a mobile number registered in Ahmedabad. You need formal cooperation from the Gujarat Police.

---

### Task 2.1 — Build Your Prompt Using C-T-F-E-C
Fill in each component before writing your full prompt:

| Component | Your Input |
|-----------|-----------|
| **Context** (your role + situation) | |
| **Task** (what should AI do) | |
| **Format** (letter structure required) | |
| **Examples** (tone/style guidance) | |
| **Constraints** (limits + compliance) | |

---

### Task 2.2 — Write the Full Prompt
Combine all five components above into one complete prompt:

```
YOUR FULL PROMPT:

[Write here]
```

---

### Task 2.3 — Generate and Evaluate
Paste your prompt into ChatGPT or Claude. Evaluate the output against this checklist:

- [ ] Proper GoI letter header (From, To, Subject, Date, Ref No.)
- [ ] Formal salutation
- [ ] Clear statement of the cybercrime situation
- [ ] Specific assistance requested (not vague)
- [ ] Mention of case reference / FIR number
- [ ] Professional closing with designation
- [ ] Under the word limit you specified

If any boxes are unchecked — refine your prompt and try again.

---

## ✅ SOLUTION — Exercise 2

### Task 2.1 — C-T-F-E-C Breakdown

| Component | Model Answer |
|-----------|-------------|
| **Context** | DCP Cyber Crime, Mumbai. Multi-state UPI fraud case targeting senior citizens. Suspect traced to Ahmedabad. |
| **Task** | Draft a formal letter to the Commissioner of Police, Ahmedabad requesting subscriber data and detention of a suspect |
| **Format** | GoI official letter format — From/To/Subject/Ref No./Date/Body/Closing/Signature block |
| **Examples** | Formal, third-person, factual — similar to an official police communication docket |
| **Constraints** | Under 400 words. No casual language. Include specific legal provision (IT Act Section 66D). Clearly state the urgency and requested action timeline. |

---

### Task 2.2 — Model Full Prompt

```
You are the Deputy Commissioner of Police (DCP), Cyber Crime Division, Mumbai Police.

A coordinated UPI fraud scheme has been uncovered targeting senior citizens across 
Maharashtra, Gujarat, and Rajasthan. Victims were contacted via spoofed bank helpline 
numbers and defrauded of amounts ranging from ₹50,000 to ₹8,00,000 each. 
A total of 47 complaints have been registered. Digital forensics have traced a primary 
suspect's mobile number (registered in Ahmedabad) as the coordination point for the 
fraud network.

Draft a formal official letter to the Commissioner of Police, Ahmedabad City requesting:
1. Immediate subscriber detail verification for the identified mobile number
2. Detention and questioning of the suspect if located
3. Sharing of any related complaints filed in Gujarat jurisdiction

The letter must:
- Follow Government of India official correspondence format
- Include: From, To, Subject, Reference No. (use placeholder), Date, and formal 
  Signature block with designation and office address
- Reference IT Act Section 66D (cheating by personation using computer resource)
- Be written in formal third-person English
- Be under 400 words
- State a clear response timeline: within 72 hours given the ongoing nature of the fraud
- Avoid vague language — every request must be specific and actionable

Maintain the tone of a senior police officer writing to a counterpart in another state.
```

---

### Task 2.3 — Expected Output Structure

```
FROM:    DCP (Cyber Crime), Mumbai Police
TO:      The Commissioner of Police, Ahmedabad City
SUBJECT: Request for Inter-State Cooperation — UPI Fraud Case / IT Act Section 66D
REF NO.: MUM/CYB/2025/___
DATE:    [Date]

Respected Sir/Madam,

[Para 1 — Background of the fraud case]
[Para 2 — Specific investigative findings linking Ahmedabad suspect]
[Para 3 — Specific requests with legal provision cited]
[Para 4 — Timeline and urgency]

Yours faithfully,
[Name]
Deputy Commissioner of Police (Cyber Crime)
Mumbai Police
```

---

---

# ✅ EXERCISE 3: Summarising a Case Document
**Time: 10 minutes**

---

## 📝 TODO LIST

### Scenario
You have received a 12-page forensic audit report on a financial fraud case. Your SP has asked for a 1-page executive summary to present at a senior officers' review meeting in 30 minutes. You will use AI to generate the summary.

---

### Task 3.1 — Write a Summarisation Prompt
Below is an excerpt from the report. Write a prompt that instructs AI to produce a clean, 1-page executive summary suitable for a senior officers' meeting.

**Report Excerpt (use this as the document):**

```
FORENSIC AUDIT REPORT — EXCERPT
Case: Financial Irregularities in Municipal Procurement, Nashik District
Period Under Review: April 2022 – March 2024

Findings:
1. Procurement orders worth ₹4.2 crore were issued to three shell companies — 
   M/s Ratan Enterprises, M/s Bhumi Traders, and M/s Shree Agencies — all registered 
   at the same address in Nashik with overlapping directorship.
2. Payments were processed within 24–48 hours of invoice submission, bypassing the 
   standard 21-day verification period mandated by GFR 2017.
3. Physical verification confirms that no work or supply was delivered against 14 of 
   the 22 purchase orders examined.
4. Bank account analysis reveals that ₹3.1 crore was transferred to a single personal 
   account within 72 hours of credit, indicating layering consistent with money 
   laundering patterns.
5. The approving officer's digital signature was used on 9 occasions outside business 
   hours, including two instances on declared public holidays.
6. Whistleblower testimony corroborated by CCTV logs indicates that physical documents 
   were removed from the records room on 3 separate occasions in January 2024.
```

Write your summarisation prompt here:

```
YOUR PROMPT:

[Write here]
```

---

### Task 3.2 — Evaluate the Output
Check if the AI-generated summary includes:
- [ ] Total amount under scrutiny
- [ ] Key irregularities (brief, not exhaustive)
- [ ] Potential legal violations identified
- [ ] Recommended immediate actions
- [ ] Presented in bullet or section format suitable for a briefing

---

## ✅ SOLUTION — Exercise 3

### Model Summarisation Prompt

```
You are a senior IPS officer preparing a briefing for a review meeting. 

Below is an excerpt from a forensic audit report on a financial fraud case in Nashik. 
Based on this content, produce a structured 1-page Executive Summary that:

- Opens with a 2-sentence Case Overview (what happened, total amount, period)
- Lists Key Findings in no more than 5 bullet points — each under 25 words
- Identifies Applicable Legal Provisions (IPC / Prevention of Corruption Act / PMLA)
- Recommends 3 Immediate Actions for the investigating team
- Ends with a Risk Assessment sentence (one line on urgency level)

Format: Use bold headers for each section. Total output should not exceed 350 words.
Write in formal, precise language suitable for a senior officers' review meeting.
Avoid legal jargon — write for a senior administrator, not a lawyer.

--- REPORT EXCERPT BELOW ---

[Paste the report excerpt here]
```

---

### Expected Output Structure

```
EXECUTIVE SUMMARY — NASHIK MUNICIPAL PROCUREMENT FRAUD

CASE OVERVIEW
Financial irregularities totalling ₹4.2 crore identified in municipal procurement 
between April 2022 and March 2024 involving shell companies and bypassed verification.

KEY FINDINGS
• Three shell companies at same address received ₹4.2 crore in procurement orders
• Payments processed in 24–48 hrs vs. mandatory 21-day GFR 2017 verification period
• 14 of 22 purchase orders show no delivery of work or supply
• ₹3.1 crore transferred to personal account within 72 hrs — possible layering
• Approving officer's digital signature used outside hours including public holidays

APPLICABLE LEGAL PROVISIONS
IPC Sec 420 (cheating), Prevention of Corruption Act 1988, PMLA 2002 (Sec 3 — 
money laundering), IT Act Sec 66 (unauthorised use of digital signature)

IMMEDIATE ACTIONS RECOMMENDED
1. Freeze the identified personal account and the three shell company accounts
2. Impound digital signature records and initiate forensic audit of login timestamps
3. Secure records room under seal and initiate custodial inquiry re: document removal

RISK LEVEL: HIGH — Active destruction of evidence risk; immediate asset freezing advised.
```

---

---

# ✅ EXERCISE 4: Preparing a Briefing Note
**Time: 10 minutes | Pair Work**

---

## 📝 TODO LIST

### Scenario
Work with the officer next to you. You are jointly preparing a briefing note for your DGP on the growing threat of **AI-generated deepfake videos being used in sextortion cases** targeting government employees across India. The DGP has 5 minutes to read the note before a press interaction.

---

### Task 4.1 — Divide and Draft (5 minutes)
**Officer A** writes the prompt for the threat background section.  
**Officer B** writes the prompt for the recommended response and action points section.

```
OFFICER A — Threat Background Prompt:

[Write here]


OFFICER B — Recommended Response Prompt:

[Write here]
```

---

### Task 4.2 — Combine and Generate (5 minutes)
Merge both prompts into one single comprehensive prompt. Generate the full briefing note. Review it together and note one thing each of you would refine.

Officer A would refine: _______________________________________________

Officer B would refine: _______________________________________________

---

## ✅ SOLUTION — Exercise 4

### Model Combined Prompt

```
You are a senior IPS officer drafting an urgent briefing note for the Director General 
of Police (DGP).

The subject is: AI-generated deepfake videos being weaponised in sextortion cases 
targeting government employees and officers across India. Several cases have been 
reported in the past 6 months in Delhi, Bengaluru, and Hyderabad.

Produce a structured 1-page Briefing Note that includes:

SECTION 1 — THREAT OVERVIEW (3–4 sentences)
- What is happening, who is being targeted, how deepfakes are being created and deployed

SECTION 2 — SCALE AND INTELLIGENCE (3 bullet points)
- Known statistics or patterns from recent reported cases
- Typical ransom/extortion demand range
- Platforms being exploited (WhatsApp, Telegram, email)

SECTION 3 — CURRENT LAW ENFORCEMENT GAPS (2–3 bullet points)
- Why existing response frameworks are insufficient
- Jurisdictional and technological investigation challenges

SECTION 4 — RECOMMENDED ACTIONS (numbered, maximum 5)
- Immediate, short-term, and policy-level recommendations
- Include one recommendation on inter-agency coordination with CERT-In and MeitY

SECTION 5 — SUGGESTED DGP TALKING POINT (1–2 sentences for press interaction)
- Reassuring but firm tone, acknowledging the threat while signalling action

Format: Formal briefing note. Use bold section headers. Under 400 words total.
Tone: Clear, direct, no sensationalism. Written for a very senior audience with 5 
minutes to read and absorb.
```

---

---

# ✅ EXERCISE 5: Refining AI Output for Government Standards
**Time: 10 minutes | Group Exercise**

---

## 📝 TODO LIST

### Scenario
The group will collectively review the AI output below. It was generated from a basic prompt ("Write a letter from police to a bank about a fraud case"). The output is useful but does **not** meet Government of India correspondence standards.

---

### Raw AI Output to Evaluate

```
Hey,

I'm writing to let you know that we're investigating a fraud case and we need your help. 
One of your customers has been involved in some suspicious transactions. We'd like you 
to freeze the account and send us the transaction history for the past 6 months. This is 
pretty urgent so please get back to us ASAP.

The account number is 9876543210 and the branch is MG Road, Bengaluru.

Let me know if you need anything else.

Thanks,
Inspector Raj
```

---

### Task 5.1 — Group Audit (5 minutes)
As a group, identify everything wrong with this output. Use the table:

| # | Problem Found | What It Should Be Instead |
|---|--------------|--------------------------|
| 1 | | |
| 2 | | |
| 3 | | |
| 4 | | |
| 5 | | |
| 6 | | |

---

### Task 5.2 — Write a Refinement Prompt (5 minutes)
Write a follow-up prompt you would give the AI (after its first output) to fix this letter:

```
REFINEMENT PROMPT:

[Write here]
```

---

## ✅ SOLUTION — Exercise 5

### Task 5.1 — Problems in the Raw Output

| # | Problem Found | What It Should Be Instead |
|---|--------------|--------------------------|
| 1 | Casual greeting "Hey" | Formal salutation: *"The Branch Manager / Respected Sir or Madam"* |
| 2 | Informal tone throughout | Formal, third-person official tone |
| 3 | "ASAP" — unprofessional | Specific timeline: *"within 48 hours of receipt of this letter"* |
| 4 | No letter header (From/To/Subject/Ref No./Date) | Full GoI correspondence header required |
| 5 | No legal provision cited | Should reference CrPC Section 91 (production of documents) or relevant provision |
| 6 | No designation, office, or official signature block | Full designation, police station, district, contact number |
| 7 | No FIR reference | Mandatory: *"FIR No. ___/2025 under Section ___ IPC"* |

---

### Task 5.2 — Model Refinement Prompt

```
The letter above was generated but does not meet government correspondence standards. 
Please completely rewrite it as a formal official police letter with the following corrections:

1. Add a proper GoI letter header: From (Inspector's name, designation, police station, 
   district), To (Branch Manager, bank name, branch address), Subject line, Reference 
   number (use placeholder), and Date

2. Replace all casual language with formal third-person official language throughout

3. Add the legal basis for the request — cite CrPC Section 91 (order to produce 
   documents) and mention the registered FIR number (use FIR No. ___/2025 as placeholder)

4. Replace "ASAP" with a specific action timeline: compliance within 48 hours

5. Expand the body to include three formal paragraphs:
   - Para 1: Reference to the case and nature of fraud
   - Para 2: Specific documents/actions requested with legal authority
   - Para 3: Consequence of non-compliance and contact details for coordination

6. Close with: "Yours faithfully," followed by full name, designation, badge number, 
   police station, district, and office phone number

Output must be under 350 words and ready for signature without further editing.
```

---

---

## 🏁 Debrief & Discussion (5 minutes)

### Key Questions for the Group

1. **Which exercise was hardest?** Why — was it knowing what to ask, or how to phrase it?

2. **What surprised you** about the difference between your first prompt and the model solution?

3. **The Accountability Question:** If an AI drafts an official letter and it contains a factual error — who is responsible? The officer who signed it, or the AI?

4. **One Commitment:** Name one routine task in your current role where you will use prompt engineering starting this week.

---

## 📌 Quick Reference Card — Take This With You

### The C-T-F-E-C Framework

```
C — CONTEXT    : Your role, designation, situation
T — TASK       : Exactly what you want AI to do  
F — FORMAT     : Letter / Summary / Bullet list / Table
E — EXAMPLES   : Tone, style, or sample to follow
C — CONSTRAINTS: Word limit, compliance rules, what to avoid
```

### Three Ready-to-Use Prompt Starters

**For Official Letters:**
> *"You are a [Designation] in [State/City]. Draft a formal letter to [Recipient] regarding [Subject]. Use GoI correspondence format. Include subject line, ref number, and signature block. Under [X] words. Formal third-person tone."*

**For Summarising Documents:**
> *"Summarise the following document in [X] bullet points / [X] words. Target audience: [senior officers / DGP / press]. Highlight: key findings, legal implications, and recommended actions. Avoid jargon."*

**For Briefing Notes:**
> *"Draft a briefing note for [Senior Officer/Designation] on [Topic]. Include: threat overview, key facts, gaps, and [X] recommended actions. Under [X] words. Formal tone. Ready to read in 5 minutes."*

---

### Golden Rule

> **AI is a first-draft engine. The officer is always the final authority.**  
> Review every output. Verify every fact. Sign only what you stand behind.

---

*Lab designed for IPS Officers GenAI Training Programme | Module 2: Introduction to GenAI & Prompt Engineering*  
*Facilitator: [Name] | Organisation: [Organisation]*
