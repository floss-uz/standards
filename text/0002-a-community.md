- Standartization Name: Shaping up what it means to be a community
- Start Date: 2025-04-09
- RFC PR: [floss-uz/standards#0003](https://github.com/floss-uz/standards/pull/3)
- STD Issue: [floss-uz/standards#0002](https://github.com/floss-uz/standards/issues/2)
- Severity: MUST

# Summary

[summary]: #summary

This RFC explains what it means to be a part of [Uzbek Open Source]
(a.k.a Floss Uzbekistan) community and the requirements a community
SHOULD meet before they join or become a representative member of
[Uzbek Open Source] community.

# Motivation

[motivation]: #motivation

Over the last few weeks, we greeted many existing developer communities to
Uzbek Open Source community. However, due to constantly changing shape of
every community, it was decided to create and RFC that explicitly explains
the requirements that a new joining community MUST meet or how a pre-existing
community SHOULD shape up to. This RFC will prevent any further confuses and
misunderstanding on explanation of "What it means to be a community inside
Floss Uzbekistan".

# Detailed design

[detailed-design]: #detailed-design

We, a standing current committees of Uzbek Open Source, suggest that a chat-based community MUST
have around 50 members, approximately 10 active members and about 2 moderators (including owner).
It is MUST to have a GitHub organization if the joining community is about:

- a programming language
- a technology that is a domain to many others
- an aggregator to multiple other chat based communities

Also, the member community SHOULD have a website showing representatives of the community,
the list of member sub-communities (any type) and the ongoing active projects with links
to GitHub repositories and the GitHub organization.

After acceptance, if community doesn't have a telegram assistant, the community MUST implement
a telegram bot which helps members with accessing useful links, information about the
technology they are focusing on and also links to website and github organization.

It's also worth to mention that either telegram chat or GitHub organization MUST NOT be deleted
at any cost as these two elements represent the community and its efforts as a member of Floss
Uzbekistan.

The community MUST invite Floss Uzbekistan's telegram bot [@flossuzbot] to their chat to let users
easily switch over other Floss Uzbekistan supported communities and bond stronger relationship with
other communities.

**These are suggestions to guide community structure, with the final decision to be determined by
the council.**

The optional requirements MUST be satisfied as soon as the community gets accepted to
Floss Uzbekistan. Otherwise, if community refuses or does not implement given requirements
in given time, the comittee still can decline and remove the community from the network.
Afterwards, the community might be subjected to changes proposed by the committees of Floss
Uzbekistan.

# Guide-level explanation

[guide-level-explanation]: #guide-level-explanation

**Basic requirements before a community joins our network:**

- Make sure you have a telegram chat community with 50+ members in it.
- Your community MUST exist more than 3 months.
- Check if at least 10 people are keeping it active on daily basis.
- See if you have 2 moderators that are maintaining chats.
- Then check if you have a GitHub organization to represent your community, if you don't have one, create it.
- If you don't have website, reserve a domain at .uz TLD for your community to later use in website.
- Use your domain to verify your github organization.
- If you don't have a website, initiate a repository at github organization and create very basic at least html and deploy it.
- Upon completing the steps above, reach Floss Uzbekistan chair via either Telegram chat at [@flossuzc] or [open a discussion at Github].

**Further extra-steps to perform after getting accepted:**

- Let your community member know that the community has became a member of Floss Uzbekistan network.
- Add [@flossuzbot] to your community chat.
- Organize your GitHub organization and create necessary projects
- If you don't have an assistant telegram bot in your community, implement it alongside website and finish as soon as possible.
- Alter team changes to Floss Uzbeksitan's website and other sources by adding chair and maintainer or request a Floss maintainer to do it for you.

# Unresolved questions

[unresolved-questions]: #unresolved-questions

- Does this RFC cover all type of community effort?
- Does this RFC make community acceptance smooth enough?

# Future possibilities

[future-possibilities]: #future-possibilities

The current RFC already addresses the core issue with community's joining
process. However, things that should be implemented throughout the proccess
should be explored broader and explain further in the upcoming RFCs. The
current implementation is not fully complete and is subjected to further
modifications based on upcoming experience.

[Uzbek Open Source]: https://github.com/floss-uz
[@flossuzc]: https://t.me/flossuzc
[open a discussion at Github]: https://github.com/orgs/floss-uz/discussions
[@flossuzbot]: https://t.me/flossuzbot
