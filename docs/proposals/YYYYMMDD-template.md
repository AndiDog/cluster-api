---
title: Proposal Template
authors:
  - "@janedoe"
reviewers:
  - "@janedoe"
creation-date: yyyy-mm-dd
last-updated: yyyy-mm-dd
status: provisional|experimental|implementable|implemented|deferred|rejected|withdrawn|replaced
see-also:
  - "/docs/proposals/20190101-we-heard-you-like-proposals.md"
  - "/docs/proposals/20190102-everyone-gets-a-proposal.md"
replaces:
  - "/docs/proposals/20181231-replaced-proposal.md"
superseded-by:
  - "/docs/proposals/20190104-superceding-proposal.md"
---

# Title
- Keep it simple and descriptive.
- A good title can help communicate what the proposal is and should be considered as part of any review.

<!-- BEGIN Remove before PR -->
To get started with this template:
1. **Make a copy of this template.**
  Copy this template into `docs/enhancements` and name it `YYYYMMDD-my-title.md`, where `YYYYMMDD` is the date the proposal was first drafted.
1. **Fill out the required sections.**
1. **Create a PR.**
  Aim for single topic PRs to keep discussions focused.
  If you disagree with what is already in a document, open a new PR with suggested changes.

The canonical place for the latest set of instructions (and the likely source of this file) is [here](https://raw.githubusercontent.com/kubernetes-sigs/cluster-api/main/docs/proposals/YYYYMMDD-template.md).

The `Metadata` section above is intended to support the creation of tooling around the proposal process.
This will be a YAML section that is fenced as a code block.
See the proposal process for details on each of these items.

<!-- END Remove before PR -->

## Table of Contents

<!-- START doctoc generated TOC please keep comment here to allow auto update -->
<!-- DON'T EDIT THIS SECTION, INSTEAD RE-RUN doctoc TO UPDATE -->

- [Glossary](#glossary)
- [Summary](#summary)
- [Motivation](#motivation)
  - [Goals](#goals)
  - [Non-Goals/Future Work](#non-goalsfuture-work)
- [Proposal](#proposal)
  - [User Stories](#user-stories)
    - [Story 1](#story-1)
    - [Story 2](#story-2)
  - [Requirements (Optional)](#requirements-optional)
    - [Functional Requirements](#functional-requirements)
      - [FR1](#fr1)
      - [FR2](#fr2)
    - [Non-Functional Requirements](#non-functional-requirements)
      - [NFR1](#nfr1)
      - [NFR2](#nfr2)
  - [Implementation Details/Notes/Constraints](#implementation-detailsnotesconstraints)
  - [Security Model](#security-model)
  - [Risks and Mitigations](#risks-and-mitigations)
- [Alternatives](#alternatives)
- [Upgrade Strategy](#upgrade-strategy)
- [Additional Details](#additional-details)
  - [Test Plan [optional]](#test-plan-optional)
  - [Graduation Criteria [optional]](#graduation-criteria-optional)
  - [Version Skew Strategy [optional]](#version-skew-strategy-optional)
- [Implementation History](#implementation-history)

<!-- END doctoc generated TOC please keep comment here to allow auto update -->

## Glossary

Refer to the [Cluster API Book Glossary](https://cluster-api.sigs.k8s.io/reference/glossary.html).

If this proposal adds new terms, or defines some, make the changes to the book's glossary when in PR stage.

## Summary

The `Summary` section is incredibly important for producing high quality user-focused documentation such as release notes or a development roadmap.
It should be possible to collect this information before implementation begins in order to avoid requiring implementors to split their attention between writing release notes and implementing the feature itself.

A good summary is probably at least a paragraph in length.

## Motivation

This section is for explicitly listing the motivation, goals and non-goals of this proposal.

- Describe why the change is important and the benefits to users.
- The motivation section can optionally provide links to [experience reports](https://github.com/golang/go/wiki/ExperienceReports)
to demonstrate the interest in a proposal within the wider Kubernetes community.

### Goals

- List the specific high-level goals of the proposal.
- How will we know that this has succeeded?

### Non-Goals/Future Work

- What high-levels are out of scope for this proposal?
- Listing non-goals helps to focus discussion and make progress.

## Proposal

This is where we get down to the nitty gritty of what the proposal actually is.

- What is the plan for implementing this feature?
- What data model changes, additions, or removals are required?
- Provide a scenario, or example.
- Use diagrams to communicate concepts, flows of execution, and states.

[PlantUML](http://plantuml.com) is the preferred tool to generate diagrams,
place your `.plantuml` files under `images/` and run `make diagrams` from the docs folder.

### User Stories

- Detail the things that people will be able to do if this proposal is implemented.
- Include as much detail as possible so that people can understand the "how" of the system.
- The goal here is to make this feel real for users without getting bogged down.

#### Story 1

#### Story 2

### Requirements (Optional)

Some authors may wish to use requirements in addition to user stories.
Technical requirements should derived from user stories, and provide a trace from
use case to design, implementation and test case. Requirements can be prioritised
using the MoSCoW (MUST, SHOULD, COULD, WON'T) criteria.

The FR and NFR notation is intended to be used as cross-references across a CAEP.

The difference between goals and requirements is that between an executive summary
and the body of a document. Each requirement should be in support of a goal,
but narrowly scoped in a way that is verifiable or ideally - testable.

#### Functional Requirements

Functional requirements are the properties that this design should include.

##### FR1

##### FR2

#### Non-Functional Requirements

Non-functional requirements are user expectations of the solution. Include
considerations for performance, reliability and security.

##### NFR1

##### NFR2

### Implementation Details/Notes/Constraints

- What are some important details that didn't come across above.
- What are the caveats to the implementation?
- Go in to as much detail as necessary here.
- Talk about core concepts and how they relate.

### Security Model

Document the intended security model for the proposal, including implications
on the Kubernetes RBAC model. Questions you may want to answer include:

* Does this proposal implement security controls or require the need to do so?
  * If so, consider describing the different roles and permissions with tables.
* Are their adequate security warnings where appropriate (see https://shostack.org/files/papers/ReederEtAl_NEATatMicrosoft.pdf for guidance).
* Are regex expressions going to be used, and are their appropriate defenses against DOS.
* Is any sensitive data being stored in a secret, and only exists for as long as necessary?

### Risks and Mitigations

- What are the risks of this proposal and how do we mitigate? Think broadly.
- How will UX be reviewed and by whom?
- How will security be reviewed and by whom?
- Consider including folks that also work outside the SIG or subproject.

## Alternatives

The `Alternatives` section is used to highlight and record other possible approaches to delivering the value proposed by a proposal.

## Upgrade Strategy

If applicable, how will the component be upgraded? Make sure this is in the test plan.

Consider the following in developing an upgrade strategy for this enhancement:
- What changes (in invocations, configurations, API use, etc.) is an existing cluster required to make on upgrade in order to keep previous behavior?
- What changes (in invocations, configurations, API use, etc.) is an existing cluster required to make on upgrade in order to make use of the enhancement?

## Additional Details

### Test Plan [optional]

**Note:** *Section not required until targeted at a release.*

Consider the following in developing a test plan for this enhancement:
- Will there be e2e and integration tests, in addition to unit tests?
- How will it be tested in isolation vs with other components?

No need to outline all of the test cases, just the general strategy.
Anything that would count as tricky in the implementation and anything particularly challenging to test should be called out.

All code is expected to have adequate tests (eventually with coverage expectations).
Please adhere to the [Kubernetes testing guidelines][testing-guidelines] when drafting this test plan.

[testing-guidelines]: https://git.k8s.io/community/contributors/devel/sig-testing/testing.md

### Graduation Criteria [optional]

**Note:** *Section not required until targeted at a release.*

Define graduation milestones.

These may be defined in terms of API maturity, or as something else. Initial proposal should keep
this high-level with a focus on what signals will be looked at to determine graduation.

Consider the following in developing the graduation criteria for this enhancement:
- [Maturity levels (`alpha`, `beta`, `stable`)][maturity-levels]
- [Deprecation policy][deprecation-policy]

Clearly define what graduation means by either linking to the [API doc definition](https://kubernetes.io/docs/concepts/overview/kubernetes-api/#api-versioning),
or by redefining what graduation means.

In general, we try to use the same stages (alpha, beta, GA), regardless how the functionality is accessed.

[maturity-levels]: https://git.k8s.io/community/contributors/devel/sig-architecture/api_changes.md#alpha-beta-and-stable-versions
[deprecation-policy]: https://kubernetes.io/docs/reference/using-api/deprecation-policy/

### Version Skew Strategy [optional]

If applicable, how will the component handle version skew with other components? What are the guarantees? Make sure
this is in the test plan.

Consider the following in developing a version skew strategy for this enhancement:
- Does this enhancement involve coordinating behavior in the control plane and in the kubelet? How does an n-2 kubelet without this feature available behave when this feature is used?
- Will any other components on the node change? For example, changes to CSI, CRI or CNI may require updating that component before the kubelet.

## Implementation History

- [ ] MM/DD/YYYY: Proposed idea in an issue or [community meeting]
- [ ] MM/DD/YYYY: Compile a Google Doc following the CAEP template (link here)
- [ ] MM/DD/YYYY: First round of feedback from community
- [ ] MM/DD/YYYY: Present proposal at a [community meeting]
- [ ] MM/DD/YYYY: Open proposal PR

<!-- Links -->
[community meeting]: https://docs.google.com/document/d/1ushaVqAKYnZ2VN_aa3GyKlS4kEd6bSug13xaXOakAQI/edit#heading=h.pxsq37pzkbdq
