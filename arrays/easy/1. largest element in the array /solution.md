BRUTE FORCE:
```
class Solution {
    public int largestElement(int[] nums) {
        Arrays.sort(nums);

        return nums[nums.length-1];
    }
}
```
<img width="1920" height="1140" alt="image" src="https://github.com/user-attachments/assets/44dce5e7-55ea-4477-9642-f062e3b85a4e" />





OPTIMISED: 
```
class Solution {
    public int largestElement(int[] nums) {
        int max = 0;
        for(int i=0; i < nums.length; i++){
            if(nums[i]>= max){
                max = nums[i];
            }
        }
        return max;
    }
}
```
<img width="1920" height="1140" alt="image" src="https://github.com/user-attachments/assets/7676db1b-4944-4147-83d5-92c09d821ca2" />

