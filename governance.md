# Community Governance

- [HEBench Home](README.md)
- [About HEBench](about_hebench.md)
- [Available Backends](hebench_published_backends.md)
- [Getting Started](quickstart_guide.md)
- Governance
  - [Revision History](#revision-history)
  - [HEBench Framework](#hebench-framework)
  - [HEBench Community Membership](#hebench-community-membership)
  - [Emeritus Status](#emeritus-status)
  - [Voting](#voting)
  - [Submissions to HEBench](#submissions-to-hebench)
- [Code of Conduct](conduct.md)

<br>

The purpose of this document is to establish the governance for the HEBench community with defined rules to guide the growth of the community.

This document DOES NOT supersede the code of conduct of HEBench.

## Revision History

This is a living document, and it is expected to be updated over time to better meet the needs of the HEBench community.

* 0.1 (Dec 7, 2021) Initial draft.
* 0.2 (Aug 22, 2022) Draft to add approved membership and submission changes (Approved by Steering Team on Aug 5, 2022)

## HEBench Framework

The HEBench Framework (HEBench) is maintained by the HEBench Organization. It is a community effort spanning industry and academia to provide a standard framework for benchmarking Homomorphic Encryption. 

To be considered official, all benchmarking results must be obtained through HEBench and validated by the HEBench community as specified in the Submissions section.

## HEBench Community Membership

### Membership Tiers

There are four tiers of membership within the HEBench Community:
* **Standard Membership**: As HEBench is a fully open-source community-led project, any individual that wants to contribute may be a Standard Member. Standard Members have direct access to the HEBench community-wide discussions and annoucements.
* **Advanced Membership**: Advanced Members are Standard Members that are also part of any of the work teams. They provide direct contribution to the HEBench Framework and Community.
* **Advisor Membership**: Advisory Members are individuals or organizations that are part of the Advisory Team. They provide expert feedback and advice to the Steering Team to aide in the decision making process.
* **Steering Membership**: Steering Members are organization representatives that are part of the Steering Team. They form the governing body of the HEBench Organization.

Membership procedures are outlined on the membership procedures page of HEBench.org.

### Teams and Roles

Here are defined the primary teams participating in HEBench community activities.

List of HEBench community teams:

* Leadership Teams
  * Steering Team
  * Advisory Team

* Work Teams
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

Moderator role: A moderator for Steering Team meetings is required. Topic to select new moderator can be brought up by Steering Team. Moderator tasks include, but not limited to, steering each team meeting with a list of topics to discuss, addressing each member on their turn, and keeping meeting minutes.

### Advisory Team

The Advisory Team is made up of significant contributors to both Homomorphic Encryption and the HEBench Communities. They provide their expertise as feedback and advice to allow the Steering Team to make educated decisions regarding HEBench. 

Advisors can sit in on the HEBench Steering meetings and may sponsor topics of discussion.

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
* Reviewing cryptographic security and implementation in submitted backends.  
  * Make sure that claimed cryptographic parameters are respected, and operations are performed correctly.
* Give feedback to Steering Team and others on topics regarding the use of cryptography and how the framework, flows and workloads map to cryptographic algorithms (not necessarily to existing algorithms, but also future proof).

## Emeritus Status

Steering Team members that are inactive (commits, GitHub comments/issues/reviews, meetings, and voting) in the past six months will be asked if they want to become Emeritus. If they do not want to become Emeritus, a second occurrence will result in an automatic status update.

Emeritus members can attend Steering meetings and propose topics, but cannot vote.

### Reinstating

Emeritus members can only be reinstated to the Steering Team by a steering vote.

## Voting

Only the Steering team has voting rights. The members of the Steering team may call a vote on any topic proposal after discussion among the members.

While discouraged, any member can abstain or not vote. However, only "yes" and "no" votes count towards a decision. Voting "no" is the only way to express opposition to a proposal. A voting result with more "yes" than "no" moves the proposal forward; otherwise, the proposal fails.

Restrictions on voting:
- There must only be one vote active on a particular topic at any time.
- A topic cannot be voted on more than once a month.
- Topic spamming or bullying of any kind is strictly forbiden.
- There must always be the options to vote "yes", "no".
- There must always be the option to abstain on a vote, and it is the default option if a member doesn't vote.

Before voting on a decision, involved members present the topic and it is discussed among the Steering team. Other teams may pass recommendations up to the Steering team for a vote or a topic. Decisions that require actions by other teams are communicated to the appropriate team to execute.


This document can only be changed by a vote where 2/3 of all the members on the Steering team vote "yes" on the changes.

## Submissions to HEBench

HEBench will be taking Backend submissions for supported workloads during a rolling submission period (e.g. the submission period is always open). Submitted Backends will undergo review by the Submissions Team and peer review by the HEBench Community. Benchmark results for the accepted Backends will be displayed in the submission section of HEBench.org. 

Submission procedures are outlined on the Submissions page of HEBench.org.

<br/>

Back to [HEBench Home](README.md)
