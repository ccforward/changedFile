ChangedFile
==============

get directory change files list

## Usage

```js
var cf = require('cf');

var changed = cf.get('./',function(item){
	if(item.match(/^node_modules|^\./)) return false;
	return true;
});

console.log(changed); // [];
```

## License
MIT license
