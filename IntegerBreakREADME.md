dp[0] = 1
dp[i] = Math.max(dp[j],dp[j-i]*i]

We are using an array dp to store the max number of the total of breaks from the original array. We have two for loops i and j that will represent what we can choose and the sum of the items we are going choose. This is why we compare current dp of the jth position with dp if (j-i)+i because we can choose i as well. When we go through the entire original array we can then check j in order to get the max number from the dp array which will be at the end. This will be done with a variable int max that in the beginning with be initialized to 0 and later used to compare it with dp[j] for the max number. 
