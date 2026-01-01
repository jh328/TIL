var createCounter = function(n) {
    return function(){
        return n++;
    }
}

화살표 함수
const createCounter = (n) => () => n++;