# P(romise) Timeout

> Timeout a promise after a specified amount of time

## Usage

```js
import pTimeout from 'https://deno.land/x/p_timeout@1.0.0/mod.ts

const delayedPromise = new Promise(resolve => setTimeout(resolve, 500))

pTimeout(delayedPromise, 50).then(() => 'foo')
//=> [TimeoutError: Promise timed out after 50 milliseconds]
```

## API

See https://doc.deno.land/https/deno.land/x/p_timeout@1.0.0/mod.ts

## License/Credits
- P(romise) Timeout is licensed under the MIT license. 
- Code is adapted from [Sindre's p-timeout for node](https://github.com/sindresorhus/p-timeout) (also under the MIT license)