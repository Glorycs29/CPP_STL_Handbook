<p>Let's simulate the game process until the number of health points of each monster becomes k
 or less. Then we can consider that the i
-th monster has aimodk
 health instead of ai
 (except for the case when ai
 is divisible by k
, then the remaining health is k
, not 0
).
</p>
<p>
Now, the health points of all monsters are from 1
 to k
, so each time we damage a monster, we kill it. Therefore, monsters with k
 health points will die first, then the ones with k−1
 health points, and so on. So, let's sort the monsters by their remaining health points in descending order
 (don't forget that, if two monsters have the same health, then they should be compared by index).
 And the order you get after sorting is the answer to the problem.
</p>
