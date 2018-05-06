# day2.2
数据库的查询语句

查询所有行所有类
select * from Students

查询部分行
select * from Students where QQ='140663777' 

查询部分列
select StudentName,Age,Address from Students

指定列别名
select StudenName as 姓名，age as 年龄 from Students
select Address + '='+ StudentName from Students

常量列
select StudentName,123 as 体重 from Students

限定行数
select top 3 * from Students
select top 10 percent * from Students

排序（降序）
select * from Students where address='上海' order byStudentNo desc
select * from Students order by asc

获取长度并打印输出
select LeN(StudentName) as 姓名 StudentName from Studnets

当前日期
select GETDATE()
往后加3个月
select DATEADD(MM,3,GETDATE())

对年龄求和
select sum(age) from Students
求平均成绩
select AVG(avg) from Students
最大最小
select MAX(age),MIN(age) from Studnets

模糊查询
select * from studnet where stuname like '%value%'

数据库增删改查
创建数据库
create database dbname

删除数据库
drop database dbname

创建数据库表
create table tname()
---括号里是需要的各种参数

删除表
drop table tname

增加
insert into tname(student) values(studentno,studentname,studentaddress,studentage)
删除
delete from  tname
delete from tname where studentname="tangming"
更新
update tname set studentname="huahua" where shtedntno=1


给表添加主键
alter table tname add primary key(col)



