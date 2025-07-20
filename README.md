# Verify SST Auth
Verify that Mariadb Galera cluster node is correctly configured for Mariabackup SST.

Script by Edward Stoever for Mariadb Support.

This script is self-explanatory. 

Output from this script looks like this:
```
root@m1:~/verify_sst_auth$ ./verify_mariabackup_SST.sh
--wsrep_sst_method=mariabackup --wsrep_sst_auth=mariabackup:password
mariabackup:password
+--------------------+
| PRIVILEGES_GRANTED |
+--------------------+
| RELOAD             |
| LOCK TABLES        |
| BINLOG MONITOR     |
+--------------------+
+-------------------------------------------------------------------------------------------------+
| NOTE                                                                                            |
+-------------------------------------------------------------------------------------------------+
| 'mariabackup'@'localhost' needs 4 privileges: RELOAD, PROCESS, LOCK TABLES, and BINLOG MONITOR. |
+-------------------------------------------------------------------------------------------------+
root@m1:~/verify_sst_auth$
``