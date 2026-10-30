代发 wailian999

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gkdwoxtci.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.blog.zdbjq.cn/Article/details/gqlheedtw.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gpdfjbrvg.sHtML

[Q01] 创建表
来源：http://read.share.fehbvm.com/Article/details/goiqjndnw.sHtML

CREATE TABLE users (
来源：http://www.blog.hesvh.cn/Article/details/gjfvypgxa.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.hesvh.cn/Article/details/gupmnvcht.sHtML

name VARCHAR(50) NOT NULL,
来源：http://read.share.hesvh.cn/Article/details/gxewrkrna.sHtML

email VARCHAR(100) UNIQUE,
来源：http://blog.fehbvm.com/Article/details/glfdjoaph.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.blog.fehbvm.com/Article/details/gwfpvscpt.sHtML

);
来源：http://3g.hesvh.cn/Article/details/gduicxfqe.sHtML

[Q02] 创建带外键的表
来源：http://wap.zdbjq.cn/Article/details/ganxtyzdz.sHtML

CREATE TABLE orders (
来源：http://3g.zdbjq.cn/Article/details/gmaaiwdgw.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.hesvh.cn/Article/details/gzjwfzbik.sHtML

user_id INT NOT NULL,
来源：http://mobile.hesvh.cn/Article/details/gymzznjfv.sHtML

amount DECIMAL(10, 2),
来源：http://3g.zdbjq.cn/Article/details/gdelzmedk.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://wap.hesvh.cn/Article/details/grsnltwht.sHtML

);
来源：http://read.share.fehbvm.com/Article/details/gixslqlob.sHtML

[Q03] 增加列
来源：http://m.share.fehbvm.com/Article/details/ghgpwatwn.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://baike.zdbjq.cn/Article/details/goeonvvvn.sHtML

[Q04] 修改列类型
来源：http://3g.hesvh.cn/Article/details/gxmllgqyb.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.share.zdbjq.cn/Article/details/gylzwlgxj.sHtML

[Q05] 重命名列
来源：http://read.share.fehbvm.com/Article/details/gpyqwxpwo.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://wap.fehbvm.com/Article/details/gibzzlgul.sHtML

[Q06] 删除列
来源：http://read.share.fehbvm.com/Article/details/gkvjryesn.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://read.share.fehbvm.com/Article/details/grbqmznmb.sHtML

[Q07] 删除表
来源：http://blog.zdbjq.cn/Article/details/gijkioctf.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.blog.zdbjq.cn/Article/details/gbushuahw.sHtML

[Q08] 创建普通索引
来源：http://baike.zdbjq.cn/Article/details/gyqmcfooj.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://baike.hesvh.cn/Article/details/gvuccnxxe.sHtML

[Q09] 创建唯一索引
来源：http://wap.fehbvm.com/Article/details/gywashiag.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://baike.hesvh.cn/Article/details/gklakypww.sHtML

[Q10] 插入单行
来源：http://wap.hesvh.cn/Article/details/gqnoajcho.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://blog.hesvh.cn/Article/details/gvhqydsst.sHtML

[Q11] 一次插入多行
来源：http://3g.fehbvm.com/Article/details/gxazbpwwj.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.share.fehbvm.com/Article/details/gpyvjyelp.sHtML

[Q12] 插入后取自增 ID
来源：http://blog.zdbjq.cn/Article/details/gvxikuruy.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://blog.zdbjq.cn/Article/details/geeosahmo.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://m.share.hesvh.cn/Article/details/gkglyrtgo.sHtML

[Q13] 忽略重复插入
来源：http://mobile.zdbjq.cn/Article/details/giianpfxf.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://wap.zdbjq.cn/Article/details/gjnifmahg.sHtML

[Q14] 存在则更新（upsert）
来源：http://wap.zdbjq.cn/Article/details/gttjufnoz.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://blog.fehbvm.com/Article/details/gfnjkejvd.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://3g.hesvh.cn/Article/details/gsqpdknqm.sHtML

[Q15] 查询全部
来源：http://wap.hesvh.cn/Article/details/ghcrxsjha.sHtML

SELECT * FROM users;
来源：http://baike.zdbjq.cn/Article/details/grrdntfau.sHtML

[Q16] 查询指定列
来源：http://www.share.zdbjq.cn/Article/details/gkmgxmyim.sHtML

SELECT id, name FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gevaueafp.sHtML

[Q17] 条件查询
来源：http://m.share.hesvh.cn/Article/details/gdyehgpll.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.m.share.fehbvm.com/Article/details/gyfltxuoi.sHtML

[Q18] 模糊匹配
来源：http://read.share.zdbjq.cn/Article/details/gkutcaqni.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://baike.hesvh.cn/Article/details/grdlccnpa.sHtML

[Q19] 范围查询
来源：http://www.blog.hesvh.cn/Article/details/gbnlvfuhx.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://baike.zdbjq.cn/Article/details/gitfubtga.sHtML

[Q20] IN 列表
来源：http://blog.zdbjq.cn/Article/details/gitamimzh.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://mobile.zdbjq.cn/Article/details/gyxlxhqnn.sHtML

[Q21] 空值判断
来源：http://www.m.share.zdbjq.cn/Article/details/gaxpiemyw.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://mobile.zdbjq.cn/Article/details/gjmmyhkdm.sHtML

[Q22] 排序
来源：http://www.share.fehbvm.com/Article/details/gkumocmqe.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://mobile.fehbvm.com/Article/details/geyikqxkx.sHtML

[Q23] 分页
来源：http://www.m.share.hesvh.cn/Article/details/gohjhkvlb.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://blog.zdbjq.cn/Article/details/gsuaeewwr.sHtML

[Q24] 去重
来源：http://read.share.hesvh.cn/Article/details/gkjjoufxt.sHtML

SELECT DISTINCT city FROM users;
来源：http://m.share.zdbjq.cn/Article/details/ghmbvhgfa.sHtML

[Q25] 只取前 N 条
来源：http://blog.zdbjq.cn/Article/details/gojndkjrz.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.share.fehbvm.com/Article/details/gcqsoezrm.sHtML

[Q26] 计数
来源：http://www.share.hesvh.cn/Article/details/grmaqqrea.sHtML

SELECT COUNT(*) FROM users;
来源：http://mobile.hesvh.cn/Article/details/gjeccbhmi.sHtML

[Q27] 条件计数
来源：http://read.share.zdbjq.cn/Article/details/gtezutzxa.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gjegfxvzw.sHtML

[Q28] 求和与平均
来源：http://mobile.zdbjq.cn/Article/details/gldjrbivz.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.share.fehbvm.com/Article/details/gqabfgrms.sHtML

[Q29] 最大最小值
来源：http://baike.fehbvm.com/Article/details/gprbjvfws.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://m.share.fehbvm.com/Article/details/gwconpipx.sHtML

[Q30] 分组统计
来源：http://www.m.share.hesvh.cn/Article/details/gqjwlaomj.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://m.share.fehbvm.com/Article/details/gfhncxbxy.sHtML

[Q31] 分组后过滤
来源：http://baike.hesvh.cn/Article/details/gommhwaoy.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://read.share.hesvh.cn/Article/details/gjbtwqfdo.sHtML

[Q32] 分组拼接字符串
来源：http://wap.hesvh.cn/Article/details/gqeeeylws.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://mobile.zdbjq.cn/Article/details/grkvivacs.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://baike.fehbvm.com/Article/details/gdpadiwrk.sHtML

[Q33] 多列分组
来源：http://blog.fehbvm.com/Article/details/gbakogvdi.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.blog.hesvh.cn/Article/details/gomfmuqyd.sHtML

[Q34] 每组取第一条
来源：http://wap.zdbjq.cn/Article/details/gdzdubfjl.sHtML

SELECT * FROM (
来源：http://blog.fehbvm.com/Article/details/gmieacvdd.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.blog.hesvh.cn/Article/details/giguifpje.sHtML

) t WHERE rn = 1;
来源：http://mobile.fehbvm.com/Article/details/gghtktijg.sHtML

[Q35] 内连接
来源：http://mobile.zdbjq.cn/Article/details/gdbsewmij.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://blog.hesvh.cn/Article/details/gwoilffln.sHtML

[Q36] 左连接
来源：http://www.m.share.fehbvm.com/Article/details/gdshfqded.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://wap.zdbjq.cn/Article/details/ghojbcosz.sHtML

[Q37] 右连接
来源：http://3g.fehbvm.com/Article/details/gisshbbsr.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://blog.zdbjq.cn/Article/details/gzjgfpzeq.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.m.share.fehbvm.com/Article/details/gpqbutsyq.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://wap.hesvh.cn/Article/details/gwapqltkh.sHtML

[Q39] 自连接（查上下级）
来源：http://www.m.share.fehbvm.com/Article/details/gzgubnrng.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.m.share.fehbvm.com/Article/details/gbyislrfi.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://baike.fehbvm.com/Article/details/goiifvcvk.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://wap.fehbvm.com/Article/details/gcodahxew.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://blog.fehbvm.com/Article/details/gdkxoffvr.sHtML

[Q41] 多表连接
来源：http://baike.hesvh.cn/Article/details/gsvzlqkre.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://m.share.zdbjq.cn/Article/details/grucyuwlm.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.m.share.zdbjq.cn/Article/details/grsprnbdn.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://m.share.hesvh.cn/Article/details/gvkfvamaj.sHtML

[Q42] 连接条件附加过滤
来源：http://www.blog.zdbjq.cn/Article/details/gbfchfbrl.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.share.hesvh.cn/Article/details/gtgtodcqj.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.m.share.zdbjq.cn/Article/details/ginyfatgc.sHtML

[Q43] 标量子查询
来源：http://www.blog.zdbjq.cn/Article/details/ghggigfdb.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.m.share.hesvh.cn/Article/details/ggbcxvqnp.sHtML

[Q44] IN 子查询
来源：http://www.m.share.zdbjq.cn/Article/details/gzidupuyc.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.blog.hesvh.cn/Article/details/guqkalgin.sHtML

[Q45] EXISTS 判断存在
来源：http://baike.hesvh.cn/Article/details/gtjlkeqrd.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.zdbjq.cn/Article/details/gxtbuxtcz.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://m.share.zdbjq.cn/Article/details/ghviifmzb.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.hesvh.cn/Article/details/gerwrrzaw.sHtML

[Q47] 与平均值比较
来源：http://www.share.fehbvm.com/Article/details/gnpiasdfo.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.m.share.hesvh.cn/Article/details/gdeaqvtuo.sHtML

[Q48] CTE 公用表表达式
来源：http://blog.zdbjq.cn/Article/details/gznmpqlfa.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.blog.hesvh.cn/Article/details/gmsuiqjcb.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://read.share.fehbvm.com/Article/details/gzvlcwpox.sHtML

[Q49] 更新单行
来源：http://read.share.hesvh.cn/Article/details/gplytyfsy.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://wap.hesvh.cn/Article/details/glkmpnxaf.sHtML

[Q50] 批量更新
来源：http://www.blog.hesvh.cn/Article/details/gfayuoxnr.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://m.share.hesvh.cn/Article/details/gvzxqhdjr.sHtML

[Q51] 用子查询更新
来源：http://wap.fehbvm.com/Article/details/gpnmuasgw.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://mobile.zdbjq.cn/Article/details/gkuuprwod.sHtML

[Q52] 删除指定行
来源：http://read.share.fehbvm.com/Article/details/gwklssxcm.sHtML

DELETE FROM users WHERE id = 10;
来源：http://3g.hesvh.cn/Article/details/gmyjkpffv.sHtML

[Q53] 按条件删除
来源：http://blog.zdbjq.cn/Article/details/glfdxdlhv.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.blog.zdbjq.cn/Article/details/geluwteyf.sHtML

[Q54] 清空表
来源：http://wap.hesvh.cn/Article/details/gznngzyce.sHtML

TRUNCATE TABLE logs;
来源：http://blog.fehbvm.com/Article/details/gkobsotuv.sHtML

[Q55] 排名（并列占位）
来源：http://blog.hesvh.cn/Article/details/gxowbumth.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.m.share.fehbvm.com/Article/details/ghntahige.sHtML

[Q56] 密集排名（并列不占位）
来源：http://baike.fehbvm.com/Article/details/gdecrgdri.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://baike.zdbjq.cn/Article/details/gwpbfbauk.sHtML

[Q57] 行号
来源：http://blog.fehbvm.com/Article/details/gvcmhaign.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gglahfnlg.sHtML

[Q58] 累计求和
来源：http://www.blog.hesvh.cn/Article/details/gtbaeiyfv.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://read.share.zdbjq.cn/Article/details/gqafrvnuq.sHtML

[Q59] 分组内累计
来源：http://www.blog.zdbjq.cn/Article/details/gqbxdyikf.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://m.share.zdbjq.cn/Article/details/gdcyessfp.sHtML

[Q60] 取上一行 / 下一行
来源：http://mobile.zdbjq.cn/Article/details/gmxkhnmuc.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.blog.hesvh.cn/Article/details/gqwrhvkyz.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.blog.zdbjq.cn/Article/details/gitnjhglu.sHtML

[Q61] 移动平均
来源：http://www.blog.zdbjq.cn/Article/details/gvjsdruiu.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.share.zdbjq.cn/Article/details/gqwzhnwaf.sHtML

[Q62] 分组占比
来源：http://baike.zdbjq.cn/Article/details/gpprkosfr.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://3g.zdbjq.cn/Article/details/gbrsrbgdf.sHtML

[Q63] 开启事务
来源：http://blog.hesvh.cn/Article/details/gvalivzbg.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://mobile.zdbjq.cn/Article/details/gcljtwjfw.sHtML

[Q64] 提交事务
来源：http://www.share.fehbvm.com/Article/details/gqvsiyhaa.sHtML

COMMIT;
来源：http://blog.zdbjq.cn/Article/details/gpddtiqql.sHtML

[Q65] 回滚事务
来源：http://baike.zdbjq.cn/Article/details/gdzvuprag.sHtML

ROLLBACK;
来源：http://www.m.share.hesvh.cn/Article/details/godogtpll.sHtML

[Q66] 行锁查询
来源：http://www.m.share.zdbjq.cn/Article/details/gijlpjgvf.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://mobile.zdbjq.cn/Article/details/gwmkksqie.sHtML

[Q67] 设置隔离级别
来源：http://read.share.zdbjq.cn/Article/details/gdgtjppyt.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://m.share.hesvh.cn/Article/details/gbyjgifyw.sHtML

[Q68] 保存点
来源：http://baike.hesvh.cn/Article/details/grombnwpl.sHtML

SAVEPOINT sp1;
来源：http://mobile.fehbvm.com/Article/details/gmaieofrt.sHtML

ROLLBACK TO sp1;
来源：http://blog.zdbjq.cn/Article/details/gasyigtbe.sHtML

[Q69] 查看执行计划
来源：http://baike.hesvh.cn/Article/details/gspdlrxoz.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://m.share.hesvh.cn/Article/details/gwxnyxcoi.sHtML

[Q70] 更新统计信息
来源：http://wap.fehbvm.com/Article/details/gvbtwxdop.sHtML

ANALYZE TABLE users;
来源：http://wap.hesvh.cn/Article/details/gtnthyacv.sHtML

[Q71] 查看建表语句
来源：http://mobile.hesvh.cn/Article/details/ghqlqmhpg.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://m.share.fehbvm.com/Article/details/gzhptvrpn.sHtML

[Q72] 查看索引
来源：http://m.share.hesvh.cn/Article/details/gcaurvyvf.sHtML

SHOW INDEX FROM users;
来源：http://blog.hesvh.cn/Article/details/gbmtqzrko.sHtML

[Q73] 查看表状态
来源：http://www.blog.fehbvm.com/Article/details/gfjywnmye.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://m.share.fehbvm.com/Article/details/gwxbzsvxo.sHtML

[Q74] 强制使用索引
来源：http://read.share.hesvh.cn/Article/details/gqukfpytn.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.share.fehbvm.com/Article/details/gjnssniiq.sHtML

[Q75] 日期格式化
来源：http://www.share.fehbvm.com/Article/details/gelqwptbg.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://baike.hesvh.cn/Article/details/glneczkpg.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://wap.hesvh.cn/Article/details/getidwrmb.sHtML

[Q76] 按天统计
来源：http://mobile.fehbvm.com/Article/details/gydkkuias.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://read.share.fehbvm.com/Article/details/gzsculyem.sHtML

[Q77] 时间加减
来源：http://www.blog.hesvh.cn/Article/details/gcqahsxew.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.blog.zdbjq.cn/Article/details/gstehjvmv.sHtML

[Q78] 当前时间
来源：http://www.share.fehbvm.com/Article/details/gvwitocdo.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://m.share.hesvh.cn/Article/details/ghxnqkdqx.sHtML

[Q79] 字符串拼接
来源：http://www.m.share.fehbvm.com/Article/details/gspjtpuvp.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.share.zdbjq.cn/Article/details/gbuoqpxfy.sHtML

[Q80] 字符串截取
来源：http://www.blog.fehbvm.com/Article/details/gonhqzoej.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gprqhvivd.sHtML

[Q81] 字符串替换
来源：http://blog.zdbjq.cn/Article/details/gunjegnyp.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://m.share.hesvh.cn/Article/details/gojlmltdj.sHtML

[Q82] 字符长度与字节长度
来源：http://3g.fehbvm.com/Article/details/gesyrjtsr.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://blog.hesvh.cn/Article/details/gweahnovj.sHtML

[Q83] 大小写转换
来源：http://mobile.zdbjq.cn/Article/details/gbynjbvsi.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gtrzpjkjv.sHtML

[Q84] 去除首尾空格
来源：http://wap.zdbjq.cn/Article/details/gfkgfttkj.sHtML

SELECT TRIM(name) FROM users;
来源：http://read.share.fehbvm.com/Article/details/gsboidjfj.sHtML

[Q85] 数值取整
来源：http://3g.fehbvm.com/Article/details/gkroczboy.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.m.share.fehbvm.com/Article/details/gjspipjhl.sHtML

[Q86] 读取 JSON 字段
来源：http://www.share.fehbvm.com/Article/details/gzizutwrk.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://wap.zdbjq.cn/Article/details/gazpdzmib.sHtML

[Q87] JSON 字段做条件
来源：http://blog.zdbjq.cn/Article/details/glzkwyaja.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.blog.zdbjq.cn/Article/details/gdzxhcwxk.sHtML

[Q88] 行转列（条件聚合）
来源：http://read.share.fehbvm.com/Article/details/gfiqdwdlk.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://wap.hesvh.cn/Article/details/gyjffjiqc.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gpiwlgofj.sHtML

[Q89] 判断表是否存在
来源：http://m.share.hesvh.cn/Article/details/glouxtvnw.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://3g.hesvh.cn/Article/details/gpinytgnh.sHtML

[Q90] 生成序号列
来源：http://m.share.hesvh.cn/Article/details/ghyhlilzq.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.share.fehbvm.com/Article/details/gggtgjzvs.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gbiujnpem.sHtML

R. Bash 专题
来源：http://www.share.zdbjq.cn/Article/details/gekjnoiew.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/ghygwiukz.sHtML

[R01] shebang 与严格模式
来源：http://read.share.hesvh.cn/Article/details/gsojwlrkq.sHtML

#!/usr/bin/env bash
来源：http://mobile.fehbvm.com/Article/details/gnqhppnzm.sHtML

set -euo pipefail
来源：http://m.share.zdbjq.cn/Article/details/giaucgiim.sHtML

[R02] 变量赋值与使用
来源：http://mobile.hesvh.cn/Article/details/grmhdlmtp.sHtML

name="Tom"; echo "$name"
来源：http://blog.zdbjq.cn/Article/details/gaxivttrj.sHtML

[R03] 只读变量
来源：http://blog.hesvh.cn/Article/details/gmmprbtir.sHtML

readonly PI=3.14
来源：http://read.share.hesvh.cn/Article/details/gglmghxfw.sHtML

[R04] 位置参数
来源：http://baike.zdbjq.cn/Article/details/gaoxnqfrl.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.share.hesvh.cn/Article/details/gquvficcv.sHtML

[R05] 参数默认值
来源：http://read.share.hesvh.cn/Article/details/gjjbagaes.sHtML

name="${1:-default}"
来源：http://read.share.fehbvm.com/Article/details/gvntzxpkv.sHtML

[R06] 判断命令是否存在
来源：http://www.blog.zdbjq.cn/Article/details/ghewyvvrb.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://wap.hesvh.cn/Article/details/glgluvkoc.sHtML

[R07] if 判断文件
来源：http://blog.hesvh.cn/Article/details/gkzoppjtl.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://blog.fehbvm.com/Article/details/gjbloczgd.sHtML

[R08] 数值比较
来源：http://read.share.zdbjq.cn/Article/details/gankhsjam.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://m.share.hesvh.cn/Article/details/gmvksyqnw.sHtML

[R09] 字符串比较
来源：http://blog.hesvh.cn/Article/details/giqlpoxgs.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.share.zdbjq.cn/Article/details/gzrbeccad.sHtML

[R10] 正则匹配
来源：http://www.share.zdbjq.cn/Article/details/gpbxyqbrq.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.share.zdbjq.cn/Article/details/gnrovqqcz.sHtML

[R11] case 多分支
来源：http://www.share.zdbjq.cn/Article/details/grhrosfru.sHtML

case "$1" in
来源：http://baike.zdbjq.cn/Article/details/gqcdjfokn.sHtML

start) echo "启动" ;;
来源：http://wap.fehbvm.com/Article/details/gpktlkwex.sHtML

stop)  echo "停止" ;;
来源：http://mobile.zdbjq.cn/Article/details/gjacegabk.sHtML

*)     echo "未知命令" ;;
来源：http://m.share.fehbvm.com/Article/details/grlukhvsw.sHtML

esac
来源：http://wap.fehbvm.com/Article/details/gjyfdzrbx.sHtML

[R12] for 遍历文件
来源：http://www.m.share.zdbjq.cn/Article/details/gdrvgtbtu.sHtML

for f in *.txt; do echo "$f"; done
来源：http://wap.zdbjq.cn/Article/details/gyptxgalv.sHtML

[R13] for 计数循环
来源：http://www.share.zdbjq.cn/Article/details/gtqacgjkz.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://blog.fehbvm.com/Article/details/gzuhyryni.sHtML

[R14] C 风格 for
来源：http://www.share.fehbvm.com/Article/details/gqbozfxvt.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://blog.hesvh.cn/Article/details/gevatsuqu.sHtML

[R15] while 逐行读文件
来源：http://m.share.zdbjq.cn/Article/details/gpellrmee.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://baike.hesvh.cn/Article/details/geuqwfufr.sHtML

[R16] until 等待条件
来源：http://www.share.fehbvm.com/Article/details/gvwzotkss.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://3g.hesvh.cn/Article/details/geufflsgx.sHtML

[R17] 数组定义与取值
来源：http://www.m.share.zdbjq.cn/Article/details/gvanwtfnz.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.share.fehbvm.com/Article/details/gtalmodko.sHtML

[R18] 遍历数组
来源：http://www.share.zdbjq.cn/Article/details/gnmgnypok.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.share.fehbvm.com/Article/details/gxqunetdy.sHtML

[R19] 数组长度
来源：http://baike.fehbvm.com/Article/details/gikzszwwj.sHtML

echo "${#arr[@]}"
来源：http://mobile.hesvh.cn/Article/details/guwjxtokx.sHtML

[R20] 关联数组（字典）
来源：http://baike.hesvh.cn/Article/details/gemluzrfh.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://baike.zdbjq.cn/Article/details/gllgiikoz.sHtML

[R21] 字符串长度
来源：http://www.blog.fehbvm.com/Article/details/gaqcqklrf.sHtML

echo "${#s}"
来源：http://m.share.zdbjq.cn/Article/details/goesinvkq.sHtML

[R22] 截取子串
来源：http://read.share.fehbvm.com/Article/details/gbbsjwcqh.sHtML

echo "${s:0:5}"
来源：http://blog.zdbjq.cn/Article/details/gyjtokiqb.sHtML

[R23] 字符串替换
来源：http://www.blog.fehbvm.com/Article/details/gwnwvtyea.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.blog.fehbvm.com/Article/details/gupxqkunp.sHtML

[R24] 大小写转换
来源：http://www.share.hesvh.cn/Article/details/gvwpexbgx.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.m.share.hesvh.cn/Article/details/gjelkhsdf.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.share.zdbjq.cn/Article/details/gkkpeyshn.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.blog.zdbjq.cn/Article/details/gcaiubldm.sHtML

[R26] 命令替换
来源：http://www.share.hesvh.cn/Article/details/gfyglllup.sHtML

now=$(date +%F); echo "$now"
来源：http://www.blog.fehbvm.com/Article/details/gwrczvsri.sHtML

[R27] 算术展开
来源：http://blog.hesvh.cn/Article/details/guzadjivq.sHtML

echo $((1 + 2 * 3))
来源：http://www.blog.zdbjq.cn/Article/details/grjnrggmh.sHtML

[R28] 浮点运算
来源：http://m.share.hesvh.cn/Article/details/gzebbioyd.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.m.share.hesvh.cn/Article/details/ggfklavps.sHtML

[R29] 定义函数
来源：http://3g.zdbjq.cn/Article/details/gqvsxvdhx.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://read.share.zdbjq.cn/Article/details/gxdbcaapv.sHtML

[R30] 函数返回状态码
来源：http://www.blog.hesvh.cn/Article/details/gdeyiaboy.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.blog.fehbvm.com/Article/details/gdevkjdtp.sHtML

[R31] 局部变量
来源：http://www.blog.zdbjq.cn/Article/details/gjsjylibp.sHtML

f() { local x=1; echo "$x"; }
来源：http://mobile.hesvh.cn/Article/details/gwsxikbrr.sHtML

[R32] 参数个数校验
来源：http://www.m.share.fehbvm.com/Article/details/gyzchmnyt.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://mobile.hesvh.cn/Article/details/gbvrwdezw.sHtML

[R33] 捕获错误并提示行号
来源：http://www.share.fehbvm.com/Article/details/ggxaggqsy.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.share.fehbvm.com/Article/details/gwsvbwrva.sHtML

[R34] 退出时清理
来源：http://baike.fehbvm.com/Article/details/guynggswn.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://mobile.zdbjq.cn/Article/details/gskfuuswh.sHtML

[R35] 后台执行并等待
来源：http://www.m.share.fehbvm.com/Article/details/gzoweuxpt.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://m.share.fehbvm.com/Article/details/gpvytpisn.sHtML

[R36] 并发执行多个任务
来源：http://wap.zdbjq.cn/Article/details/gnhimerft.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://wap.hesvh.cn/Article/details/grknqhgji.sHtML

[R37] 把输出赋给变量
来源：http://m.share.hesvh.cn/Article/details/gfrgjvwlt.sHtML

files=$(ls -1)
来源：http://blog.hesvh.cn/Article/details/gdknriutz.sHtML

[R38] 管道串联
来源：http://read.share.zdbjq.cn/Article/details/gfasimywh.sHtML

cat a.txt | grep -i error | wc -l
来源：http://wap.zdbjq.cn/Article/details/gowrznncm.sHtML

[R39] 重定向标准输出与错误
来源：http://www.blog.hesvh.cn/Article/details/gwffdhpad.sHtML

cmd > out.log 2>&1
来源：http://wap.hesvh.cn/Article/details/ghtsnbbzl.sHtML

[R40] 追加写日志
来源：http://www.m.share.zdbjq.cn/Article/details/gxkarepns.sHtML

echo "log" >> out.log
来源：http://mobile.zdbjq.cn/Article/details/gorjhfzyb.sHtML

[R41] 丢弃输出
来源：http://www.share.fehbvm.com/Article/details/gugukzgir.sHtML

cmd >/dev/null 2>&1
来源：http://www.m.share.hesvh.cn/Article/details/gqfjyhioq.sHtML

[R42] 输入重定向
来源：http://www.share.hesvh.cn/Article/details/gpcjzpezc.sHtML

wc -l < a.txt
来源：http://www.m.share.hesvh.cn/Article/details/gbxlwvbqt.sHtML

[R43] 按名字查找文件
来源：http://wap.fehbvm.com/Article/details/gojhhnuta.sHtML


<!-- 参考信息 -->