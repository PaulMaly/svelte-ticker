# Svelte Ticker for Svelte 3 [demo](https://svelte.dev/repl/89ebabbb47c64fe591c01010de096f93?version=3.16.4)

[![NPM version](https://img.shields.io/npm/v/svelte-ticker.svg?style=flat)](https://www.npmjs.com/package/svelte-ticker) [![NPM downloads](https://img.shields.io/npm/dm/svelte-ticker.svg?style=flat)](https://www.npmjs.com/package/svelte-ticker)

Simple Svelte component which automatically makes its contents scrollable ticker-style if it's necessary. Looks like html `<marquee>` tag but much better. Can be useful for such things like News Tickers etc.

## Features

- 4 directions
- duration & delay
- responsive
- infinity or exact looping
- pausing on hover

## Install

```bash
npm i svelte-ticker --save-dev
```

```bash
yarn add svelte-ticker
```

CDN: [UNPKG](https://unpkg.com/svelte-ticker/) | [jsDelivr](https://cdn.jsdelivr.net/npm/svelte-ticker/) (available as `window.Ticker`)

## Usage

```svelte
<Ticker>
    <strong>Your very long string here or even html elements</strong>
</Ticker>

<script>
    import Ticker from 'svelte-ticker';
</script>
```

If you are **not** using using es6, instead of importing add 

```html
<script src="/path/to/svelte-ticker/index.js"></script>
```

just before closing body tag.

## API

## Props

| Name | Type | Description | Required | Default |
| --- | --- | --- | --- | --- |
| `direction` | `String` | Possible values: 'left', 'right', 'top', 'bottom' | No | `left` |
| `duration` | `Number` | Animation duration in seconds | No | `30` |
| `delay` | `Number` | Delay before animation goes in seconds | No | `0` |
| `loop` | `Boolean|Number` | Determines should the animation be looped or played number the times. | No | `true` |
| `pausing` | `Boolean` | Determines should the animation be paused on hover | No | `true` |
| `alternate` | `Boolean` | Determines should the animation be played forwards first, then backwards | No | `false` |
| `behavior` | `String` |Possible values: 'auto' and 'always' | No | `auto` |

## License

MIT &copy; [PaulMaly](https://github.com/PaulMaly)
