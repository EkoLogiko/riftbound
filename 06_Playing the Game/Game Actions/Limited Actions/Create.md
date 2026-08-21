---
aliases:
  - create
  - created
  - Created
  - creates
  - Creates
  - Creating
  - creating
---
**Creating** is a [[Limited Action]] consisting in producing a [[Game Object]] that previously did not exist in the game. Players may only **Create** [[Game Object|Game Objects]] when directed to by [[Game Effect|Game Effects]].

[[Game Effect]] that **Create** one or more [[Game Object|Game Objects]] will direct where those Game Objects must go - the Game Objects are **Created** directly to the zones in question. If a zone is not specified by the effect, the Game Object will be created to the appropriate zone for its type.
- [[Permanent|Permanents]] will be Created at any location on [[The Board]] that they can be played to.
- [[Spell|Spells]] will be Created on [[The Chain]].
- [[Rune|Runes]] will be Created at [[Base]].
- [[Champion Legend|Legends]] will be Created in the [[Legend Zone]].
- [[Battlefield|Battlefields]] will be Created in the [[Battlefield Zone]].

The zone a Game Object is created to can be specified implicitly by the [[Game Action]] being performed.

>*Example*: **“Play a 1 [M] Recruit token”** specifies a zone where the token is Created to implicitly, by specifying the token is played and thus created on the chain.
>*Example*: **“Create a 1 [M] Recruit token”** does not specify a zone, so the Recruit token will be created at any location on the board that it can be played to.

A [[Game Effect]] that Creates a [[Game Object]] will specify the state and nature of the Game Object created. If the Game Object is a [[Token]], it will follow the normal rules for tokens.

Unless specified otherwise by the Game Effect that Creates a Game Object, any such Game Object is owned by the player who Created it. [[Control]] is established as usual for Game Objects of the appropriate type.
- A Created [[Permanent]], [[Rune]], [[Champion Legend|Legend]], or [[Spell]] is controlled by its owner as it is Created.
- A Created [[Battlefield]] is **uncontrolled** as it is Created.

Prior to being **Created**, these Game Objects did not exist outside of the zone they were Created to. After being Created, they may change zones as appropriate for Game Objects of their type.

This action, when instructed, is usually formatted as *"Create [X] at [Y]" or “Add [X] to [Y].”*