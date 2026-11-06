A **Trigger Condition** is the clause with *"When"*, *"At"*, or *"the Nth Time"* written as part of a [[Triggered Ability]].
Any additional conditional statement **immediately after** the Condition must be true in order for the Condition to be fulfilled. Such a conditional statement is part of the Trigger Condition and not the ability's Effect.

>*Example*: Sona, Harmonious reads **“At the end of your turn, if I'm at a battlefield, ready up to 4 friendly runes.”** Her Trigger Ability’s Condition will be fulfilled in the Ending Step, but the Triggered Ability will only be placed on the chain if she is located at a battlefield when the Condition is fulfilled. If she is removed in reaction to the triggered ability, it will still resolve.
>*Example*: Loose Cannon reads **“At the start of your Beginning Phase, draw 1 if you have one or fewer cards in your hand.”** The **“if you have one or fewer cards in your hand”** conditional statement is not immediately after the trigger condition, so it is part of the effect and not the condition.

The Condition of a [[Triggered Ability]] is evaluated after a potentially inciting event has been processed, unless the event the Condition checks is the source of the triggered ability leaving the board.
If a [[Game Object]] has a [[Triggered Ability]] that is active in a specific zone, it is evaluated and subsequently triggered if it enters that zone at the same time that its Trigger’s condition is met.

>*Example*: Immortal Phoenix says **“When you kill a unit with a spell, you may pay [1][C] to play me from your trash.”** This ability triggers if Immortal Phoenix is in your trash immediately after you kill a unit with a spell, even if the unit you killed with a spell was that Immortal Phoenix.

A [[Game Object]] will not be able to successfully evaluate its Trigger Condition, however, if it leaves the zone that its Trigger is active from at the same time that its Trigger is satisfied.
>*Example*: Viktor, Leader says **“When another non-Recruit unit you control dies, play a 1 [M] Recruit unit token into your base.”** This ability triggers if Viktor is on the board immediately after another non-Recruit unit you control dies. It does not trigger if Viktor and another non-Recruit unit you control die during the same game action (for instance, if they are both killed in the same Cleanup due to the damage dealt by Unchecked Power).

If a [[Game Object]] has a [[Triggered Ability]] whose condition is the [[Game Object]] leaving [[The Board]], such a [[Triggered Ability]] is processed immediatly before the [[Game Object]] changes zone.
>*Example*: If a game object has a Deathknell ability, which triggers on the game object dying, it will be processed and placed on the chain just prior to the game object being placed in the trash, during the event of the game object dying.
>*Example*: Treasure Trove has a triggered ability that triggers as it “leaves the board.” Such a triggered ability is processed and placed on the chain just before Treasure Trove completes the action of leaving the board by being moved to another zone.

[[Triggered Ability|Triggered Abilities]] that trigger from [[Game Object|Game Objects]] leaving [[The Board]] trigger and are placed on [[The Chain]] *after* any [[Replacement Effect|Replacement Effects]] are processed. If a [[Replacement Effect]] causes the [[Game Object]] to not leave [[The Board]] in the appropriate way, the relevant [[Triggered Ability|Triggered Abilities]] will not trigger.
>*Example*: If a unit’s death is replaced by an event of that unit being healed, exhausted, and recalled, that unit’s Deathknell abilities will not trigger, as the unit’s death event is replaced and does not occur.
>*Example*: If Treasure Trove’s being killed is replaced with it being banished, it will still trigger just before the banish action is executed.

While the [[Triggered Ability]] is being processed, note any information about the source of the [[Triggered Ability]] or the state of the game as needed in order to process the resulting [[Triggered Ability]].
>*Example*: A unit reads in part “When I leave the board, deal 2 to a unit where I was.” Its controller plays Retreat on the unit, returning it to hand. Before the unit is returned to hand, the triggered ability is placed on the chain and the necessary information about that unit is noted. When the triggered ability is being finalized, we can identify the former location of the unit in question with the noted information.