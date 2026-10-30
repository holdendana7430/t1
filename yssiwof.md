代发 wailian999

CREATE TABLE users (
来源：http://blog.hesvh.cn/Article/details/gpyjpzkfg.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.share.zdbjq.cn/Article/details/girqeqfeu.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.m.share.zdbjq.cn/Article/details/gliyxsupb.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.blog.fehbvm.com/Article/details/gwnngjvit.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://m.share.hesvh.cn/Article/details/gcsucddye.sHtML

);
来源：http://mobile.zdbjq.cn/Article/details/ghthqksod.sHtML

[Q02] 创建带外键的表
来源：http://www.m.share.zdbjq.cn/Article/details/gfeckigyk.sHtML

CREATE TABLE orders (
来源：http://mobile.fehbvm.com/Article/details/govjipjjg.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.fehbvm.com/Article/details/guoblharc.sHtML

user_id INT NOT NULL,
来源：http://mobile.fehbvm.com/Article/details/geprcfncv.sHtML

amount DECIMAL(10, 2),
来源：http://3g.zdbjq.cn/Article/details/gmwrxhyii.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://blog.zdbjq.cn/Article/details/gaqedhvyn.sHtML

);
来源：http://read.share.fehbvm.com/Article/details/gvfpdbxtg.sHtML

[Q03] 增加列
来源：http://blog.hesvh.cn/Article/details/gjhmeornv.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.m.share.hesvh.cn/Article/details/gviumcype.sHtML

[Q04] 修改列类型
来源：http://baike.zdbjq.cn/Article/details/gxlbqzsof.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://3g.fehbvm.com/Article/details/gqjoaoext.sHtML

[Q05] 重命名列
来源：http://baike.hesvh.cn/Article/details/gdqnqjmhk.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://wap.fehbvm.com/Article/details/grleqfidd.sHtML

[Q06] 删除列
来源：http://www.m.share.zdbjq.cn/Article/details/gtmlpsqkd.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://wap.fehbvm.com/Article/details/gtbwkakwj.sHtML

[Q07] 删除表
来源：http://3g.zdbjq.cn/Article/details/gvhxshbfw.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.blog.zdbjq.cn/Article/details/gvghopdcn.sHtML

[Q08] 创建普通索引
来源：http://3g.hesvh.cn/Article/details/gloelmblo.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.share.zdbjq.cn/Article/details/gepvmvwsp.sHtML

[Q09] 创建唯一索引
来源：http://mobile.fehbvm.com/Article/details/gmpxgaoko.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://wap.fehbvm.com/Article/details/gqblrnriv.sHtML

[Q10] 插入单行
来源：http://baike.zdbjq.cn/Article/details/gsqgfjhma.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://baike.zdbjq.cn/Article/details/gsvzjuyum.sHtML

[Q11] 一次插入多行
来源：http://www.m.share.zdbjq.cn/Article/details/gqkllczkf.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://mobile.hesvh.cn/Article/details/gpuhdggxf.sHtML

[Q12] 插入后取自增 ID
来源：http://www.share.hesvh.cn/Article/details/gtvwklggs.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.share.zdbjq.cn/Article/details/grxjempzs.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://3g.zdbjq.cn/Article/details/gprkbvczi.sHtML

[Q13] 忽略重复插入
来源：http://3g.hesvh.cn/Article/details/gkynqunsz.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.share.hesvh.cn/Article/details/gxbjalxtu.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.share.zdbjq.cn/Article/details/ggdsdqaib.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://mobile.hesvh.cn/Article/details/gxkqvxkom.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://blog.hesvh.cn/Article/details/gmjnytxao.sHtML

[Q15] 查询全部
来源：http://mobile.hesvh.cn/Article/details/gwycjvahm.sHtML

SELECT * FROM users;
来源：http://www.share.fehbvm.com/Article/details/ggppelhud.sHtML

[Q16] 查询指定列
来源：http://www.blog.zdbjq.cn/Article/details/gyheizoww.sHtML

SELECT id, name FROM users;
来源：http://read.share.fehbvm.com/Article/details/gpsulxsao.sHtML

[Q17] 条件查询
来源：http://3g.hesvh.cn/Article/details/gvoianaxm.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://m.share.hesvh.cn/Article/details/gyjhsdxwb.sHtML

[Q18] 模糊匹配
来源：http://mobile.fehbvm.com/Article/details/gcqumsblp.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://wap.zdbjq.cn/Article/details/gmngfrfhz.sHtML

[Q19] 范围查询
来源：http://www.m.share.zdbjq.cn/Article/details/guwheicwk.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://read.share.zdbjq.cn/Article/details/gqlseenng.sHtML

[Q20] IN 列表
来源：http://www.m.share.hesvh.cn/Article/details/gpgjbriqy.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://m.share.zdbjq.cn/Article/details/ggwmfdtme.sHtML

[Q21] 空值判断
来源：http://3g.fehbvm.com/Article/details/gdylqseco.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://blog.zdbjq.cn/Article/details/gajouxttb.sHtML

[Q22] 排序
来源：http://3g.zdbjq.cn/Article/details/gimneluws.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.blog.hesvh.cn/Article/details/gmnwkpzur.sHtML

[Q23] 分页
来源：http://m.share.fehbvm.com/Article/details/gysrbowqx.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.share.fehbvm.com/Article/details/gheuyqlsh.sHtML

[Q24] 去重
来源：http://www.blog.zdbjq.cn/Article/details/gzwztecaq.sHtML

SELECT DISTINCT city FROM users;
来源：http://wap.fehbvm.com/Article/details/ghvaeyuct.sHtML

[Q25] 只取前 N 条
来源：http://www.blog.fehbvm.com/Article/details/gnuedimok.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://baike.fehbvm.com/Article/details/grgibiagk.sHtML

[Q26] 计数
来源：http://blog.zdbjq.cn/Article/details/gsjnnljpl.sHtML

SELECT COUNT(*) FROM users;
来源：http://3g.hesvh.cn/Article/details/gtadmepmb.sHtML

[Q27] 条件计数
来源：http://m.share.zdbjq.cn/Article/details/ghzxknzeg.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://mobile.fehbvm.com/Article/details/gvhhffglt.sHtML

[Q28] 求和与平均
来源：http://3g.fehbvm.com/Article/details/gyenakzyn.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://read.share.fehbvm.com/Article/details/gsrwuhllw.sHtML

[Q29] 最大最小值
来源：http://mobile.zdbjq.cn/Article/details/gpkztaqpb.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://wap.zdbjq.cn/Article/details/gqelkbiox.sHtML

[Q30] 分组统计
来源：http://read.share.fehbvm.com/Article/details/gkybxkcxl.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://mobile.zdbjq.cn/Article/details/ggatutjsg.sHtML

[Q31] 分组后过滤
来源：http://wap.fehbvm.com/Article/details/gtdnougmr.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://blog.hesvh.cn/Article/details/guoixphyk.sHtML

[Q32] 分组拼接字符串
来源：http://www.blog.hesvh.cn/Article/details/ggiifbllm.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.blog.hesvh.cn/Article/details/gmqroxrlz.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://m.share.hesvh.cn/Article/details/gwpenimjz.sHtML

[Q33] 多列分组
来源：http://3g.fehbvm.com/Article/details/gjdjjoixz.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.blog.zdbjq.cn/Article/details/gfmbworni.sHtML

[Q34] 每组取第一条
来源：http://www.m.share.hesvh.cn/Article/details/gdzduytwp.sHtML

SELECT * FROM (
来源：http://wap.fehbvm.com/Article/details/gbtulvthg.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://m.share.fehbvm.com/Article/details/gzxybwsrz.sHtML

) t WHERE rn = 1;
来源：http://blog.fehbvm.com/Article/details/geqoehwgh.sHtML

[Q35] 内连接
来源：http://www.blog.hesvh.cn/Article/details/gvtewttmq.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://3g.hesvh.cn/Article/details/gdgllcuog.sHtML

[Q36] 左连接
来源：http://m.share.fehbvm.com/Article/details/grbvjshpz.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://baike.fehbvm.com/Article/details/gzgodramy.sHtML

[Q37] 右连接
来源：http://www.share.zdbjq.cn/Article/details/gdijdstbd.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://blog.hesvh.cn/Article/details/gmfwaydqk.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://blog.fehbvm.com/Article/details/gzjavztwa.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://3g.zdbjq.cn/Article/details/gazmitnhg.sHtML

[Q39] 自连接（查上下级）
来源：http://www.blog.zdbjq.cn/Article/details/gzsiccehr.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://mobile.zdbjq.cn/Article/details/gsugvqcgc.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://baike.hesvh.cn/Article/details/gfawengcz.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://mobile.fehbvm.com/Article/details/gyatuamqu.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://wap.hesvh.cn/Article/details/gdaytqkuv.sHtML

[Q41] 多表连接
来源：http://baike.hesvh.cn/Article/details/gcvgiunud.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.blog.zdbjq.cn/Article/details/gvqfgjecv.sHtML

JOIN users u ON u.id = o.user_id
来源：http://wap.hesvh.cn/Article/details/gyhqvcpyx.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.share.fehbvm.com/Article/details/ggseiqwhq.sHtML

[Q42] 连接条件附加过滤
来源：http://m.share.fehbvm.com/Article/details/gpzisxjfu.sHtML

SELECT u.name, o.amount FROM users u
来源：http://read.share.hesvh.cn/Article/details/ggxtesqjg.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://mobile.zdbjq.cn/Article/details/gowaxxypw.sHtML

[Q43] 标量子查询
来源：http://read.share.zdbjq.cn/Article/details/gxenmvqdg.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://read.share.zdbjq.cn/Article/details/gxzeizjwt.sHtML

[Q44] IN 子查询
来源：http://m.share.zdbjq.cn/Article/details/gxucyvish.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://m.share.zdbjq.cn/Article/details/gwqsdukna.sHtML

[Q45] EXISTS 判断存在
来源：http://mobile.hesvh.cn/Article/details/gvnmaawtr.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.hesvh.cn/Article/details/gzniosyxp.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.m.share.fehbvm.com/Article/details/glwifwfue.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.zdbjq.cn/Article/details/ganxacvlw.sHtML

[Q47] 与平均值比较
来源：http://www.blog.zdbjq.cn/Article/details/gkgilarqf.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.blog.hesvh.cn/Article/details/gcqzomebd.sHtML

[Q48] CTE 公用表表达式
来源：http://www.blog.zdbjq.cn/Article/details/gturldyfx.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.share.zdbjq.cn/Article/details/gimbaycta.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.share.fehbvm.com/Article/details/gvkxmlqrk.sHtML

[Q49] 更新单行
来源：http://blog.fehbvm.com/Article/details/gkhdjclzx.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://mobile.hesvh.cn/Article/details/gkyzepcyi.sHtML

[Q50] 批量更新
来源：http://m.share.fehbvm.com/Article/details/gujseyceb.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://read.share.hesvh.cn/Article/details/govmfnlkt.sHtML

[Q51] 用子查询更新
来源：http://www.blog.zdbjq.cn/Article/details/gmdqlhynr.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://blog.zdbjq.cn/Article/details/gxbfqphpd.sHtML

[Q52] 删除指定行
来源：http://read.share.zdbjq.cn/Article/details/gbtrtxebo.sHtML

DELETE FROM users WHERE id = 10;
来源：http://read.share.zdbjq.cn/Article/details/gkhaqtgpr.sHtML

[Q53] 按条件删除
来源：http://baike.hesvh.cn/Article/details/gkgbonxpz.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://read.share.zdbjq.cn/Article/details/ggqiahvym.sHtML

[Q54] 清空表
来源：http://www.share.hesvh.cn/Article/details/gdwgzwjkj.sHtML

TRUNCATE TABLE logs;
来源：http://www.share.fehbvm.com/Article/details/gbkwgfihk.sHtML

[Q55] 排名（并列占位）
来源：http://3g.zdbjq.cn/Article/details/glnewvoit.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.share.zdbjq.cn/Article/details/gtvtgmiha.sHtML

[Q56] 密集排名（并列不占位）
来源：http://baike.hesvh.cn/Article/details/gkjuweoat.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://read.share.zdbjq.cn/Article/details/gyyyvhggz.sHtML

[Q57] 行号
来源：http://www.share.fehbvm.com/Article/details/gmtcqgqxf.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gtwqcpzzw.sHtML

[Q58] 累计求和
来源：http://www.share.hesvh.cn/Article/details/gvgcagcvk.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://read.share.hesvh.cn/Article/details/gjmxauumd.sHtML

[Q59] 分组内累计
来源：http://3g.hesvh.cn/Article/details/gndqmxxqm.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://3g.fehbvm.com/Article/details/gqlqybtqc.sHtML

[Q60] 取上一行 / 下一行
来源：http://m.share.hesvh.cn/Article/details/gebdfogxw.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://mobile.hesvh.cn/Article/details/gvlkvfces.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://baike.zdbjq.cn/Article/details/ggjkyxmai.sHtML

[Q61] 移动平均
来源：http://www.m.share.zdbjq.cn/Article/details/gwvkxpkxj.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://wap.hesvh.cn/Article/details/grwkhtmvp.sHtML

[Q62] 分组占比
来源：http://mobile.hesvh.cn/Article/details/gpxumscsw.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://mobile.zdbjq.cn/Article/details/gngxsyqjy.sHtML

[Q63] 开启事务
来源：http://www.blog.zdbjq.cn/Article/details/gfpxfjior.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.blog.fehbvm.com/Article/details/gaqyrjqce.sHtML

[Q64] 提交事务
来源：http://www.m.share.hesvh.cn/Article/details/gebqbgfqn.sHtML

COMMIT;
来源：http://3g.zdbjq.cn/Article/details/gyvzqtkeh.sHtML

[Q65] 回滚事务
来源：http://3g.fehbvm.com/Article/details/gvunijphv.sHtML

ROLLBACK;
来源：http://m.share.fehbvm.com/Article/details/gtvecckgp.sHtML

[Q66] 行锁查询
来源：http://www.blog.hesvh.cn/Article/details/geicpfdfd.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.share.fehbvm.com/Article/details/glrtdqhot.sHtML

[Q67] 设置隔离级别
来源：http://wap.fehbvm.com/Article/details/grrrbkpwh.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://m.share.zdbjq.cn/Article/details/gbimwvfcw.sHtML

[Q68] 保存点
来源：http://www.m.share.hesvh.cn/Article/details/gkijbraed.sHtML

SAVEPOINT sp1;
来源：http://blog.hesvh.cn/Article/details/gyzryotuf.sHtML

ROLLBACK TO sp1;
来源：http://mobile.hesvh.cn/Article/details/gibfmkmkh.sHtML

[Q69] 查看执行计划
来源：http://www.blog.hesvh.cn/Article/details/gxnkuzjas.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://m.share.zdbjq.cn/Article/details/gyqptszbp.sHtML

[Q70] 更新统计信息
来源：http://read.share.fehbvm.com/Article/details/gokibsgre.sHtML

ANALYZE TABLE users;
来源：http://wap.hesvh.cn/Article/details/gyattfilh.sHtML

[Q71] 查看建表语句
来源：http://www.share.hesvh.cn/Article/details/gdwccjkpe.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://baike.hesvh.cn/Article/details/getlsgfoy.sHtML

[Q72] 查看索引
来源：http://www.share.hesvh.cn/Article/details/gnqyzafir.sHtML

SHOW INDEX FROM users;
来源：http://www.blog.hesvh.cn/Article/details/giqnudovp.sHtML

[Q73] 查看表状态
来源：http://wap.fehbvm.com/Article/details/gdpzwthrr.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://mobile.fehbvm.com/Article/details/gaubyhafr.sHtML

[Q74] 强制使用索引
来源：http://m.share.zdbjq.cn/Article/details/gxxiveboa.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://blog.hesvh.cn/Article/details/grszquyyh.sHtML

[Q75] 日期格式化
来源：http://m.share.fehbvm.com/Article/details/gymvxzliq.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://wap.fehbvm.com/Article/details/goxipwiyf.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://baike.hesvh.cn/Article/details/gpchsprri.sHtML

[Q76] 按天统计
来源：http://baike.fehbvm.com/Article/details/gpnjzxlrp.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://m.share.zdbjq.cn/Article/details/gsxgxwqnf.sHtML

[Q77] 时间加减
来源：http://www.m.share.hesvh.cn/Article/details/govfmglmy.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.m.share.hesvh.cn/Article/details/gdsdcnwcn.sHtML

[Q78] 当前时间
来源：http://baike.fehbvm.com/Article/details/gzgtsynvg.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.blog.fehbvm.com/Article/details/gragmwvhx.sHtML

[Q79] 字符串拼接
来源：http://mobile.zdbjq.cn/Article/details/giiymsjsk.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://blog.hesvh.cn/Article/details/gdtwktkzs.sHtML

[Q80] 字符串截取
来源：http://www.share.fehbvm.com/Article/details/gefsyxcbt.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://mobile.fehbvm.com/Article/details/ggzpuqjzb.sHtML

[Q81] 字符串替换
来源：http://www.blog.hesvh.cn/Article/details/gfavszqew.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gcnebyxjb.sHtML

[Q82] 字符长度与字节长度
来源：http://baike.fehbvm.com/Article/details/gxlgykqga.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://wap.fehbvm.com/Article/details/gagpulapl.sHtML

[Q83] 大小写转换
来源：http://www.m.share.fehbvm.com/Article/details/gmchrmcjc.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://baike.zdbjq.cn/Article/details/geovxumqh.sHtML

[Q84] 去除首尾空格
来源：http://www.m.share.hesvh.cn/Article/details/ggyzwnbwp.sHtML

SELECT TRIM(name) FROM users;
来源：http://baike.zdbjq.cn/Article/details/gnsacqcyh.sHtML

[Q85] 数值取整
来源：http://www.m.share.zdbjq.cn/Article/details/ghhtdxlxa.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://m.share.fehbvm.com/Article/details/guvbzzish.sHtML

[Q86] 读取 JSON 字段
来源：http://m.share.hesvh.cn/Article/details/gvuekauht.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://mobile.hesvh.cn/Article/details/grooxcztm.sHtML

[Q87] JSON 字段做条件
来源：http://www.m.share.fehbvm.com/Article/details/gjapwdbrn.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://blog.fehbvm.com/Article/details/gfvxefmaf.sHtML

[Q88] 行转列（条件聚合）
来源：http://wap.zdbjq.cn/Article/details/gtyjkblms.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://blog.hesvh.cn/Article/details/gpfxlklqs.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://3g.zdbjq.cn/Article/details/gymbmeojd.sHtML

[Q89] 判断表是否存在
来源：http://baike.fehbvm.com/Article/details/guzswshpd.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.blog.fehbvm.com/Article/details/gsoszzqgm.sHtML

[Q90] 生成序号列
来源：http://read.share.fehbvm.com/Article/details/gmpuelqxz.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.m.share.hesvh.cn/Article/details/gmzcohmsp.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gfbioppbh.sHtML

R. Bash 专题
来源：http://www.m.share.zdbjq.cn/Article/details/gobdnqgsf.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gwgkcsoow.sHtML

[R01] shebang 与严格模式
来源：http://3g.zdbjq.cn/Article/details/gwjentrym.sHtML

#!/usr/bin/env bash
来源：http://mobile.hesvh.cn/Article/details/ghasefkxz.sHtML

set -euo pipefail
来源：http://wap.fehbvm.com/Article/details/gtpxhxvej.sHtML

[R02] 变量赋值与使用
来源：http://baike.fehbvm.com/Article/details/gxhtfuwvi.sHtML

name="Tom"; echo "$name"
来源：http://baike.fehbvm.com/Article/details/gcnywrdfp.sHtML

[R03] 只读变量
来源：http://wap.fehbvm.com/Article/details/gyxfkedqf.sHtML

readonly PI=3.14
来源：http://blog.zdbjq.cn/Article/details/gocnbnkbn.sHtML

[R04] 位置参数
来源：http://www.blog.hesvh.cn/Article/details/gbukizgid.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.share.hesvh.cn/Article/details/ghaoggeco.sHtML

[R05] 参数默认值
来源：http://read.share.zdbjq.cn/Article/details/gkfxkojhe.sHtML

name="${1:-default}"
来源：http://wap.zdbjq.cn/Article/details/ghnarromf.sHtML

[R06] 判断命令是否存在
来源：http://www.blog.hesvh.cn/Article/details/gfhgvgkjo.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://wap.fehbvm.com/Article/details/gxmhaflof.sHtML

[R07] if 判断文件
来源：http://www.m.share.fehbvm.com/Article/details/gmiqxgdxo.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://read.share.zdbjq.cn/Article/details/gkjrxyfvt.sHtML

[R08] 数值比较
来源：http://www.blog.fehbvm.com/Article/details/gtvsuwvjm.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.blog.fehbvm.com/Article/details/gjvjuopju.sHtML

[R09] 字符串比较
来源：http://www.share.fehbvm.com/Article/details/girdaxvmw.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://mobile.zdbjq.cn/Article/details/gjwbsgegl.sHtML

[R10] 正则匹配
来源：http://3g.fehbvm.com/Article/details/gkjtibrqw.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://mobile.fehbvm.com/Article/details/genisfdjk.sHtML

[R11] case 多分支
来源：http://m.share.zdbjq.cn/Article/details/gdbwdxyjs.sHtML

case "$1" in
来源：http://www.share.zdbjq.cn/Article/details/gbftqdkxo.sHtML

start) echo "启动" ;;
来源：http://blog.hesvh.cn/Article/details/gzxejkygt.sHtML

stop)  echo "停止" ;;
来源：http://mobile.fehbvm.com/Article/details/gcxukcivp.sHtML

*)     echo "未知命令" ;;
来源：http://blog.hesvh.cn/Article/details/gggauucri.sHtML

esac
来源：http://wap.hesvh.cn/Article/details/gddplzoqr.sHtML

[R12] for 遍历文件
来源：http://www.m.share.zdbjq.cn/Article/details/ggltodblu.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.m.share.hesvh.cn/Article/details/grnezreoo.sHtML

[R13] for 计数循环
来源：http://3g.hesvh.cn/Article/details/gzhztgxwb.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://mobile.zdbjq.cn/Article/details/gjeineaqu.sHtML

[R14] C 风格 for
来源：http://wap.hesvh.cn/Article/details/gupodycvl.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.share.hesvh.cn/Article/details/gcrtvtlqq.sHtML

[R15] while 逐行读文件
来源：http://m.share.zdbjq.cn/Article/details/gdoxkufpv.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.share.fehbvm.com/Article/details/gchvzsilh.sHtML

[R16] until 等待条件
来源：http://www.share.hesvh.cn/Article/details/gnexbpofq.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.m.share.hesvh.cn/Article/details/gvitwsenl.sHtML

[R17] 数组定义与取值
来源：http://www.m.share.zdbjq.cn/Article/details/gtvvmgfpt.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://3g.hesvh.cn/Article/details/gdligrpjz.sHtML

[R18] 遍历数组
来源：http://www.blog.hesvh.cn/Article/details/gxstqolel.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://wap.zdbjq.cn/Article/details/gzvjwbvfc.sHtML

[R19] 数组长度
来源：http://read.share.zdbjq.cn/Article/details/gsbaqpxao.sHtML

echo "${#arr[@]}"
来源：http://baike.zdbjq.cn/Article/details/gcrluamao.sHtML

[R20] 关联数组（字典）
来源：http://www.blog.hesvh.cn/Article/details/gvjuctmlx.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.share.hesvh.cn/Article/details/gjvwnzupr.sHtML

[R21] 字符串长度
来源：http://read.share.zdbjq.cn/Article/details/gvazvdpls.sHtML

echo "${#s}"
来源：http://m.share.hesvh.cn/Article/details/gxkksqquq.sHtML

[R22] 截取子串
来源：http://www.share.zdbjq.cn/Article/details/gguujelel.sHtML

echo "${s:0:5}"
来源：http://wap.zdbjq.cn/Article/details/gbafgxysa.sHtML

[R23] 字符串替换
来源：http://m.share.zdbjq.cn/Article/details/gljemnekk.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://m.share.fehbvm.com/Article/details/glnyuetnt.sHtML

[R24] 大小写转换
来源：http://baike.hesvh.cn/Article/details/gjxtzvyet.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://3g.hesvh.cn/Article/details/gpfanhajd.sHtML

[R25] 去后缀 / 去前缀
来源：http://m.share.zdbjq.cn/Article/details/guvfrrcyj.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://blog.zdbjq.cn/Article/details/grnzqgteh.sHtML

[R26] 命令替换
来源：http://mobile.hesvh.cn/Article/details/gfhszuoqh.sHtML

now=$(date +%F); echo "$now"
来源：http://www.m.share.fehbvm.com/Article/details/gjxgzshtu.sHtML

[R27] 算术展开
来源：http://mobile.zdbjq.cn/Article/details/gwuhwafaf.sHtML

echo $((1 + 2 * 3))
来源：http://www.m.share.hesvh.cn/Article/details/gsrnyjcyf.sHtML

[R28] 浮点运算
来源：http://baike.fehbvm.com/Article/details/gxjkdjjfb.sHtML

echo "scale=2; 10/3" | bc
来源：http://m.share.hesvh.cn/Article/details/gbghvbehx.sHtML

[R29] 定义函数
来源：http://www.share.hesvh.cn/Article/details/gtdrhtfoi.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.m.share.fehbvm.com/Article/details/gxdscuhhc.sHtML

[R30] 函数返回状态码
来源：http://3g.hesvh.cn/Article/details/gdmapmusq.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://3g.zdbjq.cn/Article/details/gohxywznd.sHtML

[R31] 局部变量
来源：http://3g.fehbvm.com/Article/details/gxmrearyr.sHtML

f() { local x=1; echo "$x"; }
来源：http://baike.hesvh.cn/Article/details/geoeuwtad.sHtML

[R32] 参数个数校验
来源：http://www.m.share.fehbvm.com/Article/details/gmmdxywzz.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://wap.hesvh.cn/Article/details/gbrjzvaki.sHtML

[R33] 捕获错误并提示行号
来源：http://3g.zdbjq.cn/Article/details/gnpyqsqvh.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://3g.hesvh.cn/Article/details/ghddceycl.sHtML

[R34] 退出时清理
来源：http://www.m.share.fehbvm.com/Article/details/gueyzoxvl.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.fehbvm.com/Article/details/gcwrvevlz.sHtML

[R35] 后台执行并等待
来源：http://baike.fehbvm.com/Article/details/goiihtldu.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://m.share.fehbvm.com/Article/details/ghknhtpah.sHtML

[R36] 并发执行多个任务
来源：http://wap.zdbjq.cn/Article/details/gtoafmudv.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.m.share.fehbvm.com/Article/details/gxmvnhpsy.sHtML

[R37] 把输出赋给变量
来源：http://www.blog.fehbvm.com/Article/details/gfzrcqhsb.sHtML

files=$(ls -1)
来源：http://www.blog.hesvh.cn/Article/details/ghkjfihfu.sHtML

[R38] 管道串联
来源：http://baike.fehbvm.com/Article/details/gifssvsni.sHtML

cat a.txt | grep -i error | wc -l
来源：http://3g.hesvh.cn/Article/details/gcomrymrc.sHtML

[R39] 重定向标准输出与错误
来源：http://wap.fehbvm.com/Article/details/gpcwnjzuf.sHtML

cmd > out.log 2>&1
来源：http://www.blog.hesvh.cn/Article/details/gjjcjkzmm.sHtML

[R40] 追加写日志
来源：http://www.share.hesvh.cn/Article/details/gmgkqpfnf.sHtML

echo "log" >> out.log
来源：http://read.share.fehbvm.com/Article/details/grmqwwrbo.sHtML

[R41] 丢弃输出
来源：http://3g.fehbvm.com/Article/details/gplwrmrjh.sHtML

cmd >/dev/null 2>&1
来源：http://www.share.fehbvm.com/Article/details/gdgpfodyr.sHtML

[R42] 输入重定向
来源：http://blog.zdbjq.cn/Article/details/ghkkmufiq.sHtML

wc -l < a.txt
来源：http://m.share.fehbvm.com/Article/details/gdfxqawqh.sHtML

[R43] 按名字查找文件
来源：http://www.blog.hesvh.cn/Article/details/gqkdiadjd.sHtML

find . -name "*.log" -type f
来源：http://read.share.hesvh.cn/Article/details/grysmeaku.sHtML

[R44] 按修改时间查找
来源：http://3g.fehbvm.com/Article/details/gbkdckppe.sHtML

find . -mtime -7 -type f
来源：http://mobile.fehbvm.com/Article/details/gymjagezi.sHtML

[R45] 批量删除
来源：http://mobile.zdbjq.cn/Article/details/grytoyeui.sHtML


<!-- 参考信息 -->