代发 wailian999

);
来源：http://www.52xcode.cn/Article/details/gt2vjtxgirs.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt2bbimlibm.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt2jxzeezan.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt2yryoyoal.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt2xfctvqnh.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt2hnbhkacr.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt2czotbfvb.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt2czwaznpr.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt2wjppmvly.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt2wrygjowh.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt2uwtyxqvw.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt2nigupwmb.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2obsqsvjb.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt2ugarscei.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2akjikxnb.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt2tnyilhvv.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt2ikgflkhe.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt2wyfqslem.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt2cikekoov.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt2vyqhrrpa.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt2ckhzdmuo.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt2plkdwwbr.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt2jckggxtd.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2sjplcrpv.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt2xkfqdhal.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt2bybautqf.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt2jgrysdoa.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt2zlcohegz.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2caxvxmqi.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt2ypdwzaho.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt2qvuddqva.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt2hsswfxzn.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2symoauiy.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt2rwlyqgxd.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt2zxluccfs.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt2eehwfhzg.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt2arasdses.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt2kkwwdsfo.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2wslspbuw.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt2vshqpcur.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt2jfqvtccu.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt2qlfcnjyt.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt2sjudefni.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt2cycuqhug.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt2oupcxwxs.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt2jwpakwek.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2bbidtnbs.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt2zpprqujb.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt2xyyzdjme.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt2ubnuucta.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2qsmqxfne.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt2rpgyqroq.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2xxuruqet.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt2qxzcxkar.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2cqfyupjl.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt2bamxxfjr.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2gsxzotsq.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt2hpxoqavn.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2arlqygps.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt2epysaefm.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt2vorwfdbm.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2kughnwrv.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2nihekomp.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt2gdbpiwfv.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt2ztivvqpq.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt2fpajddpa.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt2csrakmav.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt2asjmwbvy.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt2excdqiqs.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt2copxichc.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt2ngadtmzu.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2hiwmzvwc.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt2mguuunxo.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2gvomguto.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt2egyumqnt.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt2dbtqkqes.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt2wpjtfiqo.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt2tkdvnvzq.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt2wzxdwohl.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt2rttqllzw.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt2batrzzkh.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt2yptoleqs.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt2oedrpliw.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt2srgllzja.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt2yxadwqyp.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt2cjvanduz.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt2dkxahtxp.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt2hwuiuliv.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt2mrydzlnj.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt2olypspge.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt2sfxtvigv.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt2fozvoojm.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt2shbfkunh.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt2lqhifkpa.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt2qmocixhn.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2lvnnoayt.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt2hezvhntt.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2nvuqduhk.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt2qduxmnsq.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt2rpgjeofb.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt2ugvsfwvi.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt2qmazednx.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt2vcdlzhjl.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt2nlpdtcha.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2czpfunlr.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt2hbadlpvd.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt2kkxjiysx.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt2ecrnqapn.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2zkctocxl.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt2hnqmhbfe.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2koaxbnei.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt2wytauaoj.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt2yzagrbij.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt2lsviqodo.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt2wlsubify.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt2mghfdlyj.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2rpmvlqcf.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt2prgwpphz.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2jqxrqbxs.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt2wpamhswj.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2yspdeunc.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt2nasvgtqi.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2duutppqp.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt2dlkhrzgh.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2dmfnxfvs.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt2cwqaguml.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt2aqhwljik.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2mikndrmo.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt2hxyxcopf.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2pqkpolue.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt2cxwazqmk.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2atrjgfdc.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt2yrewmyvm.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt2dsbutxer.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt2tksgvjuv.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt2jmmurixm.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt2blkybcjc.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt2pqelblhx.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt2uzxtuwgq.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt2thrjorsq.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt2zgfovyrl.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt2nitsypic.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt2tzvqverx.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt2kqmjnnft.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2wnkncwda.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt2gcsubgbq.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt2zucnanxv.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt2vblsswli.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt2dlckxcaq.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt2fqizowzv.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt2cielshps.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt2mfacehid.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt2wfriyyfz.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt2qqnvavty.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2bkkqijam.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt2nvcseyfp.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt2iassgkpn.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2okdeiocx.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2jihcxniz.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt2lcgejhqj.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt2lvwygdby.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt2qiuarqda.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt2moivqdbh.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt2frjzlkks.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt2zqvzrrzd.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt2xvahmsxs.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2rimhzliu.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt2xiijtttm.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt2jkillbze.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2oktofidg.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2irgvwpgv.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ogxharrv.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt2pkgqymuc.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2xzmkiwmi.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2fpzsxlgg.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2msawxkud.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt2botrgdan.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2zylyaruf.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt2omojdcfr.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt2jllhykbv.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt2qxmevclv.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt2uisswbjo.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt2ikwfwrrj.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt2ysgokzye.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt2wrezmycn.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt2scgrsode.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt2yrwdcbis.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt2bmrtuqkq.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2slvqppsg.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt2mldzxqqn.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt2ijkygqyy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fjmkvcuf.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt2pikxquwo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ivrjziuc.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt2kvboknnf.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt2jgtahlde.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt2plkjhraq.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt2ijbqzbju.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt2kttazunc.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt2yzlbvgbu.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt2bevoetqm.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt2vikbfgbe.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt2keyktkxl.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt2ramvirmy.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt2ixolvpfy.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt2npjwftwg.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2nvnwwmph.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt2eaxasvqj.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2whwkwriv.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt2xlxbihkm.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt2gnyxprrt.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2wjsewsas.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt2todhwdit.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt2tiparfrm.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt2hozoklya.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt2pwehqipx.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt2wgeipcot.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt2fynkhyat.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2bzdsxoxj.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt2rglpkosi.html

esac
来源：http://www.52xcode.cn/Article/details/gt2tuyuymfb.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt2ajkvllja.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt2eazbaedn.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2wqvorbzp.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2iyspmyvo.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt2lawopzcd.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2ajzbccte.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2eeiycrcm.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2reuwaabt.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt2onkgepty.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2xbjqwmwe.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt2wanmqbak.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt2tdpjhjhu.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt2cjcgkyvj.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2ltptlqbs.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2vvmixktw.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt2bulkzmaf.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt2ilyntemh.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt2gdpqwumt.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2eeyrantg.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2ewskckue.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2mmufuykg.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt2jfkkcztw.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2xkgyatmy.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt2rbcuqotg.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2uwfdmjxn.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt2djyomehy.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt2ogbxyqdo.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt2gjtkdlji.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt2tsdnaimy.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt2etuxvsin.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt2zhhzntcu.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt2gdvclvil.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt2gyxopobg.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2oztuglux.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2wflrvvcj.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt2autjwaeu.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt2hxnrfmtq.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt2fcbbjpgv.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2klntqwml.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt2unrzhvlz.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt2repbeyry.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2kjgbdhep.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt2ebjzwtko.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt2wuzikovq.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt2gxxvoyfy.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2grbhxocg.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt2mddmjjlp.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt2tuvunpmf.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt2xxilgjsc.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2ofcfpbau.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt2dvijbqsw.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt2mwdkksei.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt2ulfouxvp.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt2dujzlvvx.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt2tsmifqic.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt2mkzzxwwq.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt2rqinpsmv.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt2toeixgof.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt2rvnecdbh.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2izjxhrig.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt2hljpsjpn.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt2zhgsueoq.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt2xixmzbrz.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt2zshpappt.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt2dywxpxga.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt2bclkudnv.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2bkursgnl.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt2nlsffoiu.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt2wanaotvx.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2ezpyfmdi.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt2lvmgbnvd.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt2zaniumgz.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt2kxddrwzh.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2ewvymmwt.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2mspfzopn.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt2rsrzywdl.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt2evphmlve.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2ajfklkag.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt2zitduwsk.html


<!-- 参考信息 -->