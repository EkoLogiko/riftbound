
(Also see [[Mistargeting]])
(Also see [[Linked Instructions]])
(Also see [[Referents]])

A [[Spell|spell]] or [[Ability|ability]] resolves even if some or all of its [[Target|targets]] are illegal. A target is illegal as the spell resolves if it no longer meets the targeting requirements of the spell, or if it has changed [[Zone]] to or from a [[Non-Board Zone]].

>*Example*: An enemy unit at a battlefield is no longer a legal target if it is no longer an enemy, no longer a unit, or no longer at a battlefield. 
>*Example*: A unit with 3 or less Might is no longer a legal target if it is no longer a unit or if its Might is greater than 3.
>*Example*: Something that's exhausted is no longer a legal target if it is no longer exhausted. (It can't stop being "something.")

If a target ceases to meet the targeting requirements while the spell is on the chain, then meets them again, it's a legal target.
>*Example*: A spell targets **"a unit at a battlefield."** A player reacts with a spell that moves the unit to base, then another player reacts with a spell that moves it back to that battlefield, then the original spell resolves. The unit is a legal target.

If a target changes [[Zone]] to or from a [[Non-Board Zone]] and then returns to its original zone, it is no longer a legal target, because it's not treated as the same object.

If any of the spell's targets are no longer legal, those [[Game Object|Game Objects]], players, or zones are unaffected by the spell as it resolves. Any instructions related to an illegal target can’t be followed. Instructions that can't be followed, either because of illegal targets or other circumstances, are ignored.

>*Example*: A player plays Void Seeker, a spell that says **"Deal 4 to a unit at a battlefield. Draw 1."** The unit's controller uses a [[Reaction]] to move the unit to their base. Since the unit is no longer a legal target, it is not dealt any damage. Void Seeker's controller still draws 1.
>*Example*: A player plays Bellow’s Breath targeting a unit in combat that reads in part “I can’t be chosen by enemy spells and abilities unless I’m in combat.” In reaction, that unit’s controller plays Flash, moving the unit to their base. The unit is no longer in combat, so it is no longer a legal target for Bellow’s Breath. The unit will be unaffected by Bellow’s Breath as it resolves.
>*Example*: A player plays Hidden Blade from the facedown zone at a battlefield, targeting an enemy unit. In reaction to Hidden Blade, their opponent plays Tideturner from facedown at another battlefield, choosing to swap locations with the unit Hidden Blade targeted. When Hidden Blade resolves, the chosen unit is no longer at the appropriate battlefield, so any instructions related to that unit are ignored.
>*Example*: A player plays Ride the Wind choosing to move their unit at Vilemaw’s Lair to base. Base is a legal move destination for Ride the Wind, but on resolution of Ride the Wind’s effect, the move instruction will be ignored because Vilemaw’s restriction makes the instruction impossible.

Instructions that can be partially followed are followed as much as possible and ignored otherwise
>*Example*: A player plays a spell that says **"Discard 2, then draw 2."** If their hand is empty, the instruction to discard 2 will be ignored. They'll still draw 2. If they had 1 card in hand, they would discard it and draw 2.

If the spell checks information about a target that is no longer legal or a card or permanent whose location, zone, or status has changed such that that information is no longer available, that check returns "null" and all calculations based on it are ignored.
>*Example*: A unit that is no longer on the board is treated as having null Might, null cost, etc.
>*Example*: A unit that is no longer on the board has no location, is neither exhausted nor readied, etc.
>*Example*: Baited Hook says **"[1][C], [E]: Kill a friendly unit. Look at the top 5 cards of your Main Deck. You may banish a unit from among them that has Might up to 1 more than the killed unit and play it, ignoring its cost. Then recycle the rest."** While Baited Hook’s ability is on the chain, an opponent reacts with a spell that returns the friendly unit to its owner's hand. Because the friendly unit is no longer a legal target, it can't be killed and its Might is treated as null. Baited Hook’s controller looks at the top 5 cards of their Main Deck, but can’t choose any unit from among them.
>*Example*: Strike Down reads **“Choose an equipped friendly unit. It deals damage equal to its Might to an enemy unit. Then detach an Equipment from it.”** While Strike Down is on the chain targeting a unit with only one Equipment attached to it, that unit has its Equipment detached via Angle Shot. When Strike Down goes to resolve, the targeted unit is no longer legal, so the unit’s Might will return as “null” and the instructions related to it are ignored.

If the spell checks information about a target that is legal or a card or permanent whose location, zone, or status has not changed such that information is no longer available, that information is accessible.

A spell or ability that moves something to a different zone as a cost or effect can "look back" at its characteristics before it changes zones.

A spell or ability that leaves [[The Chain]] during the process of its resolution will cease further execution of its instructions. This immediately causes the spell or ability to finish resolving.

If a [[Delayed Ability]]’s duration has ended before it was generated, the Delayed Ability is not generated and any instructions related to it are ignored.

>*Example*: Targon’s Peak is a battlefield that reads in part **“When you conquer here, ready up to 2 runes at the end of this turn.”** If Targon’s Peak is conquered during the Ending Phase after the beginning of the ending step, such as via an effect like thrill of the Hunt, the [[Delayed Trigger]] will not be generated.
>*Example*: Akshan, Mischievous reads in part “When you play me, if you paid the additional cost, move an enemy gear to your base. You control it until I leave the board. If it's an Equipment, attach it to me.” If Akshan leaves the board in reaction to his play effect, the [[Delayed Passive Ability]] “You control it until I leave the board,” will not be generated. You will not gain control of the targeted gear even for a moment