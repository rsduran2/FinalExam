dp[0] = nums[i][j]
dp[i] += Math.min(nums[i-1][j-1],nums[i-1][j],nums[i-1][j+1]
  
  
Using an array, dp, to keep track of the cost to reach an element in the last row. dp[0] is set this way because we will be starting at the beginning row and beginning column, in this case, at position 1 for both since we will be using row-1 and col-1 to balance this out. We want to check at which col at the current row position holds the smallest number. This is using two for loops that will be set at i = 1 and j = 1 since setting them at zero would return errors and this makes sure each col and/ row is properly visited. We also do check all possiblities so that no col that could have a smaller number is skipped. Once a number in the col is chosen, then we move onto the next row until we reach the last one and there we just check the smallest number. 
