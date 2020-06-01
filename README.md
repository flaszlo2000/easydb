# easydb
This is a small tool to make my life easier when I have to work with sqlite databases.
<hr>
It requires 3 essential key in the json:
<ul>
  <li>
    src: the path of the db file, here the sqlite is ensures that the file is going to be created, only the path must be correct
  </li>
  <li>
    tables: this is an object what includes all of the information about the tables (like what and how to make them).<br>
    For instance:
  </li>
</ul>

```yaml
{
   "tables": {
                "test": "id:INTEGER NOT NULL PRIMARY KEY AUTOINCREMENT UNIQUE;value:TEXT"
             }
}
```

<ul>
  <li>
  requires_fill: this should include those datas what are required to pre fill. For example if you want to make a small database with a small "links" table (like in an IoT project) what includes all of the needed links (server addresses, where to send the datas links and so on) what are constant, then this is a great option to set all of those datas.
  </li>
</ul>

<b>Note: </b> this creates the databases with every special option but only checks for the exist of them, this means the program wont check the settings! (at the current version)
