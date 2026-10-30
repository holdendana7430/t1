代发 wailian999

CREATE INDEX idx_users_email ON users(email);
来源：http://baike.fehbvm.com/Article/details/gerfvnrny.sHtML

[Q09] 创建唯一索引
来源：http://wap.fehbvm.com/Article/details/gerlmyvhn.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://baike.fehbvm.com/Article/details/geyfvipez.sHtML

[Q10] 插入单行
来源：http://3g.fehbvm.com/Article/details/gbyzqdfik.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.share.fehbvm.com/Article/details/ghpfefzxi.sHtML

[Q11] 一次插入多行
来源：http://3g.fehbvm.com/Article/details/ggfaxyocn.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://3g.zdbjq.cn/Article/details/gazmjjbto.sHtML

[Q12] 插入后取自增 ID
来源：http://mobile.hesvh.cn/Article/details/gahtruwqz.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://3g.zdbjq.cn/Article/details/glwqgqmle.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://blog.zdbjq.cn/Article/details/gsxwcxgww.sHtML

[Q13] 忽略重复插入
来源：http://mobile.fehbvm.com/Article/details/gumrjvzvw.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.share.zdbjq.cn/Article/details/gqsinqppy.sHtML

[Q14] 存在则更新（upsert）
来源：http://blog.hesvh.cn/Article/details/guatzjhor.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://read.share.fehbvm.com/Article/details/gededuzfi.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://baike.hesvh.cn/Article/details/gyryuatwr.sHtML

[Q15] 查询全部
来源：http://baike.zdbjq.cn/Article/details/gsawabiuw.sHtML

SELECT * FROM users;
来源：http://baike.hesvh.cn/Article/details/gyugujcjv.sHtML

[Q16] 查询指定列
来源：http://www.share.zdbjq.cn/Article/details/gyrwibodi.sHtML

SELECT id, name FROM users;
来源：http://read.share.hesvh.cn/Article/details/gucwxqaah.sHtML

[Q17] 条件查询
来源：http://www.m.share.hesvh.cn/Article/details/gfuxohllp.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.blog.zdbjq.cn/Article/details/gzcymvbip.sHtML

[Q18] 模糊匹配
来源：http://mobile.hesvh.cn/Article/details/gsmteduvn.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://mobile.fehbvm.com/Article/details/gvvpqsjwg.sHtML

[Q19] 范围查询
来源：http://www.share.hesvh.cn/Article/details/gupynofdc.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://m.share.zdbjq.cn/Article/details/gamajllhi.sHtML

[Q20] IN 列表
来源：http://wap.fehbvm.com/Article/details/gvtqkjhfc.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.blog.fehbvm.com/Article/details/gfyhcpwkz.sHtML

[Q21] 空值判断
来源：http://www.blog.hesvh.cn/Article/details/gegnfhzhz.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://baike.hesvh.cn/Article/details/gcpumthgk.sHtML

[Q22] 排序
来源：http://wap.zdbjq.cn/Article/details/gjgkerawg.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://wap.zdbjq.cn/Article/details/gzocyckzr.sHtML

[Q23] 分页
来源：http://www.share.fehbvm.com/Article/details/gbbdnfson.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://mobile.fehbvm.com/Article/details/ghgksbroy.sHtML

[Q24] 去重
来源：http://www.blog.hesvh.cn/Article/details/gqyvjjicy.sHtML

SELECT DISTINCT city FROM users;
来源：http://wap.zdbjq.cn/Article/details/gesezpkfr.sHtML

[Q25] 只取前 N 条
来源：http://mobile.hesvh.cn/Article/details/gvxyrtgjx.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.m.share.hesvh.cn/Article/details/gyasvlaeu.sHtML

[Q26] 计数
来源：http://wap.zdbjq.cn/Article/details/glzwhozil.sHtML

SELECT COUNT(*) FROM users;
来源：http://m.share.hesvh.cn/Article/details/gnwxwfshh.sHtML

[Q27] 条件计数
来源：http://www.m.share.hesvh.cn/Article/details/gatcqotys.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://mobile.fehbvm.com/Article/details/gwnlqxwwq.sHtML

[Q28] 求和与平均
来源：http://www.m.share.hesvh.cn/Article/details/gxgrnxtup.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://baike.hesvh.cn/Article/details/gkzsnksvw.sHtML

[Q29] 最大最小值
来源：http://www.blog.fehbvm.com/Article/details/gczxhteha.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.share.hesvh.cn/Article/details/glbbyackk.sHtML

[Q30] 分组统计
来源：http://wap.fehbvm.com/Article/details/geqeuzszv.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://mobile.fehbvm.com/Article/details/gjwugfjeu.sHtML

[Q31] 分组后过滤
来源：http://www.share.fehbvm.com/Article/details/gqfxcxtye.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.blog.zdbjq.cn/Article/details/ghlfxkhze.sHtML

[Q32] 分组拼接字符串
来源：http://www.m.share.fehbvm.com/Article/details/gpsvjayqp.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://mobile.zdbjq.cn/Article/details/giryavnqy.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://read.share.fehbvm.com/Article/details/gehdbgqkc.sHtML

[Q33] 多列分组
来源：http://m.share.fehbvm.com/Article/details/gwinpgwwb.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.blog.fehbvm.com/Article/details/gutufognz.sHtML

[Q34] 每组取第一条
来源：http://3g.hesvh.cn/Article/details/gnkcyplxl.sHtML

SELECT * FROM (
来源：http://www.m.share.hesvh.cn/Article/details/ghceywckc.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.blog.zdbjq.cn/Article/details/gwowkxdeo.sHtML

) t WHERE rn = 1;
来源：http://www.share.zdbjq.cn/Article/details/gmbxixnat.sHtML

[Q35] 内连接
来源：http://www.share.hesvh.cn/Article/details/gtvqphahs.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.share.hesvh.cn/Article/details/gabojcezb.sHtML

[Q36] 左连接
来源：http://blog.hesvh.cn/Article/details/gvlsbqhjv.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.share.fehbvm.com/Article/details/guatuvmun.sHtML

[Q37] 右连接
来源：http://baike.hesvh.cn/Article/details/gbpvarktv.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.share.hesvh.cn/Article/details/gxckbjwzy.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://wap.zdbjq.cn/Article/details/grggidogs.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://baike.zdbjq.cn/Article/details/gggwqnzff.sHtML

[Q39] 自连接（查上下级）
来源：http://3g.fehbvm.com/Article/details/gustsvzhf.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.m.share.fehbvm.com/Article/details/gskoxjaok.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://wap.hesvh.cn/Article/details/gaonutnzy.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.m.share.zdbjq.cn/Article/details/ggsvnafmj.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.m.share.zdbjq.cn/Article/details/gmkvkufha.sHtML

[Q41] 多表连接
来源：http://m.share.fehbvm.com/Article/details/ghtupqvjc.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://wap.fehbvm.com/Article/details/guimkbblu.sHtML

JOIN users u ON u.id = o.user_id
来源：http://baike.zdbjq.cn/Article/details/gbulygbfj.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.share.fehbvm.com/Article/details/gysjtfboe.sHtML

[Q42] 连接条件附加过滤
来源：http://mobile.zdbjq.cn/Article/details/gsgeytpav.sHtML

SELECT u.name, o.amount FROM users u
来源：http://blog.hesvh.cn/Article/details/gnoutbcxx.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://blog.hesvh.cn/Article/details/gwhieuwvg.sHtML

[Q43] 标量子查询
来源：http://www.blog.zdbjq.cn/Article/details/glmwcdvrp.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://3g.fehbvm.com/Article/details/gdsatrycq.sHtML

[Q44] IN 子查询
来源：http://baike.fehbvm.com/Article/details/ghfbjltvq.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://wap.hesvh.cn/Article/details/gqsaqtual.sHtML

[Q45] EXISTS 判断存在
来源：http://wap.hesvh.cn/Article/details/gqyalkwqk.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.zdbjq.cn/Article/details/gvlhqbseo.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://3g.fehbvm.com/Article/details/gpwnnajhk.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.fehbvm.com/Article/details/grmthguxr.sHtML

[Q47] 与平均值比较
来源：http://read.share.hesvh.cn/Article/details/gdeeaofzu.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.m.share.hesvh.cn/Article/details/gwubfanxj.sHtML

[Q48] CTE 公用表表达式
来源：http://blog.zdbjq.cn/Article/details/gqhwosjle.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.blog.zdbjq.cn/Article/details/gkxhspqky.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://m.share.fehbvm.com/Article/details/gvssxwdap.sHtML

[Q49] 更新单行
来源：http://www.share.fehbvm.com/Article/details/gywygpdip.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.blog.fehbvm.com/Article/details/gyrcfyyum.sHtML

[Q50] 批量更新
来源：http://read.share.hesvh.cn/Article/details/gwpqpbeap.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.share.zdbjq.cn/Article/details/gupumcoqd.sHtML

[Q51] 用子查询更新
来源：http://mobile.zdbjq.cn/Article/details/gzahmsueh.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.m.share.hesvh.cn/Article/details/gftmpqwov.sHtML

[Q52] 删除指定行
来源：http://3g.zdbjq.cn/Article/details/gkekkkrxd.sHtML

DELETE FROM users WHERE id = 10;
来源：http://baike.fehbvm.com/Article/details/gnjncpvkw.sHtML

[Q53] 按条件删除
来源：http://wap.zdbjq.cn/Article/details/gyslayzcq.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://mobile.hesvh.cn/Article/details/gpdmvibcx.sHtML

[Q54] 清空表
来源：http://baike.fehbvm.com/Article/details/gedumwkob.sHtML

TRUNCATE TABLE logs;
来源：http://baike.hesvh.cn/Article/details/ghmhyjxpk.sHtML

[Q55] 排名（并列占位）
来源：http://read.share.hesvh.cn/Article/details/gojkwfycc.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://m.share.hesvh.cn/Article/details/gokjsmhtr.sHtML

[Q56] 密集排名（并列不占位）
来源：http://3g.zdbjq.cn/Article/details/gaubzvhoj.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://blog.zdbjq.cn/Article/details/gnetordzo.sHtML

[Q57] 行号
来源：http://www.blog.zdbjq.cn/Article/details/gvejtmrid.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gechcmzfa.sHtML

[Q58] 累计求和
来源：http://www.share.fehbvm.com/Article/details/glfttqjwv.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://wap.zdbjq.cn/Article/details/gqtoeejbm.sHtML

[Q59] 分组内累计
来源：http://wap.fehbvm.com/Article/details/gfjpdzadm.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://read.share.zdbjq.cn/Article/details/ghmcwvjhx.sHtML

[Q60] 取上一行 / 下一行
来源：http://wap.hesvh.cn/Article/details/gjvqdacxz.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://mobile.zdbjq.cn/Article/details/gtkfowjxx.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://m.share.zdbjq.cn/Article/details/gepsfaqbx.sHtML

[Q61] 移动平均
来源：http://m.share.zdbjq.cn/Article/details/goxwjkzlt.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.blog.zdbjq.cn/Article/details/glhjyjnjx.sHtML

[Q62] 分组占比
来源：http://wap.hesvh.cn/Article/details/gqyveosug.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://blog.fehbvm.com/Article/details/gldomfspz.sHtML

[Q63] 开启事务
来源：http://wap.fehbvm.com/Article/details/gmpiefrum.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://blog.zdbjq.cn/Article/details/gggqoeipt.sHtML

[Q64] 提交事务
来源：http://www.m.share.zdbjq.cn/Article/details/grfnofbuy.sHtML

COMMIT;
来源：http://www.share.fehbvm.com/Article/details/gtostarnb.sHtML

[Q65] 回滚事务
来源：http://3g.fehbvm.com/Article/details/gwjjlwsfb.sHtML

ROLLBACK;
来源：http://wap.fehbvm.com/Article/details/gcvukbgdq.sHtML

[Q66] 行锁查询
来源：http://read.share.fehbvm.com/Article/details/ghhpebjcm.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.share.fehbvm.com/Article/details/gmmieyxbl.sHtML

[Q67] 设置隔离级别
来源：http://blog.fehbvm.com/Article/details/gjmugpuxu.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://blog.hesvh.cn/Article/details/gnvcaxdtc.sHtML

[Q68] 保存点
来源：http://baike.hesvh.cn/Article/details/gjmrjvxwt.sHtML

SAVEPOINT sp1;
来源：http://www.m.share.fehbvm.com/Article/details/ggsfflxhd.sHtML

ROLLBACK TO sp1;
来源：http://baike.fehbvm.com/Article/details/gwhrvfbwd.sHtML

[Q69] 查看执行计划
来源：http://wap.hesvh.cn/Article/details/gtwffescl.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://read.share.fehbvm.com/Article/details/gymbinyae.sHtML

[Q70] 更新统计信息
来源：http://3g.fehbvm.com/Article/details/gkmlnztnz.sHtML

ANALYZE TABLE users;
来源：http://blog.zdbjq.cn/Article/details/gnwyxdqiz.sHtML

[Q71] 查看建表语句
来源：http://blog.hesvh.cn/Article/details/goihpgfol.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://read.share.zdbjq.cn/Article/details/gqvmnrdrw.sHtML

[Q72] 查看索引
来源：http://3g.hesvh.cn/Article/details/gfrdjzzhu.sHtML

SHOW INDEX FROM users;
来源：http://blog.hesvh.cn/Article/details/gkrxrkyxw.sHtML

[Q73] 查看表状态
来源：http://m.share.hesvh.cn/Article/details/gkvnmrwin.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://read.share.zdbjq.cn/Article/details/guecfqrju.sHtML

[Q74] 强制使用索引
来源：http://wap.hesvh.cn/Article/details/gostpwusd.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.blog.hesvh.cn/Article/details/gtpbibdwd.sHtML

[Q75] 日期格式化
来源：http://blog.zdbjq.cn/Article/details/gkfpjexxh.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://m.share.fehbvm.com/Article/details/gebxztspi.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://wap.hesvh.cn/Article/details/gvjvgdgvo.sHtML

[Q76] 按天统计
来源：http://wap.hesvh.cn/Article/details/gahusppti.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://m.share.fehbvm.com/Article/details/gcklhrsuj.sHtML

[Q77] 时间加减
来源：http://read.share.fehbvm.com/Article/details/gwrmldltz.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.share.hesvh.cn/Article/details/gjrqxdqlw.sHtML

[Q78] 当前时间
来源：http://www.blog.zdbjq.cn/Article/details/gvptzvxuo.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://m.share.hesvh.cn/Article/details/gjruagttl.sHtML

[Q79] 字符串拼接
来源：http://3g.hesvh.cn/Article/details/gltxmojir.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://baike.zdbjq.cn/Article/details/gxvvlcluf.sHtML

[Q80] 字符串截取
来源：http://www.share.zdbjq.cn/Article/details/gupnyzdin.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://3g.zdbjq.cn/Article/details/gfkojxilz.sHtML

[Q81] 字符串替换
来源：http://m.share.fehbvm.com/Article/details/gjgxqtpfa.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://m.share.hesvh.cn/Article/details/gnheigerk.sHtML

[Q82] 字符长度与字节长度
来源：http://www.m.share.hesvh.cn/Article/details/gkuyserpq.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gamnbmlwv.sHtML

[Q83] 大小写转换
来源：http://www.m.share.fehbvm.com/Article/details/gzegwkmlo.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://mobile.fehbvm.com/Article/details/gdhitidib.sHtML

[Q84] 去除首尾空格
来源：http://mobile.zdbjq.cn/Article/details/geuvfbndc.sHtML

SELECT TRIM(name) FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gibsddnhg.sHtML

[Q85] 数值取整
来源：http://www.m.share.hesvh.cn/Article/details/gbnugfpxk.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.blog.zdbjq.cn/Article/details/gucqhoume.sHtML

[Q86] 读取 JSON 字段
来源：http://mobile.zdbjq.cn/Article/details/gvqfcczqh.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://blog.zdbjq.cn/Article/details/grpqelcpj.sHtML

[Q87] JSON 字段做条件
来源：http://m.share.zdbjq.cn/Article/details/gojeuiysn.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://m.share.hesvh.cn/Article/details/grqirzwrf.sHtML

[Q88] 行转列（条件聚合）
来源：http://3g.zdbjq.cn/Article/details/gcqbcdfws.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.blog.hesvh.cn/Article/details/gbwtjydyh.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://wap.fehbvm.com/Article/details/gypzytxsb.sHtML

[Q89] 判断表是否存在
来源：http://www.blog.hesvh.cn/Article/details/gxsebrdss.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://wap.hesvh.cn/Article/details/gwvzyzlky.sHtML

[Q90] 生成序号列
来源：http://read.share.hesvh.cn/Article/details/gfjnnywrw.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://wap.fehbvm.com/Article/details/gmkqmjbvu.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/grcigexbt.sHtML

R. Bash 专题
来源：http://wap.fehbvm.com/Article/details/glwarqbkx.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gkdfkygqr.sHtML

[R01] shebang 与严格模式
来源：http://m.share.zdbjq.cn/Article/details/ghrsjzfxt.sHtML

#!/usr/bin/env bash
来源：http://www.m.share.fehbvm.com/Article/details/gbkpjrujx.sHtML

set -euo pipefail
来源：http://baike.fehbvm.com/Article/details/gbhfvfusz.sHtML

[R02] 变量赋值与使用
来源：http://www.m.share.zdbjq.cn/Article/details/gngombzit.sHtML

name="Tom"; echo "$name"
来源：http://baike.zdbjq.cn/Article/details/gtrkpnciz.sHtML

[R03] 只读变量
来源：http://m.share.fehbvm.com/Article/details/gizufpich.sHtML

readonly PI=3.14
来源：http://mobile.zdbjq.cn/Article/details/giphfcjen.sHtML

[R04] 位置参数
来源：http://www.share.hesvh.cn/Article/details/ggiuuekqm.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.m.share.fehbvm.com/Article/details/gmabpzubg.sHtML

[R05] 参数默认值
来源：http://www.blog.zdbjq.cn/Article/details/geomoedua.sHtML

name="${1:-default}"
来源：http://3g.fehbvm.com/Article/details/gtirnpztp.sHtML

[R06] 判断命令是否存在
来源：http://mobile.zdbjq.cn/Article/details/gzdajdhcz.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.m.share.zdbjq.cn/Article/details/gimngcdvo.sHtML

[R07] if 判断文件
来源：http://blog.zdbjq.cn/Article/details/ghkxorcmy.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://baike.fehbvm.com/Article/details/grstilasc.sHtML

[R08] 数值比较
来源：http://www.blog.fehbvm.com/Article/details/gyfotzjys.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://3g.fehbvm.com/Article/details/gzabgmgsh.sHtML

[R09] 字符串比较
来源：http://mobile.fehbvm.com/Article/details/gqfpamnkv.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://read.share.hesvh.cn/Article/details/gzbxjekqp.sHtML

[R10] 正则匹配
来源：http://www.blog.zdbjq.cn/Article/details/gojxkiovt.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://mobile.zdbjq.cn/Article/details/gzqoaahgu.sHtML

[R11] case 多分支
来源：http://3g.hesvh.cn/Article/details/grtmgidhk.sHtML

case "$1" in
来源：http://3g.fehbvm.com/Article/details/gpeenmldu.sHtML

start) echo "启动" ;;
来源：http://read.share.zdbjq.cn/Article/details/gkhyhoccx.sHtML

stop)  echo "停止" ;;
来源：http://baike.hesvh.cn/Article/details/gbuscfpze.sHtML

*)     echo "未知命令" ;;
来源：http://baike.zdbjq.cn/Article/details/gxxjgjnbq.sHtML

esac
来源：http://www.blog.zdbjq.cn/Article/details/gzzwlgjtk.sHtML

[R12] for 遍历文件
来源：http://www.blog.zdbjq.cn/Article/details/glapoiedo.sHtML

for f in *.txt; do echo "$f"; done
来源：http://mobile.fehbvm.com/Article/details/gjtzeycgj.sHtML

[R13] for 计数循环
来源：http://www.blog.fehbvm.com/Article/details/gblpwoahj.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.blog.zdbjq.cn/Article/details/gvvdsrhen.sHtML

[R14] C 风格 for
来源：http://mobile.hesvh.cn/Article/details/gmmphbdrd.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://read.share.hesvh.cn/Article/details/grqufdjpa.sHtML

[R15] while 逐行读文件
来源：http://baike.hesvh.cn/Article/details/gquumsnem.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://read.share.fehbvm.com/Article/details/gbqaarrii.sHtML

[R16] until 等待条件
来源：http://wap.zdbjq.cn/Article/details/grvqhfqww.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://wap.hesvh.cn/Article/details/gcmkozqme.sHtML

[R17] 数组定义与取值
来源：http://m.share.fehbvm.com/Article/details/gpsflvayq.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://wap.hesvh.cn/Article/details/giocncmuq.sHtML

[R18] 遍历数组
来源：http://www.blog.fehbvm.com/Article/details/gaxbqclmy.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://baike.zdbjq.cn/Article/details/gwheyphzf.sHtML

[R19] 数组长度
来源：http://mobile.fehbvm.com/Article/details/ggjvhstpo.sHtML

echo "${#arr[@]}"
来源：http://mobile.fehbvm.com/Article/details/gzdwtkivg.sHtML

[R20] 关联数组（字典）
来源：http://wap.hesvh.cn/Article/details/ggiqbuluv.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://blog.hesvh.cn/Article/details/gmwnctzps.sHtML

[R21] 字符串长度
来源：http://www.share.hesvh.cn/Article/details/gsekvrbio.sHtML

echo "${#s}"
来源：http://3g.zdbjq.cn/Article/details/ghymxbdqp.sHtML

[R22] 截取子串
来源：http://wap.fehbvm.com/Article/details/gmeykskef.sHtML

echo "${s:0:5}"
来源：http://read.share.fehbvm.com/Article/details/gafptxvgx.sHtML

[R23] 字符串替换
来源：http://m.share.zdbjq.cn/Article/details/gvveltczp.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://baike.hesvh.cn/Article/details/gfxqzmofo.sHtML

[R24] 大小写转换
来源：http://3g.hesvh.cn/Article/details/gtnsutfeu.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://baike.hesvh.cn/Article/details/gdmunddsj.sHtML

[R25] 去后缀 / 去前缀
来源：http://wap.hesvh.cn/Article/details/gjysmasxx.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://mobile.zdbjq.cn/Article/details/gbvcqtbyq.sHtML

[R26] 命令替换
来源：http://mobile.hesvh.cn/Article/details/gxvrhzrcx.sHtML

now=$(date +%F); echo "$now"
来源：http://wap.hesvh.cn/Article/details/giewophtm.sHtML

[R27] 算术展开
来源：http://www.share.zdbjq.cn/Article/details/gjasfcvzc.sHtML

echo $((1 + 2 * 3))
来源：http://www.blog.hesvh.cn/Article/details/gwfcyhzhr.sHtML

[R28] 浮点运算
来源：http://read.share.fehbvm.com/Article/details/gmhpcpjbh.sHtML

echo "scale=2; 10/3" | bc
来源：http://baike.fehbvm.com/Article/details/ggqorsqtb.sHtML

[R29] 定义函数
来源：http://mobile.hesvh.cn/Article/details/gwzsbkakj.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://3g.zdbjq.cn/Article/details/gfumzotfc.sHtML

[R30] 函数返回状态码
来源：http://www.share.hesvh.cn/Article/details/gwjitgscd.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.m.share.zdbjq.cn/Article/details/gdnelgvbs.sHtML

[R31] 局部变量
来源：http://baike.hesvh.cn/Article/details/giakliprr.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.m.share.fehbvm.com/Article/details/gtybqrvmp.sHtML

[R32] 参数个数校验
来源：http://baike.zdbjq.cn/Article/details/gmwwuesei.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://m.share.fehbvm.com/Article/details/gradzeshq.sHtML

[R33] 捕获错误并提示行号
来源：http://www.m.share.fehbvm.com/Article/details/gkenqpjnc.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://mobile.fehbvm.com/Article/details/gtayrtpfb.sHtML

[R34] 退出时清理
来源：http://www.blog.hesvh.cn/Article/details/gxnndfvia.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.fehbvm.com/Article/details/gikcsrlzl.sHtML

[R35] 后台执行并等待
来源：http://www.m.share.zdbjq.cn/Article/details/gvecqdcay.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://m.share.hesvh.cn/Article/details/gmweeubyh.sHtML

[R36] 并发执行多个任务
来源：http://wap.fehbvm.com/Article/details/gvdqtzbls.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://m.share.hesvh.cn/Article/details/gtlhltzzd.sHtML

[R37] 把输出赋给变量
来源：http://wap.hesvh.cn/Article/details/gdaxsleww.sHtML

files=$(ls -1)
来源：http://3g.zdbjq.cn/Article/details/glsfcexjo.sHtML

[R38] 管道串联
来源：http://www.share.fehbvm.com/Article/details/giaxwgexx.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.m.share.hesvh.cn/Article/details/gutuipexn.sHtML

[R39] 重定向标准输出与错误
来源：http://3g.fehbvm.com/Article/details/gdwpxedsz.sHtML

cmd > out.log 2>&1
来源：http://3g.hesvh.cn/Article/details/grtvhyaej.sHtML

[R40] 追加写日志
来源：http://mobile.fehbvm.com/Article/details/gvjoznqtg.sHtML

echo "log" >> out.log
来源：http://blog.fehbvm.com/Article/details/gitaqgdcq.sHtML

[R41] 丢弃输出
来源：http://m.share.hesvh.cn/Article/details/ghfrvsvhc.sHtML

cmd >/dev/null 2>&1
来源：http://blog.zdbjq.cn/Article/details/gvwifvlyx.sHtML

[R42] 输入重定向
来源：http://wap.hesvh.cn/Article/details/gqlwzhwwy.sHtML

wc -l < a.txt
来源：http://mobile.fehbvm.com/Article/details/gpizbcmox.sHtML

[R43] 按名字查找文件
来源：http://wap.fehbvm.com/Article/details/govelpdqd.sHtML

find . -name "*.log" -type f
来源：http://wap.hesvh.cn/Article/details/gmszeedhl.sHtML

[R44] 按修改时间查找
来源：http://m.share.hesvh.cn/Article/details/gnpiizseg.sHtML

find . -mtime -7 -type f
来源：http://www.blog.zdbjq.cn/Article/details/gxmqugjxi.sHtML

[R45] 批量删除
来源：http://mobile.zdbjq.cn/Article/details/gaunssdjn.sHtML

find . -name "*.tmp" -delete
来源：http://m.share.hesvh.cn/Article/details/gahhfdbnp.sHtML

[R46] 递归替换文件内容
来源：http://m.share.hesvh.cn/Article/details/gdhomjorx.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.share.hesvh.cn/Article/details/ggawkgdln.sHtML

[R47] sed 单行替换
来源：http://www.m.share.zdbjq.cn/Article/details/gevcstplo.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://wap.zdbjq.cn/Article/details/gxfmwlmrt.sHtML

[R48] awk 取指定列
来源：http://blog.zdbjq.cn/Article/details/gtpxhlbwz.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.m.share.zdbjq.cn/Article/details/gcrljylek.sHtML

[R49] awk 带条件
来源：http://www.blog.hesvh.cn/Article/details/gmwfzjcra.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wap.hesvh.cn/Article/details/gdevbexsr.sHtML

[R50] awk 求和
来源：http://read.share.hesvh.cn/Article/details/gsqgnerre.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.m.share.fehbvm.com/Article/details/grmgzowcd.sHtML

[R51] 排序去重取前几
来源：http://baike.zdbjq.cn/Article/details/grukvykjh.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://mobile.hesvh.cn/Article/details/gavrsszdo.sHtML

[R52] 统计行数
来源：http://www.m.share.zdbjq.cn/Article/details/gnarcsdwx.sHtML

wc -l a.txt
来源：http://read.share.hesvh.cn/Article/details/ggjnviamj.sHtML

[R53] 查看文件头与实时尾
来源：http://www.blog.hesvh.cn/Article/details/gvzfvuphw.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://m.share.fehbvm.com/Article/details/gpxxlbmip.sHtML

[R54] 比较两个文件
来源：http://m.share.zdbjq.cn/Article/details/gmkhtctoi.sHtML

diff a.txt b.txt
来源：http://read.share.hesvh.cn/Article/details/govqkzizz.sHtML

[R55] 压缩与解压
来源：http://m.share.zdbjq.cn/Article/details/gvkgauzfx.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.m.share.fehbvm.com/Article/details/gnzbpwhfx.sHtML

[R56] 远程拷贝
来源：http://www.m.share.zdbjq.cn/Article/details/gkhaxvmiq.sHtML

scp file user@host:/path/
来源：http://baike.fehbvm.com/Article/details/gjwvfutkf.sHtML

[R57] 远程执行命令
来源：http://www.share.zdbjq.cn/Article/details/gyzgjyjwj.sHtML


<!-- 参考信息 -->