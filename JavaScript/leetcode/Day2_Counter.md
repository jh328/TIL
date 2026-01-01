```
var createCounter = function(n) {
    return function(){
        return n++;
    }
}
```

```
화살표 함수
const createCounter = (n) => () => n++;
```

```
클로저란? 외부 함수의 실행이 끝나서 소멸 되었음애도 불구하고, 내부 함수가 외부 함수의 변수를 여전히 기억하고 접근할 수 있는 현상을 말한다.
```