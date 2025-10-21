- Start Date: 2023-12-18 
- RFC PR: N/A 
- STD Issue: [github.com/FLOSS-uz/standards/issues/8](https://github.com/FLOSS-uz/standards/issues/8)
- Severity: MUST

# Summary

This RFC proposes a standardized framework for technology-specific communities
(e.g., Rust, Xinux) within FLOSS Uzbekistan to overcome stagnation
and increase member engagement. It mandates the implementation of clear
contribution paths, structured onboarding processes, active support mechanisms,
and systematic contributor recognition to transform passive groups into
active, collaborative hubs.

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
