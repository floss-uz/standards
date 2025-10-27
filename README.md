# FLOSS Uzbekistan RFCs - [RFC Book](https://std.floss.uz/)

[FLOSS RFCs]: #floss-rfcs

The "RFC" (request for comments) process is intended to provide a
consistent and controlled path for new features to enter the project
and communities, so that whole uzbek it communities with its developers
can be confident about the direction the uzbek is evolving in.

Many changes, including typo fixes and documentation improvements can be
implemented and reviewed via the normal GitHub pull request workflow.

Some changes though are "substantial", and we ask that these be put
through a bit of a design process and produce a consensus among the FLOSS
Uzbekistan community and the [core team].

## Table of Contents

[Table of Contents]: #table-of-contents

- [Opening](#floss-rfcs)
- [Table of Contents]
- [When you need to follow this process]
- [Specific guidelines]
- [Before creating an RFC]
- [What the process is]
- [The RFC life-cycle]
- [Reviewing RFCs]
- [Implementing an RFC]
- [RFC Postponement]
- [Help this is all too informal!]
- [License]
- [Contributions]

## When you need to follow this process

[When you need to follow this process]: #when-you-need-to-follow-this-process

You need to follow this process if you intend to make "substantial"
changes to the FLOSS Uzebkistan distribution. What constitutes a "substantial"
change is evolving based on community norms, but may include the following.

- Any semantic or syntactic change to the standards.
- Removing stds, including those that are feature-gated.
- Changes to the interface between the stds and rule-sets, intrinsics.
- Additions to `stds`.

Some changes do not require an RFC:

- Rephrasing, reorganizing, refactoring, or otherwise "changing shape
  does not change meaning".
- Additions only likely to be _noticed by_ other core-of-floss,
  invisible to members-of-floss.

If you submit a pull request to implement a new feature without going
through the RFC process, it may be closed with a polite request to
submit an RFC first.

### Specific guidelines

[Specific guidelines]: #specific-guidelines

For more details on when an RFC is required for the following areas, please see
the Rust community's [sub-team] specific guidelines for:

- [general changes](changes.md)
<!-- - [language changes](lang_changes.md) -->

## Before creating an RFC

[Before creating an RFC]: #before-creating-an-rfc

A hastily-proposed RFC can hurt its chances of acceptance. Low quality
proposals, proposals for previously-rejected features, or those that don't fit
into the near-term roadmap, may be quickly rejected, which can be demotivating
for the unprepared contributor. Laying some groundwork ahead of the RFC can
make the process smoother.

Although there is no single way to prepare for submitting an RFC, it is
generally a good idea to pursue feedback from other project developers
beforehand, to ascertain that the RFC may be desirable; having a consistent
impact on the project requires concerted effort toward consensus-building.

The most common preparations for writing and submitting an RFC include talking
the idea over on our [official telegram chat], and occasionally posting "pre-RFCs"
on the developer forum. You may file issues on this repo for discussion, but
these are not actively looked at by the core team members.

As a rule of thumb, receiving encouraging feedback from long-standing project
developers, and particularly members of the relevant [core-team] is a good
indication that the RFC is worth pursuing.

## What the process is

[What the process is]: #what-the-process-is

In short, to get a standards added to Uzbek communities, one must first get the RFC
merged into the RFC repository as a markdown file. At that point the RFC is
"active" and may be implemented with the goal of eventual inclusion into general
collection of overall STDs applied over all uzbek communities that are affected with
rules applied by its maintainers.

- Fork the RFC repo [RFC repository]
- Copy `0000-template.md` to `text/0000-my-std.md` (where "my-std" is
  descriptive). Don't assign an RFC number yet; This is going to be the PR
  number and we'll rename the file accordingly if the RFC is accepted.
- Fill in the RFC. Put care into the details: RFCs that do not present
  convincing motivation, demonstrate lack of understanding of the design's
  impact, or are disingenuous about the drawbacks or alternatives tend to
  be poorly-received.
- Submit a pull request. As a pull request the RFC will receive design
  feedback from the larger community, and the author should be prepared to
  revise it in response.
- Now that your RFC has an open pull request, use the issue number of the PR
  to update your `0000-` prefix to that number.
- Each pull request will be labeled with the most relevant [core-team] member,
  which will lead to its being triaged by that member in a future meeting and
  assigned to a member of the [core-team].
- Build consensus and integrate feedback. RFCs that have broad support are
  much more likely to make progress than those that don't receive any
  comments. Feel free to reach out to the RFC assignee in particular to get
  help identifying obstacles.
- The sub-team will discuss the RFC pull request, as much as possible in the
  comment thread of the pull request itself. Offline discussion will be
  summarized on the pull request comment thread.
- RFCs rarely go through this process unchanged, especially as alternatives
  and drawbacks are shown. You can make edits, big and small, to the RFC to
  clarify or change the design, but make changes as new commits to the pull
  request, and leave a comment on the pull request explaining your changes.
  Specifically, do not squash or rebase commits after they are visible on the
  pull request.
- At some point, a member of the [core-team] member will propose a "motion for final
  comment period" (FCP), along with a _disposition_ for the RFC (merge, close,
  or postpone).
  - This step is taken when enough of the tradeoffs have been discussed that
    the subteam is in a position to make a decision. That does not require
    consensus amongst all participants in the RFC thread (which is usually
    impossible). However, the argument supporting the disposition on the RFC
    needs to have already been clearly articulated, and there should not be a
    strong consensus _against_ that position outside of the subteam. Subteam
    members use their best judgment in taking this step, and the FCP itself
    ensures there is ample time and notification for stakeholders to push
    back if it is made prematurely.
  - For RFCs with lengthy discussion, the motion to FCP is usually preceded by
    a _summary comment_ trying to lay out the current state of the discussion
    and major tradeoffs/points of disagreement.
  - Before actually entering FCP, _all_ members of the subteam must sign off;
    this is often the point at which many subteam members first review the
    RFC in full depth.
- In most cases, the FCP period is quiet, and the RFC is either merged or
  closed. However, sometimes substantial new arguments or ideas are raised,
  the FCP is canceled, and the RFC goes back into development mode.

## The RFC life-cycle

[The RFC life-cycle]: #the-rfc-life-cycle

Once an RFC becomes "active" then authors may implement it and submit the
feature as a pull request to the Rust repo. Being "active" is not a rubber
stamp, and in particular still does not mean the feature will ultimately be
merged; it does mean that in principle all the major stakeholders have agreed
to the feature and are amenable to merging it.

Furthermore, the fact that a given RFC has been accepted and is "active"
implies nothing about what priority is assigned to its implementation, nor does
it imply anything about whether a Rust developer has been assigned the task of
implementing the feature. While it is not _necessary_ that the author of the
RFC also write the implementation, it is by far the most effective way to see
an RFC through to completion: authors should not expect that other project
developers will take on responsibility for implementing their accepted feature.

Modifications to "active" RFCs can be done in follow-up pull requests. We
strive to write each RFC in a manner that it will reflect the final design of
the feature; but the nature of the process means that we cannot expect every
merged RFC to actually reflect what the end result will be at the time of the
next major release.

In general, once accepted, RFCs should not be substantially changed. Only very
minor changes should be submitted as amendments. More substantial changes
should be new RFCs, with a note added to the original RFC. Exactly what counts
as a "very minor change" is up to the sub-team to decide; check
[Sub-team specific guidelines] for more details.

## Reviewing RFCs

[Reviewing RFCs]: #reviewing-rfcs

While the RFC pull request is up, the core-team member may schedule meetings
with the author and/or relevant members to discuss the issues in greater
detail, and in some cases the topic may be discussed at a core-team meeting. In
either case a summary from the meeting will be posted back to the RFC pull
request.

A core-team makes final decisions about RFCs after the benefits and drawbacks
are well understood. These decisions can be made at any time, but the core-team
will regularly issue decisions. When a decision is made, the RFC pull request
will either be merged or closed. In either case, if the reasoning is not clear
from the discussion in thread, the core-team will add a comment describing the
rationale for the decision.

## Implementing an RFC

[Implementing an RFC]: #implementing-an-rfc

Some accepted RFCs represent vital features that need to be implemented right
away. Other accepted RFCs can represent features that can wait until some
arbitrary developer or community member feels like doing the work. Every
accepted RFC has an associated issue tracking its implementation in the STD
repository; thus that associated issue can be assigned a priority via the
triage process that the team uses for all issues in the STD repository.

The author of an RFC is not obligated to implement it. Of course, the RFC
author (like any other member) is welcome to post an implementation for
review after the RFC has been accepted.

If you are interested in working on the implementation for an "active" RFC, but
cannot determine if someone else is already working on it, feel free to ask
(e.g. by leaving a comment on the associated issue).

## RFC Postponement

[RFC Postponement]: #rfc-postponement

Some RFC pull requests are tagged with the "postponed" label when they are
closed (as part of the rejection process). An RFC closed with "postponed" is
marked as such because we want neither to think about evaluating the proposal
nor about implementing the described feature until some time in the future, and
we believe that we can afford to wait until then to do so. Postponed pull
requests may be re-opened when the time is right. We don't have any formal
process for that, you should ask members of the relevant core-team.

Usually an RFC pull request marked as "postponed" has already passed an
informal first round of evaluation, namely the round of "do we think we would
ever possibly consider making this change, as outlined in the RFC pull request,
or some semi-obvious variation of it." (When the answer to the latter question
is "no", then the appropriate response is to close the RFC, not postpone it.)

### Help this is all too informal!

[Help this is all too informal!]: #help-this-is-all-too-informal

The process is intended to be as lightweight as reasonable for the present
circumstances. As usual, we are trying to let the process be driven by
consensus and community norms, not impose more structure than necessary.

## License

[License]: #license

This repository is currently in the process of being licensed under either of:

- Apache License, Version 2.0, ([LICENSE-APACHE](LICENSE-APACHE) or https://www.apache.org/licenses/LICENSE-2.0)
- MIT license ([LICENSE-MIT](LICENSE-MIT) or https://opensource.org/licenses/MIT)

at your option. Some parts of the repository are already licensed according to those terms. For more see [RFC N/A](#) and its [tracking issue](#).

### Contributions

[Contributions]: #contributions

Unless you explicitly state otherwise, any contribution intentionally submitted for inclusion in the work by you, as defined in the Apache-2.0 license, shall be dual licensed as above, without any additional terms or conditions.

[official telegram chat]: https://t.me/flossuzc
[RFC repository]: https://github.com/floss-uz/standards
[core-team]: #
