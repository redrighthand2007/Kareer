# KAREER
## Personal Career Operating System — Master PRD + Step-by-Step Implementation Plan

**Product Type:** Personal Career Portfolio + Development System  
**Core Concept:** Me-Centered Career OS  
**Frontend:** HTML5 + CSS3 + Vanilla JavaScript ES6+ only  
**Backend:** None for the current version  
**Data:** Local browser storage for the current version  
**Architecture:** Vanilla JS SPA / Hash Router  
**Primary User:** One student — the owner of the Kareer system

---

# 1. PRODUCT DEFINITION

## 1.1 One-Line Definition

**Kareer is a personal career operating system that helps one student understand themselves professionally, choose a direction, build skills, create proof through projects, learn consistently, find opportunities, apply, prepare for interviews, and measure progress.**

The product is **not** primarily a career-information website.

It is **MY career system.**

---

# 2. THE ME-CENTERED PRINCIPLE

Everything revolves around the student.

The central question is not:

> "What careers exist?"

The central question is:

> **"Where am I, where do I want to go, what am I missing, and what should I do next?"**

Career exploration exists only to support that journey.

## Kareer's center

```text
                         ┌───────────────┐
                         │      ME       │
                         │   MY PROFILE  │
                         └───────┬───────┘
                                 │
             ┌───────────────────┼───────────────────┐
             ↓                   ↓                   ↓
          SKILLS              PROJECTS           LEARNING
             │                   │                   │
             └─────────────┬─────┴─────┬─────────────┘
                           ↓
                     TARGET ROLE
                           │
                           ↓
                      SKILL GAPS
                           │
                           ↓
                       ROADMAP
                           │
                           ↓
                     OPPORTUNITIES
                           │
                           ↓
                      APPLICATIONS
                           │
                           ↓
                      INTERVIEWS
                           │
                           ↓
                        RESULTS
                           │
                           ↓
                       PROGRESS
                           │
                           └────────→ ME
```

Every new feature must strengthen this loop.

---

# 3. CORE PRODUCT LOOP

```text
ME
 ↓
PROFILE
 ↓
SKILLS
 ↓
EVIDENCE
 ↓
PROJECTS
 ↓
TARGET ROLE
 ↓
SKILL GAPS
 ↓
ROADMAP
 ↓
LEARNING
 ↓
OPPORTUNITIES
 ↓
APPLICATIONS
 ↓
INTERVIEWS
 ↓
PROGRESS
 ↓
ME
```

This is the fundamental architecture of the product.

---

# 4. PROBLEM

A student's professional information is normally scattered across:

- GitHub
- LinkedIn
- Resume files
- Certificates
- Course platforms
- DSA platforms
- Project folders
- Notes
- Job spreadsheets
- Internship applications

Kareer brings them together into one connected system.

Instead of:

```text
GitHub
LinkedIn
Resume
Certificates
DSA
Courses
Projects
Job spreadsheet
Notes
```

Kareer creates:

```text
                ME
                 │
        ┌────────┴────────┐
        ↓                 ↓
      PROFILE           GOAL
        │                 │
        ↓                 ↓
      SKILLS        TARGET ROLE
        │                 │
        ↓                 ↓
     EVIDENCE       SKILL GAPS
        │                 │
        └───────┬─────────┘
                ↓
             PROJECTS
                ↓
             ROADMAP
                ↓
            LEARNING
                ↓
          OPPORTUNITIES
                ↓
           APPLICATIONS
                ↓
            INTERVIEWS
                ↓
             PROGRESS
```

---

# 5. PRODUCT GOALS

Kareer should allow a student to:

1. Build a professional identity.
2. Record education and interests.
3. Track skills.
4. Attach evidence to skills.
5. Build and document projects.
6. Explore possible careers.
7. Compare career paths.
8. Select a target role.
9. Understand required skills.
10. Identify personal skill gaps.
11. Build a personalized roadmap.
12. Track learning.
13. Track DSA/problem solving.
14. Manage career-related tasks.
15. Track internships/jobs.
16. Track applications.
17. Track interviews.
18. Maintain resume information.
19. Analyze job descriptions.
20. Receive AI-assisted recommendations.
21. Measure career progress.

---

# 6. NON-GOALS

Kareer will NOT initially become:

- Social media
- Student-to-student messaging
- Full recruitment marketplace
- Full LMS
- Automated job application system
- Deterministic personality/career prediction system
- Salary/employment guarantee platform
- College management system
- Generic productivity/task-management application

The product must remain **personal-career focused**.

---

# 7. TARGET USER

## Primary

Students, especially:

- 12th-pass students exploring careers
- College CS/IT students
- Software development students
- Data Science students
- Data Analytics students
- Data Engineering students
- AI/ML students
- Cybersecurity students
- Cloud/DevOps students

## Initial Persona

```text
Student
   │
   ├── Doesn't know exact career direction
   ├── Has scattered skills/projects
   ├── Learns inconsistently
   ├── Doesn't know what to build
   ├── Doesn't know skill gaps
   ├── Wants internships/jobs
   └── Needs one system to organize everything
```

---

# 8. APPLICATION STRUCTURE

There is **no public section in the current version**.

There is also **no login/signup flow for now**.

When the application opens, it should **directly land on the student's personal dashboard**.

## Current Version

```text
Application Opens
       ↓
   MY DASHBOARD
       ↓
 ┌─────┼─────┬──────┬───────┐
 ↓     ↓     ↓      ↓       ↓
Profile Skills Projects Learning Career
 ↓     ↓     ↓      ↓       ↓
Resume Evidence DSA Roadmap Opportunities
                         ↓
                    Applications
                         ↓
                     Interviews
                         ↓
                     Analytics
                         ↓
                     AI Copilot
```

## Main Navigation

- Dashboard
- My Profile
- Skills
- Evidence
- Projects
- Learning
- DSA
- Career Direction
- Roadmap
- Tasks
- Opportunities
- Applications
- Interviews
- Resume
- Achievements
- Analytics
- AI Copilot
- Settings

## Future Authentication

Authentication is intentionally postponed.

Later:

```text
Login
 ↓
ID / Password
 ↓
Database
 ↓
My Personal Kareer
```

The current architecture should be kept modular enough that authentication can be added later without rebuilding the application.

---

# 9. DASHBOARD — THE CENTER OF KAREER

The dashboard is not simply an analytics screen.

It should answer:

> **"What is happening in my career right now?"**

## Dashboard

### Identity

- Profile
- Name
- Headline
- Education
- Target role
- Profile completeness

### Current state

- Career readiness
- Portfolio readiness
- Skill readiness
- Project progress
- Learning progress
- Interview readiness

### Today

- Today's tasks
- Learning goal
- DSA goal
- Project task
- Next action

### Career

- Target role
- Skill gaps
- Required skills
- Matching skills
- Recommended next action

### Projects

- Active projects
- Portfolio-ready projects
- Recently completed projects

### Opportunities

- Saved opportunities
- Applications
- Upcoming deadlines
- Interviews

### AI

- Career Copilot
- Recommended next action

---

# 10. STAGE-BY-STAGE IMPLEMENTATION PLAN

The project must be built **vertically**.

Do NOT build the entire frontend first and backend afterward.

Each stage should finish:

```text
Feature
 ↓
UI
 ↓
Data Model
 ↓
Data Logic
 ↓
Testing
 ↓
Definition of Done
```

The current version uses browser-local data. Backend/database synchronization can be introduced later when authentication is added.

---

# STAGE 0 — UNDERSTAND AND PREPARE

## Goal

Understand the existing application before modifying it.

If an existing repository is being transformed into Kareer, first identify the reusable frontend architecture.

## Steps

### 0.1 Create Git branch

```text
git checkout -b feature/kareer
```

### 0.2 Run existing application

Confirm:

- frontend works
- routing works
- existing pages work
- deployment works

Authentication/backend dependencies are not required for the current Kareer version.

### 0.3 Understand repository

Identify:

```text
HTML entry
↓
Router
↓
Views
↓
Services
↓
Browser data/storage
```

### 0.4 Identify reusable modules

Keep where useful:

- router
- reusable CSS
- utility functions
- UI components
- form handling
- validation
- responsive foundations
- deployment configuration

### 0.5 Identify insurance-specific code

Mark for removal:

- insurance terminology
- policy logic
- quote logic
- customer terminology
- insurance dashboard
- insurance database models
- insurance-specific forms

## Deliverables

```text
Architecture document
Feature map
Migration map
Data plan
UI plan
```

## Done when

You understand the current application well enough to modify it without accidentally destroying useful frontend infrastructure.

---

# STAGE 1 — KAREER VISUAL FOUNDATION

## Goal

Transform the existing application into the Kareer identity.

## Frontend restriction

Only:

```text
HTML5
CSS3
Vanilla JavaScript ES6+
```

No:

```text
React
Vue
Angular
Next.js
TypeScript
Tailwind
Bootstrap
```

## Build

### Branding

Replace the old domain branding with:

```text
Kareer
Personal Career OS
```

### Design system

Create:

```text
css/
├── variables.css
├── base.css
├── layout.css
├── components.css
├── pages.css
└── responsive.css
```

### Components

Build reusable:

- Navbar
- Sidebar
- Cards
- Buttons
- Inputs
- Selects
- Modals
- Skill chips
- Progress bars
- Progress rings
- Timeline
- Roadmap nodes
- Tables
- Tabs
- Badges
- Toasts
- Loading states
- Error states
- Empty states

## UI philosophy

Modern SaaS.

Information-rich but not cluttered.

The interface should feel like:

```text
Personal Developer Dashboard
+
Career Command Center
+
Portfolio
+
Learning System
```

---

# STAGE 2 — PERSONAL PROFILE

## Goal

Make the student the actual center of the application.

There is **no login/signup in this stage**.

The application assumes the current user is the owner.

## Initial flow

```text
Application opens
 ↓
Dashboard
 ↓
Profile
 ↓
Edit my information
 ↓
Return to Dashboard
```

## Profile

Store:

```text
userId
name
headline
bio
education
degree
branch
graduationYear
interests
targetRoles
github
linkedin
portfolio
profileCompleteness
createdAt
updatedAt
```

For the current version, this data is stored locally in the browser.

## Steps

1. Create personal profile data model.
2. Build profile page.
3. Build edit profile form.
4. Add education.
5. Add professional links.
6. Add interests.
7. Add target roles.
8. Calculate completeness.
9. Connect dashboard to profile data.
10. Persist data locally.

## Done when

Opening Kareer directly shows the student's own dashboard and profile information can be created/edited/persisted.

---

# STAGE 3 — SKILLS + EVIDENCE

## Goal

Move from:

> "I know Python."

to:

> "I know Python, and here is the evidence."

## Skill

```text
skillId
userId
name
category
currentLevel
targetLevel
status
createdAt
updatedAt
```

## Categories

- Programming
- Web
- Data
- AI/ML
- Databases
- Cloud
- DevOps
- Tools
- Soft Skills

## Evidence

Types:

- Project
- GitHub repository
- Certification
- Course
- DSA
- Competition
- Achievement
- Internship
- Other

## Relationship

```text
SKILL
 ↓
EVIDENCE
 ↓
PROJECT / CERTIFICATE / DSA / ACHIEVEMENT
```

## Build

1. Skill entity.
2. Skill CRUD.
3. Skill list.
4. Add skill modal.
5. Edit skill.
6. Delete skill.
7. Evidence entity.
8. Evidence CRUD.
9. Evidence form.
10. Connect evidence to skills.
11. Current level.
12. Target level.
13. Evidence coverage.

## Done when

Kareer can answer:

> **What skills do I claim, and what proves them?**

---

# STAGE 4 — PROJECTS

## Goal

Make projects first-class professional assets.

## Project

```text
projectId
userId
title
description
problem
techStack
skillIds
githubURL
liveURL
demoURL
screenshots
architectureNotes
resumeBullets
status
startDate
endDate
```

## Project lifecycle

```text
IDEA
 ↓
PLANNING
 ↓
BUILDING
 ↓
COMPLETED
 ↓
DOCUMENTED
 ↓
PORTFOLIO READY
```

## Build

1. Project entity.
2. Project CRUD.
3. Project list.
4. Project cards.
5. Project detail.
6. Tech stack.
7. Skill selector.
8. GitHub URL.
9. Live URL.
10. Demo URL.
11. Screenshots.
12. Architecture notes.
13. Resume bullets.
14. Portfolio-ready indicator.

## Relationship

```text
PROJECT
 ├── demonstrates → SKILL
 ├── creates → EVIDENCE
 ├── supports → TARGET ROLE
 └── contributes → RESUME
```

For the current frontend-only version, screenshots/assets can initially be referenced or handled locally rather than uploaded to a backend.

## Done when

A project can be turned into a documented portfolio asset.

---

# STAGE 5 — CAREER EXPLORER

## Goal

Help the student understand possible directions.

**Important:** Career Explorer is a supporting module, not the center of the product.

## Initial CS/Data/AI roles

```text
Software Engineer
Backend Engineer
Frontend Engineer
Mobile Developer
Data Analyst
Data Scientist
Data Engineer
Analytics Engineer
ML Engineer
AI Engineer
Cybersecurity
Cloud / DevOps
Systems
Research
BI Analyst
```

## Career record

```text
roleId
name
category
description
typicalWork
requiredSkills
preferredSkills
education
tools
mathematics
programming
exampleProjects
entryLevelRoles
roadmap
relatedRoles
sources
lastReviewed
```

## Career page

Show:

- What it is
- What professionals do
- Required skills
- Preferred skills
- Programming
- Mathematics
- Tools
- Education
- Example projects
- Entry roles
- Learning path
- Related roles
- Sources
- Last reviewed

## Build

1. Career catalog.
2. Career cards.
3. Search.
4. Filter.
5. Career detail.
6. CS explorer.
7. Data/AI explorer.
8. Career comparison.
9. Select target role.

## Done when

The student can understand and compare career options and choose a target.

---

# STAGE 6 — TARGET ROLE + SKILL GAP ENGINE

## Goal

Connect:

```text
ME
 ↓
MY SKILLS
 ↓
TARGET ROLE
 ↓
REQUIRED SKILLS
 ↓
GAPS
```

This is one of Kareer's most important intelligence layers.

## Example

Target:

```text
Data Scientist
```

Required:

```text
Python
SQL
Statistics
Pandas
NumPy
Machine Learning
Model Evaluation
```

Student:

```text
Python       4/5
SQL          3/5
Statistics   2/5
Pandas       3/5
ML           1/5
```

Kareer identifies:

```text
Strong:
Python

Partial:
SQL
Pandas

Critical gaps:
Statistics
Machine Learning
```

## Initial deterministic readiness

```text
readiness =
weighted(
    currentSkillLevel /
    requiredSkillLevel
)
```

Critical skills receive higher weights.

## Build

1. Create role-skill mappings.
2. Normalize skill names.
3. Compare user skills.
4. Find missing skills.
5. Find partial matches.
6. Identify critical gaps.
7. Check evidence.
8. Calculate readiness.
9. Display skill-gap visualization.
10. Recommend next actions.

## Skill graph

Example:

```text
Python
 ↓
NumPy / Pandas
 ↓
Data Analysis
 ↓
Statistics
 ↓
Machine Learning
 ↓
Model Evaluation
 ↓
Deployment
```

Another:

```text
SQL
 ↓
Databases
 ↓
ETL
 ↓
Data Pipelines
 ↓
Spark
 ↓
Cloud
```

## Done when

The student can clearly see:

```text
What I have
What I lack
Why it matters
What I should do
```

---

# STAGE 7 — ROADMAP + LEARNING

## Goal

Turn skill gaps into an executable plan.

## Flow

```text
TARGET ROLE
 ↓
REQUIRED SKILLS
 ↓
SKILL GAPS
 ↓
LEARNING SEQUENCE
 ↓
PROJECTS
 ↓
EXPERIENCE
 ↓
INTERNSHIP
 ↓
INTERVIEW
 ↓
JOB READINESS
```

## Roadmap

Include:

- Milestones
- Tasks
- Dependencies
- Target dates
- Priority
- Progress
- Resources
- Notes
- Projects

## Learning

Track:

- Courses
- Resources
- Notes
- Study goals
- Weekly goals
- Learning status

## Important rule

Kareer must NOT become another generic task manager.

A task exists because it supports:

```text
Career goal
Skill
Project
Roadmap
Application
Interview
```

## Example

```text
Target:
Backend Developer

Today's work:

45 min → DSA
60 min → API project
30 min → SQL
20 min → revision
```

## Done when

Selecting a target role produces a usable roadmap that the student can execute.

---

# STAGE 8 — DSA + PRODUCTIVITY

## DSA

Track:

```text
Problem
Platform
Topic
Difficulty
Status
Attempts
Notes
Date solved
Revision status
```

## Analytics

```text
Problems solved
Problems/week
Topic distribution
Difficulty distribution
Accuracy
Revision backlog
Weak topics
Streak
Progress over time
```

## Productivity

Build:

- Today
- Tasks
- Weekly plan
- Goals
- Habits
- Notes

But always connect them to the career roadmap.

---

# STAGE 9 — OPPORTUNITIES + APPLICATIONS

## Goal

Connect development to actual opportunities.

## Opportunity

```text
opportunityId
title
company
role
location
url
deadline
skills
source
savedAt
```

## Application

```text
applicationId
opportunityId
userId
status
appliedDate
resumeVersion
notes
nextAction
followUpDate
```

## Pipeline

```text
SAVED
 ↓
PREPARING
 ↓
APPLIED
 ↓
ASSESSMENT
 ↓
INTERVIEW
 ↓
OFFER
```

Alternative outcomes:

```text
REJECTED
WITHDRAWN
```

## Interview

```text
interviewId
applicationId
round
date
type
topics
result
notes
preparationStatus
```

## Build

1. Opportunity entity.
2. Opportunity form.
3. Saved opportunities.
4. Application entity.
5. Application board.
6. Application details.
7. Interview entity.
8. Interview tracker.
9. Deadlines.
10. Follow-ups.
11. Job-specific skill matching.

## Job matching

```text
JOB DESCRIPTION
 ↓
REQUIRED SKILLS
 ↓
MY SKILLS
 ↓
EVIDENCE
 ↓
MISSING SKILLS
 ↓
RECOMMENDED ACTION
```

## Done when

A student can manage an opportunity from:

```text
Found
→ Saved
→ Applied
→ Assessment
→ Interview
→ Result
```

---

# STAGE 10 — RESUME + PROFESSIONAL PRESENCE

## Goal

Turn Kareer's structured data into application material.

## Resume data

```text
Summary
Education
Skills
Projects
Experience
Certifications
Achievements
Links
```

## Resume versions

Examples:

```text
Software Engineer
Data Analyst
Data Scientist
ML Engineer
General
```

## Build

1. Resume data model.
2. Resume editor.
3. Resume versions.
4. Select target-role projects.
5. Select verified skills.
6. Select achievements.
7. Resume preview.
8. Later: export.
9. Later: AI wording.

## Critical rule

AI must never fabricate:

- Experience
- Projects
- Skills
- Metrics
- Achievements
- Employment

Resume content must originate from verified Kareer data.

---

# STAGE 11 — AI CAREER COPILOT

## Goal

Add AI **after** the structured Kareer system works.

AI is not the source of truth.

```text
STRUCTURED DATA
       ↓
      AI
       ↓
PERSONALIZED ACTION
```

## AI V1 — Career Copilot

Capabilities:

- Career questions
- Career explanations
- Career comparison
- Skill explanations
- Roadmap explanations

## AI V2 — Personalized Planning

- Generate roadmap
- Break goals into tasks
- Recommend next skill
- Adapt roadmap
- Recommend projects

## AI V3 — Career Intelligence

- Skill-gap analysis
- Job matching
- Resume-job matching
- Readiness analysis
- Application recommendations

## AI V4 — Interview Coach

- Technical questions
- Behavioral questions
- Follow-up questions
- Answer evaluation
- Weak-topic detection
- Preparation recommendations

## Current-version note

AI should initially be treated as a future integration layer. Do not block the core Kareer product on AI.

The frontend should call a future AI service through a clean service abstraction rather than embedding provider-specific logic throughout the UI.

---

# 12. AI ARCHITECTURE

The frontend remains pure HTML/CSS/Vanilla JS.

Current version:

```text
HTML
 CSS
 JS
  │
  ↓
AI Service Abstraction
  │
  ↓
Future AI Provider
  │
  ↓
Structured Response
  │
  ↓
Frontend
```

The exact AI provider/backend architecture can be added later.

---

# 13. AI GROUNDING RULES

Kareer must distinguish:

```text
VERIFIED USER DATA
        ↓
STRUCTURED CAREER DATA
        ↓
GENERAL GUIDANCE
        ↓
PERSONALIZED RECOMMENDATION
```

AI cannot invent portfolio evidence.

For example, if Kareer contains:

```text
Python
SQL
2 projects
```

AI cannot say:

```text
You have 2 years of Python experience.
```

unless that information actually exists.

AI should explain:

```text
You currently demonstrate Python through these projects...
```

---

# STAGE 12 — PERSONAL ANALYTICS

## Goal

Make growth measurable.

## Portfolio metrics

- Profile completeness
- Projects completed
- Portfolio-ready projects
- Evidence coverage

## Skill metrics

- Skills acquired
- Current levels
- Target levels
- Skill gaps
- Evidence-backed skills

## Learning

- Tasks completed
- Courses
- Roadmap progress
- Weekly consistency
- Learning time

## DSA

- Problems solved
- Topics
- Difficulty
- Weak areas

## Career

- Target role
- Readiness
- Skill gap count
- Project alignment

## Applications

- Saved opportunities
- Applications
- Interviews
- Outcomes
- Conversion rates

---

# 14. READINESS MODEL

Every score must be explainable.

Example dashboard:

```text
Portfolio Readiness       78%
Skill Readiness           64%
Project Evidence          82%
Learning Progress         71%
Interview Readiness       52%
────────────────────────────
Overall Career Progress   68%
```

Never show a score without explaining how it was calculated.

---

# STAGE 13 — DATA / ANALYTICS / AI SHOWCASE

This stage makes Kareer itself demonstrate technical ability.

## Career map

```text
Data Analyst
Data Scientist
Data Engineer
ML Engineer
AI Engineer
Analytics Engineer
BI Analyst
Research
```

## Same dataset, different roles

```text
SAME DATASET
     │
     ├── Data Analyst
     │      → Reporting
     │      → Dashboards
     │      → Business insights
     │
     ├── Data Scientist
     │      → Statistics
     │      → Prediction
     │      → Modeling
     │
     ├── Data Engineer
     │      → Pipelines
     │      → Storage
     │      → Processing
     │
     └── ML Engineer
            → Model systems
            → Deployment
            → Production
```

This demonstrates that Kareer is not merely a CRUD application.

---

# 15. PROJECT COMPLEXITY LADDER

Use Kareer to demonstrate increasing technical complexity.

```text
LEVEL 1
Basic project

LEVEL 2
CRUD application

LEVEL 3
API + Database

LEVEL 4
Data pipeline

LEVEL 5
ML model

LEVEL 6
Production deployment

LEVEL 7
End-to-end system
```

The project recommendation engine can use:

```text
Target role
+
Current skills
+
Missing skills
+
Existing projects
+
Project complexity
=
Recommended next project
```

---

# STAGE 14 — POLISH + PRODUCTION

## Frontend

Check:

- Responsive layout
- Mobile
- Tablet
- Desktop
- Accessibility
- Loading states
- Error states
- Empty states
- Form validation
- Navigation
- Performance

## Local data

Check:

- Persistence
- Data initialization
- Data migration/versioning
- Reset capability
- Export capability
- Import capability

## Future backend readiness

Ensure the application separates:

```text
UI
 ↓
Service layer
 ↓
Data source
```

so the current browser-local data source can later be replaced by a database without rewriting every page.

---

# 16. DATABASE / DATA MODEL

## Current Version

There is **no backend database yet**.

Use browser-local storage as the temporary persistence layer.

Suggested abstraction:

```text
UI
 ↓
data/service layer
 ↓
localStorage
```

Later:

```text
UI
 ↓
data/service layer
 ↓
API
 ↓
database
```

## User/Profile

```text
User
├── userId
├── name
├── headline
├── bio
├── education
├── branch
├── graduationYear
├── interests
├── targetRoles
├── github
├── linkedin
├── portfolio
├── profileCompleteness
├── createdAt
└── updatedAt
```

## Skill

```text
Skill
├── skillId
├── userId
├── name
├── category
├── currentLevel
├── targetLevel
├── status
├── createdAt
└── updatedAt
```

## Evidence

```text
Evidence
├── evidenceId
├── userId
├── type
├── title
├── url
├── description
├── date
├── relatedSkillIds
└── relatedProjectIds
```

## Project

```text
Project
├── projectId
├── userId
├── title
├── description
├── problem
├── techStack
├── skillIds
├── githubURL
├── liveURL
├── demoURL
├── screenshots
├── architectureNotes
├── resumeBullets
├── status
├── startDate
└── endDate
```

## Career Role

```text
Career
├── roleId
├── name
├── category
├── description
├── typicalWork
├── requiredSkills
├── preferredSkills
├── education
├── tools
├── relatedRoles
├── exampleProjects
├── roadmap
├── sourceLinks
└── lastReviewed
```

## Roadmap

```text
Roadmap
├── roadmapId
├── userId
├── targetRoleId
├── milestones
├── tasks
├── targetSkills
├── progress
├── startDate
└── targetDate
```

## Opportunity

```text
Opportunity
├── opportunityId
├── title
├── company
├── role
├── location
├── url
├── deadline
├── skills
├── source
└── savedAt
```

## Application

```text
Application
├── applicationId
├── opportunityId
├── userId
├── status
├── appliedDate
├── resumeVersion
├── notes
├── nextAction
└── followUpDate
```

## Interview

```text
Interview
├── interviewId
├── applicationId
├── round
├── date
├── type
├── topics
├── result
├── notes
└── preparationStatus
```

---

# 17. DATA SERVICE ARCHITECTURE

Because there is no database in the current version, do not directly call localStorage from every page.

Create one data layer.

Example:

```text
js/
├── data/
│   ├── store.js
│   ├── profile-store.js
│   ├── skills-store.js
│   ├── projects-store.js
│   └── roadmap-store.js
```

The UI talks to:

```text
ProfileService
SkillService
ProjectService
RoadmapService
```

Those services currently talk to:

```text
LocalStorage
```

Later they can talk to:

```text
Database API
```

without changing the UI architecture significantly.

---

# 18. FRONTEND ARCHITECTURE

Strictly:

```text
HTML5
CSS3
Vanilla JavaScript ES6+
```

## Suggested structure

```text
kareer/
│
├── index.html
│
├── assets/
│   ├── images/
│   └── icons/
│
├── css/
│   ├── variables.css
│   ├── base.css
│   ├── layout.css
│   ├── components.css
│   ├── pages.css
│   └── responsive.css
│
├── js/
│   ├── app.js
│   ├── router.js
│   ├── state.js
│   │
│   ├── views/
│   │   ├── dashboard.js
│   │   ├── profile.js
│   │   ├── skills.js
│   │   ├── evidence.js
│   │   ├── projects.js
│   │   ├── learning.js
│   │   ├── dsa.js
│   │   ├── careers.js
│   │   ├── roadmap.js
│   │   ├── opportunities.js
│   │   ├── applications.js
│   │   ├── interviews.js
│   │   ├── resume.js
│   │   ├── analytics.js
│   │   └── ai.js
│   │
│   ├── components/
│   │   ├── navbar.js
│   │   ├── sidebar.js
│   │   ├── card.js
│   │   ├── modal.js
│   │   ├── progress.js
│   │   ├── skill-card.js
│   │   ├── project-card.js
│   │   ├── roadmap.js
│   │   └── empty-state.js
│   │
│   ├── services/
│   │   ├── profile.js
│   │   ├── skills.js
│   │   ├── evidence.js
│   │   ├── projects.js
│   │   ├── careers.js
│   │   ├── roadmap.js
│   │   ├── opportunities.js
│   │   └── ai.js
│   │
│   ├── data/
│   │   ├── store.js
│   │   └── career-catalog.js
│   │
│   └── utils/
│       ├── validation.js
│       ├── formatting.js
│       └── calculations.js
│
└── docs/
    ├── architecture.md
    ├── data-model.md
    └── implementation.md
```

---

# 19. CURRENT DATA FLOW

```text
index.html
     ↓
app.js
     ↓
router.js
     ↓
dashboard.js
     ↓
service layer
     ↓
localStorage
```

Example:

```text
User edits profile
       ↓
Profile View
       ↓
Profile Service
       ↓
Local Storage
       ↓
Dashboard refresh
```

---

# 20. FUTURE DATA FLOW

When login/database is eventually added:

```text
index.html
     ↓
app.js
     ↓
router.js
     ↓
View
     ↓
Service Layer
     ↓
API
     ↓
Database
```

Authentication can then be inserted above the protected application layer:

```text
Login
 ↓
Authentication
 ↓
User identity
 ↓
Kareer Dashboard
```

The current frontend should not be tightly coupled to this future architecture.

---

# 21. SECURITY — CURRENT VERSION

Because there is no login or backend currently:

The current version should focus on:

- Avoiding sensitive data collection.
- Safe DOM rendering.
- Input validation.
- Avoiding unsafe HTML injection.
- Keeping application data local.
- Avoiding hardcoded future API secrets.
- Separating future service/API logic from UI.

When authentication/backend is introduced later, add:

- Authentication
- Authorization
- Server-side validation
- Secure sessions
- Database access controls
- Rate limiting
- Secure API keys
- Audit logging
- Data deletion/export
- AI security controls

---

# 22. TESTING STRATEGY

Testing happens at every stage.

## Frontend

Test:

- Navigation
- Forms
- Validation
- CRUD interactions
- Responsive layout
- Loading
- Errors
- Empty states
- Local persistence

## Data

Test:

- Create
- Read
- Update
- Delete
- Refresh persistence
- Invalid records
- Missing records
- Data reset
- Data export/import when implemented

## AI

Test later:

- Hallucination
- Missing data
- Contradictory data
- Long job descriptions
- Prompt injection
- Fabrication prevention
- Structured output

---

# 23. CRITICAL END-TO-END TEST

The most important test is:

```text
OPEN KAREER
 ↓
MY DASHBOARD
 ↓
PROFILE
 ↓
SKILL
 ↓
EVIDENCE
 ↓
PROJECT
 ↓
TARGET ROLE
 ↓
SKILL GAP
 ↓
ROADMAP
 ↓
LEARNING / DSA
 ↓
OPPORTUNITY
 ↓
APPLICATION
 ↓
INTERVIEW
 ↓
DASHBOARD
 ↓
PROGRESS
```

If this journey works, Kareer's core concept works.

---

# 24. EXACT BUILD ORDER

Build in this order:

```text
01. Understand existing application

02. Create Kareer branch

03. Remove old/insurance theme

04. Create Kareer branding

05. Create design system

06. Build application shell

07. Build navigation

08. Make application open directly on Dashboard

09. Create local data/store abstraction

10. Build personal profile

11. Build education

12. Build professional links

13. Build profile completeness

14. Build Skills CRUD

15. Build Evidence CRUD

16. Connect Evidence → Skills

17. Build Projects CRUD

18. Connect Projects → Skills

19. Build Career database

20. Build Career Explorer

21. Build CS/Data/AI Explorer

22. Build Career Comparison

23. Add Target Role

24. Build Role → Skill mapping

25. Build Skill Gap engine

26. Build Skill Dependency Graph

27. Build Roadmap

28. Build Tasks

29. Build Learning tracker

30. Build DSA tracker

31. Connect progress to Dashboard

32. Build Opportunities

33. Build Application Pipeline

34. Build Interview Tracker

35. Build Job Skill Matching

36. Build Resume data

37. Build Resume versions

38. Build Resume preview

39. Build Analytics

40. Create AI service abstraction

41. Integrate AI Career Copilot later

42. Add AI Skill Gap later

43. Add AI Project Recommendation later

44. Add JD Analysis later

45. Add Interview Coach later

46. Security/data review

47. E2E testing

48. Responsive polish

49. Performance optimization

50. Production deployment

51. Add authentication in a future phase

52. Replace local data with database in a future phase
```

---

# 25. MVP — DO NOT BUILD EVERYTHING

The first strong version should focus on the core loop.

## MVP CORE

### Personal

- Profile
- Education
- Skills
- Evidence
- Projects

### Career

- Career Explorer
- CS/Data/AI Explorer
- Career Comparison
- Target Role
- Required Skills
- Skill Gap

### Development

- Roadmap
- Tasks
- Learning
- DSA

### Opportunities

- Internship/job tracker
- Applications
- Interviews

### Dashboard

Everything summarized in one place.

### AI

AI should initially be optional/future-facing.

The first working MVP does not need to depend on AI.

---

# 26. FEATURES TO DELAY

Do NOT start with:

- Login
- Signup
- Database backend
- Social networking
- Mentor marketplace
- Recruiter platform
- Automated job applications
- Advanced ML recommendation models
- Complex vector database
- Full LMS
- Massive job aggregation
- Advanced notifications
- Mobile app

Build the personal career loop first.

---

# 27. FUTURE EXPANSION

After the core system is stable:

```text
Authentication
 ↓
ID / Password
 ↓
Database
 ↓
Multi-device persistence
 ↓
GitHub integration
 ↓
Repository analysis
 ↓
Contribution analytics
 ↓
Public portfolio
 ↓
Shareable profile
 ↓
Public project pages
 ↓
Advanced job matching
 ↓
Opportunity aggregation
 ↓
AI mock interviews
 ↓
AI architecture review
 ↓
Automated evidence extraction
 ↓
Advanced analytics
 ↓
ML recommendation ranking
```

---

# 28. DEVELOPMENT PHASES

## Phase 1 — Foundation

Build:

- Branding
- Design system
- SPA shell
- Navigation
- Direct dashboard entry
- Local data layer

---

## Phase 2 — Personal Portfolio

Build:

- Profile
- Education
- Skills
- Evidence
- Projects

---

## Phase 3 — Career Intelligence

Build:

- Career Explorer
- CS Explorer
- Career comparison
- Target role
- Required skills
- Skill gaps

---

## Phase 4 — Development System

Build:

- Roadmap
- Tasks
- Learning
- DSA
- Progress

---

## Phase 5 — Opportunities

Build:

- Opportunities
- Applications
- Interviews
- Resume

---

## Phase 6 — Analytics + AI

Build:

- Analytics
- Career Copilot
- Skill-gap AI
- Project recommendations
- JD analysis
- Interview coach

---

## Phase 7 — Future Backend

Only after the frontend product is stable:

- Login
- ID/password
- User accounts
- Database
- API
- Multi-device synchronization
- Server-side AI
- Backend security

---

# 29. CAREER DATA STRATEGY

Start small.

```text
30–50 major careers
+
10–15 CS/Data/AI specializations
+
structured skills
+
role mappings
+
roadmaps
```

Career information should be structured rather than generated randomly by AI.

Dynamic factual information such as:

- salary
- demand
- employment outlook

must have:

```text
Source
Source date
Review date
```

---

# 30. KAREER'S DIFFERENTIATOR

A normal career website:

```text
Take quiz
 ↓
You should become Data Scientist
```

Kareer:

```text
ME
 ↓
Understand myself
 ↓
Explore options
 ↓
Compare options
 ↓
Choose target
 ↓
Analyze my current skills
 ↓
Find gaps
 ↓
Build roadmap
 ↓
Learn
 ↓
Build projects
 ↓
Create evidence
 ↓
Find opportunities
 ↓
Apply
 ↓
Prepare
 ↓
Interview
 ↓
Measure progress
 ↓
Improve
```

**That is the product.**

---

# 31. FINAL SUCCESS CRITERION

Kareer is successful when one student can open the application and understand:

### Who am I?

```text
Profile
Education
Interests
Skills
Experience
Projects
Achievements
```

### Where am I going?

```text
Target Role
Career Direction
Required Skills
```

### What am I missing?

```text
Skill Gaps
Missing Evidence
Weak Areas
```

### What should I do?

```text
Roadmap
Tasks
Learning
Projects
DSA
```

### What opportunities are available?

```text
Jobs
Internships
Applications
Interviews
```

### How am I progressing?

```text
Skills
Projects
Learning
Applications
Readiness
Career Progress
```

### What should I do next?

```text
AI + deterministic recommendation engine
```

---

# 32. FINAL PRODUCT LOOP

```text
                         ┌──────────┐
                         │    ME    │
                         └────┬─────┘
                              ↓
                         ┌──────────┐
                         │ PROFILE  │
                         └────┬─────┘
                              ↓
                         ┌──────────┐
                         │  SKILLS  │
                         └────┬─────┘
                              ↓
                        ┌───────────┐
                        │  EVIDENCE │
                        └─────┬─────┘
                              ↓
                        ┌───────────┐
                        │ PROJECTS  │
                        └─────┬─────┘
                              ↓
                       ┌────────────┐
                       │ TARGET ROLE│
                       └──────┬─────┘
                              ↓
                       ┌────────────┐
                       │ SKILL GAPS │
                       └──────┬─────┘
                              ↓
                        ┌───────────┐
                        │ ROADMAP   │
                        └─────┬─────┘
                              ↓
                       ┌────────────┐
                       │  LEARNING  │
                       └──────┬─────┘
                              ↓
                       ┌────────────┐
                       │ PROJECTS   │
                       └──────┬─────┘
                              ↓
                      ┌──────────────┐
                      │ OPPORTUNITIES│
                      └──────┬───────┘
                             ↓
                      ┌─────────────┐
                      │ APPLICATIONS│
                      └──────┬──────┘
                             ↓
                      ┌─────────────┐
                      │ INTERVIEWS  │
                      └──────┬──────┘
                             ↓
                       ┌───────────┐
                       │ PROGRESS  │
                       └─────┬─────┘
                             │
                             └──────────→ ME
```

# FINAL PRINCIPLE

**Kareer is not a website that tells me what career I should choose.**

**Kareer is the system that helps me understand myself professionally, choose a direction, build proof of my abilities, develop toward a target role, turn that development into opportunities, and continuously improve.**

Every feature must answer one of these:

> **Who am I?**

> **What can I do?**

> **What proves it?**

> **Where am I going?**

> **What am I missing?**

> **What should I build?**

> **What should I learn?**

> **What should I do today?**

> **Which opportunities fit me?**

> **How am I progressing?**

If a feature does not strengthen this loop, it should not be prioritized.

## Current Technical Principle

For the first version:

```text
HTML5
+
CSS3
+
Vanilla JavaScript
+
Local Browser Storage
+
Structured Local Data
=
Kareer
```

No login.

No database.

No backend.

No cloud dependency.

The application opens directly into **my personal dashboard**.

Later, authentication and database persistence can be added behind the existing service/data abstraction.
