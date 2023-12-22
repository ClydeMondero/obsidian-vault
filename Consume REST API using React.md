[[REST]] [[React]]

# Consume REST API using React
#resource 

```js
import React, { useState, useEffect } from 'react';

const App = () => {
   const [posts, setPosts] = useState([]);
   useEffect(() => {
      fetch('https://jsonplaceholder.typicode.com/posts?_limit=10')
         .then((response) => response.json())
         .then((data) => {
            console.log(data);
            setPosts(data);
         })
         .catch((err) => {
            console.log(err.message);
         });
   }, []);

return (
   // ... consume here
);
};
```

[Reference](https://www.freecodecamp.org/news/how-to-consume-rest-apis-in-react/) 