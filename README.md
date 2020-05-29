# easydb
This is a small tool to make my life easier when I have to work with sqlite databases.
<hr>
It requires 3 essential key in the json:
<ul>
  <li>src: the path of the db file, here the sqlite is ensures that the file is going to be created, only the path must be correct</li>
  <li>
    tables: this is an object what includes all of the information about the tables (like what and how to make them).<br>
    For instance:
  </li>

```yaml
{
   "tables": {
                "test": "id:INTEGER NOT NULL PRIMARY KEY AUTOINCREMENT UNIQUE;value:TEXT"
             }
}
```

  <li></li>
</ul>

