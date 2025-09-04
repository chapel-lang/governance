Governance of the Chapel Project
================================

This file describes the current governance of the Chapel Language
project, covering the language's definition; the code base that
implements its compiler, library modules, runtime, and tools; and the
project's documentation.  It was last updated in September 2025.  This
file goes hand-in-hand with the project's technical charter,
`CHARTER.md`, which defines the project's operations, roles and
responsibilities, IP policy, and serves as the core governance of the
project's LLC.

Over time, we anticipate improving the Chapel project's governance.
If you have specific requests with respect to how the project is
governed, please feel encouraged to capture those in an issue on this
repository, or to bring it up [in our community
forums](https://chapel-lang.org/community/).


This document has two main sections: the first defines technical roles
and the second outlines the project's decision-making process.


Technical Roles
===============

This section defines the following technical roles for the Chapel
community:

* the Technical Steering Committee (TSC) and its Chair
* the Tech Lead
* Subteam Leads, who are tasked with heading up specific efforts
* Committers, who have merge permissions to the major repositories
* Contributors, who have contributed technical artifacts into the
  Chapel release
* Community Collaborators, who contribute in other ways such as
  feature requests, bug reports, and feedback.

Generally speaking, all committers are contributors, and any
contributor or community collaborator can request to join the TSC.  At
present, we are lacking a means for a community members to be a
contributor, but one of the roles of the TSC will be to define this
process.


Technical Steering Committee (TSC)
----------------------------------

Role: The project's overall technical direction is governed by the
Technical Steering Committee, whose members' roles are detailed in
`CHARTER.md`.  At the inception of the project, TSC membership was
offered to everyone with commit privileges to the chapel-lang/chapel
repo.  This led to the current TSC membership, which is:

* Jade Abraham
* Brad Chamberlain
* Lydia Duncan
* Daniel Fedorin
* Abhishek Girish
* Ben Harshbarger
* John Hartman
* Engin Kayraklioglu
* Shreyas Khandekar
* Anna Rift
* Elliot Ronaghan
* Andy Stone
* Karlon West

See `CHARTER.md` for additional information about TSC membership,
roles, and responsibilities.


TSC Chair
---------

The TSC may decide to define a chair for the committee and elect
someone to that role, with responsibilities such as presiding over
meetings of the TSC and serving as the primary communication point
between the Chapel project and the High Performance Software
Foundation (HPSF).  The TSC Chair would serve until their resignation
or replacement by the TSC.

At the time of this writing, the TSC has not yet met and opted to do,
so the position of chair is currently undefined and unfilled.


Tech Lead
---------

Role: The project technical lead's role is to help guide decisions for
the project in ways that are technically sound, responsive to user
needs and concerns, cognizant of the project's history and past
decisions, and compatible with other efforts being undertaken across
the project.  With the formation of the TSC, the technical lead role
may be supplanted or ammended by the role of a TSC chair, but this has
yet to be determined.

[Brad Chamberlain](https://github.com/bradcray) currently holds this
role, as a founding member of the Chapel project who has been
continually involved with it since the outset.  Brad has served as the
technical lead of the project since 2006, after inheriting the role
from David Callahan.


Subteam Leads
-------------

Role: As the scope of the Chapel project has grown, a number of
subteams have been spun up to focus on specific initiatives at finer
granularities.  Generally speaking, these subteam leads have a great
deal of latitude in making decisions to meet their subteams' goals,
but are expected to keep the TSC, through its chair, aware of major
decisions, particularly for those that are contentious, represent a
significant change in direction, or have the possibility of impacting
other subteams.

At present, the Chapel subteam leads are as follows:

* Community Management: [Abhishek Girish](https://github.com/agirish)
* Compiler: [Ben Harshbarger](https://github.com/benharsh)
* DevOps: [Anna Rift](https://github.com/arifthpe)
* GPU: [Engin Kayraklioglu](https://github.com/e-kayrakli)
* Performance: [Ben Harshbarger](https://github.com/benharsh)
* Runtime, Platform, and Portability: [Jade Abraham](https://github.com/jabraham17)
* User Support: [Lydia Duncan](https://github.com/lydia-duncan)


Committers
----------

Role: Committers are those who have merge-commit privileges to the
[main Chapel repository](https://github.com/chapel-lang/chapel).
These team members are expected to participate in reviewing PRs for
appropriateness, consistency, and potential security issues.
Committers are also typically expected to help with triaging failures
in the nightly regression tests on a rotating basis, though exceptions
are made for those who are also serving as the team's managers or
spending most of their time on other projects.

All PRs are expected to be reviewed by at least one committer other
than the PR's author; specifically, PRs created by a committer should
typically be reviewed by another committer.  An exception exists for
PRs considered "trivial"—so simple or straightforward that asking for
a review would feel like a waste of a colleague's time rather than a
benefit to the project.  When in doubt, a review should be requested,
and when a non-trivial PR has been merged without review, this should
be pointed out to the Committer, optionally through the TSC or Tech
Lead.  Committers who don't feel confident reviewing a PR will
typically call in additional committers to help with the review or
provide additional thoughts.  A committer who authors or merges a PR
is typically responsible for any testing fallout caused by that PR,
typically by involving the author when the PR was not theirs.  In some
cases, the reviewing committer or another volunteer may step up to
help out.

At present, the list of committers includes all of the
technical leaders listed previously, as well as:

* [Soohoon Choi](https://github.com/soohoonchoi)
* [Matt Drozt](https://github.com/MattToast)
* [Daniel Fedorin](https://github.com/DanilaFe)
* [Michael Ferguson](https://github.com/mppf)
* [John Hartman](https://github.com/jhh67)
* [Shreyas Khandekar](https://github.com/ShreyasKhandekar)
* [David Longnecker](https://github.com/dlongnecke-cray)
* [Ben McDonald](https://github.com/bmcdonald3)
* [Brandon Neth](https://github.com/brandon-neth)
* [Ahmad Rezaii](https://github.com/arezaii)
* [Oliver Alvarado Rodriguez](https://github.com/alvaradoo)
* [Andy Stone](https://github.com/stonea)
* [Michelle Strout](https://github.com/mstrout)
* [Karlon West](https://github.com/karlonw)
* [Tim Zinsky](https://github.com/tzinsky)


Community Contributors
----------------------

Role: This role describes those who have contributed code or
documentation changes that are part of the project's release
artifacts.  Such contributions are typically made by directly opening
a [pull request (PR) against the main project
repository](https://github.com/chapel-lang/chapel/pulls) containing
and explaining their proposed changes.  The commits within such PRs
must be signed by the developer to certify conformance with the
[Developer Certificate of Origin
(DCO)](https://github.com/chapel-lang/chapel/blob/main/.github/CONTRIBUTING.md).

As noted above, such PRs must be reviewed and merged by a core
contributor as a means of maintaining and improving the quality of the
code base, and to help manage any fallout that may show up afterwards,
such as failures or performance regressions in the nightly testing.

The contributor role also includes those who regularly triage nightly
correctness and performance regression test configurations, as well as
those who help develop and maintain Chapel release artifacts, such as
formulas for package managers or binary distributions.

Our project tracks the list of core and community contributors in the
main repository's
[CONTRIBUTORS.md](https://github.com/chapel-lang/chapel/blob/main/CONTRIBUTORS.md)
file, separately identifying those who have contributed to the most
recent release as a means of giving distinction to those who have been
active most recently.


Community Collaborators
-----------------------

Role: This role describes those who are active in the community and
aid us in making the Chapel language and implementation better through
suggestions, questions, feature requests, bug reports, and the like
(as opposed to through direct contributions of code or documentation).
Such contributions are invaluable to the project's effort, and Chapel
has improved immensely over time as a result of them.  We do not
currently track a list of people in this role due to the challenges in
doing so accurately and completely, but it is possible to identify
many such individuals through their interactions on GitHub and in our
[community forums](https://chapel-lang.org/community/).


Decision-Making
===============

Generally speaking, decision-making on the Chapel project is done by
the technical leadership and committers on a consensus basis, taking
the opinions of end-users into account when the decision is likely to
affect them.  Most decisions are made through GitHub issues, with more
major ones getting advertised or discussed in public weekly project
meetings.  Project-wide decisions tend to involve all active
committers.  Those that are specific to a given effort can be made by
a subteam lead and its members, keeping other developers and community
members apprised of key decisions.  When a decision cannot be made by
consensus among the developer community or appropriate subteam, it
should be escalated to the TSC for guidance or a vote.

Two flavors of votes are used by the project.  The first type is the
most common and is used to gauge the level of support for an idea or
direction, rather than being strictly binding.  In such votes, those
in the minority are typically given the opportunity to continue to
push for alternative approaches, or to concede to the majority, having
registered their opinion.  Essentially, this type of vote can be
considered a straw poll mechanism to gauge how close or far the
community is from consensus on a given topic.

The second type of vote is a vote of the TSC, which is formal,
binding, and documented in `CHARTER.md`.  In practice, these votes are
expected to be taken sparingly and reserved for matters that involve
the project governance or in cases where consensus cannot be reached
through other means.

For non-trivial decisions in language design, library APIs, or code
architecture, the project or subteam often forms an ad hoc subteam
including at least three committers to explore the topic and propose a
solution, where anyone in the broader community is encouraged to
participate if they feel interested or invested.  Once the ad hoc
subteam has reached a conclusion, it is summarized back to the full
community, typically in a GitHub issue or similarly public setting.
Generally speaking, those who did not volunteer to join the ad hoc
subteam are requested to go along with its decision, unless they have
an insight or strong reason that the proposal is
untenable—particularly if it involves factors the subteam was not, or
could not have been, aware of.  In practice, this has happened only
very rarely.

Decisions that relate to the design of the language or libraries are
captured and discussed on public [GitHub issues labeled with `type:
Design`](https://github.com/chapel-lang/chapel/issues?q=is%3Aissue%20label%3A%22type%3A%20Design%22)
as a means of soliciting input from the community. Many of these
issues are opened or requested by users directly. Decisions that are
particularly impactful to user codes are advertised directly to users
to get their feedback, by pointing them to the GitHub issues or
contacting them directly.  For some of the most impactful changes, we
run polls and work hard to involve as many users as possible in order
to avoid surprises and attempt to develop a consensus community view.
The tech lead may serve as a final decision-maker or may bring the
matter to the TSC in the event that the community can't come to a
decision.
