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
