# Overview & Philosophy

## What This Game Is

**After Them** is a single-player, browser-based space strategy game about archaeology, logistics, and survival in the
face of slow catastrophe. The player assumes the role of a Minister of Exploration and Natural Resources in a
civilization facing environmental collapse.

The game is inspired by **Stars!** in structure and spirit—celebrating discovery, meaningful logistics, and incremental
mastery—but it deliberately rejects the traditional 4X framework. There is no military conquest. There are no rival
factions. The antagonist is the galaxy itself: entropy, degradation, and time.

## Core Design Pillars

The game preserves three qualities from its inspirations:

**Discovery** — Finding things should feel like unwrapping a gift, not sampling a random table. Multi-stage revelation
creates a queue of partially-known things the player always waits to learn more about, sustaining the "one more turn"
impulse.

**Logistics** — Moving resources and managing networks is satisfying in itself, not merely a means to an end. The player
designs architecture; the world runs on standing orders. The interesting decisions are about system design: bottlenecks,
throughput, network topology, and role.

**Incremental Mastery** — Progress feels earned. Each step opens new possibilities. The player learns a qualitative
vocabulary, develops intuitions about artifact patterns, and grows skilled at reading a system they didn't fully
understand at the outset.

## What It Is Not

- **Not a 4X game.** Explore and expand, yes. Exploit, yes. Exterminate: no. The fourth pillar is replaced by the
  pressure of entropy.
- **Not narrative-heavy.** The game is intentionally abstract and systemic. Story emerges from play, not from authored
  sequences. The prior civilization is deliberately mysterious—their artifacts are research notes on a problem, not
  artifacts of a culture.
- **Not multiplayer or faction-based.** All actors are part of the same government. Inter-ministry politics are flavor;
  the ministries do not compete for victory.
- **Not visually ambitious.** The game is the important part. Visual style is explicitly not a priority.

## The Player's Perspective

The player is the **Minister of Exploration and Natural Resources**, one voice in a small government of competing
mandates. The player does not manage other ministries—they are abstractions. The player interacts with them through
requests (requisitions) and receives from them through dispatches (reports, deliveries, warnings).

This role creates a natural constraint: **the player has agency over their own ministry's decisions, but must navigate
the constraints and priorities of others.** A requisition goes into Fleet's queue; Fleet decides when to build it based
on available capacity and competing demands. Science routes research effort according to their own judgment and the
needs of Settlement. The player influences these systems but does not control them.

The role also creates texture and realism without becoming a political game: the player cannot vote which end-state to
pursue. The ministries are not invested in the outcome. They care about their mandates: Fleet builds, Science
researches, Settlement survives. The player's job is to navigate these constraints and make the outcome.

## The Three Core Activities

The player's ministry has three overlapping responsibilities:

**Survey** — map the galaxy, characterize locations, identify sites of archaeological or resource interest, monitor
degradation advance. This is the upstream activity everything else depends on. Without survey, you don't know where to
dig or where to mine. Without new survey work, your picture of the galaxy stays static as degradation advances.

**Archaeology** — excavate artifact sites, route finds to research facilities, develop outpost specializations,
synthesize findings into understanding. The primary output is knowledge, which flows to Science and ultimately unlocks
new capabilities. But knowledge doesn't keep colonies alive or build ships.

**Mining** — locate and extract resources, including rare elements. The primary output is material, which funds
requisitions and shapes accessible capabilities. A rich mining operation can accelerate your entire program. But mining
operations don't discover the solutions the player needs.

These three activities compete for the same limited resources: ships, logistics capacity, specialist time, requisition
priority. The tension is **structural and unresolvable**—there is no "correct" balance, because the correct balance
depends on circumstances that change as the game unfolds:

- Early, survey dominates: you don't know enough to dig intelligently or mine profitably. A player who skimps on survey
  may miss critical information about degradation timing or artifact distribution.
- Mid-game often sees archaeology peak: you have enough data to know where to dig, and you need the knowledge artifacts
  unlock. But this requires logistics capacity and mining output to sustain.
- Late-game mining becomes critical: certain capabilities require rare elements, and if you haven't found a source,
  you're blocked. A player who neglected mining in the mid-game may find their late-game constrained.

The player is always balancing investment across all three, and the cost of getting that balance wrong is real—not in
terms of an explicit penalty system, but because resources spent on one activity are unavailable for another. A ship
tasked to survey is not available for excavation support. An outpost staffed for artifact analysis is not optimized for
resource processing. Every major decision involves a tradeoff.

This tension is the game's **central resource allocation problem**, and it's one of the primary levers that creates
divergent playstyles. A player who commits heavily to early archaeology discovers win conditions faster, but may face
late-game resource constraints. A player who prioritizes mining gains execution capacity but may misunderstand the
artifact landscape. The player who balances all three carefully navigates the space better but moves more slowly through
each.

## The Player's Actions

The player's actions cluster around four verbs. Most execution is automatic once directed:

**Direct** — Assign ships to survey destinations, initiate or defer excavations, establish or wind down mining
operations. These are initiating actions; nearly everything else follows.

**Route** — Configure the logistics network: establish freighter connections, set standing orders, decide which outpost
receives which artifact, manage specialist flow. Routing decisions integrate the three activities into a coherent
operation.

**Interpret** — Engage with the investigative layer: read dispatches, pull records, search the warehouse, set research
flags. Interpretation produces routing decisions—the synthesis moment where reading becomes action.

**Requisition** — Request capabilities from Fleet: ships, outposts, infrastructure. Requisitions enter a priority queue;
the player controls ordering, Fleet controls fulfillment.

## The Threat: Degradation as Antagonist

A slow catastrophe propagates outward from a point of origin, caused by the prior civilization's activities (a mechanism
the player uncovers through archaeology). It is environmental, not military. It does not lead toward combat. It is the
galaxy running down.

Degradation is the pressure mechanism, not a puzzle to solve immediately. In Act One, it is a distant warning. At the
midpoint (the Threshold), it begins. In Act Two, it is active pressure—the logistics network is under stress, colonies
become difficult decisions, and the clock is visible.

The threat is **not inevitable defeat**. The game has seven viable win conditions, each representing a different human
response to catastrophe: escape, transcendence, adaptation, preservation, sheltering, fixing, or redirection. All are
capable of saving the civilization, though they differ in difficulty and scope.

## Design Spirit: What to Preserve

- **Legible probability with genuine surprise.** The galaxy has structure and patterns the player learns to read. But it
  still surprises them. Artifact clusters have probable patterns without being transparent recipes. Degradation
  propagates according to rules, but the player never has perfect information about what comes next.

- **Failure is legible.** A player who doesn't read signals—who misses where degradation is coming from, or commits
  resources to an unviable win condition—can see in hindsight why they lost. This is not about random chance; it's about
  what the player noticed and what they chose to do.

- **Divergent progression.** Two players who find different artifacts, work different sites, make different interpretive
  choices, and specialize different outposts end up with meaningfully different civilizations. Tech progression is not
  convergent on a single tree; it fans out.

- **Synthesis is the player's job.** The game provides information, patterns, and the tools to search. It does not make
  connections automatically. The player who reads dispatches carefully, remembers what they've seen, and connects
  warehouse finds to new discoveries is rewarded for paying attention. The "intern moment"—remembering an old report
  that now makes sense—is an intended high point.
