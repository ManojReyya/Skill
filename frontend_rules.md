🧠 Core Principles

ALWAYS write clean, readable, and maintainable UI code.
FOLLOW separation of concerns (UI, logic, state).
KEEP components small and reusable.
AVOID unnecessary complexity.
DO NOT duplicate UI logic (DRY).
BUILD for scalability and readability.


🧩 Component Design Rules


Each component MUST have a single responsibility.


PREFER functional components over class components.


KEEP components:

Small
Reusable
Testable



SPLIT large components into smaller ones.


AVOID deeply nested component trees.



⚙️ State Management Rules

USE local state for simple UI logic.
USE global state ONLY when necessary.

Preferred Tools

useState → simple state
useReducer → complex state logic
Context API → shared state (limited scope)
Redux / Zustand → large applications


🔄 Data Flow Rules

FOLLOW unidirectional data flow.
PASS data via props (parent → child).
AVOID prop drilling:

Use context or state management when needed.




🔌 API & Data Fetching


NEVER call APIs directly inside UI rendering.


USE:

useEffect (React)
or data-fetching libraries (React Query / SWR)



ALWAYS:

Handle loading state
Handle error state
Handle empty state




🎨 UI & Styling Rules

KEEP UI consistent and clean.
FOLLOW design system (if available).
USE:

Tailwind / CSS Modules / Styled Components



Styling Rules

AVOID inline styles (except dynamic cases)
USE reusable style classes
KEEP responsiveness in mind


📱 Responsiveness


UI MUST be responsive across:

Mobile
Tablet
Desktop



USE:

Flexbox / Grid
Media queries




⚡ Performance Rules

AVOID unnecessary re-renders.

USE:


React.memo


useMemo


useCallback


LAZY load components when needed.


OPTIMIZE large lists (virtualization if needed).



🧪 Error Handling & UX


ALWAYS show:

Loading indicators
Error messages
Empty states



NEVER leave blank or crashing UI.



🔐 Frontend Security

NEVER store sensitive data in frontend.
AVOID exposing API keys.
SANITIZE user input.
PREVENT XSS attacks.
USE secure cookies or tokens for auth.


🧱 Routing Rules

USE proper routing (React Router / framework routing).
PROTECT routes:

Authenticated routes MUST be guarded.




📦 Project Structure
Example structure:
/components
/pages
/hooks
/services (API calls)
/utils
/styles


KEEP structure consistent.
SEPARATE logic and UI.


🔄 Forms Handling

USE controlled components.
VALIDATE all user input.

Preferred Tools:

React Hook Form
Formik


🧪 Testing Rules


WRITE tests for:

Components
Critical UI flows



USE:

Jest
React Testing Library




📊 Accessibility (IMPORTANT)

USE semantic HTML.
SUPPORT keyboard navigation.
ADD aria attributes where needed.
ENSURE contrast and readability.


🚀 Build & Deployment

OPTIMIZE build size.
MINIFY assets.
USE lazy loading.


❌ Anti-Patterns (STRICT)

Large monolithic components ❌
Inline API calls in UI ❌
Hardcoded values ❌
Uncontrolled side effects ❌
Ignoring loading/error states ❌


✅ AI Behavior Guidelines

ALWAYS create reusable components.
ALWAYS handle loading, error, and empty states.
NEVER mix UI and business logic.
ALWAYS optimize re-renders.
ALWAYS ensure responsive design.
PREFER clean and simple solutions over complex ones.


⚡ Optional (Advanced Frontend)
📈 Advanced Concepts

Server-side rendering (SSR)
Static site generation (SSG)
Code splitting
Micro-frontends (advanced)
State normalization
