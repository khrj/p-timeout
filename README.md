<div align="center">
    <img src="assets/logo.svg" width="350" height="350" alt="People standing in Timeout illustration">
    <h1>Promise Timeout</h1>
    <p>
        <b>Timeout a promise after a specified amount of time. Deno port of <a href="https://github.com/sindresorhus/p-timeout">sindresorhus's p-timeout for node</a></b>
    </p>
    <p>
        <img alt="build status" src="https://img.shields.io/github/workflow/status/khrj/p-timeout/Deno?label=checks" >
        <img alt="language" src="https://img.shields.io/github/languages/top/khrj/p-timeout" >
        <img alt="code size" src="https://img.shields.io/github/languages/code-size/khrj/p-timeout">
        <img alt="issues" src="https://img.shields.io/github/issues/khrj/p-timeout" >
        <img alt="license" src="https://img.shields.io/github/license/khrj/p-timeout">
        <img alt="version" src="https://img.shields.io/github/v/release/khrj/p-timeout">
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
import pTimeout from "https://deno.land/x/p_timeout@1.0.2/mod.ts"

const delayedPromise = new Promise(resolve => setTimeout(resolve, 500))

await pTimeout({
    promise: delayedPromise,
    milliseconds: 50,
})

// => [TimeoutError: Promise timed out after 50 milliseconds]
```

## API

See https://doc.deno.land/https/deno.land/x/p_timeout@1.0.2/mod.ts

## Supporters

- HUGE thanks to @sindresorhus -- this repository is mostly his code, modified to work with Deno

[![Stargazers repo roster for @khrj/p-timeout](https://reporoster.com/stars/khrj/p-timeout)](https://github.com/khrj/p-timeout/stargazers)

[![Forkers repo roster for @khrj/p-timeout](https://reporoster.com/forks/khrj/p-timeout)](https://github.com/khrj/p-timeout/network/members)

## Related

- [p-queue](https://github.com/khrj/p-queue)
- [p-retried](https://github.com/khrj/p-retried)
- [retried](https://github.com/khrj/retried)
- [...more](https://github.com/khrj/deno-modules)

## License

- Promise Timeout is licensed under the MIT license.
- Code is adapted from [Sindre's p-timeout for node](https://github.com/sindresorhus/p-timeout) (also under the MIT license)
