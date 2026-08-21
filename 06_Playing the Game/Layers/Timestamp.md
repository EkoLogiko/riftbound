If more than one effect applies in the same [[Layer]] but no dependency is established, then **Timestamp** order is applied to the effects within that [[Layer]] and sublayer.

When an effect begins applying, it establishes a time for which it is compared against other [[Game Effect|Game Effects]] for purposes of resolving Layered effects as its Timestamp.

**Timestamps** are not rote values. Timestamps are relative comparisons between effects and when they began applying to the game. Timestamps **are not referenced** by [[Game Effect|Game Effects]] in any way. They are only used to finalize layered effects.

When [[Rules Text]] becomes [[Inactive]] for any reason, **it loses its** **Timestamp**. When it ceases to be [[Inactive]], a **new Timestamp is established**.

Effects are applied such that the earliest **Timestamp** within each [[Layer]] and Sublayer applies first, followed by other Effects in that Layer and Sublayer in chronological order.