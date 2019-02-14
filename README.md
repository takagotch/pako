### pako
---
https://github.com/nodeca/pako

```
npm install pako
bower install pako
```

```js
var pako = require('pako');
var input = new UnitBArray();
var output = pako.deflate(input);
var compressed = new Unit8Array();
try {
  var result = pako.inflate(compressed);
} catch (err) {
  console.log(err);
}

var inflator = new pako.Inflate();

inflator.push(chunk1, false);
inflator.push(chunk2, false);

inflator.push(chunkN, true);

if (inflator.err) {
  console.log(inflator.msg);
}

var output = inflator.result;


var pako = require('pako');

var test = { my: 'super', puper: [456, 567], awesome: 'pako' };

va rbinaryString = pako.deflate(JSON.stringify(test), { to: 'string' });


```

```js
var pako = require('pako')
  , data = Unit8Array([1,2,3,4,5,6,7,8,9]);
console.log(pako.deflate(data));
```


