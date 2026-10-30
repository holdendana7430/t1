代发 wailian999

CREATE TABLE users (
来源：http://www.blog.fanxiaobao.xyz/Article/details/gskohjrib.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjboaufpt.sHtML

name VARCHAR(50) NOT NULL,
来源：http://blog.fanxiaobao.xyz/Article/details/gbafjtyzx.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.m.share.fanxiaobao.xyz/Article/details/garpldzkg.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://blog.fanxiaobao.xyz/Article/details/gevmbtaki.sHtML

);
来源：http://blog.fanxiaobao.xyz/Article/details/gwxpwvjjg.sHtML

[Q02] 创建带外键的表
来源：http://mobile.fanxiaobao.xyz/Article/details/gztombcbt.sHtML

CREATE TABLE orders (
来源：http://read.share.fanxiaobao.xyz/Article/details/ghrfxnkoo.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.fanxiaobao.xyz/Article/details/gocnayoug.sHtML

user_id INT NOT NULL,
来源：http://blog.fanxiaobao.xyz/Article/details/gdaoxxdse.sHtML

amount DECIMAL(10, 2),
来源：http://wap.fanxiaobao.xyz/Article/details/glutogguu.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://wap.fanxiaobao.xyz/Article/details/gdghjglgh.sHtML

);
来源：http://wap.fanxiaobao.xyz/Article/details/ghirptknc.sHtML

[Q03] 增加列
来源：http://3g.fanxiaobao.xyz/Article/details/gmwbqbftb.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geftycbzr.sHtML

[Q04] 修改列类型
来源：http://mobile.fanxiaobao.xyz/Article/details/gemrswcew.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://blog.fanxiaobao.xyz/Article/details/goypprvbk.sHtML

[Q05] 重命名列
来源：http://blog.fanxiaobao.xyz/Article/details/gdoodarkx.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gddvznvgu.sHtML

[Q06] 删除列
来源：http://blog.fanxiaobao.xyz/Article/details/gpjplvnqr.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://blog.fanxiaobao.xyz/Article/details/gfslsupuk.sHtML

[Q07] 删除表
来源：http://blog.fanxiaobao.xyz/Article/details/gfmxldohu.sHtML

DROP TABLE IF EXISTS orders;
来源：http://mobile.fanxiaobao.xyz/Article/details/gecnabhiz.sHtML

[Q08] 创建普通索引
来源：http://m.share.fanxiaobao.xyz/Article/details/grglwcxsi.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfgavgmif.sHtML

[Q09] 创建唯一索引
来源：http://www.share.fanxiaobao.xyz/Article/details/ggrbywuin.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://baike.fanxiaobao.xyz/Article/details/gnnvjtkxn.sHtML

[Q10] 插入单行
来源：http://wap.fanxiaobao.xyz/Article/details/ggjktfmdc.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://blog.fanxiaobao.xyz/Article/details/guuhwtfwo.sHtML

[Q11] 一次插入多行
来源：http://read.share.fanxiaobao.xyz/Article/details/gumkdowrm.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://read.share.fanxiaobao.xyz/Article/details/gxiuczpuz.sHtML

[Q12] 插入后取自增 ID
来源：http://mobile.fanxiaobao.xyz/Article/details/ghloebsqw.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://m.share.fanxiaobao.xyz/Article/details/gdddfaoqq.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.share.fanxiaobao.xyz/Article/details/gxmngqumu.sHtML

[Q13] 忽略重复插入
来源：http://wap.fanxiaobao.xyz/Article/details/gmckafitj.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://mobile.fanxiaobao.xyz/Article/details/glkwhhbeb.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gziinvsro.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://baike.fanxiaobao.xyz/Article/details/giviqfghd.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://read.share.fanxiaobao.xyz/Article/details/gxannzahz.sHtML

[Q15] 查询全部
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gktirlbtp.sHtML

SELECT * FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gvrfdauja.sHtML

[Q16] 查询指定列
来源：http://wap.fanxiaobao.xyz/Article/details/goqzsrrhd.sHtML

SELECT id, name FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggsmaagpi.sHtML

[Q17] 条件查询
来源：http://m.share.fanxiaobao.xyz/Article/details/gdztzrlnt.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://read.share.fanxiaobao.xyz/Article/details/gjbmqfjxl.sHtML

[Q18] 模糊匹配
来源：http://www.share.fanxiaobao.xyz/Article/details/gayaaavwa.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://read.share.fanxiaobao.xyz/Article/details/gxtzcuvuh.sHtML

[Q19] 范围查询
来源：http://read.share.fanxiaobao.xyz/Article/details/gxmarystn.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://m.share.fanxiaobao.xyz/Article/details/gwwbpflsy.sHtML

[Q20] IN 列表
来源：http://blog.fanxiaobao.xyz/Article/details/gnemggiig.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://blog.fanxiaobao.xyz/Article/details/gzchbyfpb.sHtML

[Q21] 空值判断
来源：http://mobile.fanxiaobao.xyz/Article/details/gabxdbhar.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://mobile.fanxiaobao.xyz/Article/details/gpqtwagdj.sHtML

[Q22] 排序
来源：http://read.share.fanxiaobao.xyz/Article/details/ggckhkjxe.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://3g.fanxiaobao.xyz/Article/details/gkjpklgmq.sHtML

[Q23] 分页
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxpzxosys.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://mobile.fanxiaobao.xyz/Article/details/guwlljaox.sHtML

[Q24] 去重
来源：http://read.share.fanxiaobao.xyz/Article/details/gzvqkytdp.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grvggnxvx.sHtML

[Q25] 只取前 N 条
来源：http://www.share.fanxiaobao.xyz/Article/details/gnoiruruw.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwwwlimts.sHtML

[Q26] 计数
来源：http://wap.fanxiaobao.xyz/Article/details/ggewspibp.sHtML

SELECT COUNT(*) FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gtcppnall.sHtML

[Q27] 条件计数
来源：http://www.share.fanxiaobao.xyz/Article/details/gwwsoadrn.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gtdbzhksd.sHtML

[Q28] 求和与平均
来源：http://www.blog.fanxiaobao.xyz/Article/details/girpeynqe.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://m.share.fanxiaobao.xyz/Article/details/gbzwglqdn.sHtML

[Q29] 最大最小值
来源：http://www.share.fanxiaobao.xyz/Article/details/geombdsso.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gosnfshbd.sHtML

[Q30] 分组统计
来源：http://mobile.fanxiaobao.xyz/Article/details/gjvblfdsd.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcyxjrhjv.sHtML

[Q31] 分组后过滤
来源：http://www.share.fanxiaobao.xyz/Article/details/grekhppqe.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://3g.fanxiaobao.xyz/Article/details/gjcgcryab.sHtML

[Q32] 分组拼接字符串
来源：http://www.share.fanxiaobao.xyz/Article/details/goejerqba.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://wap.fanxiaobao.xyz/Article/details/gpyyipcvs.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://mobile.fanxiaobao.xyz/Article/details/gkdsjwyik.sHtML

[Q33] 多列分组
来源：http://mobile.fanxiaobao.xyz/Article/details/gnrhgqzua.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://read.share.fanxiaobao.xyz/Article/details/gupmlhkhf.sHtML

[Q34] 每组取第一条
来源：http://mobile.fanxiaobao.xyz/Article/details/gppxadins.sHtML

SELECT * FROM (
来源：http://mobile.fanxiaobao.xyz/Article/details/gczjebhbv.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://m.share.fanxiaobao.xyz/Article/details/gjhksokxt.sHtML

) t WHERE rn = 1;
来源：http://blog.fanxiaobao.xyz/Article/details/gninnppjm.sHtML

[Q35] 内连接
来源：http://wap.fanxiaobao.xyz/Article/details/gweaqhcdn.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwrqbsvti.sHtML

[Q36] 左连接
来源：http://blog.fanxiaobao.xyz/Article/details/gqejzocrc.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://3g.fanxiaobao.xyz/Article/details/guswbmuck.sHtML

[Q37] 右连接
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqrdyjhap.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://m.share.fanxiaobao.xyz/Article/details/gvnxgzggw.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://m.share.fanxiaobao.xyz/Article/details/gtbftuvng.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://blog.fanxiaobao.xyz/Article/details/gibvrcwtt.sHtML

[Q39] 自连接（查上下级）
来源：http://m.share.fanxiaobao.xyz/Article/details/grrpgfpnd.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtsqjuvoa.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://read.share.fanxiaobao.xyz/Article/details/gnqwerbze.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://read.share.fanxiaobao.xyz/Article/details/gvcvnkcrx.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://baike.fanxiaobao.xyz/Article/details/ggehddnvy.sHtML

[Q41] 多表连接
来源：http://3g.fanxiaobao.xyz/Article/details/gjfdpjmyt.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://read.share.fanxiaobao.xyz/Article/details/gckxolukz.sHtML

JOIN users u ON u.id = o.user_id
来源：http://mobile.fanxiaobao.xyz/Article/details/gsfxybjvm.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://read.share.fanxiaobao.xyz/Article/details/gqsxbrbcl.sHtML

[Q42] 连接条件附加过滤
来源：http://blog.fanxiaobao.xyz/Article/details/ggwmxsgcc.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkhsbkqly.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://m.share.fanxiaobao.xyz/Article/details/ghapdzzzm.sHtML

[Q43] 标量子查询
来源：http://www.share.fanxiaobao.xyz/Article/details/gkiukcfso.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://m.share.fanxiaobao.xyz/Article/details/gvquecqqq.sHtML

[Q44] IN 子查询
来源：http://3g.fanxiaobao.xyz/Article/details/gotjlkhyh.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://read.share.fanxiaobao.xyz/Article/details/grbxdmwwl.sHtML

[Q45] EXISTS 判断存在
来源：http://mobile.fanxiaobao.xyz/Article/details/gjmzeorrw.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtcbnvljz.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbjlsrfbh.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghmqztlrp.sHtML

[Q47] 与平均值比较
来源：http://www.share.fanxiaobao.xyz/Article/details/ghrumqqcl.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://baike.fanxiaobao.xyz/Article/details/gopahgdzx.sHtML

[Q48] CTE 公用表表达式
来源：http://wap.fanxiaobao.xyz/Article/details/gfhiaaoae.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://m.share.fanxiaobao.xyz/Article/details/gvyopirxr.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://mobile.fanxiaobao.xyz/Article/details/gqycdgfrv.sHtML

[Q49] 更新单行
来源：http://mobile.fanxiaobao.xyz/Article/details/gzompvmui.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyfsswgls.sHtML

[Q50] 批量更新
来源：http://read.share.fanxiaobao.xyz/Article/details/gdpofgvwj.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://m.share.fanxiaobao.xyz/Article/details/gbhufbhgp.sHtML

[Q51] 用子查询更新
来源：http://www.share.fanxiaobao.xyz/Article/details/gbstdpxdm.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmgrqguyh.sHtML

[Q52] 删除指定行
来源：http://wap.fanxiaobao.xyz/Article/details/gqgqnseks.sHtML

DELETE FROM users WHERE id = 10;
来源：http://mobile.fanxiaobao.xyz/Article/details/gbqecilzm.sHtML

[Q53] 按条件删除
来源：http://3g.fanxiaobao.xyz/Article/details/gfpdrxche.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://blog.fanxiaobao.xyz/Article/details/gikrsvjju.sHtML

[Q54] 清空表
来源：http://mobile.fanxiaobao.xyz/Article/details/gpfrjppkf.sHtML

TRUNCATE TABLE logs;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmyatfuhu.sHtML

[Q55] 排名（并列占位）
来源：http://www.share.fanxiaobao.xyz/Article/details/gkyexkbzq.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.blog.fanxiaobao.xyz/Article/details/guopvwike.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdyzjahxd.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://mobile.fanxiaobao.xyz/Article/details/glscyiouo.sHtML

[Q57] 行号
来源：http://wap.fanxiaobao.xyz/Article/details/gsrokryqh.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpwjnztzk.sHtML

[Q58] 累计求和
来源：http://read.share.fanxiaobao.xyz/Article/details/gzxnfommf.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://m.share.fanxiaobao.xyz/Article/details/glvajwsbf.sHtML

[Q59] 分组内累计
来源：http://mobile.fanxiaobao.xyz/Article/details/gskdhncmy.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.share.fanxiaobao.xyz/Article/details/gmagjhfrh.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmkllalga.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://3g.fanxiaobao.xyz/Article/details/gytybbqzm.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://baike.fanxiaobao.xyz/Article/details/gefnnaiul.sHtML

[Q61] 移动平均
来源：http://baike.fanxiaobao.xyz/Article/details/gvlefoeke.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.share.fanxiaobao.xyz/Article/details/gqvovfmcm.sHtML

[Q62] 分组占比
来源：http://baike.fanxiaobao.xyz/Article/details/ghfkbdzfz.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://3g.fanxiaobao.xyz/Article/details/gwtwphihi.sHtML

[Q63] 开启事务
来源：http://baike.fanxiaobao.xyz/Article/details/gfshwxenk.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://blog.fanxiaobao.xyz/Article/details/groktdaxa.sHtML

[Q64] 提交事务
来源：http://baike.fanxiaobao.xyz/Article/details/grbyyvujy.sHtML

COMMIT;
来源：http://read.share.fanxiaobao.xyz/Article/details/guixzhdtq.sHtML

[Q65] 回滚事务
来源：http://mobile.fanxiaobao.xyz/Article/details/geicxupxe.sHtML

ROLLBACK;
来源：http://3g.fanxiaobao.xyz/Article/details/gvzpvbbmk.sHtML

[Q66] 行锁查询
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnprfswqk.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://3g.fanxiaobao.xyz/Article/details/gglkgdutq.sHtML

[Q67] 设置隔离级别
来源：http://m.share.fanxiaobao.xyz/Article/details/gjelqadol.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://read.share.fanxiaobao.xyz/Article/details/gexhakvhf.sHtML

[Q68] 保存点
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghbbofhiw.sHtML

SAVEPOINT sp1;
来源：http://blog.fanxiaobao.xyz/Article/details/gkmcfcsnt.sHtML

ROLLBACK TO sp1;
来源：http://blog.fanxiaobao.xyz/Article/details/gtokeukwq.sHtML

[Q69] 查看执行计划
来源：http://blog.fanxiaobao.xyz/Article/details/gdnfcngfn.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://3g.fanxiaobao.xyz/Article/details/gouhwippk.sHtML

[Q70] 更新统计信息
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grherrfep.sHtML

ANALYZE TABLE users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzoqanmxg.sHtML

[Q71] 查看建表语句
来源：http://mobile.fanxiaobao.xyz/Article/details/gyhwrhowz.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.share.fanxiaobao.xyz/Article/details/gskdknism.sHtML

[Q72] 查看索引
来源：http://read.share.fanxiaobao.xyz/Article/details/gdlrpeekn.sHtML

SHOW INDEX FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gkkjocfhf.sHtML

[Q73] 查看表状态
来源：http://www.share.fanxiaobao.xyz/Article/details/gpvqmxsni.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.share.fanxiaobao.xyz/Article/details/gmxizxabj.sHtML

[Q74] 强制使用索引
来源：http://blog.fanxiaobao.xyz/Article/details/gabdypngk.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://baike.fanxiaobao.xyz/Article/details/galbbvlle.sHtML

[Q75] 日期格式化
来源：http://baike.fanxiaobao.xyz/Article/details/glvxpjeao.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://baike.fanxiaobao.xyz/Article/details/ghsiveywx.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://baike.fanxiaobao.xyz/Article/details/gtccogrrw.sHtML

[Q76] 按天统计
来源：http://read.share.fanxiaobao.xyz/Article/details/gurdnthfv.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://m.share.fanxiaobao.xyz/Article/details/gshqxgkwd.sHtML

[Q77] 时间加减
来源：http://wap.fanxiaobao.xyz/Article/details/gggplhttf.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsbgvrtgt.sHtML

[Q78] 当前时间
来源：http://www.share.fanxiaobao.xyz/Article/details/gipbuawui.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.blog.fanxiaobao.xyz/Article/details/giscqierv.sHtML

[Q79] 字符串拼接
来源：http://www.share.fanxiaobao.xyz/Article/details/gyglgxcxy.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://wap.fanxiaobao.xyz/Article/details/gvmktufav.sHtML

[Q80] 字符串截取
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghokdzsqk.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grfyglqpg.sHtML

[Q81] 字符串替换
来源：http://www.share.fanxiaobao.xyz/Article/details/gmdlkxukg.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gouojyfzy.sHtML

[Q82] 字符长度与字节长度
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvvlreazr.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/govfsrgxf.sHtML

[Q83] 大小写转换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnufarhcy.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gharqytkg.sHtML

[Q84] 去除首尾空格
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcqfaiuxo.sHtML

SELECT TRIM(name) FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gyvtipctu.sHtML

[Q85] 数值取整
来源：http://wap.fanxiaobao.xyz/Article/details/gjlnggtze.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://m.share.fanxiaobao.xyz/Article/details/gildkrcjr.sHtML

[Q86] 读取 JSON 字段
来源：http://read.share.fanxiaobao.xyz/Article/details/gsjbpwpof.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://baike.fanxiaobao.xyz/Article/details/gacltbtvc.sHtML

[Q87] JSON 字段做条件
来源：http://baike.fanxiaobao.xyz/Article/details/gskbxzaen.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://m.share.fanxiaobao.xyz/Article/details/gidtebraj.sHtML

[Q88] 行转列（条件聚合）
来源：http://baike.fanxiaobao.xyz/Article/details/gvoyvbepx.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.blog.fanxiaobao.xyz/Article/details/gviaqetzz.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gwtuvmepd.sHtML

[Q89] 判断表是否存在
来源：http://www.blog.fanxiaobao.xyz/Article/details/gczewzioa.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://3g.fanxiaobao.xyz/Article/details/gbehslkkz.sHtML

[Q90] 生成序号列
来源：http://wap.fanxiaobao.xyz/Article/details/gchcktycq.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://baike.fanxiaobao.xyz/Article/details/gabdolnzk.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gfyvxybfh.sHtML

R. Bash 专题
来源：http://www.blog.fanxiaobao.xyz/Article/details/goubybidj.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gabsyzdtv.sHtML

[R01] shebang 与严格模式
来源：http://www.share.fanxiaobao.xyz/Article/details/gyhehzing.sHtML

#!/usr/bin/env bash
来源：http://www.m.share.fanxiaobao.xyz/Article/details/govgswedq.sHtML

set -euo pipefail
来源：http://baike.fanxiaobao.xyz/Article/details/gyzmsmkzy.sHtML

[R02] 变量赋值与使用
来源：http://3g.fanxiaobao.xyz/Article/details/gdrcxkvyo.sHtML

name="Tom"; echo "$name"
来源：http://www.share.fanxiaobao.xyz/Article/details/gbviptzqo.sHtML

[R03] 只读变量
来源：http://blog.fanxiaobao.xyz/Article/details/gylmelkyx.sHtML

readonly PI=3.14
来源：http://baike.fanxiaobao.xyz/Article/details/goqzbsugy.sHtML

[R04] 位置参数
来源：http://read.share.fanxiaobao.xyz/Article/details/gzcsdknvr.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://mobile.fanxiaobao.xyz/Article/details/gilumtrlq.sHtML

[R05] 参数默认值
来源：http://www.share.fanxiaobao.xyz/Article/details/grxvmgkrh.sHtML

name="${1:-default}"
来源：http://m.share.fanxiaobao.xyz/Article/details/ggwmnysxu.sHtML

[R06] 判断命令是否存在
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqhadvjoe.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gppkjctab.sHtML

[R07] if 判断文件
来源：http://baike.fanxiaobao.xyz/Article/details/giucmcdtw.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://mobile.fanxiaobao.xyz/Article/details/gbwiajmwl.sHtML

[R08] 数值比较
来源：http://mobile.fanxiaobao.xyz/Article/details/gbeyerdor.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbrcwmgoo.sHtML

[R09] 字符串比较
来源：http://baike.fanxiaobao.xyz/Article/details/gjphzjhtc.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://read.share.fanxiaobao.xyz/Article/details/gdjggodnd.sHtML

[R10] 正则匹配
来源：http://www.share.fanxiaobao.xyz/Article/details/ghygvsfei.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://baike.fanxiaobao.xyz/Article/details/gjyvmwssc.sHtML

[R11] case 多分支
来源：http://3g.fanxiaobao.xyz/Article/details/gdevzjfgf.sHtML

case "$1" in
来源：http://www.share.fanxiaobao.xyz/Article/details/ghyslxubu.sHtML

start) echo "启动" ;;
来源：http://mobile.fanxiaobao.xyz/Article/details/gjwvpuwim.sHtML

stop)  echo "停止" ;;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfggaomhv.sHtML

*)     echo "未知命令" ;;
来源：http://wap.fanxiaobao.xyz/Article/details/gqzmeptnu.sHtML

esac
来源：http://blog.fanxiaobao.xyz/Article/details/gfmmiorcf.sHtML

[R12] for 遍历文件
来源：http://baike.fanxiaobao.xyz/Article/details/gbnwvfdmf.sHtML

for f in *.txt; do echo "$f"; done
来源：http://wap.fanxiaobao.xyz/Article/details/goyiskbnh.sHtML

[R13] for 计数循环
来源：http://3g.fanxiaobao.xyz/Article/details/gnibtlaqz.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://baike.fanxiaobao.xyz/Article/details/gukmlpeqs.sHtML

[R14] C 风格 for
来源：http://blog.fanxiaobao.xyz/Article/details/gqgivemxp.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://blog.fanxiaobao.xyz/Article/details/gmlufyosd.sHtML

[R15] while 逐行读文件
来源：http://wap.fanxiaobao.xyz/Article/details/gluaxwurc.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gmsueigoz.sHtML

[R16] until 等待条件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gatfidoys.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gghbpzmvc.sHtML

[R17] 数组定义与取值
来源：http://read.share.fanxiaobao.xyz/Article/details/gsyowpnzk.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://baike.fanxiaobao.xyz/Article/details/gbmqatuzm.sHtML

[R18] 遍历数组
来源：http://3g.fanxiaobao.xyz/Article/details/gljhehpac.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://wap.fanxiaobao.xyz/Article/details/gbbuorvck.sHtML

[R19] 数组长度
来源：http://wap.fanxiaobao.xyz/Article/details/gzyiascfw.sHtML

echo "${#arr[@]}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gcqqaazeu.sHtML

[R20] 关联数组（字典）
来源：http://m.share.fanxiaobao.xyz/Article/details/gamebjmqa.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gbvurgxai.sHtML

[R21] 字符串长度
来源：http://3g.fanxiaobao.xyz/Article/details/gxngwvwud.sHtML

echo "${#s}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gighzeqxo.sHtML

[R22] 截取子串
来源：http://read.share.fanxiaobao.xyz/Article/details/gqheoixrz.sHtML

echo "${s:0:5}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gofummgol.sHtML

[R23] 字符串替换
来源：http://read.share.fanxiaobao.xyz/Article/details/gtzrslujk.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.share.fanxiaobao.xyz/Article/details/gtwefycqp.sHtML

[R24] 大小写转换
来源：http://blog.fanxiaobao.xyz/Article/details/gdrinqvkz.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gqhybxqyp.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsgzlgqdl.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://baike.fanxiaobao.xyz/Article/details/gqbttddcq.sHtML

[R26] 命令替换
来源：http://blog.fanxiaobao.xyz/Article/details/gtbghraqk.sHtML

now=$(date +%F); echo "$now"
来源：http://blog.fanxiaobao.xyz/Article/details/gducamkyd.sHtML

[R27] 算术展开
来源：http://www.blog.fanxiaobao.xyz/Article/details/gawwiequl.sHtML

echo $((1 + 2 * 3))
来源：http://wap.fanxiaobao.xyz/Article/details/gheovtpiy.sHtML

[R28] 浮点运算
来源：http://baike.fanxiaobao.xyz/Article/details/gtizjbgvx.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gehbedyrj.sHtML

[R29] 定义函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtxwtthii.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://read.share.fanxiaobao.xyz/Article/details/gpnoccfft.sHtML

[R30] 函数返回状态码
来源：http://m.share.fanxiaobao.xyz/Article/details/gjxxhwegs.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://baike.fanxiaobao.xyz/Article/details/gytdujgau.sHtML

[R31] 局部变量
来源：http://www.share.fanxiaobao.xyz/Article/details/ghnevrhqd.sHtML

f() { local x=1; echo "$x"; }
来源：http://read.share.fanxiaobao.xyz/Article/details/goxoaucnq.sHtML

[R32] 参数个数校验
来源：http://read.share.fanxiaobao.xyz/Article/details/gtcixtcdf.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://blog.fanxiaobao.xyz/Article/details/gncdydxat.sHtML

[R33] 捕获错误并提示行号
来源：http://baike.fanxiaobao.xyz/Article/details/gquxpirgl.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpxegmljx.sHtML

[R34] 退出时清理
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsjwcpgez.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://baike.fanxiaobao.xyz/Article/details/gusqqzurv.sHtML

[R35] 后台执行并等待
来源：http://wap.fanxiaobao.xyz/Article/details/gvkjopvuy.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://mobile.fanxiaobao.xyz/Article/details/gnjpaufnz.sHtML

[R36] 并发执行多个任务
来源：http://wap.fanxiaobao.xyz/Article/details/ghttdomzr.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://m.share.fanxiaobao.xyz/Article/details/gpgyuzuzk.sHtML

[R37] 把输出赋给变量
来源：http://baike.fanxiaobao.xyz/Article/details/gmblnqsgu.sHtML

files=$(ls -1)
来源：http://m.share.fanxiaobao.xyz/Article/details/gmvwmvxtj.sHtML

[R38] 管道串联
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghfqmjotd.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqbcxcxdl.sHtML

[R39] 重定向标准输出与错误
来源：http://wap.fanxiaobao.xyz/Article/details/gigwvbeps.sHtML

cmd > out.log 2>&1
来源：http://read.share.fanxiaobao.xyz/Article/details/gvehszjzi.sHtML

[R40] 追加写日志
来源：http://www.share.fanxiaobao.xyz/Article/details/gitlftbug.sHtML

echo "log" >> out.log
来源：http://wap.fanxiaobao.xyz/Article/details/gmtknhdns.sHtML

[R41] 丢弃输出
来源：http://blog.fanxiaobao.xyz/Article/details/gkawihlkr.sHtML

cmd >/dev/null 2>&1
来源：http://m.share.fanxiaobao.xyz/Article/details/gekzuczbr.sHtML

[R42] 输入重定向
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaypscykb.sHtML

wc -l < a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/grfhzierx.sHtML

[R43] 按名字查找文件
来源：http://baike.fanxiaobao.xyz/Article/details/giigskzuk.sHtML

find . -name "*.log" -type f
来源：http://blog.fanxiaobao.xyz/Article/details/gbpslvxsm.sHtML

[R44] 按修改时间查找
来源：http://read.share.fanxiaobao.xyz/Article/details/grefjkwtg.sHtML

find . -mtime -7 -type f
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghdnvgbix.sHtML

[R45] 批量删除
来源：http://mobile.fanxiaobao.xyz/Article/details/gmhiahmlb.sHtML


<!-- 参考信息 -->