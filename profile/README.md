# SANGU Software Engineering

This GitHub organization is the home for software engineering course materials and programming examples for **SANGU University** computer science students. The **13-week course** combines engineering principles with programming: understanding requirements, designing software, implementing and testing it, collaborating through Git, and delivering and maintaining a working application.

Topics build on one another. Students learn to express behaviour before testing it, establish tests before refactoring, and understand runtime environments before automating deployment. UML and Mermaid help connect requirements, design decisions, and code throughout the course.

## Learning outcomes

By the end of the course, students should be able to:

- Translate stakeholder needs into clear requirements, acceptance criteria, and behavioural contracts.
- Select a development process, plan small increments, estimate effort, and manage risks and changes.
- Collaborate using Git, GitHub, pull requests, issue tracking, and constructive code review.
- Build a Java project with Maven, explain dependency resolution and artifacts, and compare Gradle and npm, recognising Yarn as an alternative package manager.
- Implement modular software using functions, classes, interfaces, and appropriate design principles.
- Read and create focused UML diagrams, and maintain Mermaid diagrams alongside code.
- Write meaningful tests, investigate defects, and refactor without changing intended behaviour.
- Evaluate architecture against reliability, availability, scalability, security, and maintainability requirements.
- Use Docker, Compose, and GitHub Actions to build reproducible environments and automate delivery.
- Diagnose operational failures and maintain software using logs, monitoring, tests, and documentation.
- Apply professional responsibility to privacy, accessibility, open-source reuse, and AI-assisted development.

## Prerequisites and course format

Students should have completed a course in a high-level programming language or object-oriented programming and have **B1 English** for reading technical materials. They should understand variables, control flow, functions, and basic collections. Week 1 refreshes programming foundations; classes and interfaces are revisited before object-oriented design in week 6.

The course carries **6 ECTS** and a **150-hour workload**, including 13 lecture hours and 26 laboratory hours. Teaching combines explanations, live programming demonstrations, and hands-on practice in a language students already know. Examples progress from small functions to collaborating modules and a deployable application.

The agenda below lists **lecture topics only**. Laboratory instructions, assignments, and assessment arrangements are provided separately. Git begins in week 2. Build tools have a dedicated week 3 before larger application development; later lessons reuse that build setup.

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
| **3** | **Build tools and dependency management** | Distinguish compilers, runtimes, build tools, dependency managers, and registries. Project structure, configuration, direct and transitive dependencies, versions, and artifacts. Use Maven as the main Java example: pom.xml, dependency coordinates, lifecycle phases, compilation, and JAR packaging. Compare Gradle tasks, plugins, build scripts, and wrappers. Introduce Node.js before npm: package.json, scripts, package-lock.json, and npm install versus npm ci. Mention Yarn as an alternative package manager. Explain wrappers, compatible runtime versions, dependency locking where supported, and which files belong in Git. The test phase is introduced conceptually; test authoring follows in week 7. npm scripts invoke configured tools rather than providing a compiler or a universal build pipeline. |
| **4** | **Requirements and workflow modelling** | Stakeholders, elicitation, functional and non-functional requirements, prioritisation, and specifications. User stories, acceptance criteria, preconditions, and postconditions. UML use case and activity diagrams. Mermaid syntax, `flowchart`, Markdown code fences, and rendering diagrams on GitHub. Distinguish UML activity notation from general flowcharts. |
| **5** | **Development processes and project planning** | Code-and-fix, waterfall, prototyping, and iterative and incremental development. Agile principles, Scrum, and Kanban. Backlogs, task decomposition, estimation uncertainty, dependencies, scope changes, risks, and progress monitoring. Team responsibilities and criteria for completed work. |
| **6** | **Modular programming and object-oriented design** | Functional decomposition, information hiding, cohesion, coupling, and separation of concerns. Objects, classes, constructors, encapsulation, and interfaces. Composition versus inheritance and selected SOLID principles. UML class relationships and multiplicities; Mermaid `classDiagram`. Connecting a model to its implementation. |
| **7** | **Behaviour, testing, and debugging** | Maven test lifecycle from week 3. Contracts, verification and validation, assertions, test cases, and unit tests. Normal and error cases, equivalence partitions, and boundaries. UML state machines and Mermaid `stateDiagram-v2`; tests for valid and invalid transitions. Errors, exceptions, reproduction steps, breakpoints, stack traces, and regression tests. Introduction to integration and acceptance testing. |
| **8** | **Code quality, safe refactoring, and CI** | Code smells, duplication, technical debt, complexity, and maintainability metrics. Refactoring supported by tests; TDD and its red–green–refactor cycle. Black-box and white-box testing, coverage limitations, formatters, and linters. Reuse week 3 build configuration and wrappers. Continuous integration with GitHub Actions workflows, triggers, jobs, and steps. |
| **9** | **Architecture and component interactions** | Architecture versus detailed design. Layers, a modular monolith, interfaces, and dependency boundaries. UML component and sequence diagrams; Mermaid `sequenceDiagram`. Integration and acceptance tests, test doubles, and mocking tradeoffs. Reliability, availability, scalability, maintainability, timeouts, bounded retries, and architecture decision records. |
| **10** | **Secure and responsible software construction** | Assets, trust boundaries, and threats. Authentication and authorisation, validation, safe data access, least privilege, secrets, and dependency risks. Security-focused negative tests. Privacy, data minimisation, accessibility, licences, and attribution. Reviewing and independently verifying AI-generated code. |
| **11** | **Runtime environments, Docker, and deployment modelling** | Source code, artifacts, processes, runtime environments, and configuration. Containers, images, Dockerfiles, builds, registries, Docker Hub, and versioning. Ports, networking, volumes, and secret handling. Docker Compose. UML deployment diagrams and Mermaid infrastructure flowcharts connecting components to runtime environments. |
| **12** | **DevOps, delivery pipelines, and documentation publishing** | Development and operations responsibilities. Continuous integration, delivery, and deployment. Container builds, versioned artifacts, release tags, environments, quality gates, smoke tests, and rollback with GitHub Actions. Publishing Mermaid diagrams on GitHub Pages and other web platforms using configured rendering or image exports. |
| **13** | **Logging, observability, maintenance, and integrated review** | Log levels, destinations, formatting, and structured records. Logs, metrics, traces, health checks, latency, errors, and alerts. Operational diagnosis, sensitive-data protection, incident response, rollback, and blameless review. Regression testing, dependency updates, compatibility, technical debt, and keeping diagrams and documentation current. Briefly trace a change through the complete lifecycle, including diagrams and build configuration. |

### Why this sequence?

Programming foundations support Git collaboration and code review. Week 3 then introduces project structure, dependency management, and repeatable builds before modular application development. Markdown and GitHub come before Mermaid publishing. Requirements establish the behaviour that planning, design, and tests must address. Classes and interfaces precede class-level testing; tests and debugging precede refactoring and CI.

Architecture then connects modules into a system and gives security analysis concrete boundaries. Runtime environments and containers precede delivery automation. Logging and maintenance build on a system students can already understand, test, and release. Week 13 combines maintenance with a brief integrated review, keeping the course at 13 teaching weeks.

### Week 1 foundation checklist

Week 1 establishes the vocabulary and programming baseline used throughout the course.

- **Engineering context:** users, requirements, lifecycle activities, quality, constraints, and change.
- **Programming essentials:** functions, inputs and outputs, collections, conditionals, and loops.
- **Code readability:** naming, formatting, small responsibilities, and understandable control flow.
- **Professional responsibility:** explain your work, acknowledge assistance, and verify claims and generated code.

Git is introduced in week 2, build tools in week 3, UML and Mermaid in week 4, and automated testing in week 7.

## Build tools and dependency management

Week 3 uses **Maven as the main Java build tool**, with short comparisons to **Gradle** and **npm**. Yarn is mentioned as an alternative JavaScript package manager. Students learn one workflow thoroughly enough to reuse it, rather than maintaining the same application in several tools.

| Tool | Teaching scope |
| --- | --- |
| **Maven** | Project layout, `pom.xml`, dependency coordinates, lifecycle phases, compiler configuration, JAR packaging, and Maven Wrapper. Reuse the setup for tests in week 7 and CI in week 8. |
| **Gradle** | Task-based builds, plugins, `build.gradle` or `build.gradle.kts`, dependency declarations, and Gradle Wrapper. Compare its approach with Maven. |
| **npm** | Introduce Node.js, then `package.json`, local dependencies, scripts, `package-lock.json`, and `npm install` versus `npm ci`. Scripts invoke project tools; npm itself is not a Java compiler or a JavaScript bundler. |
| **Yarn** | Recognise an alternative package manager and its lockfile. Follow the project's chosen manager rather than mixing lockfiles. |

Explain direct and transitive dependencies, package registries versus Git repositories, version selection, and generated output. Wrappers select build-tool versions; compatible runtimes and controlled dependency versions also matter. Introduce the test phase conceptually in week 3, then teach test authoring in week 7. Dependency-installation scripts can execute code, so use trusted packages and review project scripts before running them.

Read the official [Maven introduction](https://maven.apache.org/guides/getting-started/maven-in-five-minutes.html), [Gradle concepts](https://docs.gradle.org/current/userguide/gradle_basics.html), [npm scripts guide](https://docs.npmjs.com/cli/v11/using-npm/scripts/), [npm ci reference](https://docs.npmjs.com/cli/v11/commands/npm-ci/), and [Yarn introduction](https://yarnpkg.com/getting-started).

## UML and Mermaid coverage

Select a diagram according to the question it answers. Keep models small enough to read and specific enough to compare with the implementation.

| View | Engineering question | First taught |
| --- | --- | --- |
| **UML use case** | Who uses the system, and for which goals? | Week 4 |
| **UML activity** | How does a workflow proceed and branch? | Week 4 |
| **UML class** | What responsibilities and relationships exist between types? | Week 6 |
| **UML state machine** | Which lifecycle transitions are valid? | Week 7 |
| **UML component** | What are the main parts and their interfaces? | Week 9 |
| **UML sequence** | How do collaborators complete a scenario? | Week 9 |
| **UML deployment** | Where do artifacts execute, and how do environments connect? | Week 11 |

Mermaid coverage progresses through `flowchart` (week 4), `classDiagram` (week 6), `stateDiagram-v2` (week 7), and `sequenceDiagram` (week 9), followed by infrastructure views and web publishing. UML is a modelling language; Mermaid is an authoring and rendering tool. General Mermaid flowcharts can illustrate workflows and infrastructure without claiming to use formal UML activity or deployment notation.

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
