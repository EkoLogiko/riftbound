---
aliases:
  - Preventing
  - prevent
  - Prevents
  - prevents
  - preventing
  - Prevented
  - prevented
---
**Preventing** [[Damage]] is a [[Limited Action]] and a [[Delayed Replacement]] consisting in reducing the [[Damage]] a set of [[Game Object|Game Objects]] would take. **Prevent** is an action that interacts with [[Damage]]. Players may only Prevent Damage when directed to by [[Game Effect|Game Effects]].

Prevent includes any applied [[Bonus Damage]] when determining the total damage being prevented.

Prevent appears in statements that define an amount of damage and the source of the damage it will affect, as well as the timespan it will be relevant for.

Prevent **will always apply to the next damage** that would be dealt to a unit affected by the Prevent action.

Prevent actions are usually formatted as *“Prevent the next X [source] damage that would be dealt to a [unit] this turn.”* The X is referred to as the **Prevent Value**. X can be *“All,”* which specifies an infinite amount of damage.

When damage is Prevented, it is replaced with an event where it deals that much damage reduced by the **Prevent Value** tracked on the [[Unit]] specifically. The damage being dealt as a result of Preventing can never be less than 0, but can be 0. This is equivalent to not dealing damage. Damage dealt to a Unit that has that all of that damage Prevented is not considered to have been dealt to it at all.

When damage is dealt this way, reduce the **Prevent Value** being tracked on the Unit affected by the Prevent action by the prevented amount, then:
- If the Prevent Value is 0 or less, then Prevent is no longer being tracked on the [[Unit]] in question, and the effect expires.
- Else, the reduced value is the newly tracked Prevent Value.
- If the Prevent Value is “All” then it remains “All.”
# Prevent in [[Combat]]
[[Damage]] can still be assigned to [[Unit|Units]] in [[Combat]] that are affected by **Prevent**. The damage dealt as a result of that assignment will be affected by the Prevent action.
Damage can be assigned to a [[Unit]] up to a value that would be [[Lethal Damage]] considering the Prevent Value of all Prevent Actions on a Unit, following the normal rules for [[Damage Assignment]]. No amount of damage is ever considered lethal if the Prevent Value is “All.”

>*Example*: A unit with 2 [M] is being assigned damage in the combat damage step. The unit has “prevent the first 3 damage I would take each combat.” The unit would need to be assigned 5 damage in order to have lethal damage assigned to it.