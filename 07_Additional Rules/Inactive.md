Card text can occasionally be assigned to be ignored, disregarded, or otherwise rendered as not applicable during the course of play. This state is referred to as **Inactive**. Text marked this way is not applied at all while in this state.

**Inactive** [[Ability|Abilities]] do not [[Triggered Ability|trigger]], do not apply, and cannot be [[Activated Abilities|activated]].
**Inactive** instructions are not processed.

**Inactive** text is still present on cards. Cards with **Inactive** text still have [[Keyword|Keywords]] for the sake of [[Game Effect|Game Effects]] that want to reference or see if a card has a [[Keyword]].

[[Game Effect|Game Effects]] that parse or interpret text to determine [[Target|target]] eligibility may still parse **Inactive** text for the sake of eligibility.

>*Example*: Spinning Axe is a gear with [[Temporary]]. While it’s attached and its rules text is inactive, its [Temporary] ability doesn’t trigger. However, a spell that reads **“Destroy a gear with [Temporary]”** could still choose and destroy Spinning Axe.

[[Rules Text]] **is never Inactive by default**.
[[Effect Text]] is **Inactive** unless the card with the [[Effect Text]] is [[Attached]].
# Exceptions
**Inactive** text **can partially cease to be Inactive** under specific circumstances and exceptions.
- If an [[Attached]] card has a [[Passive Ability]] or [[Replacement Effect]] that applies during the process of [[Attach|Attaching]] or a [[Triggered Ability]] that triggers off of [[Attach|Attaching]], that text exists and can be processed as it [[Attach|Attached]].
- If an [[Attached]] card has a [[Passive Ability]] or [[Replacement Effect]] that applies during the process of [[Detach|Detaching]] or a [[Triggered Ability]] that triggers off of [[Detach|Detaching]], that text exists and can be processed as it [[Detach|Detaches]].
- If an [[Attach|Attached]] card has an [[Equip]] ability, the [[Weaponmaster]] keyword can reference that [[Equip]] ability and any abilities that passively modify that [[Equip]] ability.
- If a [[Dependent Ability]] is a [[Triggered Ability]] whose condition occurs at the same time as the [[Dependent Keyword]]’s condition being fulfilled, that text exists and can be processed as it is fulfilled.