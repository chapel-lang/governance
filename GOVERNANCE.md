# Governance of the Chapel Project

This file describes the current governance of the Chapel Language
project, covering both the language's definition and the code base
implementing its compiler, library modules, and runtime.  It was last
updated in January 2025.

We anticipate improving the Chapel project's governance, with the aim
of making it more of a community-governed project, over time.  If this
is of interest to you, please let us know.  If you have specific
requests with respect to how the project is governed, please open an
issue on this repository.


## Technical Leadership

**Technical Lead:** [Brad Chamberlain](bradcray)

Role: Generally speaking, the role of the project technical lead is to
help guide technical decisions for the project in ways that are
technically sound, responsive to user needs and concerns, cognizant of
the project's history and past direction, and compatible with other
decisions being made across the project.  As a founding member of the
Chapel project who has been continually involved with it since the
outset, Brad has served in this role since ~2006, making him something
like the project's BDFL.


**Subteam Leads**

Role: As the scope of the Chapel project has grown, a number of
subteams have been formed to focus on specific initiatives at finer
granularities.  Generally speaking, these subteam leads have a great
deal of latitude in making decisions supporting their goals, but are
encouraged to keep the technical lead in the loop, particularly for
decisions that are contentious, represent a significant change in
direction, or have the possibility of impacting other subteams.

At present, the subteam leads are as follows:

* Community Management: [Brandon Neth](https://github.com/brandon-neth)
* Compiler: [Ben Harshbarger](https://github.com/benharsh)
* DevOps: [Tim Zinsky](https://github.com/tzinsky)
* GPU: [Engin Kayraklioglu](e-kayrakli)
* Performance: [Andy Stone](https://github.com/stonea)
* Runtime / Platform / Portability: [John Hartman](https://github.com/jhh67)
* User Support / Language Stabilization: [Lydia Duncan](https://github.com/lydia-duncan)


**Core Contributors**

Role: Core contributors are those who have merge privileges to the
[main Chapel repository](https://github.com/chapel-lang/chapel).
These team members are expected to participate in reviewing PRs for
appropriateness, consistency, and potential security issues.  Core
contributors are also typically expected to help with triaging
failures in the nightly regression tests, though exceptions are often
made for core contributors who are also serving as managers on the
team, focusing on DevOps or Build/Test/Release issues, or spending
most of their time on other projects.

All PRs are expected to be reviewed by at least one core contributor
other than the PR's author; specifically, PRs created by a core
contributor should typically be reviewed by another core contributor.
An exception exists for PRs considered "trivial"—so simple or
straightforward that asking for a review would feel like a waste of a
colleague's time rather than a benefit to the project.  When in doubt,
a review should be requested.  Core contributors who don't feel
confident reviewing a PR will typically call in additional core
contributors to help with the review or provide additional thoughts.
A core contributor who authors or merges a PR is typically responsible
for any testing fallout caused by that PR, typically by involving the
PR's author.  In some cases, the reviewing core contributor or another
volunteer may step up to help out.

At present, the list of core contributors includes all of the
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


** Decision-Making **

Generally speaking, decision-making on the Chapel project is done by
the technical leadership and contributors in this section on a
consensus basis, taking the opinions of end-users into account when
the decision is likely to effect them.

For non-trivial internal decisions, or initial explorations into
public decisions, the project typically forms an ad hoc subteam of at
least three core contributors to explore the topic and propose a
solution, where anyone on the team is encouraged to participate if
they are interested.  Once the subteam has reached a conclusion, it is
summarized back to the full team.  Generally speaking, those who did
not join the subteam are expected to go along with the subteam's
decision, unless they have an insight or strong reason that the
proposal is untenable, particularly if it involves factors the subteam
was unaware of.  In practice, this happens only very rarely.

Decisions that relate to the design of the language or libraries are
captured and discussed on public [GitHub
issues](https://github.com/chapel-lang/chapel/issues?q=is%3Aissue) as
a means of soliciting input from the community. Many of these issues
are opened or requested by users directly. Decisions that are
particularly impactful to user codes are advertised directly to users
to get their feedback by pointing them to the GitHub issues or
contacting them directly.  For some of the most impactful changes, we
have run polls and worked hard to involve as many users as possible in
order to avoid surprises and attempt to develop a consensus community
view.


## Community Contributors

Role: This role describes those who have contributed code or
documentation changes that are part of the project's release
artifacts, typically by directly opening a [pull request (PR) against
the main project
repository](https://github.com/chapel-lang/chapel/pulls) that contains
their commits to improve the code base or documentation.  The commits
within a PR must be signed off to certify conformance with the
[Developers Certificate of
Origin](https://github.com/chapel-lang/chapel/blob/main/.github/CONTRIBUTING.md).

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


## Community Collaborators and Users

Role: This role describes those who are active in the community and
aid us in making the Chapel language and implementation better through
suggestions, questions, feature requests, corrections, and the like
rather than through specific contributions of code and documentation.
We greatly value such contributions to the effort, and our project has
improved immensely as a result of it.  We do not currently track a
list of people in this role because of its ephemeral nature, but it is
not difficult to find such contributors in our [community
forums](https://chapel-lang.org/community/), present and past.
