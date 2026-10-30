代发 wailian999

CREATE TABLE users (
来源：http://www.share.fanxiaobao.xyz/Article/details/gfpdgxuwv.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.fanxiaobao.xyz/Article/details/gwpcxckru.sHtML

name VARCHAR(50) NOT NULL,
来源：http://wap.fanxiaobao.xyz/Article/details/gjagabong.sHtML

email VARCHAR(100) UNIQUE,
来源：http://baike.fanxiaobao.xyz/Article/details/gzasvaers.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://3g.fanxiaobao.xyz/Article/details/gqsciaqsb.sHtML

);
来源：http://3g.fanxiaobao.xyz/Article/details/gluqiwlgk.sHtML

[Q02] 创建带外键的表
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goyrwhoqm.sHtML

CREATE TABLE orders (
来源：http://wap.fanxiaobao.xyz/Article/details/gmeadbyhb.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.fanxiaobao.xyz/Article/details/gogfxypyj.sHtML

user_id INT NOT NULL,
来源：http://blog.fanxiaobao.xyz/Article/details/guccyhxur.sHtML

amount DECIMAL(10, 2),
来源：http://3g.fanxiaobao.xyz/Article/details/gqlgtoxzp.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://mobile.fanxiaobao.xyz/Article/details/guagddzhw.sHtML

);
来源：http://mobile.fanxiaobao.xyz/Article/details/gsvkammjm.sHtML

[Q03] 增加列
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcqalwxnt.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://read.share.fanxiaobao.xyz/Article/details/ggtmafjvn.sHtML

[Q04] 修改列类型
来源：http://read.share.fanxiaobao.xyz/Article/details/ggvvgmylr.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://wap.fanxiaobao.xyz/Article/details/gdafdqgcx.sHtML

[Q05] 重命名列
来源：http://m.share.fanxiaobao.xyz/Article/details/gqftdtequ.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://3g.fanxiaobao.xyz/Article/details/geogcpbyw.sHtML

[Q06] 删除列
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghwrbxhjb.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.share.fanxiaobao.xyz/Article/details/gtvuzytdv.sHtML

[Q07] 删除表
来源：http://read.share.fanxiaobao.xyz/Article/details/gxvglginy.sHtML

DROP TABLE IF EXISTS orders;
来源：http://mobile.fanxiaobao.xyz/Article/details/gteikjyif.sHtML

[Q08] 创建普通索引
来源：http://3g.fanxiaobao.xyz/Article/details/gftdqzinj.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://m.share.fanxiaobao.xyz/Article/details/gegqtqaok.sHtML

[Q09] 创建唯一索引
来源：http://blog.fanxiaobao.xyz/Article/details/gvuegbinw.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://3g.fanxiaobao.xyz/Article/details/gnhcxujfj.sHtML

[Q10] 插入单行
来源：http://www.share.fanxiaobao.xyz/Article/details/gxntnlfha.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://read.share.fanxiaobao.xyz/Article/details/gcomuruqj.sHtML

[Q11] 一次插入多行
来源：http://blog.fanxiaobao.xyz/Article/details/gczalvyvk.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.share.fanxiaobao.xyz/Article/details/ghbtozrqn.sHtML

[Q12] 插入后取自增 ID
来源：http://3g.fanxiaobao.xyz/Article/details/glkrzocbs.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://blog.fanxiaobao.xyz/Article/details/gzjjfffqz.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpdsnbzae.sHtML

[Q13] 忽略重复插入
来源：http://m.share.fanxiaobao.xyz/Article/details/gdnqqzasg.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkozzawrd.sHtML

[Q14] 存在则更新（upsert）
来源：http://mobile.fanxiaobao.xyz/Article/details/ggapkghrb.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://3g.fanxiaobao.xyz/Article/details/gyuofpvyr.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://wap.fanxiaobao.xyz/Article/details/gitzrcqya.sHtML

[Q15] 查询全部
来源：http://read.share.fanxiaobao.xyz/Article/details/gdtcflrxm.sHtML

SELECT * FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gbabppimo.sHtML

[Q16] 查询指定列
来源：http://m.share.fanxiaobao.xyz/Article/details/gpxhvzjpv.sHtML

SELECT id, name FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gjhyclpgq.sHtML

[Q17] 条件查询
来源：http://blog.fanxiaobao.xyz/Article/details/gortyrsld.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gawxjhglb.sHtML

[Q18] 模糊匹配
来源：http://www.share.fanxiaobao.xyz/Article/details/gnxpdviqk.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://blog.fanxiaobao.xyz/Article/details/gmkrlghgh.sHtML

[Q19] 范围查询
来源：http://mobile.fanxiaobao.xyz/Article/details/gvqrxngjq.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://wap.fanxiaobao.xyz/Article/details/gauavkget.sHtML

[Q20] IN 列表
来源：http://www.blog.fanxiaobao.xyz/Article/details/goulnimsf.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://mobile.fanxiaobao.xyz/Article/details/gtmsbkfli.sHtML

[Q21] 空值判断
来源：http://www.share.fanxiaobao.xyz/Article/details/gkiboukeb.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://blog.fanxiaobao.xyz/Article/details/gguwpmugz.sHtML

[Q22] 排序
来源：http://blog.fanxiaobao.xyz/Article/details/glcrjcmoz.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://blog.fanxiaobao.xyz/Article/details/gffyyemas.sHtML

[Q23] 分页
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtenocswm.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://blog.fanxiaobao.xyz/Article/details/ggcvhatps.sHtML

[Q24] 去重
来源：http://blog.fanxiaobao.xyz/Article/details/gcxgefnsg.sHtML

SELECT DISTINCT city FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gdbraztgh.sHtML

[Q25] 只取前 N 条
来源：http://blog.fanxiaobao.xyz/Article/details/gunyeinan.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://m.share.fanxiaobao.xyz/Article/details/gumaqeirp.sHtML

[Q26] 计数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gijidraer.sHtML

SELECT COUNT(*) FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gaakvgvfk.sHtML

[Q27] 条件计数
来源：http://baike.fanxiaobao.xyz/Article/details/gemjbkpvu.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giwexmuwz.sHtML

[Q28] 求和与平均
来源：http://mobile.fanxiaobao.xyz/Article/details/gszxdlwso.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.share.fanxiaobao.xyz/Article/details/gqrxudjsg.sHtML

[Q29] 最大最小值
来源：http://mobile.fanxiaobao.xyz/Article/details/gaydoqhtz.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gysqphkah.sHtML

[Q30] 分组统计
来源：http://m.share.fanxiaobao.xyz/Article/details/gukyhtryv.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcfakfuqq.sHtML

[Q31] 分组后过滤
来源：http://m.share.fanxiaobao.xyz/Article/details/glpenwyrk.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://wap.fanxiaobao.xyz/Article/details/gnjmjbqqy.sHtML

[Q32] 分组拼接字符串
来源：http://baike.fanxiaobao.xyz/Article/details/ggwfpmkhq.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.share.fanxiaobao.xyz/Article/details/ggkvsvnpc.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://m.share.fanxiaobao.xyz/Article/details/gbajlsgvj.sHtML

[Q33] 多列分组
来源：http://3g.fanxiaobao.xyz/Article/details/gvuejvyio.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://wap.fanxiaobao.xyz/Article/details/gbiccmxdv.sHtML

[Q34] 每组取第一条
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjejdradp.sHtML

SELECT * FROM (
来源：http://www.blog.fanxiaobao.xyz/Article/details/gasyzeuls.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://3g.fanxiaobao.xyz/Article/details/gizquvevh.sHtML

) t WHERE rn = 1;
来源：http://blog.fanxiaobao.xyz/Article/details/gcvbqumkq.sHtML

[Q35] 内连接
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmmpinrgt.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://m.share.fanxiaobao.xyz/Article/details/gdqduhwbk.sHtML

[Q36] 左连接
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyvhrfxrf.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://baike.fanxiaobao.xyz/Article/details/glnopmzsv.sHtML

[Q37] 右连接
来源：http://baike.fanxiaobao.xyz/Article/details/gpfpwwrez.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://mobile.fanxiaobao.xyz/Article/details/gwsvjspqp.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://baike.fanxiaobao.xyz/Article/details/glixtsnqd.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://read.share.fanxiaobao.xyz/Article/details/gonssukgt.sHtML

[Q39] 自连接（查上下级）
来源：http://read.share.fanxiaobao.xyz/Article/details/gevfmwhfs.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://3g.fanxiaobao.xyz/Article/details/gdxoficsb.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://baike.fanxiaobao.xyz/Article/details/gmrtsolqg.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://blog.fanxiaobao.xyz/Article/details/gxaaindot.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://mobile.fanxiaobao.xyz/Article/details/ghuhqawyw.sHtML

[Q41] 多表连接
来源：http://wap.fanxiaobao.xyz/Article/details/ghozqtjiz.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://read.share.fanxiaobao.xyz/Article/details/ginftvvav.sHtML

JOIN users u ON u.id = o.user_id
来源：http://m.share.fanxiaobao.xyz/Article/details/gqvviegcy.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfbrwezhj.sHtML

[Q42] 连接条件附加过滤
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfhouytdm.sHtML

SELECT u.name, o.amount FROM users u
来源：http://baike.fanxiaobao.xyz/Article/details/ggevlxntz.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://read.share.fanxiaobao.xyz/Article/details/gcesbxksa.sHtML

[Q43] 标量子查询
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnxsikhwj.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://baike.fanxiaobao.xyz/Article/details/gvpqpwnwd.sHtML

[Q44] IN 子查询
来源：http://wap.fanxiaobao.xyz/Article/details/ghhupzhgt.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.share.fanxiaobao.xyz/Article/details/gwfqoctwd.sHtML

[Q45] EXISTS 判断存在
来源：http://wap.fanxiaobao.xyz/Article/details/gnqsdhsex.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyeyvyqvl.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.blog.fanxiaobao.xyz/Article/details/gonxpxewe.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.fanxiaobao.xyz/Article/details/gmfvtvsxu.sHtML

[Q47] 与平均值比较
来源：http://blog.fanxiaobao.xyz/Article/details/gcufoeict.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.share.fanxiaobao.xyz/Article/details/gznmyikyn.sHtML

[Q48] CTE 公用表表达式
来源：http://baike.fanxiaobao.xyz/Article/details/geyaorhub.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gritwlkzc.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://blog.fanxiaobao.xyz/Article/details/gcwkeoslw.sHtML

[Q49] 更新单行
来源：http://mobile.fanxiaobao.xyz/Article/details/gbeviausb.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://read.share.fanxiaobao.xyz/Article/details/gaiszkmks.sHtML

[Q50] 批量更新
来源：http://mobile.fanxiaobao.xyz/Article/details/gswkbihyg.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.share.fanxiaobao.xyz/Article/details/gselwefen.sHtML

[Q51] 用子查询更新
来源：http://mobile.fanxiaobao.xyz/Article/details/gwwaopssb.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://blog.fanxiaobao.xyz/Article/details/gxudpufqj.sHtML

[Q52] 删除指定行
来源：http://www.blog.fanxiaobao.xyz/Article/details/giqkcvbzh.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggzcvauqf.sHtML

[Q53] 按条件删除
来源：http://read.share.fanxiaobao.xyz/Article/details/gbbnncdiy.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.blog.fanxiaobao.xyz/Article/details/guloilbdb.sHtML

[Q54] 清空表
来源：http://mobile.fanxiaobao.xyz/Article/details/gcgoukezi.sHtML

TRUNCATE TABLE logs;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gozclujsu.sHtML

[Q55] 排名（并列占位）
来源：http://blog.fanxiaobao.xyz/Article/details/gtphthuhk.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://3g.fanxiaobao.xyz/Article/details/gikopxejv.sHtML

[Q56] 密集排名（并列不占位）
来源：http://blog.fanxiaobao.xyz/Article/details/gmlzlyxzu.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://blog.fanxiaobao.xyz/Article/details/gvocbmeda.sHtML

[Q57] 行号
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glwxraiyv.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gsjxjittc.sHtML

[Q58] 累计求和
来源：http://www.share.fanxiaobao.xyz/Article/details/gkgppofds.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjmcghmei.sHtML

[Q59] 分组内累计
来源：http://blog.fanxiaobao.xyz/Article/details/gkbtgtdbs.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://blog.fanxiaobao.xyz/Article/details/gymoceeax.sHtML

[Q60] 取上一行 / 下一行
来源：http://read.share.fanxiaobao.xyz/Article/details/gohbzgazw.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfwfdwfjf.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjlnlatft.sHtML

[Q61] 移动平均
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnhyhwmis.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.share.fanxiaobao.xyz/Article/details/gnkrepnaj.sHtML

[Q62] 分组占比
来源：http://read.share.fanxiaobao.xyz/Article/details/glkpejpgq.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://mobile.fanxiaobao.xyz/Article/details/gjrjxwzmy.sHtML

[Q63] 开启事务
来源：http://mobile.fanxiaobao.xyz/Article/details/gfiweaijz.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://blog.fanxiaobao.xyz/Article/details/gtxatazoa.sHtML

[Q64] 提交事务
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggyspmgep.sHtML

COMMIT;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcdxcibwc.sHtML

[Q65] 回滚事务
来源：http://wap.fanxiaobao.xyz/Article/details/gwcnuetwf.sHtML

ROLLBACK;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqwnbulqd.sHtML

[Q66] 行锁查询
来源：http://mobile.fanxiaobao.xyz/Article/details/ggvgmxemt.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://m.share.fanxiaobao.xyz/Article/details/gdiihfkqt.sHtML

[Q67] 设置隔离级别
来源：http://baike.fanxiaobao.xyz/Article/details/gmmieniyd.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://3g.fanxiaobao.xyz/Article/details/gmcohscav.sHtML

[Q68] 保存点
来源：http://www.blog.fanxiaobao.xyz/Article/details/guinlomsm.sHtML

SAVEPOINT sp1;
来源：http://3g.fanxiaobao.xyz/Article/details/gjyvcngpc.sHtML

ROLLBACK TO sp1;
来源：http://mobile.fanxiaobao.xyz/Article/details/gsgisxilc.sHtML

[Q69] 查看执行计划
来源：http://wap.fanxiaobao.xyz/Article/details/gkswzbmwr.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://m.share.fanxiaobao.xyz/Article/details/giijtjglc.sHtML

[Q70] 更新统计信息
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxccqvhgq.sHtML

ANALYZE TABLE users;
来源：http://wap.fanxiaobao.xyz/Article/details/gmnzroglw.sHtML

[Q71] 查看建表语句
来源：http://m.share.fanxiaobao.xyz/Article/details/gliqdtrld.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://wap.fanxiaobao.xyz/Article/details/gstfotvbc.sHtML

[Q72] 查看索引
来源：http://read.share.fanxiaobao.xyz/Article/details/gpsrnhehf.sHtML

SHOW INDEX FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdnjbhzra.sHtML

[Q73] 查看表状态
来源：http://m.share.fanxiaobao.xyz/Article/details/gfucgkjwx.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://mobile.fanxiaobao.xyz/Article/details/gmoaxzvwy.sHtML

[Q74] 强制使用索引
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxtwytyjn.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://3g.fanxiaobao.xyz/Article/details/gpyvwjbfu.sHtML

[Q75] 日期格式化
来源：http://baike.fanxiaobao.xyz/Article/details/gjedrbjuo.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gseclufrm.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvevxnlef.sHtML

[Q76] 按天统计
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gduycydkx.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://m.share.fanxiaobao.xyz/Article/details/gvmuqkade.sHtML

[Q77] 时间加减
来源：http://m.share.fanxiaobao.xyz/Article/details/gyrucxnmu.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://baike.fanxiaobao.xyz/Article/details/gfawectwb.sHtML

[Q78] 当前时间
来源：http://blog.fanxiaobao.xyz/Article/details/gbijztrru.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://mobile.fanxiaobao.xyz/Article/details/geyrtgfts.sHtML

[Q79] 字符串拼接
来源：http://baike.fanxiaobao.xyz/Article/details/gwlepkngw.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://blog.fanxiaobao.xyz/Article/details/gfkhwhpmx.sHtML

[Q80] 字符串截取
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghvugilsn.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gnxmoeobm.sHtML

[Q81] 字符串替换
来源：http://www.share.fanxiaobao.xyz/Article/details/gumqzohlu.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/ggribndon.sHtML

[Q82] 字符长度与字节长度
来源：http://www.share.fanxiaobao.xyz/Article/details/gfusbeypq.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfwgehvpo.sHtML

[Q83] 大小写转换
来源：http://wap.fanxiaobao.xyz/Article/details/glcpikttw.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gaaktebbe.sHtML

[Q84] 去除首尾空格
来源：http://www.blog.fanxiaobao.xyz/Article/details/glafjeozy.sHtML

SELECT TRIM(name) FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gjidickex.sHtML

[Q85] 数值取整
来源：http://read.share.fanxiaobao.xyz/Article/details/gpntktqrd.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://baike.fanxiaobao.xyz/Article/details/gguflyzyd.sHtML

[Q86] 读取 JSON 字段
来源：http://read.share.fanxiaobao.xyz/Article/details/gsybhmhej.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://blog.fanxiaobao.xyz/Article/details/gusjiiotf.sHtML

[Q87] JSON 字段做条件
来源：http://blog.fanxiaobao.xyz/Article/details/gyxsuyhav.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://blog.fanxiaobao.xyz/Article/details/gkllqjdrl.sHtML

[Q88] 行转列（条件聚合）
来源：http://3g.fanxiaobao.xyz/Article/details/gbaynpksk.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://read.share.fanxiaobao.xyz/Article/details/goauzqjjg.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gloluarqz.sHtML

[Q89] 判断表是否存在
来源：http://www.share.fanxiaobao.xyz/Article/details/gzdhzjbdh.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://wap.fanxiaobao.xyz/Article/details/gnddhcedw.sHtML

[Q90] 生成序号列
来源：http://baike.fanxiaobao.xyz/Article/details/gjdckvepi.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://mobile.fanxiaobao.xyz/Article/details/gjvpyizne.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gwjejtqdo.sHtML

R. Bash 专题
来源：http://www.blog.fanxiaobao.xyz/Article/details/giypwrfof.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gpfmlhoos.sHtML

[R01] shebang 与严格模式
来源：http://mobile.fanxiaobao.xyz/Article/details/gstegddla.sHtML

#!/usr/bin/env bash
来源：http://mobile.fanxiaobao.xyz/Article/details/gdrplnwsw.sHtML

set -euo pipefail
来源：http://mobile.fanxiaobao.xyz/Article/details/gtvxaxjfo.sHtML

[R02] 变量赋值与使用
来源：http://wap.fanxiaobao.xyz/Article/details/glwoqpiwv.sHtML

name="Tom"; echo "$name"
来源：http://blog.fanxiaobao.xyz/Article/details/glqnxfztn.sHtML

[R03] 只读变量
来源：http://baike.fanxiaobao.xyz/Article/details/gpvczowox.sHtML

readonly PI=3.14
来源：http://mobile.fanxiaobao.xyz/Article/details/gatexuqux.sHtML

[R04] 位置参数
来源：http://read.share.fanxiaobao.xyz/Article/details/gdjzrgomf.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.share.fanxiaobao.xyz/Article/details/ggvxtafwz.sHtML

[R05] 参数默认值
来源：http://blog.fanxiaobao.xyz/Article/details/gvfhtownv.sHtML

name="${1:-default}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggefstjzb.sHtML

[R06] 判断命令是否存在
来源：http://www.blog.fanxiaobao.xyz/Article/details/gprfqsqei.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gfvvlbgpl.sHtML

[R07] if 判断文件
来源：http://3g.fanxiaobao.xyz/Article/details/gqtpcbqsk.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glvhgllwe.sHtML

[R08] 数值比较
来源：http://mobile.fanxiaobao.xyz/Article/details/gkuwwxchl.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://baike.fanxiaobao.xyz/Article/details/gdblhizzd.sHtML

[R09] 字符串比较
来源：http://read.share.fanxiaobao.xyz/Article/details/gciyuuxhl.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://blog.fanxiaobao.xyz/Article/details/gkisegxsf.sHtML

[R10] 正则匹配
来源：http://www.share.fanxiaobao.xyz/Article/details/gfupuumbm.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://3g.fanxiaobao.xyz/Article/details/gflrkudtf.sHtML

[R11] case 多分支
来源：http://mobile.fanxiaobao.xyz/Article/details/glbyjyhmg.sHtML

case "$1" in
来源：http://read.share.fanxiaobao.xyz/Article/details/gzglulyny.sHtML

start) echo "启动" ;;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glghukdca.sHtML

stop)  echo "停止" ;;
来源：http://read.share.fanxiaobao.xyz/Article/details/gmedpqdus.sHtML

*)     echo "未知命令" ;;
来源：http://3g.fanxiaobao.xyz/Article/details/gciroqjqv.sHtML

esac
来源：http://www.share.fanxiaobao.xyz/Article/details/gglwuraxl.sHtML

[R12] for 遍历文件
来源：http://baike.fanxiaobao.xyz/Article/details/gpjhvzmeq.sHtML

for f in *.txt; do echo "$f"; done
来源：http://wap.fanxiaobao.xyz/Article/details/gnmyrperl.sHtML

[R13] for 计数循环
来源：http://blog.fanxiaobao.xyz/Article/details/grozsnsub.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzlsxuvwe.sHtML

[R14] C 风格 for
来源：http://mobile.fanxiaobao.xyz/Article/details/ggvckvmvq.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://3g.fanxiaobao.xyz/Article/details/gdqldemsr.sHtML

[R15] while 逐行读文件
来源：http://wap.fanxiaobao.xyz/Article/details/gpidxyvqt.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gknxgqonh.sHtML

[R16] until 等待条件
来源：http://3g.fanxiaobao.xyz/Article/details/gsbkhfzgd.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gksanqwzb.sHtML

[R17] 数组定义与取值
来源：http://baike.fanxiaobao.xyz/Article/details/gzlzkfhng.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://blog.fanxiaobao.xyz/Article/details/gbrsgkozv.sHtML

[R18] 遍历数组
来源：http://m.share.fanxiaobao.xyz/Article/details/gbcmgkpsd.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://blog.fanxiaobao.xyz/Article/details/gkeqpqraq.sHtML

[R19] 数组长度
来源：http://baike.fanxiaobao.xyz/Article/details/gwoexiuzx.sHtML

echo "${#arr[@]}"
来源：http://baike.fanxiaobao.xyz/Article/details/ggwqeskov.sHtML

[R20] 关联数组（字典）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gogowgqud.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqmarmmja.sHtML

[R21] 字符串长度
来源：http://blog.fanxiaobao.xyz/Article/details/gamjlxnpi.sHtML

echo "${#s}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gllnwywyv.sHtML

[R22] 截取子串
来源：http://www.share.fanxiaobao.xyz/Article/details/giklhdlxh.sHtML

echo "${s:0:5}"
来源：http://baike.fanxiaobao.xyz/Article/details/ghmxwjoyl.sHtML

[R23] 字符串替换
来源：http://www.share.fanxiaobao.xyz/Article/details/gtemtzvmn.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://mobile.fanxiaobao.xyz/Article/details/gyismbchw.sHtML

[R24] 大小写转换
来源：http://wap.fanxiaobao.xyz/Article/details/gogpzeoey.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://blog.fanxiaobao.xyz/Article/details/geduktvqe.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.share.fanxiaobao.xyz/Article/details/gmcvndalo.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gqrgjsfzw.sHtML

[R26] 命令替换
来源：http://blog.fanxiaobao.xyz/Article/details/gqlusuhbr.sHtML

now=$(date +%F); echo "$now"
来源：http://www.blog.fanxiaobao.xyz/Article/details/glvhtcfts.sHtML

[R27] 算术展开
来源：http://mobile.fanxiaobao.xyz/Article/details/gfqygafyt.sHtML

echo $((1 + 2 * 3))
来源：http://3g.fanxiaobao.xyz/Article/details/gferqlcnx.sHtML

[R28] 浮点运算
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdxivsjdp.sHtML

echo "scale=2; 10/3" | bc
来源：http://read.share.fanxiaobao.xyz/Article/details/gadpwcjup.sHtML

[R29] 定义函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gzlihoepn.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.share.fanxiaobao.xyz/Article/details/gxbvpowrk.sHtML

[R30] 函数返回状态码
来源：http://www.share.fanxiaobao.xyz/Article/details/gabauyorp.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzzkppunr.sHtML

[R31] 局部变量
来源：http://blog.fanxiaobao.xyz/Article/details/gfizrcdcr.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gegacxfuq.sHtML

[R32] 参数个数校验
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkjojxzjj.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gvwvorbil.sHtML

[R33] 捕获错误并提示行号
来源：http://read.share.fanxiaobao.xyz/Article/details/gngnsnzrs.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://wap.fanxiaobao.xyz/Article/details/gmkoxfmcb.sHtML

[R34] 退出时清理
来源：http://wap.fanxiaobao.xyz/Article/details/gjndmvial.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.share.fanxiaobao.xyz/Article/details/gwbfrbwqf.sHtML

[R35] 后台执行并等待
来源：http://baike.fanxiaobao.xyz/Article/details/gfbfgzcos.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.share.fanxiaobao.xyz/Article/details/gijzjtymu.sHtML

[R36] 并发执行多个任务
来源：http://m.share.fanxiaobao.xyz/Article/details/gcuazuzna.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://read.share.fanxiaobao.xyz/Article/details/gaqulgdfo.sHtML

[R37] 把输出赋给变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjlifnnpq.sHtML

files=$(ls -1)
来源：http://baike.fanxiaobao.xyz/Article/details/gbevacefo.sHtML

[R38] 管道串联
来源：http://read.share.fanxiaobao.xyz/Article/details/gxsboughj.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.share.fanxiaobao.xyz/Article/details/grjbfisoj.sHtML

[R39] 重定向标准输出与错误
来源：http://read.share.fanxiaobao.xyz/Article/details/gwhxzpcnz.sHtML

cmd > out.log 2>&1
来源：http://mobile.fanxiaobao.xyz/Article/details/glcxwzmnu.sHtML

[R40] 追加写日志
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtvqxhwnt.sHtML

echo "log" >> out.log
来源：http://read.share.fanxiaobao.xyz/Article/details/gdloviymk.sHtML

[R41] 丢弃输出
来源：http://wap.fanxiaobao.xyz/Article/details/grkxptljc.sHtML

cmd >/dev/null 2>&1
来源：http://blog.fanxiaobao.xyz/Article/details/gpqkynbhm.sHtML

[R42] 输入重定向
来源：http://blog.fanxiaobao.xyz/Article/details/gohaemfuy.sHtML

wc -l < a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gurjkrnnp.sHtML

[R43] 按名字查找文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gzetxqohb.sHtML

find . -name "*.log" -type f
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmgpyxxng.sHtML

[R44] 按修改时间查找
来源：http://www.blog.fanxiaobao.xyz/Article/details/gevhrivdz.sHtML

find . -mtime -7 -type f
来源：http://wap.fanxiaobao.xyz/Article/details/gauvxpklp.sHtML

[R45] 批量删除
来源：http://wap.fanxiaobao.xyz/Article/details/gixqdmvea.sHtML


<!-- 参考信息 -->