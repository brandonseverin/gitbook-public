# Set

* [MDN](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Set)

## Notes:

* Use `Set.add` vs `Map.set`
* Use `Set.size` vs `Array.length`
* To remove/delete: use `delete`

## Set Cloning

```javascript
const new = new Set(old);
```

Or if enabled:

```javascript
const new = ...old
```

## Set Iteration

```javascript
for (let value of set.values()) {
  ...
}
```

## To Array

```javascript
Array.from(new Set())
```

## Differences

[https://github.com/aizatto/nodejs/blob/master/src/fn.js\#L42](https://github.com/aizatto/nodejs/blob/master/src/fn.js#L42)

```javascript
function setMath<T>(a: Set<T>, b: Set<T>) {
  return {
    remove: [...a].filter(x => !b.has(x)),
    add: [...b].filter(x => !a.has(x)),
  };
}
```

## 

