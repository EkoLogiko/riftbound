---
aliases:
  - Split
  - Splits
---

If a card specifies that an amount of [[Damage]] may be **split** among some number of [[Unit|Units]], then each Unit chosen is [[Target|Targeted]]. The [[Target|Targets]] are chosen when the [[Spell|spell]] or [[Ability|ability]] is finalized on [[The Chain]].

A number of Targets can only be chosen up to, and not exceeding, the initial amount of [[Damage]] available when the spell is played.

>*Example*: A player playing a spell that instructs them to "Split 5 damage" may only choose up to 5 units, but may choose fewer.

Each Target is valid, and contributes to Targeting Effects individually.

The choice of how much [[Damage]] is divided across the split is not decided until the resolution of the [[Spell|spell]] or [[Ability|ability]]. Each [[Target]] must receive a valid amount of [[Damage]]: valid damage is a positive integer amount, greater than or equal to 1 damage.

If, at resolution of the [[Spell|spell]] or [[Ability|ability]], there are more [[Target|Targets]] than available damage to divide, then the player who controls the effect dealing [[Damage]] determines which Targets cease being Targets. That player cannot choose to have fewer Targets than they have damage to split when choosing which Targets cease being Targets. Any costs that were paid, or effects that were triggered as a result of those [[Game Object|Game Objects]] being chosen as Targets remain in effect, paid, or otherwise triggered.

>*Example*: A player plays Alpha Strike, which reads in part **“Choose a friendly unit. It deals damage equal to its Might split among enemy units at battlefields.”** They target their 5 [M] unit and five 1 [M] enemy Recruits at battlefields. In reaction, their opponent plays Feral Strength targeting one of their recruits, and Frigid Touch targeting the 5 [M] unit. When Alpha Strike resolves, they have 3 damage to split, and must choose which targets cease being targets. They can’t choose for 4 of the units to cease being targets so that they can deal 3 to the 3 [M] recruit. They can only choose at most 2 of the targets to cease being targets.

These choices cannot be changed after this step unless instructed to by a [[Spell|spell]] or [[Ability|ability]].

A player may not make choices during this step that will deterministically result in illegal choices or actions later in this process unless they have no choice. 

>*Example*: A player plays a card which reads **“As an additional cost to play this, kill the unit you control with the most Might. Give a friendly unit +[M] equal to the killed unit’s Might this turn. Predict 2.”** They cannot choose to target their unit with the highest Might during this step of finalization.