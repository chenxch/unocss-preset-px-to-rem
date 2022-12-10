# unocss-preset-pxtorem

Coverts px to rem for utils.

Support simultaneous use with `vant`.

## Installation

```bash
npm i -D unocss-preset-pxtorem
```

```ts
import presetPxToRem from 'unocss-preset-pxtorem'

Unocss({
  presets: [
    presetPxToRem()
  ],
})
```

## Config
```ts
presetPxToRem(options: PxToRemOptions = {})

interface PxToRemOptions {
  /**
   * 75px = 1 rem
   * @default 75
   */
  rootValue?: number
  /**
   * precision
   * @default 5
   */
   unitPrecision?: number
}

```

## Usage

```html
<div class="m-75px" w-35px></div>
```

<table><tr><td width="500px" valign="top">

### without

```css
.m-75px {
  margin: 75px;
}

.w-35px{
  width: 35px;
}
```

</td><td width="500px" valign="top">

### with

```css
.m-75px {
  margin: 1rem;
}

.w-35px{
  width: 0.46667rem;
}
```

</td></tr></table>

## License

MIT License &copy; 2022-PRESENT [Xc](https://github.com/chenxch)
