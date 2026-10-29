代发 wailian999

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://3g.fehbvm.com/Article/details/gcmexcrxh.sHtML

[Q05] 重命名列
来源：http://www.m.share.fehbvm.com/Article/details/gsibmotqf.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://mobile.fehbvm.com/Article/details/gxttdtfrb.sHtML

[Q06] 删除列
来源：http://baike.fehbvm.com/Article/details/gpcwnvggh.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.m.share.zdbjq.cn/Article/details/gheuzdkyj.sHtML

[Q07] 删除表
来源：http://m.share.fehbvm.com/Article/details/gahylmoqp.sHtML

DROP TABLE IF EXISTS orders;
来源：http://m.share.fehbvm.com/Article/details/gwtrzqeiz.sHtML

[Q08] 创建普通索引
来源：http://www.m.share.zdbjq.cn/Article/details/gbfogsmyu.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.blog.fehbvm.com/Article/details/gszemhcvs.sHtML

[Q09] 创建唯一索引
来源：http://read.share.fehbvm.com/Article/details/gmswfozch.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://m.share.hesvh.cn/Article/details/gvqszimmw.sHtML

[Q10] 插入单行
来源：http://www.share.fehbvm.com/Article/details/gbhhcbqhq.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://read.share.fehbvm.com/Article/details/gjklhqgch.sHtML

[Q11] 一次插入多行
来源：http://www.blog.fehbvm.com/Article/details/ghsipzqhe.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.share.hesvh.cn/Article/details/gipxnhvtj.sHtML

[Q12] 插入后取自增 ID
来源：http://read.share.hesvh.cn/Article/details/gmksogenh.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://baike.zdbjq.cn/Article/details/gqgidzmge.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://blog.fehbvm.com/Article/details/gsogzhkgg.sHtML

[Q13] 忽略重复插入
来源：http://www.m.share.fehbvm.com/Article/details/gsxiabove.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://baike.zdbjq.cn/Article/details/gqwbbnrcg.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.blog.hesvh.cn/Article/details/gfililjlc.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.m.share.hesvh.cn/Article/details/gfismwgdm.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://3g.fehbvm.com/Article/details/gqfmbqzxz.sHtML

[Q15] 查询全部
来源：http://m.share.fehbvm.com/Article/details/gozejwipj.sHtML

SELECT * FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gtwongcqu.sHtML

[Q16] 查询指定列
来源：http://www.m.share.hesvh.cn/Article/details/gkhjensqh.sHtML

SELECT id, name FROM users;
来源：http://blog.fehbvm.com/Article/details/glxhqjvpx.sHtML

[Q17] 条件查询
来源：http://baike.zdbjq.cn/Article/details/ganswfnpz.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://m.share.hesvh.cn/Article/details/ggqgupcry.sHtML

[Q18] 模糊匹配
来源：http://read.share.fehbvm.com/Article/details/gxrhqjnvf.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.m.share.zdbjq.cn/Article/details/ggodgfvjn.sHtML

[Q19] 范围查询
来源：http://www.share.hesvh.cn/Article/details/gvstztwos.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://mobile.zdbjq.cn/Article/details/ghkjlpdnc.sHtML

[Q20] IN 列表
来源：http://m.share.fehbvm.com/Article/details/gveuykrtp.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://mobile.fehbvm.com/Article/details/ggsquqaxn.sHtML

[Q21] 空值判断
来源：http://m.share.zdbjq.cn/Article/details/gipvxpxnj.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.share.hesvh.cn/Article/details/guyfuscug.sHtML

[Q22] 排序
来源：http://www.m.share.zdbjq.cn/Article/details/gmegzarpt.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://baike.fehbvm.com/Article/details/gsnwfjnqz.sHtML

[Q23] 分页
来源：http://3g.hesvh.cn/Article/details/gtbmdnijn.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.blog.fehbvm.com/Article/details/gxpwwfuih.sHtML

[Q24] 去重
来源：http://www.m.share.zdbjq.cn/Article/details/gzbzromjb.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gxurtepqw.sHtML

[Q25] 只取前 N 条
来源：http://blog.zdbjq.cn/Article/details/ggvgqvepn.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.share.hesvh.cn/Article/details/gxrqhkkmc.sHtML

[Q26] 计数
来源：http://baike.zdbjq.cn/Article/details/gawkgoadq.sHtML

SELECT COUNT(*) FROM users;
来源：http://blog.hesvh.cn/Article/details/gqwtylsmw.sHtML

[Q27] 条件计数
来源：http://blog.zdbjq.cn/Article/details/gualxfhmu.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gztaofgzm.sHtML

[Q28] 求和与平均
来源：http://www.m.share.fehbvm.com/Article/details/gimjvnlno.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://mobile.fehbvm.com/Article/details/grnobnfhn.sHtML

[Q29] 最大最小值
来源：http://m.share.hesvh.cn/Article/details/gojgcubhb.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://mobile.zdbjq.cn/Article/details/goiodjmwo.sHtML

[Q30] 分组统计
来源：http://www.m.share.fehbvm.com/Article/details/givywvjkd.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.m.share.zdbjq.cn/Article/details/gtivlmazj.sHtML

[Q31] 分组后过滤
来源：http://3g.zdbjq.cn/Article/details/gdcjlgxbp.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://mobile.hesvh.cn/Article/details/grjmifwzk.sHtML

[Q32] 分组拼接字符串
来源：http://m.share.hesvh.cn/Article/details/gbmuzcvmu.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://blog.fehbvm.com/Article/details/gbfvtuefm.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.m.share.hesvh.cn/Article/details/gwfqxgvyb.sHtML

[Q33] 多列分组
来源：http://www.share.fehbvm.com/Article/details/gxubrlgcu.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://wap.hesvh.cn/Article/details/guzughygi.sHtML

[Q34] 每组取第一条
来源：http://blog.fehbvm.com/Article/details/gxjklwfrk.sHtML

SELECT * FROM (
来源：http://mobile.zdbjq.cn/Article/details/gsalquqaq.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://wap.fehbvm.com/Article/details/gxpapnyau.sHtML

) t WHERE rn = 1;
来源：http://m.share.zdbjq.cn/Article/details/gxmotqtnt.sHtML

[Q35] 内连接
来源：http://blog.fehbvm.com/Article/details/gofpyyjqi.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://blog.zdbjq.cn/Article/details/guieelyvw.sHtML

[Q36] 左连接
来源：http://mobile.hesvh.cn/Article/details/gupmbcpwe.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://m.share.hesvh.cn/Article/details/gvqvikxva.sHtML

[Q37] 右连接
来源：http://www.m.share.hesvh.cn/Article/details/gxhnivygw.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://baike.hesvh.cn/Article/details/gyvfdyglt.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://blog.fehbvm.com/Article/details/ghhrejyum.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.share.hesvh.cn/Article/details/gurrpspsp.sHtML

[Q39] 自连接（查上下级）
来源：http://baike.fehbvm.com/Article/details/gsrenwarf.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.m.share.zdbjq.cn/Article/details/gzvuqtjos.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://m.share.zdbjq.cn/Article/details/gzrztqpvj.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://read.share.fehbvm.com/Article/details/gpktvsqkt.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://3g.fehbvm.com/Article/details/gwuorocqv.sHtML

[Q41] 多表连接
来源：http://wap.fehbvm.com/Article/details/gegsakrbf.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://blog.hesvh.cn/Article/details/gjwarqltj.sHtML

JOIN users u ON u.id = o.user_id
来源：http://3g.zdbjq.cn/Article/details/gdtnkrija.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://read.share.fehbvm.com/Article/details/ghkikbwnd.sHtML

[Q42] 连接条件附加过滤
来源：http://baike.fehbvm.com/Article/details/gfdyfhxsv.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.blog.hesvh.cn/Article/details/gebdjamkx.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://blog.zdbjq.cn/Article/details/gfijdngvy.sHtML

[Q43] 标量子查询
来源：http://3g.fehbvm.com/Article/details/greiooywc.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://baike.fehbvm.com/Article/details/gffqpbzzr.sHtML

[Q44] IN 子查询
来源：http://3g.fehbvm.com/Article/details/gcqkijvta.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://m.share.fehbvm.com/Article/details/gylrtkfze.sHtML

[Q45] EXISTS 判断存在
来源：http://baike.fehbvm.com/Article/details/gwuxonrta.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.zdbjq.cn/Article/details/ggmkjlktd.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://m.share.hesvh.cn/Article/details/gmwmoqpfm.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.hesvh.cn/Article/details/gahagsdca.sHtML

[Q47] 与平均值比较
来源：http://www.blog.fehbvm.com/Article/details/glpznaqtm.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://wap.hesvh.cn/Article/details/gawsupdhm.sHtML

[Q48] CTE 公用表表达式
来源：http://3g.zdbjq.cn/Article/details/gswexreyn.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.blog.fehbvm.com/Article/details/grkqacbag.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.blog.fehbvm.com/Article/details/giluhiucm.sHtML

[Q49] 更新单行
来源：http://www.share.hesvh.cn/Article/details/glbzkjphr.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://read.share.hesvh.cn/Article/details/gnwjzclrl.sHtML

[Q50] 批量更新
来源：http://www.share.fehbvm.com/Article/details/guqkljbhe.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://3g.hesvh.cn/Article/details/ghvjwmjnl.sHtML

[Q51] 用子查询更新
来源：http://mobile.fehbvm.com/Article/details/gzsrnxzyy.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://read.share.zdbjq.cn/Article/details/gpfexjngo.sHtML

[Q52] 删除指定行
来源：http://m.share.fehbvm.com/Article/details/gcbhbhyzt.sHtML

DELETE FROM users WHERE id = 10;
来源：http://blog.hesvh.cn/Article/details/gxfuqdkri.sHtML

[Q53] 按条件删除
来源：http://blog.zdbjq.cn/Article/details/golonadbr.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://3g.fehbvm.com/Article/details/gtesjajqp.sHtML

[Q54] 清空表
来源：http://mobile.hesvh.cn/Article/details/gwehlvrii.sHtML

TRUNCATE TABLE logs;
来源：http://m.share.fehbvm.com/Article/details/gyvqjxwjv.sHtML

[Q55] 排名（并列占位）
来源：http://www.share.fehbvm.com/Article/details/gjbpjhqbu.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://read.share.fehbvm.com/Article/details/gaehcpfqx.sHtML

[Q56] 密集排名（并列不占位）
来源：http://baike.hesvh.cn/Article/details/gcolpjbjl.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.blog.fehbvm.com/Article/details/gcxoabujg.sHtML

[Q57] 行号
来源：http://www.share.fehbvm.com/Article/details/gkeyoaxmz.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/ghbvrscvo.sHtML

[Q58] 累计求和
来源：http://mobile.zdbjq.cn/Article/details/ghwbmurfi.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://wap.zdbjq.cn/Article/details/gsarblcup.sHtML

[Q59] 分组内累计
来源：http://baike.zdbjq.cn/Article/details/gytaoodiz.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://3g.hesvh.cn/Article/details/goouwqjme.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.share.zdbjq.cn/Article/details/gkbmcontv.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.blog.hesvh.cn/Article/details/gpjpvwnvf.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://3g.zdbjq.cn/Article/details/gccaugbft.sHtML

[Q61] 移动平均
来源：http://wap.hesvh.cn/Article/details/gwvsjinvq.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://3g.hesvh.cn/Article/details/gjtsxtxyb.sHtML

[Q62] 分组占比
来源：http://www.blog.hesvh.cn/Article/details/gerpjpivg.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://mobile.fehbvm.com/Article/details/gwnqjxbfh.sHtML

[Q63] 开启事务
来源：http://www.blog.zdbjq.cn/Article/details/gibpfumue.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://read.share.hesvh.cn/Article/details/gmefcsvcm.sHtML

[Q64] 提交事务
来源：http://wap.zdbjq.cn/Article/details/gvwnxdfrl.sHtML

COMMIT;
来源：http://blog.fehbvm.com/Article/details/gytncletn.sHtML

[Q65] 回滚事务
来源：http://www.blog.zdbjq.cn/Article/details/gdynxtuia.sHtML

ROLLBACK;
来源：http://3g.fehbvm.com/Article/details/gibsqzhbd.sHtML

[Q66] 行锁查询
来源：http://3g.fehbvm.com/Article/details/gvgmovggl.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://3g.hesvh.cn/Article/details/gulgvyser.sHtML

[Q67] 设置隔离级别
来源：http://www.m.share.zdbjq.cn/Article/details/gjmslislo.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://3g.hesvh.cn/Article/details/gpdheuyea.sHtML

[Q68] 保存点
来源：http://www.share.zdbjq.cn/Article/details/glodkeuum.sHtML

SAVEPOINT sp1;
来源：http://mobile.fehbvm.com/Article/details/gxalskeqm.sHtML

ROLLBACK TO sp1;
来源：http://baike.fehbvm.com/Article/details/gmpisnphk.sHtML

[Q69] 查看执行计划
来源：http://www.blog.fehbvm.com/Article/details/grpzruliw.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://3g.zdbjq.cn/Article/details/gjwfoxcyj.sHtML

[Q70] 更新统计信息
来源：http://www.blog.fehbvm.com/Article/details/gcrlmhara.sHtML

ANALYZE TABLE users;
来源：http://mobile.hesvh.cn/Article/details/gcnzxnmvs.sHtML

[Q71] 查看建表语句
来源：http://www.m.share.hesvh.cn/Article/details/guiyprvfp.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.m.share.fehbvm.com/Article/details/glszdmbnw.sHtML

[Q72] 查看索引
来源：http://mobile.zdbjq.cn/Article/details/ggnoirpaf.sHtML

SHOW INDEX FROM users;
来源：http://www.share.hesvh.cn/Article/details/gsolzktmd.sHtML

[Q73] 查看表状态
来源：http://www.blog.fehbvm.com/Article/details/gzzibewtz.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.share.zdbjq.cn/Article/details/gqoiqtabx.sHtML

[Q74] 强制使用索引
来源：http://blog.zdbjq.cn/Article/details/gqucpgyjg.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://read.share.zdbjq.cn/Article/details/gvoxwmobm.sHtML

[Q75] 日期格式化
来源：http://www.share.fehbvm.com/Article/details/ghpydhueq.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://m.share.zdbjq.cn/Article/details/gohqtaumy.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://read.share.zdbjq.cn/Article/details/glxscxjqd.sHtML

[Q76] 按天统计
来源：http://baike.zdbjq.cn/Article/details/gccjtejoh.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://baike.zdbjq.cn/Article/details/gxsghbmgh.sHtML

[Q77] 时间加减
来源：http://www.m.share.hesvh.cn/Article/details/ghtehxhfs.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://wap.fehbvm.com/Article/details/ghgyucsbo.sHtML

[Q78] 当前时间
来源：http://wap.fehbvm.com/Article/details/gjutoqlgb.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://blog.hesvh.cn/Article/details/gjhjjhsjf.sHtML

[Q79] 字符串拼接
来源：http://www.m.share.zdbjq.cn/Article/details/gnhzcjnnx.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://read.share.zdbjq.cn/Article/details/ggbaubjig.sHtML

[Q80] 字符串截取
来源：http://baike.fehbvm.com/Article/details/gggitsmmi.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://read.share.fehbvm.com/Article/details/glbxndaes.sHtML

[Q81] 字符串替换
来源：http://m.share.zdbjq.cn/Article/details/gcjyojthg.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://m.share.hesvh.cn/Article/details/goueprewz.sHtML

[Q82] 字符长度与字节长度
来源：http://m.share.zdbjq.cn/Article/details/gfyjgwkkj.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://wap.fehbvm.com/Article/details/gpkngdqcu.sHtML

[Q83] 大小写转换
来源：http://blog.fehbvm.com/Article/details/gjdwgjcke.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.share.fehbvm.com/Article/details/gbjugbvar.sHtML

[Q84] 去除首尾空格
来源：http://3g.hesvh.cn/Article/details/gpexumbfp.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gywgsrjzu.sHtML

[Q85] 数值取整
来源：http://3g.fehbvm.com/Article/details/gdykjrktw.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://baike.hesvh.cn/Article/details/gqyvpnbuj.sHtML

[Q86] 读取 JSON 字段
来源：http://www.m.share.zdbjq.cn/Article/details/gcpnbqfkw.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.share.hesvh.cn/Article/details/gtyruxlfj.sHtML

[Q87] JSON 字段做条件
来源：http://www.share.hesvh.cn/Article/details/gfqqetfql.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.blog.zdbjq.cn/Article/details/ggpybeuyr.sHtML

[Q88] 行转列（条件聚合）
来源：http://baike.fehbvm.com/Article/details/gcdblcqbb.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.share.hesvh.cn/Article/details/gzmnhhcgy.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gilywtnnr.sHtML

[Q89] 判断表是否存在
来源：http://www.m.share.hesvh.cn/Article/details/gncsfhjxf.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://read.share.hesvh.cn/Article/details/gcquasnkc.sHtML

[Q90] 生成序号列
来源：http://read.share.hesvh.cn/Article/details/gjrinjgsc.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://wap.hesvh.cn/Article/details/gabwkakso.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gejektkjy.sHtML

R. Bash 专题
来源：http://www.share.zdbjq.cn/Article/details/gxartnmnu.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gxisvpuli.sHtML

[R01] shebang 与严格模式
来源：http://3g.hesvh.cn/Article/details/ghizmogxs.sHtML

#!/usr/bin/env bash
来源：http://www.m.share.hesvh.cn/Article/details/gvgybvrpy.sHtML

set -euo pipefail
来源：http://baike.fehbvm.com/Article/details/ggyvmuagp.sHtML

[R02] 变量赋值与使用
来源：http://www.m.share.fehbvm.com/Article/details/goczvieub.sHtML

name="Tom"; echo "$name"
来源：http://blog.zdbjq.cn/Article/details/gltqluhfr.sHtML

[R03] 只读变量
来源：http://mobile.hesvh.cn/Article/details/gxgmnpzoy.sHtML

readonly PI=3.14
来源：http://www.share.zdbjq.cn/Article/details/gvlkqqrtu.sHtML

[R04] 位置参数
来源：http://www.m.share.hesvh.cn/Article/details/grszlhdnx.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://blog.hesvh.cn/Article/details/gmycpvddu.sHtML

[R05] 参数默认值
来源：http://www.blog.fehbvm.com/Article/details/gzzqyaxur.sHtML

name="${1:-default}"
来源：http://www.m.share.zdbjq.cn/Article/details/grguipttj.sHtML

[R06] 判断命令是否存在
来源：http://read.share.zdbjq.cn/Article/details/grdjwjzer.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://mobile.zdbjq.cn/Article/details/ggwaqspji.sHtML

[R07] if 判断文件
来源：http://www.blog.fehbvm.com/Article/details/gcqkmdywv.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://blog.zdbjq.cn/Article/details/gckqhetqd.sHtML

[R08] 数值比较
来源：http://blog.hesvh.cn/Article/details/gykxlugvm.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://blog.zdbjq.cn/Article/details/gsodxesou.sHtML

[R09] 字符串比较
来源：http://www.share.zdbjq.cn/Article/details/gvjthszud.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://mobile.zdbjq.cn/Article/details/gsjdajvma.sHtML

[R10] 正则匹配
来源：http://read.share.hesvh.cn/Article/details/grverrfoc.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://3g.fehbvm.com/Article/details/gllbsmwky.sHtML

[R11] case 多分支
来源：http://3g.zdbjq.cn/Article/details/geagoaojb.sHtML

case "$1" in
来源：http://www.share.zdbjq.cn/Article/details/gfsxpkqsl.sHtML

start) echo "启动" ;;
来源：http://blog.fehbvm.com/Article/details/glgjmjzvi.sHtML

stop)  echo "停止" ;;
来源：http://blog.hesvh.cn/Article/details/ggdcpivnj.sHtML

*)     echo "未知命令" ;;
来源：http://3g.hesvh.cn/Article/details/gnjpxawxo.sHtML

esac
来源：http://blog.zdbjq.cn/Article/details/gljqfagiz.sHtML

[R12] for 遍历文件
来源：http://www.blog.fehbvm.com/Article/details/gzmcpvgzd.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.share.fehbvm.com/Article/details/gmongxjed.sHtML

[R13] for 计数循环
来源：http://www.m.share.hesvh.cn/Article/details/grsagvqjb.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://read.share.hesvh.cn/Article/details/gxdeujyws.sHtML

[R14] C 风格 for
来源：http://m.share.zdbjq.cn/Article/details/gpavekaap.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.m.share.fehbvm.com/Article/details/gmwyualvk.sHtML

[R15] while 逐行读文件
来源：http://baike.zdbjq.cn/Article/details/gjkpxtfxg.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://baike.zdbjq.cn/Article/details/gvjcyyzkx.sHtML

[R16] until 等待条件
来源：http://3g.hesvh.cn/Article/details/gqrevrngz.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://read.share.zdbjq.cn/Article/details/gyjdlpflf.sHtML

[R17] 数组定义与取值
来源：http://wap.fehbvm.com/Article/details/gyiqzjvdb.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://wap.zdbjq.cn/Article/details/gffleggno.sHtML

[R18] 遍历数组
来源：http://baike.fehbvm.com/Article/details/gufwkwdjt.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.blog.hesvh.cn/Article/details/gloxxyelv.sHtML

[R19] 数组长度
来源：http://www.m.share.zdbjq.cn/Article/details/geettprke.sHtML

echo "${#arr[@]}"
来源：http://m.share.hesvh.cn/Article/details/gcawaqeux.sHtML

[R20] 关联数组（字典）
来源：http://blog.zdbjq.cn/Article/details/ghkbewhnq.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://baike.zdbjq.cn/Article/details/gnspewcuu.sHtML

[R21] 字符串长度
来源：http://mobile.zdbjq.cn/Article/details/gxzeaubmv.sHtML

echo "${#s}"
来源：http://www.m.share.hesvh.cn/Article/details/gadtuuugl.sHtML

[R22] 截取子串
来源：http://www.m.share.fehbvm.com/Article/details/gqoykysns.sHtML

echo "${s:0:5}"
来源：http://baike.fehbvm.com/Article/details/gsqnkapuy.sHtML

[R23] 字符串替换
来源：http://blog.hesvh.cn/Article/details/gbtoezcxr.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://baike.hesvh.cn/Article/details/gdnegaseo.sHtML

[R24] 大小写转换
来源：http://mobile.hesvh.cn/Article/details/gtwfvidjx.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://mobile.hesvh.cn/Article/details/gxocarmnq.sHtML

[R25] 去后缀 / 去前缀
来源：http://read.share.fehbvm.com/Article/details/glwwvbiin.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.blog.zdbjq.cn/Article/details/gganfmrau.sHtML

[R26] 命令替换
来源：http://mobile.hesvh.cn/Article/details/gpralouid.sHtML

now=$(date +%F); echo "$now"
来源：http://mobile.zdbjq.cn/Article/details/gqzbrwmey.sHtML

[R27] 算术展开
来源：http://mobile.hesvh.cn/Article/details/gbagkzves.sHtML

echo $((1 + 2 * 3))
来源：http://www.share.fehbvm.com/Article/details/gifhpieja.sHtML

[R28] 浮点运算
来源：http://www.share.fehbvm.com/Article/details/gmlbdsrje.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.m.share.hesvh.cn/Article/details/gcaizsrfy.sHtML

[R29] 定义函数
来源：http://www.share.hesvh.cn/Article/details/gthavwmnd.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.blog.hesvh.cn/Article/details/gwapqgqgq.sHtML

[R30] 函数返回状态码
来源：http://3g.hesvh.cn/Article/details/gjklqykjw.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://wap.zdbjq.cn/Article/details/gthhwcntl.sHtML

[R31] 局部变量
来源：http://baike.zdbjq.cn/Article/details/glfabwolr.sHtML

f() { local x=1; echo "$x"; }
来源：http://m.share.zdbjq.cn/Article/details/gdvvcahbj.sHtML

[R32] 参数个数校验
来源：http://m.share.hesvh.cn/Article/details/gbxlsnejr.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.blog.fehbvm.com/Article/details/gfugvszpt.sHtML

[R33] 捕获错误并提示行号
来源：http://www.m.share.zdbjq.cn/Article/details/gbymwrvye.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://m.share.zdbjq.cn/Article/details/gkrykvvcn.sHtML

[R34] 退出时清理
来源：http://blog.fehbvm.com/Article/details/grlhoxnvv.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.share.hesvh.cn/Article/details/gknvzlbuc.sHtML

[R35] 后台执行并等待
来源：http://www.blog.zdbjq.cn/Article/details/gdxmdpyrx.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.blog.hesvh.cn/Article/details/ggekxtsyk.sHtML

[R36] 并发执行多个任务
来源：http://baike.fehbvm.com/Article/details/gwipocjqb.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://baike.zdbjq.cn/Article/details/gyycfarsk.sHtML

[R37] 把输出赋给变量
来源：http://mobile.fehbvm.com/Article/details/gymuhrjfl.sHtML

files=$(ls -1)
来源：http://mobile.hesvh.cn/Article/details/gbyfpnqgo.sHtML

[R38] 管道串联
来源：http://baike.hesvh.cn/Article/details/gjzlsydmm.sHtML

cat a.txt | grep -i error | wc -l
来源：http://3g.zdbjq.cn/Article/details/ggethjhwc.sHtML

[R39] 重定向标准输出与错误
来源：http://mobile.fehbvm.com/Article/details/gfluzvcou.sHtML

cmd > out.log 2>&1
来源：http://baike.zdbjq.cn/Article/details/grdwdyfuq.sHtML

[R40] 追加写日志
来源：http://baike.hesvh.cn/Article/details/gfsphjisv.sHtML

echo "log" >> out.log
来源：http://blog.hesvh.cn/Article/details/ganvlpyqp.sHtML

[R41] 丢弃输出
来源：http://wap.fehbvm.com/Article/details/gqsvbxunt.sHtML

cmd >/dev/null 2>&1
来源：http://baike.zdbjq.cn/Article/details/gkmqkaavl.sHtML

[R42] 输入重定向
来源：http://blog.fehbvm.com/Article/details/gntdghqjo.sHtML

wc -l < a.txt
来源：http://read.share.hesvh.cn/Article/details/gpmcibtdq.sHtML

[R43] 按名字查找文件
来源：http://mobile.hesvh.cn/Article/details/gxfcrdtnf.sHtML

find . -name "*.log" -type f
来源：http://blog.zdbjq.cn/Article/details/gpoxqboke.sHtML

[R44] 按修改时间查找
来源：http://www.m.share.fehbvm.com/Article/details/gxzyvoguc.sHtML

find . -mtime -7 -type f
来源：http://www.blog.zdbjq.cn/Article/details/gcsssgvas.sHtML

[R45] 批量删除
来源：http://blog.fehbvm.com/Article/details/gnahnykof.sHtML

find . -name "*.tmp" -delete
来源：http://read.share.fehbvm.com/Article/details/gluzuaufe.sHtML

[R46] 递归替换文件内容
来源：http://m.share.fehbvm.com/Article/details/gyvkgdjhn.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://m.share.zdbjq.cn/Article/details/gkxxfseir.sHtML

[R47] sed 单行替换
来源：http://www.share.fehbvm.com/Article/details/ghxanhomg.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://wap.fehbvm.com/Article/details/gqiooceed.sHtML

[R48] awk 取指定列
来源：http://www.m.share.fehbvm.com/Article/details/gdokutcgs.sHtML

awk '{print $1, $3}' a.txt
来源：http://m.share.fehbvm.com/Article/details/gmedxjmlg.sHtML

[R49] awk 带条件
来源：http://wap.zdbjq.cn/Article/details/gxxhwptso.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://read.share.fehbvm.com/Article/details/glgebgxvp.sHtML

[R50] awk 求和
来源：http://3g.zdbjq.cn/Article/details/gytsbafeb.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://baike.hesvh.cn/Article/details/giltwniec.sHtML

[R51] 排序去重取前几
来源：http://wap.zdbjq.cn/Article/details/gfiyzkhly.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://mobile.fehbvm.com/Article/details/gvrwqhlxz.sHtML

[R52] 统计行数
来源：http://www.m.share.fehbvm.com/Article/details/gngqclrxc.sHtML

wc -l a.txt
来源：http://www.m.share.hesvh.cn/Article/details/gfognhywf.sHtML

[R53] 查看文件头与实时尾
来源：http://3g.fehbvm.com/Article/details/gqelcykgb.sHtML


<!-- 参考信息 -->