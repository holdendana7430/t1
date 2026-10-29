代发 wailian999

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://read.share.fehbvm.com/Article/details/gvtgnfgdx.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://blog.hesvh.cn/Article/details/ghtndrzqo.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.blog.fehbvm.com/Article/details/gwqochiqx.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://blog.fehbvm.com/Article/details/gvpejjpzr.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.share.zdbjq.cn/Article/details/gtqbaamal.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://wap.fehbvm.com/Article/details/gxqgbsgbw.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.blog.fehbvm.com/Article/details/gczsqyftc.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://mobile.zdbjq.cn/Article/details/gmewivexl.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/ghwhjpqqr.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://baike.fehbvm.com/Article/details/gkunuahgh.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gtrtvrrop.sHtML

[Q01] 创建表
来源：http://m.share.zdbjq.cn/Article/details/gdqliogwg.sHtML

CREATE TABLE users (
来源：http://mobile.hesvh.cn/Article/details/gjattpwkr.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.fehbvm.com/Article/details/gbbijhmvb.sHtML

name VARCHAR(50) NOT NULL,
来源：http://baike.hesvh.cn/Article/details/glerjcchc.sHtML

email VARCHAR(100) UNIQUE,
来源：http://mobile.fehbvm.com/Article/details/gsqlkdktl.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.m.share.zdbjq.cn/Article/details/gysqryvib.sHtML

);
来源：http://wap.zdbjq.cn/Article/details/ghbnjupkf.sHtML

[Q02] 创建带外键的表
来源：http://read.share.hesvh.cn/Article/details/gassarfyp.sHtML

CREATE TABLE orders (
来源：http://www.blog.hesvh.cn/Article/details/gtgtipvgu.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.zdbjq.cn/Article/details/gwkvqpexp.sHtML

user_id INT NOT NULL,
来源：http://m.share.fehbvm.com/Article/details/gthvkvted.sHtML

amount DECIMAL(10, 2),
来源：http://mobile.zdbjq.cn/Article/details/gdhsblynx.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://read.share.fehbvm.com/Article/details/gptegngdk.sHtML

);
来源：http://3g.zdbjq.cn/Article/details/gpfitrluc.sHtML

[Q03] 增加列
来源：http://3g.hesvh.cn/Article/details/gecsxoeyn.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.m.share.zdbjq.cn/Article/details/gkusjildm.sHtML

[Q04] 修改列类型
来源：http://mobile.fehbvm.com/Article/details/gjbmpfwqb.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://blog.fehbvm.com/Article/details/gikoyhyds.sHtML

[Q05] 重命名列
来源：http://m.share.hesvh.cn/Article/details/grcjsidlc.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://3g.hesvh.cn/Article/details/gewmhflqm.sHtML

[Q06] 删除列
来源：http://blog.fehbvm.com/Article/details/gaszrmrpd.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.share.zdbjq.cn/Article/details/gbyvxnlix.sHtML

[Q07] 删除表
来源：http://www.share.fehbvm.com/Article/details/gaujzmnng.sHtML

DROP TABLE IF EXISTS orders;
来源：http://baike.fehbvm.com/Article/details/gjqwuwyyn.sHtML

[Q08] 创建普通索引
来源：http://www.m.share.zdbjq.cn/Article/details/gksvfdrec.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://mobile.zdbjq.cn/Article/details/gmvbmxmnl.sHtML

[Q09] 创建唯一索引
来源：http://wap.zdbjq.cn/Article/details/gpcqerifg.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.share.hesvh.cn/Article/details/gxnykwuyd.sHtML

[Q10] 插入单行
来源：http://3g.fehbvm.com/Article/details/gcrxfdhit.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://wap.zdbjq.cn/Article/details/gkfcapifn.sHtML

[Q11] 一次插入多行
来源：http://baike.zdbjq.cn/Article/details/gnllclznc.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://blog.hesvh.cn/Article/details/grwaocnxk.sHtML

[Q12] 插入后取自增 ID
来源：http://m.share.zdbjq.cn/Article/details/gptjvmwwe.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://m.share.hesvh.cn/Article/details/ggfqbqtqt.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://wap.zdbjq.cn/Article/details/grafusuzw.sHtML

[Q13] 忽略重复插入
来源：http://m.share.fehbvm.com/Article/details/gkbdzzpyi.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://baike.zdbjq.cn/Article/details/gpcpywjno.sHtML

[Q14] 存在则更新（upsert）
来源：http://wap.hesvh.cn/Article/details/gyzdgmgcp.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://3g.hesvh.cn/Article/details/gvwczfdzc.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://mobile.fehbvm.com/Article/details/gkuvfbyoq.sHtML

[Q15] 查询全部
来源：http://m.share.hesvh.cn/Article/details/gllavpqsa.sHtML

SELECT * FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gmpqbhkfp.sHtML

[Q16] 查询指定列
来源：http://www.m.share.fehbvm.com/Article/details/gzvfirtke.sHtML

SELECT id, name FROM users;
来源：http://m.share.hesvh.cn/Article/details/gumvevrfi.sHtML

[Q17] 条件查询
来源：http://www.m.share.zdbjq.cn/Article/details/gdmqlwhej.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://read.share.zdbjq.cn/Article/details/gbgcpbzsb.sHtML

[Q18] 模糊匹配
来源：http://3g.hesvh.cn/Article/details/gqrxtyccy.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://wap.fehbvm.com/Article/details/gwmugmzvr.sHtML

[Q19] 范围查询
来源：http://read.share.zdbjq.cn/Article/details/gfyxrrgwu.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://wap.zdbjq.cn/Article/details/gqubkpqsq.sHtML

[Q20] IN 列表
来源：http://www.blog.hesvh.cn/Article/details/gnepvqttl.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://mobile.hesvh.cn/Article/details/gvizfhjri.sHtML

[Q21] 空值判断
来源：http://www.blog.hesvh.cn/Article/details/gfhdbdsmc.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.m.share.zdbjq.cn/Article/details/glhcufupz.sHtML

[Q22] 排序
来源：http://wap.fehbvm.com/Article/details/goxclbpsc.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://read.share.zdbjq.cn/Article/details/gxwdyprxk.sHtML

[Q23] 分页
来源：http://read.share.zdbjq.cn/Article/details/gksiqmorx.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://wap.zdbjq.cn/Article/details/gmjjkrdsr.sHtML

[Q24] 去重
来源：http://www.m.share.zdbjq.cn/Article/details/gtwpkadoe.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gjkimkaez.sHtML

[Q25] 只取前 N 条
来源：http://m.share.hesvh.cn/Article/details/gednqeeci.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://blog.hesvh.cn/Article/details/gdmulnqkh.sHtML

[Q26] 计数
来源：http://www.blog.hesvh.cn/Article/details/gbntjwyaz.sHtML

SELECT COUNT(*) FROM users;
来源：http://baike.hesvh.cn/Article/details/gheaxoaue.sHtML

[Q27] 条件计数
来源：http://m.share.fehbvm.com/Article/details/gkipqugck.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.share.hesvh.cn/Article/details/gfhndsqoq.sHtML

[Q28] 求和与平均
来源：http://wap.fehbvm.com/Article/details/gtvwdpiqp.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.m.share.fehbvm.com/Article/details/gxxficgpn.sHtML

[Q29] 最大最小值
来源：http://3g.hesvh.cn/Article/details/gnrkhsotw.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://read.share.fehbvm.com/Article/details/gpvxxavby.sHtML

[Q30] 分组统计
来源：http://baike.fehbvm.com/Article/details/gbiimuypf.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://mobile.hesvh.cn/Article/details/gpwohjolx.sHtML

[Q31] 分组后过滤
来源：http://read.share.zdbjq.cn/Article/details/guakhsylt.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.blog.zdbjq.cn/Article/details/giwqliggf.sHtML

[Q32] 分组拼接字符串
来源：http://www.m.share.hesvh.cn/Article/details/gqvmbeurx.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.share.zdbjq.cn/Article/details/glulpbxkl.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://3g.zdbjq.cn/Article/details/gjhvexail.sHtML

[Q33] 多列分组
来源：http://m.share.fehbvm.com/Article/details/gzlplhqfa.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://wap.hesvh.cn/Article/details/gkfloshfc.sHtML

[Q34] 每组取第一条
来源：http://mobile.zdbjq.cn/Article/details/glolqjcgh.sHtML

SELECT * FROM (
来源：http://m.share.zdbjq.cn/Article/details/gpuijntni.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://baike.hesvh.cn/Article/details/gmhrlopwz.sHtML

) t WHERE rn = 1;
来源：http://www.share.zdbjq.cn/Article/details/guktmonqp.sHtML

[Q35] 内连接
来源：http://www.blog.zdbjq.cn/Article/details/gukfpkfjg.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://wap.zdbjq.cn/Article/details/gckdczyxv.sHtML

[Q36] 左连接
来源：http://www.m.share.hesvh.cn/Article/details/grzcwddur.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://blog.zdbjq.cn/Article/details/gxohnbncu.sHtML

[Q37] 右连接
来源：http://m.share.hesvh.cn/Article/details/gscxftlhc.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.share.zdbjq.cn/Article/details/gxgiqrueo.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://m.share.hesvh.cn/Article/details/gjluhpwwf.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.share.hesvh.cn/Article/details/gqhehqlnd.sHtML

[Q39] 自连接（查上下级）
来源：http://3g.zdbjq.cn/Article/details/gxvpgfhlq.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://wap.hesvh.cn/Article/details/gqofjvkbi.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://wap.hesvh.cn/Article/details/gsyqrjnka.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://3g.zdbjq.cn/Article/details/gvhqpnmim.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://baike.fehbvm.com/Article/details/gzxcfumay.sHtML

[Q41] 多表连接
来源：http://3g.zdbjq.cn/Article/details/gruzixsqj.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.share.zdbjq.cn/Article/details/gwrleymab.sHtML

JOIN users u ON u.id = o.user_id
来源：http://baike.fehbvm.com/Article/details/ghafudrxc.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://wap.zdbjq.cn/Article/details/gewuqskud.sHtML

[Q42] 连接条件附加过滤
来源：http://blog.hesvh.cn/Article/details/gckwappat.sHtML

SELECT u.name, o.amount FROM users u
来源：http://wap.fehbvm.com/Article/details/gwnuuajsm.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.blog.hesvh.cn/Article/details/gjspwypjc.sHtML

[Q43] 标量子查询
来源：http://read.share.zdbjq.cn/Article/details/gindzmobw.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.m.share.zdbjq.cn/Article/details/gsroajrmp.sHtML

[Q44] IN 子查询
来源：http://read.share.fehbvm.com/Article/details/gqrssexan.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.blog.zdbjq.cn/Article/details/gbiqahomz.sHtML

[Q45] EXISTS 判断存在
来源：http://www.m.share.zdbjq.cn/Article/details/gtrrotzie.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.hesvh.cn/Article/details/gmgihlqnr.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://baike.zdbjq.cn/Article/details/gqubdoslt.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.zdbjq.cn/Article/details/gafkcubkp.sHtML

[Q47] 与平均值比较
来源：http://wap.fehbvm.com/Article/details/gccqanyvj.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.blog.zdbjq.cn/Article/details/glekidjss.sHtML

[Q48] CTE 公用表表达式
来源：http://www.share.hesvh.cn/Article/details/gfuiizcjq.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://blog.zdbjq.cn/Article/details/ghheqbikg.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.blog.hesvh.cn/Article/details/gwvvhugks.sHtML

[Q49] 更新单行
来源：http://read.share.fehbvm.com/Article/details/glwppebyi.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.share.fehbvm.com/Article/details/gpfkzswis.sHtML

[Q50] 批量更新
来源：http://3g.hesvh.cn/Article/details/gbvltstmz.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://read.share.zdbjq.cn/Article/details/gscgbnccx.sHtML

[Q51] 用子查询更新
来源：http://wap.hesvh.cn/Article/details/gxwafsmxc.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://wap.zdbjq.cn/Article/details/gluqtffcl.sHtML

[Q52] 删除指定行
来源：http://baike.fehbvm.com/Article/details/gtbkwdmcw.sHtML

DELETE FROM users WHERE id = 10;
来源：http://read.share.hesvh.cn/Article/details/gquaxgxeo.sHtML

[Q53] 按条件删除
来源：http://mobile.hesvh.cn/Article/details/gvejoethm.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.share.hesvh.cn/Article/details/gfrcgkuxo.sHtML

[Q54] 清空表
来源：http://read.share.zdbjq.cn/Article/details/gvpdsbocu.sHtML

TRUNCATE TABLE logs;
来源：http://3g.fehbvm.com/Article/details/gonzwriyo.sHtML

[Q55] 排名（并列占位）
来源：http://m.share.fehbvm.com/Article/details/gusxvwpnr.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://wap.zdbjq.cn/Article/details/gudrryafp.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.share.zdbjq.cn/Article/details/gnrjtuvko.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://m.share.fehbvm.com/Article/details/gpeymqxvt.sHtML

[Q57] 行号
来源：http://read.share.zdbjq.cn/Article/details/gfwbdbreb.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gyhzrdbml.sHtML

[Q58] 累计求和
来源：http://www.m.share.fehbvm.com/Article/details/gxyjrlrru.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://mobile.zdbjq.cn/Article/details/gzsdabgzy.sHtML

[Q59] 分组内累计
来源：http://www.blog.hesvh.cn/Article/details/goylrguqx.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://blog.zdbjq.cn/Article/details/gxswnwgsu.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.share.fehbvm.com/Article/details/gutsronuh.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://m.share.fehbvm.com/Article/details/gkysogvzk.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://blog.fehbvm.com/Article/details/gbomsaeoe.sHtML

[Q61] 移动平均
来源：http://wap.fehbvm.com/Article/details/giihmlolv.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.share.hesvh.cn/Article/details/gmmirzpdv.sHtML

[Q62] 分组占比
来源：http://wap.zdbjq.cn/Article/details/gpqggxpeh.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://m.share.zdbjq.cn/Article/details/gxcdunokw.sHtML

[Q63] 开启事务
来源：http://baike.fehbvm.com/Article/details/gnegracqr.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.m.share.zdbjq.cn/Article/details/gxnxzvnvu.sHtML

[Q64] 提交事务
来源：http://www.share.fehbvm.com/Article/details/gfdpmxatk.sHtML

COMMIT;
来源：http://3g.zdbjq.cn/Article/details/gzsxzhibp.sHtML

[Q65] 回滚事务
来源：http://baike.fehbvm.com/Article/details/gcepiwgxo.sHtML

ROLLBACK;
来源：http://m.share.fehbvm.com/Article/details/galramclh.sHtML

[Q66] 行锁查询
来源：http://m.share.hesvh.cn/Article/details/gqtdrpbds.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://mobile.fehbvm.com/Article/details/gagysxywn.sHtML

[Q67] 设置隔离级别
来源：http://www.blog.zdbjq.cn/Article/details/gdogiswug.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://m.share.fehbvm.com/Article/details/gxbdfencf.sHtML

[Q68] 保存点
来源：http://m.share.hesvh.cn/Article/details/gshqelgmu.sHtML

SAVEPOINT sp1;
来源：http://mobile.zdbjq.cn/Article/details/gihfjkyxx.sHtML

ROLLBACK TO sp1;
来源：http://www.m.share.fehbvm.com/Article/details/gmxydjkzk.sHtML

[Q69] 查看执行计划
来源：http://3g.fehbvm.com/Article/details/giqosvhzv.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://3g.zdbjq.cn/Article/details/gackltdvm.sHtML

[Q70] 更新统计信息
来源：http://3g.zdbjq.cn/Article/details/gvbtwjqbz.sHtML

ANALYZE TABLE users;
来源：http://mobile.hesvh.cn/Article/details/gskebwagv.sHtML

[Q71] 查看建表语句
来源：http://m.share.fehbvm.com/Article/details/gxfoqlfqi.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.share.hesvh.cn/Article/details/gycjrcumf.sHtML

[Q72] 查看索引
来源：http://3g.zdbjq.cn/Article/details/gqemxdgze.sHtML

SHOW INDEX FROM users;
来源：http://mobile.zdbjq.cn/Article/details/ggtlznddk.sHtML

[Q73] 查看表状态
来源：http://baike.fehbvm.com/Article/details/glgxturld.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://baike.hesvh.cn/Article/details/godsoqygh.sHtML

[Q74] 强制使用索引
来源：http://m.share.hesvh.cn/Article/details/geghhjurd.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://m.share.fehbvm.com/Article/details/gsbvmucdr.sHtML

[Q75] 日期格式化
来源：http://blog.fehbvm.com/Article/details/govuncffh.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://m.share.hesvh.cn/Article/details/gccrgsbgm.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://mobile.hesvh.cn/Article/details/gfuqwhaue.sHtML

[Q76] 按天统计
来源：http://wap.hesvh.cn/Article/details/gcylpjvho.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://blog.hesvh.cn/Article/details/gfvabnmre.sHtML

[Q77] 时间加减
来源：http://read.share.hesvh.cn/Article/details/gdaivbavl.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://mobile.hesvh.cn/Article/details/gwukwwier.sHtML

[Q78] 当前时间
来源：http://mobile.fehbvm.com/Article/details/giozfhfhe.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.share.hesvh.cn/Article/details/gckcyqbcj.sHtML

[Q79] 字符串拼接
来源：http://3g.hesvh.cn/Article/details/gazbjzfby.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.m.share.fehbvm.com/Article/details/gydlswuba.sHtML

[Q80] 字符串截取
来源：http://m.share.hesvh.cn/Article/details/guyaorsrt.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://m.share.zdbjq.cn/Article/details/guolqcfnm.sHtML

[Q81] 字符串替换
来源：http://www.m.share.hesvh.cn/Article/details/gzhgfzife.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.share.zdbjq.cn/Article/details/glpwvizag.sHtML

[Q82] 字符长度与字节长度
来源：http://mobile.zdbjq.cn/Article/details/gnguffikw.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gulxpqgth.sHtML

[Q83] 大小写转换
来源：http://www.share.zdbjq.cn/Article/details/gfiwkdxfs.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://baike.fehbvm.com/Article/details/gkbbcgwsj.sHtML

[Q84] 去除首尾空格
来源：http://www.blog.fehbvm.com/Article/details/gyfrszzxp.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gtwzutwkk.sHtML

[Q85] 数值取整
来源：http://baike.hesvh.cn/Article/details/gtjfpzfnn.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://baike.hesvh.cn/Article/details/gzsmzqsxd.sHtML

[Q86] 读取 JSON 字段
来源：http://wap.zdbjq.cn/Article/details/gdazfwzka.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.share.hesvh.cn/Article/details/ggckaqemf.sHtML

[Q87] JSON 字段做条件
来源：http://mobile.fehbvm.com/Article/details/gobthvlgb.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.share.hesvh.cn/Article/details/gglvrmamd.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.m.share.fehbvm.com/Article/details/gdettkapb.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://wap.zdbjq.cn/Article/details/ghlmolxit.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gixxsrhvo.sHtML

[Q89] 判断表是否存在
来源：http://mobile.hesvh.cn/Article/details/ggqynvodk.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://read.share.zdbjq.cn/Article/details/ggrlssuuo.sHtML

[Q90] 生成序号列
来源：http://m.share.fehbvm.com/Article/details/ggdzmakni.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://m.share.zdbjq.cn/Article/details/gkandboid.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gkxkkbxxh.sHtML

R. Bash 专题
来源：http://3g.hesvh.cn/Article/details/gzssiiefm.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gyojncpwo.sHtML

[R01] shebang 与严格模式
来源：http://3g.fehbvm.com/Article/details/gdibswscw.sHtML

#!/usr/bin/env bash
来源：http://www.share.hesvh.cn/Article/details/gnawrsuvd.sHtML

set -euo pipefail
来源：http://m.share.fehbvm.com/Article/details/gafahkjvf.sHtML

[R02] 变量赋值与使用
来源：http://blog.zdbjq.cn/Article/details/gxkepjqpm.sHtML

name="Tom"; echo "$name"
来源：http://www.blog.fehbvm.com/Article/details/gikxqtgjb.sHtML

[R03] 只读变量
来源：http://wap.fehbvm.com/Article/details/gkypfrfwo.sHtML

readonly PI=3.14
来源：http://3g.hesvh.cn/Article/details/gfyrdxmeb.sHtML

[R04] 位置参数
来源：http://www.m.share.zdbjq.cn/Article/details/gjbjhcmvl.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://read.share.fehbvm.com/Article/details/glholzyoi.sHtML

[R05] 参数默认值
来源：http://read.share.hesvh.cn/Article/details/gnsajarwm.sHtML

name="${1:-default}"
来源：http://www.blog.hesvh.cn/Article/details/gvkkclzwn.sHtML

[R06] 判断命令是否存在
来源：http://3g.fehbvm.com/Article/details/gqckysjqs.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.blog.zdbjq.cn/Article/details/gksmxggbl.sHtML

[R07] if 判断文件
来源：http://read.share.fehbvm.com/Article/details/grbsoxgkt.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.blog.zdbjq.cn/Article/details/gdqmwoojy.sHtML

[R08] 数值比较
来源：http://www.m.share.fehbvm.com/Article/details/gadiarsgo.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.blog.hesvh.cn/Article/details/gxpqkqcel.sHtML

[R09] 字符串比较
来源：http://3g.hesvh.cn/Article/details/gnjvevegg.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://3g.zdbjq.cn/Article/details/gsahfjpdu.sHtML

[R10] 正则匹配
来源：http://read.share.zdbjq.cn/Article/details/gjfsitxqs.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://mobile.zdbjq.cn/Article/details/gybrfgfpv.sHtML

[R11] case 多分支
来源：http://wap.hesvh.cn/Article/details/gfgoztcyh.sHtML

case "$1" in
来源：http://read.share.fehbvm.com/Article/details/grherhwsi.sHtML

start) echo "启动" ;;
来源：http://read.share.fehbvm.com/Article/details/gbxrjiiyi.sHtML

stop)  echo "停止" ;;
来源：http://baike.fehbvm.com/Article/details/gsjcmktjw.sHtML

*)     echo "未知命令" ;;
来源：http://www.m.share.hesvh.cn/Article/details/gtendobsu.sHtML

esac
来源：http://www.blog.hesvh.cn/Article/details/gahcdxjpa.sHtML

[R12] for 遍历文件
来源：http://m.share.fehbvm.com/Article/details/ggzwwpomq.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.m.share.fehbvm.com/Article/details/gtrcjrbfb.sHtML

[R13] for 计数循环
来源：http://www.share.zdbjq.cn/Article/details/gsakwqtlr.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.blog.zdbjq.cn/Article/details/guzcafenh.sHtML

[R14] C 风格 for
来源：http://www.blog.zdbjq.cn/Article/details/gughisqso.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://read.share.hesvh.cn/Article/details/gyktvturq.sHtML

[R15] while 逐行读文件
来源：http://read.share.fehbvm.com/Article/details/gshohvodi.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.m.share.hesvh.cn/Article/details/gvucvledx.sHtML

[R16] until 等待条件
来源：http://mobile.fehbvm.com/Article/details/gqcawczvj.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://baike.hesvh.cn/Article/details/ghwjnjbde.sHtML

[R17] 数组定义与取值
来源：http://www.blog.hesvh.cn/Article/details/gtoqqxklx.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://m.share.fehbvm.com/Article/details/gelmtlhxz.sHtML

[R18] 遍历数组
来源：http://read.share.zdbjq.cn/Article/details/gwwdiojoa.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://blog.fehbvm.com/Article/details/grcwgwavv.sHtML

[R19] 数组长度
来源：http://m.share.zdbjq.cn/Article/details/ggaycqwns.sHtML

echo "${#arr[@]}"
来源：http://m.share.fehbvm.com/Article/details/gdcsyznqy.sHtML

[R20] 关联数组（字典）
来源：http://blog.hesvh.cn/Article/details/gsujvmoyx.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://baike.hesvh.cn/Article/details/gszqowsdq.sHtML

[R21] 字符串长度
来源：http://www.m.share.hesvh.cn/Article/details/gghxgclvq.sHtML

echo "${#s}"
来源：http://baike.hesvh.cn/Article/details/gmpcnyplu.sHtML

[R22] 截取子串
来源：http://3g.hesvh.cn/Article/details/gctpwjols.sHtML

echo "${s:0:5}"
来源：http://baike.zdbjq.cn/Article/details/gmpeikarl.sHtML

[R23] 字符串替换
来源：http://wap.hesvh.cn/Article/details/gmocxrsbd.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://m.share.hesvh.cn/Article/details/gdlnmeawi.sHtML

[R24] 大小写转换
来源：http://baike.fehbvm.com/Article/details/grxejuusc.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.share.hesvh.cn/Article/details/gltrhiykf.sHtML

[R25] 去后缀 / 去前缀
来源：http://3g.zdbjq.cn/Article/details/gvmlxnbfv.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://blog.zdbjq.cn/Article/details/gdyiimfwg.sHtML

[R26] 命令替换
来源：http://www.m.share.fehbvm.com/Article/details/gpvyqiwyw.sHtML

now=$(date +%F); echo "$now"
来源：http://mobile.hesvh.cn/Article/details/gpdelfpsv.sHtML

[R27] 算术展开
来源：http://www.blog.zdbjq.cn/Article/details/gtiwgvfve.sHtML

echo $((1 + 2 * 3))
来源：http://www.share.zdbjq.cn/Article/details/gwpbfetgr.sHtML

[R28] 浮点运算
来源：http://3g.fehbvm.com/Article/details/gxbhlwfep.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.m.share.zdbjq.cn/Article/details/guslwidec.sHtML

[R29] 定义函数
来源：http://blog.zdbjq.cn/Article/details/gzljuvinp.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://3g.zdbjq.cn/Article/details/gsrwbbnog.sHtML

[R30] 函数返回状态码
来源：http://www.share.fehbvm.com/Article/details/gxrtlxxiu.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://baike.fehbvm.com/Article/details/gnnlcgumx.sHtML

[R31] 局部变量
来源：http://read.share.hesvh.cn/Article/details/gcwbdlxeb.sHtML

f() { local x=1; echo "$x"; }
来源：http://baike.zdbjq.cn/Article/details/gbsygkyjg.sHtML

[R32] 参数个数校验
来源：http://www.m.share.hesvh.cn/Article/details/gcsrxzfzl.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.blog.hesvh.cn/Article/details/gnhovqspw.sHtML

[R33] 捕获错误并提示行号
来源：http://www.m.share.zdbjq.cn/Article/details/ggxlfarem.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.share.zdbjq.cn/Article/details/gifjkjmec.sHtML

[R34] 退出时清理
来源：http://www.blog.hesvh.cn/Article/details/gfbcjzgdc.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://3g.hesvh.cn/Article/details/gyglkrkil.sHtML

[R35] 后台执行并等待
来源：http://www.blog.hesvh.cn/Article/details/gvowslmow.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://3g.zdbjq.cn/Article/details/gfthbmunl.sHtML

[R36] 并发执行多个任务
来源：http://www.share.zdbjq.cn/Article/details/gzuypwcpk.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://m.share.zdbjq.cn/Article/details/gstkunjmi.sHtML

[R37] 把输出赋给变量
来源：http://read.share.zdbjq.cn/Article/details/gipxsmqxw.sHtML

files=$(ls -1)
来源：http://blog.fehbvm.com/Article/details/gwfhtvqpb.sHtML

[R38] 管道串联
来源：http://www.share.hesvh.cn/Article/details/grlqspqtt.sHtML

cat a.txt | grep -i error | wc -l
来源：http://m.share.zdbjq.cn/Article/details/gniiycqpu.sHtML

[R39] 重定向标准输出与错误
来源：http://www.blog.hesvh.cn/Article/details/ggnszelxk.sHtML


<!-- 参考信息 -->