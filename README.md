# Integrative Project – Semester 3 – Group G152 (2024/25)

**Degree:** BSc in Computer Engineering / or equivalent  
**Course:** Integrative Project (2nd semester of Year 3)  
**Repository:** `sem3-pi_2024_25_G152`

---

## Table of Contents  
- [Project Overview](#project-overview)  
- [Current Repository State](#current-repository-state)  
- [Key Components & Features](#key-components-features)  
- [Technologies & Requirements](#technologies-requirements)  
- [Installation, Build & Execution](#installation-build-execution)  
- [Repository Structure](#repository-structure)  
- [Work Flow & Contribution Guidelines](#work-flow-contribution-guidelines)  
- [Testing & Quality Assurance](#testing-quality-assurance)  
- [Continuous Integration / Badges](#continuous-integration-badges)  
- [Roadmap & Future Enhancements](#roadmap-future-enhancements)  
- [License & Contacts](#license-contacts)

---

## Project Overview  
This repository contains the codebase and supporting artefacts for the Integrative Project (PI) of Semester 3 (academic year 2024/25) for Group G152. The project is executed under an Agile methodology (Scrum), utilising GitHub Projects for backlog/sprints, Git for version control, and Maven (or equivalent) for build management.

The objective is to design, implement, test, document and deliver a working software solution that meets the defined user stories, architectural requirements, and sprint deliverables.

---

## Current Repository State  
- Initial project skeleton with Maven (or chosen build tool) configuration.  
- Supporting documentation and templates provided (in `docs/`).  
- Notebook or planning artefact for user-stories/sprint planning (e.g., `matcp.ipynb`).  
- Source code directory (`src/`) with package structure and main entry point (e.g., `com.yourorganisation.project.Main`).  
- Unit tests directory (`test/`) setup for future expansion.

---

## Key Components & Features  
Based on the current repository contents, major building blocks include:  
- **Main Application Module**: Java (or language of choice) application packaged to produce an executable jar or equivalent.  
- **User Story & Sprint Planning Artefact**: A Jupyter Notebook (`matcp.ipynb`) or equivalent – used for capturing user stories, acceptance criteria, backlog items and sprint planning.  
- **Documentation & Templates**: Located under `docs/`, includes templates for requirements, design models (UML), test plans, and sprint retrospective outputs.  
- **Tests & Quality Infrastructure**: Framework configured for unit/integration tests and code coverage analysis.

---

## Technologies & Requirements  
Minimum required software and tools:  
- **Java** (version 17 or higher recommended)  
- **Maven** (version 3.6+ or compatible)  
- **Git** (for version control)  
- **IDE**: IntelliJ IDEA, Eclipse, or VSCode with Java support  
- **Jupyter Notebook** (for planning artefact editing)  
Adjust the versions and tools if your project uses Kotlin, Gradle, or another stack.

---

## Installation, Build & Execution

### 1) Clone the repository  
```bash
git clone https://github.com/BMSaiko/sem3-pi_2024_25_G152.git
cd sem3-pi_2024_25_G152
2) Build & Run Unit Tests
bash
Copiar código
mvn clean test
3) Package the Application
Ensure your pom.xml (or equivalent) is configured with a mainClass (e.g., com.yourorganisation.project.Main) and a plugin to create a “jar-with-dependencies”. Then execute:

bash
Copiar código
mvn package
4) Execute the Application
bash
Copiar código
java -jar target/yourprojectname-version-jar-with-dependencies.jar
Replace yourprojectname-version-jar-with-dependencies.jar with the actual artifact name.

5) Run from IDE
Open the project in your IDE as a Maven project and run the main class. Ensure the entry point matches what is configured in the build tool.

Repository Structure
bash
Copiar código
/ (root)
├── docs/                        ← Documentation & templates for sprints
│   ├── system-documentation/    ← UML diagrams, ADRs, design decisions
│   └── sprint1/…                ← Sprint artefacts and deliverables
├── src/                         ← Application source code
│   └── main/java/com/…         
├── test/                        ← Unit/integration tests
├── matcp.ipynb                  ← Notebook for backlog/user stories/sprint planning
├── pom.xml                      ← Maven build file (or build config)
├── README.md                    ← This file
└── LICENSE                      ← License file (if present)
Work Flow & Contribution Guidelines
Branch Structure:

main — stable & release-ready code

Feature branches: <US-ID>_<short-feature-name> (e.g., 12_US4_login-module)

Pull Requests: All merges into main must be via pull request, reviewed by another team member.

Commit Messages: Use a clear format, such as:

makefile
Copiar código
US-12: Implement login validations
User Stories: Format:

css
Copiar código
As a [persona], I want [functionality], so that [benefit].
Each story must include acceptance criteria, size (story points), priority, assignee and definition of done.

Sprint Cadence: Each sprint includes Planning → Development → Review → Retrospective phases.

Testing & Quality Assurance
Unit tests are written using JUnit (or equivalent framework).

Use a code coverage tool such as JaCoCo to monitor coverage, with threshold (e.g., 70%).

Use static analysis tools (e.g., Checkstyle, SpotBugs) for code quality.

Example Maven commands:

bash
Copiar código
mvn test jacoco:report
mvn test jacoco:check
Continuous Integration / Badges
It is highly recommended to set up GitHub Actions (or other CI) to automate:

Maven build (mvn clean verify)

Unit tests

Code coverage check

Static analysis
Add these badges to the top of this README, such as:

bash
Copiar código
[![Build Status](https://github.com/BMSaiko/sem3-pi_2024_25_G152/actions/workflows/maven.yml/badge.svg)](https://github.com/BMSaiko/sem3-pi_2024_25_G152/actions)
[![Coverage Status](https://coveralls.io/repos/github/BMSaiko/sem3-pi_2024_25_G152/badge.svg?branch=main)](https://coveralls.io/github/BMSaiko/sem3-pi_2024_25_G152?branch=main)
Roadmap & Future Enhancements
Short-Term

Complete coverage of core modules with unit tests.

Ensure build produces a working jar-with-dependencies.

Update documentation (docs/system-documentation/) with UML diagrams and ADRs.

Mid-Term

Implement and automate CI/CD pipeline.

Add integration tests and system tests.

Update backlog notebook (matcp.ipynb) with new user stories for upcoming sprints.

Long-Term

Create GitHub Releases for major versions.

Package and deploy as a Docker container or cloud service (if applicable).

Provide user-guide and operations handbook for end-users or administrators.

License & Contacts
License: Please refer to the LICENSE file for full license details (e.g., MIT, Apache-2.0).

Team: Fill in your team member names, roles, and contact information.

Issues: For bugs, feature requests or contributions, please open an Issue in this repository.

Credits
Thank you to everyone involved — project lead, developers, testers, and reviewer team members.
Templates and initial skeleton provided in this repository by the academic unit.

