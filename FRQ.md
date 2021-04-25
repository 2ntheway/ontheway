## node js中的模块引入问题

```js
var x = 5;
var addX = function (value) {
 return value + x;
};
//对外输出
module.exports.x = x;
module.exports.addX = addX;
//引入模块
var example = require('./example.js');
console.log(example.x); // 5
console.log(example.addX(1)); // 6
```

