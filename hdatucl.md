代发 wailian999

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://read.share.fehbvm.com/Article/details/gvanzrneb.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.blog.hesvh.cn/Article/details/gzapnckci.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.blog.hesvh.cn/Article/details/gbqtrjsjd.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://read.share.hesvh.cn/Article/details/gekqseyyl.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://baike.fehbvm.com/Article/details/gxrutpftm.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://read.share.zdbjq.cn/Article/details/gtfiynoht.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.blog.hesvh.cn/Article/details/givyvggat.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://m.share.fehbvm.com/Article/details/gxethxwve.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gyvwofvzn.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://mobile.zdbjq.cn/Article/details/grqcpvzyo.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gnhyptwii.sHtML

[Q01] 创建表
来源：http://wap.zdbjq.cn/Article/details/gwvlusogy.sHtML

CREATE TABLE users (
来源：http://blog.hesvh.cn/Article/details/ghoelwuwc.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.zdbjq.cn/Article/details/gfesgdxvd.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.m.share.hesvh.cn/Article/details/giqjtnvmd.sHtML

email VARCHAR(100) UNIQUE,
来源：http://3g.zdbjq.cn/Article/details/gzophhagm.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.share.hesvh.cn/Article/details/gdqmbvuhs.sHtML

);
来源：http://read.share.hesvh.cn/Article/details/gqapuenvx.sHtML

[Q02] 创建带外键的表
来源：http://3g.hesvh.cn/Article/details/gpkeanqpj.sHtML

CREATE TABLE orders (
来源：http://m.share.zdbjq.cn/Article/details/gcsfojarj.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.fehbvm.com/Article/details/gcbylqtpj.sHtML

user_id INT NOT NULL,
来源：http://baike.hesvh.cn/Article/details/gvgnmjhlz.sHtML

amount DECIMAL(10, 2),
来源：http://mobile.zdbjq.cn/Article/details/gszkmswya.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.m.share.fehbvm.com/Article/details/gomwtnuxl.sHtML

);
来源：http://baike.hesvh.cn/Article/details/gchysjmur.sHtML

[Q03] 增加列
来源：http://read.share.zdbjq.cn/Article/details/gjaaogzrf.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://wap.zdbjq.cn/Article/details/gmohclepp.sHtML

[Q04] 修改列类型
来源：http://m.share.hesvh.cn/Article/details/gxwuxmhgt.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.share.hesvh.cn/Article/details/gpazkhiap.sHtML

[Q05] 重命名列
来源：http://read.share.zdbjq.cn/Article/details/gtfgygagt.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://m.share.hesvh.cn/Article/details/gmfqmgcpj.sHtML

[Q06] 删除列
来源：http://mobile.fehbvm.com/Article/details/gzaalposo.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://read.share.fehbvm.com/Article/details/gqpluhwmk.sHtML

[Q07] 删除表
来源：http://www.blog.zdbjq.cn/Article/details/gmtgzqxfa.sHtML

DROP TABLE IF EXISTS orders;
来源：http://3g.hesvh.cn/Article/details/gunkmszst.sHtML

[Q08] 创建普通索引
来源：http://3g.zdbjq.cn/Article/details/gxiwwpsud.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://read.share.hesvh.cn/Article/details/gyqytbkhb.sHtML

[Q09] 创建唯一索引
来源：http://read.share.hesvh.cn/Article/details/gtrllgnjt.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://baike.zdbjq.cn/Article/details/grtyrptbq.sHtML

[Q10] 插入单行
来源：http://www.share.hesvh.cn/Article/details/ggbtxhbvy.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://mobile.zdbjq.cn/Article/details/gpnnguaog.sHtML

[Q11] 一次插入多行
来源：http://www.m.share.fehbvm.com/Article/details/gfqhsnflw.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://mobile.fehbvm.com/Article/details/gafavhutf.sHtML

[Q12] 插入后取自增 ID
来源：http://www.blog.zdbjq.cn/Article/details/ghpsevcyf.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.m.share.fehbvm.com/Article/details/gfdlyivjs.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://3g.fehbvm.com/Article/details/gdqpozujt.sHtML

[Q13] 忽略重复插入
来源：http://mobile.fehbvm.com/Article/details/gjoynhlik.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://baike.zdbjq.cn/Article/details/gsuetmiys.sHtML

[Q14] 存在则更新（upsert）
来源：http://baike.hesvh.cn/Article/details/gxkgjcnza.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://blog.fehbvm.com/Article/details/gghxrtuzx.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://3g.fehbvm.com/Article/details/gqrdaijoj.sHtML

[Q15] 查询全部
来源：http://www.m.share.hesvh.cn/Article/details/ghrsepzqg.sHtML

SELECT * FROM users;
来源：http://blog.fehbvm.com/Article/details/gjhfrinzl.sHtML

[Q16] 查询指定列
来源：http://baike.zdbjq.cn/Article/details/gwdnpvnxk.sHtML

SELECT id, name FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gjhmvpexo.sHtML

[Q17] 条件查询
来源：http://www.m.share.hesvh.cn/Article/details/gpzwnqfjw.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://mobile.hesvh.cn/Article/details/gtczvierx.sHtML

[Q18] 模糊匹配
来源：http://wap.hesvh.cn/Article/details/gtybdkpuf.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://mobile.hesvh.cn/Article/details/gmauuxfiv.sHtML

[Q19] 范围查询
来源：http://blog.hesvh.cn/Article/details/gnvbfoxia.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://read.share.hesvh.cn/Article/details/gjqcptlmg.sHtML

[Q20] IN 列表
来源：http://mobile.zdbjq.cn/Article/details/gtcrogxtp.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://3g.hesvh.cn/Article/details/goyzdrxml.sHtML

[Q21] 空值判断
来源：http://www.share.fehbvm.com/Article/details/geiijhnky.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.share.zdbjq.cn/Article/details/gxpueoqpv.sHtML

[Q22] 排序
来源：http://www.blog.fehbvm.com/Article/details/gygrzvaqy.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://wap.fehbvm.com/Article/details/gssyzssje.sHtML

[Q23] 分页
来源：http://www.blog.hesvh.cn/Article/details/gztxbyjkg.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.share.hesvh.cn/Article/details/gipyutihi.sHtML

[Q24] 去重
来源：http://www.blog.hesvh.cn/Article/details/gegexnbmx.sHtML

SELECT DISTINCT city FROM users;
来源：http://baike.fehbvm.com/Article/details/gvfakvayb.sHtML

[Q25] 只取前 N 条
来源：http://blog.zdbjq.cn/Article/details/ghtclagxu.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.m.share.fehbvm.com/Article/details/gmqduwspv.sHtML

[Q26] 计数
来源：http://www.share.fehbvm.com/Article/details/gldyzijfj.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/geojhdibw.sHtML

[Q27] 条件计数
来源：http://blog.zdbjq.cn/Article/details/gvehmscxp.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://wap.zdbjq.cn/Article/details/gpsfjzcpn.sHtML

[Q28] 求和与平均
来源：http://www.m.share.fehbvm.com/Article/details/gdujgjtar.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://3g.zdbjq.cn/Article/details/gwljaywzq.sHtML

[Q29] 最大最小值
来源：http://m.share.hesvh.cn/Article/details/gnpzigepu.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://read.share.fehbvm.com/Article/details/gbzoqhued.sHtML

[Q30] 分组统计
来源：http://www.share.zdbjq.cn/Article/details/gwcphfvmx.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.share.zdbjq.cn/Article/details/ghswhcwmq.sHtML

[Q31] 分组后过滤
来源：http://www.m.share.zdbjq.cn/Article/details/gqzzlprxf.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.share.fehbvm.com/Article/details/ggvqdigbu.sHtML

[Q32] 分组拼接字符串
来源：http://m.share.fehbvm.com/Article/details/gqhtsvqho.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.blog.zdbjq.cn/Article/details/gubdfjzty.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://blog.hesvh.cn/Article/details/gshkmamyv.sHtML

[Q33] 多列分组
来源：http://m.share.fehbvm.com/Article/details/gplkkhlfr.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://blog.zdbjq.cn/Article/details/gwgtghwuf.sHtML

[Q34] 每组取第一条
来源：http://read.share.hesvh.cn/Article/details/gqgmbpavt.sHtML

SELECT * FROM (
来源：http://m.share.zdbjq.cn/Article/details/gaxynarju.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://mobile.hesvh.cn/Article/details/gkswdsdkl.sHtML

) t WHERE rn = 1;
来源：http://mobile.zdbjq.cn/Article/details/gvibmynfu.sHtML

[Q35] 内连接
来源：http://www.m.share.zdbjq.cn/Article/details/gjxqfrref.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://3g.zdbjq.cn/Article/details/gieibhcqo.sHtML

[Q36] 左连接
来源：http://wap.fehbvm.com/Article/details/gorcykkkw.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://wap.hesvh.cn/Article/details/gemsykcai.sHtML

[Q37] 右连接
来源：http://baike.hesvh.cn/Article/details/ghoektwmz.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.share.hesvh.cn/Article/details/gfhcqoayg.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://mobile.fehbvm.com/Article/details/gdoarcbfy.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://blog.fehbvm.com/Article/details/gfdvwbcdr.sHtML

[Q39] 自连接（查上下级）
来源：http://baike.fehbvm.com/Article/details/ggshevgyt.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://mobile.zdbjq.cn/Article/details/gaompcbph.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://blog.fehbvm.com/Article/details/gksabqzao.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://read.share.fehbvm.com/Article/details/gxslzvizb.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.share.fehbvm.com/Article/details/gvduedzyd.sHtML

[Q41] 多表连接
来源：http://m.share.hesvh.cn/Article/details/gwdattjni.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://baike.zdbjq.cn/Article/details/glaevaeuc.sHtML

JOIN users u ON u.id = o.user_id
来源：http://blog.fehbvm.com/Article/details/gvhlarllp.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://baike.fehbvm.com/Article/details/gdfsqtxio.sHtML

[Q42] 连接条件附加过滤
来源：http://wap.fehbvm.com/Article/details/gotzurzec.sHtML

SELECT u.name, o.amount FROM users u
来源：http://mobile.hesvh.cn/Article/details/gszbbfffc.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.blog.fehbvm.com/Article/details/gkxoiiepf.sHtML

[Q43] 标量子查询
来源：http://3g.fehbvm.com/Article/details/ghardmzxa.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://3g.zdbjq.cn/Article/details/gfyuoyvfb.sHtML

[Q44] IN 子查询
来源：http://wap.zdbjq.cn/Article/details/ggndniyvb.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.share.hesvh.cn/Article/details/gkuvnufwv.sHtML

[Q45] EXISTS 判断存在
来源：http://3g.zdbjq.cn/Article/details/glkzvitgc.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.hesvh.cn/Article/details/gsgdepvrk.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.m.share.fehbvm.com/Article/details/gwdmdsoll.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.hesvh.cn/Article/details/gyeabvenb.sHtML

[Q47] 与平均值比较
来源：http://www.m.share.fehbvm.com/Article/details/glemaxpnn.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://baike.fehbvm.com/Article/details/ghthmgoey.sHtML

[Q48] CTE 公用表表达式
来源：http://baike.hesvh.cn/Article/details/giejytjdm.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://m.share.zdbjq.cn/Article/details/gxmewhvxu.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.share.hesvh.cn/Article/details/gofimsjmz.sHtML

[Q49] 更新单行
来源：http://read.share.zdbjq.cn/Article/details/gyeorutxe.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://3g.fehbvm.com/Article/details/gbnedjrlo.sHtML

[Q50] 批量更新
来源：http://blog.fehbvm.com/Article/details/gedwbsppn.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://wap.fehbvm.com/Article/details/gxovhblfp.sHtML

[Q51] 用子查询更新
来源：http://www.share.zdbjq.cn/Article/details/gxistraxo.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://wap.hesvh.cn/Article/details/gtjsydtrs.sHtML

[Q52] 删除指定行
来源：http://wap.zdbjq.cn/Article/details/gliyjdclj.sHtML

DELETE FROM users WHERE id = 10;
来源：http://blog.hesvh.cn/Article/details/gdbhwdnke.sHtML

[Q53] 按条件删除
来源：http://wap.fehbvm.com/Article/details/gqywvysnp.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://baike.hesvh.cn/Article/details/gpxxzbmrr.sHtML

[Q54] 清空表
来源：http://read.share.fehbvm.com/Article/details/gduhufshx.sHtML

TRUNCATE TABLE logs;
来源：http://baike.fehbvm.com/Article/details/gektujika.sHtML

[Q55] 排名（并列占位）
来源：http://blog.hesvh.cn/Article/details/gqnfktgwq.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://wap.hesvh.cn/Article/details/grkiasowl.sHtML

[Q56] 密集排名（并列不占位）
来源：http://wap.zdbjq.cn/Article/details/gcpsiwiha.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://mobile.zdbjq.cn/Article/details/gwewlfyio.sHtML

[Q57] 行号
来源：http://baike.fehbvm.com/Article/details/gbzpvcdpf.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://baike.zdbjq.cn/Article/details/gwzvmpuan.sHtML

[Q58] 累计求和
来源：http://mobile.zdbjq.cn/Article/details/gbwgjcqfp.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://m.share.fehbvm.com/Article/details/gxknmkpkz.sHtML

[Q59] 分组内累计
来源：http://m.share.hesvh.cn/Article/details/gyrmdftcp.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.blog.zdbjq.cn/Article/details/gkamtxkyh.sHtML

[Q60] 取上一行 / 下一行
来源：http://baike.hesvh.cn/Article/details/ghzoniila.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://blog.zdbjq.cn/Article/details/gmjwnatxa.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://read.share.fehbvm.com/Article/details/ghgddlhpk.sHtML

[Q61] 移动平均
来源：http://baike.fehbvm.com/Article/details/goypxnsqo.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://blog.zdbjq.cn/Article/details/gqakoocfb.sHtML

[Q62] 分组占比
来源：http://read.share.hesvh.cn/Article/details/geafejcyq.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.blog.fehbvm.com/Article/details/gvkoetdzd.sHtML

[Q63] 开启事务
来源：http://read.share.hesvh.cn/Article/details/gicncapno.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://mobile.zdbjq.cn/Article/details/gyoqyxrtm.sHtML

[Q64] 提交事务
来源：http://baike.hesvh.cn/Article/details/gwprdtxkx.sHtML

COMMIT;
来源：http://www.share.hesvh.cn/Article/details/gcxkpxvks.sHtML

[Q65] 回滚事务
来源：http://www.m.share.zdbjq.cn/Article/details/gjbhikshv.sHtML

ROLLBACK;
来源：http://m.share.fehbvm.com/Article/details/gydruzium.sHtML

[Q66] 行锁查询
来源：http://www.m.share.fehbvm.com/Article/details/gzfyfshco.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://m.share.hesvh.cn/Article/details/ggpdqsexw.sHtML

[Q67] 设置隔离级别
来源：http://www.share.hesvh.cn/Article/details/gorkkyzha.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://m.share.zdbjq.cn/Article/details/gxbzbiyvp.sHtML

[Q68] 保存点
来源：http://3g.zdbjq.cn/Article/details/gnlpmkhvz.sHtML

SAVEPOINT sp1;
来源：http://3g.zdbjq.cn/Article/details/geroiwsnj.sHtML

ROLLBACK TO sp1;
来源：http://3g.hesvh.cn/Article/details/girxhzwdg.sHtML

[Q69] 查看执行计划
来源：http://read.share.zdbjq.cn/Article/details/gmmnhoyif.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.share.fehbvm.com/Article/details/griemctoi.sHtML

[Q70] 更新统计信息
来源：http://3g.hesvh.cn/Article/details/grbjbqtlv.sHtML

ANALYZE TABLE users;
来源：http://read.share.hesvh.cn/Article/details/gsyeagbbn.sHtML

[Q71] 查看建表语句
来源：http://wap.fehbvm.com/Article/details/gmshhjuxi.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://blog.fehbvm.com/Article/details/gblvzmdxd.sHtML

[Q72] 查看索引
来源：http://blog.fehbvm.com/Article/details/grwkgrbpn.sHtML

SHOW INDEX FROM users;
来源：http://3g.hesvh.cn/Article/details/gvsiadxuc.sHtML

[Q73] 查看表状态
来源：http://www.m.share.zdbjq.cn/Article/details/gbnsqorkf.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://mobile.hesvh.cn/Article/details/gdiziokfl.sHtML

[Q74] 强制使用索引
来源：http://m.share.hesvh.cn/Article/details/gndmkwyot.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://wap.hesvh.cn/Article/details/gfvzdrsvq.sHtML

[Q75] 日期格式化
来源：http://blog.hesvh.cn/Article/details/gbfmktblx.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://m.share.zdbjq.cn/Article/details/gwettkgow.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://3g.zdbjq.cn/Article/details/gpxehlsds.sHtML

[Q76] 按天统计
来源：http://read.share.fehbvm.com/Article/details/gaabegbef.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.share.hesvh.cn/Article/details/gzhbgpwho.sHtML

[Q77] 时间加减
来源：http://www.m.share.hesvh.cn/Article/details/garvgeoyb.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://wap.fehbvm.com/Article/details/gfgtdrxxw.sHtML

[Q78] 当前时间
来源：http://wap.fehbvm.com/Article/details/gbpihzpso.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.blog.fehbvm.com/Article/details/goanhmyjx.sHtML

[Q79] 字符串拼接
来源：http://mobile.hesvh.cn/Article/details/gsqfmrmey.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://wap.fehbvm.com/Article/details/ghlbclrxc.sHtML

[Q80] 字符串截取
来源：http://m.share.hesvh.cn/Article/details/grhqthfee.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gqisduxoa.sHtML

[Q81] 字符串替换
来源：http://3g.hesvh.cn/Article/details/gefycjfwf.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://3g.fehbvm.com/Article/details/gtgwurxts.sHtML

[Q82] 字符长度与字节长度
来源：http://3g.hesvh.cn/Article/details/gauyfvobh.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://wap.zdbjq.cn/Article/details/gdylfefwq.sHtML

[Q83] 大小写转换
来源：http://www.share.hesvh.cn/Article/details/gxlvcfvju.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gbwheeejz.sHtML

[Q84] 去除首尾空格
来源：http://www.share.hesvh.cn/Article/details/gedlzjfhu.sHtML

SELECT TRIM(name) FROM users;
来源：http://wap.fehbvm.com/Article/details/gssqznfgv.sHtML

[Q85] 数值取整
来源：http://3g.fehbvm.com/Article/details/gvexpjhoh.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.blog.hesvh.cn/Article/details/ggktizwio.sHtML

[Q86] 读取 JSON 字段
来源：http://www.blog.zdbjq.cn/Article/details/gvphuuqng.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.blog.hesvh.cn/Article/details/gfqmavvwb.sHtML

[Q87] JSON 字段做条件
来源：http://www.blog.hesvh.cn/Article/details/guaotudmc.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://read.share.hesvh.cn/Article/details/gncievbhy.sHtML

[Q88] 行转列（条件聚合）
来源：http://read.share.hesvh.cn/Article/details/gxsdxupmc.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://blog.zdbjq.cn/Article/details/gysxejqyg.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/ggxzwziqz.sHtML

[Q89] 判断表是否存在
来源：http://m.share.fehbvm.com/Article/details/glovphvgk.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.share.zdbjq.cn/Article/details/gykshfgor.sHtML

[Q90] 生成序号列
来源：http://mobile.fehbvm.com/Article/details/grgwuxhlg.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://wap.fehbvm.com/Article/details/gzmfvjjiy.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gnaysqfgp.sHtML

R. Bash 专题
来源：http://read.share.fehbvm.com/Article/details/gjofmfzgv.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gssgcooiq.sHtML

[R01] shebang 与严格模式
来源：http://baike.zdbjq.cn/Article/details/glyootcvd.sHtML

#!/usr/bin/env bash
来源：http://www.blog.zdbjq.cn/Article/details/gzwhjtxym.sHtML

set -euo pipefail
来源：http://m.share.zdbjq.cn/Article/details/gsyzlsfhk.sHtML

[R02] 变量赋值与使用
来源：http://www.blog.fehbvm.com/Article/details/gsmzjfflb.sHtML

name="Tom"; echo "$name"
来源：http://www.m.share.hesvh.cn/Article/details/gmxfkkckh.sHtML

[R03] 只读变量
来源：http://www.share.zdbjq.cn/Article/details/gusgkypik.sHtML

readonly PI=3.14
来源：http://baike.fehbvm.com/Article/details/gbjauljvv.sHtML

[R04] 位置参数
来源：http://baike.fehbvm.com/Article/details/ggllzwzvt.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.m.share.zdbjq.cn/Article/details/geiwcohmb.sHtML

[R05] 参数默认值
来源：http://read.share.fehbvm.com/Article/details/ghzqbasdv.sHtML

name="${1:-default}"
来源：http://www.share.hesvh.cn/Article/details/gowmzgqpt.sHtML

[R06] 判断命令是否存在
来源：http://m.share.fehbvm.com/Article/details/gspuytzza.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://blog.hesvh.cn/Article/details/gtaanages.sHtML

[R07] if 判断文件
来源：http://blog.zdbjq.cn/Article/details/gtdsxvapm.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://read.share.hesvh.cn/Article/details/gppraspdh.sHtML

[R08] 数值比较
来源：http://www.share.hesvh.cn/Article/details/gdbrhjbet.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.blog.fehbvm.com/Article/details/gdotwkwzx.sHtML

[R09] 字符串比较
来源：http://www.blog.zdbjq.cn/Article/details/ghlxzufub.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://baike.fehbvm.com/Article/details/gfsqlhqmh.sHtML

[R10] 正则匹配
来源：http://3g.hesvh.cn/Article/details/gncddnwii.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://blog.fehbvm.com/Article/details/graoucjjc.sHtML

[R11] case 多分支
来源：http://read.share.fehbvm.com/Article/details/gbffmdftb.sHtML

case "$1" in
来源：http://baike.zdbjq.cn/Article/details/gtamazsdq.sHtML

start) echo "启动" ;;
来源：http://mobile.zdbjq.cn/Article/details/gzhlxivyx.sHtML

stop)  echo "停止" ;;
来源：http://m.share.fehbvm.com/Article/details/gttvbxqyq.sHtML

*)     echo "未知命令" ;;
来源：http://www.share.hesvh.cn/Article/details/gyuulreee.sHtML

esac
来源：http://mobile.zdbjq.cn/Article/details/gumpkwnel.sHtML

[R12] for 遍历文件
来源：http://www.m.share.hesvh.cn/Article/details/gopdsixsl.sHtML

for f in *.txt; do echo "$f"; done
来源：http://3g.hesvh.cn/Article/details/gkrbvqtlr.sHtML

[R13] for 计数循环
来源：http://read.share.zdbjq.cn/Article/details/grcyfdkey.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://blog.fehbvm.com/Article/details/gwnvkoyjp.sHtML

[R14] C 风格 for
来源：http://m.share.zdbjq.cn/Article/details/gvmcgfxen.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.share.fehbvm.com/Article/details/gfnczirhi.sHtML

[R15] while 逐行读文件
来源：http://www.m.share.hesvh.cn/Article/details/gkkcvsgua.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://3g.fehbvm.com/Article/details/gyghpxtyt.sHtML

[R16] until 等待条件
来源：http://baike.zdbjq.cn/Article/details/gjydhcsqv.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://baike.zdbjq.cn/Article/details/gppngrfhg.sHtML

[R17] 数组定义与取值
来源：http://read.share.fehbvm.com/Article/details/gzlxcunqw.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://3g.fehbvm.com/Article/details/gdnaxrdkc.sHtML

[R18] 遍历数组
来源：http://baike.hesvh.cn/Article/details/gsgqwcqnf.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://mobile.hesvh.cn/Article/details/gylumgxpg.sHtML

[R19] 数组长度
来源：http://m.share.hesvh.cn/Article/details/grbnayios.sHtML

echo "${#arr[@]}"
来源：http://3g.hesvh.cn/Article/details/gmbygyrni.sHtML

[R20] 关联数组（字典）
来源：http://www.share.hesvh.cn/Article/details/gvnxtqzwi.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://m.share.zdbjq.cn/Article/details/guawuxjrm.sHtML

[R21] 字符串长度
来源：http://baike.fehbvm.com/Article/details/gqkpaqtak.sHtML

echo "${#s}"
来源：http://www.m.share.fehbvm.com/Article/details/gxtcqczaf.sHtML

[R22] 截取子串
来源：http://www.m.share.fehbvm.com/Article/details/gzkevnhem.sHtML

echo "${s:0:5}"
来源：http://baike.zdbjq.cn/Article/details/gfqwfqagr.sHtML

[R23] 字符串替换
来源：http://3g.hesvh.cn/Article/details/ghrebhqna.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://m.share.zdbjq.cn/Article/details/gdrjtosts.sHtML

[R24] 大小写转换
来源：http://m.share.zdbjq.cn/Article/details/gxrkdbzhe.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.blog.fehbvm.com/Article/details/gvevkokbx.sHtML

[R25] 去后缀 / 去前缀
来源：http://3g.zdbjq.cn/Article/details/gcgefbmgw.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://blog.hesvh.cn/Article/details/gypogcgco.sHtML

[R26] 命令替换
来源：http://baike.hesvh.cn/Article/details/gixantkuk.sHtML

now=$(date +%F); echo "$now"
来源：http://wap.hesvh.cn/Article/details/gocedfsqf.sHtML

[R27] 算术展开
来源：http://wap.fehbvm.com/Article/details/gfzxhonuy.sHtML

echo $((1 + 2 * 3))
来源：http://read.share.zdbjq.cn/Article/details/gbdhyuujv.sHtML

[R28] 浮点运算
来源：http://wap.hesvh.cn/Article/details/gioaqeoby.sHtML

echo "scale=2; 10/3" | bc
来源：http://m.share.zdbjq.cn/Article/details/gdrcaobad.sHtML

[R29] 定义函数
来源：http://wap.hesvh.cn/Article/details/godzybccy.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.share.zdbjq.cn/Article/details/gofefrfeb.sHtML

[R30] 函数返回状态码
来源：http://www.m.share.hesvh.cn/Article/details/gdmjzpnrn.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://read.share.zdbjq.cn/Article/details/gjmpcmmgc.sHtML

[R31] 局部变量
来源：http://mobile.hesvh.cn/Article/details/gvsdmmxxy.sHtML

f() { local x=1; echo "$x"; }
来源：http://blog.zdbjq.cn/Article/details/gljuiyvhq.sHtML

[R32] 参数个数校验
来源：http://baike.hesvh.cn/Article/details/garuhrsfe.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://blog.hesvh.cn/Article/details/gfyrtrsbh.sHtML

[R33] 捕获错误并提示行号
来源：http://www.blog.fehbvm.com/Article/details/geeeumrhs.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://m.share.fehbvm.com/Article/details/grevvmwkl.sHtML

[R34] 退出时清理
来源：http://wap.zdbjq.cn/Article/details/gknzufihd.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.zdbjq.cn/Article/details/gafvnxhct.sHtML

[R35] 后台执行并等待
来源：http://mobile.hesvh.cn/Article/details/gpxudmzbl.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://m.share.fehbvm.com/Article/details/gqpegfozh.sHtML

[R36] 并发执行多个任务
来源：http://www.blog.fehbvm.com/Article/details/ghczzkvdi.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://blog.hesvh.cn/Article/details/ghajzabpy.sHtML

[R37] 把输出赋给变量
来源：http://mobile.hesvh.cn/Article/details/gvxrpibzu.sHtML

files=$(ls -1)
来源：http://www.m.share.hesvh.cn/Article/details/gflhknnmi.sHtML

[R38] 管道串联
来源：http://wap.zdbjq.cn/Article/details/gmqhpsahm.sHtML

cat a.txt | grep -i error | wc -l
来源：http://baike.hesvh.cn/Article/details/gweqjewkt.sHtML

[R39] 重定向标准输出与错误
来源：http://www.m.share.fehbvm.com/Article/details/gmxgtsffb.sHtML


<!-- 参考信息 -->