# Description of the taxonomy terms

> For now this is just a dump of the paper. It needs to be cleaned/reviewed

--- 

- [Problem](#problem)
  - [Cause](#cause)
    - [Agent](#agent)
    - [Technology](#technology)
    - [Lifecycle phase](#lifecycle-phase)
    - [Temporality](#temporality)
  - [Impact](#impact)
    - [Type](#type)
    - [Lifecycle phase](#lifecycle-phase-1)
    - [Nature](#nature)
- [Countermeasure](#countermeasure)
  - [Intervention](#intervention)
    - [Agent](#agent-1)
    - [Action](#action)
      - [Domain](#domain)
      - [Sustainable R's](#sustainable-rs)
    - [Lifecycle phase](#lifecycle-phase-2)
    - [Temporality](#temporality-1)
  - [Impact](#impact-1)
- [Evidence](#evidence)
  - [Data](#data)
  - [Metrics](#metrics)
  - [Angle](#angle)
  - [Reasoning](#reasoning)
  - [Boundaries](#boundaries)

---

## Problem

### Cause

#### Agent

Environmental problems related to technology are always connected to human activity in some way, as human agents either make or use technology. 
Often, different agents may contribute to a given problem, e.g., users, designers, engineers, deployers, providers, importers, or policy-makers. 
Some agents are always present: without users, computing systems serve no purpose; without developers and engineers, they would not exist. Others may only be relevant in specific contexts. 
At the same time, the same or other agents may also play a role in mitigating these problems.

Agents may cause problems if they are either

|Term|Description|
|:---|:---|
|**Uninformed** | Agents may lack the knowledge needed to recognize their role in causing environmental harm. For instance, software developers may not be aware of the energy implications of their design choices.|
|**Unmotivated**| Even when the relevant information is available, some agents may not care sufficiently, may prioritize other goals, or even oppose the sustainable actions. This can manifest in overuse of digital services, disregard for efficiency in development, or neglect of sustainability in procurement and deployment choices.|
|**Unable**|Sometimes, agents are motivated and aware, yet lack the power to act. Users may face systems with no sustainable alternatives or settings. Developers may be constrained by organizational decisions or lack the authority to change core infrastructure.|

#### Technology

We make a distinction between physical `hardware` and digital `software` products—not because one can exist
without the other, but rather because many anecdotes have a clear
focus on one or the other. Both hardware and software can suffer
from several sustainability `issues`, including

> TODO: do not forget to update the labels.

- `Unsustainably Operated` Using dirty and/or non-renewable energy.
- `Bloated` More powerful than needed for its use. Unused software
features increase binary sizes and hence both download
times and storage needs. Unused hardware features have
an embodied footprint that is never amortized.
- `with Questionable Functionality` Contains functions that leverage,
possibly unintentionally, resource-intensive technologies,
e.g., generative AI or hyperledgers.
- `with Short Lifetime` Not used long enough to amortize the environ-
mental production costs. For hardware, this can be caused
by low-quality production or use-case specificity (i.e., not usable for other, comparable use cases). For software, this
can be caused by planned obsolescence or end-of-life due
to company policy decisions.
- `with High Environmental Footprint` Produced under questionable
circumstances and extensively using rare, non-renewable
materials and non-renewable energy.
- `Stagnating` Innovation is blocked by habits, regulations, or loss
of interoperability. For instance, if a small potential effi-
ciency gain requires throwing away significant amounts of
hardware in exchange.

#### Lifecycle phase

A sustainability problem usually manifests at one or several of the lifecycle phases of a computing system.

- `Design` involves decisions that define and constrain the system.
- `Production (Hardware)` is where the embodied footprint is caused.
- `Deployment (Software)` is where software runs on hardware.
- `Operation` is where work is done, causing the operational footprint.
- `Decommission` discards stored data/software, stops using hardware.

#### Temporality 

Beyond identifying the lifecycle phase
in which a problem originates, it is also useful to consider when
the underlying cause occurs. Some problems stem from one-off
decisions, such as hardware design choices or infrastructure in-
vestments, while others arise from ongoing practices, like usage
patterns or operational defaults. Also, if the cause lies in the past,
post-hoc mitigation of its effects is the only option; if it is still on-
going, there may be a chance to stop it. Timing also matters for the
impact: some effects occur immediately, while others accumulate
slowly or only become visible after a delay.

### Impact

#### Type 

We adopt the classification of technology impact
from Hilty and Aebischer [18], which distinguishes:

- `Direct` or lifecycle impacts result from the resource used to manufacture, operate, and recycle a computing system.
- `Indirect` or enabling impacts capture the external effects from using a computing system. Those can either be negative (e.g., a
software update causing hardware obsolescence) or posit-
ive (e.g., heating control resulting in reduced energy usage).
- `Systemic` or structural impacts are the consequence of persistent
changes observable at the macro level, such as behavior
change. A rebound effect [20] is an example of negative
systemic impacts; there could be positive ones too.

Systemic impacts are challenging to assess, as they often arise from
complex interdependencies, long-term feedback loops, or social
and economic dynamics far beyond the control of any single agent.

#### Lifecycle phase

The cause(s) of a problem may stem from a different lifecycle phase than those were the impact occurs, which is why `lifecycle phase` appears both under [cause](#cause) and [impact](#impact).

See [above](#lifecycle-phase) for the lifecycle phases description.

> TODO: add an example
 
#### Nature

Plain text description of the nature of the impact; that is, what the actual impact _is_.

## Countermeasure

### Intervention

#### Agent

The agents capable of
performing countermeasures are, in principle, the same as those
involved in causing sustainability problems—users, developers, en-
gineers, providers, policy-makers, and others. However, not all 
agents who contribute to a problem are equally positioned to inter-
vene. Performing a countermeasure requires not just involvement,
but also the capacity to act effectively and responsibly.
Some agents are particularly well-situated to drive change due to
their structural role or access to key decisions—for instance, infra-
structure providers, product owners, or regulatory bodies. Others
may play a supporting or enabling role, such as end users who re-
spond to better defaults, or engineers who highlight opportunities
for improvement. In many cases, effective countermeasures depend
on coordination across multiple agent types. Thus, while any agent
can in principle contribute to a more sustainable computing ecosys-
tem, their actual capacity to intervene varies widely. Recognizing
these differences is essential when evaluating the feasibility, scope,
and responsibility of potential countermeasures. In any case, agents
need to be informed, motivated, and able to make a change.

#### Action

##### Domain

Similar to other fields of climate action, there are several ways to achieve change:

- `Technological` leverages scientific or engineering inventions to
apply changes in (ideally widely deployed) technology.
- `Regulatory` is caused by legislators or other interest groups passing
regulations that legally enforce changes.
- `Behavioral` leaves it to individual agents to decide to change, inde-
pendently of regulations or technology.

##### Sustainable R's

In Zero Waste communities, one often reads
about various forms of five R’s (uncredited). They represent an
order of guide verbs to agents, who want to act more sustainably.
Earlier verbs have an impact on earlier phases of product / service
lifecycles and hence potentially largest impact. Here, we present a
variant fine-tuned to sustainable computing, the seven R’s:

- `Rethink` your current use of computing.
- `Refuse` additional / extended products and services.
- `Reduce` your use of computing.
- `Reuse` obsolete but functional hardware in a different use case.
- `Repair` broken hardware / software to continue its original use.
- `Recycle` by extracting resources via manmade processing cycles.
- `Rot` to give resources back to natural processing cycles.

#### Lifecycle phase

An intervention may target one or several
of the system’s lifecycle phases, which will often be
the same as where the problem manifests, but not always. E.g., users
may be uninformed about the high operational cost of a system they
use; a countermeasure is to introduce “efficiency labels” [2, 40] to
create pressure during the design of future system generations.

See [above](#lifecycle-phase) for the lifecycle phases description.

#### Temporality

Just as problems can arise from
past decisions or ongoing practices, countermeasures can be either
reactive or preventive. Some may address the lingering effects of
past actions, while others aim to stop current practices or avoid
future harm. Timing also influences effectiveness: early interven-
tion can prevent long-term damage, while delayed action may only soften its consequences. In cases where impacts unfold slowly or
with delay, timely countermeasures are important even if the prob-
lem is not yet fully visible.

### Impact

The (hopefully positive) impact of a countermeasure can be described exactly as the negative impact of a problem.

See [above](#impact) for the description.

## Evidence

### Data

Naturally, observations in the
real world (e.g., measurements) and models (e.g., analytical projec-
tions) are the basis for unveiling problems and validating counter-
measures.

### Metrics

Most sustainability questions are multi-dimensional
by nature. For example, opting for a heat-pump instead of a water-
based cooling system will increase energy use but decrease water
use; those two dimensions are not directly comparable.

... 

> TODO: to be completed

### Angle

When assessing the impact of a system,
one may approach the problem from two opposite directions.

- `Top-Down` One may consider the entire footprint of a system, e.g.,
a datacenter, and divide it by the total output of the system.
This approach requires few measurements (e.g., the total en-
ergy consumed by a datacenter) but also lacks granularity;
i.e., it obfuscates the relative impact of the different parts of
the system. For example, one can easily derive an average
energy cost per query by dividing the total by the number
of queries served in a year, which will include not only
the system serving the query, but also other infrastructure
costs, such as cooling. Accounting is usually done this way.
- `Bottom-Up` Conversely, one can start from the bottom, measure
all the individual costs, and add them up to get the sys-
tem’s total. This provides a more fine-grained view on the
respective importance of the system’s parts. This likely un-
derestimates the total footprint, as one is bound to forget
or be unable to measure some parts.

Differentiating those two approaches is important as they serve
different purposes and are not inter-exchangable. Top-down is
appropriate for accounting while bottom-up helps performance
optimization by identifying the precise contributions of different
system parts in its footprint.

### Reasoning

When assessing the impact of countermeasures, there are two fundamentally different ways:

- `Attributional` One may ask: What is the footprint of system X ?
Or, who is responsible for that footprint? This is an attri-
butional reasoning, which is essentially accounting—it is
about getting the total number right.
- `Consequential` Conversely, one may wonder what is the impact of
an action Y ? Consequential reasoning aims to assess the
respective benefits of alternatives. The difference between
action A and action B is more important than the total.

### Boundaries

Impact assessment studies must clearly identify
their boundaries; that is, where does the system we study end? It is
particularly important for consequential reasoning: a given action
may have positive consequences within one’s boundary, but negat-
ive ones outside. A current example is carbon-aware computing,
which may reduce the carbon footprint of a cloud provider but
leads to an increase in the footprint for the power grid. While it is virtually impossible to account for all externalities for a true global net impact assessment, one must be aware and mindful of potential consequences outside of one’s system boundaries.