[[React]]

# Change document title in React
#resource 

```javascript
import React, { useEffect } from 'react';

function Example() {
  useEffect(() => {
    document.title = 'My Page Title';
  }, []);
}
```

[Reference](https://stackoverflow.com/a/46176359) 