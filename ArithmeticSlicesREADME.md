dp[0] = 0
dp[1] = 0
dp[i] =
  if(n[i]-n[i-1] == n[i-1]-[n-2]
  dp[i] = 1+dp[i-1]
  
Using an array dp to keep track of the count of slices. dp[0] = 0 because it's less than three numbers. dp[1] = 0 doesn't really need to be intialized in this sense because it'll already be zero and possibly change where are dp[0] shouldn't. From there, it's recursively going through the array counting each of the slices.
