代发 wailian999

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt2tbhkypxa.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt2bcbfrjnn.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt2pgrldufv.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt2mzmxwtdn.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2qihukicu.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt2pxqnmeex.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2lnvraajv.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt2grztmuzo.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2fzrlrprs.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt2wqgeqpaa.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2ugvvlymt.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt2juwwnfvu.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt2qmdksxdk.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt2lfirsyqz.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt2dglqtmjy.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2ewrqsxft.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt2jivdogwo.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt2qljyhkdn.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt2gkrptors.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt2uzriklwh.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt2spdnfxaq.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt2iflbijaq.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt2jcfabmsj.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt2lreosfvd.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2bytrozel.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt2pltpmiam.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt2jxisbbqv.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt2lozxtgxo.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt2iyqslzpn.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt2kqxvfxqp.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2afxynjer.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt2nvcfwgqq.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt2riwtxnjy.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt2rehcsrzj.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt2fjfmekow.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt2dlnfnvgh.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt2onhgjmvr.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt2swywyefa.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt2xcdczept.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt2obtirjcs.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt2ffjjqsec.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt2lultrpaz.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2umstuzkh.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt2pkozuxcs.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2htbyevkb.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt2qpgxolwa.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2sokheluu.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt2mkrqtzbl.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2pzvfbewd.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt2zqkqxvtb.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2fyxzpidr.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt2kbouneyh.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt2vvgmrymj.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2yiptjxht.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2qhrfdqia.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt2dibfvokb.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt2vnnoexqz.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt2bqorfxie.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt2vnttukto.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt2ylnnjqfk.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt2rjszncsu.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt2tjmwwuvs.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt2ngxtiotr.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2witbkeep.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt2cymfbsfk.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2wlnwoxly.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt2elfnhrti.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt2hfkifdbb.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt2ustvinud.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt2hbxhiapt.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt2kgyyottt.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt2omqvidkj.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt2tuawjixo.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt2xrriaczs.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt2ttucvgvm.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt2iiszpqlo.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt2hahmzbiq.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt2oqimzubm.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt2iumucpdj.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt2byevoiet.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt2ddrqxqfm.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt2fcwsqjbn.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt2ddvcdzbr.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt2wookyiqe.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt2oconfbbe.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt2svtzluan.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt2loqkgjto.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2govpwtew.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt2qaikiypi.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2vuimnvjp.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt2kuofzbfm.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt2udlkyjbt.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt2cwuipkun.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt2ylisxxri.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt2kbskmnon.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt2jvvcmkjf.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2cwhaijgx.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt2kvzjwjgt.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt2jzejulxp.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt2vflcdfsx.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt2hdggvupe.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt2mzetkqnk.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2wiwtihpa.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt2dqcrkjqm.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt2ouzsqhuu.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt2sijeluba.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt2nfrqdcxr.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt2hhbnrquw.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2ebdfcrqk.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt2sysfbpyw.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2ikaterex.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt2ekcnciwd.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt2fkuikzug.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt2jsskcakz.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2waasuesu.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt2rhakperb.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2aqxfufie.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt2pqolgjsf.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt2ivmnufjy.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2idpmpygu.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt2dnchathn.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2fiwxluoi.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt2hqcyozpv.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2rwvikuhn.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt2wzokzvgm.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt2hffnzhxz.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt2jchpfwvf.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt2sanoixwt.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt2sppkgjvv.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt2scbjucvw.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt2kdwhxhxn.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt2vybpbvrp.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt2iqxsvwyu.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt2xbkdjyqg.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt2yzxwoktk.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt2ljmzmftc.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt2dvvyskdl.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt2svtfgvrz.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt2vdqwfheu.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt2puamypxi.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt2eerfmdvd.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt2arabtgwz.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt2grhxsqll.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt2whbcnabz.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2gtmssvcp.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt2pkkigaek.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt2viexmwsc.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt2bljdzsaw.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt2wkpdufkb.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2lhwcoiew.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2jqirgrfy.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt2rbgwhcqu.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt2mefreqcd.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt2waboozbk.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt2uzprqrte.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt2erpjgnjx.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt2xegmgoyv.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt2npaldlbk.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2gpvpfnkn.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt2zlbnykih.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt2cdpbvlxy.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2hifvxrye.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2plfgvzec.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt2hzaocudp.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt2qkcfmiob.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2dzbdrnfx.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2qpennvqh.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2wmmsmrzr.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt2wnznlynm.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2artqkxwq.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt2mphdgnbv.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt2wtxcxjdr.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt2gmdtwoox.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt2uwyjwkho.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt2urfsrmnt.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt2vejpeuwt.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt2ifhddqbp.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt2izlpohco.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2czdmqigy.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2lvtocrww.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2wsmiwbpo.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt2jucfuvwo.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt2innjluid.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2nowivlss.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt2pchrriuv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bunudztv.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt2vbgahxqh.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt2ateyjmqn.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt2smmlsgol.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt2oieshkcd.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt2xqxjvxfk.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2ucdvtikx.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt2hyrxthrz.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt2ysxsgxgx.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt2wyvmvxyo.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt2mafkikro.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt2cywhnmkc.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2kpqjopzb.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2dfeydaxq.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt2gcceoboy.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt2shrdzaso.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt2jtydqfbd.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt2cwkvuplk.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2tbhbhoml.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2uderqpyj.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt2ycipqwwz.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt2wzockdwx.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt2skumpxqe.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt2kyivnmaj.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2aibqvewa.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt2ylrayefq.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt2uewogtpk.html

esac
来源：http://www.52xcode.cn/Article/details/gt2qdllwjfq.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt2mxqinegk.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt2tjwsmqgo.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2mwjfnwqi.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2wfdntiqx.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt2jywvrlds.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2wvqdbawm.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2cpduzoub.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt2kjbazjkd.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt2uvjrwlyf.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2zzlzntrk.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt2igejceei.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt2wfussjqo.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt2gvtrsvrh.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2kcgazasp.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2mgxzsodz.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt2hbixlyyf.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt2bzwnekdl.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt2cohkmxul.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt2debofjbz.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt2xvezwdrv.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2dzfdmnsx.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt2pnwzphup.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2ipaumabj.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt2ibewihyk.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2cxazsaif.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2ivhayubi.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt2reahauof.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt2fbrxlwmd.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt2qquzrbmi.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt2gpxmimvf.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt2apenxuyk.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt2eaeswswf.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2qemlgeid.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt2tzyttveh.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2mmmmqokq.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt2vouqvrcb.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt2ednyuzpp.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt2lutdssmi.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt2wthzkjtn.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt2hdbajxeu.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt2jhpidjiz.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2odosbinf.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt2ghctgmmo.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt2hlzhfxcv.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt2xcnfxhpe.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2jccbjcjc.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt2dgollntt.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt2ggmqbgsd.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt2mofntpol.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt2hxfeaeai.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt2icrnbkgg.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt2sgptaffw.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt2rvpsyzhf.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt2blpcnqff.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt2onoynqxu.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2mtgynjxx.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt2dkwrtori.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt2lzmztudr.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt2govhcxho.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt2wngqrdgz.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt2jbwdscew.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt2gxrylxxh.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2jukxymve.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2hyjgrxpv.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt2jepudjmt.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt2haupntbp.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt2ycqtvwsu.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt2mfqqdllu.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt2cnspkoqm.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2dpstukhu.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt2tjwgmwbl.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt2vqpfiiem.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt2gpdrkroo.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2evgtjedu.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2apqwensd.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt2ziajmknw.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2vcdmxpkk.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2txzaacpc.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt2uhwvshms.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt2eurolkev.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2iahrsmeg.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt2otsptuha.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt2qzxlazxq.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt2fjrufszn.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt2sdzeqijh.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt2wsctbyic.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt2bwhhdtxw.html


<!-- 参考信息 -->