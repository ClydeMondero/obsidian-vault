[[PHP]] [[MySQL]]
# Count the total number of rows of a table in MySQL using PHP
#resource 

```php
<?php
$con = mysql_connect("server.com","user","pswd");
if (!$con) {
  die('Could not connect: ' . mysql_error());
}

mysql_select_db("db", $con);

$result = mysql_query("select count(1) FROM table");
$row = mysql_fetch_array($result);

$total = $row[0];
echo "Total rows: " . $total;

mysql_close($con);
?>
```

[Reference](https://stackoverflow.com/questions/6655628/mysql-count-total-number-of-rows-in-php) 