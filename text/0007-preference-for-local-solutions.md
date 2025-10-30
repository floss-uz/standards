- Start Date: 2025-10-30
- RFC PR: [floss-uz/standards#0017](https://github.com/floss-uz/standards/pull/17)
- STD Issue: N/A
- Severity: MUST

# Summary

This RFC mandates a preference policy across all FLOSS Uzbekistan member
communities to prioritize the **use, adoption, and contribution** to
locally-developed open-source projects over comparable external (non-Uzbek)
solutions. The goal is to establish the local FLOSS network as the primary
"customer" base and active contributor pool for its own projects, rapidly
accelerating project maturity and filling critical domestic technology gaps.

# Motivation

Many high-quality, locally-developed projects within the FLOSS Uzbekistan
network suffer from stagnation because they lack a critical mass of users
and real-world testing. Developers often default to established international
solutions (due to familiarity or perceived safety), leaving local alternatives
without the vital feedback and contributions needed to mature.

**To solve this:**

1. **FLOSS Uzbekistan must become the primary customer** of its own projects.

2. By mandating preference, we ensure local projects receive immediate usage,
bug reports, and code contributions necessary to achieve the quality and
reliability required for wider commercial adoption.

3. This policy is designed to foster a self-sustaining ecosystem and develop
national technical competence, not to restrict open source principles.

# I. Detailed Design and Preference Policy

All technology-specific communities (e.g., Rust, DevOps, Haskell communities)
and their members **MUST** adhere to the following policy:

## A. Mandatory Preference Hierarchy (MUST)

When selecting a tool, library, framework, or solution for a project (whether
internal, personal, or commercial work endorsed by the community), the member
**MUST** follow this order of preference:

1. **Local FLOSS Solution:** The solution is developed by a FLOSS Uzbekistan
member community or is featured on a community's **Local Resource Curation
List (Awesome Lists)**.

2. **External, Licensed Open Source Solution:** The solution is internationally
available under a recognized open-source license (preferably GPLv3 or
compatible).

3. **Proprietary/Closed-Source Solution:** The solution is non-FLOSS.

## B. The "Local First" Requirement (MUST)

Before adopting any solution lower on the preference hierarchy, the member
**MUST** first conduct a good-faith evaluation of the highest-ranking
available **Local FLOSS Solution**.

- **Evaluation:** The member **MUST** assess whether the local solution
functionally meets the required needs or could meet them with reasonable
contributions.

- **Documentation:** If the local solution is rejected, the member **SHOULD**
document the technical reason for rejection (e.g., missing critical feature,
major bug, insufficient performance). This documentation serves as direct,
invaluable feedback to the local project's maintainers.

- **Contribution Mandate:** If the local solution is adopted, the project
members are encouraged to contribute code, documentation, or issue reports
back to the local solution's repository.

# II. Guide-Level Explanation

To maintainers and community members:

- **Be a Customer First:** Before you `npm install` or `cargo add` a tool from
the internet, check your community's **Awesome List** or ask in the main chat:
"Is there an Uzbek solution for this?"

- **Local Projects Need You:** When you find a local solution that is 80%
ready, don't discard it. Use it, and submit the 20% of missing functionality
as a contribution (bug report, feature request, or code PR). That small
effort turns a stagnant project into a stable one.

- **Documenting Rejection:** If you must use an external tool, take 5 minutes
to explain why the local solution didn't work. This feedback is more valuable
than any donation — it tells the maintainers exactly what they need to
build next.

# III. Unresolved Questions

- How will the council enforce the "good-faith evaluation" requirement
without imposing unnecessary bureaucracy on developers?

- Should there be a grace period (e.g., 6 months) for adopting this policy in
existing commercial projects that already rely heavily on external solutions?

# IV. Future Possibilities

The success of this policy can lead to the creation of a **"FLOSS Uzbekistan
Certified Solution"** program, which grants official recognition and potential
marketing benefits to local projects that meet stability and documentation
standards. This certification would further reinforce the "Local First" policy.
