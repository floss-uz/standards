- Standartization Name: English as the Primary Language for Formal
Communication and Technical Standardization

- Start Date: 2025-10-31

- RFC PR: N/A

- STD Issue: N/A

- Severity: MUST

# Summary

This RFC mandates the use of **English** as the **Primary Language** for
all formal communication, technical documentation, and code contributions
within the FLOSS Uzbekistan network. This policy aligns the community with
global open-source standards, ensuring maximum accessibility to international
contributors and tools. Furthermore, all Uzbek technical communication **MUST**
standardize on the **Latin alphabet**, deprecating the use of Cyrillic script.

# Motivation

While promoting the Uzbek language is important for local empowerment,
mandating English for formal technical communication provides critical benefits
for the long-term sustainability and quality of FLOSS Uzbekistan projects:

1. **Maximizing Global Contribution:** English is the lingua franca of
software development. Standardizing on English immediately lowers the
barrier to entry for international contributors, users, and reviewers,
directly increasing the talent pool and external feedback loop.

2. **Tooling Compatibility:** English simplifies interaction with essential
global tools (GitHub, automated translation services, static analysis tools)
which are primarily designed around Latin-based languages.

3. **Professional Readiness:** Mandating English prepares Uzbek developers
for global careers and high-level international collaboration, reinforcing
the community's role in professional development.

4. **Uzbek Script Standardization:** Deprecating the Cyrillic alphabet for
technical writing eliminates internal confusion and aligns with the widely
recognized Latin script used in modern coding environments and data processing.

# I. Detailed Design and Language Mandates

All technology-specific communities (e.g., Rust, Haskell, DevOps) and their
members MUST adhere to the following language requirements:

## A. Formal Communication (MUST be English)

All official and formal communications channels **MUST** use English
exclusively:

- **RFCs and Standards:** All new RFCs and proposed standards **MUST**
be written in English.

- **Code Review:** All Pull Request (PR) titles, descriptions, and review
comments **MUST** be in English.

- **Issue Tracking:** All GitHub issues, bug reports, feature requests,
and issue comments **MUST** be in English.

- **Official Announcements:** Major announcements, official blog posts **MUST**
be delivered in English.

## B. Technical Documentation and Readmes

English **MUST** be the source of truth for all technical documentation.

- **Documentation Priority (MUST):** Project documentation (e.g., reference
guides, API documentation, tutorials) MUST be authored in English first. The
English version serves as the canonical source.

- **Uzbek Documentation (SHOULD):** An Uzbek version of documentation is
strongly encouraged as a secondary resource but is not mandatory unless
specified by a separate localization standard.

- **Project Readmes (MUST):** Every repository MUST provide an English
version of the README.md. An Uzbek version may be provided alongside it
(e.g., in the same file or a separate README_uz.md).

## C. Uzbek Script Standardization (MUST)

When writing technical content in the Uzbek language (e.g., in documentation,
readmes, or internal code comments):

- **Latin Alphabet Only:** Only the Latin alphabet **MUST** be used.

- **Cyrillic Deprecation:** The use of the Cyrillic alphabet for all official
FLOSS Uzbekistan technical communications, repositories, and documentation
is deprecated and **MUST** be phased out.

# II. Guide-Level Explanation

For community members and contributors:

- **English is the Default:** When you open a PR, write an RFC, or report
a bug on GitHub, use clear, concise English. This is non-negotiable for
formal submissions.

- **Prioritize English Docs:** If you are a technical writer or contributor
to documentation, create and maintain the English version first.

- **Use Latin for Uzbek:** When you switch to Uzbek for a piece of
documentation or a comment, only use the Latin alphabet.

For community leaders and maintainers:

- **Active Enforcement:** Politely but firmly reject PRs and RFCs submitted
in non-English languages, asking the contributor to resubmit in English.

- **Migration Plan:** For existing documentation that uses Cyrillic Uzbek,
establish a plan to migrate the content to the Latin script within six (6)
months of this standard's adoption.

# III. Unresolved Questions

- Will the FLOSS Uzbekistan council provide automated tooling or resources
to help communities migrate existing Cyrillic-based documentation to the
Latin alphabet?

# IV. Future Possibilities
