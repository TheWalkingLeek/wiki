Bei ActiveRecord queries kann die .to_sql Methode genutzt werden um den genauen Query zu erhalten.


```
Person.all.to_sql
--> SELECT * FROM people LIMIT... 
```
