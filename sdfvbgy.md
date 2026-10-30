代发 wailian999

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://read.share.zdbjq.cn/Article/details/gpfaqccag.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://read.share.fehbvm.com/Article/details/gpnuseafo.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://m.share.zdbjq.cn/Article/details/gcuxjzbqi.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://wap.fehbvm.com/Article/details/gkffwyzxz.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/ghvazhdmc.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://wap.fehbvm.com/Article/details/gvuzojpem.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gjgywxssm.sHtML

[Q01] 创建表
来源：http://m.share.hesvh.cn/Article/details/gdzyhqndx.sHtML

CREATE TABLE users (
来源：http://baike.fehbvm.com/Article/details/gifjcndbv.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.fehbvm.com/Article/details/ggjiodxmk.sHtML

name VARCHAR(50) NOT NULL,
来源：http://baike.fehbvm.com/Article/details/grwqrasjb.sHtML

email VARCHAR(100) UNIQUE,
来源：http://mobile.fehbvm.com/Article/details/gywpiceoh.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://mobile.fehbvm.com/Article/details/gobzgnwwc.sHtML

);
来源：http://m.share.zdbjq.cn/Article/details/gaflcnaod.sHtML

[Q02] 创建带外键的表
来源：http://3g.fehbvm.com/Article/details/gcrrqvybi.sHtML

CREATE TABLE orders (
来源：http://www.m.share.zdbjq.cn/Article/details/gkjrgtcvw.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://mobile.fehbvm.com/Article/details/gjaziimyl.sHtML

user_id INT NOT NULL,
来源：http://3g.zdbjq.cn/Article/details/gejisxros.sHtML

amount DECIMAL(10, 2),
来源：http://www.m.share.hesvh.cn/Article/details/gjikqzdbc.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://blog.hesvh.cn/Article/details/gkhrmujtn.sHtML

);
来源：http://baike.hesvh.cn/Article/details/gizavnygc.sHtML

[Q03] 增加列
来源：http://blog.fehbvm.com/Article/details/gimovxhcu.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.share.zdbjq.cn/Article/details/gqvesfkax.sHtML

[Q04] 修改列类型
来源：http://www.m.share.zdbjq.cn/Article/details/gqhopbuez.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://blog.hesvh.cn/Article/details/gkkibgsiz.sHtML

[Q05] 重命名列
来源：http://baike.hesvh.cn/Article/details/giacyrrni.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.share.hesvh.cn/Article/details/gfroyovqm.sHtML

[Q06] 删除列
来源：http://baike.fehbvm.com/Article/details/gmybppgsj.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://3g.zdbjq.cn/Article/details/gmurbmnsc.sHtML

[Q07] 删除表
来源：http://wap.fehbvm.com/Article/details/gfqpxbeok.sHtML

DROP TABLE IF EXISTS orders;
来源：http://read.share.fehbvm.com/Article/details/gpecjbwwk.sHtML

[Q08] 创建普通索引
来源：http://wap.fehbvm.com/Article/details/gbsyszgmw.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://3g.fehbvm.com/Article/details/gyzcexuxe.sHtML

[Q09] 创建唯一索引
来源：http://m.share.fehbvm.com/Article/details/guhwsdzxy.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://m.share.fehbvm.com/Article/details/gmtdpcmpg.sHtML

[Q10] 插入单行
来源：http://www.share.zdbjq.cn/Article/details/gtgtomzom.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://wap.hesvh.cn/Article/details/ghwjfysam.sHtML

[Q11] 一次插入多行
来源：http://www.blog.hesvh.cn/Article/details/gbvezbntt.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.blog.fehbvm.com/Article/details/ghpbukqim.sHtML

[Q12] 插入后取自增 ID
来源：http://read.share.zdbjq.cn/Article/details/gyezdrgzk.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.m.share.hesvh.cn/Article/details/ggdfumlvk.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://read.share.zdbjq.cn/Article/details/gjigmxpib.sHtML

[Q13] 忽略重复插入
来源：http://read.share.hesvh.cn/Article/details/gppwqyvxb.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://baike.fehbvm.com/Article/details/gngjqnabv.sHtML

[Q14] 存在则更新（upsert）
来源：http://blog.fehbvm.com/Article/details/gxnfihicu.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://mobile.zdbjq.cn/Article/details/gypbqdkzi.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://mobile.hesvh.cn/Article/details/gdspfzqkf.sHtML

[Q15] 查询全部
来源：http://wap.hesvh.cn/Article/details/gwvleplqu.sHtML

SELECT * FROM users;
来源：http://m.share.zdbjq.cn/Article/details/guznmqbah.sHtML

[Q16] 查询指定列
来源：http://read.share.zdbjq.cn/Article/details/gentmwtgp.sHtML

SELECT id, name FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gstukzayy.sHtML

[Q17] 条件查询
来源：http://www.share.zdbjq.cn/Article/details/gcggxxcxs.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://m.share.fehbvm.com/Article/details/gnobqmubg.sHtML

[Q18] 模糊匹配
来源：http://baike.zdbjq.cn/Article/details/gmjuxabds.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://read.share.zdbjq.cn/Article/details/gauwxcvwn.sHtML

[Q19] 范围查询
来源：http://m.share.zdbjq.cn/Article/details/gjjykiwak.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://mobile.zdbjq.cn/Article/details/gyjsngrzu.sHtML

[Q20] IN 列表
来源：http://3g.zdbjq.cn/Article/details/gkrycjhny.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.share.fehbvm.com/Article/details/gxqgxaezd.sHtML

[Q21] 空值判断
来源：http://www.share.zdbjq.cn/Article/details/ghvgfkhoz.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.blog.fehbvm.com/Article/details/gtpkgnnzn.sHtML

[Q22] 排序
来源：http://www.m.share.hesvh.cn/Article/details/gjxsiwnit.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://mobile.fehbvm.com/Article/details/grysvppew.sHtML

[Q23] 分页
来源：http://baike.fehbvm.com/Article/details/gcledxktb.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://blog.fehbvm.com/Article/details/gtgupzcht.sHtML

[Q24] 去重
来源：http://read.share.hesvh.cn/Article/details/gbbxhigjn.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gsnkfvkbf.sHtML

[Q25] 只取前 N 条
来源：http://blog.fehbvm.com/Article/details/gieimojkr.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://read.share.zdbjq.cn/Article/details/gtsumftog.sHtML

[Q26] 计数
来源：http://mobile.zdbjq.cn/Article/details/gezcsjwuc.sHtML

SELECT COUNT(*) FROM users;
来源：http://mobile.hesvh.cn/Article/details/gxthndzhh.sHtML

[Q27] 条件计数
来源：http://www.share.hesvh.cn/Article/details/geqgbzwfq.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://baike.fehbvm.com/Article/details/gofqwlmnh.sHtML

[Q28] 求和与平均
来源：http://www.blog.zdbjq.cn/Article/details/gxxvatlgp.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://3g.fehbvm.com/Article/details/gjynsxifl.sHtML

[Q29] 最大最小值
来源：http://www.m.share.fehbvm.com/Article/details/ghggcganf.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://blog.fehbvm.com/Article/details/gydjankfn.sHtML

[Q30] 分组统计
来源：http://blog.hesvh.cn/Article/details/gmlvkegaa.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://mobile.zdbjq.cn/Article/details/gpzrjbtxp.sHtML

[Q31] 分组后过滤
来源：http://www.share.hesvh.cn/Article/details/guwynvzsn.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.m.share.zdbjq.cn/Article/details/gmwgjdcmm.sHtML

[Q32] 分组拼接字符串
来源：http://m.share.zdbjq.cn/Article/details/gwgjderqg.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://m.share.zdbjq.cn/Article/details/gxzruncoi.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://blog.fehbvm.com/Article/details/ggwwxwwpf.sHtML

[Q33] 多列分组
来源：http://wap.zdbjq.cn/Article/details/gomoflcii.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.blog.fehbvm.com/Article/details/gnpaaffgg.sHtML

[Q34] 每组取第一条
来源：http://baike.fehbvm.com/Article/details/grvryzqws.sHtML

SELECT * FROM (
来源：http://baike.zdbjq.cn/Article/details/gcnbsuave.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://baike.zdbjq.cn/Article/details/gnyiblphi.sHtML

) t WHERE rn = 1;
来源：http://wap.hesvh.cn/Article/details/gvvgghdzn.sHtML

[Q35] 内连接
来源：http://wap.fehbvm.com/Article/details/gnqiiyusz.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.share.hesvh.cn/Article/details/ghvatkndf.sHtML

[Q36] 左连接
来源：http://www.m.share.zdbjq.cn/Article/details/gfriwkcsf.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://blog.zdbjq.cn/Article/details/gekyodxxs.sHtML

[Q37] 右连接
来源：http://3g.hesvh.cn/Article/details/gkjdarzmo.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://3g.zdbjq.cn/Article/details/geatluqum.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://wap.hesvh.cn/Article/details/geslacvyk.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.m.share.zdbjq.cn/Article/details/golsdrteh.sHtML

[Q39] 自连接（查上下级）
来源：http://www.blog.zdbjq.cn/Article/details/ggujkjgbz.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://blog.zdbjq.cn/Article/details/gzucnwooe.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.share.zdbjq.cn/Article/details/gdfhmovtj.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://m.share.hesvh.cn/Article/details/gjsfceyxj.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://wap.zdbjq.cn/Article/details/gjjimubnu.sHtML

[Q41] 多表连接
来源：http://baike.fehbvm.com/Article/details/ghuefjjfl.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://3g.hesvh.cn/Article/details/grbplnrza.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.share.zdbjq.cn/Article/details/genkdqdaq.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://blog.zdbjq.cn/Article/details/gunvajbjn.sHtML

[Q42] 连接条件附加过滤
来源：http://www.m.share.hesvh.cn/Article/details/gavpgwtwp.sHtML

SELECT u.name, o.amount FROM users u
来源：http://baike.zdbjq.cn/Article/details/gwnzpihui.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.share.zdbjq.cn/Article/details/gzyvshceg.sHtML

[Q43] 标量子查询
来源：http://m.share.fehbvm.com/Article/details/ghoyentfg.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://mobile.zdbjq.cn/Article/details/gkitpibyn.sHtML

[Q44] IN 子查询
来源：http://wap.zdbjq.cn/Article/details/gmmtbvbeo.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.share.fehbvm.com/Article/details/gzujsawtb.sHtML

[Q45] EXISTS 判断存在
来源：http://baike.hesvh.cn/Article/details/gsbhdcvcw.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.zdbjq.cn/Article/details/gaswdisoz.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://blog.zdbjq.cn/Article/details/gspoouyco.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.fehbvm.com/Article/details/gdgznaamp.sHtML

[Q47] 与平均值比较
来源：http://www.m.share.hesvh.cn/Article/details/gvzwyhcrr.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.blog.hesvh.cn/Article/details/gimjkhysa.sHtML

[Q48] CTE 公用表表达式
来源：http://m.share.zdbjq.cn/Article/details/gkxxseivp.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://baike.fehbvm.com/Article/details/gzhgfdgsv.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.m.share.fehbvm.com/Article/details/gxwiceuep.sHtML

[Q49] 更新单行
来源：http://blog.hesvh.cn/Article/details/gfuofwbbu.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://blog.hesvh.cn/Article/details/gwsyrdscm.sHtML

[Q50] 批量更新
来源：http://www.m.share.fehbvm.com/Article/details/gwylevrla.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://blog.fehbvm.com/Article/details/ggghkxwkm.sHtML

[Q51] 用子查询更新
来源：http://read.share.hesvh.cn/Article/details/gubwknlsm.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.m.share.zdbjq.cn/Article/details/gyfuwalmt.sHtML

[Q52] 删除指定行
来源：http://3g.zdbjq.cn/Article/details/gvwmizkgy.sHtML

DELETE FROM users WHERE id = 10;
来源：http://3g.zdbjq.cn/Article/details/gjbbxxvyk.sHtML

[Q53] 按条件删除
来源：http://www.m.share.fehbvm.com/Article/details/glkmqnxzo.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://m.share.fehbvm.com/Article/details/gcrincnug.sHtML

[Q54] 清空表
来源：http://3g.hesvh.cn/Article/details/guzjvntus.sHtML

TRUNCATE TABLE logs;
来源：http://3g.fehbvm.com/Article/details/gnzibtlcp.sHtML

[Q55] 排名（并列占位）
来源：http://read.share.fehbvm.com/Article/details/goklnpjom.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.m.share.hesvh.cn/Article/details/gphcedfgz.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.share.fehbvm.com/Article/details/grxpvnswt.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://baike.hesvh.cn/Article/details/gcafypxji.sHtML

[Q57] 行号
来源：http://blog.zdbjq.cn/Article/details/gmnmdzxkp.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/govxpbrym.sHtML

[Q58] 累计求和
来源：http://baike.zdbjq.cn/Article/details/gpyvlpkee.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://baike.zdbjq.cn/Article/details/grzzaxppr.sHtML

[Q59] 分组内累计
来源：http://mobile.fehbvm.com/Article/details/gtkbpurqx.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://read.share.hesvh.cn/Article/details/gnrnpgryp.sHtML

[Q60] 取上一行 / 下一行
来源：http://baike.zdbjq.cn/Article/details/gmwmhugqq.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://wap.hesvh.cn/Article/details/grrfvgsvi.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://wap.fehbvm.com/Article/details/gxoeulknw.sHtML

[Q61] 移动平均
来源：http://www.blog.hesvh.cn/Article/details/gpqdpyxjh.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://m.share.zdbjq.cn/Article/details/genclvyzp.sHtML

[Q62] 分组占比
来源：http://m.share.hesvh.cn/Article/details/gwfltqxpp.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://blog.fehbvm.com/Article/details/geczjtagv.sHtML

[Q63] 开启事务
来源：http://read.share.hesvh.cn/Article/details/gnkgeltxr.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.blog.hesvh.cn/Article/details/gqfkkvlcs.sHtML

[Q64] 提交事务
来源：http://mobile.zdbjq.cn/Article/details/ggmptugdk.sHtML

COMMIT;
来源：http://baike.fehbvm.com/Article/details/gobpesjvz.sHtML

[Q65] 回滚事务
来源：http://blog.hesvh.cn/Article/details/ggvsfuhrj.sHtML

ROLLBACK;
来源：http://read.share.hesvh.cn/Article/details/gvbzmauni.sHtML

[Q66] 行锁查询
来源：http://www.m.share.hesvh.cn/Article/details/gmcxlsqwa.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://baike.fehbvm.com/Article/details/grzqnhshu.sHtML

[Q67] 设置隔离级别
来源：http://read.share.zdbjq.cn/Article/details/ghqamwfae.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://m.share.zdbjq.cn/Article/details/gcpoixbeh.sHtML

[Q68] 保存点
来源：http://www.blog.fehbvm.com/Article/details/gyqbrecce.sHtML

SAVEPOINT sp1;
来源：http://m.share.zdbjq.cn/Article/details/gbbaeabgp.sHtML

ROLLBACK TO sp1;
来源：http://www.blog.zdbjq.cn/Article/details/gqbdoewop.sHtML

[Q69] 查看执行计划
来源：http://www.share.hesvh.cn/Article/details/gtghnhdwx.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://baike.zdbjq.cn/Article/details/glwearalz.sHtML

[Q70] 更新统计信息
来源：http://3g.zdbjq.cn/Article/details/gbxxbgcjw.sHtML

ANALYZE TABLE users;
来源：http://www.blog.fehbvm.com/Article/details/gwecjgeef.sHtML

[Q71] 查看建表语句
来源：http://www.m.share.fehbvm.com/Article/details/gmxdbdofw.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://3g.fehbvm.com/Article/details/grqmdksyz.sHtML

[Q72] 查看索引
来源：http://www.share.fehbvm.com/Article/details/ghoorpomg.sHtML

SHOW INDEX FROM users;
来源：http://3g.fehbvm.com/Article/details/geqrbpxek.sHtML

[Q73] 查看表状态
来源：http://m.share.hesvh.cn/Article/details/gnaweniyq.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://blog.hesvh.cn/Article/details/gvjfnsupj.sHtML

[Q74] 强制使用索引
来源：http://wap.fehbvm.com/Article/details/gfwfyuxlq.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.share.hesvh.cn/Article/details/ggpninhrs.sHtML

[Q75] 日期格式化
来源：http://3g.fehbvm.com/Article/details/gpwhifypw.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://blog.hesvh.cn/Article/details/gvkzjvtqt.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.m.share.hesvh.cn/Article/details/gsjcopdit.sHtML

[Q76] 按天统计
来源：http://www.m.share.hesvh.cn/Article/details/gawqlpfss.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://read.share.fehbvm.com/Article/details/gndiavugf.sHtML

[Q77] 时间加减
来源：http://m.share.zdbjq.cn/Article/details/gldqcrlgo.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://blog.hesvh.cn/Article/details/guluvfjom.sHtML

[Q78] 当前时间
来源：http://baike.fehbvm.com/Article/details/gjtvvateg.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://3g.zdbjq.cn/Article/details/geujnjspe.sHtML

[Q79] 字符串拼接
来源：http://3g.hesvh.cn/Article/details/gumukbuzn.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://baike.fehbvm.com/Article/details/gnoxclrvw.sHtML

[Q80] 字符串截取
来源：http://wap.zdbjq.cn/Article/details/gbvxidaaj.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/glvrcdriw.sHtML

[Q81] 字符串替换
来源：http://mobile.zdbjq.cn/Article/details/gyfvbngcc.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.share.hesvh.cn/Article/details/gqwceimur.sHtML

[Q82] 字符长度与字节长度
来源：http://read.share.hesvh.cn/Article/details/gninrzffs.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://mobile.fehbvm.com/Article/details/gxgaxmrxn.sHtML

[Q83] 大小写转换
来源：http://mobile.zdbjq.cn/Article/details/gkmzlnggg.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://mobile.hesvh.cn/Article/details/gkqyczukl.sHtML

[Q84] 去除首尾空格
来源：http://wap.hesvh.cn/Article/details/gwazzszzk.sHtML

SELECT TRIM(name) FROM users;
来源：http://read.share.hesvh.cn/Article/details/gvtcqfjrd.sHtML

[Q85] 数值取整
来源：http://wap.hesvh.cn/Article/details/gullclzyo.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://m.share.fehbvm.com/Article/details/gchiijhfd.sHtML

[Q86] 读取 JSON 字段
来源：http://www.share.hesvh.cn/Article/details/gwoheythi.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://read.share.hesvh.cn/Article/details/gpjpgfrgc.sHtML

[Q87] JSON 字段做条件
来源：http://blog.hesvh.cn/Article/details/gafwfvivb.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://mobile.hesvh.cn/Article/details/gzxkphyqn.sHtML

[Q88] 行转列（条件聚合）
来源：http://wap.zdbjq.cn/Article/details/gxxrxgmkw.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://mobile.fehbvm.com/Article/details/gqntbmihi.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://3g.zdbjq.cn/Article/details/gxavmhzcp.sHtML

[Q89] 判断表是否存在
来源：http://3g.fehbvm.com/Article/details/gxvwoswii.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://blog.fehbvm.com/Article/details/gxadsdupd.sHtML

[Q90] 生成序号列
来源：http://mobile.fehbvm.com/Article/details/glsinafdm.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://mobile.fehbvm.com/Article/details/gkbbxttjn.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gbfhzzjaa.sHtML

R. Bash 专题
来源：http://mobile.fehbvm.com/Article/details/gnmzapxkm.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gfjebvyar.sHtML

[R01] shebang 与严格模式
来源：http://read.share.fehbvm.com/Article/details/glfdgkyqv.sHtML

#!/usr/bin/env bash
来源：http://3g.zdbjq.cn/Article/details/gbkqyhhxx.sHtML

set -euo pipefail
来源：http://read.share.fehbvm.com/Article/details/gfiotxnpu.sHtML

[R02] 变量赋值与使用
来源：http://www.blog.hesvh.cn/Article/details/glamgezna.sHtML

name="Tom"; echo "$name"
来源：http://m.share.fehbvm.com/Article/details/gpogpcxhu.sHtML

[R03] 只读变量
来源：http://mobile.fehbvm.com/Article/details/ghysscttj.sHtML

readonly PI=3.14
来源：http://3g.zdbjq.cn/Article/details/geqanstnn.sHtML

[R04] 位置参数
来源：http://www.m.share.zdbjq.cn/Article/details/grmmludfw.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://wap.zdbjq.cn/Article/details/gvtrtkfin.sHtML

[R05] 参数默认值
来源：http://wap.hesvh.cn/Article/details/gqetdinmr.sHtML

name="${1:-default}"
来源：http://3g.fehbvm.com/Article/details/gxmscusew.sHtML

[R06] 判断命令是否存在
来源：http://mobile.zdbjq.cn/Article/details/gkdxrasjc.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.blog.zdbjq.cn/Article/details/gkcoyiytd.sHtML

[R07] if 判断文件
来源：http://www.share.hesvh.cn/Article/details/gtzyoakdd.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.share.fehbvm.com/Article/details/gkjilmmbi.sHtML

[R08] 数值比较
来源：http://mobile.hesvh.cn/Article/details/gmhsytyxj.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://3g.fehbvm.com/Article/details/gvkbhiwyb.sHtML

[R09] 字符串比较
来源：http://www.share.hesvh.cn/Article/details/ggcskdjhs.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://baike.zdbjq.cn/Article/details/gizuczkye.sHtML

[R10] 正则匹配
来源：http://www.m.share.hesvh.cn/Article/details/gusokwnhv.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.m.share.hesvh.cn/Article/details/gpnviiohu.sHtML

[R11] case 多分支
来源：http://www.blog.zdbjq.cn/Article/details/gmvcpoiat.sHtML

case "$1" in
来源：http://blog.hesvh.cn/Article/details/gvjhdxgsz.sHtML

start) echo "启动" ;;
来源：http://blog.fehbvm.com/Article/details/gajinctsl.sHtML

stop)  echo "停止" ;;
来源：http://wap.fehbvm.com/Article/details/gzjpcqvso.sHtML

*)     echo "未知命令" ;;
来源：http://mobile.hesvh.cn/Article/details/gorryaofr.sHtML

esac
来源：http://blog.zdbjq.cn/Article/details/gpvdguxzo.sHtML

[R12] for 遍历文件
来源：http://www.blog.hesvh.cn/Article/details/goavdqkyb.sHtML

for f in *.txt; do echo "$f"; done
来源：http://read.share.hesvh.cn/Article/details/gdeeqsgpj.sHtML

[R13] for 计数循环
来源：http://blog.zdbjq.cn/Article/details/gfabhnaqv.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://m.share.zdbjq.cn/Article/details/gjusqnxjz.sHtML

[R14] C 风格 for
来源：http://m.share.zdbjq.cn/Article/details/grvfknbov.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://mobile.fehbvm.com/Article/details/gwqeaawei.sHtML

[R15] while 逐行读文件
来源：http://mobile.hesvh.cn/Article/details/gprlsghog.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://blog.hesvh.cn/Article/details/gecbdzcjl.sHtML

[R16] until 等待条件
来源：http://www.blog.fehbvm.com/Article/details/gxlihbbcd.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://3g.zdbjq.cn/Article/details/gbxokgasy.sHtML

[R17] 数组定义与取值
来源：http://m.share.zdbjq.cn/Article/details/giufbgrcx.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://read.share.zdbjq.cn/Article/details/ghwqrlpbf.sHtML

[R18] 遍历数组
来源：http://blog.hesvh.cn/Article/details/gddrzygys.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://wap.fehbvm.com/Article/details/gwxiibgtx.sHtML

[R19] 数组长度
来源：http://www.share.zdbjq.cn/Article/details/gbwewpxza.sHtML

echo "${#arr[@]}"
来源：http://3g.zdbjq.cn/Article/details/gpahibtbc.sHtML

[R20] 关联数组（字典）
来源：http://mobile.hesvh.cn/Article/details/goopaiysu.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://blog.zdbjq.cn/Article/details/gkktffzbv.sHtML

[R21] 字符串长度
来源：http://www.blog.hesvh.cn/Article/details/gffbyfdjo.sHtML

echo "${#s}"
来源：http://3g.fehbvm.com/Article/details/glgygrsuu.sHtML

[R22] 截取子串
来源：http://3g.hesvh.cn/Article/details/gqzcamwgj.sHtML

echo "${s:0:5}"
来源：http://www.share.hesvh.cn/Article/details/ghaxegpvb.sHtML

[R23] 字符串替换
来源：http://www.m.share.zdbjq.cn/Article/details/gawvfyuim.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://mobile.zdbjq.cn/Article/details/gqtfiydci.sHtML

[R24] 大小写转换
来源：http://www.blog.hesvh.cn/Article/details/gjeiubhpj.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://m.share.hesvh.cn/Article/details/gkfuipall.sHtML

[R25] 去后缀 / 去前缀
来源：http://m.share.hesvh.cn/Article/details/grzbjkktf.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://mobile.hesvh.cn/Article/details/gcgmtbeqv.sHtML

[R26] 命令替换
来源：http://baike.fehbvm.com/Article/details/gdtuvpcpt.sHtML

now=$(date +%F); echo "$now"
来源：http://www.share.fehbvm.com/Article/details/gsrffaehc.sHtML

[R27] 算术展开
来源：http://www.m.share.zdbjq.cn/Article/details/gwjlluofs.sHtML

echo $((1 + 2 * 3))
来源：http://read.share.zdbjq.cn/Article/details/gdhfcshdr.sHtML

[R28] 浮点运算
来源：http://read.share.zdbjq.cn/Article/details/gbopymuns.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.m.share.hesvh.cn/Article/details/gnffdkkee.sHtML

[R29] 定义函数
来源：http://3g.fehbvm.com/Article/details/gryzpdanx.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://m.share.fehbvm.com/Article/details/gvyhgdsok.sHtML

[R30] 函数返回状态码
来源：http://www.share.fehbvm.com/Article/details/gvlvhggmg.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.blog.fehbvm.com/Article/details/gmgckzdjd.sHtML

[R31] 局部变量
来源：http://3g.fehbvm.com/Article/details/gsqbqfmgp.sHtML

f() { local x=1; echo "$x"; }
来源：http://mobile.fehbvm.com/Article/details/gkqujcpfi.sHtML

[R32] 参数个数校验
来源：http://wap.hesvh.cn/Article/details/gpxbdlsie.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://m.share.zdbjq.cn/Article/details/ggjtcacwp.sHtML

[R33] 捕获错误并提示行号
来源：http://baike.fehbvm.com/Article/details/gaaapyxko.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://3g.hesvh.cn/Article/details/gyliizwzo.sHtML

[R34] 退出时清理
来源：http://blog.hesvh.cn/Article/details/ggwqtqkcm.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.share.fehbvm.com/Article/details/gmsbmwsjl.sHtML

[R35] 后台执行并等待
来源：http://m.share.zdbjq.cn/Article/details/gfiortone.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://blog.fehbvm.com/Article/details/guyudbwsf.sHtML

[R36] 并发执行多个任务
来源：http://read.share.zdbjq.cn/Article/details/gbsplnjzd.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://blog.zdbjq.cn/Article/details/gqicumkrt.sHtML

[R37] 把输出赋给变量
来源：http://3g.hesvh.cn/Article/details/gdsleswel.sHtML

files=$(ls -1)
来源：http://www.m.share.zdbjq.cn/Article/details/gxlyvlsyp.sHtML

[R38] 管道串联
来源：http://blog.zdbjq.cn/Article/details/gbmyyktmn.sHtML

cat a.txt | grep -i error | wc -l
来源：http://m.share.zdbjq.cn/Article/details/gkouauqzc.sHtML

[R39] 重定向标准输出与错误
来源：http://m.share.hesvh.cn/Article/details/grolpjijk.sHtML

cmd > out.log 2>&1
来源：http://blog.fehbvm.com/Article/details/ghgakhaxe.sHtML

[R40] 追加写日志
来源：http://www.m.share.hesvh.cn/Article/details/gmffumrsj.sHtML

echo "log" >> out.log
来源：http://baike.fehbvm.com/Article/details/gszbfnbeb.sHtML

[R41] 丢弃输出
来源：http://baike.hesvh.cn/Article/details/gnvbuijjg.sHtML


<!-- 参考信息 -->