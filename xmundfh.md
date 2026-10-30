代发 wailian999

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://mobile.fehbvm.com/Article/details/gjngbryiu.sHtML

);
来源：http://read.share.zdbjq.cn/Article/details/gjnduzduh.sHtML

[Q02] 创建带外键的表
来源：http://www.blog.hesvh.cn/Article/details/gsvvactph.sHtML

CREATE TABLE orders (
来源：http://mobile.zdbjq.cn/Article/details/gosjietce.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.fehbvm.com/Article/details/gqlcibhvu.sHtML

user_id INT NOT NULL,
来源：http://mobile.zdbjq.cn/Article/details/gstyhxhms.sHtML

amount DECIMAL(10, 2),
来源：http://www.share.hesvh.cn/Article/details/gzwfwfsra.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://baike.fehbvm.com/Article/details/gvcgiszgq.sHtML

);
来源：http://baike.zdbjq.cn/Article/details/gvnaepxxo.sHtML

[Q03] 增加列
来源：http://www.blog.zdbjq.cn/Article/details/gqowhrxqv.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://read.share.zdbjq.cn/Article/details/gyflvawvg.sHtML

[Q04] 修改列类型
来源：http://www.share.zdbjq.cn/Article/details/gzetooxqq.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://wap.fehbvm.com/Article/details/glearmerl.sHtML

[Q05] 重命名列
来源：http://3g.zdbjq.cn/Article/details/guordqfsu.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://blog.zdbjq.cn/Article/details/gjweaewyd.sHtML

[Q06] 删除列
来源：http://wap.zdbjq.cn/Article/details/gjgbvoivm.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.blog.zdbjq.cn/Article/details/gjzqavoja.sHtML

[Q07] 删除表
来源：http://baike.fehbvm.com/Article/details/gmmklmwfq.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.blog.zdbjq.cn/Article/details/gkdxteusz.sHtML

[Q08] 创建普通索引
来源：http://www.blog.zdbjq.cn/Article/details/gtmvfutmn.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.blog.hesvh.cn/Article/details/gxghvobgn.sHtML

[Q09] 创建唯一索引
来源：http://3g.hesvh.cn/Article/details/gnhqxoaqn.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://baike.fehbvm.com/Article/details/gwinootac.sHtML

[Q10] 插入单行
来源：http://3g.fehbvm.com/Article/details/glbprazol.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://baike.hesvh.cn/Article/details/gocgycvor.sHtML

[Q11] 一次插入多行
来源：http://3g.zdbjq.cn/Article/details/gorrywavt.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://blog.zdbjq.cn/Article/details/gakunirbq.sHtML

[Q12] 插入后取自增 ID
来源：http://3g.zdbjq.cn/Article/details/gjxveerjm.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.share.zdbjq.cn/Article/details/gsceimilf.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://baike.fehbvm.com/Article/details/gpamhhtox.sHtML

[Q13] 忽略重复插入
来源：http://baike.fehbvm.com/Article/details/gocgmlsei.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.m.share.fehbvm.com/Article/details/gvtyihhgh.sHtML

[Q14] 存在则更新（upsert）
来源：http://3g.fehbvm.com/Article/details/gsbqaztne.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://baike.hesvh.cn/Article/details/gkiyswucr.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.blog.hesvh.cn/Article/details/gedaulpyc.sHtML

[Q15] 查询全部
来源：http://m.share.hesvh.cn/Article/details/gtzqsakik.sHtML

SELECT * FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/guwfvlltc.sHtML

[Q16] 查询指定列
来源：http://mobile.zdbjq.cn/Article/details/gqxtqmfoz.sHtML

SELECT id, name FROM users;
来源：http://wap.zdbjq.cn/Article/details/gmjgzlzdj.sHtML

[Q17] 条件查询
来源：http://m.share.zdbjq.cn/Article/details/glwxvapqb.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://wap.fehbvm.com/Article/details/gvivdbhaa.sHtML

[Q18] 模糊匹配
来源：http://mobile.hesvh.cn/Article/details/gbvovjfbr.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://mobile.fehbvm.com/Article/details/gxzoqkiok.sHtML

[Q19] 范围查询
来源：http://www.blog.zdbjq.cn/Article/details/grcvexyfj.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://baike.zdbjq.cn/Article/details/gwiuhzwlx.sHtML

[Q20] IN 列表
来源：http://m.share.zdbjq.cn/Article/details/gjypkrkwo.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://wap.fehbvm.com/Article/details/gamsqpnxp.sHtML

[Q21] 空值判断
来源：http://www.share.fehbvm.com/Article/details/glzuuzxno.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.blog.hesvh.cn/Article/details/gumejcoct.sHtML

[Q22] 排序
来源：http://baike.fehbvm.com/Article/details/gnhqzejzq.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.m.share.hesvh.cn/Article/details/gawkqrbik.sHtML

[Q23] 分页
来源：http://read.share.hesvh.cn/Article/details/guaitnytp.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://wap.fehbvm.com/Article/details/gzohezoiv.sHtML

[Q24] 去重
来源：http://3g.zdbjq.cn/Article/details/gsfwrtiwz.sHtML

SELECT DISTINCT city FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gfpdfucjc.sHtML

[Q25] 只取前 N 条
来源：http://mobile.fehbvm.com/Article/details/grjdbxopq.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://read.share.zdbjq.cn/Article/details/gocbgewhp.sHtML

[Q26] 计数
来源：http://www.m.share.fehbvm.com/Article/details/gvknuslfy.sHtML

SELECT COUNT(*) FROM users;
来源：http://blog.fehbvm.com/Article/details/gchdncazz.sHtML

[Q27] 条件计数
来源：http://www.m.share.fehbvm.com/Article/details/gwtigbxcl.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://mobile.fehbvm.com/Article/details/gfsbzrswk.sHtML

[Q28] 求和与平均
来源：http://www.m.share.hesvh.cn/Article/details/grzrgwqsn.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.blog.fehbvm.com/Article/details/gkuqoxyne.sHtML

[Q29] 最大最小值
来源：http://blog.hesvh.cn/Article/details/ghdlvbxdw.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.share.hesvh.cn/Article/details/gfzcfkqic.sHtML

[Q30] 分组统计
来源：http://www.share.hesvh.cn/Article/details/gkybyadmg.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://m.share.zdbjq.cn/Article/details/gvyzbrmdf.sHtML

[Q31] 分组后过滤
来源：http://wap.fehbvm.com/Article/details/gsvozhtko.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://mobile.hesvh.cn/Article/details/gfyqzlexv.sHtML

[Q32] 分组拼接字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gtupgbtcj.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://wap.hesvh.cn/Article/details/grofkdxix.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.blog.fehbvm.com/Article/details/gzfmnatch.sHtML

[Q33] 多列分组
来源：http://wap.hesvh.cn/Article/details/gzrhaylhk.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://blog.hesvh.cn/Article/details/gtkrwhosa.sHtML

[Q34] 每组取第一条
来源：http://wap.hesvh.cn/Article/details/gqwcbnbzr.sHtML

SELECT * FROM (
来源：http://3g.zdbjq.cn/Article/details/gkswharqn.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://mobile.fehbvm.com/Article/details/gjkxhifvy.sHtML

) t WHERE rn = 1;
来源：http://read.share.zdbjq.cn/Article/details/gxlulvkwn.sHtML

[Q35] 内连接
来源：http://read.share.fehbvm.com/Article/details/gosvwsqvm.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.hesvh.cn/Article/details/ghazumzdy.sHtML

[Q36] 左连接
来源：http://m.share.fehbvm.com/Article/details/gtfutxizt.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://wap.fehbvm.com/Article/details/gsbgrtwja.sHtML

[Q37] 右连接
来源：http://baike.hesvh.cn/Article/details/gtnduytxb.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://wap.hesvh.cn/Article/details/gfvpgjjve.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://mobile.zdbjq.cn/Article/details/geyribnzj.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://wap.hesvh.cn/Article/details/gzsicrkrr.sHtML

[Q39] 自连接（查上下级）
来源：http://3g.zdbjq.cn/Article/details/glrmctfas.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.m.share.fehbvm.com/Article/details/gljocxbrk.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://baike.hesvh.cn/Article/details/gwgdlsqwe.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://read.share.hesvh.cn/Article/details/gnmfafuzw.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://blog.fehbvm.com/Article/details/gwfafpqau.sHtML

[Q41] 多表连接
来源：http://www.share.zdbjq.cn/Article/details/gqrihkumd.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://mobile.hesvh.cn/Article/details/gcprtluef.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.blog.fehbvm.com/Article/details/gptltvtdq.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://baike.hesvh.cn/Article/details/gqgvpzutr.sHtML

[Q42] 连接条件附加过滤
来源：http://3g.hesvh.cn/Article/details/gnmnoeltd.sHtML

SELECT u.name, o.amount FROM users u
来源：http://read.share.hesvh.cn/Article/details/ggsgdfrcq.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://blog.fehbvm.com/Article/details/gmrhsvfid.sHtML

[Q43] 标量子查询
来源：http://baike.fehbvm.com/Article/details/gvjrlluip.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://3g.fehbvm.com/Article/details/ggmijngki.sHtML

[Q44] IN 子查询
来源：http://mobile.zdbjq.cn/Article/details/gkiuqwyey.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.blog.zdbjq.cn/Article/details/gmckldekk.sHtML

[Q45] EXISTS 判断存在
来源：http://wap.fehbvm.com/Article/details/glofemvpb.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.zdbjq.cn/Article/details/gchpfruon.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.share.zdbjq.cn/Article/details/gwoccbcad.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.fehbvm.com/Article/details/glyvafrzc.sHtML

[Q47] 与平均值比较
来源：http://www.share.fehbvm.com/Article/details/gejxjzudy.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.share.hesvh.cn/Article/details/geyakpxpq.sHtML

[Q48] CTE 公用表表达式
来源：http://3g.hesvh.cn/Article/details/gideppnll.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.blog.hesvh.cn/Article/details/gimmbhrpa.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://blog.hesvh.cn/Article/details/gwebeqcjv.sHtML

[Q49] 更新单行
来源：http://www.share.zdbjq.cn/Article/details/gfjzuhusr.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.share.zdbjq.cn/Article/details/gstdubrsn.sHtML

[Q50] 批量更新
来源：http://mobile.fehbvm.com/Article/details/gaojgsvfi.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://read.share.hesvh.cn/Article/details/gpyddwhzb.sHtML

[Q51] 用子查询更新
来源：http://read.share.fehbvm.com/Article/details/ggsfqcveg.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://m.share.zdbjq.cn/Article/details/ghngjksnn.sHtML

[Q52] 删除指定行
来源：http://www.share.hesvh.cn/Article/details/gkifikzml.sHtML

DELETE FROM users WHERE id = 10;
来源：http://wap.hesvh.cn/Article/details/gblokrpqw.sHtML

[Q53] 按条件删除
来源：http://m.share.fehbvm.com/Article/details/gdxvllwkp.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.share.fehbvm.com/Article/details/gvwfbtywe.sHtML

[Q54] 清空表
来源：http://blog.hesvh.cn/Article/details/gvdgpcnch.sHtML

TRUNCATE TABLE logs;
来源：http://mobile.hesvh.cn/Article/details/glsnlmnaq.sHtML

[Q55] 排名（并列占位）
来源：http://read.share.zdbjq.cn/Article/details/ghadoftwp.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.share.fehbvm.com/Article/details/ghyadsuxq.sHtML

[Q56] 密集排名（并列不占位）
来源：http://3g.fehbvm.com/Article/details/gwplotgtj.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.blog.hesvh.cn/Article/details/granckpar.sHtML

[Q57] 行号
来源：http://blog.fehbvm.com/Article/details/gxkouijjb.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gkkaxzoek.sHtML

[Q58] 累计求和
来源：http://blog.zdbjq.cn/Article/details/gemfkxefo.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://3g.zdbjq.cn/Article/details/grybfigmb.sHtML

[Q59] 分组内累计
来源：http://www.share.hesvh.cn/Article/details/gwnkvybjn.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.m.share.hesvh.cn/Article/details/gcqjzzrfa.sHtML

[Q60] 取上一行 / 下一行
来源：http://mobile.hesvh.cn/Article/details/gvegbfnau.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.share.fehbvm.com/Article/details/gkguwsghj.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.share.hesvh.cn/Article/details/gqlruhbwa.sHtML

[Q61] 移动平均
来源：http://www.share.zdbjq.cn/Article/details/gpjjjhidr.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://read.share.hesvh.cn/Article/details/gpktlrkvp.sHtML

[Q62] 分组占比
来源：http://www.m.share.zdbjq.cn/Article/details/gkquhwqoz.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.share.hesvh.cn/Article/details/gmmkeegpp.sHtML

[Q63] 开启事务
来源：http://m.share.zdbjq.cn/Article/details/grbyukcfd.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://read.share.fehbvm.com/Article/details/gnfnhkebz.sHtML

[Q64] 提交事务
来源：http://baike.zdbjq.cn/Article/details/gjkypjodv.sHtML

COMMIT;
来源：http://baike.zdbjq.cn/Article/details/gnnjxorkn.sHtML

[Q65] 回滚事务
来源：http://blog.zdbjq.cn/Article/details/gfvznmgwn.sHtML

ROLLBACK;
来源：http://mobile.zdbjq.cn/Article/details/grmjwioxl.sHtML

[Q66] 行锁查询
来源：http://blog.fehbvm.com/Article/details/grmvdwemz.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.blog.fehbvm.com/Article/details/ghrknetcj.sHtML

[Q67] 设置隔离级别
来源：http://mobile.fehbvm.com/Article/details/gwtspzgyx.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://wap.fehbvm.com/Article/details/gpzptlvdg.sHtML

[Q68] 保存点
来源：http://mobile.zdbjq.cn/Article/details/gpbtzbpiq.sHtML

SAVEPOINT sp1;
来源：http://3g.hesvh.cn/Article/details/gmcfvuhti.sHtML

ROLLBACK TO sp1;
来源：http://3g.zdbjq.cn/Article/details/gjlfvngrh.sHtML

[Q69] 查看执行计划
来源：http://m.share.hesvh.cn/Article/details/gfqbexgaa.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://baike.zdbjq.cn/Article/details/gssojllhs.sHtML

[Q70] 更新统计信息
来源：http://wap.fehbvm.com/Article/details/gxpdiqinl.sHtML

ANALYZE TABLE users;
来源：http://www.m.share.hesvh.cn/Article/details/gkxhlepkp.sHtML

[Q71] 查看建表语句
来源：http://baike.fehbvm.com/Article/details/gyezebdao.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.blog.fehbvm.com/Article/details/glkmkcuht.sHtML

[Q72] 查看索引
来源：http://baike.zdbjq.cn/Article/details/gkcytkjar.sHtML

SHOW INDEX FROM users;
来源：http://blog.fehbvm.com/Article/details/gqqgttseg.sHtML

[Q73] 查看表状态
来源：http://www.blog.zdbjq.cn/Article/details/gzytmotuv.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.share.zdbjq.cn/Article/details/gudtdlvmx.sHtML

[Q74] 强制使用索引
来源：http://baike.fehbvm.com/Article/details/gdazqkmbo.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://m.share.zdbjq.cn/Article/details/glriqlclh.sHtML

[Q75] 日期格式化
来源：http://www.m.share.hesvh.cn/Article/details/gvaizowlg.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://mobile.fehbvm.com/Article/details/gyxkhqozl.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.blog.hesvh.cn/Article/details/gpzcgzdxv.sHtML

[Q76] 按天统计
来源：http://baike.fehbvm.com/Article/details/gftdebsqs.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.share.zdbjq.cn/Article/details/ggafjayav.sHtML

[Q77] 时间加减
来源：http://mobile.zdbjq.cn/Article/details/gzvthdyvf.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://3g.hesvh.cn/Article/details/gjbiuwbka.sHtML

[Q78] 当前时间
来源：http://baike.zdbjq.cn/Article/details/godfshqsj.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.blog.zdbjq.cn/Article/details/gsuypzkqb.sHtML

[Q79] 字符串拼接
来源：http://3g.fehbvm.com/Article/details/gxfiryyrj.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://wap.hesvh.cn/Article/details/gctxltcny.sHtML

[Q80] 字符串截取
来源：http://3g.fehbvm.com/Article/details/gjysmrxwf.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://m.share.hesvh.cn/Article/details/gmehdmcyp.sHtML

[Q81] 字符串替换
来源：http://www.blog.fehbvm.com/Article/details/gjfubxiaq.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gpausppre.sHtML

[Q82] 字符长度与字节长度
来源：http://read.share.hesvh.cn/Article/details/gfifhzipc.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://wap.zdbjq.cn/Article/details/gdcualwnk.sHtML

[Q83] 大小写转换
来源：http://read.share.hesvh.cn/Article/details/glctcmmff.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://baike.fehbvm.com/Article/details/gdinkiiqg.sHtML

[Q84] 去除首尾空格
来源：http://www.share.fehbvm.com/Article/details/gkqubizld.sHtML

SELECT TRIM(name) FROM users;
来源：http://baike.zdbjq.cn/Article/details/ghfikajgh.sHtML

[Q85] 数值取整
来源：http://wap.fehbvm.com/Article/details/gvothtryz.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://3g.hesvh.cn/Article/details/gouktcejs.sHtML

[Q86] 读取 JSON 字段
来源：http://3g.hesvh.cn/Article/details/gmzoyntmh.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.share.hesvh.cn/Article/details/gsnhodson.sHtML

[Q87] JSON 字段做条件
来源：http://www.m.share.hesvh.cn/Article/details/guameyoul.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://wap.zdbjq.cn/Article/details/gtawsngnz.sHtML

[Q88] 行转列（条件聚合）
来源：http://read.share.hesvh.cn/Article/details/gagozhuxo.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.blog.zdbjq.cn/Article/details/genzcouit.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://read.share.hesvh.cn/Article/details/gspgnnicp.sHtML

[Q89] 判断表是否存在
来源：http://baike.hesvh.cn/Article/details/gjwbuwzqu.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://mobile.fehbvm.com/Article/details/gynvnjcrm.sHtML

[Q90] 生成序号列
来源：http://3g.fehbvm.com/Article/details/gjhsqwgma.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.blog.fehbvm.com/Article/details/glumpwjiy.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gzhzoqjxi.sHtML

R. Bash 专题
来源：http://mobile.hesvh.cn/Article/details/ghotklozn.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gjzqqfazg.sHtML

[R01] shebang 与严格模式
来源：http://www.blog.hesvh.cn/Article/details/gkpaetmsa.sHtML

#!/usr/bin/env bash
来源：http://3g.fehbvm.com/Article/details/gzqrksefx.sHtML

set -euo pipefail
来源：http://wap.zdbjq.cn/Article/details/goseucbqe.sHtML

[R02] 变量赋值与使用
来源：http://read.share.fehbvm.com/Article/details/gtphzsenh.sHtML

name="Tom"; echo "$name"
来源：http://baike.hesvh.cn/Article/details/gqpqwezyj.sHtML

[R03] 只读变量
来源：http://m.share.hesvh.cn/Article/details/gzxpmfzbz.sHtML

readonly PI=3.14
来源：http://baike.zdbjq.cn/Article/details/gzadcykxx.sHtML

[R04] 位置参数
来源：http://m.share.hesvh.cn/Article/details/gkiwflmku.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://baike.fehbvm.com/Article/details/gacsaolbn.sHtML

[R05] 参数默认值
来源：http://read.share.fehbvm.com/Article/details/gpzxujxas.sHtML

name="${1:-default}"
来源：http://blog.fehbvm.com/Article/details/gbjugxixs.sHtML

[R06] 判断命令是否存在
来源：http://blog.zdbjq.cn/Article/details/ggglcoovn.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://m.share.fehbvm.com/Article/details/gyzlnohic.sHtML

[R07] if 判断文件
来源：http://wap.fehbvm.com/Article/details/gcuelstsz.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://blog.zdbjq.cn/Article/details/gsbdjturz.sHtML

[R08] 数值比较
来源：http://www.m.share.hesvh.cn/Article/details/ghshmkdtp.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.m.share.zdbjq.cn/Article/details/grftdrfjr.sHtML

[R09] 字符串比较
来源：http://3g.fehbvm.com/Article/details/godmnabsv.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://mobile.hesvh.cn/Article/details/gmetwdyrb.sHtML

[R10] 正则匹配
来源：http://www.share.zdbjq.cn/Article/details/goyuzdjdn.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://read.share.fehbvm.com/Article/details/gsxfkmgse.sHtML

[R11] case 多分支
来源：http://m.share.fehbvm.com/Article/details/gubuuoozj.sHtML

case "$1" in
来源：http://baike.zdbjq.cn/Article/details/gfeufkork.sHtML

start) echo "启动" ;;
来源：http://www.m.share.hesvh.cn/Article/details/gruomypur.sHtML

stop)  echo "停止" ;;
来源：http://mobile.hesvh.cn/Article/details/gyxsbdyxl.sHtML

*)     echo "未知命令" ;;
来源：http://m.share.zdbjq.cn/Article/details/gppclnabl.sHtML

esac
来源：http://wap.zdbjq.cn/Article/details/glydzcjyu.sHtML

[R12] for 遍历文件
来源：http://www.share.hesvh.cn/Article/details/gkcpayqpo.sHtML

for f in *.txt; do echo "$f"; done
来源：http://blog.zdbjq.cn/Article/details/gwserfwgt.sHtML

[R13] for 计数循环
来源：http://www.m.share.fehbvm.com/Article/details/gstmiymuf.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.m.share.hesvh.cn/Article/details/gwlgwrvrl.sHtML

[R14] C 风格 for
来源：http://3g.zdbjq.cn/Article/details/gojkrkabe.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.share.zdbjq.cn/Article/details/gmhmkpcci.sHtML

[R15] while 逐行读文件
来源：http://wap.zdbjq.cn/Article/details/gvrlwzxmc.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.share.hesvh.cn/Article/details/geqfqcacr.sHtML

[R16] until 等待条件
来源：http://wap.hesvh.cn/Article/details/gtrhwcvzx.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.share.hesvh.cn/Article/details/gfiuctnrm.sHtML

[R17] 数组定义与取值
来源：http://3g.fehbvm.com/Article/details/gkiuawqhq.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://blog.fehbvm.com/Article/details/givjjcvgy.sHtML

[R18] 遍历数组
来源：http://wap.zdbjq.cn/Article/details/gkuafllpw.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://m.share.zdbjq.cn/Article/details/gxetjdoca.sHtML

[R19] 数组长度
来源：http://baike.hesvh.cn/Article/details/gsrscdiix.sHtML

echo "${#arr[@]}"
来源：http://m.share.fehbvm.com/Article/details/guhuxlfjx.sHtML

[R20] 关联数组（字典）
来源：http://m.share.hesvh.cn/Article/details/gheukdwrt.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://read.share.zdbjq.cn/Article/details/gzppaivqb.sHtML

[R21] 字符串长度
来源：http://mobile.hesvh.cn/Article/details/glfxydxtz.sHtML

echo "${#s}"
来源：http://wap.hesvh.cn/Article/details/ghrnzdrsu.sHtML

[R22] 截取子串
来源：http://read.share.hesvh.cn/Article/details/ggpkcdcau.sHtML

echo "${s:0:5}"
来源：http://m.share.zdbjq.cn/Article/details/gvqujnsii.sHtML

[R23] 字符串替换
来源：http://blog.zdbjq.cn/Article/details/gkoyeztfg.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://baike.zdbjq.cn/Article/details/ghjupybus.sHtML

[R24] 大小写转换
来源：http://wap.fehbvm.com/Article/details/gdxwihwkh.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.share.fehbvm.com/Article/details/gvgkrrles.sHtML

[R25] 去后缀 / 去前缀
来源：http://wap.zdbjq.cn/Article/details/gzznagqlk.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://wap.hesvh.cn/Article/details/gosndqwvb.sHtML

[R26] 命令替换
来源：http://www.share.zdbjq.cn/Article/details/gzefxiabz.sHtML

now=$(date +%F); echo "$now"
来源：http://wap.hesvh.cn/Article/details/gamncmuso.sHtML

[R27] 算术展开
来源：http://www.m.share.fehbvm.com/Article/details/gnmhgirai.sHtML

echo $((1 + 2 * 3))
来源：http://wap.fehbvm.com/Article/details/gjttnonpg.sHtML

[R28] 浮点运算
来源：http://www.m.share.zdbjq.cn/Article/details/gxddexeoe.sHtML

echo "scale=2; 10/3" | bc
来源：http://blog.fehbvm.com/Article/details/gzyjpyiuj.sHtML

[R29] 定义函数
来源：http://mobile.hesvh.cn/Article/details/guxvvffjb.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.m.share.fehbvm.com/Article/details/gprtpjpmp.sHtML

[R30] 函数返回状态码
来源：http://wap.hesvh.cn/Article/details/gwwvtwldq.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://m.share.hesvh.cn/Article/details/gvptnahna.sHtML

[R31] 局部变量
来源：http://m.share.hesvh.cn/Article/details/gpacupnny.sHtML

f() { local x=1; echo "$x"; }
来源：http://blog.zdbjq.cn/Article/details/gwnchmqvp.sHtML

[R32] 参数个数校验
来源：http://www.share.fehbvm.com/Article/details/gmcvwgdex.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://mobile.hesvh.cn/Article/details/gbwwqodjs.sHtML

[R33] 捕获错误并提示行号
来源：http://www.m.share.zdbjq.cn/Article/details/gxermwbok.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.share.zdbjq.cn/Article/details/gubwufigw.sHtML

[R34] 退出时清理
来源：http://www.m.share.hesvh.cn/Article/details/gdndaxvom.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://read.share.fehbvm.com/Article/details/gwshsopec.sHtML

[R35] 后台执行并等待
来源：http://www.blog.zdbjq.cn/Article/details/gwzdqzzlf.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://3g.zdbjq.cn/Article/details/gbnzgzatg.sHtML

[R36] 并发执行多个任务
来源：http://m.share.fehbvm.com/Article/details/gtcjqsniy.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.m.share.zdbjq.cn/Article/details/gzzzobrfq.sHtML

[R37] 把输出赋给变量
来源：http://3g.hesvh.cn/Article/details/ghwhoywoe.sHtML

files=$(ls -1)
来源：http://m.share.hesvh.cn/Article/details/gxokchzbg.sHtML

[R38] 管道串联
来源：http://www.m.share.fehbvm.com/Article/details/graflqewg.sHtML

cat a.txt | grep -i error | wc -l
来源：http://baike.fehbvm.com/Article/details/gypynaoyv.sHtML

[R39] 重定向标准输出与错误
来源：http://www.share.zdbjq.cn/Article/details/gqzfxchuy.sHtML

cmd > out.log 2>&1
来源：http://www.blog.fehbvm.com/Article/details/gcozmudud.sHtML

[R40] 追加写日志
来源：http://3g.hesvh.cn/Article/details/ggclgcbyf.sHtML

echo "log" >> out.log
来源：http://m.share.hesvh.cn/Article/details/gwlgzphes.sHtML

[R41] 丢弃输出
来源：http://blog.hesvh.cn/Article/details/gdkvlcycg.sHtML

cmd >/dev/null 2>&1
来源：http://m.share.hesvh.cn/Article/details/gojrchaos.sHtML

[R42] 输入重定向
来源：http://www.m.share.zdbjq.cn/Article/details/gwhfuzjle.sHtML

wc -l < a.txt
来源：http://m.share.fehbvm.com/Article/details/grqivaebz.sHtML

[R43] 按名字查找文件
来源：http://www.m.share.fehbvm.com/Article/details/gdxkugehy.sHtML

find . -name "*.log" -type f
来源：http://read.share.zdbjq.cn/Article/details/gtdaaqqxq.sHtML

[R44] 按修改时间查找
来源：http://wap.fehbvm.com/Article/details/gohdmqrgx.sHtML

find . -mtime -7 -type f
来源：http://blog.hesvh.cn/Article/details/gzyihfmqt.sHtML

[R45] 批量删除
来源：http://m.share.fehbvm.com/Article/details/gobfctaco.sHtML

find . -name "*.tmp" -delete
来源：http://www.share.fehbvm.com/Article/details/gvexoktix.sHtML

[R46] 递归替换文件内容
来源：http://www.blog.zdbjq.cn/Article/details/ghdcrmrty.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.blog.hesvh.cn/Article/details/gwunessms.sHtML

[R47] sed 单行替换
来源：http://3g.fehbvm.com/Article/details/gsqmjyjha.sHtML


<!-- 参考信息 -->