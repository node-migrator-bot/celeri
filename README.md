CLI utility for [garden](https://github.com/spiceapps/garden)


### Usage:

```javascript

	var celery = require('celery');


	celery.on('hello :name', function(data)
	{
		console.log('Hello ' + data.name +'!');
	});

	celery.open();

	celery.parse(process.argv);
```

terminal:

	node ./cli-app hello:craig ↩
	hello craig!
or:

	node ./cli-app

	hello craig ↩
	hello craig!


