🧠 Core Rule

AI MUST read and follow project documents before writing code.
Code MUST align with documented requirements.
NEVER assume requirements without checking documents.


📘 PRD (Product Requirements Document)
Purpose
Defines what to build and why
AI Rules

ALWAYS extract:

Features
User requirements
Business goals


DO NOT add extra features not mentioned
IMPLEMENT only what PRD specifies
CLARIFY unclear requirements (or make safe assumptions)


📐 DD (Design Document)
Purpose
Defines high-level architecture and system design
AI Rules

FOLLOW architecture strictly (layers, services, flow)
DO NOT violate design decisions
RESPECT:

Module boundaries
Service responsibilities


USE defined technologies


🛠️ TD (Technical Design Document)
Purpose
Defines implementation details
AI Rules

IMPLEMENT:

APIs as specified
Data models as defined
Logic as described


DO NOT change:

Contracts (API format)
Database schema
Naming conventions


FOLLOW coding standards mentioned


📝 TODO.md
Purpose
Tracks tasks and progress
AI Rules

ALWAYS:

Pick next pending task
Mark task as complete after implementation


DO NOT skip tasks
DO NOT implement out of order unless required


🔄 Workflow Rules
AI MUST follow this order:

Read PRD → understand requirements
Read DD → understand architecture
Read TD → understand implementation
Read TODO → pick task
Implement task
Update TODO


⚠️ Consistency Rules


Code MUST match:

PRD (features)
DD (structure)
TD (implementation)



If conflict occurs:

PRIORITY:

TD
DD
PRD






✅ AI Behavior Guidelines

NEVER write random code without context
ALWAYS align with project documents
ALWAYS maintain consistency across files
PREFER documented decisions over assumptions
KEEP implementation traceable to requirements


⚡ Suggested File Structure
/docs
  ├── PRD.md
  ├── DD.md
  ├── TD.md
  ├── TODO.md
  ├── docs_rules.md

/rules
  ├── backend_rules.md
  ├── frontend_rules.md
  ├── dsa.md


✅ Final Insight (Very Important)
👉 Without docs → AI behaves like a coder
👉 With docs → AI behaves like a software engineer
This is exactly how real teams work:

Product → PRD
Architects → DD
Engineers → TD + TODO
