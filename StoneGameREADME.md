1)

player1[0] = Math.max(nums[first],nums[last])
  if(nums[first] == nums[last]) then player1[0] = nums[first]  
    first++
    turn = stoneGame(nums, first, last, player)
    
player2[0] = Math.max(nums[first],nums[last])
  if(nums[first] == nums[last]) then player2[0] = nums[first]
    first++
    turn = stoneGame(nums, first, last, player)
    
Since there are two players, there are two array to keep track of what the total amount they have after the pick a pile then the position is increased or decreased depending on which one was choosen. The array nums is considered what what've been the dp array since the positions move and the array is not changed. The reason there's a check for the equal number, depsite the fact that Math.max will still produce the same number, the condition is needed so that a position is changed after that pile is chosen. 
      
