---
aliases:
  - mistarget
  - mistargets
---

The process for a card's choice becoming *Invalid or Unavailable* is referred to as **mistargeting**. This process is checked during the [[Finalize]] process, during *step 6* of the [[Playing a Card]] process.

If all of an instruction's [[Target|Targets]] become invalid or unavailable by the time the spell begins resolving, that instruction will not execute.
If an instruction has more than one [[Target]] and fewer than all of the [[Target|Targets]] become invalid or unavailable by the time the spell begins resolving, the instruction will execute, with only the Targets available and valid being operated on.
>*Example*: Singularity reads **“deal 6 to each of up to two units.”** The instruction will execute even if one of those units is made unavailable before the spell begins.

If another spell or ability attempts to reference the number of [[Game Object|Game Objects]], players, or zones that a [[Finalized Chain Item]] targets, it will include any mistargeted choices, but not any targets that have changed to a [[Non-Board Zone]].
>*Example*: When a player moves their Volibear, Furious to an occupied enemy battlefield and combat initiates, Volibear’s attack trigger goes on the chain targeting three of the units at that battlefield. In reaction, the defending player plays Flash moving two of the three units back. That player cannot then target the attack trigger with Repulse, which reads “Choose a friendly unit at a battlefield. Counter an enemy spell or ability that chooses it and no other friendly unit.” If the defending player instead played Heedless Resurrection twice, killing the two units, Repulse can legally target the attack trigger, because two of the targets have changed to a non-board zone.

It is possible for none of a spell's instructions to be executed as it resolves, due to all of them requiring targets to act on and all of those targets becoming **mistargets**. In this case, the spell has no effect but *is still considered played*.
>*Example*: A player plays a spell that reads **"Deal 2 to a unit at a battlefield"** with no other instructions, and chooses an enemy unit at a battlefield. They also control a unit with the ability **"When you play a spell, give me +1 [M] this turn."** Before the spell resolves, the chosen unit is moved to its base. The spell resolves and its only instruction cannot be executed, but the unit's ability still triggers as the spell resolves and gives it +1 [M].