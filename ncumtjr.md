代发 wailian999

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://wap.fehbvm.com/Article/details/gcgyiybws.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://3g.fehbvm.com/Article/details/giqjeqdmp.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://blog.hesvh.cn/Article/details/glaumociz.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.blog.zdbjq.cn/Article/details/gartafylh.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/guflrnvjz.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://baike.zdbjq.cn/Article/details/gszsdxfpg.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gkuifibex.sHtML

[Q01] 创建表
来源：http://blog.fehbvm.com/Article/details/gzoorzhwo.sHtML

CREATE TABLE users (
来源：http://m.share.fehbvm.com/Article/details/gciafowut.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.hesvh.cn/Article/details/gqostyeub.sHtML

name VARCHAR(50) NOT NULL,
来源：http://m.share.fehbvm.com/Article/details/gsfbaknaw.sHtML

email VARCHAR(100) UNIQUE,
来源：http://read.share.hesvh.cn/Article/details/ghxdewzbq.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.m.share.fehbvm.com/Article/details/gdrypkvfk.sHtML

);
来源：http://mobile.fehbvm.com/Article/details/gzejetuib.sHtML

[Q02] 创建带外键的表
来源：http://mobile.fehbvm.com/Article/details/glskayfeg.sHtML

CREATE TABLE orders (
来源：http://baike.zdbjq.cn/Article/details/gqhxvvjmm.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.fehbvm.com/Article/details/gddrhmxod.sHtML

user_id INT NOT NULL,
来源：http://www.share.fehbvm.com/Article/details/ghozyfira.sHtML

amount DECIMAL(10, 2),
来源：http://read.share.hesvh.cn/Article/details/gwggozavn.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.share.fehbvm.com/Article/details/ghmjnvmav.sHtML

);
来源：http://baike.fehbvm.com/Article/details/gqaluofec.sHtML

[Q03] 增加列
来源：http://baike.fehbvm.com/Article/details/gjdfqwtvf.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.blog.zdbjq.cn/Article/details/gchrwsfkb.sHtML

[Q04] 修改列类型
来源：http://read.share.zdbjq.cn/Article/details/gmdiyxxry.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://wap.fehbvm.com/Article/details/gyqbwwkqp.sHtML

[Q05] 重命名列
来源：http://read.share.fehbvm.com/Article/details/gcjqfsfre.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://mobile.hesvh.cn/Article/details/gljmpijtt.sHtML

[Q06] 删除列
来源：http://wap.hesvh.cn/Article/details/giqllwdpk.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://m.share.fehbvm.com/Article/details/govaikjlu.sHtML

[Q07] 删除表
来源：http://baike.fehbvm.com/Article/details/gtgevkwfi.sHtML

DROP TABLE IF EXISTS orders;
来源：http://mobile.hesvh.cn/Article/details/gcrkdhfck.sHtML

[Q08] 创建普通索引
来源：http://www.m.share.zdbjq.cn/Article/details/gefcceaak.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.m.share.hesvh.cn/Article/details/gjpkhsvph.sHtML

[Q09] 创建唯一索引
来源：http://3g.fehbvm.com/Article/details/gmqdixoeo.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://mobile.hesvh.cn/Article/details/gtcowpykc.sHtML

[Q10] 插入单行
来源：http://mobile.zdbjq.cn/Article/details/gtcfibyje.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://baike.zdbjq.cn/Article/details/gjylqqeyu.sHtML

[Q11] 一次插入多行
来源：http://wap.hesvh.cn/Article/details/gvvgunaam.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.blog.zdbjq.cn/Article/details/gtrrlwgpl.sHtML

[Q12] 插入后取自增 ID
来源：http://3g.hesvh.cn/Article/details/gvkpvpjat.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.m.share.fehbvm.com/Article/details/gpmahrzio.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://blog.fehbvm.com/Article/details/gojtuqxzf.sHtML

[Q13] 忽略重复插入
来源：http://www.blog.fehbvm.com/Article/details/gsgbwxksd.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://read.share.hesvh.cn/Article/details/gmiembubw.sHtML

[Q14] 存在则更新（upsert）
来源：http://3g.hesvh.cn/Article/details/gflrusfsq.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://3g.hesvh.cn/Article/details/gifxldlxw.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://blog.zdbjq.cn/Article/details/gxylcinkd.sHtML

[Q15] 查询全部
来源：http://baike.hesvh.cn/Article/details/gcjrgsfes.sHtML

SELECT * FROM users;
来源：http://read.share.fehbvm.com/Article/details/gbiaogyhc.sHtML

[Q16] 查询指定列
来源：http://www.blog.hesvh.cn/Article/details/gqtqgoghf.sHtML

SELECT id, name FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gxctpmxqi.sHtML

[Q17] 条件查询
来源：http://m.share.fehbvm.com/Article/details/gecvedxde.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://m.share.fehbvm.com/Article/details/gaoflkgbh.sHtML

[Q18] 模糊匹配
来源：http://3g.hesvh.cn/Article/details/gzbrwblfx.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://baike.zdbjq.cn/Article/details/gsfokzmdx.sHtML

[Q19] 范围查询
来源：http://read.share.fehbvm.com/Article/details/gigbvccur.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://mobile.zdbjq.cn/Article/details/gypgbymmd.sHtML

[Q20] IN 列表
来源：http://m.share.fehbvm.com/Article/details/gophgdggg.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.share.zdbjq.cn/Article/details/gxoyftgno.sHtML

[Q21] 空值判断
来源：http://www.m.share.fehbvm.com/Article/details/gyaudehok.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://wap.zdbjq.cn/Article/details/gbyqgnumd.sHtML

[Q22] 排序
来源：http://mobile.zdbjq.cn/Article/details/gtlhqqtcc.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://wap.zdbjq.cn/Article/details/gxvpoxmig.sHtML

[Q23] 分页
来源：http://www.share.zdbjq.cn/Article/details/gzznfsobh.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.share.zdbjq.cn/Article/details/gbvttrghw.sHtML

[Q24] 去重
来源：http://read.share.zdbjq.cn/Article/details/gdjvqtehx.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.share.fehbvm.com/Article/details/glrabffka.sHtML

[Q25] 只取前 N 条
来源：http://www.m.share.hesvh.cn/Article/details/gotarylvx.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://wap.hesvh.cn/Article/details/gviiubfms.sHtML

[Q26] 计数
来源：http://www.share.zdbjq.cn/Article/details/gaogtvxhu.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gjffffryy.sHtML

[Q27] 条件计数
来源：http://read.share.hesvh.cn/Article/details/gfzykksqo.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.blog.fehbvm.com/Article/details/ghihlharb.sHtML

[Q28] 求和与平均
来源：http://read.share.zdbjq.cn/Article/details/gghyutcfj.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://blog.fehbvm.com/Article/details/gonowvlwn.sHtML

[Q29] 最大最小值
来源：http://m.share.fehbvm.com/Article/details/gzavebofo.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://3g.fehbvm.com/Article/details/gjfvrbrtd.sHtML

[Q30] 分组统计
来源：http://www.blog.fehbvm.com/Article/details/gxtvwlevc.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://m.share.zdbjq.cn/Article/details/gunfnryru.sHtML

[Q31] 分组后过滤
来源：http://www.blog.hesvh.cn/Article/details/gcuqucyvk.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://blog.fehbvm.com/Article/details/gmrqhomzr.sHtML

[Q32] 分组拼接字符串
来源：http://www.share.zdbjq.cn/Article/details/giudrfzli.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://baike.zdbjq.cn/Article/details/gnxhusvco.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://blog.zdbjq.cn/Article/details/gfvfiqoag.sHtML

[Q33] 多列分组
来源：http://mobile.hesvh.cn/Article/details/gvzcbysyf.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://m.share.zdbjq.cn/Article/details/gjzukqomy.sHtML

[Q34] 每组取第一条
来源：http://www.m.share.fehbvm.com/Article/details/gyoxzhhcn.sHtML

SELECT * FROM (
来源：http://blog.zdbjq.cn/Article/details/guvcbtdsb.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.share.fehbvm.com/Article/details/gcxyyqztc.sHtML

) t WHERE rn = 1;
来源：http://wap.fehbvm.com/Article/details/gmywdelax.sHtML

[Q35] 内连接
来源：http://mobile.fehbvm.com/Article/details/grfcpnhmw.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://mobile.hesvh.cn/Article/details/gslyvvqhy.sHtML

[Q36] 左连接
来源：http://www.m.share.zdbjq.cn/Article/details/guuzcxnqv.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://baike.zdbjq.cn/Article/details/gsmfqhvww.sHtML

[Q37] 右连接
来源：http://mobile.hesvh.cn/Article/details/gdzqhslqe.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://3g.zdbjq.cn/Article/details/gifejtvyt.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://wap.hesvh.cn/Article/details/gyvdxhxdb.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://baike.zdbjq.cn/Article/details/gynwvqumm.sHtML

[Q39] 自连接（查上下级）
来源：http://wap.hesvh.cn/Article/details/gjnheurzd.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://baike.zdbjq.cn/Article/details/gaqxxejgd.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://wap.hesvh.cn/Article/details/gxyqabxbx.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://3g.fehbvm.com/Article/details/gymbcahwd.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://read.share.hesvh.cn/Article/details/gbwreheki.sHtML

[Q41] 多表连接
来源：http://blog.hesvh.cn/Article/details/gegxikzyt.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://wap.hesvh.cn/Article/details/giovprblf.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.share.hesvh.cn/Article/details/gyoisjsfu.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://read.share.zdbjq.cn/Article/details/gtwphlrov.sHtML

[Q42] 连接条件附加过滤
来源：http://read.share.hesvh.cn/Article/details/glidcohtc.sHtML

SELECT u.name, o.amount FROM users u
来源：http://blog.hesvh.cn/Article/details/gabtprohh.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://3g.hesvh.cn/Article/details/gwrsqpvpk.sHtML

[Q43] 标量子查询
来源：http://mobile.fehbvm.com/Article/details/gkzxkupzn.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.share.hesvh.cn/Article/details/gtztrjjdv.sHtML

[Q44] IN 子查询
来源：http://3g.zdbjq.cn/Article/details/gxxztvtog.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.blog.zdbjq.cn/Article/details/gyghtmaqu.sHtML

[Q45] EXISTS 判断存在
来源：http://3g.zdbjq.cn/Article/details/gddgtfvpa.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.zdbjq.cn/Article/details/gwmkralbr.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://read.share.zdbjq.cn/Article/details/gpfojzokp.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.fehbvm.com/Article/details/gwtvasilq.sHtML

[Q47] 与平均值比较
来源：http://www.m.share.hesvh.cn/Article/details/gpltalrsj.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.blog.fehbvm.com/Article/details/gszcyhgko.sHtML

[Q48] CTE 公用表表达式
来源：http://read.share.hesvh.cn/Article/details/gistlbhyj.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.share.zdbjq.cn/Article/details/ghrteyjgq.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.m.share.zdbjq.cn/Article/details/gjqbwoaut.sHtML

[Q49] 更新单行
来源：http://wap.fehbvm.com/Article/details/gaexgxmfj.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.blog.hesvh.cn/Article/details/gxlwjlupn.sHtML

[Q50] 批量更新
来源：http://wap.hesvh.cn/Article/details/gvgigyfzm.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://3g.zdbjq.cn/Article/details/gfwlhlfka.sHtML

[Q51] 用子查询更新
来源：http://m.share.fehbvm.com/Article/details/gihwiawsd.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://m.share.hesvh.cn/Article/details/gbdcyqkrr.sHtML

[Q52] 删除指定行
来源：http://baike.fehbvm.com/Article/details/gcehyczsz.sHtML

DELETE FROM users WHERE id = 10;
来源：http://wap.fehbvm.com/Article/details/gnrnkzqqm.sHtML

[Q53] 按条件删除
来源：http://www.m.share.zdbjq.cn/Article/details/gippgbdzq.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://wap.zdbjq.cn/Article/details/gtjfbbajh.sHtML

[Q54] 清空表
来源：http://blog.zdbjq.cn/Article/details/gloxefuxe.sHtML

TRUNCATE TABLE logs;
来源：http://blog.fehbvm.com/Article/details/gqraekfld.sHtML

[Q55] 排名（并列占位）
来源：http://read.share.fehbvm.com/Article/details/gdvxdnlcp.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://read.share.fehbvm.com/Article/details/gezorjqce.sHtML

[Q56] 密集排名（并列不占位）
来源：http://baike.zdbjq.cn/Article/details/gsuxbqviw.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://3g.fehbvm.com/Article/details/gfrmecahw.sHtML

[Q57] 行号
来源：http://www.m.share.hesvh.cn/Article/details/gakjmjupl.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://wap.fehbvm.com/Article/details/gpkodjiuy.sHtML

[Q58] 累计求和
来源：http://mobile.fehbvm.com/Article/details/giewluqdx.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://baike.fehbvm.com/Article/details/gdyaywmal.sHtML

[Q59] 分组内累计
来源：http://wap.fehbvm.com/Article/details/gholvpihs.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.share.fehbvm.com/Article/details/gvoftbrwh.sHtML

[Q60] 取上一行 / 下一行
来源：http://wap.zdbjq.cn/Article/details/gtxycqpua.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://mobile.hesvh.cn/Article/details/gjlynqrsn.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.share.fehbvm.com/Article/details/gwqqbtesj.sHtML

[Q61] 移动平均
来源：http://www.m.share.hesvh.cn/Article/details/gucraioxo.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.blog.zdbjq.cn/Article/details/gxcyylzta.sHtML

[Q62] 分组占比
来源：http://www.blog.fehbvm.com/Article/details/gvhqjajel.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://blog.fehbvm.com/Article/details/gaivpbubg.sHtML

[Q63] 开启事务
来源：http://3g.fehbvm.com/Article/details/guoebzhuz.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.blog.hesvh.cn/Article/details/gtuyfgoeg.sHtML

[Q64] 提交事务
来源：http://www.blog.zdbjq.cn/Article/details/gihupjzji.sHtML

COMMIT;
来源：http://read.share.zdbjq.cn/Article/details/gvfbtdlqk.sHtML

[Q65] 回滚事务
来源：http://baike.hesvh.cn/Article/details/gdsywruxq.sHtML

ROLLBACK;
来源：http://www.share.fehbvm.com/Article/details/gpfvdsmbe.sHtML

[Q66] 行锁查询
来源：http://3g.fehbvm.com/Article/details/gixehxrjv.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://mobile.zdbjq.cn/Article/details/gclsleabu.sHtML

[Q67] 设置隔离级别
来源：http://mobile.zdbjq.cn/Article/details/gwespiudy.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://3g.fehbvm.com/Article/details/geaivkcal.sHtML

[Q68] 保存点
来源：http://read.share.fehbvm.com/Article/details/gwnrcckjw.sHtML

SAVEPOINT sp1;
来源：http://3g.hesvh.cn/Article/details/gxpkgwtsz.sHtML

ROLLBACK TO sp1;
来源：http://baike.zdbjq.cn/Article/details/gueauvxmu.sHtML

[Q69] 查看执行计划
来源：http://baike.zdbjq.cn/Article/details/gwpvvrogz.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.blog.fehbvm.com/Article/details/giknxqjmz.sHtML

[Q70] 更新统计信息
来源：http://www.share.zdbjq.cn/Article/details/gbonlyuvv.sHtML

ANALYZE TABLE users;
来源：http://wap.zdbjq.cn/Article/details/gnfzxxjpm.sHtML

[Q71] 查看建表语句
来源：http://www.m.share.fehbvm.com/Article/details/gsdkcvlmz.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.blog.hesvh.cn/Article/details/gcuzxitts.sHtML

[Q72] 查看索引
来源：http://m.share.zdbjq.cn/Article/details/gzhhhshus.sHtML

SHOW INDEX FROM users;
来源：http://www.share.fehbvm.com/Article/details/gjmtlfvdi.sHtML

[Q73] 查看表状态
来源：http://mobile.zdbjq.cn/Article/details/gtsyiqrwk.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://wap.fehbvm.com/Article/details/gytxvjvmi.sHtML

[Q74] 强制使用索引
来源：http://www.share.hesvh.cn/Article/details/gwfyxwomj.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://read.share.zdbjq.cn/Article/details/gxhmegwms.sHtML

[Q75] 日期格式化
来源：http://m.share.fehbvm.com/Article/details/ghdobcapf.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://3g.hesvh.cn/Article/details/gssjiqntl.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://mobile.zdbjq.cn/Article/details/gdixdeqki.sHtML

[Q76] 按天统计
来源：http://3g.hesvh.cn/Article/details/gvtjhdmct.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://baike.hesvh.cn/Article/details/goipihuik.sHtML

[Q77] 时间加减
来源：http://wap.hesvh.cn/Article/details/giwnhiubk.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://blog.fehbvm.com/Article/details/gmuwkvefp.sHtML

[Q78] 当前时间
来源：http://www.m.share.zdbjq.cn/Article/details/gfnbskwmo.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://wap.hesvh.cn/Article/details/gzuxdeziw.sHtML

[Q79] 字符串拼接
来源：http://m.share.hesvh.cn/Article/details/gdepmbpqn.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://wap.zdbjq.cn/Article/details/gtapproqb.sHtML

[Q80] 字符串截取
来源：http://3g.hesvh.cn/Article/details/gylidujqo.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://mobile.hesvh.cn/Article/details/gdxlblmsu.sHtML

[Q81] 字符串替换
来源：http://blog.hesvh.cn/Article/details/gnkkfepfj.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://blog.hesvh.cn/Article/details/ghrqqalfj.sHtML

[Q82] 字符长度与字节长度
来源：http://blog.hesvh.cn/Article/details/gqhznlyjp.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.share.fehbvm.com/Article/details/gzepifklp.sHtML

[Q83] 大小写转换
来源：http://baike.hesvh.cn/Article/details/grkmzpgqp.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://read.share.fehbvm.com/Article/details/gghaxolte.sHtML

[Q84] 去除首尾空格
来源：http://www.share.hesvh.cn/Article/details/gpyovcmuz.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gpcddxmjn.sHtML

[Q85] 数值取整
来源：http://baike.zdbjq.cn/Article/details/guwpjpbsf.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://3g.zdbjq.cn/Article/details/gkrdiapxt.sHtML

[Q86] 读取 JSON 字段
来源：http://m.share.fehbvm.com/Article/details/gdhdwukrv.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://baike.zdbjq.cn/Article/details/gdrwsqcmg.sHtML

[Q87] JSON 字段做条件
来源：http://wap.hesvh.cn/Article/details/gnuwpqlcv.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.share.zdbjq.cn/Article/details/glpjyjyfb.sHtML

[Q88] 行转列（条件聚合）
来源：http://blog.hesvh.cn/Article/details/gcwcgeeqy.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://read.share.zdbjq.cn/Article/details/gytzxczyv.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.share.fehbvm.com/Article/details/gmjjqyimo.sHtML

[Q89] 判断表是否存在
来源：http://www.blog.zdbjq.cn/Article/details/gzpgdvvtw.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://blog.zdbjq.cn/Article/details/gbvvzzopf.sHtML

[Q90] 生成序号列
来源：http://www.share.fehbvm.com/Article/details/ghptudwsa.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://3g.hesvh.cn/Article/details/goslypfyr.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gbuhgaukt.sHtML

R. Bash 专题
来源：http://wap.zdbjq.cn/Article/details/guxgrszlv.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gfauzazxm.sHtML

[R01] shebang 与严格模式
来源：http://3g.zdbjq.cn/Article/details/gcrnwcndt.sHtML

#!/usr/bin/env bash
来源：http://m.share.hesvh.cn/Article/details/gosgkhlle.sHtML

set -euo pipefail
来源：http://mobile.zdbjq.cn/Article/details/gfeqntlsc.sHtML

[R02] 变量赋值与使用
来源：http://3g.zdbjq.cn/Article/details/ghjujzrse.sHtML

name="Tom"; echo "$name"
来源：http://3g.hesvh.cn/Article/details/gfdvijyis.sHtML

[R03] 只读变量
来源：http://blog.zdbjq.cn/Article/details/gochtdpgi.sHtML

readonly PI=3.14
来源：http://read.share.hesvh.cn/Article/details/gcwxavust.sHtML

[R04] 位置参数
来源：http://www.blog.fehbvm.com/Article/details/gohwmhnim.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://blog.hesvh.cn/Article/details/gldsadawg.sHtML

[R05] 参数默认值
来源：http://wap.zdbjq.cn/Article/details/gjfasirwg.sHtML

name="${1:-default}"
来源：http://www.share.fehbvm.com/Article/details/gyzbmwlwl.sHtML

[R06] 判断命令是否存在
来源：http://read.share.zdbjq.cn/Article/details/gakwortik.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://baike.fehbvm.com/Article/details/gdknwnrww.sHtML

[R07] if 判断文件
来源：http://www.m.share.zdbjq.cn/Article/details/grrjugutu.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://wap.hesvh.cn/Article/details/gkuqvpkqu.sHtML

[R08] 数值比较
来源：http://mobile.zdbjq.cn/Article/details/gpxdphmwx.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.m.share.zdbjq.cn/Article/details/glzlkmopu.sHtML

[R09] 字符串比较
来源：http://www.m.share.fehbvm.com/Article/details/gocbooqwd.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://blog.fehbvm.com/Article/details/gwmfzuici.sHtML

[R10] 正则匹配
来源：http://www.m.share.zdbjq.cn/Article/details/geyidemat.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://m.share.hesvh.cn/Article/details/glczcrody.sHtML

[R11] case 多分支
来源：http://baike.fehbvm.com/Article/details/gxrxdyekk.sHtML

case "$1" in
来源：http://blog.fehbvm.com/Article/details/gxhczgdvf.sHtML

start) echo "启动" ;;
来源：http://blog.fehbvm.com/Article/details/gniyioedt.sHtML

stop)  echo "停止" ;;
来源：http://www.blog.zdbjq.cn/Article/details/gpahmwvvi.sHtML

*)     echo "未知命令" ;;
来源：http://m.share.hesvh.cn/Article/details/gcxwwfbiz.sHtML

esac
来源：http://read.share.hesvh.cn/Article/details/glglqrmpx.sHtML

[R12] for 遍历文件
来源：http://baike.fehbvm.com/Article/details/gfsgpreel.sHtML

for f in *.txt; do echo "$f"; done
来源：http://3g.hesvh.cn/Article/details/gkoecarug.sHtML

[R13] for 计数循环
来源：http://www.share.zdbjq.cn/Article/details/gqonfchds.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://3g.hesvh.cn/Article/details/gflougmun.sHtML

[R14] C 风格 for
来源：http://baike.fehbvm.com/Article/details/gjsprgryn.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://3g.zdbjq.cn/Article/details/gshrxabep.sHtML

[R15] while 逐行读文件
来源：http://blog.hesvh.cn/Article/details/grgxntcbq.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.m.share.fehbvm.com/Article/details/gsjotwkdb.sHtML

[R16] until 等待条件
来源：http://m.share.hesvh.cn/Article/details/gdycitvyt.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://read.share.fehbvm.com/Article/details/gvjubqiom.sHtML

[R17] 数组定义与取值
来源：http://baike.zdbjq.cn/Article/details/gkrucszno.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://blog.fehbvm.com/Article/details/gxqtaiolk.sHtML

[R18] 遍历数组
来源：http://www.blog.fehbvm.com/Article/details/gnxxxxfrw.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.m.share.hesvh.cn/Article/details/guxouvied.sHtML

[R19] 数组长度
来源：http://3g.fehbvm.com/Article/details/grvxdrlze.sHtML

echo "${#arr[@]}"
来源：http://www.share.zdbjq.cn/Article/details/gzkyhlrcp.sHtML

[R20] 关联数组（字典）
来源：http://www.share.fehbvm.com/Article/details/gpofscepw.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://m.share.hesvh.cn/Article/details/gkfrvpghg.sHtML

[R21] 字符串长度
来源：http://3g.fehbvm.com/Article/details/goemdlsdu.sHtML

echo "${#s}"
来源：http://www.share.fehbvm.com/Article/details/gqozfsaxc.sHtML

[R22] 截取子串
来源：http://blog.zdbjq.cn/Article/details/geslvdojz.sHtML

echo "${s:0:5}"
来源：http://read.share.fehbvm.com/Article/details/gqxwahpeq.sHtML

[R23] 字符串替换
来源：http://www.share.zdbjq.cn/Article/details/gqcvzmqan.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://baike.hesvh.cn/Article/details/guohgrwkj.sHtML

[R24] 大小写转换
来源：http://blog.hesvh.cn/Article/details/gzpvpwsmk.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://wap.hesvh.cn/Article/details/gidcldhax.sHtML

[R25] 去后缀 / 去前缀
来源：http://mobile.fehbvm.com/Article/details/gborbzwyw.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.share.fehbvm.com/Article/details/gqtsdaqum.sHtML

[R26] 命令替换
来源：http://wap.fehbvm.com/Article/details/giejvqhqd.sHtML

now=$(date +%F); echo "$now"
来源：http://read.share.fehbvm.com/Article/details/girluhwnb.sHtML

[R27] 算术展开
来源：http://wap.fehbvm.com/Article/details/ggxztktra.sHtML

echo $((1 + 2 * 3))
来源：http://m.share.hesvh.cn/Article/details/gszunsxhm.sHtML

[R28] 浮点运算
来源：http://mobile.hesvh.cn/Article/details/goytoknhk.sHtML

echo "scale=2; 10/3" | bc
来源：http://baike.zdbjq.cn/Article/details/gmcwaaqda.sHtML

[R29] 定义函数
来源：http://www.m.share.fehbvm.com/Article/details/gpstijptm.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.share.hesvh.cn/Article/details/guybfayrd.sHtML

[R30] 函数返回状态码
来源：http://www.share.fehbvm.com/Article/details/gzztevwwi.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://baike.fehbvm.com/Article/details/gvjxxlsib.sHtML

[R31] 局部变量
来源：http://mobile.fehbvm.com/Article/details/ghuoxdghq.sHtML

f() { local x=1; echo "$x"; }
来源：http://mobile.fehbvm.com/Article/details/gglswsiei.sHtML

[R32] 参数个数校验
来源：http://3g.hesvh.cn/Article/details/gawlqvndu.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://baike.fehbvm.com/Article/details/gocuvijga.sHtML

[R33] 捕获错误并提示行号
来源：http://3g.zdbjq.cn/Article/details/gywxrqgck.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://wap.zdbjq.cn/Article/details/gmsttphxv.sHtML

[R34] 退出时清理
来源：http://baike.fehbvm.com/Article/details/gnnyvoopy.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.fehbvm.com/Article/details/ggrspvhwe.sHtML

[R35] 后台执行并等待
来源：http://baike.zdbjq.cn/Article/details/gfkyjwoqn.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://wap.hesvh.cn/Article/details/giklifjho.sHtML

[R36] 并发执行多个任务
来源：http://read.share.zdbjq.cn/Article/details/gmwxxyaav.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.m.share.hesvh.cn/Article/details/ggzytjwns.sHtML

[R37] 把输出赋给变量
来源：http://www.blog.fehbvm.com/Article/details/gppbubdrz.sHtML

files=$(ls -1)
来源：http://www.share.zdbjq.cn/Article/details/gduooxvae.sHtML

[R38] 管道串联
来源：http://3g.fehbvm.com/Article/details/grfzlxwkf.sHtML

cat a.txt | grep -i error | wc -l
来源：http://baike.fehbvm.com/Article/details/gfnhytlgf.sHtML

[R39] 重定向标准输出与错误
来源：http://wap.fehbvm.com/Article/details/gitkjwigj.sHtML

cmd > out.log 2>&1
来源：http://www.blog.fehbvm.com/Article/details/gnrobfyrg.sHtML

[R40] 追加写日志
来源：http://3g.zdbjq.cn/Article/details/gxxfyephh.sHtML

echo "log" >> out.log
来源：http://3g.zdbjq.cn/Article/details/gyphsyoft.sHtML

[R41] 丢弃输出
来源：http://www.blog.fehbvm.com/Article/details/gblvhaybw.sHtML


<!-- 参考信息 -->