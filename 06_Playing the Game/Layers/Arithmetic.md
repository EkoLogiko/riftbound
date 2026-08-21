This [[Layer]] deals with the mathematics of increasing and decreasing the numeric values of the traits of [[Game Object|Game Objects]].
- [[Might]]
- [[Energy]]
- [[Cost]]
- [[Power]]

This is the third [[Layer]] to be evaluated when evaluating [[Layer|Layers]].

When an arithmetic effect from a source that is not a [[Passive Ability]] has a limitation that applies, it is limited at the time of its application, and is “remembered” at that limited level for the duration of its effect. This process is called **“snapshotting.”**

>*Example*: If an effect gives a unit **“-4 [M] to a min of 1 this turn”** choosing a unit with 2 [M], then the effect will generate -1 [M] this turn.
>*Example*: A unit reads **“Units you control here have their Might increased to 5 [M].”** This is a passive ability, so it will not snapshot.
>*Example*: A spell reads **“Increase a friendly unit’s Might to 5 [M].”** This effect is applied once, with an unlimited duration. Because it isn’t from a passive ability, it will snapshot.

Players cannot increase a numeric attribute by a negative amount. If an effect would instruct a player to do so, they increase it by 0 instead.

>*Example*: A player plays Last Stand, which reads **“Double a friendly unit's Might this turn. Give it Temporary.”** The player declares a 2 [M] unit as the target during finalization. In reaction to Last Stand, an opponent plays Eclipse targeting the 2 [M] unit. When Last Stand resolves, the unit is -2 [M]. Last Stand instructs its controller to increase the unit’s Might by its current amount, -2, when the double action is performed. This is not possible, so the unit’s Might is increased by 0 instead.

[[Might Bonus|Might Bonuses]] of [[Attached]] cards are applied in this [[Layer]].

This layer applies arithmetic in the following way:
1) Increases
	- Positive values, or increases, to [[Might]] are applied first.
	- If there is a restriction or limitation to this increase and it isn’t from a passive ability, the limitation is **“snapshotted”** for the duration of the effect.
2) Decreases
	- Negative values, or decreases, to [[Might]] are applied last.
	- If there is a restriction or limitation to this decrease and it isn’t from a passive ability, the limitation is **"snapshotted"** for the duration of the effect.