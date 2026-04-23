# The Galaxy

## Structure

The galaxy is an abstracted point-based structure in the style of Stars! — locations are systems with properties, not
physically simulated solar systems. Interest comes from the variety and combination of properties at each location, not
from physical realism.

The galaxy contains approximately 300 systems. This number is a design target, not a hard constraint; playtesting may
require adjustment.

The galaxy is procedurally generated for each run. Generation likely operates within constraints — ensuring viable win
conditions, reasonable rare element distribution, and playable degradation timing — but the specifics of those
constraints are deferred to the design phase.

## What the Player Sees

All stars are visible from turn one: their presence and location are known. This is information a spacefaring
civilization would have by default. What a star's systems actually contain requires active investigation.

## Planetary Composition

Systems contain planets, modeled at a broad categorical level (rocky, ice, gas, etc.). Planetary composition is not an
action target — the player directs actions at the system level, not at individual bodies. Composition exists as a
pattern substrate and as flavor in reports and dispatches.

When a report situates a finding — an artifact site, a rare element deposit, an unusual geological feature — it does so
with reference to the relevant body: "the excavation team has established a base on the ice moon; the system's rocky
planets show no comparable geological profile." The player learns patterns from reading enough of these reports.
Planetary composition is below the resolution of remote scanning; a ship visit is required to know what kinds of bodies
a system contains.

## System Properties

Each system has properties that matter mechanically, revealed progressively through the survey process. Not all
properties are visible at the same stage of investigation.

### Stellar Type

A spacefaring civilization reads stellar spectra as a matter of course. Stellar type is a pattern carrier: the prior
civilization had preferences, and those preferences left traces. A player who reads enough reports will notice that
certain artifact clusters appear more often around certain stellar types, or that a particular rare element keeps
turning up in systems with the same spectral signature.

These patterns are probabilistic, not deterministic. Stellar type is a hint, not a recipe.

Stellar types are drawn from a set of 5–6 categories. Binary systems are not modeled as a distinct type.

### Neighborhood Density

How many systems fall within a given radius of a location — a measure of how crowded that region of the galaxy is.
Visible from the map at all times, since all stars are visible from turn one.

Neighborhood density is a pattern carrier primarily for degradation propagation: the catastrophe may spread faster
through dense regions than sparse ones, creating corridors of accelerated advance. It may also reflect prior
civilization settlement preferences.

## Significant Points

The galaxy is seeded with approximately six significant points — procedurally placed coordinates, each with an
associated radius, collectively covering roughly half to three-quarters of the map. Some overlap between zones is
intentional; a system near two significant points may have richer or more complex patterns.

These points are never labeled or directly visible to the player. They are inferred from patterns — a cluster of
artifact-rich systems, a region where a particular rare element keeps appearing, an area where degradation seems to
advance differently. Piecing together that a region has structure, and what that structure implies, is part of the
game's investigative layer.

Each point may carry narrative weight, even if that weight is never stated explicitly. A region with high artifact
density is more satisfying to discover if it _means_ something — if the prior civilization was concentrated there for a
reason, or if the resource abundance reflects a geological history the archaeology eventually touches on. Not all points
need equal narrative significance; some may be lighter, representing geological or physical phenomena rather than prior
civilization history. But the possibility of meaning should inform how points are characterized during content design.

The specific character of each point — what patterns it carries, what narrative significance it holds — is deferred to
artifact cluster and win condition design. The degradation origin point is one significant point with a guaranteed role;
the others are open.

### Habitability

Expressed as one of four bands:

- **Optimal** — comparable to home conditions; no special support required
- **Viable** — sustainable with standard colonial infrastructure
- **Marginal** — possible but expensive; higher specialist attrition, greater resource demand
- **Uninhabitable** — below the threshold where population can survive unaided

The underlying habitability model is more granular than the bands suggest — Science and Settlement work with finer
detail — but the player's ministry sees only the band. This is sufficient for the decisions Exploration makes.

Habitability is readable from remote scan — accurate, not merely approximate. Knowing where you can live is basic
biology, and a civilization in crisis tracks this carefully. It is one of the few properties where remote sensing is
considered reliable without a ship visit.

Habitability degrades over time as the catastrophe advances. A system's band is not fixed.

### Resource Profile

Describes what a system produces: common resources, and potentially rare elements once the player has the survey
technology to detect them. Common and rare resources share the same visibility model.

Each resource type has two values:

**Extraction rate** — how much can be extracted per month. A single visible number, accurate from survey. This is the
primary operational value: what the player uses to plan mining output, requisition fulfillment, and logistics.

**Remaining reserves** — a banded value indicating how much is left in the deposit. Visible only from assessment
(extended presence). Expressed in broad terms: rich, moderate, depleting, exhausted. Declines over time as the resource
is extracted. Dispatch reports will flag significant band crossings ("mining output at Kerath IV declining — reserves
entering depletion band").

Remote scan indicates resource presence — common resources reliably, rare elements only with appropriate survey
technology — but not extraction rate or reserves. False positives apply: a resource flagged by remote scan may prove
negligible or absent on survey.

Common resource types are yet to be determined. Rare elements are defined by the artifact cluster and win condition
work; their detection requires technology developed through artifact research.

### Artifact Signature

Indicates whether there is something worth excavating, and with what degree of confidence. Expressed qualitatively
rather than numerically — "strong anomalous readings," "faint but persistent signal," "possible interference pattern" —
because archaeological confidence before excavation is genuinely uncertain, and false precision would be misleading.

Stronger signatures suggest richer sites; absence of signature is not a guarantee of absence. The player develops
intuitions about which language tends to pay off without the game making that mapping explicit.

### Degradation Estimate

A dynamic, derived property — calculated from survey data and Science's evolving models, not a fixed characteristic of
the system. Expressed as a range: months until the next habitability band crossing. Early estimates may be wide enough
to be nearly useless ("60–180 months"); they narrow as Science develops better propagation models and as the player
invests in prediction.

The origin location's estimate converges toward zero faster than any other. A player who surveys broadly and watches the
pattern of estimates across the galaxy can triangulate the origin — not through a dedicated mechanic, but by noticing
where the numbers are heading fastest. Science will surface this pattern explicitly once it becomes statistically
legible.

## Starting Conditions

A small percentage of systems are inhabited at game start, distributed across the galaxy rather than concentrated in a
cluster. This avoids giving the player's starting position undue influence over the game's shape.

The degradation origin point is placed randomly, with a minimum distance from the initially inhabited systems. Specific
constraints on this placement are deferred pending degradation propagation design.

## Pattern Carriers

Patterns in the galaxy — artifact distributions, resource clustering, degradation structure — are carried by a small set
of system and regional properties. The actual content of these patterns (which artifact clusters favor which stellar
types, which rare elements appear near which significant points) is deferred to artifact cluster and win condition
design. The carriers are:

**Stellar type** — individual system property. Carries artifact preferences, rare element associations, habitability
baseline tendencies.

**Neighborhood density** — regional property. Carries degradation propagation characteristics, possibly prior
civilization settlement patterns.

**Proximity to significant points** — regional property, never directly visible. Carries artifact concentration, rare
element clustering, and potentially degradation structure. Each point may also carry narrative significance that informs
content design without being stated to the player.

**Planet type distribution** — individual system property. Carries rare element specifics and artifact site character.
Patterns here are learned more slowly, since planetary composition requires a ship visit.

## Open Questions

- Procedural generation constraints: what guarantees does generation make about win condition viability, rare element
  distribution, and degradation placement?
- Degradation propagation: how does the catastrophe spread through the galaxy, what structures accelerate or slow it,
  and how does this interact with system properties? _(Deferred — see Open Questions)_
- Common resource types: how many, and what are they? _(Likely falls out of win condition and logistics design)_
- Rare element types and distribution: how many distinct elements, how many sources per element, and what survey
  technology is required to detect each? _(Deferred to artifact cluster and win condition design)_
- Specific constraints on degradation origin placement relative to starting systems.
- Stellar type categories: what are the 5–6 types, and do any carry mechanical properties beyond pattern weight (e.g.,
  habitability baseline, scan difficulty)?
- Significant points: what is the narrative and mechanical character of each of the ~six points beyond the degradation
  origin? _(Deferred to artifact cluster and win condition design)_
