代发 wailian999

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3yrnitngi.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt3wevcbrqf.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt3cyukkpud.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt3gffilbeh.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt3zwyiwfsk.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt3moyfbvxw.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt3wodtilmd.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt3ejaqnxoy.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3nicjpcyp.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt3afaoojjr.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3vilxmphh.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt3zoxjbjbs.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3fjrmkmhc.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt3amxdqgkn.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3obzsriiy.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt3yzmvqatl.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt3dfacxubi.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt3qhdxojer.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt3gegnstlp.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt3jkvkcpmd.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt3ocnnfvgo.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt3svrawxkz.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt3jzhxyjlw.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt3xamfrqui.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3lxmbnzdg.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt3byfqocev.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3elleekqq.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt3qrjszoij.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3pokvwguu.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt3yeabqmfg.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt3mzxpanrj.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt3shlpzcdr.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt3zdmrjnxj.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt3cfiedlkm.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt3umuijell.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt3ynnikdqa.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt3hzznuwgo.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt3qlyrgzlo.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt3kgrzmqdy.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt3dgfcfvxw.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt3dsemklvv.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3zmiitnnf.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt3yrdpxfpe.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt3xsdwvxkc.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt3iwysrwid.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt3zmfropok.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3lobjqtuu.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt3nomulmus.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3tykclzhl.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt3utmtazon.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3neijakek.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3glsmtwev.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3aurpeyrf.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt3zanqcncw.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3jqbibwgk.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt3vubwfaat.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt3uqhgtpvy.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3mteoeiiy.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3fhdoppax.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt3fdpbproy.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt3hzsyxsjo.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt3naayqprl.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt3bgnlhfvi.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt3titvbsyf.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt3lmlpjwgg.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt3cmjzcuox.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt3jxjdgkcr.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3nnjkkzae.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt3npthlrnl.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3vihgwyqf.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt3yieaxnoc.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt3shsxnoeo.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt3jrjrlmej.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt3btadqgmr.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt3siwgeuln.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt3icclvagy.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt3esrwomvg.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt3ctdpfpbr.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt3hwzlpotv.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt3vazlvhog.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt3lghdpdjr.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt3niyuoyzm.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt3goiqxeli.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt3aoeamvxc.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt3eunqroga.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt3nuwsuswk.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt3ltxcddxr.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt3znoxyzyi.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt3scgdaywq.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt3msyhclao.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt3cguiaoqs.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3zcdvmtpe.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt3onfmruzi.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3xpyrulht.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt3sfvwrrrq.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt3uocdiuvi.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt3gcazsmlf.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt3shtmnygu.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt3pswxnkko.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt3orifcbot.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3cjafmbvg.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt3oijhkwak.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt3rxmvegnw.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt3cjvphtru.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3nmuzprvx.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt3vycxvdqr.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3flfctpao.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt3xslqouhb.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3avcmxodw.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt3jxkwkodo.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt3pcbftgmy.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt3esmmiucb.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3vjnymixu.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt3oymtxzyb.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3imyejgdj.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt3fpqcerrh.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ntwcezvt.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt3hvwwzsjn.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3sqdawmjv.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt3bqbxcnmj.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3ocovgarr.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt3icsvzibq.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt3tpavfepi.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3ajvfpjho.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt3edudyjfw.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3xfzzezdb.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt3enagwjot.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3qdgdvcdw.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt3exiamsoe.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt3qiavdgtl.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt3ywdrxkpp.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt3bafjtfpl.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt3fuycbckq.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt3nmwfmixd.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt3xwmmgvfi.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt3noambdwu.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt3qkdmpngo.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt3lfdexbwh.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt3xqcpkgwn.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3bwenfynu.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3yyguvllr.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt3klamhpqr.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt3kwxsnsad.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt3kvpyvweq.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt3udbipcts.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt3ivayybsw.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt3dyxfoxqr.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt3nlrlbiws.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3qwpbyllr.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt3urzgxbyg.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3cqgvvapv.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt3fecsaojj.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt3jkwroxnt.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3biqjglnw.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3hthumjce.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt3ccqxmixh.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt3lealubsj.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt3debuoghh.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt3tjjsppsc.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt3yluadkgp.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt3hgdpoqbn.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt3kxotarbc.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3bgytotgl.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt3dpxojcsb.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt3thhjgtlx.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3lohugoso.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3fzcpckrm.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3eoctnjlf.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt3nsdirezy.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3hpmemwqk.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3nhhlxftv.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ffgnftvl.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt3sacwahql.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3hvwkycbc.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt3gsawbrot.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt3abxfokso.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt3volvmevh.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt3yqljqrfu.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt3pmhmrvwa.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt3lqdibjhq.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt3xkbyqhoa.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt3xircbvzl.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt3cdggdngk.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3avovhwnt.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3sbgjckft.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt3uwiwuysr.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt3dpvrgpcw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3thxzgpug.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt3sltktrlz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3yrxlzdhr.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt3gnzowubj.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt3yplqttzt.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt3uatwrrku.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt3blpzkrhh.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt3kcsusyss.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt3oznvdhgw.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt3mrskdymp.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt3wyofupgj.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt3mzqcowma.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt3zeqehtui.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt3lzmqtlac.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt3furnftsk.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3zpqtnjcm.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt3ucyrmaab.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt3waeeblgw.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt3aziajczi.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3szzryscm.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3uaalhnsg.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3uyxdjdap.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt3gqxcjcsp.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3jvvyilvf.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt3fysycxep.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt3yxniocjx.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3ieiuvcne.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt3rdbpmdis.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt3bzhvxuzk.html

esac
来源：http://www.52xcode.cn/Article/details/gt3bxxvsiot.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt3xiqjsehu.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt3xzcnofpz.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3akcackwf.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3bapqdxnq.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt3oosdppdl.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3skqvkylv.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3qobssovv.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt3bqnszfrm.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt3hewdybgv.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3daipvpno.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt3xdjgmsqs.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt3swhgzrbp.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt3tonpuary.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt3hsgpsdrd.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3wnzharlx.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt3ohjlawhu.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt3irlloimv.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt3jyzguaxl.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3vmdfcjkr.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt3mtsyrlsp.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3htdlpilv.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt3hgehcxqh.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3vgghnrnc.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt3fltewxgv.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3apawkbjy.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt3uqpifbrl.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt3yljehnmp.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt3iytiuqgi.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt3iedvhhdw.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt3seeafpbz.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt3wwoshxhc.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt3tnwewgqv.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt3abidxuau.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt3rutvscsq.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3prfkgwfe.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt3nttoshmb.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt3fryricuo.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt3itfjolez.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3jweqtqnt.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt3nqluiiix.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt3noiaklfn.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3odrcephz.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt3kgwuzqdo.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt3igmddwbr.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt3ikvzhjqr.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3tcecucqx.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt3tcymbedq.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt3qakfmzol.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt3wwmehrys.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt3ddzbtdpa.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt3ugxrpkbw.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt3cjxtcsqz.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt3zfqfhwba.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt3mhxpsgot.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt3fnxocfpn.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3estytsns.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt3ygyxxydn.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt3imsdfygt.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt3ubntirjj.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt3dsjxmokh.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt3yjyicuye.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt3atnyemqd.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt3lvhfbulc.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt3ecpgdokn.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt3iqzbymew.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt3vjkwzqld.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt3bzmbhvmk.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt3toenoczh.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt3jqytqaxy.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt3ebmwmnml.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt3nrvdiruo.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3hoaeplhr.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt3gqudgjam.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3utgjuzku.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt3vpfmdyno.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt3ocpbjbpk.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt3yvgtwebi.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3cjyxtzkg.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt3ydxzdbfq.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt3epefiwtx.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt3ygwiikhc.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt3cdpcxmbc.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt3xlbeylik.html


<!-- 参考信息 -->