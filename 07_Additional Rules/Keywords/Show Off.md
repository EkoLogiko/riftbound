**Show Off** is a [[Passive Ability]] [[Keyword]], normally present on Cards, and is formatted as “[Show Off] [Object].”

The “[Object]” in this ability could be one object or multiple; object/s of a given type; or it could have further specifications on qualities of the object/s. The object in question could be Game Objects on [[The Board]] or cards in [[Hand]].

>*Examples*:
>-A card reads “[Show Off] a unit.”
>-A card reads “[Show Off] a card with Energy cost [7] or more.”
>-A card reads “[Show Off] five units with different names.”

**Show Off** is functionally short for *“As you play [me/this], you may reveal [Object] from your hand and/or pick [Object] from among friendly game objects on the board.”*

**Showing Off** one or more Cards or Game Objects in this way can be referenced by [[Linked Ability|Linked Abilities]] and [[Instructions]].
>*Example*: A unit reads in part “[Show Off] five units with different names,” and “When you play me, kill all other units. If you showed off, the next unit you play this turn costs [1] less for each killed unit.”

The decision of whether or not to **Show Off** is made by the controller of the [[Chain Item]] with **Show Off** during the process of [[Finalize|finalizing]] it.

If [Object] is a set of Cards or Game Objects, that set can be composed of Game
Objects on [[The Board]] as well as Cards in [[Hand]], as long as the composed set
satisfies the **Show Off** condition.
>*Example*: A unit reads in part “[Show Off] five units with different names.” When showing off as part of playing that unit, units may be revealed from hand or picked from among friendly units on the board, as long as the group of units picked and revealed satisfies the specified quality.

If some or all of the [Object] set leave the appropriate zones during the finalization process after being shown off, it will not prevent the source of the **Show Off** ability from becoming a [[Finalized Chain Item]].
>*Example:* A spell reads “[Show Off] a Mech” and “As an additional cost to play this, discard 1.” When finalizing the spell, the same Mech being shown off can be discarded to the mandatory additional cost without preventing the spell from being finalized.

[[Linked Ability|Linked Abilities]] and [[Instructions]] can reference information about the shown off object/s.
The information referenced in this way is checked when the card/s in question are shown off during finalization. Any later changes to the shown off objects will not be considered.
>*Example*: Primordial Roar is a spell that reads “[Show Off] a unit,” and “If you showed off a unit, deal damage equal to that unit's Might to a unit.”
>*Example*: Primordial Roar is played showing off a friendly unit with 4 [M] and an enemy unit with 3 [M]. In reaction to Primordial Roar, an opponent plays Frigid Touch, giving the friendly unit -2 [M] this turn. Because the information was checked when the friendly unit was shown off, the spell still deals 4 damage to the enemy unit, killing it.

Multiple instances of **Show Off** are treated separately.
If a linked effect or instruction refers to an instance of **Show Off**, it refers to the [[Tank]] granted by the same source unless specified otherwise or there is no keyword granted by the same source.
If the linked effect or instruction specifies information about the shown off card, it is linked to only that instance of the Show Off keyword. If there is no linked keyword, an ability that references showing off is linked to all Show Off keywords on the appropriate card.
>*Example*: A card reads in part “Spells you play have ‘[Show Off] a Mighty unit.’ and ‘If you showed off, this costs [A] less.” If a spell that reads in part “[Show Off] a spell with Energy cost [7] or more,” and “If you showed off, this can’t be countered.” is played by the same controller, showing off a Mighty unit will not be sufficient to satisfy both abilities that reference showing off because they refer to instances of the show off keyword granted by different sources.

**Show Off**, and whether or not a card has **Show Off**, is a characteristic of the card and may be checked or referenced by other [[Game Effect|Game Effects]].