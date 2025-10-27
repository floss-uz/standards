- Start Date: 2025-10-27
- RFC PR: N/A
- STD Issue: N/A
- Severity: MUST

# Summary

This RFC mandates that all new projects initiated under the FLOSS Uzbekistan
network **MUST** be released under the **GNU General Public License,
Version 3 (GPLv3)**. Furthermore, all existing projects currently maintained
or formally endorsed by member communities **MUST** be relicensed under
GPLv3. This non-permissive (or copyleft) licensing strategy is proposed to
strengthen the local open-source ecosystem by ensuring code, including any
future modifications, remains permanently open and available for the entire
Uzbek community.

# Motivation

The primary goal of FLOSS Uzbekistan is to cultivate a robust, shared
technical infrastructure. Using permissive licenses (like MIT or Apache
2.0) allows companies to use and modify the code without contributing their
improvements back to the community, effectively creating proprietary forks
from public effort. This practice fragments the local ecosystem and siphons
value away from the community.

Mandating the GPLv3, a strong copyleft license, ensures that all derivative
works built upon the community's projects must also be shared under GPLv3. This
legal mechanism compels contribution back to the public pool, guaranteeing that
the intellectual effort invested by Uzbek developers collectively benefits
the entire FLOSS Uzbekistan network, thereby accelerating the growth and
maturity of the local open-source space.

# Detailed design

All technology-specific communities (e.g., Rust, Haskell, NixOS communities)
within FLOSS Uzbekistan **MUST** adhere to the following licensing mandates:

- **New Projects (MUST):** Any new open-source project initiated or adopted
by a member community after the effective date of this Standard **MUST**
use the **GNU General Public License, Version 3 (GPLv3)**.

- **Existing Projects (MUST):** All currently existing projects maintained
or officially endorsed by member communities **MUST** begin the process of
relicensing under **GPLv3**. This process requires securing permission from
all past and current copyright holders and **MUST** be completed within a
maximum of twelve (12) months from the Standard's adoption date.

- **Documentation Requirement (MUST):** The project's primary `README.md`
and `CONTRIBUTING.md` files **MUST** prominently state that contributions
are accepted only under the terms of the GPLv3.

- **License File (MUST):** Every repository **MUST** include a copy of the
`LICENSE` file containing the full text of the GPLv3.

# Benefits of Non-Permissive (Copyleft) Licensing over Permissive Licensing

The adoption of a non-permissive license like GPLv3, as opposed to permissive
licenses (like MIT, BSD, or Apache 2.0), provides substantial benefits for
a community-driven ecosystem like FLOSS Uzbekistan:

1. **Guaranteed Freedom and Community Growth (The "Viral" Effect):**

    - **Permissive:** Allows derived proprietary works. A local company
    can take a community library, improve it, and sell the improved version
    without sharing the source code, reducing the shared knowledge pool.

    - **Non-Permissive (GPLv3):** Requires any redistributed software that
    incorporates the original code (or derived code) to also be released under
    GPLv3. This powerful **copyleft** mechanism legally forces downstream
    developers, including commercial users, to contribute their improvements
    back to the public, ensuring the community always benefits from the work.

2. **Protection Against Fragmentation:**

    - **Permissive:** Creates a risk of "forking" where a company takes
    the project and continues development privately, leaving the community
    project to stagnate.

    - **Non-Permissive (GPLv3):** Discourages the creation of proprietary
    forks because the forking entity knows they will be legally required
    to release their changes, promoting a single, robust codebase shared by
    all local stakeholders.

3. **Strengthening Open-Source Principles:**

    - **Permissive:** Primarily benefits users and companies by granting
    maximal usage rights with minimal legal obligation.

    - **Non-Permissive (GPLv3):** Primarily benefits the **developers and
    the community** by ensuring that the fundamental open-source principles
    of access, study, modification, and redistribution are maintained for
    every user, permanently.

# Guide-level explanation

For all Maintainers:

- **Licensing is Mandatory:** Every project you touch or create from now on
**MUST** use the GPLv3 license.

- **The Power of Copyleft:** When you write code under GPLv3, you guarantee
that anyone who builds on your work — even a commercial company — **MUST**
release their own source code. This ensures all improvements come back to
our community.

- **Relicensing Existing Work:** You need to contact everyone who ever made
a code contribution to your project (no matter how small) and get their
explicit, written permission to change the project's license to GPLv3. This
step is non-negotiable for legal compliance. Start this process immediately.

# Unresolved questions

- What official FLOSS Uzbekistan resource will be provided to assist
communities with the legal process of tracking down and obtaining relicensing
consent from past contributors?

- How will the council handle an existing project where relicensing is
technically or legally impossible (e.g., a critical mass of contributors
cannot be located or refuse consent)?

# Future possibilities
