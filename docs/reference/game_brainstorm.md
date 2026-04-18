# After Them -- Space Archaeology Game

## Brainstorming Notes — April 2026

_This document summarizes several brainstorming sessions for a browser-based space game inspired by Stars!, aimed at
capturing the same sense of discovery, logistics, and incremental mastery — without being a clone or a conventional 4X
game. These are working ideas, not final decisions._

---

## Core Design Philosophy

The game deliberately subverts the traditional 4X formula (eXplore, eXpand, eXploit, eXterminate). The first three
pillars are embraced; the fourth is replaced entirely. Instead of extermination, the pressure comes from _entropy_ — the
galaxy itself is the antagonist.

The three qualities to preserve from Stars!:

- **Discovery** — finding things should feel like unwrapping a gift, not sampling a random table
- **Logistics** — moving resources and managing networks is satisfying in itself, not just a means to an end
- **Incremental mastery** — progress should feel earned, and each step should open new possibilities

The game is intended primarily as a single-player experience. Visual style is explicitly not a priority — the game is
the important part.

### What the Game Is Not

- Not a 4X game in the conventional sense
- Not narrative-heavy — the game is intentionally abstract and systemic, avoiding the design burden of authored story
- There are no other factions - the other ministries in the player's own government do the same sort of thing
- Not combat-focused (all the actors are part of the same government, working together, if imperfectly)

---

## The Player's Role: Minister of Exploration and Natural Resources

### Government Structure

The player's civilization is governed by a small number of ministries, each with a distinct mandate. The player controls
one of them. The others are abstractions — the player interacts with them through requests and receives from them
through dispatches, but does not manage their internal operations.

The ministries:

**Ministry of Exploration and Natural Resources** — the player's ministry. Mandate: survey the galaxy, recover and study
artifacts from the prior civilization, and locate and extract resources. These three activities are in natural tension
with each other and compete for the same ships, specialists, and logistics bandwidth.

**Ministry of Fleet and Engineering** — builds things. Ships, outposts, infrastructure. Receives findings from
Exploration (via Science) and turns them into new capabilities. Fulfills requisitions from the player on a timeline
determined by capacity and priority. Fleet's capacity is finite and shared — Settlement and Science also make demands on
it, which means the player's requisitions compete with priorities she doesn't control. She sees her queue position and a
rough sense of Fleet's overall load, but does not manage their schedule. Fleet occasionally pushes back on unrealistic
timelines or flags that capacity is constrained.

**Ministry of Science** — manages the research and advancement pipeline. Receives artifact findings from Exploration,
develops new capabilities, hands them off to Fleet for implementation. Science is an **information source**: they have
an analytical perspective on the player's artifact collection that she may lack. Dispatches from Science may surface
patterns the player hasn't noticed — a cluster of geometrically interesting finds pointing toward something Science
thinks is worth pursuing, or a flag that the current trajectory is starting to converge on something specific. Science
can also deliver unwelcome news: a research direction that looked promising may prove a dead end, and Science will say
so.

**Ministry of Settlement** — establishes and manages colonies. Operates largely independently of the player; the player
receives specialists and logistics nodes from colonies without managing them directly. Settlement is a **pressure
source**: they represent the human cost of the catastrophe, and their dispatches grow more urgent as degradation
advances. A colony struggling for supplies, a habitability index in decline, a population center at risk — these arrive
in the feed as Settlement's voice, not the player's problem to solve directly, but impossible to ignore. In the late
game, Settlement may be the loudest ministry in the dispatch feed.

These ministries create texture and explain where capabilities come from. Inter-ministry politics are flavor, not
mechanics. The ministries do not have opinions about which win condition to pursue.

### The Player's Mandate

The Ministry of Exploration and Natural Resources has three overlapping responsibilities:

**Survey** — map the galaxy, characterize locations, identify sites of archaeological or resource interest, monitor
degradation advance. Survey is the upstream activity that everything else depends on.

**Archaeology** — excavate artifact sites, route finds to research outposts, develop outpost specializations, synthesize
findings into understanding. The primary output is knowledge, which feeds Science and ultimately Fleet.

**Mining** — locate and extract resources, including rare elements. The primary output is material, which funds
requisitions and shapes which capabilities and win conditions are accessible.

The tension between these three is the game's central resource allocation problem. A ship doing archaeology isn't doing
surveys. An outpost staffed for artifact analysis isn't optimized for resource processing. The player is always
balancing investment across all three.

### The Player's Actions

The player's actions cluster around a few verbs. She does not build things directly — that's Fleet's job. She directs,
routes, interprets, and requisitions.

**Direct** — assign ships to survey destinations or regions, initiate or defer excavations, establish or wind down
mining operations. These are the player's initiating actions; almost everything else follows from them.

**Route** — configure the logistics network. Establish freighter connections, set standing orders, decide which outpost
receives which artifact, manage specialist flow between colonies and outposts. Routing decisions are where survey,
archaeology, and mining become an integrated operation rather than separate activities.

**Interpret** — engage with the investigative layer. Read dispatches, pull records, set research flags, search the
warehouse for newly legible finds. Interpretation produces routing decisions — the synthesis moment where reading
becomes action.

**Requisition** — request capabilities from Fleet. Ships, outposts, infrastructure. Requisitions go into a priority
queue; the player controls ordering, Fleet controls fulfillment rate based on available capacity and resources.

Most execution is automatic once directed. Freighters run their routes, excavations proceed turn by turn, outposts
consume specialists and produce findings. The player sets direction and responds to what comes back.

### Requisitions and the Fleet Queue

The player submits specific requests to Fleet: ship classes, outpost construction, infrastructure. These enter a
priority queue. Fleet fulfills them in order, at a rate determined by available capacity.

Resources — drawn from the player's mining operations — gate how quickly Fleet can build. Low mining output means slower
fulfillment. The player's decisions about where to mine, and what to prioritize extracting, directly shape her
operational expansion rate.

The player can reorder the queue at any time. This is the primary lever for pivoting the operation when circumstances
change — a new win condition recognized, a degradation front advancing faster than expected. Reordering is costless; the
opportunity cost is whatever was already in progress.

In the late game, the queue becomes a sacrifice mechanic. Recognizing the win condition early enough to clear the queue
and redirect Fleet's capacity is part of what the player is being tested on. A player who understands what she's
building toward too late will find Fleet producing the wrong things at exactly the wrong time.

### Outposts and Specialists

Outposts are the player's purposeful infrastructure — forward research stations, excavation support bases, mining
operation hubs. They are distinct from colonies, which are Settlement's domain.

The player requisitions outpost construction from Fleet, then directs the outpost: what it's equipped for, what
artifacts it receives, what specialists are assigned to it. Outposts develop specializations organically based on what
flows through them, and deliberately through specialist transfers.

Specialists are produced by colonies over time and flow to outposts through the logistics network. The player's primary
lever over specialization is routing: deciding which outpost receives which specialists, and which artifacts get shipped
where. Deliberate respecialization — transferring specialists to reshape an outpost's character — is possible but
costly, and constrained by network topology.

Outpost viability varies by location. Hostile environments cost more to staff and may have higher specialist attrition.
This is a soft constraint on forward operations, not a hard gate — but it shapes where outposts are practical and where
they're expensive bets.

### Colonies as Context

Colonies are Settlement's responsibility. The player doesn't manage them, but they matter:

- They produce specialists, which flow to the player's outposts
- They are destinations for resource and mineral shipments
- They are nodes in the logistics network
- They are targets for degradation

A colony going offline — to degradation or poor conditions — affects the player indirectly but tangibly: specialist
supply drops, a logistics node disappears, a freighter route needs rerouting. The player feels colony health without
managing it.

Habitability is a soft mechanic underlying colony and outpost viability. It degrades visibly over time in affected
regions, giving the player a legible signal of what's coming before it arrives.

---

## The Galaxy

### Structure

The galaxy uses an abstracted structure in the style of Stars! — locations are points with properties rather than
physically simulated solar systems. Interest comes from the _variety and combination_ of properties at each location,
not from physical realism.

### The Wound

The galaxy has a structural feature that shapes everything: a **point of origin for a slow catastrophe**, caused by the
prior civilization's activities. The exact mechanism is part of what the player uncovers through archaeology — but the
artifacts eventually reveal something more unsettling than a unique disaster. This has happened before. The degradation
is cyclical; the prior civilization faced the same threat, got partway toward a solution, and failed. Their artifacts
are not just technology — they are research notes on the same problem the player is now trying to solve.

This revelation is discovered through play, not stated at the outset. The player who goes deep enough into the right
artifact clusters inherits the prior civilization's hard-won understanding of the phenomenon itself.

### Location Properties

Each location has properties that matter mechanically, revealed progressively through the survey process:

**Habitability** is readable from early survey — knowing where you can live is basic biology, and a civilization in
crisis tracks this carefully. It is expressed as one of four bands:

- _Optimal_ — comparable to home conditions; no special support required
- _Viable_ — sustainable with standard colonial infrastructure
- _Marginal_ — possible but expensive; higher specialist attrition, greater resource demand
- _Uninhabitable_ — below the threshold where population can survive unaided

The underlying habitability model is more granular than the bands suggest, but the bands are what the player sees. The
line between Marginal and Uninhabitable is the point of no return — a system that crosses it cannot support population
without extraordinary intervention.

**Resource profile** describes what a location produces: common resources in varying abundance, and potentially rare
elements once the player has the survey technology to detect them.

**Artifact signature** indicates whether there is something worth excavating, and at what level of confidence. Stronger
signatures suggest richer sites; absence of signature is not a guarantee of absence.

**Degradation estimate** becomes available with proper survey of a sufficiently understood location: a projected
timeline until the next habitability band crossing. Early in the game these estimates carry significant uncertainty;
they narrow as Science develops better models of propagation.

### Population and Habitability

Population capacity scales with habitability band. A colony sized for Optimal conditions that drops to Viable will lose
people — and with fewer people, output falls across every activity the colony supports: specialist production, resource
extraction, research capacity. The decline is self-reinforcing. Fewer people means less support, which means conditions
become harder to maintain, which means more people leave or die.

Population does not recover. At the timescale of the game — roughly 25 years — there is no natural growth that
meaningfully offsets loss. What is possible is relocation: Settlement, working with Fleet's shipping capacity, manages
the movement of population from degrading systems to viable ones. The total population across the civilization is a
slowly declining number. The player's ultimate score is how much of it survives.

### Degradation

Degradation propagates outward from the point of origin, but not uniformly. The galaxy has structure — regions that
conduct the catastrophe faster, regions that slow it, natural barriers that deflect it. This structure is not directly
visible to the player; it becomes legible through Science's progressive modeling, fed by survey data, artifact analysis,
and Settlement's habitability reports.

The propagation model has a useful property: every properly surveyed location has a degradation estimate, and the origin
location's estimate converges toward zero faster than any other. The player who surveys broadly enough, and watches the
pattern of estimates across the galaxy, can triangulate the origin — not through a dedicated mechanic, but by noticing
where the numbers are heading fastest. Science will surface this pattern explicitly once it becomes statistically
legible, but a player paying close attention may see it first.

Degradation expresses itself at the location level as habitability band crossings. A system doesn't fail suddenly — it
crosses a boundary, which Settlement flags in a dispatch, and the player has warning before the next crossing. The
cascade that follows is population-driven: as habitability drops, population drops, and as population drops, everything
the location supports becomes less productive.

The player's indirect lever on this process is survey: finding locations with good habitability and favorable
degradation estimates gives Settlement somewhere to send people. Resourcing struggling colonies can slow the population
cascade without stopping the underlying decline. Neither action addresses the catastrophe itself — that requires
archaeology, and ultimately a win condition.

## Exploration

Exploration is the primary hook of the game. The design goal: _legible probability with genuine surprise_. The galaxy
has structure and patterns the player can learn to read, but it still surprises them.

### Multi-Stage Revelation

Discovery is a process, not a binary state. Each stage requires investment and yields partial information:

1. **Detection** — the system is visible; star type and anomalous signatures may be readable. Essentially free.
2. **Survey** — a probe or scout visits. Broad strokes: planet count, rough habitability, whether artifact signatures
   are present.
3. **Assessment** — a capable ship spends time in the system. Full details: exact habitat values, resource deposits,
   artifact locations.
4. **Excavation** — artifacts require additional investment to recover and begin studying. A known artifact site may sit
   uninvestigated for many turns.

This creates a _queue of partially-known things_ the player is always waiting to learn more about — a core driver of the
"one more turn" feeling.

Note that, in the absence of a player presence at a particular location, no new information can be gleaned. So, the
planet that was surveyed early in the game, and otherwise ignored, might need to be re-surveyed after a new rare element
is discovered. Similarly, just having a presence there isn't enough; that outpost needs to be tasked with doing another
assessment. Dispatches will come to the player automatically, but other information will usually need to be sought out.

### Colonized Worlds

A colony doesn't end exploration of a system — it transforms it. An uninhabited surveyed world is a snapshot. A colony
is an ongoing relationship with that world, gradually revealing things a survey ship never would. Inhabited worlds
(yours or others') are _more_ interesting than empty ones, not less.

### The Galaxy Has Legible Structure

Patterns exist that the player can discover through play rather than being told about:

- Artifact concentrations cluster around certain stellar types or regions, reflecting the prior civilization's
  preferences
- Habitability gradients exist across the galaxy
- Resource-rich but dangerous regions cluster together, creating neighborhood-level decisions

---

## Colonization

Colonies are **infrastructure**, not trophies. The interesting question is never "should I colonize this planet" but
"what role does this node play in my network."

A colony:

- Extends logistics range and enables deeper survey work
- Develops local expertise over time, deepening knowledge of its system
- Creates new logistics challenges as well as solving old ones
- May have a finite useful lifespan as degradation advances

Colonization is a means to exploration and survival, not a measure of success.

---

## Research: Archaeology

### Core Principle

Research is reframed as archaeology — recovering lost knowledge rather than inventing new things. The prior civilization
left behind artifacts whose purpose is often unclear. Your scientists are engineers reverse-engineering things found in
a field, not historians piecing together a story.

### The Prior Civilization

Deliberately **mysterious and unknowable**. They are not "humans but more advanced." Their artifacts don't need to tell
a coherent story, and the game doesn't need to explain who they were or what their society looked like. This removes
narrative burden entirely.

What _does_ become legible through play: their _predicament_. The artifacts are evidence of their attempted solution to
the same threat the player now faces. They got partway there. The player is finishing what they started, or finding a
different answer.

### Physical Artifacts and Intangible Knowledge

Archaeological discoveries come in two forms, with meaningfully different logistics implications:

**Intangible knowledge** — observations, measurements, theoretical frameworks extracted from studying a site — can be
broadcast directly to any suitably equipped facility. It travels at the speed of communication.

**Physical artifacts** — objects recovered from a site — can only be analyzed where they physically are. They must be
transported to a research facility, which is a logistics decision: ship it home, deliver it to the nearest outpost, or
study it in place with a forward research team. A physical artifact in transit or at a remote outpost is more precarious
than broadcast knowledge. If the outpost is lost — to degradation or poor planning — work in progress on physical
artifacts may be lost with it.

### Research Facilities

Archaeological analysis can only be done at suitably equipped locations. Population centers are the most capable
facilities. Remote outposts can also conduct research, if the player devotes the resources to establishing and
maintaining that capability.

The **opportunity cost** of research infrastructure is real: building and maintaining a research outpost competes with
other uses of the same resources. This is the allocation decision — not a per-turn percentage slider, but an
infrastructure commitment, consistent with how everything else in the game works.

Outposts develop **specializations** based on what they've been fed. An outpost that has processed many artifacts of a
given kind becomes better at interpreting that kind — recognizing patterns a generalist facility would miss. This is
another axis along which two players' civilizations diverge.

Specialization is **emergent from logistics decisions**, not selected from a menu. The player's primary lever for
shaping an outpost's specialty is choosing what to ship there. This makes artifact routing a research priority decision
in disguise: the player who thinks carefully about which outpost gets which artifact is implicitly directing their
civilization's intellectual development.

When the player wants to deliberately reshape an outpost's specialization, they can **transfer specialists** — a
personnel resource that colonies produce over time. Specialists travel the logistics network like any other resource,
which means the network topology constrains organizational flexibility. A transfer costs capability at the source
outpost and takes time to take effect at the destination; a remote outpost that's hard to reach may develop whatever
character its founding team had, simply because reassigning specialists there is expensive. The decision to transfer
must be made in anticipation of need, not in response to it.

### Artifact Description System

Artifact descriptions are generated from a structured vocabulary rather than authored individually or LLM-generated.
This keeps descriptions searchable and learnable without requiring significant runtime resources.

#### The Four Dimensions

Every artifact is examined across four dimensions, corresponding to the parameters of standard archaeological analysis.
Each dimension has an explicit result — absence is stated, not implied:

- **Visual/material** — what it looks like and what it's made of
- **Structural** — how it's organized internally
- **Behavioral** — what it does under examination
- **Contextual** — where it was found and how it was situated

#### Three States Per Dimension

Each dimension resolves to one of three states:

**Unremarkable** — examined, nothing of note. Stated explicitly ("structurally unremarkable," "no behavioral response
under standard field tests"). Not a null find — the examination happened; there simply isn't signal here.

**Notable** — examined, something present and interpretable with current understanding. This is the primary carrier of
cluster signal, expressed in qualitative, evocative language rather than labeled properties.

**Anomalous** — examined, signal present but not yet interpretable. The description conveys that _something is
happening_ without being able to characterize it ("behavioral response defies current analytical framework," "structural
organization of a type not previously encountered"). Anomalous dimensions are the primary hook for future intern
moments.

Dimensions resolve independently — understanding one dimension of an artifact gives no insight into others. An artifact
can remain partially unresolved across its entire research career, and may go into the final score screen still
partially unread.

#### Resolution and Re-examination

When Science develops new understanding, anomalous dimensions don't resolve automatically — a specialist must re-examine
the artifact. However, the theoretical framework propagates at communication speed, so any suitably equipped outpost can
perform the re-examination without waiting for knowledge to travel physically.

This is primarily a UX surface rather than a design burden: the dispatch announcing new understanding should surface
affected warehouse items and provide convenient routing actions. The interesting decision remains _which_ specialist and
_at what priority_, not the mechanical act of routing.

#### Vocabulary and Cluster Signal

Descriptions are assembled from a designed vocabulary organized by cluster and dimension. The vocabulary is large enough
that descriptions feel varied across many artifacts, but consistent enough that player pattern recognition is meaningful
— learning the vocabulary is itself a form of incremental mastery.

Cluster signal is probabilistic, not deterministic. Cluster-relevant terms appear with higher frequency in artifacts
belonging to that cluster, but aren't exclusive to it. This prevents the vocabulary from becoming a transparent tag
system while keeping it learnable.

**Cross-cluster vocabulary** is sparse and intentional. The most-connected cluster pairs share one or two terms,
appearing in both contexts. The more surprising the connection (exotic physics ↔ biology), the more value the shared
term carries when a player encounters it. Expected connections (propulsion ↔ construction) may not warrant shared
vocabulary at all.

**Negative space** is an explicit descriptive tool. A description can actively characterize what an artifact lacks as
well as what it has — "structurally unremarkable but behaviorally anomalous" is doing more work than silence on the
structural dimension. Contrast between dimensions is a learnable signal.

#### The Dispatch Feed as Action Surface

_(Deferred to design phase)_ The dispatch feed is simultaneously an information delivery layer, a search surface, and —
as the re-examination mechanic illustrates — an action surface. The interaction design of this system is a significant
UX challenge that warrants focused attention during design.

### Excavation as Process

Artifact sites are not inventories with known contents — they are unknown quantities that reveal themselves through
investment. The process has more in common with mining than with research, but is less predictable than either.

A site has a **depth** that isn't visible from survey alone. Early excavation yields surface material relatively
quickly. Whether there is more underneath is genuinely uncertain, and the return curve is not linear. A site that looks
modest might prove exceptional at depth. A site with a strong artifact signature might be mostly surface material.

Investment determines **draw depth**, not guaranteed yield. Spending more effort reaches further into the site, but what
is found remains uncertain. **Null finds** — effort that returns only confirmation that a layer is exhausted, or
fragments too degraded to yield insight — are a real and acceptable outcome. With a galactic catastrophe on the horizon,
wasted effort is a genuine danger. But not trying is worse.

Critically, depletion is **not linear or fully legible**. A single null find is not a definitive signal that a site is
exhausted — it may indicate a dry layer between productive pockets. The player is always making an inference, not
reading a progress bar. The question after a null find is always: _was that a dry layer, or is this site done?_

Sites may have characteristic **depletion profiles** that experienced players learn to read:

- Some sites are shallow but dense — high early yield, quick exhaustion
- Others are sparse throughout but occasionally very deep, with pockets of material separated by barren layers
- Reading site type from early excavation results is a learnable skill, part of the game's incremental mastery

A more specialized research outpost is better not just at interpreting finds, but at _reading the site itself_ —
distinguishing a dry layer from genuine exhaustion, recognizing the signature of a deep pocket.

The **decision to stop digging** is as interesting as the decision to continue. Knowing when to walk away from a
diminishing site and redirect resources elsewhere is a skill the game rewards.

### How Artifacts Work

Artifacts have **properties, not identities**. Each artifact carries abstract properties — examples might include energy
manipulation, material science, spatial reasoning, quantum entanglement. Technologies and capabilities emerge from
accumulating depth in a property, or from combinations of properties intersecting in ways that open new investigative
directions.

Properties are never shown to the player as labeled stats or numerical values. The game's language is always
**qualitative and evocative**, never taxonomic. An artifact isn't tagged "spatial reasoning: high" — it's described as
displaying "geometric regularity suggesting intentional design" or "field structures of unusual symmetry." The player
builds intuitions about what kinds of descriptions cluster with what kinds of understanding, without the game making
that mapping explicit.

This matters because it prevents the system from becoming a recipe lookup. The player doesn't think "I need 30 points of
spatial reasoning" — they think "that region has been yielding geometrically interesting finds, and I want to understand
how the prior civilization thought about distance and traversal."

When the player has accumulated enough depth in a direction — through the finds they've prioritized, the outposts
they've specialized, the interpretive choices they've made — new understanding surfaces. This may manifest as an
interpretive event, a capability that becomes available, or a realization that something already in the warehouse is
newly legible.

### Artifact Property Clusters (Designer Reference)

_This section describes the underlying structure of the artifact system for design purposes. These categories are never
presented to the player as labeled properties or visible taxonomies — the player experiences them through qualitative
description and accumulated intuition, not through explicit tags._

There are six property clusters:

**Propulsion/traversal** — how the prior civilization moved things through space, at scales ranging from ships to
something larger. Loosely connected to construction/materials.

**Construction/materials** — how the prior civilization built things intended to last, or to withstand extreme
conditions. Loosely connected to propulsion/traversal.

**Exotic physics** — the prior civilization's deepest theoretical work: field manipulation, energy at a fundamental
level, spacetime. The hardest cluster to read early, and the one that appears in the most win conditions. Loosely
connected to degradation mechanics; has a surprising and loose connection to biology that may surface late.

**Degradation mechanics** — what the prior civilization understood about the catastrophe they caused, and their attempts
to characterize and address it. Appears in three win conditions. Loosely connected to exotic physics.

**Biology** — the prior civilization's work on life at a fundamental level. Possibly approached through the lens of
field manipulation, which is part of why these artifacts are among the stranger finds. Loosely connected to
information/preservation; has a surprising connection to exotic physics.

**Information/preservation** — how the prior civilization stored, transmitted, and protected knowledge against loss. The
most isolated cluster, appearing in only one win condition (Seed) as a primary cluster. Loosely connected to biology.

The loose connections between clusters are not mechanical modifiers. They are a guide for writing artifact descriptions
and Science dispatches — a propulsion find might occasionally echo something seen in a construction context, or a
biology artifact might respond to the same analytical approach as an exotic physics find. These connections are hints
and occasional surprises, not bonuses.

Rare elements are the material complement to artifact knowledge: certain win conditions require not just understanding
but physical substances capable of operating at the scales involved. A player may have the knowledge without the
materials, or survey a rare element deposit without yet knowing its significance. The connection between a specific rare
element and a specific win condition becomes legible through artifact interpretation, not through direct disclosure.

### The Warehouse

Not everything excavated is immediately useful, and not everything useless now will be useless forever.

A dig produces a stream of recovered material. Based on current understanding, the player can identify some fraction as
clearly interesting — worth the logistics cost of shipping to a research facility. The rest goes into the warehouse:
stored at the dig site or a nearby outpost, catalogued with whatever qualitative description current knowledge supports,
and set aside.

Crucially, **not everything in the warehouse will ever have value**. Some finds are genuinely inert — fragments too
degraded, objects whose properties fall outside any investigative direction the player pursues. Shipping everything to
the lab wastes significant logistics capacity on material that contributes nothing. Being judicious about what gets
shipped — based on reading the dig's qualitative descriptions — is a meaningful skill.

But some warehouse items are valuable finds that current knowledge can't recognize. They sit in storage, described in
terms that meant nothing at the time: "ice-blue crystalline inclusions," "unusual resonant properties," "non-standard
alloy composition." When new understanding arrives — when the player's scientists identify schroedingerite crystals as
associated with quantum field manipulation — those descriptions become legible. The crystals were always there. Now they
have a name and a meaning.

This is the **intern moment**: the player, reading a new research finding, remembers a field report from months ago.
There it is in the warehouse inventory. They task someone (probably the intern, because everyone else is busy) to
re-examine it. The game does not make this connection automatically — that synthesis is the Minister's job. The player
who reads reports carefully and remembers what they've seen is rewarded for paying attention.

The warehouse interface needs to support this: searchable and filterable by qualitative description, so a player who
thinks to search "crystals" after the schroedingerite discovery can find what they're looking for. This is an
investigative tool, not a management screen.

### Divergent Progression

Two players who find different artifact collections, work different sites, make different interpretive choices, and
notice different warehouse connections end up with meaningfully different civilizations. Tech progression is
**divergent**, not convergent. Each playthrough feels distinct because the player's civilization has a character shaped
by what they found and how they understood it — including what they were sharp enough to recognize.

### Research as Both Means and End

Research serves two roles simultaneously:

- **Local payoffs** — better engines, better shields, better sensors, available throughout the game
- **Components of the final answer** — the same research direction that improves your ships is slowly building toward a
  win condition

The connection between artifact properties and win conditions is not one-to-one. A given property may be relevant to
more than one path; a given path may draw on several properties. But the overall shape of a player's artifact collection
— what they found, what they prioritized, how they interpreted ambiguous discoveries — determines which endings are
within reach, and which are not.

The player's path through the artifact system determines what kind of solution they're building toward, often without
them realizing it until they're partway there. The moment of recognition — _oh, this is what I've been building_ — is
one of the game's intended high points.

---

## Advancement and Capability

### Structure: Capability Bands

Capability acquisition is organized into six categories, each corresponding loosely to the artifact cluster space:

- **Mobility** — drive efficiency, range, speed
- **Construction** — outpost durability, ship resilience, large-scale engineering
- **Sensors** — survey resolution, rare element detection, degradation prediction
- **Biological** — habitability extension, population resilience, and at the deep end, fundamental biological change
- **Field manipulation** — the practical expression of exotic physics research
- **Degradation understanding** — characterizing, predicting, and eventually addressing the catastrophe

Each category has several bands of advancement — early, mid, late, and win-condition-tier. This is a tech tree in
structure, but it is never visible to the player as such. The player experiences it through Science dispatches, artifact
provenance, and her own inference — not as a map she navigates explicitly.

Within each band, the specific advance that surfaces is partly determined by which artifacts drove it. The sub-variant
emerges from the collection rather than from player selection, consistent with how win condition variants work.

### Two Types of Advance

**Capability unlocks** — something becomes possible that wasn't before. A new ship class Fleet can build, a new survey
technology, a new outpost type. Discrete and significant.

**Capability improvements** — something existing becomes meaningfully better. Drive efficiency increases, sensor
resolution improves, excavation throughput rises. These arrive as threshold events from Science rather than as smooth
accumulation, even though the underlying progress is gradual.

Both types arrive the same way: as Science dispatches, with qualitative advance notice before the threshold and artifact
provenance when the advance lands.

### Science's Role

The advancement system lives in Science's department, not the player's. The player has no direct lever on Science's
priorities — artifact routing is her only input, and Science's output is a consequence of that input, filtered through
Science's own judgment and the demands of other ministries.

Science provides two kinds of communication about advancement:

**Advance notice** — qualitative signals that a threshold is approaching. Vague enough to require interpretation ("our
current collection is starting to suggest something about traversal at larger scales"), specific enough to reward a
player who acts on it. Not a progress bar; an analytical observation from people who know more than she does.

**Advancement dispatches** — when a threshold is crossed, Science announces the advance with at least partial accounting
of what drove it. "Improved drive efficiency, drawing heavily on the geometric regularity observed in the Kerath Drift
propulsion finds." This feedback loop confirms the player's routing instincts and deepens her understanding of how
descriptive vocabulary maps to capability. It is one of the primary ways the player learns the artifact system.

The other ministries also make demands on Science. Fleet needs engineering advances; Settlement needs habitability
support, especially as Act Two progresses. The player's artifact routing is a significant input but not the only one.
This occasionally surfaces as texture in dispatches — delays, competing priorities — without becoming a political
mechanic.

### Local Payoffs and Win Condition Components Are the Same System

Local payoffs and win condition components are not separate lists — they are the same capabilities at different depths.
Better drives are early mobility advances; Gate is mobility taken to its logical extreme. Better habitability support is
early degradation understanding; Reversal is that understanding taken all the way. This means the player's research
direction is always doing double duty: improving her current operation and slowly building toward an ending.

### Cross-Capability Advances

Most advances draw primarily on a single capability category. Occasionally — rarely — an advance emerges from depth in
two categories simultaneously. These cross-capability advances are more common at win-condition tier, where they are
expected and structural. In local payoffs, they are occasional and significant: a sign that two clusters the player has
been developing in parallel have started to interact in ways Science didn't anticipate.

A cross-capability local payoff is also a form of advance notice. The player who notices that an advance drew on two
clusters, and infers that their intersection might point somewhere interesting, is reading the game at the level it
wants to reward.

### Rare Elements

Significant advances — particularly at win-condition tier — sometimes require a physical material whose properties match
the theoretical work Science has been doing. When this happens, Science announces both the need and the means to address
it: new survey technology that makes the element detectable, and enough characterization to know what to look for.

The element was always present in the galaxy. Earlier surveys would have logged it as unremarkable — another mineral
among many, not worth flagging. The new survey technology isn't new sensing capability; it's new knowledge about what to
look for. Re-surveying known systems with this knowledge in hand is often sufficient to locate a source.

This creates a three-phase structure for capability advances that require rare elements:

1. **Science signals** — threshold crossed, material requirement identified, survey technology provided
2. **Exploration hunts** — the player re-examines known systems and directs new survey work with a specific target
3. **Fleet builds** — once material is flowing to construction sites, the capability comes online

The hunting phase has a different texture from general survey work: directed rather than open-ended, with a known target
and an unknown location. How quickly it resolves depends on prior survey coverage and the element's distribution in the
galaxy. A player with broad coverage may locate a source almost immediately. A player who has been consolidating may
face a more significant search.

Rare elements are not stockpiled in advance of need. Until Science identifies what to look for and why, there is no
meaningful way to distinguish a significant element from any other mineral. The knowledge is what makes the element
visible.

---

## Information Delivery

### Three Layers

Information reaches the player through three distinct layers, each doing different work:

**The map** is the primary interaction surface and the player's main analytical tool. Spatial patterns — degradation
spread, artifact clustering, outpost specialization profiles — are best understood as geography. The map is also an
**index into the dispatch feed**: clicking a system surfaces relevant dispatches and records for that location; drawing
a region filters the feed to activity there. The map and the dispatch feed are two views of the same information, kept
in sync, not two separate interfaces.

The map supports **player-defined analytical layers** — filters constructed from the game's qualitative vocabulary,
rendered spatially. Rather than a fixed set of overlays, the player can define a layer ("systems with artifact
signatures and declining habitability and no current excavation") and see it as geography. This is the spatial
equivalent of a research flag: a theory operationalized as a view. The formula language for defining layers shares
vocabulary with the flag system, so learning one deepens facility with the other.

Most base layers are available from the start — survey coverage, habitability, basic resource concentration — because
these are things a civilization would track regardless of crisis. Some layers expand as knowledge grows: a mineral
concentration overlay exists from the beginning, but rare elements only appear on it once the player knows they exist
and has the survey technology to detect them.

**The dispatch feed** is the daily briefing layer. Dispatches are brief — a few lines of field report, enough to be
textured and interesting without being narrative. They are notifications that point toward records, not documents in
themselves. The feed is also a search surface: when the player wants to answer "where did I see something about resonant
properties," the dispatch feed is where that search begins.

**Records** are the substance behind dispatches. Pulling a record from a dispatch gives the player the full site
assessment, the complete artifact description, the warehouse inventory with its qualitative catalogue entries. This is
where the texture lives — rich enough to think about and connect to other things, but only visited when something in the
dispatch feed catches the player's attention.

### Dispatches Are Notifications; Records Are the Substance

A dispatch announces; a record contains. The dispatch from an excavation might read:

> **Dig report — Auriga Drift, third moon** Surface layer cleared. Three objects recovered; one shows unusual resonant
> properties. Two fragments, too degraded for analysis. Sending to warehouse pending routing decision.

The warehouse record for that object, when pulled, has the full qualitative description across all relevant dimensions —
enough to search against, enough to remember, enough to connect to something found later.

### Player-Directed Flagging

The player can establish **research flags** — standing instructions to the dispatch system to surface incoming reports
matching a qualitative pattern. A flag might read: "alert me to anything mentioning geometric formations or unusual
symmetry." Incoming dispatches matching the flag are highlighted; the player can also run the flag retroactively across
existing warehouse records.

Flags are also **spatially visible on the map** — at minimum, showing where flagged artifacts are currently located.
This grounds the investigative thread in geography, making it possible to see whether a pattern is spatially clustered
or distributed.

Flags operationalize a theory without confirming it. A flag can be wrong — a geometric find that clearly has nothing to
do with the player's current hypothesis is a useful contradiction. Flags are also the player's investigative history:
looking at active flags shows what they've been pursuing, and in what terms.

The vocabulary of flags is the game's qualitative descriptive language. Effective flagging requires having internalized
that language well enough to express a theory in its terms — which is itself a form of incremental mastery.

### Outpost Legibility

Outpost specializations are visible to the player as characterization profiles — a simple breakdown showing what
dimensions of artifact description the outpost has developed depth in. This makes the artifact routing decision legible:
the player can see what a given facility is good at, and ship accordingly.

Outpost profiles also create a map layer: the player can view their network filtered by characterization coverage,
identifying gaps. "My behavioral characterization is thin everywhere east of the Drift" is a strategic observation that
the map can surface directly.

As a diegetic flourish, outposts that develop notable depth in a specialty may occasionally receive **recognition from
dimension-associated organizations** — a brief dispatch announcing an award of excellence in material characterization,
or commendation for exceptional contextual analysis work. These arrive in the feed like any other communication and
reward the player who has been paying attention to what their facilities have been producing.

---

## Logistics

### Core Philosophy

Logistics is **architecture, not busywork**. The player designs the network; the network runs itself. The satisfying
part is the system design — defining routes, priorities, and transfer rules — not the turn-by-turn execution of moving
resources around. Once a route is established, freighters operate on standing orders without further attention.

The interesting decisions are about network design: where are my bottlenecks, does this route have enough throughput,
what role does this node play?

### Topology Matters, But Isn't Primary

The spatial layout of the network is meaningful — range limits, routing choices, and the distance between supply and
demand all create real constraints. But topology is interesting primarily because it _drives other decisions_, not as a
puzzle in itself. A rich system just out of reach is an impetus to research better drives. A critical node going offline
forces a rerouting problem. The map is a source of pressure, not the focus of play.

### Forcing Functions

The logistics network is mostly invisible when it's working. The interesting moments are when something forces
reconsideration:

- **Range and speed limits** create a natural exploration frontier. Your logistics capability defines the edge of your
  comfortable reach. Improving it doesn't just help existing routes — it opens new space. The feedback loop: find
  something desirable but unreachable, research, reach it, find the next thing.
- **Depletion and degradation** break established supply lines. A world that was a rich resource source may become
  tapped out or degrade into uninhabitability. Worlds that depended on it need new sources — which is an exploration
  problem in disguise. A colony going hungry might be exactly what sends a scout into a dangerous region.

These are _pull_ mechanisms, not push — the player sees something they want or loses something they had, and the network
is what connects desire to fulfillment.

### Logistics and Exploration Are the Same Loop

Exploration finds nodes. Logistics connects them. Degradation breaks connections and creates pressure to find new nodes.
These aren't separate systems — they're the same feedback loop viewed from different angles.

### Logistics and Research Are Also the Same Loop

Artifact routing is research priority-setting in disguise. The player who ships a behaviorally interesting artifact to a
behavioral characterization outpost is making an intellectual decision, not just a supply chain decision. The logistics
network is the skeleton of the archaeology operation — its shape determines what gets learned, where, and when.

Personnel (specialists) travel the same network as artifacts and resources. This means network topology also constrains
organizational flexibility: transferring specialists to reshape an outpost's specialization requires an established
route and takes time. A remote outpost may develop whatever character its founding team had simply because it's hard to
reach.

### Resources

**Common resources** are present to some degree at most locations, with significant variation in profile and abundance.
These form the everyday material of the logistics network — what colonies need to survive and what ships are built from.

**Rare elements** exist on a spectrum of scarcity. The most valuable may be present in only a handful of systems in the
entire galaxy. Finding a rich source of a rare element is a significant event, not a routine survey result.

Rare elements matter because certain technologies — including late-game capabilities tied to win conditions — benefit
strongly from them, or may require them. The connection between rare elements and specific win conditions is not
one-to-one; a given element may be relevant to more than one path, and a given path may not strictly require any single
element. But the presence or absence of rare elements in your accessible space meaningfully shapes which directions are
easier or harder to pursue.

Crucially, rare elements are **not always detectable with early survey technology**. Developing the ability to scan for
a specific element may itself require an artifact-derived technology. This means explored systems are worth revisiting —
nobody thought to scan for it before, but now that we know what to look for, it's time to go back.

**Specialists** are a personnel resource produced by colonies over time. They are the workforce of the research
operation — what outposts consume to conduct analysis, and what gets transferred when the player wants to reshape an
outpost's specialization. Specialists are fungible within their specialization; there are no named individuals, only
typed resources moving through the network.

---

## The Threat: Degradation

### Nature of the Threat

A slow catastrophe propagating through the galaxy from a point of origin. Likely caused by the prior civilization's
activities — possibly energy experimentation that destabilized something fundamental. The exact mechanism is part of
what the player uncovers through archaeology.

The threat is **environmental, not military**. It does not lead inevitably toward combat. It is the galaxy running down.

### Pacing: Three Acts

**Act One — The Warning** The game begins with the player knowing a degradation cycle is coming but not knowing exactly
when or where it will begin. A few known artifacts hint at what is coming. The early game is archaeology, exploration,
and network-building — but with a specific investigative goal: triangulate the origin point and refine the timeline
estimate.

The degradation onset is variable, and the player can invest effort in refining the prediction. A player who commits
resources to prediction gets better positioning and more time to read the artifact landscape before committing to a
direction. A player who focuses on research and construction accepts more uncertainty about the timetable — a valid but
riskier approach. At game start, the estimate might be vague ("within the next 80–120 turns"); targeted investigation
narrows the window.

The act structure does double duty: Act One is not just network-building, it is also the window for reading what kind of
game this galaxy is going to be. The artifact distribution, the rare element seeding, and the degradation timeline
together determine which win condition categories are viable. A player who reads these signals well can begin
specializing earlier; one who doesn't may over-invest in an unviable direction before pivoting.

**The Threshold** At roughly the midpoint, degradation begins. This moment is predictable but not perfectly predictable
— the player knew it was coming, may have narrowed down where, but the exact onset still carries impact. Good early-game
work means better positioning. Neglecting the warning signs means being caught flat-footed.

**Act Two — The Race** The galaxy is actively getting worse. The logistics network that felt like a comfortable puzzle
is now under pressure. Colonies in endangered systems become difficult decisions. Archaeology is now dual-purpose:
building toward a win condition _and_ trying to understand the degradation mechanics well enough to predict where it
goes next.

Act Two has its own internal arc. The player enters it having recognized a win condition _category_ — the broad domain
her artifact collection has been pointing toward. As Act Two progresses, the specific _variant_ within that category
crystallizes: not just "a shield," but which kind of shield. This realization recontextualizes earlier finds and opens a
final phase of targeted execution. The player who sees the variant clearly enough — and early enough — can still
course-correct if a different variant looks more achievable given her resources and position.

Crucially: **understanding the degradation and doing the archaeology are the same investigation.** The artifacts are
simultaneously capability upgrades and data points about how this played out before.

---

## Winning

The win condition is **not declared upfront** — it is discovered through play, consistent with the archaeology spirit.
It exists and is coherent; the player experiences it as something they figured out rather than something they were told.

### Win Condition Structure

There are seven win conditions. They are not organized into named categories for the player — the groupings that exist
are a design convenience, not a visible taxonomy. Each win condition has a primary artifact cluster pair that points
toward it, and flavor-level sub-variants that emerge from which of those clusters the player went deeper into. The
sub-variants are expressed in the ending description, not as a branching choice during play.

Not all win conditions are reachable in every run — galaxy seeding (artifact distribution and rare element availability)
determines what's viable. A run typically has one or two win conditions that pull clearly ahead, some that are marginal,
and some that never become viable. Marginal paths create red herrings at both the win condition and sub-variant level,
which is a feature: dead ends are part of archaeology.

All win conditions are theoretically capable of saving the entire population, though they differ in ceiling and
difficulty. No win condition is playing for second place.

### The Seven Win Conditions

**Fleet** — The civilization leaves in force. The prior civilization's propulsion and construction research, recovered
and extended, makes it possible to move the population out at scale. The sub-variant — generation ships versus stasis
vessels — emerges from whether the player's artifact collection ran deeper into propulsion or construction. Primary
clusters: propulsion/traversal, construction/materials.

**Gate** — The civilization leaves through something the prior civilization was building toward: point-to-point
traversal at scale. Fewer ships required, but the technology is harder and stranger, and the player needs to know where
they're going. Primary clusters: exotic physics, propulsion/traversal.

**Adaptation** — The civilization survives by becoming something new. The prior civilization was working on biology at a
fundamental level — possibly through the lens of field manipulation, which is why these artifacts are among the hardest
to read early. The people who endure are not quite the people who started. This is presented without editorial comment.
Primary clusters: biology, exotic physics.

**Seed** — The civilization survives in compressed form. Knowledge, genetics, culture — a small vessel or a hardened
archive, a long shot that preserves something essential. The sub-variant depends on what the player prioritized: a
biological seed or an informational one. Primary clusters: information/preservation, biology.

**Arrest** — The civilization stops the degradation where it is, or builds against it hard enough that it doesn't
matter. The sub-variant — whether this looks like stopping the propagation or sheltering behind extraordinary
construction — emerges from the artifact collection. You can't undo the damage, but you can end the advance. Primary
clusters: degradation mechanics, construction/materials.

**Reversal** — The civilization fixes it. Deep understanding of the degradation mechanism — what the prior civilization
started, and why it got away from them — makes it possible to run it backward. This is the hardest win condition and the
most thematically resonant. The prior civilization got close. The player finishes what they started, or finds a
different answer. Primary clusters: degradation mechanics, exotic physics.

**Redirection** — The civilization moves the problem. The degradation cannot be stopped, but with enough energy and
enough understanding of its mechanics, it can be aimed — away from populated systems, into the void. This is not a fix.
The player who achieves Redirection knows they didn't solve it. Primary clusters: degradation mechanics, energy.

### Artifact Cluster Connections to Win Conditions

Each win condition draws on two primary clusters. Exotic physics appears in Gate, Adaptation, and Reversal — it is the
deep end of the artifact space, hardest to read early, with the most win conditions available to players who go there.
Degradation mechanics appears in Arrest, Reversal, and Redirection — understanding the threat is itself a path to
surviving it. Construction/materials and propulsion/traversal share a loose connection, as do exotic physics and
degradation mechanics; biology and exotic physics have a looser, more surprising relationship that may surface late.

### Scoring

The player's final score is primarily **population saved** — a number that is visible throughout play as colonies thrive
or go offline, not revealed as a surprise at the end. Watching the civilization shrink in real time as degradation
advances gives Act Two emotional weight without requiring the game to editorialize.

The score itself is a post-game reflection: the end screen surfaces it as a summary, alongside secondary dimensions
(systems still habitable, artifact knowledge recovered, win condition achieved and its sub-variant) that give a fuller
picture of the run. The score is not visible as a running tally during play; the population number is, which is enough.

Inter-ministry politics do not affect the score. The other ministries do not have opinions about which win condition to
pursue. Settlement's pressure is about resource needs and survival, not about which answer the player is building
toward.

### Retroactive Coherence

When the player recognizes her win condition, she should be able to look back at her artifact collection and see why.
The moment of recognition — _oh, this is what I've been building_ — is one of the game's intended high points. Course
correction is possible after this moment: a player who sees where she's going, and has a hunch that a different win
condition might be more achievable, can pivot — but only if she hasn't yet committed too deeply. Reading the signals
early enough to preserve optionality is a skill the game rewards.

---

## Turn Structure

The game uses **simultaneous resolution**: the player issues orders, everything executes, results arrive. This fits both
the bureaucratic flavor of the Minister role and the hands-off character of the logistics and archaeology systems. The
player sets direction; the world acts; dispatches arrive.

**One turn equals one month of game time.** A full game spans roughly 20–25 years, giving 240–300 turns. This scale
feels right for the three-act structure: enough turns for overlapping threads to breathe, enough pressure that no turn
feels consequence-free. Monthly granularity also fits the human texture of the game — reports come in, decisions get
made, freighters complete their runs.

The Minister is an individual in the world of the game, not an abstract role. A 20–25 year game fits within a single
working lifetime, which creates a natural constraint on the game's scope and a personal dimension to the stakes. The
Minister may live to see the outcome — or not.

Also, with only one generation's worth of time in the game, the usual population fluctuations aren't an issue. So, the
player's final score (population saved) isn't something that could be gamed by doing things to massively increase the
birth rate.

**Calibration note:** Specific act lengths and degradation onset timing require playtesting. The rough target is that
Act One occupies 40–60% of total turns, but the right answer is empirical.

---

## The "One More Turn" Engine

Good turn-feel requires multiple overlapping anticipation loops running simultaneously. The player should always be
waiting for several things at once:

- A freighter almost arriving
- A survey almost completing
- A prediction window almost narrowing
- An artifact excavation almost finished
- A research interpretation almost unlocked

No turn should feel wasted. Even a quiet turn nudges several threads forward.

### The Three Early-Game Investigations

The early game has three overlapping goals that create natural prioritization tension:

1. _What is out there?_ — general exploration, colony site scouting, network building
2. _What did they leave behind?_ — artifact hunting, beginning to shape a research direction
3. _When and where does it start?_ — the prediction problem, which gives exploration specific purpose

---

## Open Questions

_(Left open at the end of the brainstorming phase; these are all design-time questions.)_

**Stuff the player finds:**

- Specific resource types — how many common resources, and what are the rare elements? Rare elements are expected to
  fall out of the artifact property cluster work.

**What the galaxy looks like:**

- What degradation looks like mechanically at an affected location
- Habitability, and how it interacts with colonies, outposts, and degradation

**Open, but deferred:**

_(Topics that aren't fully nailed down, but are good enough for brainstorming; we'll flesh these out in the proper
design phase.)_

- Specific requirements for win conditions, and their variants
