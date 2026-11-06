This [[Layer]] deals with all **copy effects**.

This is the first [[Layer]] to be evaluated when evaluating [[Layer|Layers]].

When a **Copy effect** is applied to a [[Game Object]], the traits specified by the Copy Effect replace or are added to the Copyable Traits of the Game Object being Copied as specified by the effect. If no traits are specified by a Copy Effect, all traits of the Game Object are
replaced with those of the Copied Game Object.
>*Example*: A player triggers Leblanc, Deceiver’s hold effect and plays a Reflection token, making it a copy of Honest Broker. That player then plays Mirror Image, targeting the Reflection token. When the Mirror Image Reflection token is played, it copies all of the copyable traits of the original Reflection token - which are currently those of Honest Broker which it is a copy of. That player will have three units named Honest Broker in play, two of which are token Copies with Temporary.

Effects for this [[Layer]] can be identified by the phrase *"copy"* in the text.
# Copyable Traits
The **copyable traits** of a Game Object are all of the printed—or if a copy effect is applied, copied—traits of that Game Object. In the case of a [[Token]], they are the traits the token had when it was [[Create|created]].

**Copyable traits** of a Game Object are distinct from the actual traits of that Game Object, which may be modified by subsequent applied [[Layer]] effects.
## List of Copyable Traits
- [[Card Name]]
- [[Supertype]]
- [[Card Type]]
- [[Tag|Tags]]
- [[Cost]]
- [[Domain]]
- [[Rules Text]]
- [[Effect Text]]
- [[Might]]
- [[Might Bonus]]
- [[Flavor Text]]
- Art