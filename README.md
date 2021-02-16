<div align="center">
    <img src="assets/logo.svg" width="350" height="350" alt="People standing in Timeout illustration">
    <h1>Promise Timeout</h1>
    <p>
        <b>Timeout a promise after a specified amount of time. Deno port of <a href="https://github.com/sindresorhus/p-timeout">sindresorhus's p-timeout for node</a></b>
    </p>
    <p>
        <img alt="build status" src="https://img.shields.io/github/workflow/status/KhushrajRathod/pTimeout/Deno?label=checks" >
        <img alt="language" src="https://img.shields.io/github/languages/top/KhushrajRathod/pTimeout" >
        <img alt="code size" src="https://img.shields.io/github/languages/code-size/KhushrajRathod/pTimeout">
        <img alt="issues" src="https://img.shields.io/github/issues/KhushrajRathod/pTimeout" >
        <img alt="license" src="https://img.shields.io/github/license/KhushrajRathod/pTimeout">
        <img alt="version" src="https://img.shields.io/github/v/release/KhushrajRathod/pTimeout">
    </p>
    <p>
        <b><a href="https://deno.land/x/p_timeout">View on deno.land</a></b>
    </p>
    <br>
    <br>
    <br>
</div>

## Usage

```js
import pTimeout from "https://deno.land/x/p_timeout@1.0.1/mod.ts"

const delayedPromise = new Promise(resolve => setTimeout(resolve, 500))

await pTimeout({
    promise: delayedPromise,
    milliseconds: 50,
})

// => [TimeoutError: Promise timed out after 50 milliseconds]
```

## API

See https://doc.deno.land/https/deno.land/x/p_timeout@1.0.1/mod.ts

## Supporters

- HUGE thanks to @sindresorhus -- this repository is mostly his code, modified to work with Deno

[![Stargazers repo roster for @KhushrajRathod/pTimeout](https://reporoster.com/stars/KhushrajRathod/pTimeout)](https://github.com/KhushrajRathod/pTimeout/stargazers)

[![Forkers repo roster for @KhushrajRathod/pTimeout](https://reporoster.com/forks/KhushrajRathod/pTimeout)](https://github.com/KhushrajRathod/pTimeout/network/members)

## Related

- [pQueue](https://github.com/KhushrajRathod/pQueue)
- [pRetried](https://github.com/KhushrajRathod/pRetried)
- [retried](https://github.com/KhushrajRathod/retried)
- [...more](https://github.com/KhushrajRathod/denoModules)

## License

- Promise Timeout is licensed under the MIT license.
- Code is adapted from [Sindre's p-timeout for node](https://github.com/sindresorhus/p-timeout) (also under the MIT license)
