# question-no-135
Solution to the question no 135 on leet code 

135. Candy
There are n children standing in a line. Each child is assigned a rating value given in the integer array ratings.

You are giving candies to these children subjected to the following requirements:

Each child must have at least one candy.
Children with a higher rating get more candies than their neighbors.
Return the minimum number of candies you need to have to distribute the candies to the children.

Initialize:

candies[] starts with 1 for every child (each must get at least one candy).

Left to Right Pass:

If a child has a higher rating than the one before, give them one more candy than the previous child.

Right to Left Pass:

If a child has a higher rating than the one after, make sure they have more candies than the next (take the max to not undo left pass).

Sum All Candies:

Add up all values in candies[] to get the minimum required.
