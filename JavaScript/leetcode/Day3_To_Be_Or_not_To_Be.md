```
var expect = function(val) {
    return {
        toBe: function(otherVal) {
            if (val === otherVal) {
                return true;
            } else {
                throw new Error("Not Equal");
            }
        },
        notToBe: function(otherVal) {
            if (val !== otherVal) {
                return true;
            } else {
                throw new Error("Equal");
            }
        }
    };
};
``


```
const expect = (val) => {
    return {
        toBe(v) {
            if (val === v) return true;
            throw new Error("Not Equal");
        },
        notToBe(v) {
            if (val !== v) return true;
            throw new Error("Equal");
        }
    };
};
```