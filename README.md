#  [![NPM version][npm-image]][npm-url] [![Dependency Status][daviddm-image]][daviddm-url]

> RFC2616 compliant http cache implementation


## Install

```sh
$ npm install --save oniyi-cache
```


## Usage

```js
var oniyiCache = require('oniyi-cache');

oniyiCache({
	storePrivate: false,
	storeNoStore: false,
	ignoreNoLastMod: false,
	requestValidators: [],
	responseValidators: [],
	hostConfig: {
		'www.npmjs.org': {
			storePrivate: true,
			storeNoStore: true
		}	
	}
});

```

## Methods

### hash(requestObject)
creates a hash string from the provided request object

### addHostConfigs(config)

### setHostConfigs(config)

### updateHostConfigs(config)

### clearHostConfigs(config)

### getEvaluator(hostname, config)

## Kudos

The basic concept here has been borrowed from Chris Corbyn's node-http-cache.

## License

MIT © [Benjamin Kroeger]()


[npm-image]: https://badge.fury.io/js/oniyi-cache.svg
[npm-url]: https://npmjs.org/package/oniyi-cache
