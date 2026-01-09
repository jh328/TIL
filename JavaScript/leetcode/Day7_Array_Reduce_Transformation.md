```
var reduce = function(nums, fn, init) {
    let val = init;
    
    for(let i = 0; i < nums.length; i++){
        val = fn(val, nums[i])
    }

    return val;
};
```

```
const reduce = (nums,fn,init) => {
    let answer = init;

    for(const num of nums){
        answer = fn(answer, num);
    }

    return answer;
}
```