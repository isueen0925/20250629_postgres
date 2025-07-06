## 建立資料表的語法

```sql
CREATE TABLE [IF NOT EXISTS] table_name (
   column1 datatype(length) column_constraint,
   column2 datatype(length) column_constraint,
   ...
   table_constraints
);
```

## 建立一個student的資料表

```sql
CREATE TABLE IF NOT EXISTS student(
   student_id SERIAL PRIMARY KEY,
   name varchar(20) NOT NULL,
   major varchar(20) UNIQUE
);
```

## 刪除資料表

```sql
DROP TABLE IF EXISTS student;
```

## 新增1筆資料

```sql
INSERT INTO student (name, major)
VALUES ('吳育君','歷史');
```

## 新增多筆資料

```sql
INSERT INTO student (name, major)
VALUES ('小柱','生物'),('信忠','英語');
```