## MySQLのクエリログを出力するようにする.
```sql
set global general_log = on;
set global general_log_file = '/var/lib/mysql/general_log.log';
show variables like 'general_log%';
```
表示例
```sh
docker exec -it CONTAINER_NAME tail -f /var/lib/mysql/general_log.log
```
