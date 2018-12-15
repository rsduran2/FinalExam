1)

dp[0] = 0
dp[i] = Math.max(dp[i],dp[j]+1)

We are using an array dp to keep track of the longest chain in the 2D array pairs. dp[0] doesn't necessarily need to be initialized to 0 but it's good to have in case of an error and would return 0 for no chain. There would be two for loops for i and j that would be used to compare each of the pairs with the positions of b and c being 1 and 0 respectively. This is to ensure that only b and c get compared to determine a link as stated. After the loops go through all of the possible pairs, there will be an additional for loop to go through the finished dp to find the max number. This is because there's no guarentee that the max number will be at the end since there can be multiple chains found in the array of varying sizes.
