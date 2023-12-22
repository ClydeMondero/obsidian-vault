[[PHP]]
# Count the numbers of results of a query in PHP
#resource 

```php
$query = "SELECT * FROM my_table WHERE column_name = 'some value'";

$result = mysqli_query($link, $query); $num_rows = mysqli_num_rows($result);
```

[Reference](https://www.w3docs.com/snippets/php/how-can-i-count-the-numbers-of-rows-that-a-mysql-query-returned.html#:~:text=MySQL%20query%20returned%3F-,How%20can%20I%20count%20the%20numbers%20of%20rows%20that%20a,MySQL%20query%20returned%20in%20PHP.&text=This%20code%20connects%20to%20a,rows%20returned%20by%20the%20query.) 