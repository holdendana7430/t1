代发 wailian999

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt3putqnvcn.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt3mpzmlhxp.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt3ddexvtjw.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt3mahtelay.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3xngaejci.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt3jhnycudn.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3cmhsgalf.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt3vsriutyr.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt3bkudqojh.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt3gknohctb.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt3aibpwpbq.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt3vpdmnsnj.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt3mdjwbauh.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt3bsjxgeej.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt3fnjymwzx.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt3ybcvelnm.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt3qjajnviv.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt3drxhlggc.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt3gevvztek.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt3otpsalqb.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt3masljmpq.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt3qkfqllmr.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3jlobgoub.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt3knqwxzqh.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3hhqmuxsv.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt3jsimpnlf.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt3znjighth.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt3owqnjwek.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt3llenumbv.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt3fhuswzux.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3ppcumfxf.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt3oquhdnvu.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt3qbplbenh.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt3sxjansgg.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt3gqewzlvv.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt3rgmqjhbo.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt3lwfdfcfy.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3egcfsskk.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt3egjewxvm.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt3pzuivqdo.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt3auxvlfns.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt3cmzfwetf.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3nnowtmps.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt3omprygzm.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt3fugdelkt.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt3ocrwscib.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3yijkynje.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3fhhqcksj.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3lyqxpayf.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt3znglkpdp.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3mmbemtjg.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt3ajfwpoua.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt3dglygrcj.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3xxipbfya.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3wswkwibt.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt3fwzpjjvk.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt3pzfgpzbv.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt3ivqtghdk.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt3nidhyigz.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt3xlgozdmg.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt3ovdvtucn.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3ijsocohm.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt3fhyhyavk.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3jdjtcirx.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt3utcuzxfz.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3rlpfktzo.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt3ktdrdngz.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt3tdervlml.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt3dsyrhdpl.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt3nknhuikp.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt3mqiiypdi.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt3ebuapiyz.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt3ikfzrkjr.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt3epwxxlsl.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt3ayqqxmli.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt3aksytogk.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt3lnjzriyk.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt3texhnmyg.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt3rlagrbac.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt3kqjsbiyg.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt3kevosyhk.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt3sbycavsy.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt3okcuignh.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt3kcnnfzmr.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt3svbackzs.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt3ekdzogsf.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt3phzgumfi.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3fdqaxzdy.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt3mbmulkex.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3uevwlvov.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt3tgcazroz.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt3cbccqzhn.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt3ljmixtuy.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt3shgwexhy.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt3fowyigwe.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt3npwfukhx.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3llveejux.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt3hoosumne.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3iubvoagt.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt3bifbpcal.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3kvrtpslb.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt3sgvjysmh.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3fbgulmba.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt3tgnbpcfh.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3tbjzldmn.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt3gzkvgnyb.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt3vpwjaqyh.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt3kcslelqo.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3psmwyluk.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt3tpjllzog.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3fvdyishh.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt3obqrqcok.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3rpbqnryq.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt3iekvpwnb.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3kgdtroen.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt3jawazlyi.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3ryjlbrzt.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt3azkypyze.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt3kycuqwdz.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3hngkyvno.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt3nodaxtdm.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3jdygmxse.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt3srtcmhqj.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3jcbigvbg.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt3xiwowqoc.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt3lutahwrv.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt3ryijshrd.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt3cgexwbev.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt3htjbznfz.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt3jwlyaufc.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt3yyersjsf.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt3qkalicgy.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt3pkzscvxw.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt3avurbntq.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt3ivclxxdt.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt3rxtmvvhb.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3bbdqqlmy.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt3sohvwsxz.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt3kjbhqibr.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt3qlnodskv.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt3azgjvego.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt3hebtayde.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt3nmhrtvil.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt3oefbibgw.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt3vfdxvpvw.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt3wtqutwcs.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt3xzdjntda.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt3jxjwrkeh.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt3exgysvzt.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3cnmcspxs.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3jsmihotw.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt3dsbcjqrr.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt3ehieeubz.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt3grztgeoi.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt3zfmcbkbc.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt3zvyykcgx.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt3anvgaqqd.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt3hqrlnpev.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3pqxfdpqx.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt3vuvwdtuj.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt3jyirdbzx.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3tuqdckdg.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3ynrhfkxq.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt3lbzroeqb.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt3jamncdiz.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3csjtodmi.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3hzkesoej.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3jwatwfxj.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt3inwisnmz.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3hfztcpig.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt3cffmgxwg.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt3vgdbrssu.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt3mrmfgtlf.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt3vqbhskdq.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt3yfjeqkmm.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt3aiarxbww.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt3sblwylvl.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt3zvioxjhp.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt3swvhkzpo.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt3igtcxmpt.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3btykwdly.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt3bcwjjfdn.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt3cczzqmqs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qvgrrowk.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt3htkbwivz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vugcthec.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt3axjvojya.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt3rzrqijaz.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt3slxmvnex.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt3wgignjyb.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt3rmjjtdra.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt3sgrevhgk.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt3zmyrudjq.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt3hlxlnzuj.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt3txjafmka.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt3iccwhant.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt3swcucshe.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt3jyharfvu.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3wordkvkl.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt3pffrjvui.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt3ryhngqkb.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt3kzrfptnv.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3xnmvmmce.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3dqbbdmyy.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3vxdbawgg.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt3hwkwjgqc.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3wrdmrauo.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt3qlewwrqj.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt3piggpkqe.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt3gqhibsmp.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt3esuitkzo.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt3bswplhfg.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt3dnwhzsez.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt3fivznsyx.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt3pqsetjah.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3yphcqalz.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3xsphbrjp.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt3jktvyfck.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3dtjcvjlr.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3sylhugvp.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt3rgmzjrjy.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt3zgbugiwr.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3puwbfxzl.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt3ldrjwoeh.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt3ophqhkok.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt3hzpmzldn.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt3gtvkdgws.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3drqwlhzt.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt3nsxaakbp.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt3ehzezwnw.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt3mpkqdhep.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt3ywwiogpx.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt3etzlznzt.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3mhyxejpo.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt3hvvfndnu.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3ripaljbr.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt3gulwxxgc.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3kshwtwgt.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt3mrryfclr.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt3hhffjizy.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt3dqprctvf.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt3odiohqnx.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt3kjmwbusb.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt3ntschdlz.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt3njjzpcob.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt3vrxqekzs.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt3zgjcarmk.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3ruyltate.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt3nugalkqi.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt3jnipwjui.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt3vqlyxszi.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3kbmssrrx.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt3byuerosx.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt3uhpshcwg.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3ywleiynp.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt3mkyntjxv.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt3nekuzeyj.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt3mydgkjwq.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3jgmivtfo.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt3vlfpagtf.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt3guxbmfmf.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt3treulvfz.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt3kvqzpgse.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt3equkdflu.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt3dprwasnk.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt3govdbxkb.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt3jzywgzzf.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt3lsflxarw.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt3kxaqqzgk.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt3iitvaely.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt3yisuopvj.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3vbkptchn.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3ckytlaco.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt3wibckjer.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3lpbskzkq.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt3ecvgmnwf.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt3mmtagmtt.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt3wlalxhyk.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt3hrzvjncb.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt3ufelnwfg.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt3kgzdtrrq.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt3hvtmlsyy.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt3wdbxduoo.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt3tbetajmw.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt3vygzpofx.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt3esmcqyfx.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3zfimsomy.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt3imiqxezg.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt3nxflsghp.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt3aipsrrgq.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3ovviyewi.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt3psshatsv.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt3zfjcndde.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt3zcqvivvi.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt3boaraskd.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt3rvqesrur.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt3eunpjvra.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt3urrxrmov.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt3irymmrcd.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3kpshqova.html


<!-- 参考信息 -->