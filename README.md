# JSCloneObject
JavaScript clone object 
<br> Reference: https://medium.com/@dtinth/immutable-js-persistent-data-structures-and-structural-sharing-6d163fbd73d2

```JS
const obj = {name: 'Andrei'}
function clone(obj) {
  return {...obj}; // this is pure
}

function updateName(obj) {
  const obj2 = clone
  (obj);
  obj2.name = 'Nana'
  return obj2
}
```

```JS
const updatedObj = updateName(obj)
console.log(obj, updatedObj)
```

HIGHER ORDER FUNCTION / CLOSURE JS 

```JS
//HOF
const hof = (fn) => fn(5);
hof(function a(x){ return x})
//Closure
const closure = function() {
  let count = 55;
  return function getCounter() {
    return count;
  }
}
```

```JS
const getCounter = closure()
getCounter()
getCounter()
getCounter()
```
