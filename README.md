# mysql_persistent
MySql persistent connection

#Use it as below
```
db.connection.query("SELECT * FROM `table` WHERE `id` = ? ", row_id)
          .on('result', function (row) {
            setData(row);
          })
          .on('error', function (err) {
            callback({error: true, err: err});
          });
```
