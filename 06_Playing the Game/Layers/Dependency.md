If more than one effect applies to the same [[Game Object]] in the same [[Layer]], or to each other in the same layer, then both effects will apply but their order may be determined by **Dependency**.

A **Dependency** is established if at least one of the following is true:
- Applying one of the effects alters the existence of the other.
- Applying one of the effects alters the number of objects the other effect can influence.
- Applying one of the effects alters the outcome when applying the other.

To determine which effect **Depends** on another, determine which of the prior criteria applies, and then also which effect’s evaluation is altered by the sequence of applications. That effect is said to **Depend** on the other.

>*Example*: A unit with 4 [M] is under the effects of a passive ability that reads **“Units you control here have their Might increased to 5 [M].”** Its controller plays Discipline on the unit, giving it +2 [M]. When applying Layer alterations, both effects are applied in the same layer. If we apply the passive ability first, the passive ability will give +1 [M] while the Discipline effect will give +2 [M]. If we apply them in the other order, the Discipline effect will give +2 [M], and the passive ability will give +0 [M]. The passive ability is altered by the sequence of applications, so it depends on the Discipline effect.

If both effects are altered by the application of the other, no **Dependency** can be established.

>*Example*: A unit with 4 [M] is under the effects of a passive ability that reads **“Units you control here have their Might increased to 5 [M].”** Its controller plays a spell that reads **“Give a unit +2 [M], to a maximum of 5 [M].”** If we apply the passive ability first, the passive ability will apply +1 [M] and the spell effect will apply +0 [M]. If we apply the spell effect first, it will apply +1 [M] while the passive ability applies +0 [M]. Both effects are altered by the sequence of applications, so we can’t establish a dependency.

To resolve a **dependency**, the effects within the same layer that created the dependency must be applied such that:
1) Identify which effect **Depends** on the other within the [[Layer]].
2) Apply the effect that is depended on first.
3) Immediately apply the effect that **Depends** on the first effect next.

>*Example:* A unit with 4[M] is under the effects of a passive ability that reads **“Units you control here have their Might increased to 5 [M].”** Its controller plays Discipline on the unit. As previously established, the passive ability depends on the Discipline effect. We apply the Discipline effect first, giving the unit +2 [M], and then immediately apply the passive ability that depends on it. The unit’s final Might is 6 [M].

If more than one effect applies in the same layer but no dependency is established, then [[Timestamp]] order is applied to the effects within that layer and sublayer