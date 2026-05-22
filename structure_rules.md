# structure_rules.md

## Core Rule (Highest Priority)

- BEFORE creating ANY new file:
  1. Read all rule files:
     - backend_rules.md
     - frontend_rules.md
     - dsa.md
     - docs_rules.md
  2. Understand project structure
  3. Apply architecture rules
  4. THEN write code

- NEVER skip this step
- Structure MUST come before implementation


## File Creation Rules

- Each file MUST have:
  - Single responsibility
  - Clear purpose
  - Minimal scope

- NEVER create large or multi-purpose files
- NEVER mix concerns:
  - UI + business logic
  - Data + logic
  - Multiple domains


## Structure Over Code

- PRIORITY = Structure > Code

- AI MUST:
  - Create proper folders before writing logic
  - Define clear module boundaries
  - Split features into components/services

GOOD:
  /user
    UserController.cs
    UserService.cs
    IUserService.cs
    UserRepository.cs

BAD:
  UserManager.cs (everything inside)


## File Size Rules

- Each file MUST be:
  - Small
  - Focused
  - Easy to read

- Avoid files larger than 300–400 lines
- Split logic when file grows


## Modular Design Rules

- Use:
  - Interfaces
  - Services
  - Utilities
  - Helpers

- Prefer:
  - Composition over monolithic design


## Reusability Rules

- NEVER duplicate logic
- Create reusable functions/services
- Share common code across modules


## Naming Rules

- File names MUST clearly describe purpose

GOOD:
  UserService.cs
  AuthController.cs
  PaymentRepository.cs

AVOID:
  Manager.cs
  Helper.cs


## Dependency Rules

- MUST follow Dependency Injection
- Use abstractions (interfaces)
- Avoid tight coupling


## Commenting Rules

### General
- ALWAYS add comments for:
  - Complex logic
  - Business rules
  - Non-obvious decisions

- KEEP comments concise and meaningful
- Explain WHY, not just WHAT


### What to Comment
- Business logic decisions
- Edge case handling
- Optimization reasoning


### What NOT to Comment
- Obvious/simple code
- Self-explanatory lines

BAD:
  // increment i
  i++


### Good Examples

// Validate user before saving to prevent invalid data
if (user == null) throw new Exception("Invalid user");


// Using cache to reduce DB load
var user = _cache.Get(userId);


## File Header Comments

Each file MUST start with:

// Purpose: What this file does
// Responsibility: Scope of this file
// Layer: Controller / Service / Repository / etc


Example:

// Purpose: Handles authentication logic
// Responsibility: Manages login and token generation
// Layer: Service


## Method Comments

Each method SHOULD include:

// Purpose: What the method does

Example:

// Purpose: Creates a new user after validation
public void CreateUser(User user)


## Complex Logic Comments

If logic is complex, explain steps:

// Step 1: Filter active users
// Step 2: Sort by last login
// Step 3: Take top 10


## Anti-Patterns (Strictly Forbidden)

- Large "God files"
- Multiple responsibilities in one file
- No comments in complex logic
- Over-commenting trivial code
- Creating files without reading rules


## AI Behavior Guidelines

- ALWAYS design structure FIRST, then code
- ALWAYS keep files small and modular
- ALWAYS include meaningful comments
- NEVER mix layers or responsibilities
- ALWAYS think: "Can this be split further?"


## Master Rule

AI MUST:
- Read all rules before creating files
- Prioritize structure over code
- Keep files small and focused
- Include meaningful comments explaining logic and decisions
