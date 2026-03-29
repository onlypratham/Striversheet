```
class Solution {
    public boolean check(int[] nums) {
        int count = 0;
        int n = nums.length;

        for(int i= 0;i<n;i++){
            if(nums[i]> nums[(i+1) % n]){
                count++;
            }
        }
        return count<=1;
    }
}
```

<img width="1920" height="1140" alt="image" src="https://github.com/user-attachments/assets/48d65f6a-d7b4-4ddd-bfea-869d7921dbe2" />
