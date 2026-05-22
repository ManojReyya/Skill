🧠 Core Engineering Principles
SOLID

S: Each class MUST have a single responsibility.
O: Code MUST be open for extension, closed for modification.
L: Derived classes MUST NOT break base class behavior.
I: Interfaces MUST be small and specific.
D: Depend on abstractions, NOT concrete implementations.

General Principles

DRY: Avoid code duplication.
KISS: Prefer simple solutions over complex ones.
YAGNI: Do NOT implement features unless required.
SoC: Separate concerns across layers and modules.


🧱 Design Patterns

Repository: Abstract data access logic.
Unit of Work: Manage transactions across repositories.
Dependency Injection: Use built-in DI container.
Factory: Use for object creation logic.
Singleton: Use for shared global instances (carefully).
Strategy: Encapsulate interchangeable behaviors.
Mediator (MediatR): Decouple request handling.
Builder: Construct complex objects step-by-step.


🏗️ Architecture Rules

Use layered architecture:

Controller → Service → Repository → Database


Follow Clean Architecture:

API layer MUST NOT contain business logic
Business logic MUST be isolated


Domain logic MUST be independent of frameworks
Avoid tight coupling between layers
Use interfaces between layers

Advanced (Optional)

Microservices for scalability
Domain-Driven Design (DDD) for complex domains


🔐 Security Rules

Use JWT or OAuth for authentication.
Implement role-based or policy-based authorization.
NEVER store plain text passwords; ALWAYS hash.
Enforce HTTPS in all environments.
Validate ALL incoming input.
Prevent SQL Injection using ORM or parameterized queries.
Protect against:

XSS
CSRF


Do NOT expose sensitive data in APIs.
Store secrets in environment variables or secure vaults.


⚙️ Backend Fundamentals

Follow REST API standards.
Use proper HTTP methods:

GET, POST, PUT, DELETE


Return correct HTTP status codes.
Use middleware for cross-cutting concerns.
Validate models using annotations or validators.
Use JSON for data exchange.
Use Dependency Injection consistently.


🗄️ Database & Data Rules

Use Entity Framework Core.
Use LINQ for queries.
Apply migrations properly.
Define relationships:

One-to-One
One-to-Many
Many-to-Many


Use indexing where needed.
Use transactions for critical operations.
Implement caching when needed (Redis / MemoryCache).


🚀 Performance Rules

Use async/await for I/O operations.
Implement pagination for large datasets.
Avoid loading unnecessary data.
Optimize database queries.
Use caching to reduce load.
Use connection pooling.


🧪 Testing Rules

Write unit tests for business logic.
Use xUnit or NUnit.
Use mocking frameworks (e.g., Moq).
Write integration tests for APIs.
Ensure code is testable (loose coupling).


📊 Logging & Monitoring

Use ILogger for logging.
Log errors and important events.
Use structured logging.
Handle exceptions globally.
Monitor application health.


🔄 Development Practices

Follow clean code practices.
Use meaningful naming conventions.
Conduct code reviews.
Use Git for version control.
Implement CI/CD pipelines.
Maintain separate configs for:

Development
Testing
Production




☁️ Deployment Rules

Use Kestrel/IIS for hosting.
Containerize using Docker (recommended).
Deploy to cloud platforms (e.g., Azure).
Automate deployments where possible.
Monitor deployed applications.


🧩 Advanced Concepts

Use message queues (RabbitMQ / Kafka).
Implement background jobs (Hangfire).
Use SignalR for real-time communication.
Apply distributed system principles.
Implement rate limiting to protect APIs.


✅ AI Behavior Guidelines

ALWAYS prioritize clean and maintainable code.
ALWAYS follow SOLID and architecture rules.
NEVER mix business logic with controllers.
NEVER expose sensitive or internal details.
ALWAYS validate input and handle errors properly.
PREFER abstraction and loose coupling.
OPTIMIZE only when necessary, not prematurely.
