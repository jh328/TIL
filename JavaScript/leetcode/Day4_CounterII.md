```
const createCounter = (init) => {
    let current = init;

    return {
        increment(){
            return ++ current;
        },

        decrement(){
            return --current;
        },

        reset(){
            current = init;
            return current;
        },
    }
}
```
