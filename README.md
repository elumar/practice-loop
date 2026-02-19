# Interview Practice Tool

A lightweight, browser-based interview practice tool. Draw a random question, answer against a timer, and handle follow-up questions — simulating real interview pressure without any backend or dependencies.

## Files

| File | Purpose |
|------|---------|
| `index.html` | The practice app — runs entirely in the browser |
| `questions.csv` | Question bank — edit this to add, remove, or adjust questions |

## How to Use

1. Open `index.html` in any browser (or via GitHub Pages)
2. Use the category filters to focus on a specific skill area
3. Click **Draw Question** — the question appears and the timer starts
4. Answer out loud (record via WebEx or similar)
5. Click **Answered** — timer stops, elapsed time is shown, and a follow-up question appears
6. Answer the follow-up, then draw the next question

## Editing the Question Bank

Open `questions.csv` in Excel, Google Sheets, or any text editor.

**Column structure:**

| Column | Description |
|--------|-------------|
| `question` | The interview question |
| `category` | Category label (used for filtering) |
| `time_seconds` | Timer duration in seconds (e.g., `120` = 2 minutes) |
| `followups` | Follow-up questions separated by `\|` (pipe character) |

**Example row:**
```
"Tell me about a time you resolved a conflict between two teams.",Conflict Resolution,120,"What was the hardest part?|What would you do differently?"
```

**Categories included:**
- Conflict Resolution
- Influencing Without Authority
- Competing Priorities
- Cross-Functional Work
- Executive Communication
- Process Improvement
- Handling Ambiguity
- Failure & Recovery
- Stakeholder Alignment
- Pushing Back
- Learning Agility
- Change Management
- Global Coordination
- Risk Management
- Technical Communication
- Executive Presence
- Delivery Under Constraints
- Team Development
- Program Complexity
- Motivation & Fit
- Vendor Management
- Data-Driven Influence
- Strategic vs Tactical

## Hosting on GitHub Pages

1. Create a new GitHub repository (set to **Private** if preferred)
2. Upload both files: `index.html` and `questions.csv`
3. Go to **Settings → Pages**
4. Set source to `main` branch, root folder
5. GitHub will provide a URL — bookmark it for practice sessions

## Session Workflow (with WebEx)

1. Start a WebEx recording
2. Open the tool in your browser
3. Draw questions and answer out loud
4. After the session, export the transcript
5. Use Claude with your evaluation rubric to score your responses

## Privacy Note

Keep the repository **private** if your question bank contains role-specific content or Apple-tailored answers.
