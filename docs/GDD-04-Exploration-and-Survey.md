# Exploration & Survey

## Overview

Exploration is the upstream activity that everything else depends on. Without survey, the player doesn't know where to
dig, where to mine, or where degradation is advancing. Without ongoing survey work, the picture of the galaxy stays
static while the situation changes around it.

The design goal for exploration is **legible probability with genuine surprise**. The galaxy has structure and patterns
the player can learn to read — artifact clusters around certain stellar types, habitability gradients, degradation
corridors — but it still surprises them. Survey is the activity that makes this structure visible, and the player who
surveys systematically will read the galaxy's structure better than one who cherry-picks individual leads.

## Ship Types

Exploration operates three classes of vessel, all requisitioned from Fleet and owned by the Ministry.

**Scout** — the workhorse of survey operations. Scouts visit systems to return accurate survey data, and can also
operate on standing patrol orders to provide passive scan coverage of a region. Scout capabilities — scan range, transit
speed, survey throughput — vary and improve as artifact research advances. Early scouts are capable but limited in
reach; later models extend the practical frontier of survey work significantly. The details of capability progression
are addressed in the Research & Advancement section.

**Freighter** — the backbone of Exploration's logistics network. Freighters move resources, artifacts, and specialists
between outposts, colonies, and home systems. They operate on standing route orders once established. Like scouts,
freighters see capability improvements over time — primarily in cargo capacity and range. Requisitioned from the same
Fleet queue as other vessels, which creates a real tradeoff: a freighter slot is a scout not built, and vice versa.

**Expedition Vessel** — a single-use ship that establishes an outpost at a target location. The vessel is consumed in
the process, its materials and equipment becoming the outpost's founding infrastructure. Expedition vessels are scarce
early in the game — the player may have only one — which makes early outpost placement a genuinely weighty decision.
Capability improvements to expedition vessels may affect the quality of the founding infrastructure, giving new outposts
a head start on certain kinds of work; details are deferred to Research & Advancement.

## Investigation Tiers

All stars are visible from turn one — their presence and position are known. This is information a spacefaring
civilization has by default. What a system actually contains requires active investigation.

Discovery is a process, not a binary state. Each tier requires investment and yields partial information, creating a
persistent queue of partially-known systems the player is always waiting to learn more about.

| Property                    | Remote Scan                            | Survey         | Outpost (early) |
| --------------------------- | -------------------------------------- | -------------- | --------------- |
| Stellar type                | ✓ (free)                               |                |                 |
| Habitability band           | ✓ (accurate)                           |                |                 |
| Resource presence           | ✓ (false positive risk)                |                |                 |
| Rare element presence       | ✓ (requires tech, false positive risk) |                |                 |
| Artifact signature          | ✓ (false positive risk)                |                |                 |
| Planetary composition       |                                        | ✓              |                 |
| Resource extraction rate    |                                        | ✓              |                 |
| Artifact site detail        |                                        | ✓              |                 |
| Degradation estimate        |                                        | ✓ (wide range) | narrows         |
| Remaining reserves (banded) |                                        |                | ✓               |

### Remote Scan

Systems within range of an established presence — outpost, colony, or scout on standing patrol — are passively scanned
each turn. Remote scanning provides partial information: enough to flag systems of interest, not enough to replace a
ship visit.

Habitability is the one property where remote sensing is accurate. Everything else carries false positive risk: a
resource or artifact reading flagged by remote scan may prove negligible or absent once a ship actually visits. The
instruments are good; reading signals across interstellar distances is simply an imprecise business.

False positives do resolve over time for systems under continuous passive scan — accumulated data filters out some
noise. But some ambiguous readings persist regardless of scan duration, and the distinction between "this will resolve
eventually" and "this requires a ship" is not visible to the player. This creates a natural triage behavior: wait for
fresh scan data to stabilize before committing ships, but don't assume all uncertainty will clear on its own.

Rare element detection at range requires specific survey technology developed through artifact research. Until that
technology exists, rare elements are invisible to remote scan regardless of how long a system has been under
observation.

Scan capability improves with technology. Systems previously scanned are worth re-evaluating when capability improves —
the data was always there; now it can be read more accurately.

### Survey

A scout visits the system and conducts active investigation. Survey data is accurate: a ship on location with competent
crew and good instruments returns ground truth. Planetary composition, resource extraction rates, artifact site detail,
and a wide-range degradation estimate are all reliable once a ship has visited.

This is sufficient information to make most operational decisions: whether to excavate, whether to establish a mining
operation, whether to plant an outpost. The player should feel confident acting on survey data.

Survey is a ship-turn investment. A scout dispatched to survey a system is unavailable for other work during transit and
investigation. Early game, when scouts are scarce, survey prioritization is a meaningful decision.

The artifact site detail returned by survey is qualitative — sufficient to decide whether excavation is worth pursuing,
and rich enough to begin reading patterns across systems, but not a complete picture of what a site contains. That
emerges through excavation itself.

### Outpost (Early Operation)

An outpost established in a system becomes the primary source of ongoing intelligence about that location. In its early
operation — before specialization has taken hold — the outpost functions partly as an extended characterization effort,
returning data that no ship visit alone could provide: how reserves are holding up, how the degradation estimate is
narrowing as Science's models improve.

The assessment of a system is not a distinct player action. It is what a presence in that system naturally produces over
time.

Early outpost dispatches will confirm or correct the remote scan picture. An artifact signature that looked promising
from a distance may prove a false positive once the outpost team is on the ground. This is an occasional surprise, not a
routine outcome — remote scan false positives are calibrated to be infrequent enough to be interesting rather than
frustrating. The outpost retains value regardless: it extends scan coverage, anchors the logistics network, and serves
as a forward base for deeper survey work in the region.

## Outpost Establishment

Planting an outpost is a commitment. The expedition vessel dispatched to a system is consumed in establishing the
outpost — its materials and crew becoming the founding infrastructure of the new facility. There is no retrieving the
vessel if circumstances change.

Outposts are not typed at establishment. The player is not choosing between an archaeology outpost and a mining outpost
— she is establishing a presence. What the outpost becomes is determined by subsequent routing decisions: which
specialists are assigned, which artifacts are shipped there, what standing orders it operates under. An outpost that
receives excavation specialists and artifact shipments develops archaeological depth. One that receives extraction
equipment and mining personnel becomes a resource hub. The founding decision is location; everything else follows from
how the outpost is used.

This means a failed outpost — one established on the strength of a remote scan false positive — is not wasted. It is
infrastructure: a scan node, a logistics waypoint, a base for the next push deeper into the region.

## Re-Survey and the Value of Prior Coverage

Survey data ages. A system characterized early in the game may look different after degradation advances, or after new
rare element detection technology becomes available. Re-surveying known systems is a meaningful activity, not
backtracking.

When Science develops the ability to detect a specific rare element, they will typically dispatch a recommendation to
re-scan systems that showed relevant geological profiles — the element was always there; now it can be seen. A player
with broad prior coverage may locate a source almost immediately. A player who surveyed narrowly faces a more
significant search.

The dispatch system surfaces re-survey opportunities when new capability makes them relevant. Acting on them promptly is
a skill the game rewards.

## Standing Orders and Survey Strategy

Scouts not assigned to specific destinations can operate on standing orders: patrol a region, prioritize systems with
unresolved remote scan readings, avoid systems already surveyed. Standing orders let the player set survey direction
without micromanaging individual ship assignments.

The player who surveys systematically — broad sweeps that build regional coverage before committing to specific targets
— reads the galaxy's structure better than one who pursues individual leads. Artifact clusters, habitability gradients,
and degradation corridors become legible from coverage. This is a learnable strategic preference, not a rule the game
enforces.
