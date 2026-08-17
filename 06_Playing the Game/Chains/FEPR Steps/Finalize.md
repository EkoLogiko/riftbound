---
aliases:
  - Finalized
---
Finalize is the first step of [[FEPR]]. It is followed by the [[Execute]] step.

If there is at least one [[Pending Chain Item]], the controller of the oldest Pending Chain Item must complete the steps of [[Playing a Card]] until it is a [[Finalized Chain Item]] or leaves [[The Chain]]. 
Chain Items are Finalized in the order they were appended to the Chain.

Finalizing an item to the chain does not pass [[Priority]]. 

# What happens after Finalizing?
- If, after finalizing the Chain Item, that item is a [[Unit]], [[Gear]], or an [[Ability]] that [[Add|Adds]] resources, it resolves immediately—Move to Step 4: [[Resolution|Resolve]]. 
- If, after finalizing the Chain Item, there are still Pending Chain Items, return to step 1. Finalize. 
- If, after finalizing the Chain Item, there are no more items on the chain to be Finalized, the controller of the next item on the chain gains Priority. Move to step 2: [[Execute]].