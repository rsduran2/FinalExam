dp[0] = 0
dp[i] = Math.min(dp[i], dp[sub] +1);
sub = i-j*j

Using an array called dp to keep track of how many squared numbers were used to be subtracted from the target number. dp[0] = 0 doesn't need to necessarily be initalized to 0 because it could be considered a perfect square itself but because it doesn't affect the number we don't add the 1. From there we compute the squared values and store them in an int variable to keep track of the square numbers up to the target number. Then we check for the smallest squared value that can be subtracted from the target number by comparing between the pervious value of dp[i] or the new value of dp[sub]+1. The +1 is so we can count the squared number itself.
