# HEBench Community Governance

The purpose of this document is to establish the initial governance for HEBench community with defined rules that we can adhere to during the initial stages of its creation.

## Revision History

This is a living document, and it is expected to be updated over time to better meet the needs of the HEBench community.

* 0.1 (Dec 7, 2021) Initial draft.

## GitHub Teams

The following are the existing GitHub teams with their purpose and permissions.

Name &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; | Permissions | Purpose
-|-|-
**hebench-dev** | Can clone, read any branch, and write/push to their own branches. Can manage PRs (Pull Requests) and issues. | Developer access to HEBench org. All new members start here.
**hebench-collab** | All hebench-dev permissions + can approve PRs (per repo using CODEOWNERS) and start CI (Continuous Integration). | Free up maintainers from constantly doing code reviews for all repos.
**hebench-maintain** | Full administration access to all repos. | Ability to change repo settings, and to perform all tasks from other GitHub teams.

Meritocracy based, members in **hebench-dev** can be upgraded to **hebench-collab** to be able to approve PRs and fire off CI on a per-governance team basis.

## HEBench Framework

HEBench framework (HEBench) is the HEBench community tool. To be considered official, all benchmarking results must be obtained through HEBench and validated by the HEBench community as specified later.

## Teams & Roles

Here are defined the primary teams participating in HEBench community activities.

List of HEBench community teams:

* Steering Team

* Framework Development Team

* Pathfinding Team

* Submission Team

Note: individuals may participate in multiple teams.

### Steering Team

Steering team is the governing body of the HEBench community. All final decisions are made by this team.

The philosophy is to keep leadership mostly technical, with an emphasis on hands-on-involvement. Favor data-driven decisions, design simplicity, rapid development and iteration, and focus on real user value.

Membership to the Steering Team is affiliation based, where each organization has a single voice. This is, when making decisions, every organization has a single vote of equal weight (see Voting). It is up to the Steering Team to decide who is recognized as an organization.

The Steering Team shall approve all changes in membership to all HEBench community teams, and maintain a document listing each team members' names, contact information, affiliation, date of first inclusion into the team, and other notes.

Founding organizations will be the initial members of the Steering Team. New members will be approved by the current steering team.

Moderator role: A moderator for Steering Team meetings is required. Initial moderator will be initial founder (Intel Corporation). Topic to select new moderator can be brought up by Steering Team. Moderator tasks include, but not limited to, steering each team meeting with a list of topics to discuss, addressing each member on their turn, and keeping meeting minutes.

**Action** (to be edited once completed): Frequency of Steering Team meetings and voting sessions must be selected during the first Steering Team meeting.

### Framework Development Team

This team’s tasks are related to maintaining and improving the HEBench framework.

Tasks:

* Add features that enhance utility, quality, etc.
* Propose changes to the framework.  
    Moderate to major changes to the framework must be approved by Steering team (these are changes that will affect user experience, changes to interface and behavior of framework).
* Implement new workloads or categories into HEBench frontend.
* Offer feedback to the Pathfinding and Steering teams regarding workloads, categories, and/or methodologies.

### Pathfinding Team

Pathfinding team is responsible for identifying and proposing new Workloads, categories or testing methodologies that may become part of the standard testing framework. These are based on field experience, user feedback, commonly seen use-cases, etc.

Members of this team must work with cryptography experts and framework development and submission teams to refine the Workload, Category or Testing Methodology to be proposed (based on whether it is feasible, and what parameters make sense, etc.). Once proposed, this team must research and prepare a report on the proposal itself, such as inputs, outputs, parameters, algorithm, and other details required for efficient and rapid implementation by the development teams to correctly deploy into the framework.

### Submissions Team

This team is responsible for reviewing and validating submitted backends. While anyone can use HEBench and create their own backends, and publish results, only results and backends reviewed by this team will be recognized as official HEBench backends.

This team has the following tasks:

* Review implementation of submitted backends for correctness in the framework flow (make sure that each stage is performing the correct task, and not cheating in other stages).
* Validating cryptographic security and implementation in submitted backends.  
    Make sure that claimed cryptographic parameters are respected, and operations are performed correctly.
* Give feedback to Steering Team and others on topics regarding the use of cryptography and how the framework, flows and workloads map to cryptographic algorithms (not necessarily to existing algorithms, but also future proof).

## Emeritus Status

Steering Team members that are inactive (commits, GitHub comments/issues/reviews, meetings, and voting) in the past six months will be asked if they want to become Emeritus. If they do not want to become Emeritus, a second occurrence will result in an automatic status update.

Emeritus members can attend Steering meetings and propose topics, but cannot vote.

### Reinstating

Emeritus members can only be reinstated to the Steering Team by a steering vote.

## Voting

Only the Steering team has voting rights. The members of the Steering team may also call a vote on any topic. A topic cannot be voted on more than once a month, or if there have been new developments on that particular topic.

All decisions are reached by majority voting. While any member can abstain, only "yes" and "no" votes count towards a decision.

Before voting on a decision, involved members present the topic and it is discussed among the Steering team. Other teams may pass recommendations up to the Steering team for a vote or a topic. Decisions that require actions by other teams are communicated to the appropriate team to execute.

**Action** (to be edited once completed): Voting platform(s) and the number of days required for a vote to remain open must be decided during the first Steering meeting.

This document can only be changed by Steering Team on a 2/3 vote.
