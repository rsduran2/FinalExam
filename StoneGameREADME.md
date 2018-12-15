1)

dpA[0] = Math.max(nums[first],nums[last])
 
dpL[0] = Math.max(nums[first],nums[last])

dpA[i] = Math.max(nums[first],nums[last])+ dpA[i-1]
dpL[j] = Math.max(nums[first],nums[last])+ dpL[j-1]
 
  

    
Since there are two players, there are two array to keep track of what the total amount they have after the pick a pile then the position is increased or decreased depending on which one was choosen. The array nums is considered what what've been the dp array since the positions move and the array is not changed. There will be a for loop for i and j which will represent each of the turns for each player and this will update the nums array to move the first or last position depending on which one was chosen by the player,choose a max number and add them together. Then once each player has gone and the array is empy, there will be a check for the last element in each player's array to see which is the bigger number and return a true so long as Alex had the largest amount.
      
