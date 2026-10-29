代发 wailian999

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.fehbvm.com/Article/details/gatvduxuj.sHtML

user_id INT NOT NULL,
来源：http://3g.zdbjq.cn/Article/details/glmililfk.sHtML

amount DECIMAL(10, 2),
来源：http://www.blog.hesvh.cn/Article/details/giahkkwlw.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://m.share.zdbjq.cn/Article/details/gnnsehblc.sHtML

);
来源：http://3g.fehbvm.com/Article/details/gaacdnvdq.sHtML

[Q03] 增加列
来源：http://read.share.fehbvm.com/Article/details/gramimycx.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://blog.fehbvm.com/Article/details/gyuiccymy.sHtML

[Q04] 修改列类型
来源：http://read.share.zdbjq.cn/Article/details/gvtxaopsx.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://wap.zdbjq.cn/Article/details/gmesrrqrl.sHtML

[Q05] 重命名列
来源：http://3g.hesvh.cn/Article/details/gbnucymvx.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.blog.zdbjq.cn/Article/details/gmuxfvrgs.sHtML

[Q06] 删除列
来源：http://blog.zdbjq.cn/Article/details/gdmvgystc.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://blog.hesvh.cn/Article/details/gayphiabz.sHtML

[Q07] 删除表
来源：http://m.share.hesvh.cn/Article/details/gouhbqjdx.sHtML

DROP TABLE IF EXISTS orders;
来源：http://3g.fehbvm.com/Article/details/glhymnigj.sHtML

[Q08] 创建普通索引
来源：http://wap.fehbvm.com/Article/details/ghtzaskrt.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://m.share.hesvh.cn/Article/details/gckbzidre.sHtML

[Q09] 创建唯一索引
来源：http://m.share.fehbvm.com/Article/details/gwrtngkkh.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.share.zdbjq.cn/Article/details/ghfbtixay.sHtML

[Q10] 插入单行
来源：http://www.share.zdbjq.cn/Article/details/gnqoeiomd.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://blog.hesvh.cn/Article/details/ghtupmhcd.sHtML

[Q11] 一次插入多行
来源：http://www.share.fehbvm.com/Article/details/gvzksdbqh.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://blog.hesvh.cn/Article/details/guzsufuas.sHtML

[Q12] 插入后取自增 ID
来源：http://www.share.zdbjq.cn/Article/details/grgzlbakg.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://read.share.zdbjq.cn/Article/details/gglkagjyu.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.m.share.fehbvm.com/Article/details/ggjryzrsg.sHtML

[Q13] 忽略重复插入
来源：http://m.share.hesvh.cn/Article/details/gfdglkdgv.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.blog.zdbjq.cn/Article/details/gxpoohcqu.sHtML

[Q14] 存在则更新（upsert）
来源：http://baike.hesvh.cn/Article/details/gbkvzhnzh.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://3g.hesvh.cn/Article/details/gukfozwmt.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://3g.hesvh.cn/Article/details/gnzsbeevi.sHtML

[Q15] 查询全部
来源：http://m.share.zdbjq.cn/Article/details/gbsdgabbo.sHtML

SELECT * FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/guqquyksn.sHtML

[Q16] 查询指定列
来源：http://www.m.share.hesvh.cn/Article/details/gzkgkuoey.sHtML

SELECT id, name FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gohjwtlvr.sHtML

[Q17] 条件查询
来源：http://www.share.fehbvm.com/Article/details/gtsmqyise.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.blog.hesvh.cn/Article/details/gwzahwsek.sHtML

[Q18] 模糊匹配
来源：http://www.share.zdbjq.cn/Article/details/glmhnervt.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://read.share.hesvh.cn/Article/details/ghdqgvdog.sHtML

[Q19] 范围查询
来源：http://www.m.share.fehbvm.com/Article/details/guxcaagwf.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.share.zdbjq.cn/Article/details/gyntuxoew.sHtML

[Q20] IN 列表
来源：http://www.blog.hesvh.cn/Article/details/gdewhrmii.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.share.fehbvm.com/Article/details/grfvxrggp.sHtML

[Q21] 空值判断
来源：http://www.share.hesvh.cn/Article/details/gtbrcuzjo.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.share.hesvh.cn/Article/details/gojwwnkjq.sHtML

[Q22] 排序
来源：http://baike.hesvh.cn/Article/details/goawxcqyz.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://wap.fehbvm.com/Article/details/grczjwikg.sHtML

[Q23] 分页
来源：http://www.m.share.zdbjq.cn/Article/details/gazjrttzf.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://blog.hesvh.cn/Article/details/gsdlelrhn.sHtML

[Q24] 去重
来源：http://wap.fehbvm.com/Article/details/gevbyvwsr.sHtML

SELECT DISTINCT city FROM users;
来源：http://blog.hesvh.cn/Article/details/gxcoimsyq.sHtML

[Q25] 只取前 N 条
来源：http://3g.fehbvm.com/Article/details/gyalqsxip.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://blog.zdbjq.cn/Article/details/gjnmpvoij.sHtML

[Q26] 计数
来源：http://wap.fehbvm.com/Article/details/gjqlcilci.sHtML

SELECT COUNT(*) FROM users;
来源：http://read.share.hesvh.cn/Article/details/gkzsfwvvr.sHtML

[Q27] 条件计数
来源：http://baike.hesvh.cn/Article/details/gduxsvccn.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gevfhubmi.sHtML

[Q28] 求和与平均
来源：http://www.share.hesvh.cn/Article/details/gkxeozlqt.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://blog.hesvh.cn/Article/details/gxgqasshi.sHtML

[Q29] 最大最小值
来源：http://www.share.fehbvm.com/Article/details/gmrqhdegg.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.share.fehbvm.com/Article/details/gslevabjt.sHtML

[Q30] 分组统计
来源：http://www.m.share.hesvh.cn/Article/details/gswyjdtmg.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.m.share.zdbjq.cn/Article/details/guyofgsqt.sHtML

[Q31] 分组后过滤
来源：http://www.blog.hesvh.cn/Article/details/gvhlzrffu.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://wap.zdbjq.cn/Article/details/gybxjbrxy.sHtML

[Q32] 分组拼接字符串
来源：http://blog.fehbvm.com/Article/details/ggoqzpyjy.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://wap.fehbvm.com/Article/details/gerudhsno.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://read.share.zdbjq.cn/Article/details/gwozhyalt.sHtML

[Q33] 多列分组
来源：http://wap.hesvh.cn/Article/details/glrtakvdf.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://m.share.hesvh.cn/Article/details/gtxmzjziw.sHtML

[Q34] 每组取第一条
来源：http://m.share.hesvh.cn/Article/details/gjxoppphz.sHtML

SELECT * FROM (
来源：http://www.share.fehbvm.com/Article/details/gesjdxeml.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://read.share.fehbvm.com/Article/details/gkzmlkgwf.sHtML

) t WHERE rn = 1;
来源：http://www.share.fehbvm.com/Article/details/gdwbfebkm.sHtML

[Q35] 内连接
来源：http://3g.fehbvm.com/Article/details/gpsxaxrqs.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.zdbjq.cn/Article/details/gcdmcuzll.sHtML

[Q36] 左连接
来源：http://m.share.hesvh.cn/Article/details/gmvbwdgli.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://read.share.fehbvm.com/Article/details/gajsocsqn.sHtML

[Q37] 右连接
来源：http://m.share.fehbvm.com/Article/details/gaujgzchi.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.share.zdbjq.cn/Article/details/gyfrgoqsn.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.blog.fehbvm.com/Article/details/gzjbesrra.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://m.share.hesvh.cn/Article/details/gttqscnky.sHtML

[Q39] 自连接（查上下级）
来源：http://3g.fehbvm.com/Article/details/gitbkcgoq.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.share.fehbvm.com/Article/details/gtjhqkbue.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://3g.fehbvm.com/Article/details/gyhiksomy.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://blog.hesvh.cn/Article/details/gcmudlszx.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://baike.zdbjq.cn/Article/details/gxadyweyt.sHtML

[Q41] 多表连接
来源：http://baike.fehbvm.com/Article/details/gyfpvqxnl.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.blog.zdbjq.cn/Article/details/gozjugfme.sHtML

JOIN users u ON u.id = o.user_id
来源：http://baike.hesvh.cn/Article/details/gmkquenns.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://m.share.fehbvm.com/Article/details/gesbkohyt.sHtML

[Q42] 连接条件附加过滤
来源：http://baike.hesvh.cn/Article/details/gjsxocdop.sHtML

SELECT u.name, o.amount FROM users u
来源：http://m.share.zdbjq.cn/Article/details/gmylomlfr.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://3g.fehbvm.com/Article/details/grnwmdrww.sHtML

[Q43] 标量子查询
来源：http://m.share.fehbvm.com/Article/details/gcwnucblg.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://baike.hesvh.cn/Article/details/gjeqbziie.sHtML

[Q44] IN 子查询
来源：http://m.share.hesvh.cn/Article/details/gkxmlicyd.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://baike.fehbvm.com/Article/details/gsrakzcuc.sHtML

[Q45] EXISTS 判断存在
来源：http://www.share.fehbvm.com/Article/details/gnicueooi.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.hesvh.cn/Article/details/gokxrosde.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.m.share.hesvh.cn/Article/details/gdezrohuz.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.zdbjq.cn/Article/details/gaqoxgzev.sHtML

[Q47] 与平均值比较
来源：http://www.blog.fehbvm.com/Article/details/gawubobnt.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://read.share.fehbvm.com/Article/details/gnwusehvg.sHtML

[Q48] CTE 公用表表达式
来源：http://baike.hesvh.cn/Article/details/glfzfeqcy.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://3g.fehbvm.com/Article/details/gscptzzpd.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://blog.zdbjq.cn/Article/details/gburubslc.sHtML

[Q49] 更新单行
来源：http://www.blog.fehbvm.com/Article/details/ggejjvaqk.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://m.share.zdbjq.cn/Article/details/gimmgicmx.sHtML

[Q50] 批量更新
来源：http://mobile.zdbjq.cn/Article/details/gtelzcpiu.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://m.share.fehbvm.com/Article/details/gopbowudu.sHtML

[Q51] 用子查询更新
来源：http://baike.fehbvm.com/Article/details/gcfwmwlbz.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.m.share.zdbjq.cn/Article/details/gijgwoakr.sHtML

[Q52] 删除指定行
来源：http://www.share.hesvh.cn/Article/details/gcpgiycdg.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.share.zdbjq.cn/Article/details/gwuqjzltb.sHtML

[Q53] 按条件删除
来源：http://read.share.fehbvm.com/Article/details/gtnfuwgqk.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://read.share.zdbjq.cn/Article/details/gqrpnvflo.sHtML

[Q54] 清空表
来源：http://read.share.hesvh.cn/Article/details/gifbrkero.sHtML

TRUNCATE TABLE logs;
来源：http://blog.hesvh.cn/Article/details/grxrgooky.sHtML

[Q55] 排名（并列占位）
来源：http://www.m.share.fehbvm.com/Article/details/gbszmjvwm.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://baike.hesvh.cn/Article/details/gekzupobn.sHtML

[Q56] 密集排名（并列不占位）
来源：http://m.share.zdbjq.cn/Article/details/guoudqqxj.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://baike.fehbvm.com/Article/details/grbvukepz.sHtML

[Q57] 行号
来源：http://m.share.fehbvm.com/Article/details/gaznbjtca.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://blog.zdbjq.cn/Article/details/gneskwrnb.sHtML

[Q58] 累计求和
来源：http://mobile.zdbjq.cn/Article/details/gfijyjwpl.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.m.share.fehbvm.com/Article/details/gjdlaeujv.sHtML

[Q59] 分组内累计
来源：http://3g.zdbjq.cn/Article/details/gdwayczfw.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://baike.hesvh.cn/Article/details/gzjbtoowt.sHtML

[Q60] 取上一行 / 下一行
来源：http://read.share.fehbvm.com/Article/details/gcmhxzyrn.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://blog.fehbvm.com/Article/details/gnavfsxan.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.share.hesvh.cn/Article/details/gaxmwnfoi.sHtML

[Q61] 移动平均
来源：http://baike.fehbvm.com/Article/details/gkenmmqkd.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://3g.zdbjq.cn/Article/details/gdaxgkmrn.sHtML

[Q62] 分组占比
来源：http://blog.fehbvm.com/Article/details/goounkljd.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.blog.fehbvm.com/Article/details/giszdhyhc.sHtML

[Q63] 开启事务
来源：http://www.m.share.zdbjq.cn/Article/details/giodzibof.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://baike.zdbjq.cn/Article/details/gwpkjvxrq.sHtML

[Q64] 提交事务
来源：http://read.share.hesvh.cn/Article/details/gxkieebxn.sHtML

COMMIT;
来源：http://m.share.zdbjq.cn/Article/details/ghnvwaroj.sHtML

[Q65] 回滚事务
来源：http://www.blog.fehbvm.com/Article/details/gezdoainx.sHtML

ROLLBACK;
来源：http://wap.hesvh.cn/Article/details/gntxzdpso.sHtML

[Q66] 行锁查询
来源：http://wap.fehbvm.com/Article/details/gsjhgjzdh.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.m.share.hesvh.cn/Article/details/ghhjrmjix.sHtML

[Q67] 设置隔离级别
来源：http://m.share.fehbvm.com/Article/details/gmxujwhtb.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://mobile.fehbvm.com/Article/details/gpiuwehtk.sHtML

[Q68] 保存点
来源：http://read.share.hesvh.cn/Article/details/gwnxmwwyu.sHtML

SAVEPOINT sp1;
来源：http://www.m.share.hesvh.cn/Article/details/gbipeusej.sHtML

ROLLBACK TO sp1;
来源：http://wap.hesvh.cn/Article/details/grvqymnpl.sHtML

[Q69] 查看执行计划
来源：http://wap.fehbvm.com/Article/details/gqhqgrxgk.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://read.share.fehbvm.com/Article/details/gzvlguiko.sHtML

[Q70] 更新统计信息
来源：http://blog.hesvh.cn/Article/details/gfbyqoqcg.sHtML

ANALYZE TABLE users;
来源：http://mobile.zdbjq.cn/Article/details/gqegbjhof.sHtML

[Q71] 查看建表语句
来源：http://www.share.fehbvm.com/Article/details/gpbhgnkhc.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://blog.zdbjq.cn/Article/details/gnqfijyim.sHtML

[Q72] 查看索引
来源：http://wap.zdbjq.cn/Article/details/gmpbihnsp.sHtML

SHOW INDEX FROM users;
来源：http://www.share.zdbjq.cn/Article/details/ghbhanmhn.sHtML

[Q73] 查看表状态
来源：http://www.blog.zdbjq.cn/Article/details/gdrhwfswf.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://3g.fehbvm.com/Article/details/giwhpbcvu.sHtML

[Q74] 强制使用索引
来源：http://blog.fehbvm.com/Article/details/gzvpmcmoz.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://m.share.fehbvm.com/Article/details/gzeudednf.sHtML

[Q75] 日期格式化
来源：http://wap.hesvh.cn/Article/details/gbxcwvphu.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.blog.fehbvm.com/Article/details/gpyowglhc.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.m.share.hesvh.cn/Article/details/gwrwldhjl.sHtML

[Q76] 按天统计
来源：http://www.m.share.fehbvm.com/Article/details/ghipxceuf.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://read.share.hesvh.cn/Article/details/gfbooioyh.sHtML

[Q77] 时间加减
来源：http://m.share.zdbjq.cn/Article/details/gdaehluxa.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://3g.hesvh.cn/Article/details/gqaiskrwn.sHtML

[Q78] 当前时间
来源：http://www.m.share.fehbvm.com/Article/details/gykckctza.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://read.share.hesvh.cn/Article/details/gbnprnekd.sHtML

[Q79] 字符串拼接
来源：http://baike.zdbjq.cn/Article/details/gnkjhfnqw.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.blog.fehbvm.com/Article/details/glmewfbfz.sHtML

[Q80] 字符串截取
来源：http://read.share.hesvh.cn/Article/details/gahxipfsk.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://mobile.hesvh.cn/Article/details/gxbszeutn.sHtML

[Q81] 字符串替换
来源：http://m.share.hesvh.cn/Article/details/gorlxjbta.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/glfkzrfoz.sHtML

[Q82] 字符长度与字节长度
来源：http://3g.hesvh.cn/Article/details/gfptuopng.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gwfjxnvyx.sHtML

[Q83] 大小写转换
来源：http://m.share.fehbvm.com/Article/details/gnrpudnrg.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://blog.zdbjq.cn/Article/details/ggnzmtzgc.sHtML

[Q84] 去除首尾空格
来源：http://www.m.share.fehbvm.com/Article/details/gaokogdic.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gwjmgckft.sHtML

[Q85] 数值取整
来源：http://wap.zdbjq.cn/Article/details/gqmjaveyp.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://read.share.hesvh.cn/Article/details/gwqoabczu.sHtML

[Q86] 读取 JSON 字段
来源：http://www.m.share.zdbjq.cn/Article/details/gfxiolzbo.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://m.share.zdbjq.cn/Article/details/geqitqmhh.sHtML

[Q87] JSON 字段做条件
来源：http://blog.hesvh.cn/Article/details/gelrqtmec.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://mobile.zdbjq.cn/Article/details/gilftdedu.sHtML

[Q88] 行转列（条件聚合）
来源：http://m.share.zdbjq.cn/Article/details/gcykaxiyc.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://blog.fehbvm.com/Article/details/govqkkhlg.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://baike.zdbjq.cn/Article/details/gazsblpym.sHtML

[Q89] 判断表是否存在
来源：http://m.share.fehbvm.com/Article/details/gchssdvqr.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://3g.zdbjq.cn/Article/details/ggrfwcrir.sHtML

[Q90] 生成序号列
来源：http://www.share.zdbjq.cn/Article/details/gkjamzidj.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.share.hesvh.cn/Article/details/gpsgairnf.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/ggarhhhtu.sHtML

R. Bash 专题
来源：http://blog.fehbvm.com/Article/details/gfqkqpuxh.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gjbzwpvbn.sHtML

[R01] shebang 与严格模式
来源：http://m.share.zdbjq.cn/Article/details/gyialruoz.sHtML

#!/usr/bin/env bash
来源：http://www.share.hesvh.cn/Article/details/gtmhkcrva.sHtML

set -euo pipefail
来源：http://read.share.zdbjq.cn/Article/details/giocliton.sHtML

[R02] 变量赋值与使用
来源：http://www.m.share.hesvh.cn/Article/details/gvbqesyxf.sHtML

name="Tom"; echo "$name"
来源：http://blog.zdbjq.cn/Article/details/gegvczpts.sHtML

[R03] 只读变量
来源：http://www.m.share.hesvh.cn/Article/details/ghasxnjqb.sHtML

readonly PI=3.14
来源：http://mobile.zdbjq.cn/Article/details/gemjtjwdk.sHtML

[R04] 位置参数
来源：http://wap.hesvh.cn/Article/details/gjpuypalj.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://baike.zdbjq.cn/Article/details/gunjfmtez.sHtML

[R05] 参数默认值
来源：http://m.share.fehbvm.com/Article/details/gqgthnwex.sHtML

name="${1:-default}"
来源：http://wap.fehbvm.com/Article/details/grsowsjid.sHtML

[R06] 判断命令是否存在
来源：http://3g.fehbvm.com/Article/details/gzyzvmesh.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://3g.hesvh.cn/Article/details/gjzmidocb.sHtML

[R07] if 判断文件
来源：http://blog.zdbjq.cn/Article/details/gcqawlkgn.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://baike.zdbjq.cn/Article/details/gzvhzrjrv.sHtML

[R08] 数值比较
来源：http://3g.zdbjq.cn/Article/details/gdamgbvtl.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://wap.zdbjq.cn/Article/details/ghfpohayk.sHtML

[R09] 字符串比较
来源：http://3g.hesvh.cn/Article/details/genkqfknm.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://3g.zdbjq.cn/Article/details/gxngmmhgl.sHtML

[R10] 正则匹配
来源：http://www.share.hesvh.cn/Article/details/gmkusyjss.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://read.share.fehbvm.com/Article/details/gnvtzjakt.sHtML

[R11] case 多分支
来源：http://baike.zdbjq.cn/Article/details/gljzguzjz.sHtML

case "$1" in
来源：http://mobile.zdbjq.cn/Article/details/gicwivxqt.sHtML

start) echo "启动" ;;
来源：http://www.share.fehbvm.com/Article/details/gpfxynsym.sHtML

stop)  echo "停止" ;;
来源：http://www.share.hesvh.cn/Article/details/gsxgybkiz.sHtML

*)     echo "未知命令" ;;
来源：http://m.share.hesvh.cn/Article/details/gxawbdksw.sHtML

esac
来源：http://m.share.hesvh.cn/Article/details/gyzyvohdo.sHtML

[R12] for 遍历文件
来源：http://www.share.fehbvm.com/Article/details/gtscvmzhm.sHtML

for f in *.txt; do echo "$f"; done
来源：http://wap.zdbjq.cn/Article/details/gcrwcwuku.sHtML

[R13] for 计数循环
来源：http://baike.zdbjq.cn/Article/details/ggiltacyl.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://baike.fehbvm.com/Article/details/gxkcgvdct.sHtML

[R14] C 风格 for
来源：http://3g.fehbvm.com/Article/details/ghfpcjxes.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://m.share.fehbvm.com/Article/details/gaxsihtoq.sHtML

[R15] while 逐行读文件
来源：http://blog.fehbvm.com/Article/details/gqpxryzyv.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://read.share.hesvh.cn/Article/details/gzxhhqmpw.sHtML

[R16] until 等待条件
来源：http://www.share.fehbvm.com/Article/details/gklzcztnd.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://m.share.zdbjq.cn/Article/details/gprvflypk.sHtML

[R17] 数组定义与取值
来源：http://mobile.hesvh.cn/Article/details/gesfyvpci.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.share.zdbjq.cn/Article/details/gmfltbedw.sHtML

[R18] 遍历数组
来源：http://mobile.zdbjq.cn/Article/details/gmerxubrj.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.share.zdbjq.cn/Article/details/gclirgpwd.sHtML

[R19] 数组长度
来源：http://m.share.fehbvm.com/Article/details/gvjfcnqes.sHtML

echo "${#arr[@]}"
来源：http://read.share.fehbvm.com/Article/details/ghglchwai.sHtML

[R20] 关联数组（字典）
来源：http://www.blog.zdbjq.cn/Article/details/gqxdramiu.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.m.share.fehbvm.com/Article/details/ggvikahwp.sHtML

[R21] 字符串长度
来源：http://3g.hesvh.cn/Article/details/gswrksrrd.sHtML

echo "${#s}"
来源：http://wap.fehbvm.com/Article/details/gcvozaaeg.sHtML

[R22] 截取子串
来源：http://baike.fehbvm.com/Article/details/gnjccpdfe.sHtML

echo "${s:0:5}"
来源：http://blog.hesvh.cn/Article/details/glovocipa.sHtML

[R23] 字符串替换
来源：http://mobile.zdbjq.cn/Article/details/gfnyssfic.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.blog.fehbvm.com/Article/details/ghxwfybfh.sHtML

[R24] 大小写转换
来源：http://www.blog.zdbjq.cn/Article/details/gozdcpuas.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://mobile.zdbjq.cn/Article/details/gvkzrudnn.sHtML

[R25] 去后缀 / 去前缀
来源：http://baike.zdbjq.cn/Article/details/gfldxcpaz.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.m.share.hesvh.cn/Article/details/guyqxrexn.sHtML

[R26] 命令替换
来源：http://read.share.zdbjq.cn/Article/details/gcithshrq.sHtML

now=$(date +%F); echo "$now"
来源：http://www.m.share.hesvh.cn/Article/details/gbqupklvl.sHtML

[R27] 算术展开
来源：http://m.share.zdbjq.cn/Article/details/gnifnjftr.sHtML

echo $((1 + 2 * 3))
来源：http://wap.fehbvm.com/Article/details/gyvryeoaj.sHtML

[R28] 浮点运算
来源：http://baike.fehbvm.com/Article/details/gpzxbtpws.sHtML

echo "scale=2; 10/3" | bc
来源：http://blog.fehbvm.com/Article/details/gngzjlwxr.sHtML

[R29] 定义函数
来源：http://baike.zdbjq.cn/Article/details/gwgbqtqti.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://3g.fehbvm.com/Article/details/gvgsfanxk.sHtML

[R30] 函数返回状态码
来源：http://blog.fehbvm.com/Article/details/gwysrqntb.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://m.share.hesvh.cn/Article/details/gwcqsouln.sHtML

[R31] 局部变量
来源：http://read.share.hesvh.cn/Article/details/giiwhjjdr.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.share.fehbvm.com/Article/details/giwsacqzs.sHtML

[R32] 参数个数校验
来源：http://blog.hesvh.cn/Article/details/gzrsbtjwu.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.blog.zdbjq.cn/Article/details/gpkxnyjqz.sHtML

[R33] 捕获错误并提示行号
来源：http://baike.hesvh.cn/Article/details/gmsgtdczo.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://wap.hesvh.cn/Article/details/gfrafcikd.sHtML

[R34] 退出时清理
来源：http://3g.zdbjq.cn/Article/details/gpfabuhpe.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.zdbjq.cn/Article/details/gyismkqsc.sHtML

[R35] 后台执行并等待
来源：http://mobile.hesvh.cn/Article/details/gdidyyona.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://3g.zdbjq.cn/Article/details/gobdgmgjq.sHtML

[R36] 并发执行多个任务
来源：http://wap.zdbjq.cn/Article/details/gejksadyu.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://3g.hesvh.cn/Article/details/gztpclgax.sHtML

[R37] 把输出赋给变量
来源：http://3g.zdbjq.cn/Article/details/gcqxhaedy.sHtML

files=$(ls -1)
来源：http://www.share.zdbjq.cn/Article/details/ghuiyslfn.sHtML

[R38] 管道串联
来源：http://baike.zdbjq.cn/Article/details/gcmgjswfv.sHtML

cat a.txt | grep -i error | wc -l
来源：http://read.share.hesvh.cn/Article/details/gcomhvbok.sHtML

[R39] 重定向标准输出与错误
来源：http://mobile.hesvh.cn/Article/details/gyghytzvi.sHtML

cmd > out.log 2>&1
来源：http://www.blog.fehbvm.com/Article/details/gbfuowpih.sHtML

[R40] 追加写日志
来源：http://read.share.zdbjq.cn/Article/details/gsbpgznfi.sHtML

echo "log" >> out.log
来源：http://mobile.fehbvm.com/Article/details/gwsirtsyv.sHtML

[R41] 丢弃输出
来源：http://www.m.share.zdbjq.cn/Article/details/goqudtxbh.sHtML

cmd >/dev/null 2>&1
来源：http://wap.zdbjq.cn/Article/details/gstfdctwm.sHtML

[R42] 输入重定向
来源：http://www.blog.zdbjq.cn/Article/details/gsbrlakws.sHtML

wc -l < a.txt
来源：http://www.m.share.zdbjq.cn/Article/details/gcfaakiol.sHtML

[R43] 按名字查找文件
来源：http://read.share.zdbjq.cn/Article/details/gtywukldc.sHtML

find . -name "*.log" -type f
来源：http://3g.zdbjq.cn/Article/details/guowfqvop.sHtML

[R44] 按修改时间查找
来源：http://www.share.fehbvm.com/Article/details/gmlzcqmlq.sHtML

find . -mtime -7 -type f
来源：http://www.blog.zdbjq.cn/Article/details/gkfnlgrsu.sHtML

[R45] 批量删除
来源：http://m.share.hesvh.cn/Article/details/gkcwogcwn.sHtML

find . -name "*.tmp" -delete
来源：http://baike.hesvh.cn/Article/details/gfbjhxmta.sHtML

[R46] 递归替换文件内容
来源：http://3g.hesvh.cn/Article/details/gjnlslnbr.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://blog.fehbvm.com/Article/details/gqmvrttdj.sHtML

[R47] sed 单行替换
来源：http://www.blog.fehbvm.com/Article/details/gvsvwrtaj.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://3g.zdbjq.cn/Article/details/gdobmjamf.sHtML

[R48] awk 取指定列
来源：http://www.m.share.hesvh.cn/Article/details/gmhazetaf.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.blog.zdbjq.cn/Article/details/gvjzaryse.sHtML

[R49] awk 带条件
来源：http://3g.hesvh.cn/Article/details/gvtynpvli.sHtML


<!-- 参考信息 -->