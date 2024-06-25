# cometa_lab2
Практическое задание #2, стажировка, Cometa IT Bootcamp

Ниже практическое задание №2 по программе стажировки Cometa IT Bootcamp.
Это задание посвящено базам данных. Предполагается, что вы ознакомились с файлом-мануалом, который был отправлен в группу.

Итак, практическое задание №2:
1. Удалить установленную ранее БД.
2. Установить новую БД с именем cometa.
3. Подключиться к БД cometa, создать пользователя admin с правами администратора.
4. Под admin создать в БД cometa несколько таблиц (table1, table2, etc), наполнить их любым количеством данных.
5. Найти датафайлы, файл параметров и управляющие файлы базы cometa.
6. Почитать про alert-лог БД, найти его.
7. Почитать про listener в БД Oracle, создать и настроить его с помощью команды netca.

После выполнения задания необходимо приложить (скриншотами) результат выполнения следующих команд (все команды выполнять под пользователем oracle):

* ```ls -lh датафайлы```
* ```ls -lh файлы параметров```
* ```ls -lh управляющие файлы```
* ```ls -lh alert-лог```

* ```lsnrctl status```

* ```env | grep ORA```

* ```sqlplus -s / as sysdba```
  * ```SET LINESIZE 230```
  * ```select name, created, open_mode, DATABASE_ROLE from v$database;```
  * ```select VERSION_FULL, status, DATABASE_STATUS, INSTANCE_ROLE from v$instance;```
  * ```select * from DBA_ROLE_PRIVS where GRANTED_ROLE='DBA';```
  * ```desc ADMIN.TABLE1;```
  * ```desc ADMIN.TABLE2;```
  * ```select * from ADMIN.TABLE1;```
  * ```select * from ADMIN.TABLE2;```
