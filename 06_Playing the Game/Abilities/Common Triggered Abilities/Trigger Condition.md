A **Trigger Condition** is the clause with *"When"*, *"At"*, or *"the Nth Time"* written as part of a [[Triggered Ability]].
Any additional conditional statement **immediately after** the Condition must be true in order for the Condition to be fulfilled. Such a conditional statement is part of the Trigger Condition and not the ability's Effect.

>*Example*: Sona, Harmonious reads **“At the end of your turn, if I'm at a battlefield, ready up to 4 friendly runes.”** Her Trigger Ability’s Condition will be fulfilled in the Ending Step, but the Triggered Ability will only be placed on the chain if she is located at a battlefield when the Condition is fulfilled. If she is removed in reaction to the triggered ability, it will still resolve.
>*Example*: Loose Cannon reads **“At the start of your Beginning Phase, draw 1 if you have one or fewer cards in your hand.”** The **“if you have one or fewer cards in your hand”** conditional statement is not immediately after the trigger condition, so it is part of the effect and not the condition.

The Condition of a [[Triggered Ability]] is evaluated after a potentially inciting event has been processed.
If a [[Game Object]] has a [[Triggered Ability]] that is active in a specific zone, it is evaluated and subsequently triggered if it enters that zone at the same time that its Trigger’s condition is met.

>*Example*: Immortal Phoenix says **“When you kill a unit with a spell, you may pay [1][C] to play me from your trash.”** This ability triggers if Immortal Phoenix is in your trash immediately after you kill a unit with a spell, even if the unit you killed with a spell was that Immortal Phoenix.

A [[Game Object]] will not be able to successfully evaluate its Trigger Condition, however, if it leaves the zone that its Trigger is active from at the same time that its Trigger is satisfied.

>*Example*: Viktor, Leader says **“When another non-Recruit unit you control dies, play a 1 [M] Recruit unit token into your base.”** This ability triggers if Viktor is on the board immediately after another non-Recruit unit you control dies. It does not trigger if Viktor and another non-Recruit unit you control die during the same game action (for instance, if they are both killed in the same Cleanup due to the damage dealt by Unchecked Power).