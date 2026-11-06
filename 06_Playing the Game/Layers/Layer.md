---
aliases:
  - Layers
---
**Layers** are the mechanism in which [[Game Effect|Game Effects]] alter the **Traits**, Intrinsic Abilities, or other properties of [[Game Object|Game Objects]].

**Layers** are an organizational structure. Layers only serve to structure the application and order that [[Game Effect|Game Effects]] apply to [[Game Object|Game Objects]] to maintain consistency.

The layers are applied repeatedly until all effects operating on objects **have been applied once and no changes have been processed.**
**Layers** are applied and evaluated continuously. All [[Game Object|Game Objects]] have their layers updated in the same instant, but each [[Game Object]] is treated separately and individually when evaluating layers.

# Layers Evaluation
## Official
If evaluating a [[Game Effect]]'s applicability depends on information from one or more other [[Game Object|Game Objects]], that [[Game Effect]] has an **object level dependency (OLD)**. Pausa evaluating the layers of the dependent [[Game Object]] and evaluate the layer effects of those [[Game Object|Game Objects]] whose information is references. Continue once the applicability of that [[Game Effect]] has been established or disqualified.
>*Example*: A 4 [M] unit reads in part “While I’m [Mighty], I’m a Yeti.” Another unit reads in part “I have all tags of units you control.” When the 4 [M] unit is buffed, the layers for all game objects are evaluated. While evaluating the layers for the second unit, it requires us to pause and evaluate the layers for all other units. When we’re evaluating the layers for the 4 [M] unit, after all is said and done, the unit has the Yeti tag. Once we’ve evaluated all units, we go back to evaluating the second unit, and at that time it has the Yeti tag as well.
## OR, UNOFFICIALLY BUT WAAAAAAY MORE CLEARER:
Sometimes you can’t work out an effect on one object without first knowing something about another object. For example, “I have all tags of units you control” has to look at the other units’ tags.

When this happens, finish the other object first:
1. Pause the object you’re working on.
2. Fully work out the object(s) it’s looking at, applying all their effects.
3. Resume the first object, using those finished values.

>*Example*:
>- **Unit A** has 4 Might and reads: _“While I’m [Mighty], I’m a Yeti.”_ (Mighty means 5+ Might.)
>- **Unit B** reads: _“I have all tags of units you control.”_
>You buff Unit A, so it now has 5 Might. Does Unit B have the Yeti tag
>Unit B’s effect needs Unit A’s tags, so you pause B and finish A. A has 4 + 1 = 5 Might, so it’s Mighty and gains Yeti. Then you resume B, which now sees Yeti and copies it.
>**Result:** both units are Yetis, whichever one you look at first.
## Back to Official... for 2+ OLD
If a [[Game Object]] has an **OLD** with a Game Object that itself has an **OLD** with a third Game Object and so on, determine the final point of the dependency chain and evaluate the layer effects of that Game Object first, continuing up the dependency chain until all Game Objects have had their layer effects evaluated.
## Circular OLDs
If a dependency chain loops back around on itself, identify the minimum set of Game Objects in the loop and evaluate their layer effects simultaneously, layer by layer. If any of them have Game Effects that reference Game Objects from outside the set, pause and evaluate those Game Objects first before continuing with the set.
>*Example*: A 4 [M] unit reads “If there is a [Mighty] enemy unit here, I have +5 [M].” Both players control one of these units at a battlefield during combat. Each one is buffed. A third player plays Siphon Power, which reads “Choose a battlefield. Give friendly units there +1 [M] this turn, and enemy units there -1 [M] this turn, to a minimum of 1 [M].” Both of the units there are given -1 [M]. Because they have effects that reference each other, they have a dependency chain. After evaluating their layers simultaneously, layer by layer, both units will be 4 [M].
# Layers Application
Layers are applied in sequence. Each effect in them is applied as soon as able, and only a single time across all sequences. When a sequence of applications completes, recur the process, and evaluate each layer again applying any effects that may now be applicable.
The removal or disqualification of an effect is separate from the application of the effect, but still can only be applied once.

>*Example*: Fiora, Victorious has printed Might 4 and says **“While I'm Mighty, I have Deflect, Ganking, and Shield.”** If a player places a buff on Fiora, her Might is increased in the Arithmetic layer, after the layer for Ability-Altering Effects. The Ability-Altering Effect layer is then re-checked and the abilities Deflect, Ganking, and Shield applied. Since each effect has been applied once and there are no other effects to apply, Fiora’s characteristics are finalized as 5 Might with Deflect, Ganking, and Shield. While a buffed Fiora, Victorious is in combat as a defender, an additional +1 Might will be applied in the Arithmetic layer, giving her 6 Might and the 3 keywords.
>*Example*: A buffed Fiora, Victorious is in combat as a defender when her buff is removed. Reevaluating the layers in sequence, she no longer gains Deflect, Ganking, and Shield during the Ability-Altering Effect layer, so when the Arithmetic layer is evaluated, neither the buff (which is gone) nor Shield (which she no longer has) apply. She goes directly from 6 Might with three keywords to 4 Might with no keywords.

Layers are applied in the following order:
1) [[Copy Effects]]
2) [[Trait-Altering Effects]]
3) [[Ability-Altering Effects]]
4) [[Arithmetic Effects]]

If more than one effect applies to the same [[Game Object]] in the same Layer, or to each other in the same layer, then both effects will apply but their order may be determined by [[Dependency]].