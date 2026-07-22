---
aliases:
  - control
  - Controlled
  - controlled
  - Controls
  - controls
---
**Control** is the concept of a player having influence of a [[Game Object]] and applies differently to different [[Card Type|card types]].
# [[Battlefield]]

Control is a binary, constant state established over Battlefields through the course of play:
- *Controlled*
- *Uncontrolled*
It is also an identifier for players: is either *Controlled* by a specific player or no one.
## Establishing Control
Control can be [[Contested Control|Contested]] through the course of play.
Control is established by having [[Unit|Units]] at a [[Battlefield]] at the end of a [[Showdown]] or [[Combat]] after applying the contested status:
- If a player controls Units at a Battlefield, outside of [[Combat]], they maintain Control of that Battlefield for as long as they have Units at that Battlefield.
- While a [[Combat]] or [[Showdown]] is ongoing at a Battlefield, Control of that Battlefield cannot change until instructed by [[Steps of Combat]] or Showdown.
- If a player has no Units at a Battlefield and the turn is in an [[Open State]], they lose Control of that Battlefield in the following [[Cleanup]] unless there is a [[Combat]] or [[Showdown]] ongoing there.
## [[Ability|Abilities]] of Battlefield
Control of a [[Battlefield]] determines Control of its [[Ability|Abilities]]:
- While a Battlefield is **Controlled**, its Controller controls its Abilities unless that ability indicates another player does. The controlling player takes responsibility for adding them to the [[The Chain|Chain]] if applicable, and makes all choices required by them unless otherwise specified.
- While a Battlefield is **Uncontrolled**, its Abilities are also Uncontrolled unless that ability indicates a player controls it. If there is no such indication, the [[Turn Player]] takes responsibility for adding them to the [[The Chain|Chain]] if applicable, makes all choices required by them unless otherwise specified, and is treated as their Controller if any game rule or effect requires one.
- If an Ability of a Battlefield indicates that a specific player makes a choice, that player is the Ability’s controller. They take responsibility for adding it to the [[The Chain|Chain]] if applicable and make all choices required by the ability. They and only they control the ability, regardless of who controls the Battlefield.
- “You” in a battlefield’s abilities refers to the battlefield’s Controller, as does the implied “you” in instructions that don’t specify a player like “draw 1.” If the battlefield has no Controller, “you” refers to no one, and all such instructions are ignored.

>*Example:* The Arena’s Greatest is a battlefield that reads “At the start of each player's first Beginning Phase, that player gains 1 point.” This ability will usually trigger while the battlefield has no controller. If it does, the Turn Player goes through the steps of adding the ability to the chain and receives priority after doing so, exactly as if they controlled the ability

>*Example:* Abandoned Hall is a battlefield that reads “When a player plays a spell, they may give a unit they control here +1 might this turn.” The ability indicates that the player who played the spell makes the choice, so that player takes responsibility for putting the ability on the chain and makes all choices. They control the triggered ability.
# Control of Everything Else
When a player [[Playing a Card|Plays]], [[Hide|Hides]], or [[Create|Creates]] a Card or other [[Game Object|Game Objects]], they are established as that [[Game Object]]'s Controller.
- [[Spells]]: they are the [[Spell]]'s Controller and they choose targets, modes and pay costs for it.
- [[Permanent|Permanents]] and [[Rune|Runes]]: they become the [[Game Object]] controller when they [[Entering the Board|Enter the Board]]; they make decisions about the Game Object's [[Inherent Ability|Inherent Abilities]],  [[Unique Abilities|Unique Ability]]. any [[Game Effect|Game Effects]] or decisions necessary while the card is being played and the ones about any [[Game Effect|Game Effects]] created from "When you play me" effects of [[Permanent|Permanents]].
- [[Ability|Abilities]]: they are the [[Ability]] controller; by default, the Controller of an [[Ability's Source]] is the Controller of the Ability. If an Ability’s Source is located in a [[Non-Board Zone]], the Ability’s Controller is the [[Ownership|Owner]] of the Source. That player chooses targets, mode and pays costs for the Ability.
	- Changes to Control of an [[Ability’s Source]] do not change Control of that Ability.


When a game effect or rules text refers to the Controller of a specific object, it can be referring to either context interchangeably. The method of assignment of control is different, but the status of Control is the same across all [[Game Object|Game Objects]].