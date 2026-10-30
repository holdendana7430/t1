代发 wailian999

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqmnfphaw.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://blog.fanxiaobao.xyz/Article/details/gxqsjpzey.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gelqaqqjq.sHtML

[Q01] 创建表
来源：http://blog.fanxiaobao.xyz/Article/details/gqkvfskxw.sHtML

CREATE TABLE users (
来源：http://mobile.fanxiaobao.xyz/Article/details/gvamgzxtz.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.fanxiaobao.xyz/Article/details/gjzfmjebb.sHtML

name VARCHAR(50) NOT NULL,
来源：http://mobile.fanxiaobao.xyz/Article/details/gvfnwykuv.sHtML

email VARCHAR(100) UNIQUE,
来源：http://blog.fanxiaobao.xyz/Article/details/gmqxltozv.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://baike.fanxiaobao.xyz/Article/details/gfaejqflq.sHtML

);
来源：http://baike.fanxiaobao.xyz/Article/details/gfdqarzyj.sHtML

[Q02] 创建带外键的表
来源：http://read.share.fanxiaobao.xyz/Article/details/glfuemlmw.sHtML

CREATE TABLE orders (
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfiyvllhe.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.fanxiaobao.xyz/Article/details/gdcohfazy.sHtML

user_id INT NOT NULL,
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbnhcldky.sHtML

amount DECIMAL(10, 2),
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkqxzsprj.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://read.share.fanxiaobao.xyz/Article/details/gkmlwldgw.sHtML

);
来源：http://3g.fanxiaobao.xyz/Article/details/gykxmndjs.sHtML

[Q03] 增加列
来源：http://www.share.fanxiaobao.xyz/Article/details/geyhqsohw.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://baike.fanxiaobao.xyz/Article/details/gcsdbcuog.sHtML

[Q04] 修改列类型
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnxlglcga.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://baike.fanxiaobao.xyz/Article/details/gekycqtxk.sHtML

[Q05] 重命名列
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxdpviqks.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://3g.fanxiaobao.xyz/Article/details/gfkvgcvwo.sHtML

[Q06] 删除列
来源：http://www.share.fanxiaobao.xyz/Article/details/gxxmdiosf.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://blog.fanxiaobao.xyz/Article/details/gbvgkvkyz.sHtML

[Q07] 删除表
来源：http://3g.fanxiaobao.xyz/Article/details/ggakcmwkb.sHtML

DROP TABLE IF EXISTS orders;
来源：http://blog.fanxiaobao.xyz/Article/details/gwkgrpoeh.sHtML

[Q08] 创建普通索引
来源：http://blog.fanxiaobao.xyz/Article/details/gbtavbrgg.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://mobile.fanxiaobao.xyz/Article/details/gzqsfjwir.sHtML

[Q09] 创建唯一索引
来源：http://mobile.fanxiaobao.xyz/Article/details/gkyvjojfv.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.share.fanxiaobao.xyz/Article/details/gwgfbfyck.sHtML

[Q10] 插入单行
来源：http://blog.fanxiaobao.xyz/Article/details/gagmrwlba.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://read.share.fanxiaobao.xyz/Article/details/gkmnjeibp.sHtML

[Q11] 一次插入多行
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpxxpievw.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.blog.fanxiaobao.xyz/Article/details/glxomkvaj.sHtML

[Q12] 插入后取自增 ID
来源：http://mobile.fanxiaobao.xyz/Article/details/gdmjlhwxv.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.m.share.fanxiaobao.xyz/Article/details/garmusbah.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://m.share.fanxiaobao.xyz/Article/details/gllrpgavx.sHtML

[Q13] 忽略重复插入
来源：http://www.share.fanxiaobao.xyz/Article/details/ggebsfvnq.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzzsrwcfd.sHtML

[Q14] 存在则更新（upsert）
来源：http://3g.fanxiaobao.xyz/Article/details/gyvkcdtai.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqixjnmea.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://mobile.fanxiaobao.xyz/Article/details/ggkvobjlp.sHtML

[Q15] 查询全部
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwexrvujw.sHtML

SELECT * FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gqodkfpjs.sHtML

[Q16] 查询指定列
来源：http://baike.fanxiaobao.xyz/Article/details/gzmxxiwny.sHtML

SELECT id, name FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gmavqkjsj.sHtML

[Q17] 条件查询
来源：http://wap.fanxiaobao.xyz/Article/details/gasngsfdg.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.share.fanxiaobao.xyz/Article/details/gspisjonl.sHtML

[Q18] 模糊匹配
来源：http://baike.fanxiaobao.xyz/Article/details/gbaqtuxpg.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://mobile.fanxiaobao.xyz/Article/details/gjpjfalsd.sHtML

[Q19] 范围查询
来源：http://wap.fanxiaobao.xyz/Article/details/gjjkmdwck.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://baike.fanxiaobao.xyz/Article/details/gtmkpkchs.sHtML

[Q20] IN 列表
来源：http://blog.fanxiaobao.xyz/Article/details/ginxctssi.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://wap.fanxiaobao.xyz/Article/details/gzmookzkc.sHtML

[Q21] 空值判断
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghksvsinw.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://baike.fanxiaobao.xyz/Article/details/gvuxtywll.sHtML

[Q22] 排序
来源：http://wap.fanxiaobao.xyz/Article/details/gnrrkmmci.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.share.fanxiaobao.xyz/Article/details/gizamyxig.sHtML

[Q23] 分页
来源：http://www.blog.fanxiaobao.xyz/Article/details/gahvhskgi.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://baike.fanxiaobao.xyz/Article/details/grxodshml.sHtML

[Q24] 去重
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvspgykkf.sHtML

SELECT DISTINCT city FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gbffgxcmv.sHtML

[Q25] 只取前 N 条
来源：http://www.blog.fanxiaobao.xyz/Article/details/gznjqhuct.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.blog.fanxiaobao.xyz/Article/details/gltsqufjm.sHtML

[Q26] 计数
来源：http://baike.fanxiaobao.xyz/Article/details/ggdpkdvup.sHtML

SELECT COUNT(*) FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gtgihxuda.sHtML

[Q27] 条件计数
来源：http://read.share.fanxiaobao.xyz/Article/details/gbbjbkylm.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gudfbvxli.sHtML

[Q28] 求和与平均
来源：http://www.share.fanxiaobao.xyz/Article/details/goeigygqd.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://read.share.fanxiaobao.xyz/Article/details/gjnzltocf.sHtML

[Q29] 最大最小值
来源：http://m.share.fanxiaobao.xyz/Article/details/gosdssoqr.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gefxjlchp.sHtML

[Q30] 分组统计
来源：http://blog.fanxiaobao.xyz/Article/details/gvcbizbxi.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://wap.fanxiaobao.xyz/Article/details/gmmzrssiv.sHtML

[Q31] 分组后过滤
来源：http://3g.fanxiaobao.xyz/Article/details/gtasrnehi.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://wap.fanxiaobao.xyz/Article/details/gfiwuezwe.sHtML

[Q32] 分组拼接字符串
来源：http://wap.fanxiaobao.xyz/Article/details/gdvtrvpsr.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://m.share.fanxiaobao.xyz/Article/details/gqqythwtn.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://m.share.fanxiaobao.xyz/Article/details/gjkrxfvwc.sHtML

[Q33] 多列分组
来源：http://read.share.fanxiaobao.xyz/Article/details/gvjtetvrl.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://read.share.fanxiaobao.xyz/Article/details/gpzmokmgy.sHtML

[Q34] 每组取第一条
来源：http://www.share.fanxiaobao.xyz/Article/details/gadmzxajs.sHtML

SELECT * FROM (
来源：http://mobile.fanxiaobao.xyz/Article/details/gupuzyaxa.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://m.share.fanxiaobao.xyz/Article/details/gskmrlmqa.sHtML

) t WHERE rn = 1;
来源：http://m.share.fanxiaobao.xyz/Article/details/gfkadzufw.sHtML

[Q35] 内连接
来源：http://wap.fanxiaobao.xyz/Article/details/gejqscgye.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://3g.fanxiaobao.xyz/Article/details/ghvredpeh.sHtML

[Q36] 左连接
来源：http://blog.fanxiaobao.xyz/Article/details/gtzydugaq.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://mobile.fanxiaobao.xyz/Article/details/gzsngxtuj.sHtML

[Q37] 右连接
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqzikfseb.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://read.share.fanxiaobao.xyz/Article/details/gigklswyn.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://read.share.fanxiaobao.xyz/Article/details/gocpthmmy.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gubsmtrcz.sHtML

[Q39] 自连接（查上下级）
来源：http://m.share.fanxiaobao.xyz/Article/details/gjlauviru.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://mobile.fanxiaobao.xyz/Article/details/gwdoorsmn.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://baike.fanxiaobao.xyz/Article/details/gbnzcosax.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://mobile.fanxiaobao.xyz/Article/details/gqrhiceof.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://read.share.fanxiaobao.xyz/Article/details/gvobooqhg.sHtML

[Q41] 多表连接
来源：http://3g.fanxiaobao.xyz/Article/details/gvwfqmvsw.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.blog.fanxiaobao.xyz/Article/details/guaapsgnm.sHtML

JOIN users u ON u.id = o.user_id
来源：http://mobile.fanxiaobao.xyz/Article/details/gqfyvvlly.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://m.share.fanxiaobao.xyz/Article/details/gbqokdyxo.sHtML

[Q42] 连接条件附加过滤
来源：http://mobile.fanxiaobao.xyz/Article/details/gkbmwcjia.sHtML

SELECT u.name, o.amount FROM users u
来源：http://mobile.fanxiaobao.xyz/Article/details/gwzmuhgop.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://wap.fanxiaobao.xyz/Article/details/guenkdcik.sHtML

[Q43] 标量子查询
来源：http://read.share.fanxiaobao.xyz/Article/details/gsmohpvgd.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://mobile.fanxiaobao.xyz/Article/details/gjuyeeddm.sHtML

[Q44] IN 子查询
来源：http://wap.fanxiaobao.xyz/Article/details/gntncfpzj.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://m.share.fanxiaobao.xyz/Article/details/gyeoggyxa.sHtML

[Q45] EXISTS 判断存在
来源：http://www.m.share.fanxiaobao.xyz/Article/details/govxhyoav.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.fanxiaobao.xyz/Article/details/gkbyidsfr.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbmxfgmdb.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.fanxiaobao.xyz/Article/details/gfrakivel.sHtML

[Q47] 与平均值比较
来源：http://baike.fanxiaobao.xyz/Article/details/gttreybui.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://wap.fanxiaobao.xyz/Article/details/gpnqkdsbv.sHtML

[Q48] CTE 公用表表达式
来源：http://read.share.fanxiaobao.xyz/Article/details/gvxobalqg.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://blog.fanxiaobao.xyz/Article/details/gvtjzgamx.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://baike.fanxiaobao.xyz/Article/details/gpbwdhopw.sHtML

[Q49] 更新单行
来源：http://www.share.fanxiaobao.xyz/Article/details/gdcnbyplz.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://baike.fanxiaobao.xyz/Article/details/gihhzfmrj.sHtML

[Q50] 批量更新
来源：http://read.share.fanxiaobao.xyz/Article/details/gxepriywu.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://3g.fanxiaobao.xyz/Article/details/ggzszdpaq.sHtML

[Q51] 用子查询更新
来源：http://3g.fanxiaobao.xyz/Article/details/gnixaouea.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmyvwycqd.sHtML

[Q52] 删除指定行
来源：http://mobile.fanxiaobao.xyz/Article/details/gyivdhkcx.sHtML

DELETE FROM users WHERE id = 10;
来源：http://m.share.fanxiaobao.xyz/Article/details/givfqdkoe.sHtML

[Q53] 按条件删除
来源：http://baike.fanxiaobao.xyz/Article/details/gezdgnrfu.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://mobile.fanxiaobao.xyz/Article/details/gfabdedrx.sHtML

[Q54] 清空表
来源：http://blog.fanxiaobao.xyz/Article/details/gvcumwnex.sHtML

TRUNCATE TABLE logs;
来源：http://mobile.fanxiaobao.xyz/Article/details/gvcnezhez.sHtML

[Q55] 排名（并列占位）
来源：http://3g.fanxiaobao.xyz/Article/details/gmevvoaaf.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://wap.fanxiaobao.xyz/Article/details/gbpigveln.sHtML

[Q56] 密集排名（并列不占位）
来源：http://baike.fanxiaobao.xyz/Article/details/gakemzyrs.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvgpwwsul.sHtML

[Q57] 行号
来源：http://wap.fanxiaobao.xyz/Article/details/gxpusvajq.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/grpqtchkr.sHtML

[Q58] 累计求和
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwkvhpovg.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://3g.fanxiaobao.xyz/Article/details/gqkwfdide.sHtML

[Q59] 分组内累计
来源：http://3g.fanxiaobao.xyz/Article/details/gllbspjdf.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://wap.fanxiaobao.xyz/Article/details/gajlbckrj.sHtML

[Q60] 取上一行 / 下一行
来源：http://wap.fanxiaobao.xyz/Article/details/gyxdlpgqz.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://m.share.fanxiaobao.xyz/Article/details/gsjknrros.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://blog.fanxiaobao.xyz/Article/details/gjlddllyv.sHtML

[Q61] 移动平均
来源：http://mobile.fanxiaobao.xyz/Article/details/gvqnwgjqq.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://mobile.fanxiaobao.xyz/Article/details/gcsgmzvqu.sHtML

[Q62] 分组占比
来源：http://mobile.fanxiaobao.xyz/Article/details/geymdkuiy.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://3g.fanxiaobao.xyz/Article/details/gdnxgzizi.sHtML

[Q63] 开启事务
来源：http://read.share.fanxiaobao.xyz/Article/details/gegxcjhnq.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggzvsxljc.sHtML

[Q64] 提交事务
来源：http://mobile.fanxiaobao.xyz/Article/details/gtxvkqxdy.sHtML

COMMIT;
来源：http://3g.fanxiaobao.xyz/Article/details/gevorqcuy.sHtML

[Q65] 回滚事务
来源：http://mobile.fanxiaobao.xyz/Article/details/glfpcsfef.sHtML

ROLLBACK;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goatdeghy.sHtML

[Q66] 行锁查询
来源：http://3g.fanxiaobao.xyz/Article/details/gwtldzuhi.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://blog.fanxiaobao.xyz/Article/details/geefscgvs.sHtML

[Q67] 设置隔离级别
来源：http://m.share.fanxiaobao.xyz/Article/details/gfxcohptd.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.share.fanxiaobao.xyz/Article/details/gepocwkfg.sHtML

[Q68] 保存点
来源：http://www.share.fanxiaobao.xyz/Article/details/geydbejax.sHtML

SAVEPOINT sp1;
来源：http://read.share.fanxiaobao.xyz/Article/details/gcuwxlwtl.sHtML

ROLLBACK TO sp1;
来源：http://baike.fanxiaobao.xyz/Article/details/gvjwizlhl.sHtML

[Q69] 查看执行计划
来源：http://m.share.fanxiaobao.xyz/Article/details/gmipxtmwn.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkluqjwyw.sHtML

[Q70] 更新统计信息
来源：http://www.blog.fanxiaobao.xyz/Article/details/gehuwtvyd.sHtML

ANALYZE TABLE users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gqiwrzgfo.sHtML

[Q71] 查看建表语句
来源：http://m.share.fanxiaobao.xyz/Article/details/gjbkdeiri.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://blog.fanxiaobao.xyz/Article/details/gyqeucung.sHtML

[Q72] 查看索引
来源：http://mobile.fanxiaobao.xyz/Article/details/glmctsvai.sHtML

SHOW INDEX FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gocwvrmfh.sHtML

[Q73] 查看表状态
来源：http://m.share.fanxiaobao.xyz/Article/details/gcxoajcdk.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://mobile.fanxiaobao.xyz/Article/details/gydofnvgh.sHtML

[Q74] 强制使用索引
来源：http://m.share.fanxiaobao.xyz/Article/details/ghweveyrs.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.blog.fanxiaobao.xyz/Article/details/goepodwpa.sHtML

[Q75] 日期格式化
来源：http://read.share.fanxiaobao.xyz/Article/details/gthxqhjid.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://blog.fanxiaobao.xyz/Article/details/gkzpzwkfq.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://baike.fanxiaobao.xyz/Article/details/gmsuzqiux.sHtML

[Q76] 按天统计
来源：http://blog.fanxiaobao.xyz/Article/details/gkrhbqayc.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://3g.fanxiaobao.xyz/Article/details/gzfrozari.sHtML

[Q77] 时间加减
来源：http://m.share.fanxiaobao.xyz/Article/details/gyqjcsotd.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://3g.fanxiaobao.xyz/Article/details/gutbqyuhr.sHtML

[Q78] 当前时间
来源：http://baike.fanxiaobao.xyz/Article/details/geftekxjf.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://wap.fanxiaobao.xyz/Article/details/goxmwpzia.sHtML

[Q79] 字符串拼接
来源：http://3g.fanxiaobao.xyz/Article/details/gxeidohmg.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://baike.fanxiaobao.xyz/Article/details/gkveqxhrp.sHtML

[Q80] 字符串截取
来源：http://blog.fanxiaobao.xyz/Article/details/gqnyukikh.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/genhnbcao.sHtML

[Q81] 字符串替换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gujkuxwqi.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gqwrvqsec.sHtML

[Q82] 字符长度与字节长度
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxrrqfmjg.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gblkqllul.sHtML

[Q83] 大小写转换
来源：http://blog.fanxiaobao.xyz/Article/details/gedihjbza.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/glydruxrv.sHtML

[Q84] 去除首尾空格
来源：http://read.share.fanxiaobao.xyz/Article/details/geewjbkpc.sHtML

SELECT TRIM(name) FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gghhkqtef.sHtML

[Q85] 数值取整
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gspalfjoz.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqmkrzdsw.sHtML

[Q86] 读取 JSON 字段
来源：http://baike.fanxiaobao.xyz/Article/details/gjrcwpatf.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://read.share.fanxiaobao.xyz/Article/details/gtuevkpbd.sHtML

[Q87] JSON 字段做条件
来源：http://blog.fanxiaobao.xyz/Article/details/gaqhyphrw.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://blog.fanxiaobao.xyz/Article/details/gnmiwuoca.sHtML

[Q88] 行转列（条件聚合）
来源：http://m.share.fanxiaobao.xyz/Article/details/ghvsnvlfp.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://wap.fanxiaobao.xyz/Article/details/gvgvlmogs.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/guwbjoavp.sHtML

[Q89] 判断表是否存在
来源：http://blog.fanxiaobao.xyz/Article/details/gkikrtops.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://baike.fanxiaobao.xyz/Article/details/gljwjkgky.sHtML

[Q90] 生成序号列
来源：http://mobile.fanxiaobao.xyz/Article/details/ggmzsoisn.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://m.share.fanxiaobao.xyz/Article/details/gbrflmxkf.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gffmvqzpt.sHtML

R. Bash 专题
来源：http://mobile.fanxiaobao.xyz/Article/details/geqowrfbc.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gugfteylp.sHtML

[R01] shebang 与严格模式
来源：http://mobile.fanxiaobao.xyz/Article/details/gjovvjcdv.sHtML

#!/usr/bin/env bash
来源：http://baike.fanxiaobao.xyz/Article/details/gpzmmtbew.sHtML

set -euo pipefail
来源：http://www.share.fanxiaobao.xyz/Article/details/ggbtysizb.sHtML

[R02] 变量赋值与使用
来源：http://mobile.fanxiaobao.xyz/Article/details/gqogvzjya.sHtML

name="Tom"; echo "$name"
来源：http://m.share.fanxiaobao.xyz/Article/details/guiwzzzra.sHtML

[R03] 只读变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gviqblwlp.sHtML

readonly PI=3.14
来源：http://baike.fanxiaobao.xyz/Article/details/gzcbmbvth.sHtML

[R04] 位置参数
来源：http://read.share.fanxiaobao.xyz/Article/details/gwgaomcad.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://baike.fanxiaobao.xyz/Article/details/guxbsmjud.sHtML

[R05] 参数默认值
来源：http://m.share.fanxiaobao.xyz/Article/details/gctdbwqtw.sHtML

name="${1:-default}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gyfsqiitq.sHtML

[R06] 判断命令是否存在
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvgwvkjjb.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://wap.fanxiaobao.xyz/Article/details/gwvhvdmle.sHtML

[R07] if 判断文件
来源：http://wap.fanxiaobao.xyz/Article/details/gflscogpr.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://read.share.fanxiaobao.xyz/Article/details/gnndvdqkm.sHtML

[R08] 数值比较
来源：http://blog.fanxiaobao.xyz/Article/details/gefdqmpfm.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://3g.fanxiaobao.xyz/Article/details/gyqgflveq.sHtML

[R09] 字符串比较
来源：http://m.share.fanxiaobao.xyz/Article/details/gfhulaegx.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://baike.fanxiaobao.xyz/Article/details/gzsoomqav.sHtML

[R10] 正则匹配
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpesdtvvv.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnlubozfh.sHtML

[R11] case 多分支
来源：http://3g.fanxiaobao.xyz/Article/details/gpnvrhskz.sHtML

case "$1" in
来源：http://3g.fanxiaobao.xyz/Article/details/gmnqyofpe.sHtML

start) echo "启动" ;;
来源：http://wap.fanxiaobao.xyz/Article/details/gukwzxpor.sHtML

stop)  echo "停止" ;;
来源：http://blog.fanxiaobao.xyz/Article/details/glyasskyw.sHtML

*)     echo "未知命令" ;;
来源：http://baike.fanxiaobao.xyz/Article/details/gqduyunmy.sHtML

esac
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfvelbytx.sHtML

[R12] for 遍历文件
来源：http://3g.fanxiaobao.xyz/Article/details/gemgcrhyw.sHtML

for f in *.txt; do echo "$f"; done
来源：http://read.share.fanxiaobao.xyz/Article/details/ggwozbtxm.sHtML

[R13] for 计数循环
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkogqjwly.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://wap.fanxiaobao.xyz/Article/details/gphzyvvra.sHtML

[R14] C 风格 for
来源：http://www.share.fanxiaobao.xyz/Article/details/gvnoxwrxw.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://wap.fanxiaobao.xyz/Article/details/gvxugtxmz.sHtML

[R15] while 逐行读文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gjmunburm.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gfsuwqbei.sHtML

[R16] until 等待条件
来源：http://baike.fanxiaobao.xyz/Article/details/gqfufzwgq.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://read.share.fanxiaobao.xyz/Article/details/guzcaschx.sHtML

[R17] 数组定义与取值
来源：http://m.share.fanxiaobao.xyz/Article/details/grpndmwob.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gicpgnqfz.sHtML

[R18] 遍历数组
来源：http://blog.fanxiaobao.xyz/Article/details/gzvivszma.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gzfwunfvm.sHtML

[R19] 数组长度
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdtwwmbbt.sHtML

echo "${#arr[@]}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gyofpfbri.sHtML

[R20] 关联数组（字典）
来源：http://baike.fanxiaobao.xyz/Article/details/gvnfampnl.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gvksoabmo.sHtML

[R21] 字符串长度
来源：http://baike.fanxiaobao.xyz/Article/details/gcpyfkohk.sHtML

echo "${#s}"
来源：http://baike.fanxiaobao.xyz/Article/details/gktmuyuyp.sHtML

[R22] 截取子串
来源：http://baike.fanxiaobao.xyz/Article/details/gtxmdyivp.sHtML

echo "${s:0:5}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gttkbubwu.sHtML

[R23] 字符串替换
来源：http://3g.fanxiaobao.xyz/Article/details/gbaucwotj.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://read.share.fanxiaobao.xyz/Article/details/gfddxhywz.sHtML

[R24] 大小写转换
来源：http://blog.fanxiaobao.xyz/Article/details/gyquxzfmt.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gjdragnmh.sHtML

[R25] 去后缀 / 去前缀
来源：http://wap.fanxiaobao.xyz/Article/details/gmucqzabk.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gqnhgrkgm.sHtML

[R26] 命令替换
来源：http://read.share.fanxiaobao.xyz/Article/details/gzmheycis.sHtML

now=$(date +%F); echo "$now"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyslstohl.sHtML

[R27] 算术展开
来源：http://mobile.fanxiaobao.xyz/Article/details/gqqaonhrj.sHtML

echo $((1 + 2 * 3))
来源：http://3g.fanxiaobao.xyz/Article/details/gquotgqnz.sHtML

[R28] 浮点运算
来源：http://read.share.fanxiaobao.xyz/Article/details/guaidgtyv.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.share.fanxiaobao.xyz/Article/details/glsrifxzz.sHtML

[R29] 定义函数
来源：http://baike.fanxiaobao.xyz/Article/details/glazojuaw.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://blog.fanxiaobao.xyz/Article/details/gzihzqart.sHtML

[R30] 函数返回状态码
来源：http://wap.fanxiaobao.xyz/Article/details/gvsbrtfpw.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://wap.fanxiaobao.xyz/Article/details/gvaxhxjww.sHtML

[R31] 局部变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grfymvguc.sHtML

f() { local x=1; echo "$x"; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gzqytmjyf.sHtML

[R32] 参数个数校验
来源：http://baike.fanxiaobao.xyz/Article/details/ghwzatjuo.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gsqzluiat.sHtML

[R33] 捕获错误并提示行号
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjaanmsar.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://m.share.fanxiaobao.xyz/Article/details/gpbhlokya.sHtML

[R34] 退出时清理
来源：http://mobile.fanxiaobao.xyz/Article/details/gwalinavm.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://mobile.fanxiaobao.xyz/Article/details/gmhszffwb.sHtML

[R35] 后台执行并等待
来源：http://3g.fanxiaobao.xyz/Article/details/gpmfrwwoo.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://3g.fanxiaobao.xyz/Article/details/gorzryqgs.sHtML

[R36] 并发执行多个任务
来源：http://blog.fanxiaobao.xyz/Article/details/gpvydxfvh.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://read.share.fanxiaobao.xyz/Article/details/giuxfecun.sHtML

[R37] 把输出赋给变量
来源：http://read.share.fanxiaobao.xyz/Article/details/gudbywefc.sHtML

files=$(ls -1)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gagykvlbd.sHtML

[R38] 管道串联
来源：http://read.share.fanxiaobao.xyz/Article/details/gllxjsdxu.sHtML

cat a.txt | grep -i error | wc -l
来源：http://read.share.fanxiaobao.xyz/Article/details/gfqsqbsbm.sHtML

[R39] 重定向标准输出与错误
来源：http://3g.fanxiaobao.xyz/Article/details/gesvvehtv.sHtML

cmd > out.log 2>&1
来源：http://blog.fanxiaobao.xyz/Article/details/gtprjqewz.sHtML

[R40] 追加写日志
来源：http://read.share.fanxiaobao.xyz/Article/details/gmqhyyyle.sHtML

echo "log" >> out.log
来源：http://mobile.fanxiaobao.xyz/Article/details/gsoobsouq.sHtML

[R41] 丢弃输出
来源：http://mobile.fanxiaobao.xyz/Article/details/gmvhpybew.sHtML

cmd >/dev/null 2>&1
来源：http://3g.fanxiaobao.xyz/Article/details/gpsemmfew.sHtML

[R42] 输入重定向
来源：http://mobile.fanxiaobao.xyz/Article/details/gerolkvgt.sHtML

wc -l < a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gchnfujtk.sHtML

[R43] 按名字查找文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gtxkhqesq.sHtML


<!-- 参考信息 -->