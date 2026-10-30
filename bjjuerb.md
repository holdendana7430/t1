代发 wailian999

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.fanxiaobao.xyz/Article/details/gairltuky.sHtML

user_id INT NOT NULL,
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpngrxvjz.sHtML

amount DECIMAL(10, 2),
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbvsnslja.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.share.fanxiaobao.xyz/Article/details/gnkwdqofc.sHtML

);
来源：http://wap.fanxiaobao.xyz/Article/details/gicnwnflc.sHtML

[Q03] 增加列
来源：http://mobile.fanxiaobao.xyz/Article/details/gqgxkkrgt.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://mobile.fanxiaobao.xyz/Article/details/gxiijjkpx.sHtML

[Q04] 修改列类型
来源：http://mobile.fanxiaobao.xyz/Article/details/gfjsuzual.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.share.fanxiaobao.xyz/Article/details/gbihnafxn.sHtML

[Q05] 重命名列
来源：http://3g.fanxiaobao.xyz/Article/details/giecbjmxm.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://blog.fanxiaobao.xyz/Article/details/gdsvcutqs.sHtML

[Q06] 删除列
来源：http://3g.fanxiaobao.xyz/Article/details/ggqljldak.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://read.share.fanxiaobao.xyz/Article/details/gdzipkdnh.sHtML

[Q07] 删除表
来源：http://wap.fanxiaobao.xyz/Article/details/gdkjckmaw.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.share.fanxiaobao.xyz/Article/details/gkykthwdg.sHtML

[Q08] 创建普通索引
来源：http://3g.fanxiaobao.xyz/Article/details/gcwimjais.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://baike.fanxiaobao.xyz/Article/details/grytsiefu.sHtML

[Q09] 创建唯一索引
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyjbriexm.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://baike.fanxiaobao.xyz/Article/details/gsogzdwhw.sHtML

[Q10] 插入单行
来源：http://blog.fanxiaobao.xyz/Article/details/gfpkvmazu.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.share.fanxiaobao.xyz/Article/details/gzvefhllc.sHtML

[Q11] 一次插入多行
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gynljnzny.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxrbszsvh.sHtML

[Q12] 插入后取自增 ID
来源：http://mobile.fanxiaobao.xyz/Article/details/gwnzaznap.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gerfermgi.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://mobile.fanxiaobao.xyz/Article/details/grtmkkrgg.sHtML

[Q13] 忽略重复插入
来源：http://read.share.fanxiaobao.xyz/Article/details/goegfvqbi.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.share.fanxiaobao.xyz/Article/details/gytgadofr.sHtML

[Q14] 存在则更新（upsert）
来源：http://mobile.fanxiaobao.xyz/Article/details/gabggykbd.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://baike.fanxiaobao.xyz/Article/details/gpuoyoyuz.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.share.fanxiaobao.xyz/Article/details/gonwrsqgp.sHtML

[Q15] 查询全部
来源：http://mobile.fanxiaobao.xyz/Article/details/geipdlvnh.sHtML

SELECT * FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/grzlolaes.sHtML

[Q16] 查询指定列
来源：http://3g.fanxiaobao.xyz/Article/details/glmkupcbd.sHtML

SELECT id, name FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gznaqdapn.sHtML

[Q17] 条件查询
来源：http://www.share.fanxiaobao.xyz/Article/details/gkvhbbrzd.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://m.share.fanxiaobao.xyz/Article/details/gwufxugya.sHtML

[Q18] 模糊匹配
来源：http://wap.fanxiaobao.xyz/Article/details/gpsawwrqq.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.blog.fanxiaobao.xyz/Article/details/giyqeypil.sHtML

[Q19] 范围查询
来源：http://3g.fanxiaobao.xyz/Article/details/grmdbmcuz.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://wap.fanxiaobao.xyz/Article/details/gjjmdyxea.sHtML

[Q20] IN 列表
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyinbzwmy.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbrifqubr.sHtML

[Q21] 空值判断
来源：http://www.share.fanxiaobao.xyz/Article/details/gdjvvxvxu.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://blog.fanxiaobao.xyz/Article/details/gpwmygzxw.sHtML

[Q22] 排序
来源：http://m.share.fanxiaobao.xyz/Article/details/gcfpgdaxh.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://read.share.fanxiaobao.xyz/Article/details/gedcgaphp.sHtML

[Q23] 分页
来源：http://3g.fanxiaobao.xyz/Article/details/gnvruabiu.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://blog.fanxiaobao.xyz/Article/details/gocvnqsqn.sHtML

[Q24] 去重
来源：http://blog.fanxiaobao.xyz/Article/details/gpwufhbzf.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfngdxict.sHtML

[Q25] 只取前 N 条
来源：http://blog.fanxiaobao.xyz/Article/details/govxxvdpf.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://read.share.fanxiaobao.xyz/Article/details/gjeecdftz.sHtML

[Q26] 计数
来源：http://3g.fanxiaobao.xyz/Article/details/gxhrwzojw.sHtML

SELECT COUNT(*) FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gsazoiphj.sHtML

[Q27] 条件计数
来源：http://3g.fanxiaobao.xyz/Article/details/glxauetql.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gsksysncq.sHtML

[Q28] 求和与平均
来源：http://www.share.fanxiaobao.xyz/Article/details/ghbibhyog.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://wap.fanxiaobao.xyz/Article/details/greoaqplw.sHtML

[Q29] 最大最小值
来源：http://mobile.fanxiaobao.xyz/Article/details/graelnxht.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gscxmgeqc.sHtML

[Q30] 分组统计
来源：http://3g.fanxiaobao.xyz/Article/details/gznnzgqwd.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://m.share.fanxiaobao.xyz/Article/details/giniygqcy.sHtML

[Q31] 分组后过滤
来源：http://3g.fanxiaobao.xyz/Article/details/gdarxqwnl.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://mobile.fanxiaobao.xyz/Article/details/gkykcopgu.sHtML

[Q32] 分组拼接字符串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghvnjvuzd.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://baike.fanxiaobao.xyz/Article/details/gkfagbkze.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://wap.fanxiaobao.xyz/Article/details/gcgvuirdz.sHtML

[Q33] 多列分组
来源：http://m.share.fanxiaobao.xyz/Article/details/gdbcqlgfc.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfduphfah.sHtML

[Q34] 每组取第一条
来源：http://baike.fanxiaobao.xyz/Article/details/gickvibsq.sHtML

SELECT * FROM (
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geeknnwbh.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://wap.fanxiaobao.xyz/Article/details/gylswdudx.sHtML

) t WHERE rn = 1;
来源：http://baike.fanxiaobao.xyz/Article/details/gzqpjyjsw.sHtML

[Q35] 内连接
来源：http://baike.fanxiaobao.xyz/Article/details/gsefsfgxl.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://blog.fanxiaobao.xyz/Article/details/geiimgjdx.sHtML

[Q36] 左连接
来源：http://blog.fanxiaobao.xyz/Article/details/gcenfygro.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.share.fanxiaobao.xyz/Article/details/gibknqdrv.sHtML

[Q37] 右连接
来源：http://mobile.fanxiaobao.xyz/Article/details/gaxlpwmiq.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://baike.fanxiaobao.xyz/Article/details/glgslyded.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://3g.fanxiaobao.xyz/Article/details/gvjfyieoa.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.share.fanxiaobao.xyz/Article/details/gbcjizufi.sHtML

[Q39] 自连接（查上下级）
来源：http://m.share.fanxiaobao.xyz/Article/details/gmaztxurh.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmjtkstgs.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.share.fanxiaobao.xyz/Article/details/goappascg.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://m.share.fanxiaobao.xyz/Article/details/gjlgjnxhv.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvpfsnlpm.sHtML

[Q41] 多表连接
来源：http://www.share.fanxiaobao.xyz/Article/details/garnkwrrh.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.share.fanxiaobao.xyz/Article/details/glwkvsezp.sHtML

JOIN users u ON u.id = o.user_id
来源：http://mobile.fanxiaobao.xyz/Article/details/gtadsxzew.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqxfjbvko.sHtML

[Q42] 连接条件附加过滤
来源：http://mobile.fanxiaobao.xyz/Article/details/gkdcjgcvi.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.blog.fanxiaobao.xyz/Article/details/gygjmqxyu.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://mobile.fanxiaobao.xyz/Article/details/gxopxriox.sHtML

[Q43] 标量子查询
来源：http://wap.fanxiaobao.xyz/Article/details/gwcitsayu.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://mobile.fanxiaobao.xyz/Article/details/gdfylvubr.sHtML

[Q44] IN 子查询
来源：http://baike.fanxiaobao.xyz/Article/details/gztbkbuqu.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://mobile.fanxiaobao.xyz/Article/details/gixlcluqr.sHtML

[Q45] EXISTS 判断存在
来源：http://baike.fanxiaobao.xyz/Article/details/gcpmxwwwm.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.fanxiaobao.xyz/Article/details/gbehxvrfn.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://3g.fanxiaobao.xyz/Article/details/gxjrxqbgm.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.fanxiaobao.xyz/Article/details/gzrgyysyb.sHtML

[Q47] 与平均值比较
来源：http://www.share.fanxiaobao.xyz/Article/details/gsprgvstv.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://blog.fanxiaobao.xyz/Article/details/gxjwqgvia.sHtML

[Q48] CTE 公用表表达式
来源：http://read.share.fanxiaobao.xyz/Article/details/grjngrpst.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcfowzzyp.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gogigvcde.sHtML

[Q49] 更新单行
来源：http://wap.fanxiaobao.xyz/Article/details/gyddndgyq.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://baike.fanxiaobao.xyz/Article/details/gvsxdmuca.sHtML

[Q50] 批量更新
来源：http://read.share.fanxiaobao.xyz/Article/details/gtwhcycmc.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://blog.fanxiaobao.xyz/Article/details/gizmndjpg.sHtML

[Q51] 用子查询更新
来源：http://blog.fanxiaobao.xyz/Article/details/gmxjmliev.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://3g.fanxiaobao.xyz/Article/details/glnnhaexb.sHtML

[Q52] 删除指定行
来源：http://read.share.fanxiaobao.xyz/Article/details/geulrvwkx.sHtML

DELETE FROM users WHERE id = 10;
来源：http://wap.fanxiaobao.xyz/Article/details/gphupjpfv.sHtML

[Q53] 按条件删除
来源：http://mobile.fanxiaobao.xyz/Article/details/gstfuddfm.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://3g.fanxiaobao.xyz/Article/details/gymrhrjjo.sHtML

[Q54] 清空表
来源：http://wap.fanxiaobao.xyz/Article/details/gzbnczara.sHtML

TRUNCATE TABLE logs;
来源：http://blog.fanxiaobao.xyz/Article/details/giwebaeim.sHtML

[Q55] 排名（并列占位）
来源：http://m.share.fanxiaobao.xyz/Article/details/gwcjobaue.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://m.share.fanxiaobao.xyz/Article/details/gjfciskzo.sHtML

[Q56] 密集排名（并列不占位）
来源：http://mobile.fanxiaobao.xyz/Article/details/gjjdacdrr.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.share.fanxiaobao.xyz/Article/details/gngdmayth.sHtML

[Q57] 行号
来源：http://mobile.fanxiaobao.xyz/Article/details/gzzwwmjfj.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gsxmbofhp.sHtML

[Q58] 累计求和
来源：http://wap.fanxiaobao.xyz/Article/details/gwnipbjqd.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://wap.fanxiaobao.xyz/Article/details/grgnanvyq.sHtML

[Q59] 分组内累计
来源：http://baike.fanxiaobao.xyz/Article/details/gwxevkqxk.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://mobile.fanxiaobao.xyz/Article/details/glaihxhhw.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.blog.fanxiaobao.xyz/Article/details/gubrymgqm.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.share.fanxiaobao.xyz/Article/details/gtfjfcbfb.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://mobile.fanxiaobao.xyz/Article/details/gxfeawuls.sHtML

[Q61] 移动平均
来源：http://read.share.fanxiaobao.xyz/Article/details/gctsgplef.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://read.share.fanxiaobao.xyz/Article/details/gvjlobedu.sHtML

[Q62] 分组占比
来源：http://baike.fanxiaobao.xyz/Article/details/gvplexfsz.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://3g.fanxiaobao.xyz/Article/details/gzccadpnu.sHtML

[Q63] 开启事务
来源：http://mobile.fanxiaobao.xyz/Article/details/gjjumxnhc.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://3g.fanxiaobao.xyz/Article/details/gvfibbbrf.sHtML

[Q64] 提交事务
来源：http://wap.fanxiaobao.xyz/Article/details/gptngjrni.sHtML

COMMIT;
来源：http://read.share.fanxiaobao.xyz/Article/details/ghftyajvw.sHtML

[Q65] 回滚事务
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpfbmmpvg.sHtML

ROLLBACK;
来源：http://baike.fanxiaobao.xyz/Article/details/gqansvmeu.sHtML

[Q66] 行锁查询
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnzkupbyn.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://mobile.fanxiaobao.xyz/Article/details/gptzuhhrh.sHtML

[Q67] 设置隔离级别
来源：http://baike.fanxiaobao.xyz/Article/details/gookjrglk.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwcctjyro.sHtML

[Q68] 保存点
来源：http://read.share.fanxiaobao.xyz/Article/details/gkljljgep.sHtML

SAVEPOINT sp1;
来源：http://mobile.fanxiaobao.xyz/Article/details/guiftjosv.sHtML

ROLLBACK TO sp1;
来源：http://www.share.fanxiaobao.xyz/Article/details/grihmkrwu.sHtML

[Q69] 查看执行计划
来源：http://baike.fanxiaobao.xyz/Article/details/gnyekckeq.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://3g.fanxiaobao.xyz/Article/details/gysyjrohm.sHtML

[Q70] 更新统计信息
来源：http://m.share.fanxiaobao.xyz/Article/details/gabquqvij.sHtML

ANALYZE TABLE users;
来源：http://baike.fanxiaobao.xyz/Article/details/gxfjknxky.sHtML

[Q71] 查看建表语句
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaiqgpzhr.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://read.share.fanxiaobao.xyz/Article/details/gclgjtyai.sHtML

[Q72] 查看索引
来源：http://blog.fanxiaobao.xyz/Article/details/gpdonoekf.sHtML

SHOW INDEX FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gvuuhxpzp.sHtML

[Q73] 查看表状态
来源：http://blog.fanxiaobao.xyz/Article/details/galaifhuz.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://baike.fanxiaobao.xyz/Article/details/gnmiczkkl.sHtML

[Q74] 强制使用索引
来源：http://baike.fanxiaobao.xyz/Article/details/gexazfhyv.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxkrkogbm.sHtML

[Q75] 日期格式化
来源：http://read.share.fanxiaobao.xyz/Article/details/gjtbmkepu.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://wap.fanxiaobao.xyz/Article/details/gezfqrptj.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://mobile.fanxiaobao.xyz/Article/details/gieaqlrxx.sHtML

[Q76] 按天统计
来源：http://3g.fanxiaobao.xyz/Article/details/glkxvamoc.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzxwwsvwj.sHtML

[Q77] 时间加减
来源：http://blog.fanxiaobao.xyz/Article/details/gfhflwszj.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpotghijk.sHtML

[Q78] 当前时间
来源：http://baike.fanxiaobao.xyz/Article/details/gvwtbgzgx.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://m.share.fanxiaobao.xyz/Article/details/gpubbrpfe.sHtML

[Q79] 字符串拼接
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggvkfkpyg.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.share.fanxiaobao.xyz/Article/details/ggxsqdpew.sHtML

[Q80] 字符串截取
来源：http://m.share.fanxiaobao.xyz/Article/details/gkubcaojm.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gljobdurq.sHtML

[Q81] 字符串替换
来源：http://blog.fanxiaobao.xyz/Article/details/gcivdflpr.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gbkmorcut.sHtML

[Q82] 字符长度与字节长度
来源：http://wap.fanxiaobao.xyz/Article/details/gqdetaenb.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gvymszdgt.sHtML

[Q83] 大小写转换
来源：http://blog.fanxiaobao.xyz/Article/details/gyvegumgr.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvbzoskud.sHtML

[Q84] 去除首尾空格
来源：http://read.share.fanxiaobao.xyz/Article/details/grtxwzvns.sHtML

SELECT TRIM(name) FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/guqmegtbi.sHtML

[Q85] 数值取整
来源：http://3g.fanxiaobao.xyz/Article/details/gsdbrdwzx.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqcvrlaol.sHtML

[Q86] 读取 JSON 字段
来源：http://3g.fanxiaobao.xyz/Article/details/gvvkmpion.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggzncioji.sHtML

[Q87] JSON 字段做条件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzyhodqgt.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://3g.fanxiaobao.xyz/Article/details/gtblvrlnt.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqejqhqhj.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://read.share.fanxiaobao.xyz/Article/details/gqashqjil.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gsqwxacuv.sHtML

[Q89] 判断表是否存在
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnozzfvuf.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://m.share.fanxiaobao.xyz/Article/details/guipxpdtm.sHtML

[Q90] 生成序号列
来源：http://wap.fanxiaobao.xyz/Article/details/gsnejclkh.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://baike.fanxiaobao.xyz/Article/details/gsbtjmltd.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gxgofomti.sHtML

R. Bash 专题
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyxakojoa.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwqflrebo.sHtML

[R01] shebang 与严格模式
来源：http://m.share.fanxiaobao.xyz/Article/details/grvatmzcq.sHtML

#!/usr/bin/env bash
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwsmbnuju.sHtML

set -euo pipefail
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpjnfvurm.sHtML

[R02] 变量赋值与使用
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gocwnrzlv.sHtML

name="Tom"; echo "$name"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkuakimvl.sHtML

[R03] 只读变量
来源：http://wap.fanxiaobao.xyz/Article/details/gammgulig.sHtML

readonly PI=3.14
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnsisslnc.sHtML

[R04] 位置参数
来源：http://read.share.fanxiaobao.xyz/Article/details/gxhpjelty.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giyrvyyrq.sHtML

[R05] 参数默认值
来源：http://mobile.fanxiaobao.xyz/Article/details/ghkdrffyp.sHtML

name="${1:-default}"
来源：http://mobile.fanxiaobao.xyz/Article/details/geadampku.sHtML

[R06] 判断命令是否存在
来源：http://read.share.fanxiaobao.xyz/Article/details/gmghrmhnm.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://3g.fanxiaobao.xyz/Article/details/geiwtrlnc.sHtML

[R07] if 判断文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gqehttvrk.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://mobile.fanxiaobao.xyz/Article/details/guhmtrbnd.sHtML

[R08] 数值比较
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpzmyrore.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmmshhhue.sHtML

[R09] 字符串比较
来源：http://mobile.fanxiaobao.xyz/Article/details/gikccbwxz.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://read.share.fanxiaobao.xyz/Article/details/goyrpflnu.sHtML

[R10] 正则匹配
来源：http://baike.fanxiaobao.xyz/Article/details/gkhkhucoy.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://mobile.fanxiaobao.xyz/Article/details/gazewglnx.sHtML

[R11] case 多分支
来源：http://read.share.fanxiaobao.xyz/Article/details/gthvbpilh.sHtML

case "$1" in
来源：http://baike.fanxiaobao.xyz/Article/details/gskkrkxyf.sHtML

start) echo "启动" ;;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqpolrxai.sHtML

stop)  echo "停止" ;;
来源：http://baike.fanxiaobao.xyz/Article/details/gvtzkbbms.sHtML

*)     echo "未知命令" ;;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpqwkijnu.sHtML

esac
来源：http://m.share.fanxiaobao.xyz/Article/details/gmbwjziwc.sHtML

[R12] for 遍历文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkkeuhwgv.sHtML

for f in *.txt; do echo "$f"; done
来源：http://3g.fanxiaobao.xyz/Article/details/gguwcgtox.sHtML

[R13] for 计数循环
来源：http://m.share.fanxiaobao.xyz/Article/details/gwvdpzsdp.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://wap.fanxiaobao.xyz/Article/details/ggjfkizll.sHtML

[R14] C 风格 for
来源：http://read.share.fanxiaobao.xyz/Article/details/ghfdyieyw.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://blog.fanxiaobao.xyz/Article/details/gybggxqra.sHtML

[R15] while 逐行读文件
来源：http://blog.fanxiaobao.xyz/Article/details/ghefdhzqc.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gsxucbgqt.sHtML

[R16] until 等待条件
来源：http://mobile.fanxiaobao.xyz/Article/details/gcbzwdwoh.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://m.share.fanxiaobao.xyz/Article/details/goftrqtlw.sHtML

[R17] 数组定义与取值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gahcclaod.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzshmktno.sHtML

[R18] 遍历数组
来源：http://www.blog.fanxiaobao.xyz/Article/details/ganrssvlq.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdljdankh.sHtML

[R19] 数组长度
来源：http://m.share.fanxiaobao.xyz/Article/details/gzjntcfif.sHtML

echo "${#arr[@]}"
来源：http://3g.fanxiaobao.xyz/Article/details/gcigolwvr.sHtML

[R20] 关联数组（字典）
来源：http://www.share.fanxiaobao.xyz/Article/details/gtcofgijv.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://read.share.fanxiaobao.xyz/Article/details/greqjxpwa.sHtML

[R21] 字符串长度
来源：http://blog.fanxiaobao.xyz/Article/details/gqztjdgar.sHtML

echo "${#s}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gqodbloxt.sHtML

[R22] 截取子串
来源：http://baike.fanxiaobao.xyz/Article/details/gsmzyrutj.sHtML

echo "${s:0:5}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gpgcoborw.sHtML

[R23] 字符串替换
来源：http://3g.fanxiaobao.xyz/Article/details/gglimvznz.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://baike.fanxiaobao.xyz/Article/details/gvjjpxkcv.sHtML

[R24] 大小写转换
来源：http://wap.fanxiaobao.xyz/Article/details/ghnrlkkqv.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkxixoygh.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.share.fanxiaobao.xyz/Article/details/gripbexzu.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gbdehqmmb.sHtML

[R26] 命令替换
来源：http://blog.fanxiaobao.xyz/Article/details/gisdfbxyu.sHtML

now=$(date +%F); echo "$now"
来源：http://mobile.fanxiaobao.xyz/Article/details/gpzermgwt.sHtML

[R27] 算术展开
来源：http://m.share.fanxiaobao.xyz/Article/details/goacbuqgu.sHtML

echo $((1 + 2 * 3))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmdikacme.sHtML

[R28] 浮点运算
来源：http://3g.fanxiaobao.xyz/Article/details/gusrugnsg.sHtML

echo "scale=2; 10/3" | bc
来源：http://3g.fanxiaobao.xyz/Article/details/gssfrphgz.sHtML

[R29] 定义函数
来源：http://blog.fanxiaobao.xyz/Article/details/gvfbmmgcw.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.blog.fanxiaobao.xyz/Article/details/gepzsmbyl.sHtML

[R30] 函数返回状态码
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqhukygmw.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://baike.fanxiaobao.xyz/Article/details/gibmuhbnw.sHtML

[R31] 局部变量
来源：http://m.share.fanxiaobao.xyz/Article/details/ggenewtnc.sHtML

f() { local x=1; echo "$x"; }
来源：http://baike.fanxiaobao.xyz/Article/details/gsdfipizu.sHtML

[R32] 参数个数校验
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxtujhzwb.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://blog.fanxiaobao.xyz/Article/details/gdepslduw.sHtML

[R33] 捕获错误并提示行号
来源：http://mobile.fanxiaobao.xyz/Article/details/gqoddptdp.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://3g.fanxiaobao.xyz/Article/details/gnkxzipam.sHtML

[R34] 退出时清理
来源：http://www.share.fanxiaobao.xyz/Article/details/gpbfwjwkb.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://read.share.fanxiaobao.xyz/Article/details/gupcqdhkj.sHtML

[R35] 后台执行并等待
来源：http://blog.fanxiaobao.xyz/Article/details/gwseaiaah.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://m.share.fanxiaobao.xyz/Article/details/gpokjeleo.sHtML

[R36] 并发执行多个任务
来源：http://www.share.fanxiaobao.xyz/Article/details/gpaxmpguj.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqjmhiimd.sHtML

[R37] 把输出赋给变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gckldmnww.sHtML

files=$(ls -1)
来源：http://m.share.fanxiaobao.xyz/Article/details/gukgahyaw.sHtML

[R38] 管道串联
来源：http://baike.fanxiaobao.xyz/Article/details/gteqsgrso.sHtML

cat a.txt | grep -i error | wc -l
来源：http://wap.fanxiaobao.xyz/Article/details/gwhziautf.sHtML

[R39] 重定向标准输出与错误
来源：http://blog.fanxiaobao.xyz/Article/details/glmhxvobe.sHtML

cmd > out.log 2>&1
来源：http://m.share.fanxiaobao.xyz/Article/details/gfodshxbp.sHtML

[R40] 追加写日志
来源：http://www.share.fanxiaobao.xyz/Article/details/grxaggrgx.sHtML

echo "log" >> out.log
来源：http://baike.fanxiaobao.xyz/Article/details/gjynojupr.sHtML

[R41] 丢弃输出
来源：http://3g.fanxiaobao.xyz/Article/details/gdhrfpiql.sHtML

cmd >/dev/null 2>&1
来源：http://m.share.fanxiaobao.xyz/Article/details/gwozearhq.sHtML

[R42] 输入重定向
来源：http://read.share.fanxiaobao.xyz/Article/details/gytaabdnx.sHtML

wc -l < a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/grcorqehi.sHtML

[R43] 按名字查找文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gbzxcniwj.sHtML

find . -name "*.log" -type f
来源：http://mobile.fanxiaobao.xyz/Article/details/gfcrrzxsv.sHtML

[R44] 按修改时间查找
来源：http://blog.fanxiaobao.xyz/Article/details/gjggbonoe.sHtML

find . -mtime -7 -type f
来源：http://read.share.fanxiaobao.xyz/Article/details/gbttdqobe.sHtML

[R45] 批量删除
来源：http://read.share.fanxiaobao.xyz/Article/details/glysswgqq.sHtML

find . -name "*.tmp" -delete
来源：http://www.share.fanxiaobao.xyz/Article/details/gwzitkwau.sHtML

[R46] 递归替换文件内容
来源：http://www.share.fanxiaobao.xyz/Article/details/guavxlkon.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://3g.fanxiaobao.xyz/Article/details/gyngabwqj.sHtML

[R47] sed 单行替换
来源：http://read.share.fanxiaobao.xyz/Article/details/gtmidbeye.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gxvmglosh.sHtML

[R48] awk 取指定列
来源：http://mobile.fanxiaobao.xyz/Article/details/gyklyfuja.sHtML

awk '{print $1, $3}' a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gximvbijq.sHtML

[R49] awk 带条件
来源：http://wap.fanxiaobao.xyz/Article/details/gnidlzblf.sHtML


<!-- 参考信息 -->