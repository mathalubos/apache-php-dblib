# apache-php-dblib
PHP image based on eboraas/apache with added dblib/sybase. Contains supervisord, composer and curl.

This image is meant to be environment for radsectors/sqlshim which enables sqlsrv_* functions for communication with sql server. That is really usefull for developing of php projects ,that use microsoft sqlsrv drivers, on Linux .

Minor changes must be done in conf file /etc/freetds/freetds.conf in order to connect sql server.

```
...
# A typical Microsoft server
[myHost]
host = 0.0.0.0 # change to your hostname or ip
instance = INSTANCE # fill your instance name
tds version = 8.0 # change this according to your sql server version
```
