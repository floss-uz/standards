# RFC guidelines - libraries sub-team

# Motivation

- RFCs are heavyweight:

  - RFCs generally take at minimum 2 weeks from posting to land. In
    practice it can be more on the order of months for particularly
    controversial changes.
  - RFCs are a lot of effort to write; especially for non-native speakers or
    for members of the community whose strengths are more technical than literary.
  - RFCs may involve pre-RFCs and several rewrites to accommodate feedback.
  - RFCs require a dedicated shepherd to herd the community and author towards
    consensus.
  - RFCs require review from a majority of the core team members, as well as an official
    vote.
  - RFCs can't be downgraded based on their complexity. Full process always applies.
    Easy RFCs may certainly land faster, though.
  - RFCs can be very abstract and hard to grok the consequences of (no implementation).

- PRs are low _overhead_ but potentially expensive nonetheless:

  - Easy PRs can get insta-merged by any floss-uz contributor.
  - Harder PRs can be easily escalated. You can ping subject-matter experts for second
    opinions. Ping the whole core-team!
  - Easier to grok the full consequences. Lots of tests to save the day.

- RFCs are _only_ meaningful if a significant and diverse portion of the
  community actively participates in them. The official members are not
  sufficiently diverse to establish meaningful community consensus by agreeing
  amongst themselves.

- If there are _tons_ of RFCs -- especially trivial ones -- people are less
  likely to engage with them. Official team members are super busy. Domain experts
  and industry professionals are super busy _and_ have no responsibility to engage
  in RFCs. Since these are _exactly_ the most important people to get involved in
  the RFC process, it is important that we be maximally friendly towards their
  needs.

# Is an RFC required?

The overarching philosophy is: _do whatever is easiest_. If an RFC
would be less work than an implementation, that's a good sign that an RFC is
necessary. That said, if you anticipate controversy, you might want to short-circuit
straight to an RFC. For instance new stds almost certainly merit an RFC. Especially
as `std` has become more conservative in favour of the much more agile.

- **Submit a PR** if the change is a:
  - Docfix
  - Minor tweak to an unstable std (renaming, generalizing)
  - Implementing an "addition" to std
- **Submit an RFC** if the change is a:
  - New STD
  - Semantic Change to a STD
  - Generalization of a STD (e.g. how we added rules)
  - Deprecation of a STD
- **Do the easier thing** if uncertain. (choosing a path is not final)

# Non-RFC process

- A (non-RFC) PR is likely to be **closed** if clearly not acceptable:

  - Disproportionate breaking change (small inference breakage may be acceptable)
  - Unsound
  - Doesn't fit our general design philosophy around the problem
  - Better as a rule under a certain community
  - Too marginal for std
  - Significant implementation problems

- A PR may also be closed because an RFC is appropriate.

- A (non-RFC) PR may be **merged as unstable**. In this case, the standard
  should have a fresh std gate and an associated tracking issue for
  stabilisation.

However, an accepted RFC is not a rubber-stamp for merging an implementation PR.
Nor must an implementation PR perfectly match the RFC text. Implementation details
may merit deviations, though obviously they should be justified. The RFC may be
amended if deviations are substantial, but are not generally necessary. RFCs should
favour immutability. The RFC + Issue + PR should form a total explanation of the
current implementation.

- Once something has been merged as unstable, a shepherd should be assigned
  to promote and obtain feedback on the design.

- After the final comment period, an STD should ideally take one of two paths:

  - **Stabilize** if the change is desired, and consensus is reached
  - **Deprecate** is the change is undesired, and consensus is reached
  - **Extend the FCP** is the change cannot meet consensus
    - If consensus _still_ can't be reached, consider requiring a new RFC or
      just deprecating as "too controversial for std".

- If any problems are found with a newly stabilized STD during its application period,
  _strongly_ favour reverting stability in order to prevent stabilizing a bad
  STD. Due to the speed of the trains, this is not a serious delay (~2-3 months
  if it's not a major problem).
