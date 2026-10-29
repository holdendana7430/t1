代发 wailian999

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.blog.hesvh.cn/Article/details/gaaqtwfxc.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://m.share.hesvh.cn/Article/details/gdoovunyx.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://wap.zdbjq.cn/Article/details/gpizogxit.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.share.hesvh.cn/Article/details/gtftwhtei.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/glddkzemp.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://read.share.hesvh.cn/Article/details/gpiqzflgj.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gjouezbcp.sHtML

[Q01] 创建表
来源：http://m.share.zdbjq.cn/Article/details/gdqhqmrks.sHtML

CREATE TABLE users (
来源：http://www.m.share.hesvh.cn/Article/details/gqcxbeqzz.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.zdbjq.cn/Article/details/gfuqpzfob.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.share.hesvh.cn/Article/details/gtkgxywbf.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.share.zdbjq.cn/Article/details/guhyodcbh.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://3g.hesvh.cn/Article/details/gayagcusd.sHtML

);
来源：http://baike.zdbjq.cn/Article/details/gljakrtar.sHtML

[Q02] 创建带外键的表
来源：http://www.blog.hesvh.cn/Article/details/garkbxjjs.sHtML

CREATE TABLE orders (
来源：http://baike.hesvh.cn/Article/details/gxwfhkpce.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://mobile.fehbvm.com/Article/details/ghxmmlwpr.sHtML

user_id INT NOT NULL,
来源：http://3g.hesvh.cn/Article/details/guuejqrgc.sHtML

amount DECIMAL(10, 2),
来源：http://mobile.hesvh.cn/Article/details/gvnrtohov.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://3g.fehbvm.com/Article/details/ggeyznatx.sHtML

);
来源：http://www.share.zdbjq.cn/Article/details/gcpcqfdlm.sHtML

[Q03] 增加列
来源：http://m.share.hesvh.cn/Article/details/gljadbdgf.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://m.share.hesvh.cn/Article/details/ghebghuuz.sHtML

[Q04] 修改列类型
来源：http://m.share.hesvh.cn/Article/details/gbvmcxabs.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://mobile.hesvh.cn/Article/details/glxmztypw.sHtML

[Q05] 重命名列
来源：http://baike.hesvh.cn/Article/details/gremhbakz.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://blog.zdbjq.cn/Article/details/gjsowqfrs.sHtML

[Q06] 删除列
来源：http://read.share.hesvh.cn/Article/details/gmoykumyx.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://baike.hesvh.cn/Article/details/gbwxfzjzh.sHtML

[Q07] 删除表
来源：http://baike.zdbjq.cn/Article/details/gkmkjqozg.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.m.share.fehbvm.com/Article/details/gblqntaad.sHtML

[Q08] 创建普通索引
来源：http://blog.hesvh.cn/Article/details/gpabeqfmd.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.blog.hesvh.cn/Article/details/gbcgsdkzv.sHtML

[Q09] 创建唯一索引
来源：http://mobile.hesvh.cn/Article/details/gkcsnbtme.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.share.fehbvm.com/Article/details/geytpoifr.sHtML

[Q10] 插入单行
来源：http://www.m.share.hesvh.cn/Article/details/gpzfhfdsq.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://m.share.fehbvm.com/Article/details/gvodtonti.sHtML

[Q11] 一次插入多行
来源：http://blog.zdbjq.cn/Article/details/ggsnmkimx.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://baike.zdbjq.cn/Article/details/gkvxjiqie.sHtML

[Q12] 插入后取自增 ID
来源：http://m.share.zdbjq.cn/Article/details/gdzpftjyv.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://m.share.zdbjq.cn/Article/details/ghtjjutmk.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://baike.zdbjq.cn/Article/details/gznfytyxw.sHtML

[Q13] 忽略重复插入
来源：http://3g.fehbvm.com/Article/details/gdnmbwyjb.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.share.hesvh.cn/Article/details/gklzjbpnn.sHtML

[Q14] 存在则更新（upsert）
来源：http://read.share.zdbjq.cn/Article/details/ghxsywooo.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://wap.fehbvm.com/Article/details/gjxaamasl.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.share.hesvh.cn/Article/details/gbwzupehg.sHtML

[Q15] 查询全部
来源：http://wap.hesvh.cn/Article/details/grvpjqnch.sHtML

SELECT * FROM users;
来源：http://read.share.fehbvm.com/Article/details/gpkjmwryd.sHtML

[Q16] 查询指定列
来源：http://www.blog.hesvh.cn/Article/details/gmomeefbd.sHtML

SELECT id, name FROM users;
来源：http://read.share.zdbjq.cn/Article/details/genotjcdd.sHtML

[Q17] 条件查询
来源：http://3g.hesvh.cn/Article/details/ggmjvvamb.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://baike.hesvh.cn/Article/details/gayeenqfj.sHtML

[Q18] 模糊匹配
来源：http://mobile.hesvh.cn/Article/details/gdtsfzymr.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://baike.hesvh.cn/Article/details/gkakgncmv.sHtML

[Q19] 范围查询
来源：http://www.m.share.fehbvm.com/Article/details/gckawluin.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.share.hesvh.cn/Article/details/gyjlqntbc.sHtML

[Q20] IN 列表
来源：http://www.blog.zdbjq.cn/Article/details/glgkoahyv.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.m.share.hesvh.cn/Article/details/grmryzadj.sHtML

[Q21] 空值判断
来源：http://3g.zdbjq.cn/Article/details/gmszfdsws.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://read.share.hesvh.cn/Article/details/gkacyaxjd.sHtML

[Q22] 排序
来源：http://wap.hesvh.cn/Article/details/gpjifnrjt.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.m.share.hesvh.cn/Article/details/guafdqami.sHtML

[Q23] 分页
来源：http://baike.hesvh.cn/Article/details/gkvdtnmqk.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://3g.zdbjq.cn/Article/details/gxuoznylr.sHtML

[Q24] 去重
来源：http://blog.fehbvm.com/Article/details/gvlgozvpk.sHtML

SELECT DISTINCT city FROM users;
来源：http://wap.fehbvm.com/Article/details/gxtzvxslm.sHtML

[Q25] 只取前 N 条
来源：http://baike.zdbjq.cn/Article/details/gzmktqlue.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.m.share.zdbjq.cn/Article/details/gdoplcsoc.sHtML

[Q26] 计数
来源：http://baike.hesvh.cn/Article/details/gdlomjjai.sHtML

SELECT COUNT(*) FROM users;
来源：http://3g.fehbvm.com/Article/details/gfaehlucd.sHtML

[Q27] 条件计数
来源：http://read.share.zdbjq.cn/Article/details/gdrzcmgmy.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gyugzapjs.sHtML

[Q28] 求和与平均
来源：http://m.share.hesvh.cn/Article/details/gcyocyyan.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://wap.hesvh.cn/Article/details/grirkxrty.sHtML

[Q29] 最大最小值
来源：http://wap.hesvh.cn/Article/details/goantbgwm.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://mobile.fehbvm.com/Article/details/givlxkieg.sHtML

[Q30] 分组统计
来源：http://wap.hesvh.cn/Article/details/gzwlzhbdp.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://baike.zdbjq.cn/Article/details/glfcwwdhq.sHtML

[Q31] 分组后过滤
来源：http://mobile.hesvh.cn/Article/details/grnaszqsi.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://read.share.zdbjq.cn/Article/details/gzusmoiio.sHtML

[Q32] 分组拼接字符串
来源：http://www.m.share.hesvh.cn/Article/details/ghlaldqip.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.blog.fehbvm.com/Article/details/gcofptayi.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://wap.fehbvm.com/Article/details/gnvomdnni.sHtML

[Q33] 多列分组
来源：http://read.share.fehbvm.com/Article/details/gsnvtyiih.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://mobile.fehbvm.com/Article/details/gygntswwh.sHtML

[Q34] 每组取第一条
来源：http://www.blog.hesvh.cn/Article/details/gxnueneub.sHtML

SELECT * FROM (
来源：http://www.blog.fehbvm.com/Article/details/gpcpolsfv.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://3g.fehbvm.com/Article/details/gyytxxcvw.sHtML

) t WHERE rn = 1;
来源：http://mobile.hesvh.cn/Article/details/gyvtotiwt.sHtML

[Q35] 内连接
来源：http://3g.hesvh.cn/Article/details/gegdlxfhk.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://3g.fehbvm.com/Article/details/gxsbicndd.sHtML

[Q36] 左连接
来源：http://wap.hesvh.cn/Article/details/gcjoahlmg.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://read.share.hesvh.cn/Article/details/gzgyscxmg.sHtML

[Q37] 右连接
来源：http://blog.zdbjq.cn/Article/details/gfkvisdjx.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://read.share.fehbvm.com/Article/details/gnyxwjtei.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://m.share.zdbjq.cn/Article/details/gpsrkblzg.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://m.share.fehbvm.com/Article/details/gklybwaoj.sHtML

[Q39] 自连接（查上下级）
来源：http://www.share.fehbvm.com/Article/details/glkcqtcgk.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://baike.fehbvm.com/Article/details/gcfwsjwyl.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.m.share.hesvh.cn/Article/details/guoikqzhk.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://wap.zdbjq.cn/Article/details/gqeqylgyx.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://3g.hesvh.cn/Article/details/gcuybqgbu.sHtML

[Q41] 多表连接
来源：http://m.share.fehbvm.com/Article/details/gnbjwzokp.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://mobile.hesvh.cn/Article/details/gdluoqyrl.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.m.share.zdbjq.cn/Article/details/gpkkebcyv.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.m.share.zdbjq.cn/Article/details/gyvwfqsvj.sHtML

[Q42] 连接条件附加过滤
来源：http://wap.hesvh.cn/Article/details/gnifhpepc.sHtML

SELECT u.name, o.amount FROM users u
来源：http://mobile.fehbvm.com/Article/details/gyfwkdtfs.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://baike.fehbvm.com/Article/details/gvjdobnir.sHtML

[Q43] 标量子查询
来源：http://www.m.share.zdbjq.cn/Article/details/gqjtrrifl.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.blog.fehbvm.com/Article/details/gqxlkyslg.sHtML

[Q44] IN 子查询
来源：http://wap.zdbjq.cn/Article/details/ghtfqeyhf.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://baike.hesvh.cn/Article/details/gtdmtdaom.sHtML

[Q45] EXISTS 判断存在
来源：http://www.blog.fehbvm.com/Article/details/gbarahhbs.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.hesvh.cn/Article/details/gsxpiwyjg.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.blog.fehbvm.com/Article/details/gafvqzekh.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.zdbjq.cn/Article/details/gfslwfbwo.sHtML

[Q47] 与平均值比较
来源：http://blog.fehbvm.com/Article/details/gopncpfdm.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://baike.hesvh.cn/Article/details/gibshoxnn.sHtML

[Q48] CTE 公用表表达式
来源：http://m.share.zdbjq.cn/Article/details/guuzyrccf.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://3g.fehbvm.com/Article/details/gnfidypog.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://m.share.fehbvm.com/Article/details/gyqgkguch.sHtML

[Q49] 更新单行
来源：http://www.share.hesvh.cn/Article/details/gptbmqyhl.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://mobile.hesvh.cn/Article/details/gaujqgbta.sHtML

[Q50] 批量更新
来源：http://wap.zdbjq.cn/Article/details/grwlvwkzv.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.m.share.hesvh.cn/Article/details/gwxqareks.sHtML

[Q51] 用子查询更新
来源：http://blog.fehbvm.com/Article/details/gduivikig.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://wap.hesvh.cn/Article/details/gccfxjjex.sHtML

[Q52] 删除指定行
来源：http://www.m.share.zdbjq.cn/Article/details/gyiffyomq.sHtML

DELETE FROM users WHERE id = 10;
来源：http://3g.zdbjq.cn/Article/details/gliimccll.sHtML

[Q53] 按条件删除
来源：http://m.share.fehbvm.com/Article/details/gbamsjcre.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.blog.fehbvm.com/Article/details/gihxmnmmt.sHtML

[Q54] 清空表
来源：http://wap.hesvh.cn/Article/details/ginpzovxw.sHtML

TRUNCATE TABLE logs;
来源：http://www.blog.fehbvm.com/Article/details/grucxolxd.sHtML

[Q55] 排名（并列占位）
来源：http://baike.hesvh.cn/Article/details/gxvhfnfju.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://wap.hesvh.cn/Article/details/gdbuxqfzu.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.blog.fehbvm.com/Article/details/glzvfebck.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://blog.fehbvm.com/Article/details/gjlemzguq.sHtML

[Q57] 行号
来源：http://www.blog.hesvh.cn/Article/details/gnzlwqtgc.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://3g.fehbvm.com/Article/details/gyihafybq.sHtML

[Q58] 累计求和
来源：http://www.m.share.hesvh.cn/Article/details/gucmwhfxj.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.share.hesvh.cn/Article/details/gjzibneco.sHtML

[Q59] 分组内累计
来源：http://www.blog.fehbvm.com/Article/details/gomgnydyf.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://m.share.zdbjq.cn/Article/details/gleljgqwc.sHtML

[Q60] 取上一行 / 下一行
来源：http://read.share.fehbvm.com/Article/details/glginfufx.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://blog.hesvh.cn/Article/details/gooctvwyn.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://3g.fehbvm.com/Article/details/gueenqibo.sHtML

[Q61] 移动平均
来源：http://www.blog.fehbvm.com/Article/details/gvdrqzkym.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.blog.hesvh.cn/Article/details/getybmdso.sHtML

[Q62] 分组占比
来源：http://3g.zdbjq.cn/Article/details/gzogbpvyn.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.m.share.hesvh.cn/Article/details/gawetqyuq.sHtML

[Q63] 开启事务
来源：http://read.share.zdbjq.cn/Article/details/gfirhbimb.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://read.share.zdbjq.cn/Article/details/gocnihcop.sHtML

[Q64] 提交事务
来源：http://www.m.share.zdbjq.cn/Article/details/gbuucxvgb.sHtML

COMMIT;
来源：http://baike.fehbvm.com/Article/details/gykaytwxe.sHtML

[Q65] 回滚事务
来源：http://wap.hesvh.cn/Article/details/gydldqzat.sHtML

ROLLBACK;
来源：http://3g.fehbvm.com/Article/details/gwuqklevl.sHtML

[Q66] 行锁查询
来源：http://m.share.fehbvm.com/Article/details/gipdhwcdl.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://m.share.hesvh.cn/Article/details/gzivbdwmy.sHtML

[Q67] 设置隔离级别
来源：http://3g.hesvh.cn/Article/details/givxnupkj.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://m.share.fehbvm.com/Article/details/gzijyruxj.sHtML

[Q68] 保存点
来源：http://www.blog.hesvh.cn/Article/details/ggmxaqvon.sHtML

SAVEPOINT sp1;
来源：http://www.blog.hesvh.cn/Article/details/grwcjvqhr.sHtML

ROLLBACK TO sp1;
来源：http://www.m.share.fehbvm.com/Article/details/gjvjsinqj.sHtML

[Q69] 查看执行计划
来源：http://read.share.fehbvm.com/Article/details/ghvepwikq.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.share.fehbvm.com/Article/details/gxkzlkenk.sHtML

[Q70] 更新统计信息
来源：http://mobile.hesvh.cn/Article/details/gnoswjkgz.sHtML

ANALYZE TABLE users;
来源：http://wap.zdbjq.cn/Article/details/gdbwlpokc.sHtML

[Q71] 查看建表语句
来源：http://baike.hesvh.cn/Article/details/geznnqgwz.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://wap.zdbjq.cn/Article/details/gcskiyrtm.sHtML

[Q72] 查看索引
来源：http://m.share.zdbjq.cn/Article/details/gczsewfkf.sHtML

SHOW INDEX FROM users;
来源：http://read.share.hesvh.cn/Article/details/gryyknhms.sHtML

[Q73] 查看表状态
来源：http://baike.zdbjq.cn/Article/details/guyozrlrk.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://m.share.fehbvm.com/Article/details/giilfsqlc.sHtML

[Q74] 强制使用索引
来源：http://3g.hesvh.cn/Article/details/gduvvgdvx.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://3g.fehbvm.com/Article/details/gozbjtejb.sHtML

[Q75] 日期格式化
来源：http://www.blog.hesvh.cn/Article/details/gfaakfzwy.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.blog.fehbvm.com/Article/details/gnzsdvfwn.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.blog.hesvh.cn/Article/details/gzkanitsn.sHtML

[Q76] 按天统计
来源：http://baike.fehbvm.com/Article/details/gkxjwkcaq.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.m.share.zdbjq.cn/Article/details/gqippjorl.sHtML

[Q77] 时间加减
来源：http://blog.fehbvm.com/Article/details/gyvdtijnf.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.share.fehbvm.com/Article/details/garlkexcy.sHtML

[Q78] 当前时间
来源：http://www.blog.hesvh.cn/Article/details/gmviatwdr.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://mobile.fehbvm.com/Article/details/gfdqarjeq.sHtML

[Q79] 字符串拼接
来源：http://m.share.hesvh.cn/Article/details/gatenrhkd.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.share.zdbjq.cn/Article/details/gdcyggpkz.sHtML

[Q80] 字符串截取
来源：http://www.m.share.hesvh.cn/Article/details/gsrhyhryz.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gnrjolgve.sHtML

[Q81] 字符串替换
来源：http://www.m.share.zdbjq.cn/Article/details/ghflwqejy.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://mobile.hesvh.cn/Article/details/gbxwatoih.sHtML

[Q82] 字符长度与字节长度
来源：http://wap.fehbvm.com/Article/details/gbcisxynd.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://wap.fehbvm.com/Article/details/gdjqupyva.sHtML

[Q83] 大小写转换
来源：http://www.m.share.zdbjq.cn/Article/details/gfglxyohq.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://baike.fehbvm.com/Article/details/gwyuhoplw.sHtML

[Q84] 去除首尾空格
来源：http://www.m.share.fehbvm.com/Article/details/ggagmmjep.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/grbxusphc.sHtML

[Q85] 数值取整
来源：http://www.m.share.fehbvm.com/Article/details/gwehvjkim.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://m.share.fehbvm.com/Article/details/glioizicr.sHtML

[Q86] 读取 JSON 字段
来源：http://read.share.fehbvm.com/Article/details/gnkzayvda.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://baike.zdbjq.cn/Article/details/gogtobbgh.sHtML

[Q87] JSON 字段做条件
来源：http://read.share.fehbvm.com/Article/details/gjxzylkdc.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://read.share.zdbjq.cn/Article/details/guztjpfze.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.m.share.fehbvm.com/Article/details/gpkxtuhig.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://m.share.fehbvm.com/Article/details/gkfdfpcqw.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://m.share.fehbvm.com/Article/details/gsmrofuem.sHtML

[Q89] 判断表是否存在
来源：http://blog.hesvh.cn/Article/details/ggfkavtvi.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.m.share.hesvh.cn/Article/details/gxexbzvtf.sHtML

[Q90] 生成序号列
来源：http://read.share.zdbjq.cn/Article/details/gqhsvying.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://mobile.hesvh.cn/Article/details/ghurcqkhu.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gnwrvxylt.sHtML

R. Bash 专题
来源：http://mobile.fehbvm.com/Article/details/gttipzuvh.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gkaubvxlp.sHtML

[R01] shebang 与严格模式
来源：http://3g.fehbvm.com/Article/details/ggkqcnwvw.sHtML

#!/usr/bin/env bash
来源：http://www.blog.fehbvm.com/Article/details/gtrbpakwn.sHtML

set -euo pipefail
来源：http://www.m.share.zdbjq.cn/Article/details/govbzytzi.sHtML

[R02] 变量赋值与使用
来源：http://blog.hesvh.cn/Article/details/gkuxdyykj.sHtML

name="Tom"; echo "$name"
来源：http://wap.hesvh.cn/Article/details/gzkulroqo.sHtML

[R03] 只读变量
来源：http://www.m.share.zdbjq.cn/Article/details/gojzkzbqm.sHtML

readonly PI=3.14
来源：http://www.m.share.fehbvm.com/Article/details/gxncibzmn.sHtML

[R04] 位置参数
来源：http://m.share.zdbjq.cn/Article/details/gisbnbaeg.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://baike.hesvh.cn/Article/details/ghtmzkcoh.sHtML

[R05] 参数默认值
来源：http://wap.fehbvm.com/Article/details/gojpkvvnl.sHtML

name="${1:-default}"
来源：http://3g.zdbjq.cn/Article/details/gicceiviy.sHtML

[R06] 判断命令是否存在
来源：http://www.m.share.zdbjq.cn/Article/details/gabilzscz.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://3g.hesvh.cn/Article/details/gcacaaiuo.sHtML

[R07] if 判断文件
来源：http://blog.fehbvm.com/Article/details/giztxdcns.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://3g.hesvh.cn/Article/details/gyqgzegyl.sHtML

[R08] 数值比较
来源：http://www.m.share.zdbjq.cn/Article/details/gatniweoz.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://blog.fehbvm.com/Article/details/gnlvuhinc.sHtML

[R09] 字符串比较
来源：http://read.share.fehbvm.com/Article/details/gjlgvnvep.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.blog.hesvh.cn/Article/details/glycdouna.sHtML

[R10] 正则匹配
来源：http://www.blog.fehbvm.com/Article/details/gfjjqcltm.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://baike.zdbjq.cn/Article/details/gwtahqwga.sHtML

[R11] case 多分支
来源：http://read.share.fehbvm.com/Article/details/ginwieyvx.sHtML

case "$1" in
来源：http://www.m.share.fehbvm.com/Article/details/gxqelsjcf.sHtML

start) echo "启动" ;;
来源：http://read.share.zdbjq.cn/Article/details/grlclnluq.sHtML

stop)  echo "停止" ;;
来源：http://blog.hesvh.cn/Article/details/gxvtktugm.sHtML

*)     echo "未知命令" ;;
来源：http://mobile.fehbvm.com/Article/details/gtchgzilv.sHtML

esac
来源：http://wap.hesvh.cn/Article/details/gdehgxbwi.sHtML

[R12] for 遍历文件
来源：http://read.share.fehbvm.com/Article/details/gpapmrith.sHtML

for f in *.txt; do echo "$f"; done
来源：http://blog.fehbvm.com/Article/details/gqtnqwpqd.sHtML

[R13] for 计数循环
来源：http://blog.hesvh.cn/Article/details/gtemizvkn.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://mobile.hesvh.cn/Article/details/ghakseclz.sHtML

[R14] C 风格 for
来源：http://wap.fehbvm.com/Article/details/gsfnwlnps.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://blog.zdbjq.cn/Article/details/ghqfiqfzx.sHtML

[R15] while 逐行读文件
来源：http://wap.fehbvm.com/Article/details/gbljqbbpm.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.blog.hesvh.cn/Article/details/gjiyrrlyo.sHtML

[R16] until 等待条件
来源：http://wap.hesvh.cn/Article/details/gpewrctqr.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://mobile.zdbjq.cn/Article/details/gqmtvesgz.sHtML

[R17] 数组定义与取值
来源：http://www.share.fehbvm.com/Article/details/ggdwkvtbi.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://mobile.fehbvm.com/Article/details/goclsexij.sHtML

[R18] 遍历数组
来源：http://mobile.zdbjq.cn/Article/details/gjctsuxzt.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://blog.hesvh.cn/Article/details/gyuoirywv.sHtML

[R19] 数组长度
来源：http://blog.fehbvm.com/Article/details/grsklllrs.sHtML

echo "${#arr[@]}"
来源：http://blog.hesvh.cn/Article/details/gsmlocbaf.sHtML

[R20] 关联数组（字典）
来源：http://wap.fehbvm.com/Article/details/gyrobrpmh.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://blog.fehbvm.com/Article/details/gnciklfwr.sHtML

[R21] 字符串长度
来源：http://baike.fehbvm.com/Article/details/gcffevdfg.sHtML

echo "${#s}"
来源：http://www.share.fehbvm.com/Article/details/gzyuotwmr.sHtML

[R22] 截取子串
来源：http://www.m.share.fehbvm.com/Article/details/gstqscbez.sHtML

echo "${s:0:5}"
来源：http://mobile.fehbvm.com/Article/details/gxnydeobq.sHtML

[R23] 字符串替换
来源：http://www.share.zdbjq.cn/Article/details/gefvnfrne.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://mobile.fehbvm.com/Article/details/gaalejswc.sHtML

[R24] 大小写转换
来源：http://m.share.hesvh.cn/Article/details/gtmzxhevm.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://mobile.hesvh.cn/Article/details/gbsasncpr.sHtML

[R25] 去后缀 / 去前缀
来源：http://read.share.fehbvm.com/Article/details/gdympzkba.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://m.share.fehbvm.com/Article/details/gmjvmxilt.sHtML

[R26] 命令替换
来源：http://blog.hesvh.cn/Article/details/gwnaebfyr.sHtML

now=$(date +%F); echo "$now"
来源：http://wap.zdbjq.cn/Article/details/gjccqmrzq.sHtML

[R27] 算术展开
来源：http://m.share.fehbvm.com/Article/details/ghlpcdqup.sHtML

echo $((1 + 2 * 3))
来源：http://www.m.share.zdbjq.cn/Article/details/gvhllzuiz.sHtML

[R28] 浮点运算
来源：http://www.share.fehbvm.com/Article/details/gzzxfqvpb.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.blog.hesvh.cn/Article/details/gjapykoes.sHtML

[R29] 定义函数
来源：http://blog.hesvh.cn/Article/details/gsfzdokfc.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://blog.fehbvm.com/Article/details/glkqivmna.sHtML

[R30] 函数返回状态码
来源：http://wap.zdbjq.cn/Article/details/gvwrncqdg.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://m.share.fehbvm.com/Article/details/gvlhrofvu.sHtML

[R31] 局部变量
来源：http://mobile.zdbjq.cn/Article/details/ghcmjfmgg.sHtML

f() { local x=1; echo "$x"; }
来源：http://3g.zdbjq.cn/Article/details/garbshtlc.sHtML

[R32] 参数个数校验
来源：http://read.share.fehbvm.com/Article/details/gzjgzhhcn.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.blog.zdbjq.cn/Article/details/gljgvukwg.sHtML

[R33] 捕获错误并提示行号
来源：http://www.m.share.zdbjq.cn/Article/details/ggwhaibqa.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://read.share.zdbjq.cn/Article/details/gwqhlglpv.sHtML

[R34] 退出时清理
来源：http://mobile.hesvh.cn/Article/details/gfuqxtvzn.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://m.share.fehbvm.com/Article/details/gmefegchr.sHtML

[R35] 后台执行并等待
来源：http://www.m.share.hesvh.cn/Article/details/gjgqnkqbs.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.blog.zdbjq.cn/Article/details/gvchtjkql.sHtML

[R36] 并发执行多个任务
来源：http://www.share.hesvh.cn/Article/details/gjuqdsjcu.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://baike.fehbvm.com/Article/details/gbapgqckd.sHtML

[R37] 把输出赋给变量
来源：http://blog.hesvh.cn/Article/details/gxzprnsjm.sHtML

files=$(ls -1)
来源：http://baike.hesvh.cn/Article/details/glutituel.sHtML

[R38] 管道串联
来源：http://wap.zdbjq.cn/Article/details/gubjaujrm.sHtML

cat a.txt | grep -i error | wc -l
来源：http://wap.hesvh.cn/Article/details/gzoaxqyca.sHtML

[R39] 重定向标准输出与错误
来源：http://www.blog.zdbjq.cn/Article/details/gysgfibcz.sHtML

cmd > out.log 2>&1
来源：http://m.share.zdbjq.cn/Article/details/gbnqiaxzn.sHtML

[R40] 追加写日志
来源：http://www.blog.zdbjq.cn/Article/details/gqzcquwpf.sHtML

echo "log" >> out.log
来源：http://mobile.fehbvm.com/Article/details/ggfbkzhei.sHtML

[R41] 丢弃输出
来源：http://www.blog.zdbjq.cn/Article/details/gaqtehchq.sHtML


<!-- 参考信息 -->