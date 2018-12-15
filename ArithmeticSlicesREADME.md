dp[0] = 0
dp[1] = 0
dp[i] =
  if(n[i]-n[i-1] == n[i-1]-[n-2]
  dp[i] = 1+dp[i-1]
  
Using an array dp to keep track of the count of slices. dp[0] = 0 because it's less than three numbers. dp[1] = 0 doesn't really need to be intialized in this sense because it'll already be zero and possibly change where are dp[0] shouldn't. From there, we go through the original array of n and compare the first two numbers, subtracted, then the next two, also subtracted and if they share the same differnce then we add one to the dp array. When we have finished going through the array then we just need to return the last position in dp to get the total number of slices. This accounts for multiple instances of slices, assuming that this is allowed.
