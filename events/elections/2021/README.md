# 2021 VOTERS GUIDE - KUBERNETES STEERING COMMITTEE ELECTION

## Purpose

The role of this election is to fill out the four (4) seats due for
reelection this year on the [Kubernetes Steering Committee]. Each elected
member will serve a two (2) year term.

## Changes

This year is the first year we will be using [Elekto] to conduct the election.
Elekto is a new application, commissioned as an internship by the CNCF.  As
well as having a new, shiny web UI, it relies entirely on GitHub Oauth for
voting, and as such does not use email at all.  Elekto also handles exceptions,
eligibility checks, and other aspects of the election.

This does mean some changes to the nomination, running, and voter exception
process, so please read below.

## Background

This election will shape the future of Kubernetes as a community and project.
While SIGs and WGs help shape the technical direction of the project, the
[Steering Committee Charter] covers the health of the project and community
as a whole. Some direct responsibilities of steering members to consider as
you are deciding whether to run or who to vote for:

* Through the chartering review process, delegate ownership of, responsibility
  for and authority over areas of the project to specific entities
* Define, evolve, and defend the non-technical vision / mission and the values
  of the project
* Charter and refine policy for defining new community groups and establish
  transparency and accountability policies for such groups
* Define and evolve project and group governance
  structures and policies
* Act as a final non-technical escalation point for any Kubernetes repository
* Request funds and other support from the CNCF (e.g. marketing, press, etc.)
* Define and enforce requirements for community groups to be in good standing
  such as having an approved charter

For more context, please see the [current steering committee backlog] or a
previous [governance meeting video] which led to this whole process.

## Eligibility

Please refer to the [Steering Committee Election Charter] for [Eligibility for candidacy]

Eligibility for voting in 2021 is defined as:

* People who had at least 50 contributions to the Kubernetes project over
  the past year, according to a snapshot taken 2021-09-15 of the data driving
  the [devstats developer activity counts dashboard][devstats-dashboard],
  who are also [Org Members].
  Contributions include GitHub events like creating issues, creating PRs,
  reviewing PRs, commenting on issues, etc. For full details see
  [the SQL query used by devstats for developer activity counts][devstats-sql].

* People who have submitted the [voter exception form] and are accepted by
  the election committee.

Corporate affiliation is applied after the election. If an organization finds
itself with too many representatives it is up to those individuals to come
to a consensus on who should serve on the committee.

### Voter exception

We *explicitly* believe that the above heuristic will be inaccurate
and not represent the entire community. Thus we provide the form
for those who have contributed to the project but may not meet the above
criteria. Acceptance of a form submission will be defined by a simple
majority vote, and the criteria used during this process will be used to
help refine further elections.

If you otherwise qualify to vote but have not yet applied for Org Membership,
then please [request an exception][voter exception form] (and please apply for
Org Membership as well).

Only contributions to projects and artifacts that fall under Steering
Committee's governance will be considered for voter exception.

Examples of contributions that would be considered:
* Slack admins who are not active in GitHub
* Code of Conduct Committee members whose actions are private by default

Examples of contributions that would NOT be considered:
* Contributions to ecosystem projects and products
* Organizing meetups or podcasts

### Schedule

<!-- While finalizing the dates in the schedule, ensure that:
- The Steering Committee and candidate Q+A occurs at a public SC meeting
  (usually a Monday).
- Deadline to submit voter exception forms and request a
  replacement ballot is ~3 days before voting closes.
- Private announcement of results to SC members is at least ~2 days
  before private announcement to all candidates.
- The interval between private announcement to all candidates and the
  public announcement is a weekend.
-->

| Date         | Event                    |
| ------------ | ------------------------ |
| August 19    | Steering Committee selects Election Committee |
| September 21 | Announcement of Election and publication of voters.md |
| September XX | Steering Committee Meeting with Q+A with the candidates and community |
| October 6    | All candidate bios due by 0000 UTC (5pm PST) |
| October 8    | Election Begins via email ballots |
| October 24   | Deadline to submit voter exception forms and request a replacement ballot |
| October 27   | Election Closes by 0000 UTC (5pm PST) |
| October 28   | Private announcement of Results to SC members not up for election |
| October 30   | Private announcement of Results to all candidates |
| November 1   | Public announcement of Results at Public Steering Committee Meeting |
| November 4?   | Election Retro |

## Candidacy Process

**Nomination**

1. If you want to stand for the election, create an issue in this GitHub repo
(kubernetes/community) with the title `Steering Committee Nomination: Your Name (@yourgithub)`.
If you want to nominate someone else, you may do so, but PLEASE talk to them
first.

2. After creating the issue, send an email to kubernetes-dev@googlegroups.com
with a link to the issue. The subject line of the email should be same as
the title of the issue. This email should encourage people to second your
nomination on GitHub, as +1s via email will not count. Here's an example email:

    Hi! I'm nominating _candidate_ for steering committee this year.
    If you are an eligible voter and think they should run, please add your +1 as
    a comment on the issue _link_ and mention the organization you work for.
    While supportive replies are very nice, only comments on the issue will count
    towards their eligibility.

3. If you wish to accept a nomination from someone else, reply to the nomination
**issue** saying something like "I accept the nomination".

4. Finally, the candidate closes the **issue** (`#NNN`) by opening a Pull Request
to add their bio (see below). The PR body must contain the text `Fixes #NNN` to 
automatically close the issue once the PR is merged.

5. Create the PR for your bio by copying the `nomination-template.md` file in
this directory, and creating a new file titled `candidate-YourName.md`.  Fill 
out all the fields in the template, but avoid making and format changes.

**Endorsement**

Once nominated, you must get the endorsement of three (3) different eligible
voters from three (3) different employers.  If you are eligible to vote
yourself, you count as one of the three. Endorsements from non-voting members
does not count towards the final count.

[Eligible voters] may endorse candidates of their choosing by replying to the
candidate's nomination **issue** saying something like "I endorse this nominee,
and I work for <COMPANY>" or "+1". Please state that you an eligible voter,
and include your employer's name so that we see can which candidates have
sufficient endorsements.

Note that **only endorsements on the GitHub issue will be considered**.
Endorsements on the nomination email will NOT be considered.

When a candidate has reached the necessary three endorsements, one of the
Election Officers will announce that on the GitHub issue.

**Running**

Eligible candidates can submit a pull request with a biography in this
directory with their platform and intent to run. This PR will copy `nomination-template.md`
to a file named `candidate-YourName.md`.  It will fill out the fields in
that template.

All biographical statements should be brief and to the point, with a guideline of around 
**300 words** total for all text. If your statement is excessively long, you 
will be asked to abbreviate it before it is merged.

Please refer to the [2020 candidate bios] for examples of content, although
the formatting should support the new templates. Biography statements are optional.

Missed deadlines by the candidates will be addressed by the election committee
on a per case basis to determine eligibility.

**Campaigning**

Please refer to the [Steering Committee Election Charter] and understand
that we care deeply about [limiting corporate campaigning]. The election
officers and members of the steering committee [pledge to recuse] themselves
from any form of electioneering.

You should be running as a "brand free" individual, based on your contribution
to the project as a member of this community, outside of whatever corporate
roles you may hold.

## Voting Process

Contributors may check their voter eligibility at any time once the election
process starts, by going to the [election app], logging in, navigating to
the 2021 election, and seeing if the screen there says that they are eligible.

If the app does not say that you are eligible, because you have worked on 
Kubernetes in a way that is NOT reflected in GitHub contributions, you can use 
the exception form built into the same app to ask to participate in the election.

Elections will be held using time-limited [Condorcet] ranking on [Elekto]. 
The most preferred candidates will be elected to the open seats.

Employer diversity is encouraged, and thus maximal representation will be
enforced as spelled out in the [Steering Committee Election Charter].

You will be ranking your choices of the candidates with an option for
"no opinion". In the event of a tie, a coin will be flipped.

The election will open for voting starting on the dates specified on the calendar
at the top of this document. You will be reminded that voting has opened by an
email to kubernetes-dev, but no email is required for you to vote.

### Officers

The Steering Committee has selected the following people as [election officers]:

- Alison Dowdney, @alisondy
- Josh Berkus, @jberkus
- Noah Kantrowitz, @coderanger

In addition, Arnaud M is serving as our Infra Team liaison for this election.

Please direct any questions via email to <election@k8s.io>.

### Decision

- First, the results are privately announced to the incumbent Steering Committee
members (who are not up for election) and all the candidates.

- The newly elected body will be publicly announced in the scheduled monthly
[public Steering Committee Meeting].

- Following the meeting, the raw voting results and winners will be published on the
[Kubernetes Blog].

For more information, definitions, and/or detailed election process, please refer to
the [Steering Committee Election Charter]

## Nominees

Nominees may be found in the [election app].

[Kubernetes Steering Committee]: https://github.com/kubernetes/steering
[Steering Committee Charter]: https://github.com/kubernetes/steering/blob/master/charter.md
[current steering committee backlog]: https://github.com/kubernetes/steering/projects/1
[governance meeting video]: https://www.youtube.com/watch?v=ltRKXLl0RaE&list=PL69nYSiGNLP1pkHsbPjzAewvMgGUpkCnJ&index=23

[Steering Committee Election Charter]: https://git.k8s.io/steering/elections.md
[Eligibility for voting]: https://github.com/kubernetes/steering/blob/master/elections.md#eligibility-for-voting
[Eligibility for candidacy]: https://github.com/kubernetes/steering/blob/master/elections.md#eligibility-for-candidacy
[limiting corporate campaigning]: https://github.com/kubernetes/steering/blob/master/elections.md#limiting-corporate-campaigning
[pledge to recuse]: https://github.com/kubernetes/steering/blob/master/elections.md#steering-committee-and-election-officer-recusal

[Condorcet]: https://en.wikipedia.org/wiki/Condorcet_method
[2020 candidate bios]: https://github.com/kubernetes/community/tree/master/events/elections/2020
[election officers]: https://github.com/kubernetes/community/tree/master/events/elections#election-officers
[Kubernetes Community Meeting]: https://github.com/kubernetes/community/blob/master/events/community-meeting.md
[Kubernetes Blog]: https://kubernetes.io/blog/

[devstats-sql]: https://github.com/cncf/devstats/blob/master/metrics/shared/project_developer_stats.sql
[devstats-dashboard]: https://k8s.devstats.cncf.io/d/13/developer-activity-counts-by-repository-group?orgId=1&var-period_name=Last%20year&var-metric=contributions&var-repogroup_name=All
[Org Members]: https://github.com/kubernetes/community/blob/master/community-membership.md
[Elekto]: https://elekto.dev
[election app]: https://election.k8s.io
