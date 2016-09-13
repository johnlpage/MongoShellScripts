# MongoShellScripts
My collection of MongoDB snippets

List All Databases (equal to show dbs)

```javascript
var dbs = db.adminCommand({listDatabases:1})['databases']
for (db=0;db<dbs.length;db++) {
	printjson(dbs[db]['name'])
}
```
