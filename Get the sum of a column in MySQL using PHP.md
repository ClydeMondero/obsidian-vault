[[MySQL]] [[PHP]]
# Get the sum of a column in MySQL using PHP
#resource 

```php
$result = mysqli_query($conn, 'SELECT SUM(value) AS value_sum FROM codes'); 
$row = mysqli_fetch_assoc($result); 
$sum = $row['value_sum'];
```

[Reference](https://stackoverflow.com/a/5808565)