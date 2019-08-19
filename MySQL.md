#MySQL

####启动
命令:mysql -u root -p


####创建数据库
```sql
    create database tutorial
```
####创建表
```sql
    create table tutorials_tbl(
        tutorial_id INT NOT NULL AUTO_INCREMENT,
        tutorial_title VARCHAR(100) NOT NULL,
        tutorial_author VARCHAR(40) NOT NULL,
        submission_date DATE,
        PRIMARY KEY ( tutorial_id )
    );
```