<h1 align="center">
  <br>
  <br>
  <a href="http://www.amitmerchant.com/electron-markdownify"><img src="https://raw.githubusercontent.com/multicone/portofolio/master/src/images/logo/multicone.png" alt="Markdownify" width="500"></a>
  <br>
  <br>
</h1>

<h4 align="center">A react component's library based on tailwindcss</h4>

<p align="center">
<img alt="npm bundle size (scoped)" src="https://img.shields.io/bundlephobia/min/@multicone/components">
<img alt="NPM" src="https://img.shields.io/npm/l/@multicone/components">
<img src="https://img.shields.io/badge/React-17.0.2-brightgreen">
<img src="https://camo.githubusercontent.com/7e7bdf5c529c8bc594e26038dbb1a3d360e9ede891fbdcef50b403ab5f88fc14/68747470733a2f2f696d672e736869656c64732e696f2f62616467652f636f6e747269627574696f6e732d77656c636f6d652d6f72616e67652e737667">
</p>

# Installation

```
npm i @multicone/components
```
or
```
yarn add @multicone/components
```
# Usage
Here is a quick example to get you started, it's all you need:
```js

import React from 'react'
import { Button } from '@multicone/components'
const App = () => {
  return (
    <div>
      <Button onClick={()=>alert("hello wrold")}>Herllo</Button>
    </div>
  )
}

export default App

```

# Docs
## Button
| Parameters      | Types | Defaults     |
| :---:       |    :----:   |          :---: |
| className      | `string`       | - |
| onClick   | `Function`        | ()=>{}      |
| variant   | `"deafult"` `"primary"` `"info"` `"success"` `"warning"` `"danger"` `"dark"`       | `"success"`     |

## License

[MIT]()


