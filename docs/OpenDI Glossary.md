# OpenDI Glossary

This glossary is a cross-document resource, intended for quick reference.

# Action
 The behavior that implements a [Choice](#Choice) that has been made with the intent of achieving an [Outcome](#Outcome). Actions are enacted by [Decision Maker](#decision-maker)(s) once [Decision Making](#Decision-Making) is complete.

For example, an Action might be to budget $3,000 for marketing activities. This Action would follow after making the Choice for this specific budget, out of a range of possible budgets encapsulated in a Lever.  
Compare this to the examples given for [Choice](#Choice) and [Lever](#Lever).

Note:  
Unlike in a process model, DI does not model a *series* of actions, tasks, or choices, but rather addresses the *consequences* of Actions over which the Decision Maker has no further control after the Action is taken. In our example, we think through the consequences of the marketing budget decision during the DI process, but tasks taken to spend that money are modeled using non-DI approaches like a project schedule.

# Action-to-Outcome Exploration
 The process of using *forward simulation* in a user interface or batch setting to explore how different values of actions lead to different intermediates and outcomes.

# Application Programmer Interface (API)
 A software interface with well-defined inputs, outputs, and behavior that allows a program like a CDD simulator to use the services of another independently developed piece of software like a Technology Service implementing a Decision Asset.

# Assumption
 In decision modeling or decision simulation, an assumption is an external factor about which we have some uncertainty.

# Causal Chain
 A cause-and-effect path through a [Causal Decision Diagram](#Causal-Decision-Diagram-CDD) starting at a [Lever](#Lever) ([Action](#Action)) and ending at an [Outcome](#Outcome).

# Causal Decision Diagram (CDD)
 A diagram that shows the[Decision Elements](#Decision-Element), linked by [Causal Chains](#Causal-Chain), pertinent to a [Decision](#Decision). 

See also: [Causal Decision Model (CDM)](#Causal-Decision-Model-CDM)

For an introduction to CDD concepts, see [this article by Mark Zangari](https://www.lorienpratt.com/guest-post-connecting-decisions-to-data-a-case-study-part-2-cdd-basics/).

# Causal Model
 An analytical or software model that provides qualitative or quantitative information about a Dependency or Causal Chain.
 
 Examples include machine learning models, statistical models, and economic models. 

# Causal Decision Model (CDM)
 A computerized representation of a [Causal Decision Diagram (CDD)](#Causal-Decision-Diagram-CDD).

# Choice
 One selection from the options encapsulated in a [Lever](#Lever).

Choices are later implemented as [Actions](#Action) taken by the [Decision maker](#Decision-Maker).

For example, "we will invest $3,000 in marketing" is a choice.  
Compare this to the examples given for [Action](#Action) and [Lever](#Lever).

# Collaboration Tool
 An interactive whiteboard where a distributed team can collaborate on building a [CDD](#Causal-Decision-Diagram-CDD).

Examples include:
* [Zoom](https://www.zoom.com/en/products/online-whiteboard/)
* [Lucidspark](https://lucidspark.com/landing/create/whiteboard-software)
* [Microsoft Teams Whiteboard](https://support.microsoft.com/en-us/office/use-whiteboard-in-a-teams-meeting-26f87802-b37f-4af0-806d-af79fbfb8ae6)

# Computational Resource
Resources necessary for decision simulation, managed and used by [Decision Simulation Managers](./Roles/Decision%20Simulation%20Manager.md) and [Decision Simulation Builders](./Roles/Decision%20Simulation%20Builder.md).

Examples include:
- Hardware resources
	- GPUs
	- CPUs
- Server space
- Computation time

# Convergent Thinking
 Analytical thinking.

Compare to [Divergent Thinking](#Divergent-Thinking).

# Decision
In the context of DI, a decision is about [Actions](#Action) leading to [Outcomes](#Outcome).

Understanding a decision means understanding causal relationships in [Causal Chain](#causal-chain)s.

# Decision Approach
A high-level methodology that guides the decision-making process.

Sometimes approaches may be presented as dichotomies.  
Examples include:
- Data-driven vs. intuitive
- Autocratic vs. collaborative

Decision approaches may inform and contribute to a decision at a high level, or guide the use of certain [Decision Elements](#Decision-Element). If a particular decision approach is important for a decision, it should be documented in a [Decision Artifact](#Decision-Artifact).

# Decision Approach Register
A record linking documentation about [Decision Approaches](#Decision-Approach) with their associated [CDD](#Causal-Decision-Diagram-CDD)(s).

# Decision Artifact
Any important piece of documentation for a decision.
 
Examples include:
- [CDD](#Causal-Decision-Diagram-CDD)(s) created for the decision
- Documentation about the [Decision Approach](#Decision-Approach)
- Other [Decision Documents](#Decision-Document)

# Decision Artifacts Repositories Register
A register listing all repositories used to store [Decision Artifacts](#Decision-Artifact), what artifacts belong in which repository, who curates each repository, and instructions for submitting artifacts to the repository.

# Decision Assessment
 In the Decision Assessment process, the [Decision Team](#Decision-Team) identifies concerns and decides how they may deal with the risk each concern creates (accept/mitigate/avoid).

Areas of concern may include uncertainty, provenance, bias for [Decision Elements](#Decision-Element). It is important to consider concerns that you know exist, as well as ones you can infer exist from your [CDD](#Causal-Decision-Diagram-CDD).

# Decision Element
 An element of a [CDD](#Causal-Decision-Diagram-CDD) or [CDM](#Causal-Decision-Model-CDM).
 
Examples include:
- [Lever](#lever)
- [External](#external)
- [Outcome](#outcome)
- [Goal](#Goal)
- Constraint
- [Intermediate](#intermediate)
- [Dependency](#dependency)

# Decision Element Assessment Register
 A record of Decision Uncertainties for a [CDD](#Causal-Decision-Diagram-CDD). 

# Decision Asset
An asset that can inform a [Decision](#Decision).

Decision Assets may or may not exist before the decision making process has begun. Decision Assets can include data, information, and human knowledge, as well as statistical, machine learning, behavioral, cognitive, mathematical, and other models.

# Decision Asset Register
 A record of [Decision Assets](#Decision-Asset) for a [CDD](#Causal-Decision-Diagram-CDD). 

# Decision Customer
 The person responsible for setting up the boundaries and goals for decision making. The [Decision Team](#Decision-Team) answers to the Decision Customer, who may or may not be on the team itself.
 
 Note:  
 The [Decision Maker](#Decision-Maker) and the Decision Customer may or may not be the same. The Decision Customer requests the decision. They may or may not delegate making the decision to the Decision Team, The Decision Team Leader, or someone else, or they may retain decision making and use the Decision Team as advisors.  

Because the Decision Customer does not interact with OpenDI software in ways that are different than any other role, their role is not formally described in this document.

# Decision Document
Any documents that captures the rationale for the decision and the work done by the [Decision Team](#Decision-Team).

# Decision Frame
 Constraints, boundaries, and/or requirements for the decision that come from outside of the [Decision Team](#Decision-Team).

# Decision Maker
 The person who actually makes the decision, that is the person who at some point takes an irrevocable Action (or Actions) that begin a cause-and-effect chain that will eventually lead to Outcome(s).

This role is described in [Roles and User Stories](./Roles%20and%20User%20Stories%20Overview.md#Decision-Maker).
 
 Note:  
 The Decision Maker and the [Decision Customer](#Decision-Customer) may or may not be the same. The Decision Customer requests the decision. They may or may not delegate making the decision to separate Decision Makers, or they may retain decision making and use the Decision Team as advisors.

# Decision Making
 The process of utilizing the [CDD](#Causal-Decision-Diagram-CDD) to put in place everything the [Decision Maker(s)](#Decision-Maker) need to make the decision and take [Action](#action).
 
 This includes adding existing [Decision Assets](#Decision-Asset) to the CDD, understanding uncertainties and constraints, modeling decision behavior, and determining the [Approaches](#Decision-Approach) the Decision Maker will use to make the decision. 

# Decision Modeling
 The process of creating a [CDD](#Causal-Decision-Diagram-CDD) that models the decision, showing the chains of dependencies that lead from actions to outcomes and allowing [Decision Maker(s)](#Decision-Maker) to align about the decision rationale. 

# Decision Model
 A computational rendering of a [Causal Decision Diagram](#Causal-Decision-Diagram-CDD).

# Decision Simulation
 Understanding the dynamics of the decision model and identifying patterns of decision behavior like feedback loops and unintended consequences and understand the sensitivity of the decision to various decision elements.

# Decision Simulation Scenario Record
 A form recording the information and insights gained by simulating a Scenario.

# Decision Monitoring
 The act of observing and/or measuring attributes of [Levers](#Lever), [Intermediates](#Intermediate), and other [Decision Elements](#Decision-Element) as a decision unfolds over time. 

This is performed by the Decision Monitor, described in [Roles and User Stories](./Roles%20and%20User%20Stories%20Overview.md#Decision-Monitor).

# Decision Objective Statement
 The high-level statement of the purpose (objective) of the decision, provided by the [Decision Customer](#Decision-Customer).
 
For example, "Determine if offering an Unlimited Usage plan would be a good idea".  
Objective statements are usually vague and may need further clarification before a [Decision Model](#Decision-Model) can be created.

# Decision Optimization
 Use of software automation to apply Decision Simulation to a large number of [Scenarios](#Scenario) in order to determine the [Lever](#Lever) values that produce the best [Outcomes](#Outcome) for a given set of [External](#External) assumptions or for several sets of External assumptions.

# Decision Retrospective
 Assessment of the decision process quality and recommending process improvements as needed.

# Decision Retrospective Record
 A record of Decision Retrospective work. 

# Decision Sub-Model
 A model showing actions to outcomes that appears as part of a (or another) decision model.
 
 A Decision Sub-Model may be any existing [Decision Asset](#Decision-Asset) that shows cause and effect. It need not necessarily be expressed as a [CDD](#Causal-Decision-Diagram-CDD).

# Decision Team
 A team of persons (or a single person) responsible for implementing one or more steps of the Decision Intelligence process.
 
 Possible roles for members of the Decision Team are described in [Roles and User Stories](./Roles%20and%20User%20Stories%20Overview.md#User-Roles).
# Dependency
 A [Decision Element](#Decision-Element) representing a "causal-like" link that shows how upstream factors influence downstream factors.

Dependencies form the arrows in a [CDD](#Causal-Decision-Diagram-CDD). Dependencies can be annotated to show direction of influence or more complex relationships between the Decision Elements they connect. 

# Dependency Model
 A [Decision Asset](#Decision-Asset) that is attached to a [Dependency](#Dependency) to model characteristics of that dependency.
 
 Such characteristics may include directionality and magnitude. Examples of dependency models include machine learning models, mathematical and economic models, and human behavioral models. 

# Divergent Thinking
 Creative thinking that leads to innovation. Brainstorming is an example of divergent thinking.

Compare to [Convergent Thinking](#Convergent-Thinking).

# Elicitation
 Leading a team through the process of creating a [CDD](#Causal-Decision-Diagram-CDD).

This team may include, but is not limited to, members of the [Decision Team](#Decision-Team).

# External
 A [Decision Element](#Decision-Element) representing something that the [Decision Maker(s)](#Decision-Maker) cannot control, which nevertheless influences [Intermediates](#Intermediate) and [Outcomes](#Outcome).

 Similar to [Levers](#Lever), the effect of [Externals](#External) can be variable. While some externals represent binary occurrences (things that either happen or don't happen), some represent things that may occur to a greater or lesser degree. Within a [CDM](#Causal-Decision-Model-CDM), Externals can be modeled as sliders, enabling Decision Makers to model different possible intensities or configurations of Externals.

Examples of Externals include weather, customer behavior, competitor behavior, vendor pricing, the macro economy, etc.

# Element
 See [__Decision Element__](#Decision-Element).

# Feedback Loop
 A portion of a [CDD](#Causal-Decision-Diagram-CDD) where a [Causal Chain](#Causal-Chain) starting at a given [Decision Element](#Decision-Element) loops back to become a cause of that same Decision Element.

# Forward Simulation
 The process of determining [Outcomes](#Outcome) from specific values of [Levers](#Lever) and [Externals](#External).

This typically uses a [Causal Decision Model](#Causal-Decision-Model-CDM).

# Foundation Decision Model
 A model that can be copied, used, tailored &mdash; either in whole or in part &mdash; by others.  Some have started calling Foundation decision models "Large World Models" (LWMs), so this language here might change if the consensus shifts.

# Foundation decision model repository (FDMR)
 A computer-based resource that stores [Foundation Decision Models](#Foundation-Decision-Model).  A FDMR may be public or private, and it may be cloud-based on local.

# Goal
 A [Decision Element](#Decision-Element) which tests an [Outcome](#Outcome), often to measure success.

More generally, a Goal partitions an Outcome into a binary {true, false}.

For example, if a Decision has an Outcome of "return on invested capital, measured as the percentage (net profit on \[new product] / net of capital investment), after 18 months", then an associated Goal might be "2%".

# Ground Truth
 Fundamental or observed truth used to calibrate a system. Often, these systems are [Decision Assets](#Decision-Asset).
 
 For example, a remote sensor against a measurement on-site, "on the ground" or a machine learning model against data with known results.

# Hierarchical Decision Model
 A [CDD](#Causal-Decision-Diagram-CDD) that incorporates [Decision Sub-Models](#Decision-Sub-Model).
 
 A Hierarchical Decision Model is a linked-up decision system, which doesn't narrowly optimize for one thing while creating unintended negative consequences on other things.

# "How" Chain
An upstream [Causal Chain](#Causal-Chain) from an [Outcome](#Outcome), [Intermediate](#Intermediate), or proxy for a [Lever](#Lever) to find real Lever(s) that the Decision Maker(s) have authority over.
 
 For example, a team might suggest that to "lower the cost of parts" they should "improve relationships with our vendors." "Improve relationships with our vendors" is not a Lever; it is not an action the Team or Decision Customer can take. If you ask, "how can we improve relationships with our vendors?" someone might suggest "talk with them" and if you ask "how?" again you might eventually arrive at "schedule the VP of Production to meet every month with an executive from each of our key vendors." 

See also: ["Why" Chain](#Why-Chain)

# Intermediate
 A [Decision Element](#Decision-Element) that forms the links in [Causal Chains](#Causal-Chain) that connect [Levers](#Lever) to [Outcomes](#Outcome).
 
Intermediates answer the question of why or how a [Decision Maker](#Decision-Maker) makes a [Choice](#Choice), which leads to an [Action](#Action), resulting in an [Outcome](#Outcome).

Note that Intermediates often correspond the Key Process Indicators (KPIs) used by many organizations. DI adds a causal connection structure and integration with technology like AI and data to KPIs, which provides considerable advantages.  
Intermediates can also be thought of as leading indicators, measurements you can track to provide "early warning". For instance, you might detect a problem with the outcomes of a program that has received $1M budget spend when you have only spent the first $100K: it gives you a formal method for detecting problems early and for supporting a new plan.

# Iterative Refinement
 The process by which a [CDD](#Causal-Decision-Diagram-CDD) develops in a stepwise manner over time.
 
 CDDs typically begin as a simple diagram with a limited number of [Decision Elements](#Decision-Element), to which more elements, additional details, and connections to other [Decision Assets](#Decision-Asset) are gradually added as needed to support decision making. 

# Lever
A [Decision Element](#Decision-Element) that encapsulates a [Choice](#Choice) or set of choices that could be made to achieve an [Outcome](#Outcome).

Levers always represent [Actions](#action) that the [Decision Maker](#Decision-Maker)(s) have the ability and authority to take. While some Levers represent binary options (something a decision maker will either do or not do), and some represent a fixed set of Choices, others represent things that the decision maker can do to a greater or lesser degree. These Levers can be thought of as sliders, representing a range of choices.

For example, "amount to invest in marketing" is a Lever.  
Compare this to the examples given for Choice and Action.
# OpenDI-Compliant
 Software that is, in some sense to be crystallized at a later date, consistent with the standard described by OpenDI, including this document.

# Outcome
 A [Decision Element](#Decision-Element) that represents an expected result of the decision being modeled.

Well-defined Outcomes are measurable.  
For example, an Outcome could be "return on invested capital, measured as the percentage (net profit on \[new product] / net of capital investment), after 18 months".

A test on an Outcome is a [Goal](#Goal).
 
# Proxy Outcome or Proxy Goal
 Something that may be easier to measure or manage, but which is not a true outcome/goal.

For example, much of the world treats money as a proxy for happiness.

# Root Cause Analysis / Credit Assignment
 The process of using a decision model to work "backwards" / "upstream" in a causal chain from effects to causes.

See ["How" Chain](#How-Chain).

# Scenario
 A scenario is a set of [Choices](#Choice) for the [Levers](#Lever) in a decision, which we may examine in a [CDD](#Causal-Decision-Diagram-CDD) or simulate in a [Causal Decision Model](#Causal-Decision-Model-CDM) to see the result.

# Sensitivity Analysis
 An analysis usually done as part of [Decision Simulation](#Decision-Simulation) that determines which [Levers](#Lever), [Externals](#External), [Intermediates](#Intermediate), and [Causal Chains](#Causal-Chain) have the greatest impact on [Outcomes](#Outcome).

# Sketch Graph
 A curve that can be sketched as a hand-drawn graph, used to annotate a [Dependency](#Dependency). Sketch graphs capture human knowledge about cause and effect.

# Technology Service
 A Decision Asset implemented as a software service.

# Vicious Cycle
 A [Feedback Loop](#Feedback-Loop) that reinforces undesirable effects.

# Virtuous Cycle
 A [Feedback Loop](#Feedback-Loop) that reinforces desirable effects.

# "Why" Chain
A downstream [Causal Chain](#Causal-Chain) from a [Lever](#Lever), [Intermediate](#Intermediate), [External](#External), or [Proxy Outcome](#Proxy-Outcome-or-Proxy-Goal) to find real Outcomes that better capture the effects of a [Decision](#Decision).
 
 Asking, "why," is also a way to [Elicit](#Elicitation) new [Decision Elements](#Decision-Element) to the right-hand-side of an existing Element. "Why" chains are downstream Causal Chains from Intermediates and Proxy Outcomes to real Outcomes. 

See also: ["How Chain"](#How-Chain)
