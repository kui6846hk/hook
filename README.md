# hook

```javascript
const hook = (state) => {
    let st = state
    const setState = (x) =>{
      st = x
      return st
    }
  return [st, setState]
}
[apple, setApple] = hook(10)
const eat = (qty) => {
  apple = setApple(apple - qty)
} 
eat(5)
console.info(apple)
```
