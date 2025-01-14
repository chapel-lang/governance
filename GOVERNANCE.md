Governance of the Chapel Project
================================

This file describes the current governance of the Chapel Language
project, covering both the language's definition and the code base
that implements its compiler, library modules, and runtime.  It was
last updated in January 2025.

Over time, we anticipate improving the Chapel project's governance,
with the goal of making it more of a community-governed project.  If
this topic is of interest to you, or you would like to play a role in
that transition or its result, please let us know.  If you have
specific requests with respect to how the project is governed, please
feel encouraged to capture those in an issue on this repository, or to
[reach out to the community](https://chapel-lang.org/community/).


Technical Leadership
--------------------

**Technical Lead:** [Brad Chamberlain](https://github.com/bradcray)

Role: Generally speaking, the role of the project technical lead has
been to help guide decisions for the project in ways that are
technically sound, responsive to user needs and concerns, cognizant of
the project's history and past decisions, and compatible with other
efforts being done across the project.

As a founding member of the Chapel project who has been continually
involved with it since the outset, Brad has served in this role since
2006 after inheriting it from David Callahan.  Generally speaking,
Brad strives to follow the direction of the community when that is
clear.  He has the ability to serve as an authority in decision-making
cases, as noted [below](#decision-making).


**Subteam Leads**

Role: As the scope of the Chapel project has grown, a number of
subteams have been spun up to focus on specific initiatives at finer
granularities.  Generally speaking, these subteam leads have a great
deal of latitude in making decisions to meet their subteams' goals,
but are expected to keep the technical lead aware of major decisions,
particularly for those that are contentious, represent a significant
change in direction, or have the possibility of impacting other
subteams.

At present, the Chapel subteam leads are as follows:

* Community Management: [Brandon Neth](https://github.com/brandon-neth)
* Compiler: [Ben Harshbarger](https://github.com/benharsh)
* DevOps: [Tim Zinsky](https://github.com/tzinsky)
* GPU: [Engin Kayraklioglu](https://github.com/e-kayrakli)
* Performance: [Andy Stone](https://github.com/stonea)
* Runtime, Platform, and Portability: [John Hartman](https://github.com/jhh67)
* User Support / Language Stabilization: [Lydia Duncan](https://github.com/lydia-duncan)


Committers
----------

Role: Committers are those who have merge-commit privileges to the
[main Chapel repository](https://github.com/chapel-lang/chapel).
These team members are expected to participate in reviewing PRs for
appropriateness, consistency, and potential security issues.
Committers are also typically expected to help with triaging failures
in the nightly regression tests on a rotating basis, though exceptions
are made for those who are also serving as managers on the team or
spending most of their time on other projects.

All PRs are expected to be reviewed by at least one committer other
than the PR's author; specifically, PRs created by a committer should
typically be reviewed by another committer.  An exception exists for
PRs considered "trivial"—so simple or straightforward that asking for
a review would feel like a waste of a colleague's time rather than a
benefit to the project.  When in doubt, a review should be requested.
Committers who don't feel confident reviewing a PR will typically call
in additional committers to help with the review or provide additional
thoughts.  A committer who authors or merges a PR is typically
responsible for any testing fallout caused by that PR, typically by
involving the PR's author when it was not theirs.  In some cases, the
reviewing committer or another volunteer may step up to help out.

At present, the list of committers includes all of the
technical leaders listed previously, as well as:

* [Jade Abraham](https://github.com/jabraham17)
* [Soohoon Choi](https://github.com/soohoonchoi)
* [Matt Drozt](https://github.com/MattToast)
* [Daniel Fedorin](https://github.com/DanilaFe)
* [Michael Ferguson](https://github.com/mppf)
* [Abhishek Girish](https://github.com/agirish)
* [Shreyas Khandekar](https://github.com/ShreyasKhandekar)
* [Vass Litvinov](https://github.com/vasslitvinov)
* [David Longnecker](https://github.com/dlongnecke-cray)
* [Ben McDonald](https://github.com/bmcdonald3)
* [Ahmad Rezaii](https://github.com/arezaii)
* [Anna Rift](https://github.com/riftEmber)
* [Elliot Ronaghan](https://github.com/ronawho)
* [Michelle Strout](https://github.com/mstrout)
* [Karlon West](https://github.com/karlonw)


Decision-Making
---------------

Generally speaking, decision-making on the Chapel project is done by
the technical leadership and committers on a consensus basis, taking
the opinions of end-users into account when the decision is likely to
affect them.  Project-wide decisions tend to involve all technical
leads and committers, while those that are specific to a given effort
can be made by a subteam lead and its members, keeping the technical
lead apprised of key decisions.

Votes are rarely taken in a binding manner, but are often used to
gauge the level of support for an idea or direction.  In such votes,
those in the minority are typically given the opportunity to continue
to push for alternative approaches, or to concede to the majority,
having registered their opinion.

For non-trivial decisions in language design, library APIs, or code
architecture, the project or subteam typically forms an ad hoc subteam
including at least three committers to explore the topic and propose a
solution, where anyone on the broader team is encouraged to
participate if they feel interested or invested.  Once the ad hoc
subteam has reached a conclusion, it is summarized back to the full
team.  Generally speaking, those who did not volunteer to join the ad
hoc subteam are expected to go along with its decision, unless they
have an insight or strong reason that the proposal is
untenable—particularly if it involves factors the subteam was not, or
could not have been, aware of.  In practice, this has happened only
very rarely.

Decisions that relate to the design of the language or libraries are
captured and discussed on public [GitHub
issues](https://github.com/chapel-lang/chapel/issues?q=is%3Aissue%20label%3A%22type%3A%20Design%22)
as a means of soliciting input from the community. Many of these
issues are opened or requested by users directly. Decisions that are
particularly impactful to user codes are advertised directly to users
to get their feedback by pointing them to the GitHub issues or
contacting them directly.  For some of the most impactful changes, we
have run polls and worked hard to involve as many users as possible in
order to avoid surprises and attempt to develop a consensus community
view.  The technical lead may serve as a final decision-maker in the
event that the community can't come to a decision.  In extreme cases,
the technical lead may veto a decision, though it is expected that
this would be used only very rarely.



Community Contributors
----------------------

Role: This role describes those who have contributed code or
documentation changes that are part of the project's release
artifacts, typically by directly opening a [pull request (PR) against
the main project
repository](https://github.com/chapel-lang/chapel/pulls) that contains
their commits to improve the code base and/or documentation.  The
commits within a PR must be signed off to certify conformance with the
[Developers Certificate of Origin
(DCO)](https://github.com/chapel-lang/chapel/blob/main/.github/CONTRIBUTING.md).

As noted above, such PRs must be reviewed and merged by a core
contributor as a means of maintaining and improving the quality of the
code base, and to help manage any fallout that may show up afterwards,
such as failures or performance regressions in the nightly testing.

Our project tracks the list of core and community contributors in the
main repository's
[CONTRIBUTORS.md](https://github.com/chapel-lang/chapel/blob/main/CONTRIBUTORS.md)
file, separately identifying those who have contributed to the most
recent release as a means of giving distinction to those who have been
active most recently.


Community Collaborators and Users
---------------------------------

Role: This role describes those who are active in the community and
aid us in making the Chapel language and implementation better through
suggestions, questions, feature requests, bug reports, and the like
(rather than through direct contributions of code or documentation).
Such contributions are invaluable to the project's effort, and Chapel
has improved immensely over time as a result of them.  We do not
currently track a list of people in this role due to the challenge in
doing so, but it is easy to identify many such individuals through
their actions on GitHub and in our [community
forums](https://chapel-lang.org/community/).
