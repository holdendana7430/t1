代发 wailian999

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.share.fehbvm.com/Article/details/golxjylnj.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://mobile.hesvh.cn/Article/details/gctiftqpu.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://wap.hesvh.cn/Article/details/geubjecoq.sHtML

[P08] 处理浮点精度问题
来源：http://mobile.zdbjq.cn/Article/details/goyyifhaq.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://3g.fehbvm.com/Article/details/ghgwnqcds.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://baike.zdbjq.cn/Article/details/grvhxscvx.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://baike.zdbjq.cn/Article/details/gtmxapjdv.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.share.zdbjq.cn/Article/details/gwxpyrblu.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://baike.hesvh.cn/Article/details/gjzvujubu.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://3g.zdbjq.cn/Article/details/gytlzuuzh.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://3g.hesvh.cn/Article/details/ggcviaznx.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://blog.fehbvm.com/Article/details/gmusfefhx.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gysclzlhk.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://m.share.fehbvm.com/Article/details/giuylgufi.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gyayzzvgi.sHtML

[Q01] 创建表
来源：http://m.share.fehbvm.com/Article/details/gjhlkoqef.sHtML

CREATE TABLE users (
来源：http://mobile.hesvh.cn/Article/details/gnkycjesq.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.zdbjq.cn/Article/details/gyqiovwuo.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.m.share.hesvh.cn/Article/details/gcyehlyey.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.share.hesvh.cn/Article/details/gclpmvxki.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.m.share.hesvh.cn/Article/details/gzwpxrhav.sHtML

);
来源：http://blog.zdbjq.cn/Article/details/gbtgqapvn.sHtML

[Q02] 创建带外键的表
来源：http://wap.zdbjq.cn/Article/details/gbocjxjsw.sHtML

CREATE TABLE orders (
来源：http://blog.zdbjq.cn/Article/details/gesnhbqio.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.zdbjq.cn/Article/details/gerphakty.sHtML

user_id INT NOT NULL,
来源：http://www.blog.fehbvm.com/Article/details/gxdfvuxei.sHtML

amount DECIMAL(10, 2),
来源：http://baike.hesvh.cn/Article/details/gsutbzmie.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://read.share.fehbvm.com/Article/details/glrpcwwri.sHtML

);
来源：http://blog.zdbjq.cn/Article/details/ghhmuiwyy.sHtML

[Q03] 增加列
来源：http://baike.zdbjq.cn/Article/details/gkzstvpcu.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.m.share.hesvh.cn/Article/details/gkhoggcwy.sHtML

[Q04] 修改列类型
来源：http://read.share.zdbjq.cn/Article/details/gqwxetjkq.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://wap.zdbjq.cn/Article/details/gwfjnsomj.sHtML

[Q05] 重命名列
来源：http://www.share.hesvh.cn/Article/details/gvjahkauo.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://m.share.hesvh.cn/Article/details/gjoejbzti.sHtML

[Q06] 删除列
来源：http://www.m.share.zdbjq.cn/Article/details/gauxbllix.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.share.hesvh.cn/Article/details/gylrqhqoy.sHtML

[Q07] 删除表
来源：http://wap.fehbvm.com/Article/details/gsnsrsigh.sHtML

DROP TABLE IF EXISTS orders;
来源：http://baike.hesvh.cn/Article/details/gosynhwki.sHtML

[Q08] 创建普通索引
来源：http://mobile.fehbvm.com/Article/details/gulatoiwi.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.m.share.zdbjq.cn/Article/details/gvhgdumlf.sHtML

[Q09] 创建唯一索引
来源：http://3g.fehbvm.com/Article/details/gslqfxmgj.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.share.fehbvm.com/Article/details/gyttasxmy.sHtML

[Q10] 插入单行
来源：http://www.m.share.fehbvm.com/Article/details/glzvswfyh.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.share.fehbvm.com/Article/details/gnuxjujdx.sHtML

[Q11] 一次插入多行
来源：http://read.share.fehbvm.com/Article/details/gguqprhng.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://m.share.hesvh.cn/Article/details/gqyyxutcm.sHtML

[Q12] 插入后取自增 ID
来源：http://wap.fehbvm.com/Article/details/gijigxnjb.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.blog.hesvh.cn/Article/details/geifesfyn.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.blog.zdbjq.cn/Article/details/gxlwahnmf.sHtML

[Q13] 忽略重复插入
来源：http://www.share.hesvh.cn/Article/details/gcdyolewo.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://baike.hesvh.cn/Article/details/gazduirjd.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.blog.zdbjq.cn/Article/details/gjdpanjvj.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.share.hesvh.cn/Article/details/gzgoyzzpz.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://read.share.zdbjq.cn/Article/details/gyhkxtyef.sHtML

[Q15] 查询全部
来源：http://www.share.zdbjq.cn/Article/details/gzthicvtr.sHtML

SELECT * FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gsawisccv.sHtML

[Q16] 查询指定列
来源：http://www.blog.fehbvm.com/Article/details/gbwdnrzxk.sHtML

SELECT id, name FROM users;
来源：http://baike.zdbjq.cn/Article/details/gvzqqsjix.sHtML

[Q17] 条件查询
来源：http://blog.zdbjq.cn/Article/details/ghmojrszr.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://read.share.zdbjq.cn/Article/details/girqasygp.sHtML

[Q18] 模糊匹配
来源：http://blog.zdbjq.cn/Article/details/gssgojwzn.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.share.fehbvm.com/Article/details/gscfdlgsi.sHtML

[Q19] 范围查询
来源：http://baike.zdbjq.cn/Article/details/gvojwgmge.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.blog.zdbjq.cn/Article/details/ggkxzsmcg.sHtML

[Q20] IN 列表
来源：http://mobile.hesvh.cn/Article/details/gcuasjtmv.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.share.fehbvm.com/Article/details/gkneegmxw.sHtML

[Q21] 空值判断
来源：http://mobile.hesvh.cn/Article/details/glbxpwugv.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.share.hesvh.cn/Article/details/gltfgewlz.sHtML

[Q22] 排序
来源：http://3g.hesvh.cn/Article/details/gloqzpsrd.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.m.share.hesvh.cn/Article/details/gvinnlzbx.sHtML

[Q23] 分页
来源：http://wap.zdbjq.cn/Article/details/gbvhmjjif.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://blog.fehbvm.com/Article/details/gyjlmhudl.sHtML

[Q24] 去重
来源：http://read.share.hesvh.cn/Article/details/guhgediyh.sHtML

SELECT DISTINCT city FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gkglouwra.sHtML

[Q25] 只取前 N 条
来源：http://wap.fehbvm.com/Article/details/gmuswgueu.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://baike.fehbvm.com/Article/details/gyuxvzlig.sHtML

[Q26] 计数
来源：http://www.share.hesvh.cn/Article/details/gkvrnhlxm.sHtML

SELECT COUNT(*) FROM users;
来源：http://wap.fehbvm.com/Article/details/gskmzcpqc.sHtML

[Q27] 条件计数
来源：http://read.share.fehbvm.com/Article/details/gfyjfwqnr.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gtycnhvms.sHtML

[Q28] 求和与平均
来源：http://read.share.hesvh.cn/Article/details/geuetufwq.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.share.fehbvm.com/Article/details/gjlmqjelx.sHtML

[Q29] 最大最小值
来源：http://www.share.zdbjq.cn/Article/details/gvvdgfcbr.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://baike.zdbjq.cn/Article/details/gudpbepfp.sHtML

[Q30] 分组统计
来源：http://www.share.zdbjq.cn/Article/details/gpoowqucf.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://blog.fehbvm.com/Article/details/gxnyrqmqe.sHtML

[Q31] 分组后过滤
来源：http://mobile.hesvh.cn/Article/details/gjgfgjmuf.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://m.share.hesvh.cn/Article/details/ginpwtctl.sHtML

[Q32] 分组拼接字符串
来源：http://wap.fehbvm.com/Article/details/giuqhesfk.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://read.share.fehbvm.com/Article/details/gmhufnmhw.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://m.share.hesvh.cn/Article/details/gzaeretrm.sHtML

[Q33] 多列分组
来源：http://www.blog.fehbvm.com/Article/details/geefonpbo.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://m.share.zdbjq.cn/Article/details/gryeommcp.sHtML

[Q34] 每组取第一条
来源：http://www.m.share.fehbvm.com/Article/details/gcddqhtlj.sHtML

SELECT * FROM (
来源：http://www.m.share.hesvh.cn/Article/details/gkxnzekoz.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://wap.fehbvm.com/Article/details/gksydpzwl.sHtML

) t WHERE rn = 1;
来源：http://www.share.fehbvm.com/Article/details/gehwjdffs.sHtML

[Q35] 内连接
来源：http://www.blog.fehbvm.com/Article/details/grmgomjxv.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.zdbjq.cn/Article/details/gvlxgjrau.sHtML

[Q36] 左连接
来源：http://www.m.share.fehbvm.com/Article/details/ggsbmvfox.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.fehbvm.com/Article/details/gqwuevghn.sHtML

[Q37] 右连接
来源：http://www.blog.fehbvm.com/Article/details/gnjkdjyhn.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://3g.fehbvm.com/Article/details/ggvcwnqlm.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://baike.fehbvm.com/Article/details/gmfhyreyp.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://baike.zdbjq.cn/Article/details/gksbpoqbz.sHtML

[Q39] 自连接（查上下级）
来源：http://mobile.hesvh.cn/Article/details/gsfwoqgry.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://read.share.zdbjq.cn/Article/details/gqpncqkzx.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.m.share.hesvh.cn/Article/details/gcuegfvac.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://read.share.hesvh.cn/Article/details/gvjmuakro.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://baike.fehbvm.com/Article/details/gwkueeypv.sHtML

[Q41] 多表连接
来源：http://m.share.fehbvm.com/Article/details/gwqnxbial.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://blog.hesvh.cn/Article/details/ghrcvwboy.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.share.fehbvm.com/Article/details/gtnvuqivz.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://m.share.hesvh.cn/Article/details/guvcpcwmk.sHtML

[Q42] 连接条件附加过滤
来源：http://3g.hesvh.cn/Article/details/gicxxsrqe.sHtML

SELECT u.name, o.amount FROM users u
来源：http://read.share.fehbvm.com/Article/details/gewluotij.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://mobile.hesvh.cn/Article/details/gypmdwgnh.sHtML

[Q43] 标量子查询
来源：http://www.share.zdbjq.cn/Article/details/gvdzvybcq.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://read.share.zdbjq.cn/Article/details/gqpmewmls.sHtML

[Q44] IN 子查询
来源：http://www.share.hesvh.cn/Article/details/gvnhrsbsm.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://3g.zdbjq.cn/Article/details/gurasshmi.sHtML

[Q45] EXISTS 判断存在
来源：http://read.share.zdbjq.cn/Article/details/gbbjbmgjf.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.fehbvm.com/Article/details/glohtqbnq.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://3g.hesvh.cn/Article/details/glbobqwlx.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.hesvh.cn/Article/details/gzdsekoxp.sHtML

[Q47] 与平均值比较
来源：http://blog.zdbjq.cn/Article/details/gimcdmwnx.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://m.share.zdbjq.cn/Article/details/gqhbgfysl.sHtML

[Q48] CTE 公用表表达式
来源：http://3g.zdbjq.cn/Article/details/gwinmupoh.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://wap.hesvh.cn/Article/details/glkmzllxc.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://m.share.fehbvm.com/Article/details/gykukhveu.sHtML

[Q49] 更新单行
来源：http://3g.fehbvm.com/Article/details/gzvequfpb.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://m.share.fehbvm.com/Article/details/gmwtpulco.sHtML

[Q50] 批量更新
来源：http://www.blog.hesvh.cn/Article/details/gycoicsvb.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.share.fehbvm.com/Article/details/gsmjorrdo.sHtML

[Q51] 用子查询更新
来源：http://www.m.share.zdbjq.cn/Article/details/gqigbawfn.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://read.share.zdbjq.cn/Article/details/gqhkrdozz.sHtML

[Q52] 删除指定行
来源：http://read.share.fehbvm.com/Article/details/gmgfcwevz.sHtML

DELETE FROM users WHERE id = 10;
来源：http://mobile.fehbvm.com/Article/details/gxcjvrlvo.sHtML

[Q53] 按条件删除
来源：http://mobile.zdbjq.cn/Article/details/gdsqbwywu.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://wap.hesvh.cn/Article/details/gjvetdcvd.sHtML

[Q54] 清空表
来源：http://3g.zdbjq.cn/Article/details/gngssqmoq.sHtML

TRUNCATE TABLE logs;
来源：http://mobile.fehbvm.com/Article/details/gtzdcxakv.sHtML

[Q55] 排名（并列占位）
来源：http://www.share.zdbjq.cn/Article/details/gqammualu.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://read.share.zdbjq.cn/Article/details/gxlltgnbo.sHtML

[Q56] 密集排名（并列不占位）
来源：http://wap.fehbvm.com/Article/details/glejgytic.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.share.zdbjq.cn/Article/details/gasyfdgcp.sHtML

[Q57] 行号
来源：http://www.share.fehbvm.com/Article/details/glqhyzibp.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gzrzxsovy.sHtML

[Q58] 累计求和
来源：http://www.blog.fehbvm.com/Article/details/gyckwvhde.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://baike.zdbjq.cn/Article/details/gooycfwme.sHtML

[Q59] 分组内累计
来源：http://www.m.share.hesvh.cn/Article/details/gcopjurvx.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://3g.fehbvm.com/Article/details/gmqklpxxe.sHtML

[Q60] 取上一行 / 下一行
来源：http://wap.fehbvm.com/Article/details/gxyiikndf.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://m.share.fehbvm.com/Article/details/gzivkfqes.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://m.share.fehbvm.com/Article/details/gywbbadkd.sHtML

[Q61] 移动平均
来源：http://mobile.zdbjq.cn/Article/details/ghhjuqlfc.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://mobile.fehbvm.com/Article/details/gnqelxohy.sHtML

[Q62] 分组占比
来源：http://www.share.hesvh.cn/Article/details/gxocadpos.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://wap.fehbvm.com/Article/details/gnlrafier.sHtML

[Q63] 开启事务
来源：http://wap.fehbvm.com/Article/details/gcsioutsk.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://baike.zdbjq.cn/Article/details/gptcnzmwb.sHtML

[Q64] 提交事务
来源：http://read.share.zdbjq.cn/Article/details/gfkqnhblz.sHtML

COMMIT;
来源：http://3g.zdbjq.cn/Article/details/gynqsjfge.sHtML

[Q65] 回滚事务
来源：http://www.m.share.zdbjq.cn/Article/details/gsnmzjwon.sHtML

ROLLBACK;
来源：http://m.share.fehbvm.com/Article/details/gxbhggufz.sHtML

[Q66] 行锁查询
来源：http://www.blog.fehbvm.com/Article/details/gtovaqfhv.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://baike.fehbvm.com/Article/details/gkklfyxar.sHtML

[Q67] 设置隔离级别
来源：http://blog.fehbvm.com/Article/details/gjqlzmvql.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://3g.hesvh.cn/Article/details/gonwfpyxq.sHtML

[Q68] 保存点
来源：http://wap.fehbvm.com/Article/details/gbtpvygup.sHtML

SAVEPOINT sp1;
来源：http://read.share.fehbvm.com/Article/details/gpoirijix.sHtML

ROLLBACK TO sp1;
来源：http://baike.hesvh.cn/Article/details/giooowgbg.sHtML

[Q69] 查看执行计划
来源：http://wap.fehbvm.com/Article/details/gkrrqoqhg.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://baike.hesvh.cn/Article/details/gkqdgajde.sHtML

[Q70] 更新统计信息
来源：http://read.share.fehbvm.com/Article/details/gcvwyrpis.sHtML

ANALYZE TABLE users;
来源：http://baike.hesvh.cn/Article/details/gmgqibswb.sHtML

[Q71] 查看建表语句
来源：http://read.share.zdbjq.cn/Article/details/gjjrkevro.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://baike.fehbvm.com/Article/details/gmrvjlbok.sHtML

[Q72] 查看索引
来源：http://blog.fehbvm.com/Article/details/grkodzngy.sHtML

SHOW INDEX FROM users;
来源：http://wap.zdbjq.cn/Article/details/gtoobkvic.sHtML

[Q73] 查看表状态
来源：http://www.blog.hesvh.cn/Article/details/gnoeqwzrg.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://mobile.fehbvm.com/Article/details/gcbxqfibc.sHtML

[Q74] 强制使用索引
来源：http://mobile.fehbvm.com/Article/details/givokdvye.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://m.share.hesvh.cn/Article/details/gcxjzyvbq.sHtML

[Q75] 日期格式化
来源：http://www.share.zdbjq.cn/Article/details/gsheaadpi.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://mobile.zdbjq.cn/Article/details/gqejetktw.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://mobile.hesvh.cn/Article/details/ghbercdit.sHtML

[Q76] 按天统计
来源：http://baike.zdbjq.cn/Article/details/goomucvct.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://read.share.zdbjq.cn/Article/details/gfewfvrmn.sHtML

[Q77] 时间加减
来源：http://www.blog.zdbjq.cn/Article/details/gxhqszzcb.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://3g.hesvh.cn/Article/details/gshrnblww.sHtML

[Q78] 当前时间
来源：http://mobile.hesvh.cn/Article/details/grgydfvfq.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://mobile.fehbvm.com/Article/details/gjivvsdxj.sHtML

[Q79] 字符串拼接
来源：http://3g.fehbvm.com/Article/details/gzjelhrgc.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://read.share.hesvh.cn/Article/details/gdfwpnnzq.sHtML

[Q80] 字符串截取
来源：http://m.share.zdbjq.cn/Article/details/goalanset.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://read.share.hesvh.cn/Article/details/gzabtykqa.sHtML

[Q81] 字符串替换
来源：http://mobile.hesvh.cn/Article/details/gatzhoudb.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://baike.hesvh.cn/Article/details/gowzbwtvr.sHtML

[Q82] 字符长度与字节长度
来源：http://mobile.fehbvm.com/Article/details/gnebeifzj.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://mobile.hesvh.cn/Article/details/gymnhsipp.sHtML

[Q83] 大小写转换
来源：http://blog.zdbjq.cn/Article/details/gsosbpoth.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://blog.hesvh.cn/Article/details/grwndzgfg.sHtML

[Q84] 去除首尾空格
来源：http://www.m.share.hesvh.cn/Article/details/girgrwudi.sHtML

SELECT TRIM(name) FROM users;
来源：http://baike.fehbvm.com/Article/details/gpadbxttv.sHtML

[Q85] 数值取整
来源：http://m.share.hesvh.cn/Article/details/goqhyrngc.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://mobile.fehbvm.com/Article/details/gnhzbvmlg.sHtML

[Q86] 读取 JSON 字段
来源：http://baike.zdbjq.cn/Article/details/gqlvulhem.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.share.hesvh.cn/Article/details/gxpuefjhh.sHtML

[Q87] JSON 字段做条件
来源：http://m.share.zdbjq.cn/Article/details/gderpyjhl.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://3g.hesvh.cn/Article/details/gtszjdtcm.sHtML

[Q88] 行转列（条件聚合）
来源：http://baike.fehbvm.com/Article/details/gptgzlcjg.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://wap.zdbjq.cn/Article/details/gpqjybkrq.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.share.fehbvm.com/Article/details/goivjrjsx.sHtML

[Q89] 判断表是否存在
来源：http://baike.zdbjq.cn/Article/details/goejbjaoy.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://blog.fehbvm.com/Article/details/gufrhlkrs.sHtML

[Q90] 生成序号列
来源：http://blog.fehbvm.com/Article/details/gewlzwfzd.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://baike.zdbjq.cn/Article/details/gbqbdyikt.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gkhiwaqmg.sHtML

R. Bash 专题
来源：http://blog.zdbjq.cn/Article/details/gzwnwzctw.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gapawhejo.sHtML

[R01] shebang 与严格模式
来源：http://www.blog.zdbjq.cn/Article/details/gegawuyqy.sHtML

#!/usr/bin/env bash
来源：http://www.blog.hesvh.cn/Article/details/gqotsakze.sHtML

set -euo pipefail
来源：http://blog.hesvh.cn/Article/details/gdyfwqgaz.sHtML

[R02] 变量赋值与使用
来源：http://baike.hesvh.cn/Article/details/gjzvxybax.sHtML

name="Tom"; echo "$name"
来源：http://blog.fehbvm.com/Article/details/gbkehzipu.sHtML

[R03] 只读变量
来源：http://baike.hesvh.cn/Article/details/grcubvhzq.sHtML

readonly PI=3.14
来源：http://baike.zdbjq.cn/Article/details/ggfvrllwh.sHtML

[R04] 位置参数
来源：http://m.share.hesvh.cn/Article/details/gizgovytr.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://mobile.fehbvm.com/Article/details/gkumovvmy.sHtML

[R05] 参数默认值
来源：http://baike.hesvh.cn/Article/details/ghmnjisbq.sHtML

name="${1:-default}"
来源：http://www.share.fehbvm.com/Article/details/gxnwykisn.sHtML

[R06] 判断命令是否存在
来源：http://www.blog.zdbjq.cn/Article/details/gqoufelxi.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://3g.zdbjq.cn/Article/details/gllnxynsp.sHtML

[R07] if 判断文件
来源：http://baike.hesvh.cn/Article/details/guskfqpha.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://blog.zdbjq.cn/Article/details/gpcxhhepm.sHtML

[R08] 数值比较
来源：http://www.share.fehbvm.com/Article/details/ggnkzfxve.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.m.share.hesvh.cn/Article/details/gzwxghgyv.sHtML

[R09] 字符串比较
来源：http://3g.fehbvm.com/Article/details/gzarblwzd.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://mobile.fehbvm.com/Article/details/gnamzwjns.sHtML

[R10] 正则匹配
来源：http://www.blog.fehbvm.com/Article/details/gdcuzgweb.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://mobile.fehbvm.com/Article/details/goznnbsus.sHtML

[R11] case 多分支
来源：http://www.blog.fehbvm.com/Article/details/gadjkcrxl.sHtML

case "$1" in
来源：http://blog.hesvh.cn/Article/details/gpgxqiwac.sHtML

start) echo "启动" ;;
来源：http://blog.zdbjq.cn/Article/details/gljzvqrbi.sHtML

stop)  echo "停止" ;;
来源：http://wap.hesvh.cn/Article/details/gfbdfryew.sHtML

*)     echo "未知命令" ;;
来源：http://m.share.hesvh.cn/Article/details/geqkrcreq.sHtML

esac
来源：http://blog.zdbjq.cn/Article/details/gkdeylnbs.sHtML

[R12] for 遍历文件
来源：http://3g.hesvh.cn/Article/details/gawoijqnk.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.blog.fehbvm.com/Article/details/gnbdnrvlb.sHtML

[R13] for 计数循环
来源：http://www.share.hesvh.cn/Article/details/gqgltgsom.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.blog.fehbvm.com/Article/details/glslunbez.sHtML

[R14] C 风格 for
来源：http://read.share.hesvh.cn/Article/details/ghcxpmuzv.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://wap.hesvh.cn/Article/details/gudyfbyak.sHtML

[R15] while 逐行读文件
来源：http://mobile.hesvh.cn/Article/details/gaahvurxu.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://wap.hesvh.cn/Article/details/gsccybwue.sHtML

[R16] until 等待条件
来源：http://m.share.fehbvm.com/Article/details/gajbplarv.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://wap.fehbvm.com/Article/details/gwmaasvqz.sHtML

[R17] 数组定义与取值
来源：http://blog.zdbjq.cn/Article/details/gtqvdupra.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.share.zdbjq.cn/Article/details/giwikbpkj.sHtML

[R18] 遍历数组
来源：http://baike.zdbjq.cn/Article/details/gldugwarg.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://mobile.fehbvm.com/Article/details/gmhkqfnjg.sHtML

[R19] 数组长度
来源：http://www.m.share.zdbjq.cn/Article/details/gappvewnh.sHtML

echo "${#arr[@]}"
来源：http://baike.zdbjq.cn/Article/details/gcbuqhauy.sHtML

[R20] 关联数组（字典）
来源：http://3g.fehbvm.com/Article/details/ghnfyljes.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://3g.fehbvm.com/Article/details/gzidxlazt.sHtML

[R21] 字符串长度
来源：http://www.m.share.zdbjq.cn/Article/details/grrlfkpoj.sHtML

echo "${#s}"
来源：http://mobile.zdbjq.cn/Article/details/gdlprzcjz.sHtML

[R22] 截取子串
来源：http://wap.fehbvm.com/Article/details/gpwvomaqp.sHtML

echo "${s:0:5}"
来源：http://www.m.share.hesvh.cn/Article/details/gswhskvau.sHtML

[R23] 字符串替换
来源：http://mobile.zdbjq.cn/Article/details/gnntxotte.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://baike.zdbjq.cn/Article/details/gofptnqtk.sHtML

[R24] 大小写转换
来源：http://www.blog.hesvh.cn/Article/details/gvxssanwi.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://read.share.zdbjq.cn/Article/details/gpnardzkh.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.blog.zdbjq.cn/Article/details/gyyilqlqz.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.blog.fehbvm.com/Article/details/gsrmnlidz.sHtML

[R26] 命令替换
来源：http://3g.hesvh.cn/Article/details/gxnklugeg.sHtML

now=$(date +%F); echo "$now"
来源：http://m.share.zdbjq.cn/Article/details/gnizklace.sHtML

[R27] 算术展开
来源：http://www.blog.zdbjq.cn/Article/details/gwapqpnei.sHtML

echo $((1 + 2 * 3))
来源：http://wap.fehbvm.com/Article/details/gltmsqxam.sHtML

[R28] 浮点运算
来源：http://www.share.fehbvm.com/Article/details/gjnberjiw.sHtML

echo "scale=2; 10/3" | bc
来源：http://blog.hesvh.cn/Article/details/gtfoxrqga.sHtML

[R29] 定义函数
来源：http://www.share.hesvh.cn/Article/details/gokrjwvif.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://m.share.hesvh.cn/Article/details/grkbahxxm.sHtML

[R30] 函数返回状态码
来源：http://www.share.fehbvm.com/Article/details/gwetyutfq.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://3g.zdbjq.cn/Article/details/gmvvrjfco.sHtML

[R31] 局部变量
来源：http://3g.fehbvm.com/Article/details/gnjlglqxj.sHtML

f() { local x=1; echo "$x"; }
来源：http://read.share.zdbjq.cn/Article/details/gfubrjfqv.sHtML

[R32] 参数个数校验
来源：http://baike.zdbjq.cn/Article/details/gmlylnyqz.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://mobile.zdbjq.cn/Article/details/guepmoqoz.sHtML

[R33] 捕获错误并提示行号
来源：http://read.share.hesvh.cn/Article/details/gggygcryr.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://read.share.fehbvm.com/Article/details/gztauiywe.sHtML

[R34] 退出时清理
来源：http://read.share.zdbjq.cn/Article/details/gfqcxbzpc.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://m.share.fehbvm.com/Article/details/gkqqurxrs.sHtML

[R35] 后台执行并等待
来源：http://3g.hesvh.cn/Article/details/gactnlvsp.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.blog.zdbjq.cn/Article/details/gfyifenpo.sHtML

[R36] 并发执行多个任务
来源：http://blog.zdbjq.cn/Article/details/ghwxjdanv.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://blog.hesvh.cn/Article/details/gwfhjdqzn.sHtML

[R37] 把输出赋给变量
来源：http://m.share.fehbvm.com/Article/details/gmmtzsenc.sHtML


<!-- 参考信息 -->