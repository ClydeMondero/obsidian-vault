[[React]]

# Import multiple pages from a single file in React
#resource 

```
/components
   -index.js
   -login.js
   -questions.js
```

```javascript
import Login from './login'
import Question from './question'

export {Login, Question}
```


```javascript
import {Login, Question} from './components'
```
[Reference](https://stackoverflow.com/a/70807923)