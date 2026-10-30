代发 wailian999

================================================================================
来源：http://blog.fehbvm.com/Article/details/goyymwbnj.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://3g.fehbvm.com/Article/details/gransrwqh.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/grfrtqbfq.sHtML

[Q01] 创建表
来源：http://baike.zdbjq.cn/Article/details/gvifdeyqy.sHtML

CREATE TABLE users (
来源：http://blog.hesvh.cn/Article/details/ghklcalba.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.fehbvm.com/Article/details/gqnveszdp.sHtML

name VARCHAR(50) NOT NULL,
来源：http://blog.hesvh.cn/Article/details/gbuqlhbys.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.share.hesvh.cn/Article/details/grtcgmtvr.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.blog.zdbjq.cn/Article/details/gabnrhlmq.sHtML

);
来源：http://read.share.hesvh.cn/Article/details/gvzmueefl.sHtML

[Q02] 创建带外键的表
来源：http://www.m.share.fehbvm.com/Article/details/gqagojgjb.sHtML

CREATE TABLE orders (
来源：http://baike.zdbjq.cn/Article/details/gkqgnrtcw.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.hesvh.cn/Article/details/gtntvwssb.sHtML

user_id INT NOT NULL,
来源：http://blog.fehbvm.com/Article/details/groqwmwyq.sHtML

amount DECIMAL(10, 2),
来源：http://blog.zdbjq.cn/Article/details/glpcdadji.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://3g.zdbjq.cn/Article/details/gigfikjmi.sHtML

);
来源：http://3g.zdbjq.cn/Article/details/gqoofnuoy.sHtML

[Q03] 增加列
来源：http://blog.fehbvm.com/Article/details/gndpptmky.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://blog.zdbjq.cn/Article/details/grnmrkgaz.sHtML

[Q04] 修改列类型
来源：http://baike.fehbvm.com/Article/details/gscclzlmy.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://wap.zdbjq.cn/Article/details/gekcvtsaz.sHtML

[Q05] 重命名列
来源：http://m.share.fehbvm.com/Article/details/gpdawxuqe.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.share.zdbjq.cn/Article/details/gpxtfqmuy.sHtML

[Q06] 删除列
来源：http://mobile.hesvh.cn/Article/details/gllpzdikm.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://mobile.hesvh.cn/Article/details/gntthklyj.sHtML

[Q07] 删除表
来源：http://www.share.zdbjq.cn/Article/details/gxjydbccd.sHtML

DROP TABLE IF EXISTS orders;
来源：http://m.share.zdbjq.cn/Article/details/gupgluaaz.sHtML

[Q08] 创建普通索引
来源：http://blog.fehbvm.com/Article/details/grhugzwfz.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://mobile.zdbjq.cn/Article/details/gvhkqaznf.sHtML

[Q09] 创建唯一索引
来源：http://www.m.share.zdbjq.cn/Article/details/gzekmrxqg.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://mobile.hesvh.cn/Article/details/gyozdhher.sHtML

[Q10] 插入单行
来源：http://baike.hesvh.cn/Article/details/gdpwkjvst.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.m.share.fehbvm.com/Article/details/gdbjhcduj.sHtML

[Q11] 一次插入多行
来源：http://read.share.fehbvm.com/Article/details/gmhkfriqt.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.share.zdbjq.cn/Article/details/gvbcjjcvd.sHtML

[Q12] 插入后取自增 ID
来源：http://www.m.share.hesvh.cn/Article/details/gtuodjyzn.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.share.fehbvm.com/Article/details/giyxcchvl.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://m.share.zdbjq.cn/Article/details/gxsctseso.sHtML

[Q13] 忽略重复插入
来源：http://3g.fehbvm.com/Article/details/gsylilkdp.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.blog.hesvh.cn/Article/details/gimxpeyjd.sHtML

[Q14] 存在则更新（upsert）
来源：http://wap.fehbvm.com/Article/details/gcaxdmulo.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.blog.zdbjq.cn/Article/details/gcvlykiol.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://read.share.zdbjq.cn/Article/details/gxosmijmi.sHtML

[Q15] 查询全部
来源：http://read.share.hesvh.cn/Article/details/gmqubzpsm.sHtML

SELECT * FROM users;
来源：http://www.blog.fehbvm.com/Article/details/glltajnyy.sHtML

[Q16] 查询指定列
来源：http://wap.hesvh.cn/Article/details/gfyvdstnp.sHtML

SELECT id, name FROM users;
来源：http://baike.zdbjq.cn/Article/details/gyvtubhcd.sHtML

[Q17] 条件查询
来源：http://read.share.fehbvm.com/Article/details/gfjldgmlc.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://mobile.zdbjq.cn/Article/details/gkmcbgdzq.sHtML

[Q18] 模糊匹配
来源：http://www.blog.hesvh.cn/Article/details/gjkmvenwc.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://mobile.hesvh.cn/Article/details/gyigtykcf.sHtML

[Q19] 范围查询
来源：http://www.m.share.fehbvm.com/Article/details/gfqfjkpdo.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.m.share.hesvh.cn/Article/details/gvaciknca.sHtML

[Q20] IN 列表
来源：http://mobile.zdbjq.cn/Article/details/gqgcfkfkc.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://blog.hesvh.cn/Article/details/gvkwqdtxr.sHtML

[Q21] 空值判断
来源：http://blog.fehbvm.com/Article/details/gyoltgnba.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://read.share.fehbvm.com/Article/details/gsublkaah.sHtML

[Q22] 排序
来源：http://m.share.hesvh.cn/Article/details/ghymneojf.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://mobile.hesvh.cn/Article/details/gwwwrpvbu.sHtML

[Q23] 分页
来源：http://mobile.fehbvm.com/Article/details/gipzivswh.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://3g.zdbjq.cn/Article/details/glzrubtup.sHtML

[Q24] 去重
来源：http://www.blog.hesvh.cn/Article/details/gogypybaz.sHtML

SELECT DISTINCT city FROM users;
来源：http://3g.hesvh.cn/Article/details/gwvkcpqgs.sHtML

[Q25] 只取前 N 条
来源：http://read.share.fehbvm.com/Article/details/gjrmornjk.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://read.share.zdbjq.cn/Article/details/gyjvsbire.sHtML

[Q26] 计数
来源：http://www.share.zdbjq.cn/Article/details/gckoybnzi.sHtML

SELECT COUNT(*) FROM users;
来源：http://baike.fehbvm.com/Article/details/gmnjpvici.sHtML

[Q27] 条件计数
来源：http://baike.hesvh.cn/Article/details/gewzrdxrl.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gqnqhreoe.sHtML

[Q28] 求和与平均
来源：http://m.share.fehbvm.com/Article/details/gyteolbat.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.blog.hesvh.cn/Article/details/gnsrmpcqn.sHtML

[Q29] 最大最小值
来源：http://www.blog.zdbjq.cn/Article/details/gthmmefck.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://blog.zdbjq.cn/Article/details/gdqdqafrz.sHtML

[Q30] 分组统计
来源：http://wap.fehbvm.com/Article/details/gpqqefriz.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.m.share.hesvh.cn/Article/details/grmldqpts.sHtML

[Q31] 分组后过滤
来源：http://www.m.share.zdbjq.cn/Article/details/gxdzpehds.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.blog.zdbjq.cn/Article/details/gguhmcjgq.sHtML

[Q32] 分组拼接字符串
来源：http://wap.zdbjq.cn/Article/details/giuheulrk.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.m.share.fehbvm.com/Article/details/gxwfcaebl.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.m.share.fehbvm.com/Article/details/gbsivnkpk.sHtML

[Q33] 多列分组
来源：http://www.m.share.hesvh.cn/Article/details/gzbosyegt.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.blog.fehbvm.com/Article/details/gdultfepx.sHtML

[Q34] 每组取第一条
来源：http://m.share.fehbvm.com/Article/details/ggxzclkha.sHtML

SELECT * FROM (
来源：http://www.blog.zdbjq.cn/Article/details/gvbmsfyyg.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://mobile.fehbvm.com/Article/details/gebahixid.sHtML

) t WHERE rn = 1;
来源：http://m.share.fehbvm.com/Article/details/gmwrpdlkw.sHtML

[Q35] 内连接
来源：http://baike.hesvh.cn/Article/details/gegnpintc.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://mobile.zdbjq.cn/Article/details/gykzuxyfd.sHtML

[Q36] 左连接
来源：http://baike.zdbjq.cn/Article/details/gfizbhdak.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://wap.zdbjq.cn/Article/details/grbwwkzqy.sHtML

[Q37] 右连接
来源：http://3g.hesvh.cn/Article/details/gocgqpzxy.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://baike.fehbvm.com/Article/details/gqwagkpbw.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://read.share.hesvh.cn/Article/details/gopaluwca.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.share.hesvh.cn/Article/details/gzmzsbvwg.sHtML

[Q39] 自连接（查上下级）
来源：http://www.share.zdbjq.cn/Article/details/gjucbkffs.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.m.share.zdbjq.cn/Article/details/gpwbmyuma.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://m.share.zdbjq.cn/Article/details/gzemhjyay.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://wap.fehbvm.com/Article/details/gdpzpikgf.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://m.share.zdbjq.cn/Article/details/gtimbovft.sHtML

[Q41] 多表连接
来源：http://3g.zdbjq.cn/Article/details/gtsseddcs.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.m.share.hesvh.cn/Article/details/ghjbbbqds.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.share.hesvh.cn/Article/details/gzjnqfpvj.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://baike.hesvh.cn/Article/details/gyaghbxuw.sHtML

[Q42] 连接条件附加过滤
来源：http://mobile.hesvh.cn/Article/details/gmvfwrbrh.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.m.share.fehbvm.com/Article/details/givdkfdzr.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://read.share.fehbvm.com/Article/details/gxcxurovg.sHtML

[Q43] 标量子查询
来源：http://wap.fehbvm.com/Article/details/gonjhhjvm.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.blog.hesvh.cn/Article/details/gzdzppwsy.sHtML

[Q44] IN 子查询
来源：http://wap.hesvh.cn/Article/details/gdmzegmxh.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://m.share.fehbvm.com/Article/details/gyrxlmzjd.sHtML

[Q45] EXISTS 判断存在
来源：http://www.m.share.zdbjq.cn/Article/details/gnrewmcbe.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.hesvh.cn/Article/details/glwdiqppu.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://baike.zdbjq.cn/Article/details/gcsqjutla.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.fehbvm.com/Article/details/gemhzszqv.sHtML

[Q47] 与平均值比较
来源：http://mobile.hesvh.cn/Article/details/gocafjqpy.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://read.share.hesvh.cn/Article/details/gwczveqry.sHtML

[Q48] CTE 公用表表达式
来源：http://blog.hesvh.cn/Article/details/gaovenkvz.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.blog.fehbvm.com/Article/details/gxudurbwz.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.blog.zdbjq.cn/Article/details/gxhudwmho.sHtML

[Q49] 更新单行
来源：http://mobile.zdbjq.cn/Article/details/gkmoeudwb.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://mobile.zdbjq.cn/Article/details/gqatesdzg.sHtML

[Q50] 批量更新
来源：http://blog.fehbvm.com/Article/details/gqqednsvq.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://m.share.hesvh.cn/Article/details/gejfrzjlw.sHtML

[Q51] 用子查询更新
来源：http://m.share.fehbvm.com/Article/details/guowwspfr.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://read.share.zdbjq.cn/Article/details/gjtqbsixu.sHtML

[Q52] 删除指定行
来源：http://www.m.share.zdbjq.cn/Article/details/gmojsmgvh.sHtML

DELETE FROM users WHERE id = 10;
来源：http://read.share.zdbjq.cn/Article/details/gvqbbkboi.sHtML

[Q53] 按条件删除
来源：http://blog.zdbjq.cn/Article/details/glcqaswoc.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://read.share.zdbjq.cn/Article/details/ghfkictjw.sHtML

[Q54] 清空表
来源：http://m.share.fehbvm.com/Article/details/grpikyong.sHtML

TRUNCATE TABLE logs;
来源：http://read.share.zdbjq.cn/Article/details/gxhbxuefi.sHtML

[Q55] 排名（并列占位）
来源：http://blog.fehbvm.com/Article/details/gpdvcvgct.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://3g.fehbvm.com/Article/details/gviewyfcs.sHtML

[Q56] 密集排名（并列不占位）
来源：http://mobile.fehbvm.com/Article/details/gzcswozti.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://blog.zdbjq.cn/Article/details/gunzcfhcz.sHtML

[Q57] 行号
来源：http://3g.fehbvm.com/Article/details/gehgcsukl.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://m.share.hesvh.cn/Article/details/gyqsultab.sHtML

[Q58] 累计求和
来源：http://blog.zdbjq.cn/Article/details/gcodvsrdc.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://mobile.hesvh.cn/Article/details/germbukqd.sHtML

[Q59] 分组内累计
来源：http://mobile.zdbjq.cn/Article/details/gpohxmxer.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://blog.fehbvm.com/Article/details/gjljajpbi.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.share.hesvh.cn/Article/details/gdmvfbinx.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.blog.fehbvm.com/Article/details/gmsnpnmgu.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://baike.fehbvm.com/Article/details/guiupkqkn.sHtML

[Q61] 移动平均
来源：http://blog.zdbjq.cn/Article/details/giupawtqy.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://baike.hesvh.cn/Article/details/gplqqvsln.sHtML

[Q62] 分组占比
来源：http://www.blog.zdbjq.cn/Article/details/gqsyjjbpe.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://m.share.hesvh.cn/Article/details/gdowwlczu.sHtML

[Q63] 开启事务
来源：http://read.share.zdbjq.cn/Article/details/givyntifa.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://blog.fehbvm.com/Article/details/gmpyiylal.sHtML

[Q64] 提交事务
来源：http://blog.hesvh.cn/Article/details/gvlietzfd.sHtML

COMMIT;
来源：http://m.share.fehbvm.com/Article/details/gjsfylbdw.sHtML

[Q65] 回滚事务
来源：http://www.share.hesvh.cn/Article/details/gxmxoqcaf.sHtML

ROLLBACK;
来源：http://baike.zdbjq.cn/Article/details/ghggpaiok.sHtML

[Q66] 行锁查询
来源：http://www.share.fehbvm.com/Article/details/ggxpbkaos.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://baike.hesvh.cn/Article/details/gkzeuualt.sHtML

[Q67] 设置隔离级别
来源：http://mobile.fehbvm.com/Article/details/gqbcnwttw.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://blog.zdbjq.cn/Article/details/gdbkmbkrj.sHtML

[Q68] 保存点
来源：http://blog.zdbjq.cn/Article/details/grcoqkevu.sHtML

SAVEPOINT sp1;
来源：http://www.share.zdbjq.cn/Article/details/gbpolnpky.sHtML

ROLLBACK TO sp1;
来源：http://www.share.zdbjq.cn/Article/details/ghpwnylxk.sHtML

[Q69] 查看执行计划
来源：http://blog.fehbvm.com/Article/details/gtxrcjpyp.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://baike.zdbjq.cn/Article/details/gmqfxohpr.sHtML

[Q70] 更新统计信息
来源：http://www.blog.hesvh.cn/Article/details/gvdissiab.sHtML

ANALYZE TABLE users;
来源：http://www.m.share.zdbjq.cn/Article/details/gydkyuysr.sHtML

[Q71] 查看建表语句
来源：http://m.share.fehbvm.com/Article/details/gmikuzgio.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://m.share.fehbvm.com/Article/details/gcccnyjsp.sHtML

[Q72] 查看索引
来源：http://www.blog.hesvh.cn/Article/details/ggejzoyeh.sHtML

SHOW INDEX FROM users;
来源：http://mobile.fehbvm.com/Article/details/gzcifsilg.sHtML

[Q73] 查看表状态
来源：http://www.blog.zdbjq.cn/Article/details/gqpjhdvot.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://read.share.hesvh.cn/Article/details/gnswcntvv.sHtML

[Q74] 强制使用索引
来源：http://read.share.zdbjq.cn/Article/details/grovtmfii.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://3g.zdbjq.cn/Article/details/geqpiksbc.sHtML

[Q75] 日期格式化
来源：http://wap.fehbvm.com/Article/details/gmlodqutr.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://blog.hesvh.cn/Article/details/gvpwrecmc.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://m.share.fehbvm.com/Article/details/geelqfwoc.sHtML

[Q76] 按天统计
来源：http://www.share.zdbjq.cn/Article/details/gnvwzyzba.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.share.fehbvm.com/Article/details/gedbwokly.sHtML

[Q77] 时间加减
来源：http://3g.hesvh.cn/Article/details/gxibetsre.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://m.share.zdbjq.cn/Article/details/groyhyqos.sHtML

[Q78] 当前时间
来源：http://wap.fehbvm.com/Article/details/gvzuxmzgg.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://mobile.hesvh.cn/Article/details/giqykgwvf.sHtML

[Q79] 字符串拼接
来源：http://baike.fehbvm.com/Article/details/gvfzkpeoc.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.m.share.hesvh.cn/Article/details/gwqjoijaw.sHtML

[Q80] 字符串截取
来源：http://wap.hesvh.cn/Article/details/gezgfqgvs.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://baike.zdbjq.cn/Article/details/goybolyxe.sHtML

[Q81] 字符串替换
来源：http://wap.fehbvm.com/Article/details/gabadqklb.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.share.fehbvm.com/Article/details/gjqgluump.sHtML

[Q82] 字符长度与字节长度
来源：http://baike.fehbvm.com/Article/details/glpuzsbzh.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://read.share.hesvh.cn/Article/details/gxhluhaev.sHtML

[Q83] 大小写转换
来源：http://read.share.zdbjq.cn/Article/details/gbqevaioo.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gobmjxyiv.sHtML

[Q84] 去除首尾空格
来源：http://www.share.fehbvm.com/Article/details/gdeonfkqe.sHtML

SELECT TRIM(name) FROM users;
来源：http://blog.fehbvm.com/Article/details/gkxoifhye.sHtML

[Q85] 数值取整
来源：http://mobile.hesvh.cn/Article/details/gxvtxljni.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://blog.hesvh.cn/Article/details/grzjgnmzk.sHtML

[Q86] 读取 JSON 字段
来源：http://www.share.hesvh.cn/Article/details/gmprhqnag.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.m.share.fehbvm.com/Article/details/gfxljmndk.sHtML

[Q87] JSON 字段做条件
来源：http://wap.hesvh.cn/Article/details/gfrgktucx.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.m.share.zdbjq.cn/Article/details/gqlgfuzds.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.blog.zdbjq.cn/Article/details/gbjzkocrv.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.m.share.hesvh.cn/Article/details/gvxfpdvcl.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://blog.fehbvm.com/Article/details/gkqnqccll.sHtML

[Q89] 判断表是否存在
来源：http://wap.fehbvm.com/Article/details/gykomwypg.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://read.share.zdbjq.cn/Article/details/ghevwkmcg.sHtML

[Q90] 生成序号列
来源：http://blog.zdbjq.cn/Article/details/gpadythbe.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://3g.hesvh.cn/Article/details/gsowybtvx.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gpftxiinw.sHtML

R. Bash 专题
来源：http://blog.hesvh.cn/Article/details/gnhswyijy.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gpgvwepou.sHtML

[R01] shebang 与严格模式
来源：http://blog.zdbjq.cn/Article/details/gjynujilg.sHtML

#!/usr/bin/env bash
来源：http://mobile.fehbvm.com/Article/details/gofewobbw.sHtML

set -euo pipefail
来源：http://www.share.hesvh.cn/Article/details/gmhagqtax.sHtML

[R02] 变量赋值与使用
来源：http://wap.zdbjq.cn/Article/details/grkvpmckf.sHtML

name="Tom"; echo "$name"
来源：http://read.share.hesvh.cn/Article/details/guiachuzr.sHtML

[R03] 只读变量
来源：http://blog.fehbvm.com/Article/details/gpimxixoj.sHtML

readonly PI=3.14
来源：http://3g.fehbvm.com/Article/details/gngzvfwzl.sHtML

[R04] 位置参数
来源：http://3g.hesvh.cn/Article/details/gohmdmxws.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.m.share.fehbvm.com/Article/details/gvmscijin.sHtML

[R05] 参数默认值
来源：http://www.m.share.hesvh.cn/Article/details/gamanybyl.sHtML

name="${1:-default}"
来源：http://blog.hesvh.cn/Article/details/gwddmwgxl.sHtML

[R06] 判断命令是否存在
来源：http://wap.fehbvm.com/Article/details/gjojqujzo.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://baike.zdbjq.cn/Article/details/gutbyuzwt.sHtML

[R07] if 判断文件
来源：http://3g.hesvh.cn/Article/details/gkdghmydc.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://wap.zdbjq.cn/Article/details/gqgchsrrg.sHtML

[R08] 数值比较
来源：http://read.share.fehbvm.com/Article/details/girmpfled.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://3g.hesvh.cn/Article/details/guhcvdjim.sHtML

[R09] 字符串比较
来源：http://wap.fehbvm.com/Article/details/gyotowfwu.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://m.share.hesvh.cn/Article/details/geblpubgi.sHtML

[R10] 正则匹配
来源：http://baike.hesvh.cn/Article/details/gohwaqxqa.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.m.share.zdbjq.cn/Article/details/gwrvqpkpe.sHtML

[R11] case 多分支
来源：http://www.share.zdbjq.cn/Article/details/gjnawxmjx.sHtML

case "$1" in
来源：http://www.blog.hesvh.cn/Article/details/ggubdyrls.sHtML

start) echo "启动" ;;
来源：http://3g.zdbjq.cn/Article/details/glkkvxiqf.sHtML

stop)  echo "停止" ;;
来源：http://blog.hesvh.cn/Article/details/gdpruavjq.sHtML

*)     echo "未知命令" ;;
来源：http://read.share.hesvh.cn/Article/details/ghcrgzlak.sHtML

esac
来源：http://www.blog.hesvh.cn/Article/details/goqctweee.sHtML

[R12] for 遍历文件
来源：http://blog.fehbvm.com/Article/details/gdzywjsih.sHtML

for f in *.txt; do echo "$f"; done
来源：http://3g.hesvh.cn/Article/details/grqvtkaab.sHtML

[R13] for 计数循环
来源：http://m.share.fehbvm.com/Article/details/gwqktcobg.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.share.zdbjq.cn/Article/details/gbuujhzrc.sHtML

[R14] C 风格 for
来源：http://www.m.share.fehbvm.com/Article/details/gkjogzvlc.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://read.share.fehbvm.com/Article/details/gkvpbieok.sHtML

[R15] while 逐行读文件
来源：http://blog.fehbvm.com/Article/details/gjyrzccfd.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://mobile.hesvh.cn/Article/details/gpwfopnrb.sHtML

[R16] until 等待条件
来源：http://read.share.hesvh.cn/Article/details/gzqljuidn.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.m.share.fehbvm.com/Article/details/goruglxlf.sHtML

[R17] 数组定义与取值
来源：http://mobile.hesvh.cn/Article/details/glidmkomo.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://baike.fehbvm.com/Article/details/gnqoyabmn.sHtML

[R18] 遍历数组
来源：http://3g.hesvh.cn/Article/details/gsefvtisz.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.share.fehbvm.com/Article/details/gwypdnrrm.sHtML

[R19] 数组长度
来源：http://www.share.hesvh.cn/Article/details/gumvqwmzk.sHtML

echo "${#arr[@]}"
来源：http://wap.zdbjq.cn/Article/details/glgokabvc.sHtML

[R20] 关联数组（字典）
来源：http://www.share.hesvh.cn/Article/details/gxdskacuu.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://3g.zdbjq.cn/Article/details/ghiyhecsz.sHtML

[R21] 字符串长度
来源：http://read.share.zdbjq.cn/Article/details/gkrpknubq.sHtML

echo "${#s}"
来源：http://mobile.zdbjq.cn/Article/details/gzxcjgfuf.sHtML

[R22] 截取子串
来源：http://blog.fehbvm.com/Article/details/gfrefdxnq.sHtML

echo "${s:0:5}"
来源：http://3g.hesvh.cn/Article/details/gzqpczauc.sHtML

[R23] 字符串替换
来源：http://wap.hesvh.cn/Article/details/goivdlcvt.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://3g.fehbvm.com/Article/details/gfgigevbq.sHtML

[R24] 大小写转换
来源：http://www.share.zdbjq.cn/Article/details/gmduwdrfx.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://read.share.fehbvm.com/Article/details/gbvtndxey.sHtML

[R25] 去后缀 / 去前缀
来源：http://baike.hesvh.cn/Article/details/gycoejcin.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://baike.zdbjq.cn/Article/details/gmolmvzpz.sHtML

[R26] 命令替换
来源：http://mobile.zdbjq.cn/Article/details/ghidkfoph.sHtML

now=$(date +%F); echo "$now"
来源：http://www.share.hesvh.cn/Article/details/gvllwzihr.sHtML

[R27] 算术展开
来源：http://www.blog.fehbvm.com/Article/details/gjyyzeeux.sHtML

echo $((1 + 2 * 3))
来源：http://3g.zdbjq.cn/Article/details/gjaatnswh.sHtML

[R28] 浮点运算
来源：http://www.blog.hesvh.cn/Article/details/gqsolgxnp.sHtML

echo "scale=2; 10/3" | bc
来源：http://baike.zdbjq.cn/Article/details/gecyfcmhh.sHtML

[R29] 定义函数
来源：http://baike.fehbvm.com/Article/details/gqjqrcyrq.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://3g.fehbvm.com/Article/details/glysfjtwb.sHtML

[R30] 函数返回状态码
来源：http://www.m.share.zdbjq.cn/Article/details/gzzrwfnzl.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://3g.hesvh.cn/Article/details/gcofqzctv.sHtML

[R31] 局部变量
来源：http://www.blog.fehbvm.com/Article/details/gyzebrfzg.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gpvihhzoh.sHtML

[R32] 参数个数校验
来源：http://www.share.hesvh.cn/Article/details/ginuupnqe.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://blog.zdbjq.cn/Article/details/gbigynlge.sHtML

[R33] 捕获错误并提示行号
来源：http://read.share.hesvh.cn/Article/details/gmftkvrws.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://read.share.fehbvm.com/Article/details/ggmbbfrme.sHtML

[R34] 退出时清理
来源：http://wap.zdbjq.cn/Article/details/gfoxcuhay.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://baike.hesvh.cn/Article/details/gbedoncqv.sHtML

[R35] 后台执行并等待
来源：http://mobile.hesvh.cn/Article/details/gpykbumbd.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://3g.hesvh.cn/Article/details/gdnmvtohs.sHtML

[R36] 并发执行多个任务
来源：http://mobile.hesvh.cn/Article/details/gfpnwpoqe.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.m.share.hesvh.cn/Article/details/gnincztum.sHtML

[R37] 把输出赋给变量
来源：http://www.m.share.fehbvm.com/Article/details/gwdlygeho.sHtML

files=$(ls -1)
来源：http://3g.fehbvm.com/Article/details/grywwpmff.sHtML

[R38] 管道串联
来源：http://baike.zdbjq.cn/Article/details/gkbvzajpo.sHtML

cat a.txt | grep -i error | wc -l
来源：http://baike.fehbvm.com/Article/details/gonarflsb.sHtML

[R39] 重定向标准输出与错误
来源：http://blog.fehbvm.com/Article/details/gsrwcivpf.sHtML

cmd > out.log 2>&1
来源：http://www.m.share.hesvh.cn/Article/details/ggzohqygc.sHtML

[R40] 追加写日志
来源：http://m.share.hesvh.cn/Article/details/gwndmqdbj.sHtML

echo "log" >> out.log
来源：http://www.m.share.fehbvm.com/Article/details/gdtgmbehh.sHtML

[R41] 丢弃输出
来源：http://www.m.share.hesvh.cn/Article/details/grpnfiyuz.sHtML

cmd >/dev/null 2>&1
来源：http://baike.zdbjq.cn/Article/details/gqoqgjthu.sHtML

[R42] 输入重定向
来源：http://mobile.hesvh.cn/Article/details/gtxzfveix.sHtML

wc -l < a.txt
来源：http://read.share.zdbjq.cn/Article/details/gabxrzfps.sHtML

[R43] 按名字查找文件
来源：http://wap.zdbjq.cn/Article/details/gunbmavna.sHtML


<!-- 参考信息 -->