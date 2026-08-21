**Combat Result** is a [[Task]] which defines the events happening as a result of the [[Combat]]. It is performed during the [[Resolution Step]] of the [[Steps of Combat]], after the [[Combat Cleanup]].

A Player has **won** a [[Combat]] if they received either the [[Attacker]] or [[Defender]] designation and are the only Player that has [[Unit|Units]] remaining at this [[Battlefield]] during this step.

A Player has **lost** a [[Combat]] if they received either the [[Attacker]]] or [[Defender]] designation and are the only Player that does not have any [[Unit|Units]] remaining at this [[Battlefield]] during this step.

[[Unit|Units]] at this [[Battlefield]] inherit the same **combat result** as their controllers.

There is **“No Result”** if [[Unit|Units]] were [[Recall|Recalled]] during step 3d of the [[Combat Cleanup]], if both Players have units present during this [[Task]], or if neither player has units present during this [[Task]]. If “No Result” was reached, and both players have units remaining, stage a [[Showdown]] and a [[Combat]] at this [[Battlefield]].