代发 wailian999

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3yeksizns.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3enpvvdbw.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt3opnqauir.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt3mkixdbyv.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3ampwjstb.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt3pkwarhwt.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt3hdfkzizp.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt3xukqcule.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt3bgfqprnt.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt3jbzwfqat.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt3rzrumjpo.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt3euilefzk.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt3ywokwerr.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt3bgfdbdpr.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt3hfiokvvh.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt3kgtvyhjw.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3mqxbphye.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt3cauzlvpu.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3jlrxgqsn.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt3qbqbzrsj.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3twjljwnf.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt3admulely.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3xxtsiucs.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt3fufdexai.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt3lzdgzxda.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt3vxfrdwrl.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt3bhynyjyo.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt3kxqkvnta.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt3kgylqnhs.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt3eyqatjeh.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt3nezqrvcn.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt3dgofoepq.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3mxbgjwwg.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt3xspwzsxw.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt3onoyiryu.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt3xgzlhamo.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3emqpeybu.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt3rhycicnj.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt3ufxfhaew.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt3tbgqwozz.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt3gmupsekr.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt3swagftnz.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt3jtorjwat.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt3feylfbsh.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt3urzfgsfu.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt3qiwcmtkw.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt3wvxlzpaw.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt3aceebnke.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt3nrbzrygh.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3zlwermsw.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3tcpffvex.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt3fmiiixus.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt3bvgvhjzp.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt3rmmqwwdv.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ijzvfmnb.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt3xkivpgej.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3jhrmtuvw.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt3hpwoixwq.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3ryraltip.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3xypyclfi.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3cbptsblj.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt3fagmaefl.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3atamykzx.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt3npwffhfx.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt3wfwuzafu.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3ylhwzjnn.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3ctqpydtr.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt3bbbqbqjb.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt3cuombsmf.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt3wntqvbdy.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt3vhgkqenp.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt3pfvwraov.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt3ovoravay.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt3irswiyru.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt3mpfifort.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3apiulfxw.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt3skdqxjlq.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3hehamuyj.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt3gihzdxle.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt3njjeuovu.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt3zeqgxfrb.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt3xeagkrif.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt3xpkgyyyy.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt3lmmhqsxp.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt3eqqikwxg.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt3zvmgdzqu.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt3hnyjfoto.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt3rxpcopis.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt3drzqzvnh.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt3pxygmkvr.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt3lkhhosmn.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt3bacprtyo.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt3wdvruvxx.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt3jrzivdqn.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt3dmgaidyn.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt3xaounqcz.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt3oadkxdvs.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt3ydllbkfx.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt3irmawpku.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3tzwqhmvz.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt3gxeepscx.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3opgfweka.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt3jsiawfit.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt3zppylxef.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt3ziqfxetw.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt3tfwabqgg.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt3buwtxxth.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt3yltybcpb.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3tnmfrehg.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt3wnjdlusz.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt3yomatmlv.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt3htugptxj.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3bkgolnnl.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt3bacjwfrg.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3ozgwbnhi.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt3gxhivyod.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3opezmfjg.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt3wmaaxjpy.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt3xpkmdhug.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt3hcyxpayy.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3tksknugh.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt3qjvjxfyl.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3vprkypam.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt3zmbdrlga.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt3jqbzoqtt.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt3ednhndip.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3zechceyn.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt3negoiafp.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3zmeysojy.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt3mcmwjggx.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt3khouhkco.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3fegzhcnf.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt3qaoezvou.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3oumvpawt.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt3zizijzky.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3zkzvfjwj.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt3vxcajbhe.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt3qplehmzy.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt3xotdgimu.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt3fhxbnqut.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt3ivyoikdy.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt3pvjptvdz.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt3zsciofdr.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt3kypedmdl.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt3utrmzvcc.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt3xlkyzgek.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt3gbjwfqmj.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt3tdbdqmjq.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt3ueoihhdm.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt3notyqmed.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt3ownifjum.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt3sxyfcdlm.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt3eawpqjlp.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt3mhbwcxyv.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt3qgagxorh.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt3ewdybawy.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3pqwkjozr.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt3qmuqilme.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt3pjgdnimn.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt3qyulqevo.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt3txztayzx.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3xqrfcmym.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3wgbeopag.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt3zsoqvsol.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt3ffjxvzof.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt3ioqwnpao.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt3mglwbnui.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt3xaahgqaw.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt3ibomeyqf.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt3clepgkyh.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3dzwfwxcb.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt3kyiucfxp.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt3gqrpszgq.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3chrwlpxm.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3apfvpkxs.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3rnlynnix.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt3msfrxkbc.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3fifnjyhg.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3reldyujt.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3klnjzvzo.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt3ylyjomdb.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3qfzevpgy.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt3jlmcxqfx.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt3mwhbgbwe.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt3fdigylxs.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt3xgnuqjqj.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt3hcsgzmxe.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt3aebjxrgh.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt3ifrglygi.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt3hhudwgvl.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt3lccgsbxa.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3xjfbafrw.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt3dejqyqpo.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt3lfmyszwt.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt3rdszgpwd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3omjzpehf.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt3clgnrzfg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3cmgwaeub.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt3ivphuyjl.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt3vrhgzgpu.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt3utkjikgo.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt3drlrvysz.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt3sgraigvj.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt3rcdlreud.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt3xrdmzerf.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt3rovycppk.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt3gxwlisxc.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt3jpgeclqb.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt3igbgbqnh.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt3ktkxgutz.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3uqjxkulr.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt3eeuzpkoc.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3wwylqmzo.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt3abrcauiy.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt3lvesukpw.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3iiqalzrl.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3sqbqwieb.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt3aciymlbm.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3sqyfhtiw.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt3oxzfwepm.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt3kqpjediy.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt3ezlfzqnm.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt3ftoanlcx.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt3mqxjndie.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt3hvggqktq.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt3qeljtcib.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt3ufgusnux.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3kzvoaebe.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3smjftkez.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt3cyscmbzg.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3nimebual.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3pcexepht.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt3cvzukbyk.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt3dixzlbsf.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3wklxuvsi.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt3rqwupfrb.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt3cbyosfte.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt3prewqgbe.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt3kojjtjau.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3yefndufd.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt3jtrxuido.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt3ihkqsljm.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt3gypywzuq.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt3xtxwcipu.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt3dqjgzwjo.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3ufmecbob.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt3gdsqdmmi.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3dkwosctz.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt3logifxxx.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3vlmwdfii.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt3titczzev.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt3qohoqxry.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt3hqvzaywb.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt3pnfdyiax.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt3mnsxgsxb.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt3juhcgwnh.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt3zgiqaqxf.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt3fhikeryv.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt3ammnmkjm.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3ihotulzn.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt3llhdtfui.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt3qctbgctx.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt3pzwekqcn.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3rntzutjm.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt3ilhfogvr.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt3edcwcywy.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3ysbkwidg.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt3ynmbhlio.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt3rzoucmyp.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt3teptuzwq.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3mojwmaqp.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt3crtnkagm.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt3inxygpik.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt3qbdzxkbb.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt3pbmnqvoe.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt3ryepzxow.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt3jycchvrm.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt3lwxoxcyr.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt3ygviklic.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt3rgxlqkio.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt3dwrrsduo.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt3midebpdg.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt3plskqhho.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt3pwupsbzv.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt3tnybwajm.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt3vshimuky.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt3arbsglzx.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt3ucysjzif.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt3qzxehzje.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt3ovtffstx.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt3andwmcpi.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt3enbcqllu.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt3scivdufr.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt3pffodqzj.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt3bhxsnodt.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt3iaxyxyra.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3txvpcmqo.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt3sruwgoms.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3odgefiud.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt3folzkafe.html


<!-- 参考信息 -->