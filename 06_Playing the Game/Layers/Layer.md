---
aliases:
  - Layers
---
**Layers** are the mechanism in which [[Game Effect|Game Effects]] alter the **Traits**, Intrinsic Abilities, or other properties of [[Game Object|Game Objects]].

**Layers** are an organizational structure. Layers only serve to structure the application and order that [[Game Effect|Game Effects]] apply to [[Game Object|Game Objects]] to maintain consistency.

The layers are applied repeatedly until all effects operating on objects **have been applied once and no changes have been processed.** Layers are applied in sequence. Each effect in them is applied as soon as able, and only a single time across all sequences.
When a sequence of applications completes, recur the process, and evaluate each layer again applying any effects that may now be applicable.

The removal or disqualification of an effect is separate from the application of the effect, but still can only be applied once.

>*Example*: Fiora, Victorious has printed Might 4 and says **“While I'm Mighty, I have Deflect, Ganking, and Shield.”** If a player places a buff on Fiora, her Might is increased in the Arithmetic layer, after the layer for Ability-Altering Effects. The Ability-Altering Effect layer is then re-checked and the abilities Deflect, Ganking, and Shield applied. Since each effect has been applied once and there are no other effects to apply, Fiora’s characteristics are finalized as 5 Might with Deflect, Ganking, and Shield. While a buffed Fiora, Victorious is in combat as a defender, an additional +1 Might will be applied in the Arithmetic layer, giving her 6 Might and the 3 keywords.
>*Example*: A buffed Fiora, Victorious is in combat as a defender when her buff is removed. Reevaluating the layers in sequence, she no longer gains Deflect, Ganking, and Shield during the Ability-Altering Effect layer, so when the Arithmetic layer is evaluated, neither the buff (which is gone) nor Shield (which she no longer has) apply. She goes directly from 6 Might with three keywords to 4 Might with no keywords.

Layers are applied in the following order:
1) [[Trait-Altering Effects]]
2) [[Ability-Altering Effects]]
3) [[Arithmetic]]

If more than one effect applies to the same [[Game Object]] in the same Layer, or to each other in the same layer, then both effects will apply but their order may be determined by [[Dependency]].