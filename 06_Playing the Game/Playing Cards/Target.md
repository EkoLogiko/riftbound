---
aliases:
  - target
  - Targeted
  - targeted
  - Targets
  - targets
  - targeting
---
When a card **Chooses** one or more specific [[Game Object|Game Objects]] to affect, it is **Targeted** and becomes a **Target** unless indicated otherwise by the following rules.

In order to put a [[Spell]] or [[Ability]] on the chain, valid choices must be made for all targets.
# Valid Targets
A target is a valid choice if it meets all of the following requirements:
- It is a [[Permanent]] or [[Rune]] on [[The Board]], a [[Spell]] or [[Ability]] on [[The Chain]], a player or [[Zone]], or specified explicitly or implicitly as being in some other zone.
	- “Unit,” “gear,” and “rune” refer to objects on [[The Board]] unless specified otherwise.
	- “Spell” and “ability” refer to objects on [[The Chain]] unless specified otherwise.
	- “Facedown card” refers to a card in a [[Facedown Zone]] unless specified otherwise.
	- “Legend” refers to a [[Champion Legend|Legend]] in the [[Legend Zone]] unless specified otherwise.
	- “Chosen Champion” and “unit in the Champion Zone” refer to a unit in the [[Champion Zone]] unless specified otherwise.
- It meets all targeting restrictions.
- It is not the spell or ability itself.

>*Example*: **“Kill a unit”** targets a unit on the board.
>*Example*: **“Recycle a unit from your trash”** targets a unit card in your trash.
>*Example*: A unit is a valid target for a spell that refers to a **“unit at a battlefield,”** **“enemy unit,”** **“unit you control,”** or **“unit with Might 4 or greater”** only if it meets the appropriate criteria.
>*Example*:  A unit that reads **“I can’t be chosen by enemy spells or abilities.”** is not a valid target for any enemy spell or ability, even if it meets other targeting restrictions.
>*Example*: A spell that says “Counter a spell” cannot target itself.
>*Example*: An ability of a permanent can target that permanent, because abilities and their sources are separate objects.
# What is a Target
A [[Game Object]], player, or zone mentioned in the text of a [[Spell]], [[Activated Abilities|Activated Ability]], or [[Triggered Ability]] is a target **UNLESS** any of the following are true:
- It is in a zone whose information status is not [[Public Information]]. Public zones are: 
	- [[Battlefield Zone|Battlefield Zones]]
	- [[Base|Bases]]
	- [[Trash|Trashes]]
	- [[Legend Zone|Legend Zones]]
	- [[Champion Zone|Champion Zones]]
	- [[Facedown Zone|Facedown Zones]]
- It is included only as part of a targeting restriction for another choice or only as a restriction or permission for a game action.
- It is included only as part of a [[Cost]], [[Trigger Condition]], or [[Replacement Effect]]. This includes [[Cost within Istructions]], identified by phrases like “[do X] to [do Y].” The cost within that instruction is “[do X].”
- It is programmatically selected based on its characteristics rather than chosen by the [[Spell|spell]] or [[Ability|ability]]’s controller. This exception applies solely to objects for which no choice is ever possible. This exception does not apply to objects that are the only valid choice at the moment a spell or ability is placed on the chain, but which would require a choice under other circumstances.
- It is part of a set of objects chosen in whole or in part by other players.
- It is identified in an instruction that a player **“must”** complete.

>*Example*: **“Ready a legend”** targets a legend, because the Legend Zone is Public.
>*Example*: **“Return a unit from your trash to your hand”** targets a unit card in your trash, because your trash is Public.
>*Example*: **“You may play a unit from your hand, ignoring its costs”** does not target a unit card in your hand, because your hand is not a public zone.
>*Example*:  **“Kill a unit at a battlefield”** targets a unit, but not a battlefield, because the units are targets and “at a battlefield” is a restriction.
>*Example*: **“Kill all units at a battlefield”** targets a battlefield, but not any units.
>*Example*: **“Kill all units at battlefields”** doesn’t target anything.
>*Example*: **“Play a unit from your hand to a battlefield”** doesn’t target a battlefield.
>*Example*: **“As an additional cost to play me, kill a friendly unit”** doesn’t target anything.
>*Example*: **“When a friendly unit dies, kill a gear”** targets a gear, but not a friendly unit.
>*Example*: **“When you play me, the next time a friendly unit would die this turn, return it to your hand instead”** doesn’t target anything. The replacement effect applies when any friendly unit dies.
>*Example*:  **“Choose a friendly unit. The next time it would die this turn, return it to your hand instead”** targets a friendly unit, because **“choose a friendly unit”** is not part of the replacement effect.
>*Example*: **“When I hold, you may kill another friendly unit here to draw 1”** does not target anything.
>*Example*: **“When you play me, you may spend a buff to move a friendly unit”** targets the friendly unit, but not the buff.
>*Example*: **“Kill a unit. Its controller draws 2”** targets the unit, but not its controller.
>*Example*: **“Ready your legend”** doesn’t target anything, because you can only have one legend.
>*Example*: **“Ready a friendly legend”** targets a legend, because in a 2v2 game there are two friendly legends.
>*Example*: **“Recycle all cards in your trash”** doesn’t target anything, because it affects all cards and you only have one trash.
>*Example*: **“Each player kills a unit they control”** does not target. Each player, including the one who played the spell, chooses a unit to kill as the spell or ability resolves.
>*Example*: **“You must recycle one of your runes”** doesn’t target anything. You choose from among your runes as the spell or ability resolves.
>*Example*: **“Recycle a rune you control”** targets a rune. You choose a rune you control as you put the spell or ability on the chain.
# Groups of Targets
Some cards identify a group of **Targets** with **Targeting Requirements** that must be met by the group as a whole. As they’re finalized on [[The Chain]], such cards can choose any group of valid targets that collectively fulfill the targeting restriction.

If the group of targets no longer collectively fulfill the targeting restriction as the [[Spell|spell]] or [[Ability|ability]] resolves, that spell or ability’s controller can choose a **subset** of the original targets that fulfills the targeting requirement for the spell or ability to affect.

If a [[Spell|spell]] specifies that a player may perform a [[Game Action]] on some number of [[Game Object|Game Objects]], then all choices are considered targeted and chosen independently of the decision to perform the [[Game Action]].

If a card specifies that a player chooses “any number” or “up to” some number of [[Game Object|Game Objects]] to be affected, they may choose any number of available targets, including zero. If they choose zero, the spell or ability can be played without any targets.

Some cards **split** [[Damage]]. Every [[Unit]] affected by the [[Splitting]] mechanic is a Target.

>*Example*: A player plays Fox-Fire, a spell that says in part **“Kill any number of units at a battlefield with total Might 4 or less.”** That player chooses four 1 [M] Recruit tokens at a single battlefield. As a Reaction, another player gives two of those Recruits +1 [M], so the Recruits’ Mights are 1, 1, 2, and 2. Then Fox-Fire resolves. The Recruits no longer have total Might 4 or less, so Fox-Fire’s controller must choose a legal subset of the original targets to affect. They could choose to kill the two 2 [M] Recruits, or the two 1 [M] Recruits plus one 2 [M] Recruit. The units they choose are Fox-Fire’s remaining legal targets. They can’t choose to affect units at the same battlefield that weren’t initially chosen as targets. They can, however, choose to affect units that were initially chosen as targets that left the chosen battlefield before Fox-Fire resolved as long as those units are all located at the same battlefield.