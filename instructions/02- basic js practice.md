# Basic Javascript practise for React

1. Module intro.
2. let & const.  
You won't see var in React, so most of cases we use `const`, sometimes `let`


3. Arrow Functions.
4. Exports and imports (Modules).

```js
const personCard = {
	name:'Allen'
}
export default personCard
```

The way we import `personCard` in `app.js`

```js
import personCard from './person.js'
import personCards from './person.js'

```

It is different when importing from `utility.js`

```js
export const goShopping = () => { ... }
export const baseData = 20;
```

The way we import `personCard` in `app.js`

```js
import { baseData } from './utility.js'
import { goShopping } from './utility.js'

```
 
 
 
 
```js


```