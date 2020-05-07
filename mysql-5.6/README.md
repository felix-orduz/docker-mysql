# Example MySQL 5.6

In the file: **config-felix.orduz.cnf** there are configurations for mysql 


### Up services
```bash
docker-compose up -d
```

### Change root password

```bash
docker-compose exec db mysql -u root -p'change-me'  -e "SET PASSWORD FOR 'root'@'localhost' = PASSWORD('new-password'); flush privileges;"
```