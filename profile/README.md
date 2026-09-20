# SANGU Software Engineering

This GitHub organization is the home for software engineering course materials and programming examples for **SANGU University** computer science students. The **13-week course** combines engineering principles with programming: understanding requirements, designing software, implementing and testing it, collaborating through Git, and delivering and maintaining a working application.

Topics build on one another. Students learn to express behaviour before testing it, establish tests before refactoring, and understand runtime environments before automating deployment. UML and Mermaid help connect requirements, design decisions, and code throughout the course.

## Learning outcomes

By the end of the course, students should be able to:

- Translate stakeholder needs into clear requirements, acceptance criteria, and behavioural contracts.
- Select a development process, plan small increments, estimate effort, and manage risks and changes.
- Collaborate using Git, GitHub, pull requests, issue tracking, and constructive code review.
- Implement modular software using functions, classes, interfaces, and appropriate design principles.
- Read and create focused UML diagrams, and maintain Mermaid diagrams alongside code.
- Write meaningful tests, investigate defects, and refactor without changing intended behaviour.
- Evaluate architecture against reliability, availability, scalability, security, and maintainability requirements.
- Use Docker, Compose, and GitHub Actions to build reproducible environments and automate delivery.
- Diagnose operational failures and maintain software using logs, monitoring, tests, and documentation.
- Apply professional responsibility to privacy, accessibility, open-source reuse, and AI-assisted development.

## Prerequisites and course format

Students should have completed a course in a high-level programming language or object-oriented programming and have **B1 English** for reading technical materials. They should understand variables, control flow, functions, and basic collections. Week 1 refreshes programming foundations; classes and interfaces are revisited before object-oriented design in week 5.

The course carries **6 ECTS** and a **150-hour workload**, including 13 lecture hours and 26 laboratory hours. Teaching combines explanations, live programming demonstrations, and hands-on practice in a language students already know. Examples progress from small functions to collaborating modules and a deployable application.

The agenda below lists **lecture topics only**. Laboratory instructions, assignments, and assessment arrangements are provided separately. Git begins in week 2; later topics use tools and concepts introduced earlier in the sequence.

## What is software engineering?

Software engineering applies systematic methods to building and evolving software under real constraints. Programming is a central part of that work, alongside understanding users, making design decisions, verifying behaviour, collaborating, and keeping software useful after release.

| Area | Main question | Purpose |
| --- | --- | --- |
| **Requirements and planning** | What should we build, and how should we organise the work? | Establish user needs, constraints, priorities, and manageable increments. |
| **Design and construction** | How should the software be structured and implemented? | Create understandable code with clear responsibilities and interfaces. |
| **Verification and improvement** | Does it behave correctly, and can we change it safely? | Find defects, test assumptions, review changes, and improve maintainability. |
| **Delivery and operation** | How do we release, observe, and maintain it? | Make execution reproducible, automate delivery, and respond to failures. |

These activities recur as software evolves. A changed requirement may affect the design, code, tests, deployment configuration, and documentation.

## 13-week agenda

| Week | Theme | Lecture topics |
| --- | --- | --- |
| **1** | **Software engineering and programming foundations** | Software engineering and its relationship to programming. The lifecycle from understanding a problem to maintenance. Scope, cost, schedule, quality, and change. Functions, parameters, return values, collections, and control flow. Readable code, meaningful names, formatting, and separation of responsibilities. Professional ethics and responsibility for AI-assisted work. |
| **2** | **Version control and collaborative development** | Working directory, staging, commits, and history. Local Git operations before remotes, cloning, pushing, and pulling. Branches, merging, and conflict resolution. GitHub repositories, pull requests, code review, and issue tracking. Markdown, README files, and useful code comments. |
| **3** | **Requirements and workflow modelling** | Stakeholders, elicitation, functional and non-functional requirements, prioritisation, and specifications. User stories, acceptance criteria, preconditions, and postconditions. UML use case and activity diagrams. Mermaid syntax, `flowchart`, Markdown code fences, and rendering diagrams on GitHub. Distinguish UML activity notation from general flowcharts. |
| **4** | **Development processes and project planning** | Code-and-fix, waterfall, prototyping, and iterative and incremental development. Agile principles, Scrum, and Kanban. Backlogs, task decomposition, estimation uncertainty, dependencies, scope changes, risks, and progress monitoring. Team responsibilities and criteria for completed work. |
| **5** | **Modular programming and object-oriented design** | Functional decomposition, information hiding, cohesion, coupling, and separation of concerns. Objects, classes, constructors, encapsulation, and interfaces. Composition versus inheritance and selected SOLID principles. UML class relationships and multiplicities; Mermaid `classDiagram`. Connecting a model to its implementation. |
| **6** | **Behaviour, testing, and debugging** | Contracts, verification and validation, assertions, test cases, and unit tests. Normal and error cases, equivalence partitions, and boundaries. UML state machines and Mermaid `stateDiagram-v2`; tests for valid and invalid transitions. Errors, exceptions, reproduction steps, breakpoints, stack traces, and regression tests. Introduction to integration and acceptance testing. |
| **7** | **Code quality, safe refactoring, and CI** | Code smells, duplication, technical debt, complexity, and maintainability metrics. Refactoring supported by tests; TDD and its red–green–refactor cycle. Black-box and white-box testing, coverage limitations, formatters, and linters. Build and dependency-management basics. Continuous integration with GitHub Actions workflows, triggers, jobs, and steps. |
| **8** | **Architecture and component interactions** | Architecture versus detailed design. Layers, a modular monolith, interfaces, and dependency boundaries. UML component and sequence diagrams; Mermaid `sequenceDiagram`. Integration and acceptance tests, test doubles, and mocking tradeoffs. Reliability, availability, scalability, maintainability, timeouts, bounded retries, and architecture decision records. |
| **9** | **Secure and responsible software construction** | Assets, trust boundaries, and threats. Authentication and authorisation, validation, safe data access, least privilege, secrets, and dependency risks. Security-focused negative tests. Privacy, data minimisation, accessibility, licences, and attribution. Reviewing and independently verifying AI-generated code. |
| **10** | **Runtime environments, Docker, and deployment modelling** | Source code, artifacts, processes, runtime environments, and configuration. Containers, images, Dockerfiles, builds, registries, Docker Hub, and versioning. Ports, networking, volumes, and secret handling. Docker Compose. UML deployment diagrams and Mermaid infrastructure flowcharts connecting components to runtime environments. |
| **11** | **DevOps, delivery pipelines, and documentation publishing** | Development and operations responsibilities. Continuous integration, delivery, and deployment. Container builds, versioned artifacts, release tags, environments, quality gates, smoke tests, and rollback with GitHub Actions. Publishing Mermaid diagrams on GitHub Pages and other web platforms using configured rendering or image exports. |
| **12** | **Logging, observability, and maintenance** | Log levels, destinations, formatting, and structured records. Logs, metrics, traces, health checks, latency, errors, and alerts. Operational diagnosis, sensitive-data protection, incident response, rollback, and blameless review. Regression testing, dependency updates, compatibility, technical debt, and keeping diagrams and documentation current. |
| **13** | **Integrated review and engineering decisions** | Connect the lifecycle through a complete software example. Review UML views and appropriate Mermaid use. Trace a changed requirement through models, implementation, tests, delivery, and operational documentation. Compare alternatives using evidence and constraints; consolidate the course without introducing new tools. |

### Why this sequence?

Programming foundations support Git collaboration and code review. Markdown and GitHub come before Mermaid publishing. Requirements establish the behaviour that planning, design, and tests must address. Classes and interfaces precede class-level testing; tests and debugging precede refactoring and CI.

Architecture then connects modules into a system and gives security analysis concrete boundaries. Runtime environments and containers precede delivery automation. Logging and maintenance build on a system students can already understand, test, and release. The final week connects the entire process through changes and engineering tradeoffs.

### Week 1 foundation checklist

Week 1 establishes the vocabulary and programming baseline used throughout the course.

- **Engineering context:** users, requirements, lifecycle activities, quality, constraints, and change.
- **Programming essentials:** functions, inputs and outputs, collections, conditionals, and loops.
- **Code readability:** naming, formatting, small responsibilities, and understandable control flow.
- **Professional responsibility:** explain your work, acknowledge assistance, and verify claims and generated code.

Git is introduced in week 2, UML and Mermaid in week 3, and automated testing in week 6.

## UML and Mermaid coverage

Select a diagram according to the question it answers. Keep models small enough to read and specific enough to compare with the implementation.

| View | Engineering question | First taught |
| --- | --- | --- |
| **UML use case** | Who uses the system, and for which goals? | Week 3 |
| **UML activity** | How does a workflow proceed and branch? | Week 3 |
| **UML class** | What responsibilities and relationships exist between types? | Week 5 |
| **UML state machine** | Which lifecycle transitions are valid? | Week 6 |
| **UML component** | What are the main parts and their interfaces? | Week 8 |
| **UML sequence** | How do collaborators complete a scenario? | Week 8 |
| **UML deployment** | Where do artifacts execute, and how do environments connect? | Week 10 |

Mermaid coverage progresses through `flowchart` (week 3), `classDiagram` (week 5), `stateDiagram-v2` (week 6), and `sequenceDiagram` (week 8), followed by infrastructure views and web publishing. UML is a modelling language; Mermaid is an authoring and rendering tool. General Mermaid flowcharts can illustrate workflows and infrastructure without claiming to use formal UML activity or deployment notation.

GitHub renders supported Mermaid syntax in Markdown code fences labelled `mermaid`. Preview diagrams on the target platform and check its renderer version. A GitHub Pages site needs its own Mermaid integration or exported images; repository Markdown support does not automatically configure a website. See the [GitHub diagram documentation](https://docs.github.com/en/get-started/writing-on-github/working-with-advanced-formatting/creating-diagrams) and [Mermaid user guide](https://mermaid.js.org/intro/getting-started.html).

## Learning approach

Programming examples use a familiar application domain so students can focus on engineering decisions. Working code, tests, diagrams, and documentation should describe the same behaviour. Each new technique should solve an identifiable problem, and students should be able to explain its benefits, costs, and alternatives.

Practical work accompanies the lectures through separate laboratory materials. Those materials should introduce no required tool before its lecture and should favour small, understandable changes over large amounts of framework setup. Individual understanding remains essential when students collaborate or use AI tools.

## Course resources

The [SANGU Software Engineering organization](https://github.com/sangu-software-engineering) is the home for course repositories. This profile presents the lecture agenda. The [course website repository](https://github.com/sangu-software-engineering/sangu-software-engineering.github.io) is available for developing the course website and publishing supporting materials.

- **Core textbook:** Pankaj Jalote, [A Concise Introduction to Software Engineering: With Open Source and GenAI](https://link.springer.com/book/10.1007/978-3-031-74318-4), second edition, 2025.
- **Git:** [Pro Git](https://git-scm.com/book/en/v2).
- **Software construction:** [MIT 6.102 materials, Spring 2026](https://web.mit.edu/6.102/www/sp26/).
- **Agile development:** [The Scrum Guide](https://scrumguides.org/scrum-guide.html).
- **Diagrams:** [Mermaid documentation](https://mermaid.js.org/intro/getting-started.html).
- **Containers:** [Docker getting-started documentation](https://docs.docker.com/get-started/).
- **Automation:** [GitHub Actions documentation](https://docs.github.com/en/actions).
- **Application security:** [OWASP Top 10](https://owasp.org/projects/top-ten).

The agenda draws on the SANGU syllabus and comparisons with recent courses at [MIT](https://web.mit.edu/6.102/www/sp26/), [UC Berkeley](https://cs169.org/fa26/syllabus/), [NUS](https://nus-cs2103-ay2526s1.github.io/website/), [Edinburgh](https://opencourse.inf.ed.ac.uk/inf2-sepp/schedule), and [UNSW](https://cgi.cse.unsw.edu.au/~cs1531/25T1/dashboard). The scope and sequence are adapted to this course's 13 teaching weeks.
