# Постгрес

## Полезные ссылки

1. [Дока](https://www.postgresql.org/docs/)

## Поиск по репе

- `#ТЮНИНГ` - куски конспекта в которой описаны какие (отличные от дефолтных) значения выставлять в конфигах
- `#БЕСТ_ПРАКТИС` - бест практисы

## Полезные команды

В psql
```sql
\! - выполнение команды, например `\! vi /var/lib/postgresql/data/pg_hba.conf`
\conninfo - просмотр, под кем мы залогинены
-- You are connected to database "postgres" as user "postgres" via socket in "/var/run/postgresql" at port "5432".
\h  -- help, например `\h select`
\?  -- справка по всем командам
\l  -- list databases
\dn  -- list of schemas
\dt  -- list of relations , Кроме простых таблиц, также существуют и [другие отношения](https://www.postgresql.org/docs/15/catalog-pg-class.html)
\c wb -- connect to database wb
\d+ test  -- просмотр мета информации по таблице тест

-- 
wb=#  -- база данных вб, = - ждем ввода команды (альтернатива `-` - ждет окончания ввода, `;`), # - суперпользователь 

```