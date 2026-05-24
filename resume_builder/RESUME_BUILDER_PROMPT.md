# Resume Builder Prompt

## Overview

This prompt generates a tailored, ATS-optimized resume for **Khanin Chomphusri** based on a provided job description. The output must follow the exact structure, formatting conventions, and character-count guidelines defined below. All content must be drawn from the knowledge base (`KNOWLEDGE_BASE.html`) — do not invent or exaggerate facts.

---

## Instructions for the AI Agent

You will receive:
1. The content of `KNOWLEDGE_BASE.html` (career data source of truth)
2. A **job description** (target role)

Your task:
- Select and reframe the most relevant experiences, projects, and skills from the knowledge base to match the job description
- Use the exact section structure and formatting rules below
- Mirror the writing style: active voice, strong action verbs, no personal pronouns ("I", "my"), metric-first when available
- Prioritize keywords from the job description naturally throughout the resume (for ATS compatibility)
- Do NOT include sections with no relevant content — omit rather than pad

---

## Output Structure & Formatting Rules

### 1. Header

```
[Full Name]
[Tailored Professional Title]

[Summary paragraph]

[email]   [phone]   [location]   [github or portfolio]
```

- **Full Name**: `Khanin Chomphusri` — always unchanged
- **Professional Title**: Tailor to the job description (e.g. "Senior Flutter Engineer" or "Frontend Architect — Angular / Flutter"). Max **60 characters**.
- **Summary paragraph**: 2–4 sentences. Max **400 characters total**.
  - Sentence 1: Who you are + primary expertise domain (~100 chars)
  - Sentence 2: Strongest quantifiable achievement relevant to the role (~120 chars)
  - Sentence 3: Secondary skill area that matches the JD (~80 chars)
  - Sentence 4 (optional): Passion / forward-looking statement relevant to the role (~80 chars)
- **Contact line**: single line, pipe or space separated — email, phone, location, GitHub/portfolio

---

### 2. Technical Skills

3 lines maximum. Each line = one category label + comma-separated values.

Format:
```
[Category Label]: [Skill 1], [Skill 2], [Skill 3], ...
```

- Each line max **120 characters**
- Category labels should reflect the JD (e.g. "Mobile & Frontend", "Backend & AI", "Architecture & Tools")
- Order categories by relevance to the job description (most relevant first)
- Only include skills that appear in the knowledge base AND are relevant to the JD

---

### 3. Work Experience

Format per role:
```
[Job Title]
[Company Name]                                    [Start] - [End]
[City, Country]
[One-line company/engagement context sentence]

• [Achievement bullet 1]
• [Achievement bullet 2]
• [Achievement bullet 3]
• [Achievement bullet 4 — optional]
```

- **Job Title**: Tailor wording to match JD language while staying truthful. Max **70 characters**.
- **Context sentence**: 1 sentence explaining the company or engagement. Max **120 characters**. Omit if obvious.
- **Bullet points**: 3–4 per role. Each bullet max **160 characters**.
  - Always start with a strong action verb (Architected, Engineered, Spearheaded, Delivered, Implemented, etc.)
  - Lead with the most impressive / most JD-relevant achievement
  - Include at least one metric per role where available (%, count, scale, duration)
  - Focus on impact, not task description
- **Roles to include**: Select 3–4 most relevant roles. Always include current role (Oivan Digital). Deprioritize or omit Toyota / Sathien if the JD is purely technical.

---

### 4. Personal Projects

Format per project:
```
[Project Name] ([URL or platform]) | [Your Role]
• [Achievement/feature bullet 1]
• [Achievement/feature bullet 2]
• [Achievement/feature bullet 3 — optional]
```

- **Project header**: Max **80 characters**
- **Bullet points**: 2–3 per project. Each bullet max **160 characters**.
  - Same rules as work experience bullets: action verb, impact-first, metric where possible
- Include 2–3 projects max. Select based on JD relevance:
  - Flutter JD → Convert Rai, Coolor Clone, audioarenalab.com
  - Angular / web JD → audioarenalab.com, Fontpalette, realmsup.com
  - AI / backend JD → ZATCA demo, audioarenalab.com, freqtrade
  - Full-stack JD → audioarenalab.com, realmsup.com, ZATCA demo

---

### 5. Education

Format:
```
[Degree Title]: [Field of Study]
[Institution Name]                                [Country]
[Start year] - [End year]
```

- No bullets, no descriptions unless a specific achievement is highly relevant (e.g. scholarship for academic roles)
- Always include both Master's (Loughborough) and Bachelor's (SIIT)
- Add scholarship note for SIIT only if space permits or if the JD values academic excellence

---

### 6. Certificates

Format: inline list, no descriptions
```
[Certificate Name]    [Issuer] via [Platform]
```

- Max **5–7 certificates** — select by JD relevance
- AI/ML JD → IBM RAG & Agentic AI certs, Stanford ML, DeepLearning.AI
- Product / design JD → Product Management: Building AI-Powered Products, UI/UX Design Specialization
- Always omit certs irrelevant to the role to save space

---

### 7. Achievements (optional section)

Include only if space permits or the JD values academic / non-technical merit.

Format:
```
[Achievement title]
[One-line explanation — max 120 characters]
```

- Example: "Full 4-year scholarship at SIIT — awarded for top entrance exam score; GPA requirement maintained throughout."

---

### 8. Languages

Format:
```
[Language]    [Proficiency level]
```

- Always include:
  - Thai — Native Language
  - English (895 TOEIC score) — Full Professional Proficiency
- Place at the end of the resume

---

## ATS Keyword Strategy

- Mirror exact phrases from the job description title and requirements (e.g. if JD says "React Native" and candidate has Flutter, note "Flutter (cross-platform, analogous to React Native)" — never falsely claim React Native)
- Repeat 3–5 core JD keywords naturally across the summary, skills, and at least one bullet
- Avoid keyword stuffing — one natural use per section is enough

---

## Total Length Target

- **1 page** for most roles: aim for ~3,200–3,800 characters of visible text
- **2 pages** only if the JD explicitly calls for senior/staff/architect-level with deep technical depth: max ~6,000 characters
- Cut lower-relevance roles and projects before expanding bullet counts

---

## Input Template

When using this prompt, provide the following:

```
KNOWLEDGE BASE:
[Paste KNOWLEDGE_BASE.html content here]

JOB DESCRIPTION:
[Paste the full job description here]

ADDITIONAL INSTRUCTIONS (optional):
[e.g. "Emphasize AI experience", "This is a startup, keep it concise", "Include ZATCA project"]
```
