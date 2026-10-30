代发 wailian999

CREATE TABLE users (
来源：http://www.blog.fehbvm.com/Article/details/ggpafotui.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.hesvh.cn/Article/details/gouvbalby.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.m.share.hesvh.cn/Article/details/gwblioiye.sHtML

email VARCHAR(100) UNIQUE,
来源：http://m.share.fehbvm.com/Article/details/gzgfecuhb.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://m.share.fehbvm.com/Article/details/gfpspucdi.sHtML

);
来源：http://baike.zdbjq.cn/Article/details/gzrbafmbs.sHtML

[Q02] 创建带外键的表
来源：http://3g.fehbvm.com/Article/details/gntcgfzhm.sHtML

CREATE TABLE orders (
来源：http://m.share.hesvh.cn/Article/details/gwwslohnw.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.zdbjq.cn/Article/details/gcacypsjv.sHtML

user_id INT NOT NULL,
来源：http://read.share.hesvh.cn/Article/details/gaqnfjvwz.sHtML

amount DECIMAL(10, 2),
来源：http://blog.zdbjq.cn/Article/details/gqlzbwrak.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://wap.fehbvm.com/Article/details/glcgsctbs.sHtML

);
来源：http://www.m.share.zdbjq.cn/Article/details/gtoydpwul.sHtML

[Q03] 增加列
来源：http://wap.hesvh.cn/Article/details/ggigknnro.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.blog.zdbjq.cn/Article/details/ghjuooeba.sHtML

[Q04] 修改列类型
来源：http://www.share.zdbjq.cn/Article/details/gtwjsoeyy.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://wap.hesvh.cn/Article/details/gtgukglat.sHtML

[Q05] 重命名列
来源：http://blog.hesvh.cn/Article/details/gknurnzlu.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://m.share.fehbvm.com/Article/details/gfmstbgiq.sHtML

[Q06] 删除列
来源：http://www.blog.hesvh.cn/Article/details/gvnagomxu.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://read.share.fehbvm.com/Article/details/gtjxpgdeo.sHtML

[Q07] 删除表
来源：http://baike.hesvh.cn/Article/details/gdtbbkopp.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.m.share.zdbjq.cn/Article/details/gyhpozrph.sHtML

[Q08] 创建普通索引
来源：http://blog.fehbvm.com/Article/details/genlvsjsu.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://blog.hesvh.cn/Article/details/guktxcgnm.sHtML

[Q09] 创建唯一索引
来源：http://www.m.share.hesvh.cn/Article/details/gitbcdpqh.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://3g.hesvh.cn/Article/details/gykbjesvj.sHtML

[Q10] 插入单行
来源：http://m.share.fehbvm.com/Article/details/gqtfivlyd.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.m.share.zdbjq.cn/Article/details/gweynuxri.sHtML

[Q11] 一次插入多行
来源：http://www.blog.hesvh.cn/Article/details/gwmfmgmvc.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.m.share.fehbvm.com/Article/details/gcjmpfotk.sHtML

[Q12] 插入后取自增 ID
来源：http://blog.zdbjq.cn/Article/details/gldlzcwxc.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://read.share.hesvh.cn/Article/details/getxuamcn.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.share.fehbvm.com/Article/details/gdgtejjdj.sHtML

[Q13] 忽略重复插入
来源：http://mobile.hesvh.cn/Article/details/gpqhlejhy.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://blog.hesvh.cn/Article/details/gupmatevs.sHtML

[Q14] 存在则更新（upsert）
来源：http://3g.hesvh.cn/Article/details/ghtkuljzp.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://baike.hesvh.cn/Article/details/gnbyhagnn.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://read.share.fehbvm.com/Article/details/glxffdozl.sHtML

[Q15] 查询全部
来源：http://www.share.fehbvm.com/Article/details/gtoamnuwh.sHtML

SELECT * FROM users;
来源：http://blog.fehbvm.com/Article/details/gspoyobtq.sHtML

[Q16] 查询指定列
来源：http://m.share.zdbjq.cn/Article/details/glpdiftas.sHtML

SELECT id, name FROM users;
来源：http://mobile.hesvh.cn/Article/details/gxjjlvfyb.sHtML

[Q17] 条件查询
来源：http://baike.hesvh.cn/Article/details/gorzkjmyr.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://3g.zdbjq.cn/Article/details/gziuxjvdy.sHtML

[Q18] 模糊匹配
来源：http://mobile.fehbvm.com/Article/details/gegopnzxn.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.share.hesvh.cn/Article/details/gdsclpqaq.sHtML

[Q19] 范围查询
来源：http://www.m.share.hesvh.cn/Article/details/grdizckze.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://3g.hesvh.cn/Article/details/gfklkzhli.sHtML

[Q20] IN 列表
来源：http://blog.hesvh.cn/Article/details/gexbomkfp.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.share.fehbvm.com/Article/details/gglzaxoyh.sHtML

[Q21] 空值判断
来源：http://www.share.zdbjq.cn/Article/details/gobfovxhd.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://baike.fehbvm.com/Article/details/gehhxwhbl.sHtML

[Q22] 排序
来源：http://baike.fehbvm.com/Article/details/gekhqczcs.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.m.share.hesvh.cn/Article/details/guvavsmhq.sHtML

[Q23] 分页
来源：http://blog.zdbjq.cn/Article/details/gohoqwqpu.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://read.share.zdbjq.cn/Article/details/gchbmqcwj.sHtML

[Q24] 去重
来源：http://baike.hesvh.cn/Article/details/gcklmmfwj.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gqnzqeyuq.sHtML

[Q25] 只取前 N 条
来源：http://www.blog.hesvh.cn/Article/details/gzasccyov.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://3g.hesvh.cn/Article/details/gvxulfiwz.sHtML

[Q26] 计数
来源：http://www.m.share.fehbvm.com/Article/details/gyezjknae.sHtML

SELECT COUNT(*) FROM users;
来源：http://m.share.fehbvm.com/Article/details/gdzecihzw.sHtML

[Q27] 条件计数
来源：http://3g.zdbjq.cn/Article/details/gewwfyfrc.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/giasjcwex.sHtML

[Q28] 求和与平均
来源：http://wap.hesvh.cn/Article/details/gyvcnfkrm.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://blog.hesvh.cn/Article/details/grtfkvxte.sHtML

[Q29] 最大最小值
来源：http://m.share.hesvh.cn/Article/details/ghrpkvwhh.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gesvscdjz.sHtML

[Q30] 分组统计
来源：http://www.blog.zdbjq.cn/Article/details/gvfwdmoph.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://read.share.fehbvm.com/Article/details/gxlahktjv.sHtML

[Q31] 分组后过滤
来源：http://read.share.zdbjq.cn/Article/details/gpiupkncu.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://wap.hesvh.cn/Article/details/gsbrxjdfa.sHtML

[Q32] 分组拼接字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gcddutylm.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.share.hesvh.cn/Article/details/gtjhmzmlj.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://3g.fehbvm.com/Article/details/gpjozqlqj.sHtML

[Q33] 多列分组
来源：http://wap.fehbvm.com/Article/details/gkfowfofz.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://read.share.zdbjq.cn/Article/details/gidrxshgc.sHtML

[Q34] 每组取第一条
来源：http://read.share.hesvh.cn/Article/details/geikpebka.sHtML

SELECT * FROM (
来源：http://www.m.share.fehbvm.com/Article/details/gooattjou.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://m.share.hesvh.cn/Article/details/giqsdpmrj.sHtML

) t WHERE rn = 1;
来源：http://wap.hesvh.cn/Article/details/gmwylyhmw.sHtML

[Q35] 内连接
来源：http://www.m.share.hesvh.cn/Article/details/gvfuqduhu.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://m.share.fehbvm.com/Article/details/gobwvlooa.sHtML

[Q36] 左连接
来源：http://www.share.zdbjq.cn/Article/details/gchdubjuh.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://mobile.fehbvm.com/Article/details/gffkpnbku.sHtML

[Q37] 右连接
来源：http://blog.fehbvm.com/Article/details/gfpqioamz.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.m.share.fehbvm.com/Article/details/gvqcaokra.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://baike.zdbjq.cn/Article/details/gwrzftark.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://blog.fehbvm.com/Article/details/ghepbspqm.sHtML

[Q39] 自连接（查上下级）
来源：http://m.share.hesvh.cn/Article/details/goottfnie.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://baike.zdbjq.cn/Article/details/gbogavioa.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://read.share.hesvh.cn/Article/details/gaulsqrlq.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://read.share.fehbvm.com/Article/details/gvagjinjz.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://m.share.hesvh.cn/Article/details/giilftxfw.sHtML

[Q41] 多表连接
来源：http://read.share.fehbvm.com/Article/details/gktwdidin.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://mobile.zdbjq.cn/Article/details/gimpoiukd.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.m.share.zdbjq.cn/Article/details/ggkrvgrlb.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://3g.hesvh.cn/Article/details/gxiglqpdr.sHtML

[Q42] 连接条件附加过滤
来源：http://mobile.hesvh.cn/Article/details/gwcraxjwo.sHtML

SELECT u.name, o.amount FROM users u
来源：http://baike.hesvh.cn/Article/details/gcabodmxm.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.blog.fehbvm.com/Article/details/ggqqiegnl.sHtML

[Q43] 标量子查询
来源：http://blog.hesvh.cn/Article/details/gomqoquis.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://baike.zdbjq.cn/Article/details/gmkmynued.sHtML

[Q44] IN 子查询
来源：http://wap.hesvh.cn/Article/details/grtdfztvo.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://wap.fehbvm.com/Article/details/grcypzmxz.sHtML

[Q45] EXISTS 判断存在
来源：http://www.m.share.fehbvm.com/Article/details/gsyueadyo.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.hesvh.cn/Article/details/gdckwbsqj.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://mobile.fehbvm.com/Article/details/gmmwlfxin.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.zdbjq.cn/Article/details/gppalsjis.sHtML

[Q47] 与平均值比较
来源：http://www.share.hesvh.cn/Article/details/gbhpxwcun.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://mobile.fehbvm.com/Article/details/gzwsmosvf.sHtML

[Q48] CTE 公用表表达式
来源：http://blog.zdbjq.cn/Article/details/gbajvrtap.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://mobile.fehbvm.com/Article/details/glcwsmudr.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://3g.zdbjq.cn/Article/details/gmkgegffr.sHtML

[Q49] 更新单行
来源：http://www.share.hesvh.cn/Article/details/gizumxmwj.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://read.share.fehbvm.com/Article/details/ggbzthwwq.sHtML

[Q50] 批量更新
来源：http://www.share.fehbvm.com/Article/details/gxotmydnx.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://read.share.fehbvm.com/Article/details/gtxlyfqng.sHtML

[Q51] 用子查询更新
来源：http://blog.hesvh.cn/Article/details/gmypdtrsx.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.share.zdbjq.cn/Article/details/gqazdxamo.sHtML

[Q52] 删除指定行
来源：http://www.share.fehbvm.com/Article/details/gplburimm.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.share.zdbjq.cn/Article/details/ghkhiqeeh.sHtML

[Q53] 按条件删除
来源：http://mobile.zdbjq.cn/Article/details/gfkoxzahl.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.m.share.hesvh.cn/Article/details/gzzhzydxc.sHtML

[Q54] 清空表
来源：http://wap.hesvh.cn/Article/details/gtqlhlwzl.sHtML

TRUNCATE TABLE logs;
来源：http://baike.hesvh.cn/Article/details/gsygbsrdt.sHtML

[Q55] 排名（并列占位）
来源：http://wap.zdbjq.cn/Article/details/ganxaapxr.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://wap.fehbvm.com/Article/details/gosinafvu.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.share.hesvh.cn/Article/details/gnbxnrfcx.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://3g.hesvh.cn/Article/details/gymnyhosm.sHtML

[Q57] 行号
来源：http://3g.hesvh.cn/Article/details/gkhxhlayo.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gtkexrpcs.sHtML

[Q58] 累计求和
来源：http://blog.zdbjq.cn/Article/details/gmfixbbko.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://m.share.hesvh.cn/Article/details/grvzesgnu.sHtML

[Q59] 分组内累计
来源：http://www.blog.hesvh.cn/Article/details/gcuisktfm.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.m.share.hesvh.cn/Article/details/gltqdiwbz.sHtML

[Q60] 取上一行 / 下一行
来源：http://read.share.hesvh.cn/Article/details/gpokipvsv.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.share.fehbvm.com/Article/details/gkmpnekwc.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://mobile.fehbvm.com/Article/details/gkpetmloa.sHtML

[Q61] 移动平均
来源：http://read.share.hesvh.cn/Article/details/gpwfjtyvc.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.share.fehbvm.com/Article/details/gtafrrlqr.sHtML

[Q62] 分组占比
来源：http://3g.hesvh.cn/Article/details/gwhwhejak.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.share.zdbjq.cn/Article/details/gafniihkx.sHtML

[Q63] 开启事务
来源：http://mobile.hesvh.cn/Article/details/gyxyrhyuv.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://baike.zdbjq.cn/Article/details/gvqsvgkqo.sHtML

[Q64] 提交事务
来源：http://wap.fehbvm.com/Article/details/gjgnipoyl.sHtML

COMMIT;
来源：http://blog.fehbvm.com/Article/details/gijynllag.sHtML

[Q65] 回滚事务
来源：http://m.share.fehbvm.com/Article/details/gchrancta.sHtML

ROLLBACK;
来源：http://blog.zdbjq.cn/Article/details/gcophbrdx.sHtML

[Q66] 行锁查询
来源：http://wap.zdbjq.cn/Article/details/grrepdqel.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://read.share.fehbvm.com/Article/details/gjcwsqsgq.sHtML

[Q67] 设置隔离级别
来源：http://3g.hesvh.cn/Article/details/gtodrinvp.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://m.share.zdbjq.cn/Article/details/gmgrtgywv.sHtML

[Q68] 保存点
来源：http://www.share.zdbjq.cn/Article/details/ghzxertnv.sHtML

SAVEPOINT sp1;
来源：http://www.blog.fehbvm.com/Article/details/gizcgbwuh.sHtML

ROLLBACK TO sp1;
来源：http://m.share.zdbjq.cn/Article/details/gilwfrjrc.sHtML

[Q69] 查看执行计划
来源：http://mobile.fehbvm.com/Article/details/gfekttzvf.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://wap.hesvh.cn/Article/details/gqbqfihdm.sHtML

[Q70] 更新统计信息
来源：http://read.share.hesvh.cn/Article/details/gjyjswcwg.sHtML

ANALYZE TABLE users;
来源：http://www.share.hesvh.cn/Article/details/ggivggmce.sHtML

[Q71] 查看建表语句
来源：http://www.blog.fehbvm.com/Article/details/gshkeiwgy.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.m.share.fehbvm.com/Article/details/gsqmokfuk.sHtML

[Q72] 查看索引
来源：http://mobile.fehbvm.com/Article/details/gmdawcszk.sHtML

SHOW INDEX FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gvsxvqxom.sHtML

[Q73] 查看表状态
来源：http://www.share.fehbvm.com/Article/details/gfdaumtga.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.m.share.hesvh.cn/Article/details/gxmqidevu.sHtML

[Q74] 强制使用索引
来源：http://m.share.fehbvm.com/Article/details/guhvakpje.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.m.share.fehbvm.com/Article/details/gyljilidb.sHtML

[Q75] 日期格式化
来源：http://wap.zdbjq.cn/Article/details/gdzjnhxxi.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://baike.fehbvm.com/Article/details/gfbvbfqze.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://wap.zdbjq.cn/Article/details/giyqlsrmp.sHtML

[Q76] 按天统计
来源：http://www.blog.fehbvm.com/Article/details/gwhrffioh.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://blog.hesvh.cn/Article/details/gexsxslhh.sHtML

[Q77] 时间加减
来源：http://www.share.zdbjq.cn/Article/details/gervcctlj.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://3g.hesvh.cn/Article/details/gdgbfcdlc.sHtML

[Q78] 当前时间
来源：http://www.m.share.hesvh.cn/Article/details/gktmqllag.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://baike.fehbvm.com/Article/details/gzjacsldm.sHtML

[Q79] 字符串拼接
来源：http://m.share.zdbjq.cn/Article/details/gvkcflean.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.share.hesvh.cn/Article/details/gvdlqtwdk.sHtML

[Q80] 字符串截取
来源：http://baike.hesvh.cn/Article/details/gppmqojde.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gpjsbtoaf.sHtML

[Q81] 字符串替换
来源：http://www.blog.hesvh.cn/Article/details/gqndfrabd.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gsxmesrwt.sHtML

[Q82] 字符长度与字节长度
来源：http://mobile.hesvh.cn/Article/details/gwweevxvb.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://wap.fehbvm.com/Article/details/gnflmfcin.sHtML

[Q83] 大小写转换
来源：http://read.share.fehbvm.com/Article/details/gwzdlwjlt.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://baike.fehbvm.com/Article/details/gbmxcwgai.sHtML

[Q84] 去除首尾空格
来源：http://m.share.fehbvm.com/Article/details/gsdetslvu.sHtML

SELECT TRIM(name) FROM users;
来源：http://m.share.hesvh.cn/Article/details/geirmgice.sHtML

[Q85] 数值取整
来源：http://wap.fehbvm.com/Article/details/guyebiajb.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://read.share.hesvh.cn/Article/details/gxzfnrvaz.sHtML

[Q86] 读取 JSON 字段
来源：http://blog.zdbjq.cn/Article/details/gfdvpwnme.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://blog.hesvh.cn/Article/details/gkzaqlqgg.sHtML

[Q87] JSON 字段做条件
来源：http://mobile.hesvh.cn/Article/details/gujpmjotn.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.m.share.zdbjq.cn/Article/details/gjyxwsjzl.sHtML

[Q88] 行转列（条件聚合）
来源：http://mobile.fehbvm.com/Article/details/gpfisergj.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://mobile.hesvh.cn/Article/details/gxgcawkju.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.share.hesvh.cn/Article/details/gknzebawo.sHtML

[Q89] 判断表是否存在
来源：http://www.blog.hesvh.cn/Article/details/giwzkraqi.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://3g.hesvh.cn/Article/details/gvaarahkv.sHtML

[Q90] 生成序号列
来源：http://www.blog.fehbvm.com/Article/details/gidfofemz.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://m.share.fehbvm.com/Article/details/gyyhetnkp.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gxzdohlrf.sHtML

R. Bash 专题
来源：http://read.share.fehbvm.com/Article/details/gcgiwlfoi.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/grgueungj.sHtML

[R01] shebang 与严格模式
来源：http://www.share.zdbjq.cn/Article/details/gjfjybzca.sHtML

#!/usr/bin/env bash
来源：http://3g.hesvh.cn/Article/details/gouwfrrsy.sHtML

set -euo pipefail
来源：http://wap.zdbjq.cn/Article/details/gzuwolldh.sHtML

[R02] 变量赋值与使用
来源：http://baike.hesvh.cn/Article/details/gjsqikygf.sHtML

name="Tom"; echo "$name"
来源：http://www.m.share.fehbvm.com/Article/details/geoolwbtr.sHtML

[R03] 只读变量
来源：http://blog.zdbjq.cn/Article/details/gqyybwcjo.sHtML

readonly PI=3.14
来源：http://m.share.fehbvm.com/Article/details/gihnymonp.sHtML

[R04] 位置参数
来源：http://m.share.zdbjq.cn/Article/details/gkatcngcm.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://read.share.fehbvm.com/Article/details/gnckemglz.sHtML

[R05] 参数默认值
来源：http://blog.zdbjq.cn/Article/details/ghgtzlvgd.sHtML

name="${1:-default}"
来源：http://3g.hesvh.cn/Article/details/ggudhwcgs.sHtML

[R06] 判断命令是否存在
来源：http://baike.zdbjq.cn/Article/details/gcffeepnm.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.share.fehbvm.com/Article/details/gmkgkrlkv.sHtML

[R07] if 判断文件
来源：http://blog.hesvh.cn/Article/details/glyofckyk.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://read.share.fehbvm.com/Article/details/gdvihlkwu.sHtML

[R08] 数值比较
来源：http://read.share.zdbjq.cn/Article/details/giuxnghyk.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://3g.hesvh.cn/Article/details/gilfuffgs.sHtML

[R09] 字符串比较
来源：http://wap.fehbvm.com/Article/details/gftdlqnhw.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://read.share.fehbvm.com/Article/details/gicegmrpt.sHtML

[R10] 正则匹配
来源：http://www.m.share.zdbjq.cn/Article/details/ghcjdtiem.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://baike.zdbjq.cn/Article/details/gkvmcggwi.sHtML

[R11] case 多分支
来源：http://www.m.share.zdbjq.cn/Article/details/gichgkwwz.sHtML

case "$1" in
来源：http://www.m.share.zdbjq.cn/Article/details/gefdpkebz.sHtML

start) echo "启动" ;;
来源：http://blog.hesvh.cn/Article/details/gnhssqtng.sHtML

stop)  echo "停止" ;;
来源：http://www.m.share.zdbjq.cn/Article/details/gmenyeqnd.sHtML

*)     echo "未知命令" ;;
来源：http://www.blog.zdbjq.cn/Article/details/gzhgjecyh.sHtML

esac
来源：http://www.share.fehbvm.com/Article/details/gvqbwkndf.sHtML

[R12] for 遍历文件
来源：http://m.share.zdbjq.cn/Article/details/gqdtbdfzf.sHtML

for f in *.txt; do echo "$f"; done
来源：http://3g.hesvh.cn/Article/details/gqzjansvt.sHtML

[R13] for 计数循环
来源：http://baike.zdbjq.cn/Article/details/gxffajlkq.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.share.zdbjq.cn/Article/details/gstsagcfu.sHtML

[R14] C 风格 for
来源：http://www.share.zdbjq.cn/Article/details/gituuhtkx.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://mobile.hesvh.cn/Article/details/gwaebpkjq.sHtML

[R15] while 逐行读文件
来源：http://www.m.share.zdbjq.cn/Article/details/gcadiduup.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://m.share.hesvh.cn/Article/details/gsiwyfvmy.sHtML

[R16] until 等待条件
来源：http://www.blog.zdbjq.cn/Article/details/ggopwagrm.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.m.share.zdbjq.cn/Article/details/geqqkuyta.sHtML

[R17] 数组定义与取值
来源：http://www.share.zdbjq.cn/Article/details/gwtrkqvzj.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.blog.hesvh.cn/Article/details/gkpkajyrc.sHtML

[R18] 遍历数组
来源：http://read.share.zdbjq.cn/Article/details/gfukizrod.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.share.hesvh.cn/Article/details/gjogerswq.sHtML

[R19] 数组长度
来源：http://blog.fehbvm.com/Article/details/gweyiqswm.sHtML

echo "${#arr[@]}"
来源：http://read.share.fehbvm.com/Article/details/gylphmnma.sHtML

[R20] 关联数组（字典）
来源：http://baike.hesvh.cn/Article/details/gqwlwrzcp.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://read.share.hesvh.cn/Article/details/gvfcgybni.sHtML

[R21] 字符串长度
来源：http://mobile.zdbjq.cn/Article/details/gxprcewgm.sHtML

echo "${#s}"
来源：http://wap.hesvh.cn/Article/details/ggdgfjlvv.sHtML

[R22] 截取子串
来源：http://wap.zdbjq.cn/Article/details/guucevqik.sHtML

echo "${s:0:5}"
来源：http://www.blog.fehbvm.com/Article/details/gdhuoqclh.sHtML

[R23] 字符串替换
来源：http://www.blog.hesvh.cn/Article/details/gfeqwdrdc.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://3g.zdbjq.cn/Article/details/gfpiijnnj.sHtML

[R24] 大小写转换
来源：http://www.blog.fehbvm.com/Article/details/gdncytswc.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://read.share.zdbjq.cn/Article/details/gppdgtxmm.sHtML

[R25] 去后缀 / 去前缀
来源：http://mobile.fehbvm.com/Article/details/gakeaoloo.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://3g.zdbjq.cn/Article/details/gbpfuivoo.sHtML

[R26] 命令替换
来源：http://wap.zdbjq.cn/Article/details/gjkujqphz.sHtML

now=$(date +%F); echo "$now"
来源：http://mobile.zdbjq.cn/Article/details/gbkrpeaui.sHtML

[R27] 算术展开
来源：http://wap.hesvh.cn/Article/details/gsiphrnby.sHtML

echo $((1 + 2 * 3))
来源：http://blog.fehbvm.com/Article/details/gjidoloej.sHtML

[R28] 浮点运算
来源：http://www.share.hesvh.cn/Article/details/gdcbtnfvg.sHtML

echo "scale=2; 10/3" | bc
来源：http://wap.fehbvm.com/Article/details/gccaitaqu.sHtML

[R29] 定义函数
来源：http://blog.hesvh.cn/Article/details/gluomyexc.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://mobile.hesvh.cn/Article/details/gzcbevkzk.sHtML

[R30] 函数返回状态码
来源：http://www.share.fehbvm.com/Article/details/gkjpgmgka.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://baike.zdbjq.cn/Article/details/gzrjebqzb.sHtML

[R31] 局部变量
来源：http://baike.fehbvm.com/Article/details/gpeufyfuq.sHtML

f() { local x=1; echo "$x"; }
来源：http://baike.fehbvm.com/Article/details/gkzlpamgx.sHtML

[R32] 参数个数校验
来源：http://blog.fehbvm.com/Article/details/gemonvklh.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://3g.zdbjq.cn/Article/details/grgjmnzns.sHtML

[R33] 捕获错误并提示行号
来源：http://3g.zdbjq.cn/Article/details/grnnfwzgy.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://blog.zdbjq.cn/Article/details/gykxazqxp.sHtML

[R34] 退出时清理
来源：http://3g.fehbvm.com/Article/details/gvmuvqobp.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.zdbjq.cn/Article/details/gfonroqwn.sHtML

[R35] 后台执行并等待
来源：http://wap.fehbvm.com/Article/details/gkszaveuk.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://read.share.fehbvm.com/Article/details/gndmamlkj.sHtML

[R36] 并发执行多个任务
来源：http://blog.zdbjq.cn/Article/details/gfattypag.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.blog.zdbjq.cn/Article/details/gxtaquogl.sHtML

[R37] 把输出赋给变量
来源：http://baike.fehbvm.com/Article/details/gdahekddd.sHtML

files=$(ls -1)
来源：http://wap.hesvh.cn/Article/details/gxyxssqyx.sHtML

[R38] 管道串联
来源：http://mobile.hesvh.cn/Article/details/grmpoahtd.sHtML

cat a.txt | grep -i error | wc -l
来源：http://m.share.zdbjq.cn/Article/details/gcitrqkqm.sHtML

[R39] 重定向标准输出与错误
来源：http://www.blog.hesvh.cn/Article/details/gispnuwlc.sHtML

cmd > out.log 2>&1
来源：http://mobile.hesvh.cn/Article/details/gjweqazjf.sHtML

[R40] 追加写日志
来源：http://www.share.fehbvm.com/Article/details/gqbugheyz.sHtML

echo "log" >> out.log
来源：http://3g.fehbvm.com/Article/details/gcapsupcq.sHtML

[R41] 丢弃输出
来源：http://www.m.share.hesvh.cn/Article/details/gjasghyuv.sHtML

cmd >/dev/null 2>&1
来源：http://mobile.zdbjq.cn/Article/details/gcycwhdsk.sHtML

[R42] 输入重定向
来源：http://m.share.zdbjq.cn/Article/details/gjdqubxxj.sHtML

wc -l < a.txt
来源：http://3g.zdbjq.cn/Article/details/gjbuqwlmd.sHtML

[R43] 按名字查找文件
来源：http://www.share.hesvh.cn/Article/details/gkwuxvzxv.sHtML

find . -name "*.log" -type f
来源：http://wap.zdbjq.cn/Article/details/gifapqvyj.sHtML

[R44] 按修改时间查找
来源：http://blog.fehbvm.com/Article/details/ggjtfsjdn.sHtML

find . -mtime -7 -type f
来源：http://www.m.share.hesvh.cn/Article/details/gqrtgqcvs.sHtML

[R45] 批量删除
来源：http://3g.fehbvm.com/Article/details/ggqqluqkh.sHtML


<!-- 参考信息 -->