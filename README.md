# My Dev Notes

**Java Backend & Native Android Engineering Knowledge Base**

A growing collection of technical notes, practical code examples, software architecture concepts, debugging techniques, and engineering best practices.

This repository focuses on **Java, Spring Boot, PostgreSQL, Gradle, Maven, and native Android development with Java**, covering the fundamentals and advanced engineering practices needed to build maintainable, testable, secure, and reliable software.

The purpose is to go beyond learning individual technologies and develop a deeper understanding of software design, engineering trade-offs, performance, security, testing, and production readiness.

---

## Table of Contents

- [1. Computer Science & Engineering Fundamentals](#1-computer-science--engineering-fundamentals)
- [2. Java & JVM](#2-java--jvm)
- [3. Spring Boot & Backend Development](#3-spring-boot--backend-development)
- [4. PostgreSQL & Database Engineering](#4-postgresql--database-engineering)
- [5. Native Android Development](#5-native-android-development)
- [6. Gradle, Maven & Build Engineering](#6-gradle-maven--build-engineering)
- [7. Software Architecture & Design](#7-software-architecture--design)
- [8. Testing & Code Quality](#8-testing--code-quality)
- [9. Security Engineering](#9-security-engineering)
- [10. Performance, Reliability & Observability](#10-performance-reliability--observability)
- [11. Networking & Distributed Systems](#11-networking--distributed-systems)
- [12. CI/CD & Developer Tools](#12-cicd--developer-tools)
- [13. Senior Engineering Practices](#13-senior-engineering-practices)
- [14. Practical Engineering Exercises](#14-practical-engineering-exercises)
- [Repository Structure](#repository-structure)
- [Learning Roadmap](#learning-roadmap)
- [Related Projects](#related-projects)
- [References](#references)

---

## 1. Computer Science & Engineering Fundamentals

### Data Structures & Algorithms
- Arrays, linked lists, stacks, queues, and hash tables
- Trees, heaps, graphs, and priority queues
- Searching, sorting, and common algorithmic techniques
- Time and space complexity using Big O notation
- Choosing appropriate data structures
- Problem decomposition and algorithm selection

### Operating Systems & Memory
- Processes, threads, scheduling, and synchronization
- Stack, heap, memory allocation, and resource management
- Race conditions, deadlocks, and thread safety
- File systems, sockets, and operating-system fundamentals

### Networking Fundamentals
- TCP/IP and UDP
- DNS, TLS, and HTTPS
- HTTP methods, status codes, headers, and caching
- Proxies, reverse proxies, and load balancing
- Latency, timeouts, and network failure modes

### Engineering Fundamentals
- Programming paradigms and object-oriented programming
- Abstraction, encapsulation, and modularity
- State management and immutability
- Error handling and resource lifecycle
- Reading unfamiliar code and debugging systematically

---

## 2. Java & JVM

### Core Java
- Classes, interfaces, inheritance, and composition
- Encapsulation, polymorphism, and abstraction
- Collections Framework and data structure selection
- Generics, enums, records, and nested types
- Exception handling and resource management
- `equals()`, `hashCode()`, and object contracts
- Lambdas, functional interfaces, and the Stream API
- Optional and modern date/time APIs
- Immutable objects and defensive copying
- Clean code, naming, and API design

### Advanced Java
- Concurrency, multithreading, and thread safety
- Threads, executors, and thread pools
- Synchronization, locks, and atomic variables
- `Future` and `CompletableFuture`
- Concurrent collections
- Java Memory Model and happens-before relationships
- Race conditions, deadlocks, and visibility problems
- Reflection, annotations, and dynamic proxies
- Generic type erasure
- Virtual threads and their appropriate use cases

### JVM Internals
- Class loading and bytecode fundamentals
- Heap, stack, metaspace, and object allocation
- Garbage collection and object reachability
- Memory leaks and object-retention analysis
- Heap dumps and thread dumps
- JVM profiling and diagnostic tools
- Runtime performance analysis
- JVM tuning fundamentals

### Java Engineering Practices
- Choosing appropriate data structures
- Designing reusable and maintainable APIs
- Managing exceptions at the correct boundary
- Refactoring complex methods
- Identifying unnecessary object creation
- Evaluating readability, complexity, and performance
- Understanding Java version compatibility

---

## 3. Spring Boot & Backend Development

### Spring Framework Fundamentals
- Inversion of Control and Dependency Injection
- Spring ApplicationContext and bean lifecycle
- Component scanning and configuration
- Bean scopes and lifecycle callbacks
- Profiles and externalized configuration
- Spring Boot starters and auto-configuration
- Conditional configuration
- Application startup and configuration troubleshooting
- Dependency management and Spring Boot compatibility

### REST API Engineering
- REST principles and resource modeling
- HTTP methods, status codes, headers, and content types
- Request and response DTOs
- Input validation and consistent error responses
- Pagination, sorting, and filtering
- API versioning and backward compatibility
- OpenAPI and Swagger documentation
- Idempotency and safe retry behavior
- CORS and request-size limits
- Consistent API naming and response conventions
- API contract design and evolution

### Backend Application Architecture
- Controller, service, and repository responsibilities
- Entities, DTOs, domain models, and mapping
- Business logic and domain boundaries
- Layered architecture and separation of concerns
- Dependency inversion
- Transaction boundaries and business invariants
- Reusable services and component design
- Avoiding duplicated logic and unnecessary abstractions
- Managing application configuration
- Designing code for testability and maintainability

### Spring Data JPA & Hibernate
- Entity lifecycle and persistence context
- Entity relationships and mapping strategies
- Lazy and eager fetching
- N+1 query problems
- JPQL, native SQL, and projections
- Pagination and sorting
- Cascades and orphan removal
- Entity equality and identifier strategies
- Transaction propagation and isolation
- Optimistic and pessimistic locking
- Persistence exceptions and rollback behavior
- Generated SQL and query performance
- Managing schema changes safely

### Spring Security
- Authentication versus authorization
- Security filter chain
- Password hashing and credential handling
- JWT creation, validation, expiration, and claims
- Access-token and refresh-token strategies
- Role-based and resource-based authorization
- Method-level security
- Public and protected endpoints
- Token revocation and logout considerations
- Authorization boundaries and security testing
- Secure configuration and least privilege

### Backend Integrations
- External REST API clients
- Connection, read, and request timeouts
- Retry policies, exponential backoff, and jitter
- Circuit breakers and bulkheads
- Email and file-storage integrations
- Asynchronous processing
- Scheduled jobs and background tasks
- Event-driven communication and messaging
- Caching and cache invalidation
- Handling external dependency failures
- Idempotent processing and duplicate requests

### Production-Ready Spring Boot
- Centralized exception handling
- Validation and consistent response models
- Structured logging and correlation IDs
- Spring Boot Actuator
- Health, readiness, and liveness checks
- Application metrics and tracing
- Configuration and secret management
- Database migrations with Flyway or Liquibase
- Graceful shutdown and resource cleanup
- Dependency vulnerability management
- Deployment profiles and production configuration
- Troubleshooting application startup and runtime failures

---

## 4. PostgreSQL & Database Engineering

### SQL Fundamentals
- SELECT, INSERT, UPDATE, and DELETE
- Joins, subqueries, and common table expressions
- Aggregations, GROUP BY, and HAVING
- Primary keys, foreign keys, and unique constraints
- Check constraints and referential integrity
- Normalization and relational data modeling
- Views and database functions
- SQL injection prevention
- Query readability and maintainability

### PostgreSQL
- PostgreSQL data types and schema design
- Primary-key and identifier strategies
- Indexes and index selection
- Composite, partial, and unique indexes
- Query planning with `EXPLAIN` and `EXPLAIN ANALYZE`
- Query optimization and execution plans
- Transactions and isolation levels
- Locking and concurrent updates
- Connection pooling and resource limits
- Database migrations and schema evolution
- Backup, restore, and recovery fundamentals
- Database roles and access permissions

### Database Design
- One-to-one, one-to-many, and many-to-many relationships
- Modeling business rules and invariants
- Cascading operations and referential integrity
- Audit fields and timestamps
- Soft deletion and retention policies
- Designing schemas for booking and ordering systems
- Preventing inconsistent states
- Data validation at application and database levels
- Choosing appropriate constraints and indexes

### JPA/Hibernate with PostgreSQL
- Mapping Java entities to relational tables
- Understanding the SQL generated by Hibernate
- Detecting unnecessary database queries
- Selecting appropriate fetching strategies
- Pagination with large datasets
- Transaction boundaries across service methods
- Optimistic locking and lost-update prevention
- Entity lifecycle versus database lifecycle
- Database migration and backward compatibility
- Diagnosing slow queries

### Other Data Technologies
- SQLite and Room for Android local persistence
- Firebase and Firestore where appropriate
- Relational versus document databases
- Redis and common caching scenarios
- Choosing storage based on access patterns and consistency needs

---

## 5. Native Android Development

### Android Platform Fundamentals
- Activities and fragments
- Activity and fragment lifecycles
- Configuration changes and process recreation
- State restoration and saved state
- Intents and deep links
- Permissions and runtime permission handling
- Services and background execution
- WorkManager and deferrable work
- Android application components
- Android version compatibility and API levels

### UI Development with Java & XML
- XML layouts and reusable UI components
- ViewBinding
- RecyclerView and adapters
- Material Design components
- Responsive layouts and different screen sizes
- Form validation and UI state
- Loading, empty, error, and offline states
- Accessibility and content descriptions
- Localization and right-to-left layouts
- Efficient rendering and UI responsiveness

### Android Architecture
- Model-View-ViewModel (MVVM)
- Repository pattern
- Separation of UI and business logic
- ViewModel and lifecycle-aware components
- State management and one-way data flow
- Dependency injection fundamentals
- Modularization and feature boundaries
- Managing UI state across configuration changes
- Testable application design
- Avoiding unnecessary architectural complexity

### Networking & REST API Integration
- HTTP and REST API fundamentals
- Retrofit and OkHttp
- Request and response models
- Authentication headers and token refresh
- Timeouts, retries, and network failures
- Error mapping and user-friendly messages
- Pagination and large-list loading
- Image loading and caching
- Handling expired sessions
- Synchronization with backend state

### Local Data & Offline Support
- SQLite and Room
- Entities, DAOs, and database relationships
- Room migrations
- Local caching and invalidation
- Repository coordination between remote and local data
- Offline-first architecture fundamentals
- Synchronization and conflict resolution
- WorkManager for deferred background operations
- Consistency between local and remote data
- Secure local persistence

### Concurrency & Lifecycle
- Main-thread responsibilities
- Executors and background processing
- Handler and Looper fundamentals
- Thread safety and synchronization
- Lifecycle-aware cancellation
- Avoiding blocking operations on the main thread
- Handling background-task failures
- Resource cleanup and lifecycle management

### Android Performance
- Application startup performance
- ANRs and main-thread blocking
- Memory leaks
- Android Profiler and heap analysis
- RecyclerView performance
- Image loading and memory usage
- Network and battery efficiency
- StrictMode
- Rendering and frame performance
- Profiling before optimizing

### Android Security & Release Engineering
- Android Keystore concepts
- Secure token and credential storage
- Network security configuration
- Exported components and intent validation
- Deep-link security
- WebView security considerations
- Sensitive data in logs and backups
- Permission minimization
- Build variants and release signing
- R8 and code shrinking
- Release verification and crash monitoring

---

## 6. Gradle, Maven & Build Engineering

### Gradle
- Gradle build lifecycle
- Tasks and task dependencies
- Plugins and build configuration
- Dependency configurations
- Version catalogs
- Gradle Wrapper
- Multi-module project structure
- Android build types and product flavors
- Dependency resolution and conflict handling
- Build caching and incremental builds
- Build performance optimization
- Troubleshooting failed builds
- Java toolchains and compatibility

### Maven
- Maven lifecycle, phases, and goals
- POM structure and project coordinates
- Dependencies and transitive dependencies
- Dependency scopes
- Plugins and plugin configuration
- Parent POMs and dependency management
- Multi-module Maven projects
- Maven Wrapper
- Reproducible builds
- Dependency convergence and version conflicts
- Test and packaging configuration
- Build troubleshooting

### Build & Dependency Engineering
- Gradle versus Maven: use cases and trade-offs
- Dependency version management
- Managing Java and Android plugin compatibility
- Java language versions and toolchains
- Environment-specific build configuration
- Reproducible builds and dependency locking
- Artifact versioning and release management
- Dependency vulnerability scanning
- CI integration and build troubleshooting
- Separating build configuration from application configuration

---

## 7. Software Architecture & Design

### Engineering Principles
- SOLID principles
- DRY, KISS, and YAGNI
- Composition over inheritance
- Separation of concerns
- High cohesion and low coupling
- Encapsulation and information hiding
- Dependency inversion
- Explicit contracts and clear boundaries

### Design Patterns
- Strategy
- Factory and Builder
- Adapter and Decorator
- Observer
- Proxy
- Dependency Injection
- Repository pattern
- Event-driven patterns
- Recognizing when patterns introduce unnecessary complexity

### Architectural Approaches
- Layered architecture
- Clean Architecture
- Hexagonal Architecture and ports and adapters
- Modular monoliths
- Microservices and service boundaries
- Domain-driven design fundamentals
- Domain models and business invariants
- Architecture Decision Records
- Evolutionary architecture and technical debt

### Architecture Trade-offs
- Maintainability versus complexity
- Modularity versus unnecessary abstraction
- Monolith versus microservices
- Synchronous versus asynchronous communication
- Compatibility versus rapid change
- Cost, reliability, scalability, and operational effort
- Designing for testing and future change

---

## 8. Testing & Code Quality

### Testing Fundamentals
- Unit, integration, contract, and end-to-end tests
- Test isolation and deterministic behavior
- Test fixtures and test data
- Boundary-value and negative-case testing
- Mocking, stubs, and fakes
- The test pyramid and feedback cycles
- Avoiding brittle tests
- Regression testing and reproducibility

### Backend Testing
- JUnit 5
- Mockito
- Service and business-logic tests
- Repository integration tests
- Spring application-context tests
- REST API tests
- Security and authorization tests
- Database integration with Testcontainers
- Transaction and concurrency testing
- External-service failure testing

### Android Testing
- Unit tests for ViewModels and business logic
- Repository and data-source tests
- Instrumented tests
- UI tests with Espresso
- Lifecycle and state-restoration tests
- Network-error and offline testing
- Dependency substitution and test doubles
- Testing application behavior across different states

### Code Quality
- Readability and naming
- Refactoring techniques
- Static analysis and formatting
- Complexity and maintainability
- Code-review checklists
- Regression prevention
- Meaningful test coverage
- Quality gates and automated checks
- Reviewing correctness rather than only style

---

## 9. Security Engineering

### Security Fundamentals
- Least privilege
- Defense in depth
- Threat modeling and trust boundaries
- Secure defaults
- Input validation
- Secret management
- Dependency vulnerability management
- Privacy and data minimization

### Backend Security
- OWASP Top 10
- OWASP API Security risks
- Broken access control and IDOR
- SQL injection
- Authentication and token lifecycle risks
- CSRF, CORS, SSRF, and security headers
- Password hashing
- Mass assignment and excessive data exposure
- Secure error handling and logging
- Authorization testing

### Android Security
- Secure local storage
- Network traffic protection
- Deep-link and intent validation
- Exported-component security
- WebView security
- Sensitive data in logs and backups
- Permission minimization
- Debug versus release configuration
- Secure handling of credentials and tokens

Security notes should document the threat, impact, mitigation, and verification tests.

---

## 10. Performance, Reliability & Observability

### Performance Engineering
- Establishing performance baselines
- CPU, memory, database, and network profiling
- Latency percentiles and throughput
- Identifying bottlenecks before optimizing
- Caching and invalidation
- Database query optimization
- Connection-pool configuration
- Android startup and rendering performance
- Memory and resource management

### Reliability Engineering
- Timeouts and bounded retries
- Exponential backoff and jitter
- Idempotency
- Circuit breakers and bulkheads
- Rate limiting
- Graceful degradation
- Resource limits
- Failure isolation and recovery
- Handling partial failures

### Observability
- Structured logs
- Metrics and distributed tracing
- Correlation IDs
- Health checks
- Actionable alerts
- Crash reporting
- Service-level indicators and objectives
- Evidence-based debugging
- Incident investigation and prevention

---

## 11. Networking & Distributed Systems

### Networking Fundamentals
- TCP/IP and UDP
- DNS and TLS
- HTTP and HTTPS
- Connection and read timeouts
- Proxies and reverse proxies
- Load balancing
- Latency and network failure modes

### Distributed Systems
- Synchronous versus asynchronous communication
- Messaging and event-driven architecture
- Duplicate delivery and idempotent consumers
- Retries and dead-letter queues
- Eventual consistency
- Distributed transactions
- Saga pattern
- Transactional outbox
- Service boundaries
- Distributed tracing

### System Design
- Functional and non-functional requirements
- Capacity estimation
- Availability and latency
- Scaling up versus scaling out
- Caching and load balancing
- Database and API design
- Failure modes and recovery
- Cost and operational complexity
- Documenting alternatives and trade-offs

---

## 12. CI/CD & Developer Tools

### Git & Collaboration
- Branching and commit conventions
- Pull requests and code reviews
- Merge conflicts and history management
- Reverts and recovery
- Tags and releases
- Useful commit messages

### CI/CD
- Automated builds and tests
- Static analysis and quality gates
- Artifact creation and versioning
- Environment-specific configuration
- Deployment strategies
- Rollback plans
- Post-deployment verification

### Containers & Infrastructure
- Docker fundamentals
- Images, containers, and networking
- Environment variables and secrets
- Persistent data
- Basic Kubernetes concepts where relevant
- Cloud deployment fundamentals
- Infrastructure and operating costs

### Developer Tools
- IntelliJ IDEA
- Android Studio
- Debuggers and profilers
- Terminal and shell fundamentals
- Maven and Gradle commands
- Database clients and query tools
- API clients
- Build and dependency troubleshooting

---

## 13. Senior Engineering Practices

### Technical Ownership
- Clarifying requirements before implementation
- Breaking down complex features
- Identifying dependencies and risks
- Owning features from design through release
- Monitoring outcomes and preventing regressions
- Considering maintainability and operational needs

### Technical Decision-Making
- Evaluating alternatives and trade-offs
- Avoiding premature optimization
- Balancing delivery speed and long-term quality
- Documenting assumptions and decisions
- Recognizing unnecessary complexity
- Revisiting decisions when evidence changes

### Production Troubleshooting
- Reproducing and isolating failures
- Analyzing logs, metrics, traces, and crash reports
- Distinguishing symptoms from root causes
- Investigating recent changes and dependencies
- Building minimal reproductions
- Writing regression tests
- Documenting incidents and preventive actions

### Code Review & Collaboration
- Reviewing correctness, security, performance, and maintainability
- Giving constructive and specific feedback
- Explaining technical reasoning
- Sharing knowledge and context
- Helping teammates improve
- Aligning implementation with team conventions

### Engineering Communication
- Writing technical documentation
- Communicating risks and blockers early
- Explaining trade-offs clearly
- Estimating work with explicit assumptions
- Discussing technical debt and its consequences
- Collaborating with product, QA, design, and operations

### Sustainable Engineering
- Incremental refactoring
- Dependency and platform upgrades
- Compatibility and deprecation planning
- Reducing recurring production problems
- Learning from incidents and code reviews
- Measuring improvements instead of relying on intuition

---

## 14. Practical Engineering Exercises

### Spring Boot & PostgreSQL
- Build a REST API with validation and centralized error handling.
- Implement a transactional business use case.
- Add pagination, filtering, and appropriate database indexes.
- Investigate and resolve an N+1 query issue.
- Write authorization tests for protected resources.
- Test database migrations against existing data.
- Add timeout and retry policies to an external API client.
- Add structured logging and health checks.
- Investigate a slow SQL query using an execution plan.

### Gradle & Maven
- Create a reproducible build using the appropriate wrapper.
- Investigate and resolve a dependency conflict.
- Configure unit and integration tests.
- Explore a multi-module build.
- Document a failed build and its resolution.
- Evaluate a dependency upgrade for compatibility and security.

### Native Android
- Implement loading, empty, error, and offline states.
- Add Room persistence and a migration.
- Test ViewModel and repository behavior.
- Handle process recreation and saved state.
- Diagnose a memory leak or ANR.
- Implement pagination and reliable network-error handling.
- Test deep links and sensitive-data handling.
- Profile startup performance before and after an optimization.

### Senior-Level Exercises
- Write an Architecture Decision Record.
- Design a system and explain its trade-offs.
- Perform a security and maintainability review.
- Reproduce a defect and add a regression test.
- Create a release and rollback checklist.
- Document an incident and its preventive actions.
- Compare two approaches and explain why one is more appropriate.
- Record assumptions, limitations, and remaining technical risks.

---

## Repository Structure

The intended organization is:

```text
My-Dev-Notes/
├── 01-Engineering-Fundamentals/
├── 02-Java-JVM/
├── 03-Spring-Boot-Backend/
├── 04-PostgreSQL-Databases/
├── 05-Native-Android-Java/
├── 06-Gradle-Maven-Builds/
├── 07-Architecture-Design/
├── 08-Testing-Code-Quality/
├── 09-Security/
├── 10-Performance-Reliability/
├── 11-Networking-Distributed-Systems/
├── 12-CICD-Developer-Tools/
├── 13-Senior-Engineering/
├── 14-Practical-Exercises/
└── README.md
```

Directories should be created as useful notes are added, rather than leaving the repository filled with empty folders.

### Suggested Note Format

For substantial topics, document the following where appropriate:

1. **Concept:** What is it, and what problem does it solve?
2. **Mechanics:** How does it work?
3. **Example:** A minimal, understandable implementation.
4. **Use cases:** When is this approach appropriate?
5. **Alternatives:** What other solutions exist?
6. **Trade-offs:** What complexity or limitations does it introduce?
7. **Failure modes:** What can go wrong?
8. **Testing:** How can the behavior be verified?
9. **References:** Link to official documentation or reliable technical sources.

For personal tracking, distinguish between topics explored, examples implemented, and approaches validated in a real project.

---

## Learning Roadmap

### Stage 1 — Strong Foundations
- Java fundamentals, collections, exceptions, and object-oriented design
- HTTP, REST, SQL, and relational data modeling
- Spring dependency injection and REST controllers
- Android lifecycle and UI fundamentals
- Git, Gradle, Maven, and automated testing basics

### Stage 2 — Independent Feature Development
- Spring Boot services, JPA, PostgreSQL, and transactions
- Authentication, authorization, validation, and error handling
- Android architecture, networking, and Room
- Unit and integration testing
- Debugging and maintainable code organization

### Stage 3 — Production Engineering
- Query optimization and database migrations
- Security reviews and dependency updates
- Performance profiling and observability
- CI/CD, deployment, and rollback
- Reliability, retries, and failure recovery
- Android memory, startup, and rendering performance

### Stage 4 — Senior Engineering
- Architecture and system-design trade-offs
- Technical ownership and production troubleshooting
- Maintainability and technical-debt management
- Design reviews and constructive code reviews
- Incident prevention and operational responsibility
- Clear technical communication and mentorship

Progress should be measured through demonstrated understanding, practical application, and engineering judgment—not simply the number of technologies listed.

---

## Related Projects

These projects provide practical context for studying the technologies covered in this repository.

- [BookNest](https://github.com/Melikash98/BookNest) — Java and Spring Boot backend for a hotel reservation platform.
- [BrewBite Admin](https://github.com/Melikash98/BrewBite-Admin) — Backend API for café and bakery administration.
- **Fanjano** — Café-platform project using Java, Spring Boot, and PostgreSQL.
- [PLAVIO](https://github.com/Melikash98/PLAVIO) — Native Android property and accommodation application project.
- [Haus-Suche](https://github.com/Melikash98/Haus-Suche) — Android application for finding homes and accommodation.
- [MorphNavBar](https://github.com/Melikash98/MorphNavBar) — Custom animated Android navigation component.
- [Editify](https://github.com/Melikash98/Editify) — Custom Android input component with animated hints and validation states.

Project descriptions should reflect the actual implementation and current status of each repository.

---

## References

### Java & Backend
- [Dev.java — Learn Java](https://dev.java/learn/)
- [Java Documentation](https://docs.oracle.com/en/java/)
- [Spring Framework Reference](https://docs.spring.io/spring-framework/reference/)
- [Spring Boot Documentation](https://docs.spring.io/spring-boot/index.html)
- [Spring Security Reference](https://docs.spring.io/spring-security/reference/)
- [Spring Data JPA Reference](https://docs.spring.io/spring-data/jpa/reference/)
- [PostgreSQL Documentation](https://www.postgresql.org/docs/)
- [Maven Documentation](https://maven.apache.org/guides/)
- [Gradle Documentation](https://docs.gradle.org/current/userguide/userguide.html)

### Android
- [Android Developers](https://developer.android.com/)
- [Android Architecture](https://developer.android.com/topic/architecture)
- [Android Testing](https://developer.android.com/training/testing)
- [Android Performance](https://developer.android.com/topic/performance)

### Testing, Security & Operations
- [JUnit 5 User Guide](https://junit.org/junit5/docs/current/user-guide/)
- [Mockito](https://site.mockito.org/)
- [OWASP Top 10](https://owasp.org/www-project-top-ten/)
- [OWASP API Security](https://owasp.org/www-project-api-security/)
- [Docker Documentation](https://docs.docker.com/)
- [OpenTelemetry Documentation](https://opentelemetry.io/docs/)

---

## Purpose

This repository is a long-term technical reference for learning, experimentation, and continuous improvement across **Java backend engineering and native Android development**.

The focus is on understanding fundamentals, applying sound engineering practices, evaluating trade-offs, and building software that is maintainable, testable, secure, and reliable.

**Maintained by [Melika Shooryabi](https://github.com/Melikash98).**
