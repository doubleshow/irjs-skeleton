# irjs-skeleton

It does nothing yet. Stay tunned!


# CLI

## Installation

	$ npm install irjs-skeleton -g
	
## Examples


### Find

	$ iosm find 10000 32012 32341 123412
	
	some line of result
	some line of result
	some line of result 

### Insert
	
	$ iosm insert file.json
	
	
file.json

```javascript
{
	a: '1',
	b: '2'
}
```

### Update

	$ iosm update 121212 file.json

```javascript
{
	a: '3'
}	
```

explains what will happen	

### Replace

	$ iosm replace 121212 file.json

```javascript
{
	a: '3'
}	
```

explains what will happen
	
### Delete

	$ iosm remove 1023912
	
	
# API

```javascript
var ir = require('irjs-osm')


var boundingBox = {upperLeft: 1021231, lowerLeft: 93012312} ... 

ir.find(boundingBox)
// => [record]
	
ir.find(boundingBox, { limit: 5})

ir.insert(boundingBox)

ir.update(boundingBox)

ir.delete(id)

```

# Initial Prototype

* 500 records
* A database you are most familair with
	* learn how to use the right js wrapper or api to interact with your choice of database
* published to NPM as 0.0.x
* at least one external person has tested it 


# Test

	$ mocha
	
