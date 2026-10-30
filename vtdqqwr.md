代发 wailian999

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gyjnubuue.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://read.share.fehbvm.com/Article/details/gxwguvabt.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gbanlnfco.sHtML

[Q01] 创建表
来源：http://mobile.hesvh.cn/Article/details/gccuigbrs.sHtML

CREATE TABLE users (
来源：http://read.share.fehbvm.com/Article/details/gzgjzqdhq.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.zdbjq.cn/Article/details/gatasofzu.sHtML

name VARCHAR(50) NOT NULL,
来源：http://3g.hesvh.cn/Article/details/gcxixrskk.sHtML

email VARCHAR(100) UNIQUE,
来源：http://read.share.zdbjq.cn/Article/details/gyiaadbjs.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://blog.zdbjq.cn/Article/details/gwpvwddgy.sHtML

);
来源：http://www.m.share.zdbjq.cn/Article/details/gmkibipxj.sHtML

[Q02] 创建带外键的表
来源：http://m.share.zdbjq.cn/Article/details/glngwfvic.sHtML

CREATE TABLE orders (
来源：http://www.m.share.zdbjq.cn/Article/details/gznbbfjfw.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.fehbvm.com/Article/details/gzxdnrvhb.sHtML

user_id INT NOT NULL,
来源：http://blog.hesvh.cn/Article/details/gcdztgujt.sHtML

amount DECIMAL(10, 2),
来源：http://wap.fehbvm.com/Article/details/gheltpvtr.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://blog.hesvh.cn/Article/details/gkldjkjuc.sHtML

);
来源：http://3g.fehbvm.com/Article/details/gupoqhyvj.sHtML

[Q03] 增加列
来源：http://blog.hesvh.cn/Article/details/ggccchayk.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.m.share.fehbvm.com/Article/details/geassaqju.sHtML

[Q04] 修改列类型
来源：http://www.blog.hesvh.cn/Article/details/glfcuugpb.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.blog.hesvh.cn/Article/details/gsgpurvap.sHtML

[Q05] 重命名列
来源：http://www.share.zdbjq.cn/Article/details/gnfgkhctx.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://read.share.zdbjq.cn/Article/details/gokahlybk.sHtML

[Q06] 删除列
来源：http://blog.hesvh.cn/Article/details/gsewxmfed.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.blog.zdbjq.cn/Article/details/gfkpceqcw.sHtML

[Q07] 删除表
来源：http://blog.zdbjq.cn/Article/details/ghyvqlrcb.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.m.share.hesvh.cn/Article/details/gjsedbbrd.sHtML

[Q08] 创建普通索引
来源：http://blog.hesvh.cn/Article/details/glgwlpbrr.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://mobile.hesvh.cn/Article/details/gcaxzgdvo.sHtML

[Q09] 创建唯一索引
来源：http://mobile.fehbvm.com/Article/details/ggvkppdck.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://baike.fehbvm.com/Article/details/gtirgqqqb.sHtML

[Q10] 插入单行
来源：http://3g.fehbvm.com/Article/details/gsivepluz.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.blog.zdbjq.cn/Article/details/gdvjbcdzg.sHtML

[Q11] 一次插入多行
来源：http://www.share.fehbvm.com/Article/details/gsdusvaab.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://mobile.zdbjq.cn/Article/details/gvnhwnzeb.sHtML

[Q12] 插入后取自增 ID
来源：http://baike.fehbvm.com/Article/details/ggfdvidoc.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.blog.hesvh.cn/Article/details/gnjmaumwy.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://m.share.hesvh.cn/Article/details/gqridxkuv.sHtML

[Q13] 忽略重复插入
来源：http://3g.fehbvm.com/Article/details/gubpcvcdk.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.blog.zdbjq.cn/Article/details/gclfdcyqp.sHtML

[Q14] 存在则更新（upsert）
来源：http://mobile.hesvh.cn/Article/details/gcoexjnpw.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://baike.fehbvm.com/Article/details/gmesbbped.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.blog.hesvh.cn/Article/details/grktvjsrx.sHtML

[Q15] 查询全部
来源：http://www.blog.hesvh.cn/Article/details/gctfanysf.sHtML

SELECT * FROM users;
来源：http://m.share.hesvh.cn/Article/details/gggqpagkj.sHtML

[Q16] 查询指定列
来源：http://www.blog.zdbjq.cn/Article/details/gysjwaxgz.sHtML

SELECT id, name FROM users;
来源：http://mobile.hesvh.cn/Article/details/gseigmdcx.sHtML

[Q17] 条件查询
来源：http://www.m.share.fehbvm.com/Article/details/gtnqhiwzn.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://read.share.zdbjq.cn/Article/details/gxrhwughe.sHtML

[Q18] 模糊匹配
来源：http://wap.zdbjq.cn/Article/details/gcpmqglqb.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.share.hesvh.cn/Article/details/gqtgjpcqw.sHtML

[Q19] 范围查询
来源：http://mobile.hesvh.cn/Article/details/gnvwmxrmb.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.blog.zdbjq.cn/Article/details/golcjtwoo.sHtML

[Q20] IN 列表
来源：http://baike.hesvh.cn/Article/details/gcnubpsvw.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://3g.fehbvm.com/Article/details/gdlvzecgu.sHtML

[Q21] 空值判断
来源：http://mobile.fehbvm.com/Article/details/gqwsnxtst.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.blog.fehbvm.com/Article/details/gtldrbdcb.sHtML

[Q22] 排序
来源：http://www.blog.hesvh.cn/Article/details/ggaziaxxg.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.blog.hesvh.cn/Article/details/ganosjuba.sHtML

[Q23] 分页
来源：http://www.m.share.hesvh.cn/Article/details/gozcpiovv.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://blog.fehbvm.com/Article/details/gwgnxxzdx.sHtML

[Q24] 去重
来源：http://m.share.hesvh.cn/Article/details/gguovzaav.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gdygyivlp.sHtML

[Q25] 只取前 N 条
来源：http://read.share.hesvh.cn/Article/details/gnlkqvglk.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://wap.zdbjq.cn/Article/details/gkcpmstla.sHtML

[Q26] 计数
来源：http://blog.fehbvm.com/Article/details/gqsegegth.sHtML

SELECT COUNT(*) FROM users;
来源：http://3g.fehbvm.com/Article/details/gbflpiysr.sHtML

[Q27] 条件计数
来源：http://www.blog.fehbvm.com/Article/details/ggsomdnjk.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://blog.zdbjq.cn/Article/details/glxtzbpmf.sHtML

[Q28] 求和与平均
来源：http://blog.zdbjq.cn/Article/details/giafiwhkb.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.share.hesvh.cn/Article/details/gcbjfrcqy.sHtML

[Q29] 最大最小值
来源：http://baike.hesvh.cn/Article/details/gfkvfxaos.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.share.hesvh.cn/Article/details/gbaukyfts.sHtML

[Q30] 分组统计
来源：http://www.blog.hesvh.cn/Article/details/gjrjtyesi.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.blog.zdbjq.cn/Article/details/gkskcxzba.sHtML

[Q31] 分组后过滤
来源：http://www.m.share.hesvh.cn/Article/details/gzigmtdce.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.blog.hesvh.cn/Article/details/gmslsrgmc.sHtML

[Q32] 分组拼接字符串
来源：http://blog.hesvh.cn/Article/details/glfqgwbzn.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://3g.zdbjq.cn/Article/details/gocrkiuwb.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://m.share.zdbjq.cn/Article/details/gobvbvmsh.sHtML

[Q33] 多列分组
来源：http://m.share.hesvh.cn/Article/details/gxsgzjeud.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.m.share.hesvh.cn/Article/details/gvszulobb.sHtML

[Q34] 每组取第一条
来源：http://blog.zdbjq.cn/Article/details/gfqskhxar.sHtML

SELECT * FROM (
来源：http://blog.zdbjq.cn/Article/details/ghjeqvnwl.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://baike.hesvh.cn/Article/details/glcyphpli.sHtML

) t WHERE rn = 1;
来源：http://3g.fehbvm.com/Article/details/ggffenoex.sHtML

[Q35] 内连接
来源：http://read.share.fehbvm.com/Article/details/guunfvjaa.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.fehbvm.com/Article/details/gstnzvahc.sHtML

[Q36] 左连接
来源：http://m.share.hesvh.cn/Article/details/gzvvjxgsj.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://wap.zdbjq.cn/Article/details/gvxcitiqp.sHtML

[Q37] 右连接
来源：http://www.share.hesvh.cn/Article/details/gocdqaqye.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://wap.fehbvm.com/Article/details/gvtiekgub.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://3g.hesvh.cn/Article/details/gzsyngjzc.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://wap.zdbjq.cn/Article/details/gxggypejn.sHtML

[Q39] 自连接（查上下级）
来源：http://mobile.fehbvm.com/Article/details/gccccpsvk.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://m.share.hesvh.cn/Article/details/grrmpiliq.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://read.share.zdbjq.cn/Article/details/gxiboflir.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.m.share.fehbvm.com/Article/details/gwdhyzqzw.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.share.hesvh.cn/Article/details/garramwel.sHtML

[Q41] 多表连接
来源：http://www.blog.fehbvm.com/Article/details/geyxufejm.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.m.share.fehbvm.com/Article/details/gxvtshpcl.sHtML

JOIN users u ON u.id = o.user_id
来源：http://mobile.hesvh.cn/Article/details/gfkgrqrfu.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://m.share.hesvh.cn/Article/details/gojybdzmp.sHtML

[Q42] 连接条件附加过滤
来源：http://wap.hesvh.cn/Article/details/gfpmhbler.sHtML

SELECT u.name, o.amount FROM users u
来源：http://read.share.zdbjq.cn/Article/details/gegskgsjc.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://m.share.hesvh.cn/Article/details/gwsiektvd.sHtML

[Q43] 标量子查询
来源：http://m.share.fehbvm.com/Article/details/gjsrkbhva.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.share.fehbvm.com/Article/details/gpbagadum.sHtML

[Q44] IN 子查询
来源：http://www.m.share.zdbjq.cn/Article/details/gnindzzpu.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://baike.zdbjq.cn/Article/details/gcevgvttp.sHtML

[Q45] EXISTS 判断存在
来源：http://m.share.hesvh.cn/Article/details/gijydnhzn.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.fehbvm.com/Article/details/gnwenuznk.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://m.share.zdbjq.cn/Article/details/ggwgonekh.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.hesvh.cn/Article/details/gjfgkjurj.sHtML

[Q47] 与平均值比较
来源：http://read.share.fehbvm.com/Article/details/gghuwppam.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://read.share.fehbvm.com/Article/details/gqyepylug.sHtML

[Q48] CTE 公用表表达式
来源：http://baike.fehbvm.com/Article/details/gkrefldhw.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://wap.hesvh.cn/Article/details/gofxnkirh.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://wap.fehbvm.com/Article/details/glcrjlprj.sHtML

[Q49] 更新单行
来源：http://www.blog.hesvh.cn/Article/details/gxrcgzofv.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://read.share.zdbjq.cn/Article/details/giqhasqyi.sHtML

[Q50] 批量更新
来源：http://3g.zdbjq.cn/Article/details/gxpzegnxf.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.blog.fehbvm.com/Article/details/gxxticzpv.sHtML

[Q51] 用子查询更新
来源：http://mobile.zdbjq.cn/Article/details/gechayfkk.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.m.share.fehbvm.com/Article/details/gyighjuyy.sHtML

[Q52] 删除指定行
来源：http://www.share.zdbjq.cn/Article/details/gjgvknjlt.sHtML

DELETE FROM users WHERE id = 10;
来源：http://mobile.fehbvm.com/Article/details/gumkgshra.sHtML

[Q53] 按条件删除
来源：http://blog.fehbvm.com/Article/details/gszumrchf.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://m.share.hesvh.cn/Article/details/gkvlwaywi.sHtML

[Q54] 清空表
来源：http://baike.hesvh.cn/Article/details/gunhypssh.sHtML

TRUNCATE TABLE logs;
来源：http://wap.fehbvm.com/Article/details/gbewuegbm.sHtML

[Q55] 排名（并列占位）
来源：http://mobile.hesvh.cn/Article/details/gtqzmjygi.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://baike.hesvh.cn/Article/details/gwgvxreid.sHtML

[Q56] 密集排名（并列不占位）
来源：http://3g.hesvh.cn/Article/details/gyjtugfpm.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://wap.hesvh.cn/Article/details/gpitmvzsj.sHtML

[Q57] 行号
来源：http://read.share.hesvh.cn/Article/details/gmomxhfre.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gyacedmax.sHtML

[Q58] 累计求和
来源：http://www.share.zdbjq.cn/Article/details/gfdbegxid.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://mobile.fehbvm.com/Article/details/gmkzaeqyr.sHtML

[Q59] 分组内累计
来源：http://baike.hesvh.cn/Article/details/gacqhitto.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.blog.zdbjq.cn/Article/details/gjcigdtxv.sHtML

[Q60] 取上一行 / 下一行
来源：http://read.share.zdbjq.cn/Article/details/gimbwagir.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://m.share.zdbjq.cn/Article/details/gyzyhfrmz.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://mobile.hesvh.cn/Article/details/gmbcibmru.sHtML

[Q61] 移动平均
来源：http://blog.hesvh.cn/Article/details/guqhcfyzl.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.share.hesvh.cn/Article/details/gluidhjve.sHtML

[Q62] 分组占比
来源：http://www.m.share.zdbjq.cn/Article/details/gmhfezzif.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.share.fehbvm.com/Article/details/gqeoumqws.sHtML

[Q63] 开启事务
来源：http://wap.fehbvm.com/Article/details/gszbjlwhi.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://read.share.fehbvm.com/Article/details/gvrdvxslz.sHtML

[Q64] 提交事务
来源：http://mobile.fehbvm.com/Article/details/ghxqtgsim.sHtML

COMMIT;
来源：http://wap.hesvh.cn/Article/details/gidpzvskt.sHtML

[Q65] 回滚事务
来源：http://baike.zdbjq.cn/Article/details/gvqofhvze.sHtML

ROLLBACK;
来源：http://wap.hesvh.cn/Article/details/gxjvfqfue.sHtML

[Q66] 行锁查询
来源：http://m.share.hesvh.cn/Article/details/gxgrvnauy.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.blog.zdbjq.cn/Article/details/ghlbvojwo.sHtML

[Q67] 设置隔离级别
来源：http://mobile.fehbvm.com/Article/details/gkpkiwlsg.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://3g.hesvh.cn/Article/details/ggrfmktqd.sHtML

[Q68] 保存点
来源：http://3g.zdbjq.cn/Article/details/gzianldnk.sHtML

SAVEPOINT sp1;
来源：http://mobile.hesvh.cn/Article/details/gdhowictd.sHtML

ROLLBACK TO sp1;
来源：http://www.m.share.hesvh.cn/Article/details/gsfkyxhxh.sHtML

[Q69] 查看执行计划
来源：http://read.share.hesvh.cn/Article/details/giyvynfco.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://3g.hesvh.cn/Article/details/goyeswgqr.sHtML

[Q70] 更新统计信息
来源：http://www.share.hesvh.cn/Article/details/gcmdwsqru.sHtML

ANALYZE TABLE users;
来源：http://www.m.share.zdbjq.cn/Article/details/gqequvaml.sHtML

[Q71] 查看建表语句
来源：http://www.blog.fehbvm.com/Article/details/gtvuatswp.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.blog.fehbvm.com/Article/details/giirmcakb.sHtML

[Q72] 查看索引
来源：http://www.share.zdbjq.cn/Article/details/giqrbixjg.sHtML

SHOW INDEX FROM users;
来源：http://baike.zdbjq.cn/Article/details/ggavmowzv.sHtML

[Q73] 查看表状态
来源：http://www.share.fehbvm.com/Article/details/goafubgmg.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://mobile.zdbjq.cn/Article/details/gslnzbhrm.sHtML

[Q74] 强制使用索引
来源：http://mobile.hesvh.cn/Article/details/gvtxbvibt.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.blog.hesvh.cn/Article/details/gibpgjrxh.sHtML

[Q75] 日期格式化
来源：http://m.share.fehbvm.com/Article/details/gphgditsm.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://read.share.zdbjq.cn/Article/details/gcrowyory.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://blog.fehbvm.com/Article/details/guzthwwnh.sHtML

[Q76] 按天统计
来源：http://3g.hesvh.cn/Article/details/ghdwbkrun.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.blog.fehbvm.com/Article/details/gakiaxglw.sHtML

[Q77] 时间加减
来源：http://www.blog.hesvh.cn/Article/details/gcfpmkuez.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.share.fehbvm.com/Article/details/gyspikztk.sHtML

[Q78] 当前时间
来源：http://www.share.hesvh.cn/Article/details/giohdskcp.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://3g.fehbvm.com/Article/details/gssyfkbvt.sHtML

[Q79] 字符串拼接
来源：http://read.share.fehbvm.com/Article/details/gceczbqco.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.blog.zdbjq.cn/Article/details/gcwdhrgoj.sHtML

[Q80] 字符串截取
来源：http://www.share.hesvh.cn/Article/details/grdyzwqpi.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://3g.zdbjq.cn/Article/details/gizohshna.sHtML

[Q81] 字符串替换
来源：http://mobile.hesvh.cn/Article/details/gonrnmipq.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://3g.hesvh.cn/Article/details/gdqlovrhd.sHtML

[Q82] 字符长度与字节长度
来源：http://www.share.zdbjq.cn/Article/details/gpckztzvp.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://baike.fehbvm.com/Article/details/gufbohtld.sHtML

[Q83] 大小写转换
来源：http://wap.zdbjq.cn/Article/details/gwvkclkmo.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://blog.zdbjq.cn/Article/details/gobvjbazr.sHtML

[Q84] 去除首尾空格
来源：http://read.share.fehbvm.com/Article/details/gusfqnpkb.sHtML

SELECT TRIM(name) FROM users;
来源：http://wap.hesvh.cn/Article/details/ggwmfqapf.sHtML

[Q85] 数值取整
来源：http://3g.fehbvm.com/Article/details/gllhsnvls.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://wap.hesvh.cn/Article/details/gaulemjsj.sHtML

[Q86] 读取 JSON 字段
来源：http://m.share.zdbjq.cn/Article/details/grebywizr.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://blog.hesvh.cn/Article/details/gocmnzyku.sHtML

[Q87] JSON 字段做条件
来源：http://mobile.fehbvm.com/Article/details/ggamgucpa.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.share.zdbjq.cn/Article/details/glaervlkp.sHtML

[Q88] 行转列（条件聚合）
来源：http://baike.zdbjq.cn/Article/details/gwvyeuwkj.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://m.share.zdbjq.cn/Article/details/gtymhlwja.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gdyvmxghv.sHtML

[Q89] 判断表是否存在
来源：http://read.share.zdbjq.cn/Article/details/gugbhpgcv.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://baike.hesvh.cn/Article/details/gnfkpxkvw.sHtML

[Q90] 生成序号列
来源：http://3g.hesvh.cn/Article/details/gedysulfy.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.m.share.zdbjq.cn/Article/details/gocxpjvwi.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gyqediwvf.sHtML

R. Bash 专题
来源：http://www.share.fehbvm.com/Article/details/glmhaqvmr.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/ghdsalgmu.sHtML

[R01] shebang 与严格模式
来源：http://www.blog.fehbvm.com/Article/details/gmtfjfana.sHtML

#!/usr/bin/env bash
来源：http://3g.zdbjq.cn/Article/details/gkjzswzum.sHtML

set -euo pipefail
来源：http://www.share.fehbvm.com/Article/details/gxgrnbubr.sHtML

[R02] 变量赋值与使用
来源：http://blog.hesvh.cn/Article/details/gzpgumwmj.sHtML

name="Tom"; echo "$name"
来源：http://read.share.fehbvm.com/Article/details/gdjjvbpvv.sHtML

[R03] 只读变量
来源：http://baike.zdbjq.cn/Article/details/geolvcjkp.sHtML

readonly PI=3.14
来源：http://baike.zdbjq.cn/Article/details/grlvdsnys.sHtML

[R04] 位置参数
来源：http://wap.fehbvm.com/Article/details/gjjcueehs.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://baike.fehbvm.com/Article/details/gdfgyzbxu.sHtML

[R05] 参数默认值
来源：http://www.blog.zdbjq.cn/Article/details/gwodmbssp.sHtML

name="${1:-default}"
来源：http://wap.zdbjq.cn/Article/details/gqphlttdd.sHtML

[R06] 判断命令是否存在
来源：http://www.blog.fehbvm.com/Article/details/gdkwudrkf.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://read.share.fehbvm.com/Article/details/gkgbzfjrv.sHtML

[R07] if 判断文件
来源：http://www.m.share.hesvh.cn/Article/details/glrgnucza.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.share.hesvh.cn/Article/details/gpkdhqsqs.sHtML

[R08] 数值比较
来源：http://www.share.hesvh.cn/Article/details/gxrxvvqko.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://3g.zdbjq.cn/Article/details/gkkygkzss.sHtML

[R09] 字符串比较
来源：http://read.share.hesvh.cn/Article/details/gchnsvohj.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://blog.zdbjq.cn/Article/details/gbkpfamyt.sHtML

[R10] 正则匹配
来源：http://mobile.fehbvm.com/Article/details/gbqaptdhn.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.share.zdbjq.cn/Article/details/gkhhmhkku.sHtML

[R11] case 多分支
来源：http://3g.fehbvm.com/Article/details/gxjeujnlk.sHtML

case "$1" in
来源：http://wap.zdbjq.cn/Article/details/grsasxkik.sHtML

start) echo "启动" ;;
来源：http://wap.zdbjq.cn/Article/details/gyolyiedp.sHtML

stop)  echo "停止" ;;
来源：http://mobile.hesvh.cn/Article/details/gvkdoqacz.sHtML

*)     echo "未知命令" ;;
来源：http://mobile.fehbvm.com/Article/details/goacrdcdz.sHtML

esac
来源：http://m.share.zdbjq.cn/Article/details/gjzpfheen.sHtML

[R12] for 遍历文件
来源：http://read.share.fehbvm.com/Article/details/gcyybfyhc.sHtML

for f in *.txt; do echo "$f"; done
来源：http://mobile.fehbvm.com/Article/details/gkkmomcmt.sHtML

[R13] for 计数循环
来源：http://3g.fehbvm.com/Article/details/glthnxdra.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://blog.hesvh.cn/Article/details/gaodjvhoy.sHtML

[R14] C 风格 for
来源：http://www.blog.zdbjq.cn/Article/details/gvoafocpe.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://mobile.fehbvm.com/Article/details/govcbkbju.sHtML

[R15] while 逐行读文件
来源：http://m.share.hesvh.cn/Article/details/gzshcqvnx.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://m.share.zdbjq.cn/Article/details/gszrilziw.sHtML

[R16] until 等待条件
来源：http://read.share.fehbvm.com/Article/details/gttjdzsra.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://wap.fehbvm.com/Article/details/gfrkmiwho.sHtML

[R17] 数组定义与取值
来源：http://m.share.hesvh.cn/Article/details/gxvbxkfdv.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://baike.zdbjq.cn/Article/details/gsfwuysqo.sHtML

[R18] 遍历数组
来源：http://blog.hesvh.cn/Article/details/gndzjeoty.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://wap.fehbvm.com/Article/details/gaedxosfj.sHtML

[R19] 数组长度
来源：http://3g.fehbvm.com/Article/details/ghpiajiye.sHtML

echo "${#arr[@]}"
来源：http://read.share.fehbvm.com/Article/details/gdjssbted.sHtML

[R20] 关联数组（字典）
来源：http://www.share.zdbjq.cn/Article/details/gxsmkbalk.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://wap.zdbjq.cn/Article/details/grjyoxglh.sHtML

[R21] 字符串长度
来源：http://www.m.share.zdbjq.cn/Article/details/ggzbdolua.sHtML

echo "${#s}"
来源：http://wap.hesvh.cn/Article/details/gxgxhspjd.sHtML

[R22] 截取子串
来源：http://m.share.zdbjq.cn/Article/details/gzejsbrsg.sHtML

echo "${s:0:5}"
来源：http://www.m.share.zdbjq.cn/Article/details/gtcngujun.sHtML

[R23] 字符串替换
来源：http://www.share.zdbjq.cn/Article/details/ggpkgmwil.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.blog.hesvh.cn/Article/details/gnlvvxudi.sHtML

[R24] 大小写转换
来源：http://www.share.zdbjq.cn/Article/details/gfbilcwfg.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.blog.fehbvm.com/Article/details/gltuxwhtp.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.m.share.zdbjq.cn/Article/details/grgdaqtrt.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://m.share.zdbjq.cn/Article/details/gtkxsyrqf.sHtML

[R26] 命令替换
来源：http://mobile.zdbjq.cn/Article/details/gclulfvaw.sHtML

now=$(date +%F); echo "$now"
来源：http://www.blog.hesvh.cn/Article/details/gikidedvb.sHtML

[R27] 算术展开
来源：http://www.blog.zdbjq.cn/Article/details/gwuararpa.sHtML

echo $((1 + 2 * 3))
来源：http://3g.fehbvm.com/Article/details/gbegtdydj.sHtML

[R28] 浮点运算
来源：http://www.blog.fehbvm.com/Article/details/gjmnzeare.sHtML

echo "scale=2; 10/3" | bc
来源：http://mobile.hesvh.cn/Article/details/gjmsrcgiz.sHtML

[R29] 定义函数
来源：http://3g.hesvh.cn/Article/details/gpqjhoejr.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://m.share.hesvh.cn/Article/details/giyyckqaf.sHtML

[R30] 函数返回状态码
来源：http://3g.zdbjq.cn/Article/details/gfezwphip.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://blog.hesvh.cn/Article/details/gfygvobmu.sHtML

[R31] 局部变量
来源：http://www.m.share.hesvh.cn/Article/details/gwpjwzdyt.sHtML

f() { local x=1; echo "$x"; }
来源：http://wap.hesvh.cn/Article/details/ghltiujkt.sHtML

[R32] 参数个数校验
来源：http://www.blog.hesvh.cn/Article/details/gpahouzoj.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://3g.hesvh.cn/Article/details/guggxgftn.sHtML

[R33] 捕获错误并提示行号
来源：http://m.share.zdbjq.cn/Article/details/ghpmwzauj.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://read.share.hesvh.cn/Article/details/gfmomirxk.sHtML

[R34] 退出时清理
来源：http://m.share.zdbjq.cn/Article/details/gpnaugfob.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.share.fehbvm.com/Article/details/gygtxrtet.sHtML

[R35] 后台执行并等待
来源：http://blog.zdbjq.cn/Article/details/gzrdrkyiy.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://3g.fehbvm.com/Article/details/gasjycodp.sHtML

[R36] 并发执行多个任务
来源：http://mobile.zdbjq.cn/Article/details/gsobkbxwo.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://m.share.hesvh.cn/Article/details/gxugrbjrp.sHtML

[R37] 把输出赋给变量
来源：http://wap.fehbvm.com/Article/details/gltujieab.sHtML

files=$(ls -1)
来源：http://wap.zdbjq.cn/Article/details/gqnuaplcq.sHtML

[R38] 管道串联
来源：http://m.share.hesvh.cn/Article/details/gsdnvrxpt.sHtML

cat a.txt | grep -i error | wc -l
来源：http://wap.fehbvm.com/Article/details/gutdcbbyg.sHtML

[R39] 重定向标准输出与错误
来源：http://m.share.zdbjq.cn/Article/details/gnpftxpyc.sHtML

cmd > out.log 2>&1
来源：http://wap.hesvh.cn/Article/details/gahzoetzs.sHtML

[R40] 追加写日志
来源：http://www.m.share.zdbjq.cn/Article/details/glxkwhjnk.sHtML

echo "log" >> out.log
来源：http://m.share.hesvh.cn/Article/details/gtihhzzyk.sHtML

[R41] 丢弃输出
来源：http://wap.fehbvm.com/Article/details/ggxdjluhl.sHtML

cmd >/dev/null 2>&1
来源：http://read.share.zdbjq.cn/Article/details/gewddlkdx.sHtML

[R42] 输入重定向
来源：http://wap.hesvh.cn/Article/details/gtfjqvxzc.sHtML

wc -l < a.txt
来源：http://mobile.zdbjq.cn/Article/details/gqzvbpgiz.sHtML

[R43] 按名字查找文件
来源：http://blog.hesvh.cn/Article/details/gsqvamxwb.sHtML


<!-- 参考信息 -->