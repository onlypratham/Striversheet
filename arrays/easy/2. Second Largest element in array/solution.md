```
class Solution {
    public int secondLargestElement(int[] nums) {
    int large = Integer.MIN_VALUE, second_large = Integer.MIN_VALUE;

    for(int i= 0; i<nums.length; i++){
        if(nums[i]>large){
            second_large = large;
            large = nums[i];
        }
        else if(nums[i]> second_large && nums[i] != large){
        second_large = nums[i];
        }
        }
    
    return (second_large == Integer.MIN_VALUE) ? -1:second_large;
    }
}
```

<img width="1920" height="1140" alt="image" src="https://github.com/user-attachments/assets/6822a0b9-2043-4da9-975c-50da78594937" />


