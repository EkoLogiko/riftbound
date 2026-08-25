---
aliases:
  - Units
  - unit
  - units
---

**Units** are [[Game Object]]s while:
- On [[The Board]]
	- Units are at one of several [[Location]]s while on the Board: a [[Battlefield]] or their [[Base]].
	- Units and their details are [[Public Information]] while on the Board.
	- Units can be chosen, affected, or manipulated by [[Spell|Spells]], [[Ability|Abilities]], or [[Game Action|Game Actions]] that specify *Units*.
	- Units can be [[Kill|Killed]].
- In a [[Trash]]
	- Units are treated as Cards, similar to when in the [[Hand]].
	- They retain the properties of being a Unit, but are not on the Board and thus cannot take actions or be affected by [[Spell]]s, [[Ability]], or [[Game Action|Game Actions]] that target Units on the Board.
	- Units can be affected by spells and game effects that target Units in the Trash.

Unit is also a [[Card Type]].

Unit can be marked with [[Damage]].

Units may have [[Activated Abilities]].
- The [[Activated Abilities|Activated Ability]] of Units may be executed at any time during the controlling player's [[Main Phase]] during an [[Open State]], and not during a [[Showdown]].
- This follows the same process as [[Playing a Card]]. This behaves, once activated, like a [[Spell]] without an associated card.

A unit is **alone** when there are no other friendly units at the same [[Location]].
A unit is **one on one** when it and the enemy unit at the same [[Location]] are both *alone*.
A unit is **in combat** if it is occupying a [[Battlefield]] where [[Combat]] is ongoing and has a combat designation.
# Intrinsic Properties
Units have multiple intrinsic properties unique to them:
- [[Tag]]: A Unit has zero or more Tags representing one or more champions, regions, factions, or species it belongs to. These have no intrinsic rules or behaviors by themselves. Spells, abilities, and game actions can reference these types as part of their execution.
- [[Might]]: The combat statistic of a Unit. Used to determine a Unit's contribution to [[Combat]], as well as when it is [[Kill]]ed by damaging effects.
- Units can have [[Damage]] marked on them.
- Units enter the Board [[Exhaust|Exhausted]]. This can be altered by [[Accelerate]] or similar game effects
- Units have the inherent ability to perform [[Standard Move]]s.
- Units have a [[Location]] which is the [[Base]] or [[Battlefield]] it currently occupies.