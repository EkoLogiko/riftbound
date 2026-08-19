Some information used by [[Ability|abilities]] is referenced from the source of those abilities, or from one or more targets of a [[Spell|spell]] or [[Ability|ability]]. This can usually be recognized by the presence of words like *“here,”* *“my,”* or *“its.”*
Information referenced in an instruction in this way will be checked on execution of the instruction.

>*Example*: A player moves Yasuo, Remorseful to an occupied enemy battlefield and initiates combat there. In reaction to the Yasuo, Remorseful attack trigger, their opponent plays Fight or Flight from hidden targeting Yasuo, moving him back to base. When the attack trigger resolves, *“here”* is no longer the battlefield where combat is ongoing and the attack trigger mistargets.
>*Example*: In reaction to a Yasuo, Remorseful attack trigger, an opponent plays Stupefy targeting Yasuo. When Yasuo’s attack trigger resolves, it will deal damage equal to his current Might of 5.

When a referent checks information on execution of the instruction related to a [[Target]], and that target isn’t legal, that referent will return “null” and all instructions related to it will be ignored.
# Referents and [[Triggered Ability|Triggered Abilities]]
Some information used by [[Triggered Ability|Triggered Abilities]] is referenced from the trigger condition of the ability. This information is checked when the trigger condition is fulfilled.

>*Example*: Lillia, Fae Fawn reads **“when I move from a location, play a 3 [M] Sprite token with Temporary there.”** If Lillia moves to a battlefield, her triggered ability will be placed on the chain and it will note the location she moved from when it does so. If she moves to a non-board zone in reaction to the triggered ability on the chain, it will not affect where the Sprite token will be played when the triggered ability resolves.

In the case of a [[Delayed Trigger]]'s ability, the information is referenced when the triggered ability is created unless specified otherwise.

In the case of a [[Linked Ability]] that references information from a linked triggered ability, that information may be referenced from the trigger condition of the linked triggered ability if specified.

>*Example*: Iascylla reads **“When I hold, at the start of your next Main Phase, you may move an enemy unit to this battlefield.”** The *“this battlefield”* in her [[Delayed Trigger]] ability refers to the battlefield she held, and so will be referenced from the trigger condition, when the triggered ability is generated.

Some information used by the effect of a [[Triggered Ability]] is referenced from the triggered ability itself, such as *“enemy”* and *“friendly”* status. This information is checked on execution of the referencing instruction.

>*Example*: Yasuo, Remorseful reads **“when I attack, deal damage equal to my Might to an enemy unit here.”** Yasuo moves to an occupied enemy battlefield and his attack trigger goes on the chain. In reaction to the attack trigger, the defending player plays a hidden Hostile Takeover and gains control of Yasuo. The triggered ability is unaffected by Yasuo changing controllers, and “enemy” is in reference to the triggered ability itself, so it will resolve with no issue.
>*Example*: In reaction to the same Yasuo, Remorseful trigger, say the defending player had instead played a spell that reads **“[[Reaction]]. Gain control of a triggered ability. You may make new choices for it.”** They chose the attack trigger. When Yasuo’s attack trigger resolves, if they didn’t make new choices for the trigger, the controller of the triggered ability will no longer be an enemy to the targeted unit, so the triggered ability will [[Mistargeting|mistarget]] and do nothing. If they instead chose Yasuo with the attack trigger, he would be an enemy unit to the triggered ability and so it would deal damage equal to his Might to himself.