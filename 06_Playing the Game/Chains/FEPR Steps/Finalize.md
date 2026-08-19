---
aliases:
  - Finalized
  - finalizing
  - finalization
---
Finalize is the first step of [[FEPR]]. It is followed by the [[Execute]] step.

If there is at least one [[Pending Chain Item]], the controller of the oldest Pending Chain Item must complete the steps of [[Playing a Card]] until it is a [[Finalized Chain Item]] or leaves [[The Chain]]. 
Chain Items are Finalized in the order they were appended to the Chain.

Finalizing an item to the chain does not pass [[Priority]]. 
# Finalization Process
Once a card has reached *step 6* of the [[Playing a Card|Play a Card]] process, it ceases to be a [[Pending Chain Item]]. Then, depending on its type:
- [[Permanent]] --> Leaves [[The Chain]] and becomes a [[Game Object]].
	- Any [[Passive Ability]] become active.
	- Execute all [[Rules Text]] of the card, top to bottom.
		- [[Unit]] --> Enters [[The Board]] [[Exhaust|Exhausted]], at the [[Location]] chosen during *step 2* of the [[Playing a Card|Play a Card]] process.
		- Non-Unit [[Gear]] --> Enters [[The Board]] [[Ready]] at the player's [[Base]].
- [[Spell]] or [[Ability]] --> Lingers on [[The Chain]].
	- It becomes a [[Finalized Chain Item]].
	- If there are other [[Pending Chain Item|Pending Items]] on [[The Chain]], then the controller of those Pending Items completes *Steps 2 through 5* of [[Playing a Card]] for those items before continuing.
	- Other players have an opportunity to play one or more [[Reaction]] before the resolution of spells.
	- Otherwise, execute the [[Game Effect]] of the spell, from top to bottom of the rules text of the card and then place the card in the [[Trash]] of the owning player.
	- [[Handling Illegal or Impossible Instructions]].
# What happens after Finalizing?
- If, after finalizing the Chain Item, that item is a [[Unit]], [[Gear]], or an [[Ability]] that [[Add|Adds]] resources, it resolves immediately—Move to Step 4: [[Resolution|Resolve]]. 
- If, after finalizing the Chain Item, there are still Pending Chain Items, return to step 1. Finalize. 
- If, after finalizing the Chain Item, there are no more items on the chain to be Finalized, the controller of the next item on the chain gains Priority. Move to step 2: [[Execute]].