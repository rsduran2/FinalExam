dp[0] = 0
dp[i] = Math.min(dp[i], dp[sub] +1);
sub = i-j*j

Using an array called dp to keep track of how many squared numbers were used to be subtracted from the target number. dp[0] = 0 doesn't need to necessarily be initalized to 0 but it helps to get rid of possible errors. The recursive call looks at dp[i] and dp[sub] to compare the two for the minimum amounts. The one is there to add to the number of times it can be used at that position.
