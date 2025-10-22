- Start Date: 2023-12-18 
- RFC PR: N/A 
- STD Issue: [github.com/FLOSS-uz/standards/issues/8](https://github.com/FLOSS-uz/standards/issues/8)
- Severity: MUST

# Summary

This RFC proposes a standardized framework for technology-specific communities
(e.g., Rust, Xinux) within FLOSS Uzbekistan to overcome stagnation and increase
member engagement. It mandates the implementation of clear contribution
paths, structured onboarding processes, active support mechanisms, and
systematic contributor recognition to transform passive groups into active,
collaborative hubs.

# Motivation

Many technology-focused communities in the Uzbek IT ecosystem suffer from low
engagement, lack of clear contribution paths, and high newcomer abandonment
rates. For FLOSS Uzbekistan to become a mature ecosystem, its constituent
communities must be active and self-sustaining. This standard provides a
principled set of requirements to guide these communities in creating a
welcoming, purpose-driven, and rewarding environment that converts curious
members into active contributors.

# Detailed design

All member communities of FLOSS Uzbekistan MUST implement the following four
pillars of engagement:

## 1. Defining Purpose and Diverse Contribution Paths

Every community **MUST** define a clear, local focus beyond the core
technology itself.

- **Local Project Focus (MUST):** The community **MUST** identify, initiate,
or actively contribute to at least one **local, manageable project**. This
project should have relevance to the Uzbek developer context (e.g., a
localized tool, an open-source library for common Uzbek tasks, or a simple
web application for local impact).

- **Diverse Contribution Paths (MUST):** Community leadership
**MUST** explicitly define and document contribution paths that are
**non-code-centric**. These paths **MUST** include:

    - **Translation:** Contribution to localizing documentation/tutorials
    into Uzbek.

    - **Content Creation:** Writing tutorials, articles, or creating video
    content about the technology.

    - **Community Management:** Responsibilities for organizing events,
    moderation, and newcomer welcoming.

- **Local Resource Curation (MUST):** The community **MUST** gather and
maintain a curated, public list of local open-source projects using their
technology (e.g., an "Awesome-Rust-Uzbekistan" list). This resource serves
as both a contribution path and a local showcase.

## 2. Streamlined Onboarding and First Contributions

The community **MUST** optimize the initial experience for new members.

- **Newcomer's Guide (MUST):** The community **MUST** maintain a clear, concise
**"Newcomer's Guide"** (preferably in Uzbek) that includes: an overview of
the technology, the community's purpose, a roadmap for installation/setup,
a breakdown of all key community platforms (GitHub, Telegram), and a list
of entry-level tasks.

- **"Good First Issue" Labelling (MUST):** Maintainers **MUST** actively
label a revolving set of simple, well-defined issues (e.g., typo fixes,
documentation updates, minor code cleanups) with a `Good First Issue` tag
on their main project repositories.

- **Mentorship Program (SHOULD):** The community SHOULD establish an informal
mentorship program to pair experienced developers with new members for
personalized guidance.


## 3. Cultivating Active Communication and Support

Community leadership **MUST** foster a positive, responsive, and collaborative
environment.

- **Responsiveness (MUST):** Community leaders and experienced members
**MUST** be quick to respond to questions in public channels. A clearly
defined acceptable response time for general queries SHOULD be established.

- **Public Discussion (MUST):** All substantial technical discussions,
debates, and decision-making **MUST** be promoted and conducted in public
community chats or on GitHub to ensure transparency and allow the entire
community to learn.


## 4. Recognition and Incentives

The community **MUST** establish a formal mechanism for acknowledging and
rewarding contributions.

- **Public Recognition (MUST):** Community leadership **MUST** regularly and
publicly highlight contributions (code, documentation, support, organization)
in community announcements, social media, or newsletters.

- **Recognition System (SHOULD):** The community **SHOULD** implement a
system for formal acknowledgment, such as:

    - **Contributor Badges/Roles:** Digital badges or special roles in chat
    platforms (e.g., "Documentation Contributor," "Active Helper").

    - **Gamification:** Small, monetary or non-monetary incentives or public
    leaderboards for answering questions or completing specific tasks.

## 5. Mandatory Documentation Requirements

To ensure all requirements of this standard are transparent, accessible, and
structured for easy onboarding, every technology-specific community **MUST**
implement and maintain the following core set of documents in their main
organizational repository or a dedicated standards repository.

### 5.1. The Newcomer's Guide (Dedicated Document)

The **Newcomer's Guide** is a dedicated, high-level document designed to be
the single entry point for all individuals joining the community. It **MUST**
be highly visible and easily accessible from the main chat and the GitHub
organization homepage.

### 5.2. The Contribution Guide (CONTRIBUTING.md)

The standard GitHub CONTRIBUTING.md file must be expanded to explicitly
cover the diverse contribution paths mandated by this RFC.

| Requirement | Purpose | Status | 
| --- | --- | --- | 
| **Coding Standards** | Must outline coding style, testing requirements, and the process for submitting a Pull Request (PR) to the local community project(s). | MUST |
| **Non-Code Paths** | Must dedicate clear sections detailing the process for submitting: Translations, Tutorials/Content, and how to join a Community Management/Events team. | MUST | 
| **Issue Triage Process** | Must describe how issues are labeled, how long contributors should wait for a review, and the definition of a `Good First Issue`. |MUST |

### **Detailed Structure of `CONTRIBUTING.md`**

#### 1. Getting Started and Code of Conduct

This section sets the tone and the mandatory prerequisites for all
contributors.

- **Code of Conduct (CoC) Link:** A clear, mandatory link to the community's
CODE_OF_CONDUCT.md. This is non-negotiable—all contributors must agree to
abide by the community's rules.

- Direct link to the **Newcomer's Guide** for high-level orientation.

#### 2. Code Contribution Workflow (Setup, Build, and Test)

This section provides the technical roadmap required for hands-on development.

- **Prerequisites:** List all required tools (e.g., specific version of the
SDK/runtime, Git client).

- **Local Setup:** Clear, step-by-step instructions for getting the code:
How to fork the main repository on GitHub and setting upstream.

- **Building the Project:**

    - The exact build command(s) needed (e.g., dotnet build, cargo build,
    nix-build).

    - Troubleshooting steps for common build errors in the local Uzbek
    environment.

- **Testing:**

    - The command(s) needed to run the entire test suite (e.g., dotnet test,
    cargo test).

    - A mandate: All Pull Requests MUST pass all automated tests before they
    will be reviewed.

#### 3. Style, Standards, and Submission

This covers the quality and mechanics of submitting the code for review.

- **Code Style and Quality:**

    - Mandatory tools for automated formatting (e.g., link to the community's
    .editorconfig or .rustfmt.toml).

    - Clear statement on required documentation for new functions and features.

- **Commit and Branching Standards:**

    - Define the required structure for branch names (e.g., feat/my-new-feature
    or bug/fix-123).

    - Define the preferred commit message style (e.g., conventional commits:
    fix: resolve crash on startup).

- **The Pull Request (PR) Submission:**

    - A reminder that the contributor **MUST** fill out the entire PR template.

    - Explanation of the review process, including the expected initial
    response time and guidance on how to respond constructively to feedback.

#### 4. Non-Code Contribution Paths

This critical section formalizes the diverse contribution avenues to meet
the FLOSS Uzbekistan standard.

- **Documentation and Translation:**

    - **Process:** Specify the branch or directory where documentation
    contributions should be submitted (e.g., PRs to the docs/uz folder).

    - **Translation:** if applicable, list all the documents that need to
    be translated into Uzbek.


#### 5. Licensing Information (Legal Mandate)

This section ensures legal transparency and compliance with FLOSS principles.

- **Licensing Terms (MUST):**

    - Explicitly state the project's **license** (e.g., MIT, GPLv3, etc.).

    - **MUST INCLUDE:** A statement that by submitting a Pull Request, the
    contributor agrees to license their work under the project's specified
    license.

    - Link to the full `LICENSE` file.

### 5.3. Project Showcase and Curation (AWESOME_LIST.md)

To fulfill the Local Resource Curation mandate, a dedicated document must
be maintained.

| Requirement | Purpose | Status | 
| --- | --- | --- | 
| **Document Location** | Must be a standalone list (e.g., `AWESOME_RUST_UZ.md`) in the main organizational repository. | MUST | 
| **Content** | Must be a categorized list of locally-relevant open-source projects using the community's core technology, along with contact information or contribution links for each. | MUST | 
| **Maintenance** | Must specify a leader or team responsible for regularly updating the curated list by finding new open-source projects and verifying that the project is still active. | MUST |



### 5.4 Documentation for Recognition and Support

To ensure transparency regarding incentives and acknowledgment, these
processes must be formalized.

| Requirement | Purpose | Status | 
| --- | --- | --- | 
| **Contributor List** | Must maintain an up-to-date `CONTRIBUTORS.md` file, or use a tool to automatically generate a list, acknowledging all individuals who have made a recognized contribution (code, docs, or community help)." | MUST | 
| **Recognition System Rules** | If a **Recognition System** (Badges/Gamification) is implemented (SHOULD), the rules, points system, and rewards (if any) **MUST** be clearly documented in a public location. | MUST |


# Guide-level explanation

To revitalize your community:

1. **Start a Project:** Pick a simple, local problem (e.g., a public Telegram
bot for common Uzbek tech questions) and declare it your community's official
project. This gives everyone a place to contribute.

2. **Document EVERYTHING:** Create a `Newcomers Guide` (in Uzbek) that
tells a new member exactly what to do first. Then, make sure your project
has issues labelled `Good First Issue`.

3. **Be Visible and Helpful:** Make sure questions in your main chat don't
go unanswered for hours.

4. **Celebrate:** When someone submits a pull request, fixes a bug, or even
just answers a difficult question in the chat, **publicly thank them**. Use
your community's social channels to showcase their work.


# Unresolved questions

1. What metrics will be used by the FLOSS Uzbekistan council to measure a
community's compliance and progress in implementing this standard (e.g.,
PR activity, event frequency, responsiveness score)?

2. Should the FLOSS Uzbekistan council provide template documents for
the "Newcomer's Guide" or "Good First Issue" practices to accelerate
implementation?

# Future possibilities

A future RFC could establish a **"Community Health Review"** process where
the council periodically audits member communities based on the metrics
developed from this standard. This could lead to a **"FLOSS Uzbekistan Active
Community"** certification or similar system of endorsement.
