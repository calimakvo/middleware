# middleware
Yesod Middleware sample code

## database initialize

### database create

```
$ mysqladmin -u root create mid
```

### grant

```
mysql> GRANT ALL PRIVILEGES ON mid.* TO 'mid'@'localhost' IDENTIFIED BY 'mid';
mysql> FLUSH PRIVILEGES;
```

### migration

```
$ stack exec -- yesod devel
```

### insert

```
mysql> INSERT INTO system_info(id, init) VALUES(1, 1);
```
