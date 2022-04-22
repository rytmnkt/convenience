## JSONのオブジェクトを要素名でソートする.
```js
(s=>JSON.stringify(Object.fromEntries(Object.entries(JSON.parse(s)).sort())))( `input` );
```
