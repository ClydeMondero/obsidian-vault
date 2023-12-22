[[MongoDB]]

# Queries in MongoDB
#resource 

## Querying a collection
```mongodb
db.movies.find()
db.movies.find( { "title": "Titanic" } )
```

Equivalent to the SQL Statements:
```sql
SELECT * FROM movies
SELECT * FROM movies WHERE title = "Titanic"
```

[Reference](https://www.mongodb.com/docs/mongodb-shell/crud/)