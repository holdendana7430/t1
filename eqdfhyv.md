代发 wailian999

CREATE TABLE users (
来源：http://baike.fanxiaobao.xyz/Article/details/gemkchqzn.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.share.fanxiaobao.xyz/Article/details/gtoonuded.sHtML

name VARCHAR(50) NOT NULL,
来源：http://blog.fanxiaobao.xyz/Article/details/giqqsqvxj.sHtML

email VARCHAR(100) UNIQUE,
来源：http://read.share.fanxiaobao.xyz/Article/details/gshvqzcag.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://baike.fanxiaobao.xyz/Article/details/gdwsvofyx.sHtML

);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqvdxwses.sHtML

[Q02] 创建带外键的表
来源：http://wap.fanxiaobao.xyz/Article/details/gpikbcwbw.sHtML

CREATE TABLE orders (
来源：http://read.share.fanxiaobao.xyz/Article/details/gkeglfyvx.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.fanxiaobao.xyz/Article/details/gzhgripfq.sHtML

user_id INT NOT NULL,
来源：http://www.share.fanxiaobao.xyz/Article/details/gotscdeom.sHtML

amount DECIMAL(10, 2),
来源：http://3g.fanxiaobao.xyz/Article/details/gpdavpkco.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://m.share.fanxiaobao.xyz/Article/details/gchtmlfyp.sHtML

);
来源：http://read.share.fanxiaobao.xyz/Article/details/gwyyecfaq.sHtML

[Q03] 增加列
来源：http://www.share.fanxiaobao.xyz/Article/details/gyilwgqqp.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://read.share.fanxiaobao.xyz/Article/details/gmaxpirek.sHtML

[Q04] 修改列类型
来源：http://read.share.fanxiaobao.xyz/Article/details/ghmhpqpus.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://m.share.fanxiaobao.xyz/Article/details/gqqczhgnw.sHtML

[Q05] 重命名列
来源：http://3g.fanxiaobao.xyz/Article/details/gzuxirmsw.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.share.fanxiaobao.xyz/Article/details/gqltbrdsw.sHtML

[Q06] 删除列
来源：http://3g.fanxiaobao.xyz/Article/details/gqwaegwsc.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://m.share.fanxiaobao.xyz/Article/details/gkcnyzgkl.sHtML

[Q07] 删除表
来源：http://m.share.fanxiaobao.xyz/Article/details/gccfmcrrh.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaukjlkkl.sHtML

[Q08] 创建普通索引
来源：http://blog.fanxiaobao.xyz/Article/details/geerjpiko.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://wap.fanxiaobao.xyz/Article/details/gadhdzgda.sHtML

[Q09] 创建唯一索引
来源：http://3g.fanxiaobao.xyz/Article/details/ggidzgqek.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://wap.fanxiaobao.xyz/Article/details/gqmizdewt.sHtML

[Q10] 插入单行
来源：http://www.blog.fanxiaobao.xyz/Article/details/gowvpgfhp.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.blog.fanxiaobao.xyz/Article/details/gagfpmxdo.sHtML

[Q11] 一次插入多行
来源：http://read.share.fanxiaobao.xyz/Article/details/gajqdqrhe.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbawcfuuq.sHtML

[Q12] 插入后取自增 ID
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gztfvptbb.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://m.share.fanxiaobao.xyz/Article/details/gpfqmwkpl.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.share.fanxiaobao.xyz/Article/details/gvlylscrr.sHtML

[Q13] 忽略重复插入
来源：http://wap.fanxiaobao.xyz/Article/details/gveynpccr.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://blog.fanxiaobao.xyz/Article/details/gvcnmaiqt.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdjkcxhgm.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://blog.fanxiaobao.xyz/Article/details/gdpuckqqs.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://m.share.fanxiaobao.xyz/Article/details/gurgnkcfn.sHtML

[Q15] 查询全部
来源：http://3g.fanxiaobao.xyz/Article/details/guauhekxh.sHtML

SELECT * FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gkuffequp.sHtML

[Q16] 查询指定列
来源：http://baike.fanxiaobao.xyz/Article/details/gwhxipzjm.sHtML

SELECT id, name FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gyvgtzfqz.sHtML

[Q17] 条件查询
来源：http://read.share.fanxiaobao.xyz/Article/details/girrrddcw.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://baike.fanxiaobao.xyz/Article/details/gekhcvamu.sHtML

[Q18] 模糊匹配
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glpgozmwv.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://3g.fanxiaobao.xyz/Article/details/gqwhlbime.sHtML

[Q19] 范围查询
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gublrunmv.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdiiuxdyy.sHtML

[Q20] IN 列表
来源：http://www.share.fanxiaobao.xyz/Article/details/gausdtjdh.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://wap.fanxiaobao.xyz/Article/details/gccqyhqob.sHtML

[Q21] 空值判断
来源：http://wap.fanxiaobao.xyz/Article/details/gfwxiblhr.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://read.share.fanxiaobao.xyz/Article/details/glkhjaruq.sHtML

[Q22] 排序
来源：http://wap.fanxiaobao.xyz/Article/details/gadhhxorm.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://mobile.fanxiaobao.xyz/Article/details/glssxlqfm.sHtML

[Q23] 分页
来源：http://blog.fanxiaobao.xyz/Article/details/gvuhymnut.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://read.share.fanxiaobao.xyz/Article/details/gjoeuqsss.sHtML

[Q24] 去重
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdzoytxfx.sHtML

SELECT DISTINCT city FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gwxcahgtj.sHtML

[Q25] 只取前 N 条
来源：http://3g.fanxiaobao.xyz/Article/details/gqydspvne.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://m.share.fanxiaobao.xyz/Article/details/gmdbwgmdj.sHtML

[Q26] 计数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvntweqhr.sHtML

SELECT COUNT(*) FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gzqmezoja.sHtML

[Q27] 条件计数
来源：http://read.share.fanxiaobao.xyz/Article/details/gzfkmmjdy.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gsleyqpfr.sHtML

[Q28] 求和与平均
来源：http://blog.fanxiaobao.xyz/Article/details/gvoujsyqd.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.share.fanxiaobao.xyz/Article/details/gbaezhmlm.sHtML

[Q29] 最大最小值
来源：http://www.share.fanxiaobao.xyz/Article/details/gexfpezeq.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzniihesv.sHtML

[Q30] 分组统计
来源：http://www.share.fanxiaobao.xyz/Article/details/gfdeqiiac.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://baike.fanxiaobao.xyz/Article/details/galsquyiz.sHtML

[Q31] 分组后过滤
来源：http://m.share.fanxiaobao.xyz/Article/details/gchemzkkk.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://blog.fanxiaobao.xyz/Article/details/gaeqtveud.sHtML

[Q32] 分组拼接字符串
来源：http://3g.fanxiaobao.xyz/Article/details/gnqcbjyvf.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://mobile.fanxiaobao.xyz/Article/details/gploealfg.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://mobile.fanxiaobao.xyz/Article/details/gwsooccxw.sHtML

[Q33] 多列分组
来源：http://www.blog.fanxiaobao.xyz/Article/details/gptaqjjwu.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://m.share.fanxiaobao.xyz/Article/details/gbyfrkpru.sHtML

[Q34] 每组取第一条
来源：http://wap.fanxiaobao.xyz/Article/details/gosudckrl.sHtML

SELECT * FROM (
来源：http://mobile.fanxiaobao.xyz/Article/details/ghmzveldo.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://wap.fanxiaobao.xyz/Article/details/gmrnufuqu.sHtML

) t WHERE rn = 1;
来源：http://mobile.fanxiaobao.xyz/Article/details/ggtnfjhto.sHtML

[Q35] 内连接
来源：http://3g.fanxiaobao.xyz/Article/details/gekjssotj.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.share.fanxiaobao.xyz/Article/details/gtzmyxqru.sHtML

[Q36] 左连接
来源：http://wap.fanxiaobao.xyz/Article/details/gjfopcbau.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://m.share.fanxiaobao.xyz/Article/details/gdyuoqrpt.sHtML

[Q37] 右连接
来源：http://read.share.fanxiaobao.xyz/Article/details/gwjnrrtwh.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://blog.fanxiaobao.xyz/Article/details/gppokjzfy.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxtywsygc.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://mobile.fanxiaobao.xyz/Article/details/gqeibpffs.sHtML

[Q39] 自连接（查上下级）
来源：http://m.share.fanxiaobao.xyz/Article/details/ghyrdikli.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.share.fanxiaobao.xyz/Article/details/ghzytibpx.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://mobile.fanxiaobao.xyz/Article/details/gkjbcfxln.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://read.share.fanxiaobao.xyz/Article/details/grqxtntip.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvsuvurui.sHtML

[Q41] 多表连接
来源：http://3g.fanxiaobao.xyz/Article/details/gutfclghk.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://baike.fanxiaobao.xyz/Article/details/givnysbto.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqkhhyvqm.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://read.share.fanxiaobao.xyz/Article/details/gwvsssotd.sHtML

[Q42] 连接条件附加过滤
来源：http://baike.fanxiaobao.xyz/Article/details/galbgsjch.sHtML

SELECT u.name, o.amount FROM users u
来源：http://blog.fanxiaobao.xyz/Article/details/gniwpueht.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://blog.fanxiaobao.xyz/Article/details/gjtpcaqhs.sHtML

[Q43] 标量子查询
来源：http://read.share.fanxiaobao.xyz/Article/details/gzpzwoaez.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://read.share.fanxiaobao.xyz/Article/details/gphgogztb.sHtML

[Q44] IN 子查询
来源：http://3g.fanxiaobao.xyz/Article/details/gorgfduqd.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://read.share.fanxiaobao.xyz/Article/details/gamfapkuv.sHtML

[Q45] EXISTS 判断存在
来源：http://www.share.fanxiaobao.xyz/Article/details/gzmmhjcrw.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.fanxiaobao.xyz/Article/details/gempmrnxy.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://read.share.fanxiaobao.xyz/Article/details/grmqbmzgp.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqphmjvic.sHtML

[Q47] 与平均值比较
来源：http://www.share.fanxiaobao.xyz/Article/details/gcdltofsl.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://read.share.fanxiaobao.xyz/Article/details/gjwgrdobd.sHtML

[Q48] CTE 公用表表达式
来源：http://baike.fanxiaobao.xyz/Article/details/geweqjfqw.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://3g.fanxiaobao.xyz/Article/details/glfqahnzl.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://3g.fanxiaobao.xyz/Article/details/gyqneeozq.sHtML

[Q49] 更新单行
来源：http://mobile.fanxiaobao.xyz/Article/details/grrvmeojj.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://blog.fanxiaobao.xyz/Article/details/gwkdqbzfj.sHtML

[Q50] 批量更新
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsmwdbvlk.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://wap.fanxiaobao.xyz/Article/details/gympgytfw.sHtML

[Q51] 用子查询更新
来源：http://wap.fanxiaobao.xyz/Article/details/giczcmdic.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://baike.fanxiaobao.xyz/Article/details/gvplfvhpk.sHtML

[Q52] 删除指定行
来源：http://baike.fanxiaobao.xyz/Article/details/gywwhnqqr.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gswjttpgp.sHtML

[Q53] 按条件删除
来源：http://www.share.fanxiaobao.xyz/Article/details/gwapjkwsk.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://wap.fanxiaobao.xyz/Article/details/gtbassnek.sHtML

[Q54] 清空表
来源：http://www.share.fanxiaobao.xyz/Article/details/gkysmbzyd.sHtML

TRUNCATE TABLE logs;
来源：http://3g.fanxiaobao.xyz/Article/details/gqjmxttnm.sHtML

[Q55] 排名（并列占位）
来源：http://blog.fanxiaobao.xyz/Article/details/gbmvwigta.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmlcgdyta.sHtML

[Q56] 密集排名（并列不占位）
来源：http://mobile.fanxiaobao.xyz/Article/details/gihiwdtlm.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://wap.fanxiaobao.xyz/Article/details/gviiyvgix.sHtML

[Q57] 行号
来源：http://blog.fanxiaobao.xyz/Article/details/gjtnhoizu.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghjzsbwwu.sHtML

[Q58] 累计求和
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaefwmore.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://baike.fanxiaobao.xyz/Article/details/gzstqucku.sHtML

[Q59] 分组内累计
来源：http://www.share.fanxiaobao.xyz/Article/details/ghtwxpoxa.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.share.fanxiaobao.xyz/Article/details/gdtdiaird.sHtML

[Q60] 取上一行 / 下一行
来源：http://wap.fanxiaobao.xyz/Article/details/gdgozkvop.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://baike.fanxiaobao.xyz/Article/details/gzpuycmtf.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.share.fanxiaobao.xyz/Article/details/gpdxoohss.sHtML

[Q61] 移动平均
来源：http://m.share.fanxiaobao.xyz/Article/details/gyyyuadmh.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://3g.fanxiaobao.xyz/Article/details/gtckytzuq.sHtML

[Q62] 分组占比
来源：http://www.share.fanxiaobao.xyz/Article/details/gtahkyehm.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://3g.fanxiaobao.xyz/Article/details/gfjlswcmw.sHtML

[Q63] 开启事务
来源：http://m.share.fanxiaobao.xyz/Article/details/gntalzhnr.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://wap.fanxiaobao.xyz/Article/details/gmrfzikvl.sHtML

[Q64] 提交事务
来源：http://m.share.fanxiaobao.xyz/Article/details/gnmpolzpi.sHtML

COMMIT;
来源：http://3g.fanxiaobao.xyz/Article/details/ginvizguw.sHtML

[Q65] 回滚事务
来源：http://wap.fanxiaobao.xyz/Article/details/gixwxsazr.sHtML

ROLLBACK;
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghgwxmpkr.sHtML

[Q66] 行锁查询
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtpaqfead.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.share.fanxiaobao.xyz/Article/details/gkaglefhs.sHtML

[Q67] 设置隔离级别
来源：http://read.share.fanxiaobao.xyz/Article/details/gpzltpexf.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmnezssjl.sHtML

[Q68] 保存点
来源：http://mobile.fanxiaobao.xyz/Article/details/gtycmfwvc.sHtML

SAVEPOINT sp1;
来源：http://blog.fanxiaobao.xyz/Article/details/gcvyoalxm.sHtML

ROLLBACK TO sp1;
来源：http://wap.fanxiaobao.xyz/Article/details/gvospyyhk.sHtML

[Q69] 查看执行计划
来源：http://mobile.fanxiaobao.xyz/Article/details/gltkcwqqj.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqiobudun.sHtML

[Q70] 更新统计信息
来源：http://read.share.fanxiaobao.xyz/Article/details/gitjpgzkp.sHtML

ANALYZE TABLE users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gnkptymbf.sHtML

[Q71] 查看建表语句
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghjcmuxdt.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://baike.fanxiaobao.xyz/Article/details/gjudyzxcd.sHtML

[Q72] 查看索引
来源：http://www.blog.fanxiaobao.xyz/Article/details/gojdhwwxp.sHtML

SHOW INDEX FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gpzhfmhlc.sHtML

[Q73] 查看表状态
来源：http://baike.fanxiaobao.xyz/Article/details/gieieonep.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://m.share.fanxiaobao.xyz/Article/details/gxarifsac.sHtML

[Q74] 强制使用索引
来源：http://m.share.fanxiaobao.xyz/Article/details/gymchbvql.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://m.share.fanxiaobao.xyz/Article/details/gqbxgkslk.sHtML

[Q75] 日期格式化
来源：http://read.share.fanxiaobao.xyz/Article/details/gkskxpxxp.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://3g.fanxiaobao.xyz/Article/details/gbceirusk.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://wap.fanxiaobao.xyz/Article/details/gllzmvefj.sHtML

[Q76] 按天统计
来源：http://www.share.fanxiaobao.xyz/Article/details/gdvimrlyk.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggrrpesdd.sHtML

[Q77] 时间加减
来源：http://3g.fanxiaobao.xyz/Article/details/gzvkjzryz.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkgdurqvf.sHtML

[Q78] 当前时间
来源：http://blog.fanxiaobao.xyz/Article/details/gfuwmvgio.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://wap.fanxiaobao.xyz/Article/details/gyszjppra.sHtML

[Q79] 字符串拼接
来源：http://3g.fanxiaobao.xyz/Article/details/gwhtegliw.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.share.fanxiaobao.xyz/Article/details/gasvrdvrd.sHtML

[Q80] 字符串截取
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxduczgnq.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtrlhljdu.sHtML

[Q81] 字符串替换
来源：http://3g.fanxiaobao.xyz/Article/details/gqtqtirvv.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/ghrwmyiah.sHtML

[Q82] 字符长度与字节长度
来源：http://read.share.fanxiaobao.xyz/Article/details/gafwxymkx.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gzbiduetx.sHtML

[Q83] 大小写转换
来源：http://3g.fanxiaobao.xyz/Article/details/gorkkpeiw.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gtygvsqqo.sHtML

[Q84] 去除首尾空格
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggqmodogk.sHtML

SELECT TRIM(name) FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gsyxxpucc.sHtML

[Q85] 数值取整
来源：http://3g.fanxiaobao.xyz/Article/details/gbyeisllx.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://blog.fanxiaobao.xyz/Article/details/glryxalbv.sHtML

[Q86] 读取 JSON 字段
来源：http://3g.fanxiaobao.xyz/Article/details/gdsrukbny.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://mobile.fanxiaobao.xyz/Article/details/gnqqwripf.sHtML

[Q87] JSON 字段做条件
来源：http://m.share.fanxiaobao.xyz/Article/details/gveyrnpua.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://read.share.fanxiaobao.xyz/Article/details/gsgwpjdxn.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gapktvqle.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://baike.fanxiaobao.xyz/Article/details/gpgyrhgug.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gwubegkwj.sHtML

[Q89] 判断表是否存在
来源：http://blog.fanxiaobao.xyz/Article/details/glysfrheg.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.share.fanxiaobao.xyz/Article/details/gfyfhoxgm.sHtML

[Q90] 生成序号列
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyvqkynam.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://3g.fanxiaobao.xyz/Article/details/gjyxiswbi.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gctuzxgcg.sHtML

R. Bash 专题
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmdcvdvvb.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmxqmcqnd.sHtML

[R01] shebang 与严格模式
来源：http://wap.fanxiaobao.xyz/Article/details/grnacurtx.sHtML

#!/usr/bin/env bash
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdxsomkva.sHtML

set -euo pipefail
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxxrocjly.sHtML

[R02] 变量赋值与使用
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gswgkdcbh.sHtML

name="Tom"; echo "$name"
来源：http://baike.fanxiaobao.xyz/Article/details/gygcvqgjz.sHtML

[R03] 只读变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gbfgorurm.sHtML

readonly PI=3.14
来源：http://wap.fanxiaobao.xyz/Article/details/gbkwloust.sHtML

[R04] 位置参数
来源：http://www.share.fanxiaobao.xyz/Article/details/gginfymvb.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.blog.fanxiaobao.xyz/Article/details/guibbowkp.sHtML

[R05] 参数默认值
来源：http://www.blog.fanxiaobao.xyz/Article/details/gceomazgg.sHtML

name="${1:-default}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gdvqgoxgg.sHtML

[R06] 判断命令是否存在
来源：http://read.share.fanxiaobao.xyz/Article/details/gnohvfjcm.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://baike.fanxiaobao.xyz/Article/details/gibwdfygi.sHtML

[R07] if 判断文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gsprhbtwe.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://wap.fanxiaobao.xyz/Article/details/gatsdhmge.sHtML

[R08] 数值比较
来源：http://3g.fanxiaobao.xyz/Article/details/gwxpalxzh.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.share.fanxiaobao.xyz/Article/details/gpuxqkqhy.sHtML

[R09] 字符串比较
来源：http://baike.fanxiaobao.xyz/Article/details/gwvulkbsj.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://mobile.fanxiaobao.xyz/Article/details/ggmzjskdw.sHtML

[R10] 正则匹配
来源：http://blog.fanxiaobao.xyz/Article/details/gunnuwmkv.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://3g.fanxiaobao.xyz/Article/details/gcwfnfaul.sHtML

[R11] case 多分支
来源：http://m.share.fanxiaobao.xyz/Article/details/goshmoqev.sHtML

case "$1" in
来源：http://www.share.fanxiaobao.xyz/Article/details/gxkatuceh.sHtML

start) echo "启动" ;;
来源：http://m.share.fanxiaobao.xyz/Article/details/gnigdnwhs.sHtML

stop)  echo "停止" ;;
来源：http://blog.fanxiaobao.xyz/Article/details/gmugwlllr.sHtML

*)     echo "未知命令" ;;
来源：http://baike.fanxiaobao.xyz/Article/details/gsklxgnzt.sHtML

esac
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyutjooxc.sHtML

[R12] for 遍历文件
来源：http://mobile.fanxiaobao.xyz/Article/details/glddszlle.sHtML

for f in *.txt; do echo "$f"; done
来源：http://3g.fanxiaobao.xyz/Article/details/gehkmtylj.sHtML

[R13] for 计数循环
来源：http://m.share.fanxiaobao.xyz/Article/details/gtxmcrqzu.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://baike.fanxiaobao.xyz/Article/details/guptychnd.sHtML

[R14] C 风格 for
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gudqnwoar.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://baike.fanxiaobao.xyz/Article/details/gukqqpeja.sHtML

[R15] while 逐行读文件
来源：http://wap.fanxiaobao.xyz/Article/details/gasaqfqrp.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/ggphiohjq.sHtML

[R16] until 等待条件
来源：http://www.blog.fanxiaobao.xyz/Article/details/guzsshnwh.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gznrhxsco.sHtML

[R17] 数组定义与取值
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtgppxapm.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqcjysbuz.sHtML

[R18] 遍历数组
来源：http://read.share.fanxiaobao.xyz/Article/details/guwxdmywh.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://blog.fanxiaobao.xyz/Article/details/goepmxyoe.sHtML

[R19] 数组长度
来源：http://baike.fanxiaobao.xyz/Article/details/gcfsorwuz.sHtML

echo "${#arr[@]}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gediwvbej.sHtML

[R20] 关联数组（字典）
来源：http://m.share.fanxiaobao.xyz/Article/details/gljcaecsf.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gxokmkrbe.sHtML

[R21] 字符串长度
来源：http://read.share.fanxiaobao.xyz/Article/details/gpuupcsva.sHtML

echo "${#s}"
来源：http://mobile.fanxiaobao.xyz/Article/details/ghfpugegz.sHtML

[R22] 截取子串
来源：http://baike.fanxiaobao.xyz/Article/details/gtillrmqy.sHtML

echo "${s:0:5}"
来源：http://3g.fanxiaobao.xyz/Article/details/gyjrxuvqh.sHtML

[R23] 字符串替换
来源：http://read.share.fanxiaobao.xyz/Article/details/gshocszir.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://mobile.fanxiaobao.xyz/Article/details/ghpbxuhpj.sHtML

[R24] 大小写转换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gealhixig.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghuggahvn.sHtML

[R25] 去后缀 / 去前缀
来源：http://wap.fanxiaobao.xyz/Article/details/gvujwmisf.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://baike.fanxiaobao.xyz/Article/details/gljlubtru.sHtML

[R26] 命令替换
来源：http://3g.fanxiaobao.xyz/Article/details/gbgoyqabm.sHtML

now=$(date +%F); echo "$now"
来源：http://m.share.fanxiaobao.xyz/Article/details/gnxmwjhxl.sHtML

[R27] 算术展开
来源：http://read.share.fanxiaobao.xyz/Article/details/gwmyjamxz.sHtML

echo $((1 + 2 * 3))
来源：http://read.share.fanxiaobao.xyz/Article/details/gjtnytdvt.sHtML

[R28] 浮点运算
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gptlezeff.sHtML

echo "scale=2; 10/3" | bc
来源：http://baike.fanxiaobao.xyz/Article/details/ggkjvbyyr.sHtML

[R29] 定义函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gmzrjxsib.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.share.fanxiaobao.xyz/Article/details/gwtsxtuhp.sHtML

[R30] 函数返回状态码
来源：http://3g.fanxiaobao.xyz/Article/details/galvxuhnh.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://read.share.fanxiaobao.xyz/Article/details/gbtqptftq.sHtML

[R31] 局部变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gwqccgcgo.sHtML

f() { local x=1; echo "$x"; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gusahdhoj.sHtML

[R32] 参数个数校验
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbzlmaanc.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://blog.fanxiaobao.xyz/Article/details/gniubyboj.sHtML

[R33] 捕获错误并提示行号
来源：http://m.share.fanxiaobao.xyz/Article/details/ghscmfxfp.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.share.fanxiaobao.xyz/Article/details/gqvuvyfbt.sHtML

[R34] 退出时清理
来源：http://www.share.fanxiaobao.xyz/Article/details/guoyuxmqq.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbhjcomou.sHtML

[R35] 后台执行并等待
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyarkcbhh.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqbtxsrrx.sHtML

[R36] 并发执行多个任务
来源：http://www.share.fanxiaobao.xyz/Article/details/gdfpczypi.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://m.share.fanxiaobao.xyz/Article/details/gbyavhzfe.sHtML

[R37] 把输出赋给变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gyxsmviup.sHtML

files=$(ls -1)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gikgwafsn.sHtML

[R38] 管道串联
来源：http://read.share.fanxiaobao.xyz/Article/details/gycprzmft.sHtML

cat a.txt | grep -i error | wc -l
来源：http://wap.fanxiaobao.xyz/Article/details/giexhbhsu.sHtML

[R39] 重定向标准输出与错误
来源：http://blog.fanxiaobao.xyz/Article/details/guhgdqqps.sHtML

cmd > out.log 2>&1
来源：http://3g.fanxiaobao.xyz/Article/details/gvowyzszx.sHtML

[R40] 追加写日志
来源：http://mobile.fanxiaobao.xyz/Article/details/glbwnjkjc.sHtML

echo "log" >> out.log
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkeetyvrv.sHtML

[R41] 丢弃输出
来源：http://wap.fanxiaobao.xyz/Article/details/gcaliviqs.sHtML

cmd >/dev/null 2>&1
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzmujdbaq.sHtML

[R42] 输入重定向
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbjomqvmv.sHtML

wc -l < a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gizcwxwlb.sHtML

[R43] 按名字查找文件
来源：http://www.share.fanxiaobao.xyz/Article/details/grajdwowz.sHtML

find . -name "*.log" -type f
来源：http://3g.fanxiaobao.xyz/Article/details/ggpybkrfc.sHtML

[R44] 按修改时间查找
来源：http://mobile.fanxiaobao.xyz/Article/details/gpecdsglp.sHtML

find . -mtime -7 -type f
来源：http://baike.fanxiaobao.xyz/Article/details/goslucvcy.sHtML

[R45] 批量删除
来源：http://read.share.fanxiaobao.xyz/Article/details/gkneaayql.sHtML


<!-- 参考信息 -->