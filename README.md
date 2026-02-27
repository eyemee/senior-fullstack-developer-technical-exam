# Senior Full Stack Developer Technical Examination

## Candidate Brief
Thank you for taking the time to complete this technical examination.

This assessment is designed to evaluate how you think, prioritize, build, and communicate under a constrained delivery window. We are not looking for a polished production system completed in one hour. We are looking for senior-level judgment, practical execution, sound technical tradeoffs, and a clear demonstration of ownership.

**Duration:** 1 hour  
**Submission format:** Git branch in this repository  
**Select:** One option only

---

## What We Assess
Your submission will be reviewed across the following dimensions:

- Technical judgment
- Execution speed and practicality
- Architecture and organization
- Product thinking
- Integration capability
- Documentation clarity
- Senior-level prioritization and tradeoff management

---

## Submission Protocol

### Branch Naming Convention
Create your submission in a new branch using the following format:

`your-name/senior-fullstack-exam`

**Example:**  
`jane-doe/senior-fullstack-exam`

Do not submit directly to the main branch.

---

## Approved Tooling
You may use any tools, frameworks, and platforms you are comfortable with.

### AI and Build Tools 
- ChatGPT
- Gemini
- Copilot
- Cursor
- Loveable
- Higgsfield
- Open-source libraries
- Free trial tools where applicable
Please note : you can use any tools that you are comfortable working with.

### Automation Platforms
- n8n
- Zapier
- Make.com
- GoHighLevel
  
Please note : you can use any tools that you are comfortable working with.

You may also use mocked integrations where third-party platform limitations prevent a full live implementation. If you do so, you must clearly distinguish between what is real, what is simulated, and what would be required for production readiness.

---

# Examination Options

## Option 1: AI Reel Generator Application for TikTok

### Objective
Build an application that accepts a prompt and generates **video and image reels/posts** intended for TikTok reels.

### Functional Requirements
Your application should include the following capabilities:

#### 1. Prompt Input
Allow a user to enter:
- a text prompt
- an optional style or theme
- an output type:
   - video reel and image reel

#### 2. Media Generation
Generate 
- video and image based content

The output should aim to feel:
- realistic
- commercially usable
- not obviously AI-generated in appearance

#### 3. Dashboard
Include a dashboard that shows:
- generated reels/posts
- generation status
- media previews
- prompt/title
- asset type
- created date/time

#### 4. Reel Library
Include a library or gallery view for previously generated content.

#### 5. TikTok Publishing Flow
Include either:
- a real TikTok publish flow.

### Context
We do not expect a fully production-ready media engine in one hour. We are interested in how you scope, simplify, and connect the critical flow.

---

## Option 2: TikTok Reel Posting Automation

### Objective
Build an automation that posts TikTok reels every **2 minutes**.

The reels may be:
- video reels

### Functional Requirements

#### 1. Trigger
Your workflow must include:
- a **manual trigger** for testing
- a **scheduled trigger** configured to run every 2 minutes for final submission

Please test using the manual trigger first, then revert the workflow to scheduler mode before submission.

#### 2. Google Sheet as Content Repository
Use **Google Sheets** as the reel repository.

Suggested columns:
- ID
- Title
- Caption
- Media URL
- Media Type
- Voiceover URL (optional)
- Status ["Posted", "Ready for Posting"]
- Last Posted At

#### 3. Fetch Logic
Your automation should:
- fetch the next available reel
- prepare it for posting
- once the video is posted - change the status to "POSTED"

#### 4. TikTok Post Action
Use an API call or posting step to TikTok.

#### 5. Status Update
After each attempt, update the Google Sheet with:
- posted / failed status
- timestamp
- optional error message

#### 6. Test Proof
Demonstrate that the workflow runs successfully in test mode before switching it back to scheduler mode.

---

# Technical Expectations
This examination is intentionally time-boxed. Completeness is not the primary goal. Sound judgment is.

A strong submission generally demonstrates:

- disciplined scope control
- a working core workflow
- clean structure and naming
- appropriate technical choices
- clear documentation
- pragmatic handling of third-party limitations

Mocks are acceptable when necessary, but they must be identified clearly.

---

# Required Deliverables
Your submission must include the following:

## 1. Working Branch
Push your solution to your exam branch.

## 2. README
Include a README that explains:
- what you built
- which stack and tools you used
- how to run or test it
- what is complete
- what is mocked, assumed, or partially implemented
- what you would improve with more time

## 3. Source Code or Workflow Export
- For **Option 1**, include the source code
- For **Option 2**, include the workflow export and any supporting files/scripts

## 4. Setup Instructions
Provide clear local setup or testing instructions.

## Stack Used
Frontend, backend, automation platform, APIs, services, and tools used.

## How to Run / Test
Step-by-step instructions.

## Assumptions / Limitations
What was mocked, skipped, or constrained by external platform limitations.

# Important Notes
- Select **one** option only
- Prioritize the **core workflow**
- Make practical tradeoffs
- Clearly label anything mocked or incomplete
- Do not optimize for polish over functionality
- We value clarity and execution over feature volume

## Final Note
This examination is intended to reflect a real-world, time-constrained delivery scenario.

We are not looking for perfection.  
We are looking for strong engineering judgment, decisive execution, and clear communication.

Good luck.
