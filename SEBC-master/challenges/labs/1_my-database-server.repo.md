
MariaDB [(none)]> SELECT @@hostname hostname;
+---------------------------------------------+
| hostname                                    |
+---------------------------------------------+
| ip-172-31-47-175.eu-west-1.compute.internal |
+---------------------------------------------+
1 row in set (0.00 sec)

 SHOW VARIABLES LIKE "%version%";
+-------------------------+---------------------+
| Variable_name           | Value               |
+-------------------------+---------------------+
| innodb_version          | 5.5.49-MariaDB-38.0 |
| protocol_version        | 10                  |
| slave_type_conversions  |                     |
| version                 | 5.5.52-MariaDB      |
| version_comment         | MariaDB Server      |
| version_compile_machine | x86_64              |
| version_compile_os      | Linux               |
+-------------------------+---------------------+
7 rows in set (0.00 sec)


ariaDB [(none)]> CREATE DATABASE scm;
Query OK, 1 row affected (0.00 sec)

MariaDB [(none)]> CREATE DATABASE rman;
Query OK, 1 row affected (0.00 sec)

MariaDB [(none)]> CREATE DATABASE hive;
Query OK, 1 row affected (0.00 sec)

MariaDB [(none)]> CREATE DATABASE oozie;
Query OK, 1 row affected (0.00 sec)

MariaDB [(none)]> CREATE DATABASE hue;
Query OK, 1 row affected (0.00 sec)

MariaDB [(none)]> CREATE DATABASE sentry;
Query OK, 1 row affected (0.00 sec)

MariaDB [(none)]> SHOW DATABASES;
+--------------------+
| Database           |
+--------------------+
| information_schema |
| hive               |
| hue                |
| mysql              |
| oozie              |
| performance_schema |
| rman               |
| scm                |
| sentry             |
+--------------------+
9 rows in set (0.00 sec)


