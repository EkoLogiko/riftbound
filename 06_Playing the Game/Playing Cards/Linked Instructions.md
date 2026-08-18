Some instructions may reference [[Game Object|Game Objects]] affected by, or [[Game Action|Game Actions]] performed in, other instructions in a card. The referenced and referencing instructions are called “linked instructions.”

>*Example*: Hidden Blade reads **“Kill a unit at a battlefield. Its controller draws 2.”** The **“its”** in the second instruction references the unit in the first, so the two instructions of the spell are linked.

In order for a later linked instruction to execute, its earlier linked instruction must have executed. If the earlier linked instruction is ignored for any reason, the later linked instruction will also be ignored.

>*Example*: Hidden Blade reads **“Kill a unit at a battlefield. Its controller draws 2.”** If the chosen unit changes zones or moves to base in reaction to Hidden Blade, the spell will [[Mistargeting|mistargets]] and the first instruction will be ignored. If the first instruction is ignored, the second instruction will not execute and the unit’s controller will not draw 2.

If the [[Game Action]] performed in an earlier linked instruction is replaced, this will not affect the later linked instruction, unless the later linked instruction directly references the [[Game Action]] being performed.

>*Example*: Hidden Blade reads **“Kill a unit at a battlefield. Its controller draws 2.”** This effect is split into two instructions: killing the unit and the targeted unit’s controller drawing 2. The later linked instruction doesn’t reference an action directly, so it will execute even if the kill action of the earlier linked action is replaced by some other event.
>*Example*: Deathgrip reads **“Kill a friendly unit. If you do, give +[M] equal to its Might to another friendly unit this turn.”** If the friendly unit in question is not killed by Deathgrip because its death is replaced with another event, the later linked instruction will not execute because **“if you do”** directly references the game action