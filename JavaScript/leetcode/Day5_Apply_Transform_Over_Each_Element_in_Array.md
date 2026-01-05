```
var map = function(arr,fn){
    const resutl = [];

    for(let i = 0; i < arr.length; i++){
        const value = fn(arr[i],i){
            result.push(value);
        }
    }   
    return result;
}
```

```
const map = (arr, fn ) => {
    const result = [];
    for(let i = 0; i <arr.length; i++){
        result.push(fn(arr[i],i));
    }
    return result;
}
```