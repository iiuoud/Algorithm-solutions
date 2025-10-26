## other

### 9. 回文数

```js
/**
 * @param {number} x
 * @return {boolean}
 */
var isPalindrome = function(x) {
    x=x+'';
    let l=0,r=x.length-1;
    while(l<r){
        if(x[l]===x[r]){
            l++;
            r--;
        }else{
            return false
        }
    }
    return true;
};
```

- 使用x=x+''比x.toString()用时更短，不用查询原型链并执行函数调用

