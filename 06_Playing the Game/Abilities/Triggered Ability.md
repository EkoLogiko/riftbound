---
aliases:
  - Triggered Abilities
---
**Triggered Abilities** are repeatable effects that happen when a [[Trigger Condition]] is met.

 They can usually be recognized by the words:
 - *"when"*, followed by a game action or event
 - *"at"*, followed by a point in time during the turn sequence
 - the phrase *“the [Nth] time”* followed by a [[Game Action]] or event.

>*Example*: "When you conquer here, you may spend a buff to draw 1."
>*Example*: "At the end of your turn, ready 2 runes."
>*Example*: “The first time I move each turn, you may ready something else that's exhausted.”

The phrases that identify triggered abilities do not always appear at the beginning of sentences or abilities. If an ability triggers “the [Nth] time” something happens and that [[Trigger Condition]] is met multiple times simultaneously, the ability’s controller picks one of those instances to serve as the [[Trigger Condition]]. The ability triggers only once, due to the chosen condition.

>*Example*: Wraith of Echoes reads **“The first time another friendly unit dies each turn, draw 1.”** That ability hasn’t triggered yet this turn. Two other friendly units die simultaneously (say, due to combat damage). The Wraith’s controller chooses one of those deaths to trigger Wraith’s ability.

Triggered Abilities have a [[Trigger Condition]] and a Effect.
The Effect is the [[Instructions]] that are not part of the [[Trigger Condition]].
# Presence on [[Permanent|Permanents]]
Typically active while on [[The Board]].
Triggered Abilities of [[Permanent|Permanents]] are only able to have their [[Trigger Condition]] evaluated while on [[The Board]].
# Presence on Cards Outside Of The Board
Triggered Abilities on cards outside of [[The Board]] rely on the [[Privacy]] of the zone they are in and will self-describe their context.

>*Example*: The triggered ability **"When you conquer, you may discard 1 to return this from your trash to your hand."** triggers while the card it's on is in the trash, and not anywhere else.
# Activating a Trigger Ability
When a [[Trigger Condition]] is met, a Triggered Ability behaves like an [[Activated Abilities|Activated Ability]] and is placed on [[The Chain]].

If a Triggered Ability says *“you may”* or *“they may”* as the first part of its Effect, the controller of its source will choose whether or not to perform the Triggered Ability during finalization. The decision of *“may”* when it appears in this way is solely whether or not to perform said triggered ability. If the controller of the Triggered Ability chooses not to perform that Triggered Ability during finalization, it is removed from [[The Chain]] and considered to have not triggered.

If “you may” or “they may” appears in any later part of the Effect of a triggered ability, it is decided on [[Resolution]].

>*Example*: Tideturner reads **“When you play me, you may choose a unit you control at another location. Move me to its location and it to my original location.”** This “you may” appears as the first part of its effect, so the choice represents whether or not to perform the triggered ability.
>*Example*: Ornn, Blacksmith reads **“When you play me or when I hold, look at the top 4 cards of your Main Deck. You may reveal a gear from among them and draw it. Then recycle the rest.”** This “you may” does not appear as the first part of its effect, so the choice is made on resolution. The ability is always finalized to the chain.

If a Triggered Ability contains a [[Cost within Istructions]] at the beginning of the effect or immediately following the *“you may”* or *“they may”* that appears as the first part of the effect, that [[Cost|cost]] is treated as the [[Base Cost]] of the Triggered Ability.

>*Example*: Ekko, Recurrent reads **“[[Deathknell]][>] Recycle me to ready your runes.”** In this case, **“recycle me to ready your runes”** is a [[Cost within Istructions]] that appears at the beginning of the effect of the ability, and thus “recycle me” is taken as the base cost of the triggered ability.
>*Example*: Insightful Investigator reads **“When you play me, choose an opponent. They reveal their hand. You may pay 2 XP to choose a card from their hand. If you do, they discard that card and draw 1.”** The “pay 2 XP” is a cost within instructions, but because it does not appear in the first part of the effect, it is not taken as the base cost of the triggered ability. Paying 2 XP is performed on resolution.

The [[Cost|cost]] must be paid in order to [[Finalize]] the Triggered Ability to [[The Chain]].

Triggered Abilities can be put on [[The Chain]] during [[Closed State]]s or [[Open State]]s on any player's turn.
# Simultaneous Triggers
If more than one Triggered Ability is Triggered **simultaneously**, then the player that controls the Abilities selects the order to place them on [[The Chain]]. If multiple players separately control Triggered Abilities that are Triggered simultaneously, then starting with the [[Turn Player]] and proceeding in [[Turn Order]], each player orders their Triggered Abilities on [[The Chain]].
# N Times Each Turn
Some Triggered Abilities will trigger *“once each turn,”* or *“N times each turn.”*.
Such ability will only be performed the specified number of times each turn. If its [[Trigger Condition]] would be fulfilled and it has already been performed that many times, it does not trigger.

If the Triggered Ability says *“you may”* or *“they may”* as the first part of its effect, its controller has the choice of whether or not it is performed. During [[Finalize|finalization]] of the Triggered Ability, the player who controls the Triggered Ability may choose to perform it. If they do not, it is removed from the chain.
# Common Triggered Abilities
Some Conditions are commonly used and structured in a way that explicitly defines their use and other properties of the Effect that is associated with it.
- [[Play Effects]]
- [[Targeting Effects]]
- [[Conquer Effects]]
- [[Hold Effects]]
- [[Attack Triggers]]

Some effects may instruct a player to *“activate”* one of these named triggered abilities. To do so, that player checks the condition of all of the specified effects, as if they had fulfilled the named part of the [[Trigger Condition]].

>*Example*: Reckoner’s Arena reads **“When you hold here, activate the conquer effects of units here.”** For each unit at the battlefield, you will check the trigger condition of their [[Conquer Effects]] to see if the condition has been fulfilled, treating the conquer portion of the condition as having been fulfilled. If all of the conditions are fulfilled for a conquer effect, it is placed on the chain as if it had just triggered. If any of the non-conquer parts of the condition are not fulfilled, it will not be placed on the chain.
>*Example*: A spell reads **“Activate the play effects of your gear.”** For each gear you control, you will treat it as if you had just played the gear and check the other conditions of that gear. If all of the conditions are fulfilled for a play effect, it is placed on the chain as if it had just triggered.
