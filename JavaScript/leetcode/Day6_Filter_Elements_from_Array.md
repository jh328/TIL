```
var filter = function(arr,fn){
    let answer = [];

    for(let i = 0; i < arr.length; i++){
        if(fn(arr[i],i)){
            answer.push(arr[i])
        }
    }
    return answer;
}
```

```
const filter = (arr, fn) => {
    let answer = [];

    for(let i = 0; i < arr.length; i++){
        if(fn(arr[i],i)){
            answer.push(arr[i])
        }
    }
    return answer;
}
```

```
reduce 
reduce 메서드는 4개의 인수를 가진다.
1. 누적값 (acc) 필수 2. 현재 값 (cur) 필수 3.현재 인덱스 (idx) 선택 4. 원본 배열(src) 선택
초기값으로 배열을 선언을 해야 하는 이유는 map,filter 배열에는 push를 할 때 값을 담아야 하기 때문이다.

const filter =(arr, fn) => {
    return arr.reduce((acc,cur,i) => {
        if(fn(cur,i)){
            acc.push(cur);
        }
        return acc;
    },[]) // 초기값으로 배열 선언
}
```
