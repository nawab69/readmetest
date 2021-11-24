<h1 align="center">
  <br>
  <br>
  <img src="https://i.ibb.co/6bqvcHH/logo.png" alt="multicone" width="500">
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

```js

import React from 'react'
import { Button } from '@multicone/components'

const App = () => {
  return (
    <div>
      <Button>...</Button>
    </div>
  )
}
export default App

```

| Parameters      | Types | Defaults     |
| :---:       |    :----:   |          :---: |
| className      | `string`       |  |
| onClick*   | `Function`        | ()=>{}      |
| variant   | `"default"` `"primary"` `"info"` `"success"` `"warning"` `"danger"` `"dark"`| `"default"`|
|size| `"xs"` `"sm"` `"base"` `"lg"` `"xl"` ... `"9xl"`| `"md"`|
|disabled|`boolean`|`false`|
|rounded|`"sm"` `"md"` `"lg"` `"full"`|`"md"`|
|outline|`boolean`|`false`|
| children*      | `string` `jsx` |  | 


## Checkbox

```js

import React, { useState } from 'react'
import { Checkbox } from '@multicone/components'

const App = () => {
const [checked,setChecked] = useState(false)
  return (
    <div>
      <Checkbox selected={checked} onCheck={setChecked}>...</Checkbox>
    </div>
  )
}
export default App

```
| Parameters      | Types | Defaults     |
| :---:           |    :----:   |  :---: |
| selected* | `boolean` | `false`    |
| onCheck*     | `Function` |    |
| iconSize      | `number` | `32`     |
| iconColor      | `"black"` `"white"` `"green"` `"red"` `"yellow"` `"blue"` `"purple"` `"indigo"` | `"black"`     |
| className      | `string`       |  |
| children*      | `string` `jsx` |  |   


## Radio
```js

import React, { useState } from 'react'
import { Radio } from '@multicone/components'

const App = () => {
const [selected,setSelected] = useState()

const items = [
   { name:'Dhaka', value:'d' },
   { name:'Sylhet', value:'s' } ]
   
  return (
    <div>
      <Radio items={items}/>
    </div>
  )
}
export default App
```
| Parameters      | Types       | Defaults     |
| :---:           |    :----:   |  :---: |
| items*          | `item[]`    |    |
| className       | `string`    |  |
| onCheck*       | `Function`  |    |
| textStyle      | `string`    |  |
| iconSize       | `number`    | `5`     |
| iconColor      | `"black"` `"white"` `"green"` `"red"` `"yellow"` `"blue"` `"purple"` `"indigo"` | `"black"`     |
| checkIcon       | `boolean`       | `true' |



## Select

```js

import React, { useState } from 'react'
import { Select } from '@multicone/components'

const App = () => {
const [selected,setSelected] = useState()

const items = [
   { name:'Dhaka', value:'d' },
   { name:'Sylhet', value:'s' } ]
   
  return (
    <div>
      <Select items={items} onSelect={setSelected}/>
    </div>
  )
}
export default App
```

| Parameters      | Types       | Defaults     |
| :---:           |    :----:   |  :---: |
| items*          | `item[]`    |    |
| onSelect*       | `Function`  |    |
| placeholder     | `string`    | |
| className       | `string`    |  |
| modalStyle      | `string`    |  |
| arrowSize       | `number`    | `32`     |
| arrowColor      | `"black"` `"white"` `"green"` `"red"` `"yellow"` `"blue"` `"purple"` `"indigo"` | `"black"`     |
| isCenter       | `boolean`       | `false' |



## License

[MIT]()


