A **Cleanup** will be made an [[Outstanding Task]] at the following times:
- After the game transitions to or from an [[Open State||Open]] or [[Closed State|Closed]] state.
- After the game transitions between [[Turn Phases|Phases]], unless specified otherwise.
- After a [[Pending Chain Item]] is added to [[The Chain]].
- After a [[Pending Chain Item]] becomes a [[Finalized Chain Item]] on [[The Chain]].
- After a [[Chain Item]] is removed from [[The Chain]] for any reason.
- After any number of [[Game Object|Game Objects]] enter or leave [[The Board]].
- After the status of any number of [[Game Object|Game Objects]] changes for any reason.
- After a [[Move]] is completed.

While a Cleanup is occurring, [[Chain Item|Chain Items]] cannot be [[Finalize|Finalized]] or [[Resolution|Resolves]]. New [[Pending Chain Item]] can be added, but [[Finalized Chain Item|Finalized Items]] cannot be executed and [[Priority]] and [[Focus]] are not passed or awarded.
Similarly, while Chain Items are Resolving, a Cleanup cannot occur. If an event occurs during the Resolution of a Chain Item that qualifies for a Cleanup, that Cleanup will be made an [[Outstanding Task]].

If an event occurs during a Cleanup that qualifies for a Cleanup, another Cleanup will occur immediately after the first completes, repeating until a Cleanup occurs with no new change in the game’s state. These new Cleanups are themselves Outstanding Tasks.
# Outstanding Tasks
When a Cleanup occurs, the following Tasks become Outstanding in the order described:
1) If a player has points greater than or equal to the [[Victory Score]], and more points than any opponent, that player [[Winning|wins]].
2) Assign or Remove the [[Attacker]] or [[Defender]] designation from [[Unit|Units]] as needed if there is a [[Combat]] in progress.
	1) If there are Units present at the [[Battlefield]] the Combat is taking place at, but do not have a designation, they gain the same designation as their [[Control|Controller]] now.
	2) If there are Units present at the [[Battlefield]] the Combat is taking place at, but have the opposite designation of their controller, they lose that designation, and gain the same designation as their [[Control|Controller]] now.
	3) If there are Units at locations other than the [[Battlefield]] that the Combat is taking place at, but have either Attacker or Defender designations, they lose those designations now.
3) Handle outstanding board state:
	1) All Units that have [[Lethal Damage]] marked on them and that have [[Deathknell]] or other abilities that trigger on their own death will trigger such abilities now, making note of their current location, attributes, and other information relevant to add the trigger as a [[Pending Chain Item]].
	2) All Units that have [[Lethal Damage]] marked on them are killed and placed in their owners' [[Trash]].
4) Players lose control of any controlled [[Battlefield|Battlefields]] without their Units occupying them if the turn is in an [[Open State]] and there is no [[Showdown]] or [[Combat]] ongoing there.
5) Recall all [[Attached|Unattached]] non-Unit [[Gear]] and non-Unit [[Rune|Runes]] at [[Battlefield|Battlefields]], and all [[Permanent|Permanents]] and Runes in [[Base|Bases]] other than their controller’s. Remove all [[Hidden]] cards from all Battlefields that are not controlled by the same player and place them in their owner's [[Trash]].
6) Mark a [[Showdown]] as **Staged** at each [[Battlefield]] that [[Contested Control|Contested]] was applied to. The Showdown remains Staged at that Battlefield as long as it is Contested and has units present controlled by the player that applied Contested.
7) Mark a [[Combat]] as **Staged** at each [[Battlefield]] that [[Contested]] was applied to that have Units present controlled by opposing players. The Combat remains Staged at that Battlefield as long as there are Units present from two opposing players there. If Units of two opposing players are no longer present at a Battlefield that has a Combat Staged before it has opened, the Combat will cease being Staged.
8) Remove [[Contested Control|Contested]] status from each Battlefield without Units controlled by the player who applied Contested to that Battlefield and without a [[Showdown]] or [[Combat]] ongoing there. If as a result of the removal of [[Contested Control|Contested]] status there are Units located at an uncontested Battlefield that their controller does not control, their controller applies [[Contested Control|Contested]] status to that Battlefield.
9) If the current state is a [[Neutral State|Neutral]] [[Open State|Open]] State and one or more [[Showdown|Showdowns]] are Staged at [[Battlefield|Battlefields]] without a [[Combat]] staged, the [[Turn Player ]]chooses one of those Battlefields. A [[Showdown]] begins there.
10) If the current state is a [[Neutral State|Neutral]] [[Open State|Open]] State and one or more [[Combat]] are Staged at [[Battlefield|Battlefields]], the [[Turn Player]] chooses one of those [[Battlefield|Battlefields]]. [[Combat]] begins there.
11) If the current state is [[Showdown State|Showdown]] [[Open State|Open]] State and [[Combat]] is Staged at a [[Battlefield]] where there is a [[Non-Combat Showdown]] ongoing, that [[Showdown]] becomes a [[Combat Showdown]].
# Special Cleanups
When a Special Cleanup is invoked, the unique steps added will be inserted and defined by the sub-section that invokes it.
See:
- [[Steps of Combat]]
- [[Expiration Step]] of the [[Ending Phase]]

If events during a Special Cleanup require another Cleanup, a normal Cleanup is invoked, not another iteration of the Special Cleanup.