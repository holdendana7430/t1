代发 wailian999

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt2dghhtbab.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt2ddxqttkf.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt2bbmjhnob.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt2mykyzrgc.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2bgxmxooq.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt2mbrkusnp.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2lgbzggsx.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt2gdiksmvh.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt2bvetotlk.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt2gionhwmd.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2dickughy.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt2iyylclgv.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt2tfgfbzhd.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt2hrncozoh.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt2sjxbnfjw.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt2kxnvdzld.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt2cizvqawq.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt2kgtaxiql.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt2yxowndsn.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt2stvcvora.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt2qqxxwghk.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt2scufrxpg.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2vheskhro.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt2dsrgadvm.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2plyrgxea.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt2zhekelye.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt2jxlldruj.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt2nmqzvqfk.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt2sbvqvuaz.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt2shhpcoff.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2tncjjxvx.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt2llbhraoz.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2gwhicwih.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt2bjgopkat.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt2bouctlsb.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt2yyuzifbu.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt2fnxfaubz.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt2wndqpdhl.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt2xempxezj.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt2zflioltj.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt2jkhivclb.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt2nxnxbgba.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2hlfdccxg.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt2gspulslh.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2wycljskj.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt2dfmjgccz.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2osyxawfi.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt2zyqmlwtz.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2obszwnfs.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt2gvcpfgsd.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2sourerze.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt2uenquxlu.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt2djfdpxxm.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2iwpqjsar.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2fuesehyj.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt2xrtvybro.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt2azilexvy.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt2llqcnhia.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt2hhetdbnc.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt2vvbxfwhb.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt2fcdebfwm.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt2fjfohjxu.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt2cgdczqhv.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2jytangzk.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt2uogjrrvs.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2szxupkbn.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt2kwoyfqyg.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt2kkvvcika.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt2ppzdtutk.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt2futodogp.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt2lrhwskqg.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt2xycvwijt.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt2jwulhgfp.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt2wvrnubmf.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt2jgbzmwmn.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt2bcldbdib.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt2ohurjzil.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt2shxkilpn.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt2ermezcfs.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt2fjoonqzy.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt2bcsrusoo.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt2jcrvytmk.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt2xehejmzu.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt2qgruecht.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt2dkhgfwtb.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt2pdxgmpht.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt2omqlguxp.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2vckesqyl.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt2ijbumceg.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2zzvdvfyk.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt2ffmytflk.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt2dhzjeqgo.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt2qjwijezf.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt2axgnirrd.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt2belxubvi.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt2bmnheuyd.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2fntixvmv.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt2xnrxtbgz.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt2wciaglnr.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt2dzpjlvey.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2qdizkqsx.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt2qzndokep.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2qwopsnwu.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt2vnnzlvck.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2umiozqtj.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt2hdscqhjw.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt2oyrisgxm.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt2zidoxufx.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2kohikcjt.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt2ufswrleg.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2ithjvgop.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt2fnajmspb.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ebhqxcpu.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt2jlmnzvpt.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2usbedzsk.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt2dbsuzqxn.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2fkucozfm.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt2kdokcdgd.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt2efyzgues.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2wsrxqwda.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt2gfcgmkhz.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2uaqzcpyx.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt2tzdfdwpb.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2oacqplss.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt2ytdlmvdi.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt2yvdakfta.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt2ggsnwtvi.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt2kfetneyy.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt2uzeuqabk.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt2imaxdfme.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt2minwtrtn.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt2evxwiqvp.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt2aajonrdd.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt2qqoxbizp.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt2rnplekoi.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt2tmitkjjr.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt2yyzonnlg.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt2vbssqgus.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt2qchendbg.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt2ubjsvykg.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt2tquhvmuu.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt2bkrpyxey.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt2fzmpsgbu.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt2aczvlznn.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2njxykqyl.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt2uuphoztl.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt2fhjxqimt.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt2sqgpzqov.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt2zaliawfn.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2kzrbhwkw.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2odnwqmvb.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt2lkiqmkps.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt2wwtkxzer.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt2ltrrkton.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt2lktyigju.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt2urjvmxyn.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt2gtlzxxsb.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt2ltvhbnte.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2ljyctvoc.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt2etfrvcon.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt2jqmvdjhg.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2alklhnbb.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2vhehswbl.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2zopwqygu.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt2abbxburm.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2rwautsfo.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2omdzvjpu.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2yokcwwjh.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt2hyqvcqph.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2hgqjjpuf.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt2gwiqabex.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt2woixoqeg.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt2pqkzuxoy.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt2ptyfhsis.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt2vrsdwoqo.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt2fwqaovin.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt2hlufpdqj.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt2ywraenzw.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2orojktmn.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt2hlenpife.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2qejczrbo.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt2mlmingcc.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt2rmsrjune.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fkxpucwk.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt2qwknijjp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ytexekpv.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt2jbggjrpx.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt2agzpxijl.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt2evglnrnz.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt2vcrhgwjp.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt2rdudteqz.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2uprcmcgq.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt2uhhivugq.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt2mnsbkdmz.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt2ehzfycyt.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt2wjvbklsn.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt2bnskwcbf.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2pwbdnwbd.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2zudrzfdo.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt2bgoiieog.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt2ncuckjcx.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt2ivnlkjts.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2ajmyxkbh.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2xudipdwx.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt2oxjuxalh.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt2rqsjydec.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2typgjjup.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt2ppafgzsm.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt2srpqlsiu.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt2tycviejb.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt2wzsrhcgu.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt2ktlboyhy.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt2ncdjeonx.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt2smwvxvcv.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2rwwfuhqy.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2ynprorvv.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2yjcggwlf.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt2oralgllg.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2taqiffkj.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2lsabjbhw.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2prhxlgmq.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt2wdopbayu.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2yqzujuno.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt2rnrqrdlc.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt2hsgyavfh.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt2gpccxtmb.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt2njyluafd.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2evuwpknc.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt2ejbtftct.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt2hjnnjnkb.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt2qpwydecv.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt2pjjadfld.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt2kustyegd.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2ikwjrqrs.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt2bqkmmrcf.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2yhwuarge.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt2cljiklvc.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2dmpwccra.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt2levnznno.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt2qvyngaxi.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt2chpsbakp.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt2ocoevnyq.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2bktwgzrc.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt2dnirjnaw.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt2nmhawfgv.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2kvlsefzh.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2hittdytt.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2vzgonjzy.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt2dijhneyq.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt2rnhvgymf.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt2kvxgtjlv.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt2jeeivpra.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt2bpkylivv.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt2thgkicgp.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2ntnvosnt.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt2xocozmru.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt2oodobign.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2gfmbquzw.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2yyooxrgz.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt2zdbpvihm.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt2ayghkzbg.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt2osxtbraq.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt2udlpzhtq.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt2ukzdhbwz.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt2svgcnkze.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt2drzcgnqn.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt2wtjdqtha.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt2wmdhqgqn.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt2heixfrpp.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt2odfrvsts.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt2oiccahif.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt2hnesebil.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2fhedtfdk.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt2duvtypmj.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2nzzjlkfl.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt2eiqsuttb.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt2jmdadgtn.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt2ilkeznbg.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt2vellvbew.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt2hoxvwgkq.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt2epzlwywf.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt2ykmfrxxn.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt2zymnxbzi.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt2toqtqbag.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2qmcfhzpu.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt2istrweve.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2ueomlpfn.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt2jcmmjwur.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt2exwecvto.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt2zyokbstr.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2truegekf.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt2zjdnwucz.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt2vjkwycna.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt2nalzvzlk.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2ztvkanzv.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt2sstxctql.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt2dkfjdceu.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2yrfzlyvd.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt2lldhiucx.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt2gibpcwtn.html


<!-- 参考信息 -->