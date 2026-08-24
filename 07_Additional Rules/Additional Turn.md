---
aliases:
  - Additional Turns
---
Certain [[Game Effect|Game Effects]] will instruct a player to **“take a turn after this.”** These effects create a temporary **Additional Turn** owned by that player that is inserted into the turn queue after the current turn.

[[Turn Order]] is established when the game begins as a repeating set of players. This populates a looping queue of turns that each player will take, starting with the first turn taken by the First Player, and repeating indefinitely.

When an **Additional Turn** is inserted into this queue, **it does not change** the [[Turn Order]] of the game. The owner of the **Additional Turn** just has the next queued turn. After that turn is completed, it will be removed and the queue will proceed with its previously queued turns.

If multiple **Additional Turns** are queued, they are added to the queue in the order the [[Game Effect|Game Effects]] that generated them occurred.

>*Example*: The First Player plays, through some means, two Time Warps during their turn. The Time Warps create two Additional Turns for their controller and insert them into the turn queue after the current turn. If the turn queue is represented as [> A > B > C > D >], then these Additional Turns will appear as [> A > A* > A* > B > C > D >]. After the last Additional Turn is played, the queue returns to its previously queued turns.
>*Example*: The First Player plays Promising Future during their turn, during the resolution of which the Second and Fourth Player choose, banish, and play one Time Warp each. The Fourth Player’s Time Warp resolves first, inserting an Additional Turn for them in the queue as such: [> A > D* > B > C > D >]. The Second Player’s Time Warp resolves afterwards, inserting that turn: [> A > B* > D* > B > C > D >]. When the First Player passes the turn, the Second Player will take their turn, followed by the Fourth Player, after which the queue returns to its previously queued turns.