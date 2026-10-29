代发 wailian999

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://blog.hesvh.cn/Article/details/gvjcbmtih.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://mobile.zdbjq.cn/Article/details/ggwwaajfp.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://mobile.zdbjq.cn/Article/details/gnndtdcju.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://read.share.fehbvm.com/Article/details/gdrszdrdf.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.share.hesvh.cn/Article/details/giwplocbv.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://mobile.hesvh.cn/Article/details/givlruqaw.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.m.share.hesvh.cn/Article/details/gukqiidvi.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.m.share.zdbjq.cn/Article/details/gxjquprba.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gwcivssyi.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.share.zdbjq.cn/Article/details/geaeerjrb.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/giojzxdhv.sHtML

[Q01] 创建表
来源：http://baike.fehbvm.com/Article/details/gwfsfrkrl.sHtML

CREATE TABLE users (
来源：http://www.m.share.fehbvm.com/Article/details/grfaasptf.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.hesvh.cn/Article/details/gaaesvans.sHtML

name VARCHAR(50) NOT NULL,
来源：http://baike.zdbjq.cn/Article/details/gfjsaqjpn.sHtML

email VARCHAR(100) UNIQUE,
来源：http://baike.zdbjq.cn/Article/details/gwcvzphek.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://mobile.fehbvm.com/Article/details/gegqeyunn.sHtML

);
来源：http://www.m.share.hesvh.cn/Article/details/gmzeciouj.sHtML

[Q02] 创建带外键的表
来源：http://read.share.fehbvm.com/Article/details/gsycpzrnb.sHtML

CREATE TABLE orders (
来源：http://www.m.share.fehbvm.com/Article/details/gbphjfjdp.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.hesvh.cn/Article/details/gkgxtdsit.sHtML

user_id INT NOT NULL,
来源：http://www.m.share.hesvh.cn/Article/details/gvkwtdwqx.sHtML

amount DECIMAL(10, 2),
来源：http://www.share.fehbvm.com/Article/details/gmhhktche.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://wap.zdbjq.cn/Article/details/gseoeesre.sHtML

);
来源：http://blog.hesvh.cn/Article/details/gchjcwswo.sHtML

[Q03] 增加列
来源：http://baike.hesvh.cn/Article/details/givadzjzb.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://m.share.fehbvm.com/Article/details/gorfozpob.sHtML

[Q04] 修改列类型
来源：http://wap.hesvh.cn/Article/details/gmwcvzeiz.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://read.share.hesvh.cn/Article/details/grrlgufmy.sHtML

[Q05] 重命名列
来源：http://www.share.hesvh.cn/Article/details/gqvhfgpiy.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.share.hesvh.cn/Article/details/goabcxzkx.sHtML

[Q06] 删除列
来源：http://mobile.hesvh.cn/Article/details/gaoqhhxeo.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.m.share.fehbvm.com/Article/details/gnywimbuv.sHtML

[Q07] 删除表
来源：http://www.share.fehbvm.com/Article/details/gsecaopes.sHtML

DROP TABLE IF EXISTS orders;
来源：http://mobile.hesvh.cn/Article/details/gxelbwoqr.sHtML

[Q08] 创建普通索引
来源：http://baike.hesvh.cn/Article/details/gkfaeyitj.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://3g.fehbvm.com/Article/details/gzotwkxld.sHtML

[Q09] 创建唯一索引
来源：http://mobile.fehbvm.com/Article/details/gzcbogtsn.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://wap.hesvh.cn/Article/details/gyfjcpoyj.sHtML

[Q10] 插入单行
来源：http://m.share.fehbvm.com/Article/details/gmatibkzv.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://blog.hesvh.cn/Article/details/ggluvrlod.sHtML

[Q11] 一次插入多行
来源：http://m.share.fehbvm.com/Article/details/gjutkfghm.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://wap.hesvh.cn/Article/details/gcoslvkaq.sHtML

[Q12] 插入后取自增 ID
来源：http://m.share.fehbvm.com/Article/details/gdhpgvnwj.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://blog.zdbjq.cn/Article/details/gthsjgooz.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://wap.fehbvm.com/Article/details/gqcwvluha.sHtML

[Q13] 忽略重复插入
来源：http://m.share.zdbjq.cn/Article/details/grjpsaffg.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://baike.fehbvm.com/Article/details/gornvtsff.sHtML

[Q14] 存在则更新（upsert）
来源：http://mobile.zdbjq.cn/Article/details/gnzkzayzm.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://read.share.hesvh.cn/Article/details/gacexiiio.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.blog.zdbjq.cn/Article/details/gpfshauxy.sHtML

[Q15] 查询全部
来源：http://wap.zdbjq.cn/Article/details/gmamtrbef.sHtML

SELECT * FROM users;
来源：http://blog.fehbvm.com/Article/details/gsffemjpf.sHtML

[Q16] 查询指定列
来源：http://read.share.zdbjq.cn/Article/details/giwcegsni.sHtML

SELECT id, name FROM users;
来源：http://3g.fehbvm.com/Article/details/gyfretafa.sHtML

[Q17] 条件查询
来源：http://www.share.hesvh.cn/Article/details/ghfdsfhlg.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://m.share.fehbvm.com/Article/details/gjepxlrdu.sHtML

[Q18] 模糊匹配
来源：http://www.share.fehbvm.com/Article/details/gygxezimh.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://wap.hesvh.cn/Article/details/gnyntmbvz.sHtML

[Q19] 范围查询
来源：http://wap.fehbvm.com/Article/details/gfayrbqey.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://baike.zdbjq.cn/Article/details/gygzavkjl.sHtML

[Q20] IN 列表
来源：http://read.share.fehbvm.com/Article/details/gcrzaheaj.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://wap.fehbvm.com/Article/details/glsgjqigq.sHtML

[Q21] 空值判断
来源：http://www.share.hesvh.cn/Article/details/ggaqqriox.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://blog.hesvh.cn/Article/details/ggkyokbad.sHtML

[Q22] 排序
来源：http://3g.zdbjq.cn/Article/details/gzzdgpbdy.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.share.zdbjq.cn/Article/details/gzhjyewdi.sHtML

[Q23] 分页
来源：http://www.share.zdbjq.cn/Article/details/gbopjomre.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.blog.fehbvm.com/Article/details/gwalfnmuu.sHtML

[Q24] 去重
来源：http://read.share.fehbvm.com/Article/details/givcbywoi.sHtML

SELECT DISTINCT city FROM users;
来源：http://3g.fehbvm.com/Article/details/gjhrbplgl.sHtML

[Q25] 只取前 N 条
来源：http://read.share.hesvh.cn/Article/details/gppabxlez.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://wap.fehbvm.com/Article/details/grhefxufm.sHtML

[Q26] 计数
来源：http://wap.fehbvm.com/Article/details/gjwgxfazf.sHtML

SELECT COUNT(*) FROM users;
来源：http://mobile.hesvh.cn/Article/details/gsbxhagld.sHtML

[Q27] 条件计数
来源：http://read.share.zdbjq.cn/Article/details/gledhlnju.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://m.share.fehbvm.com/Article/details/gwsaeeiyo.sHtML

[Q28] 求和与平均
来源：http://blog.fehbvm.com/Article/details/gretzebwg.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://mobile.hesvh.cn/Article/details/gwzktodna.sHtML

[Q29] 最大最小值
来源：http://read.share.zdbjq.cn/Article/details/gptqoqqsn.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://blog.hesvh.cn/Article/details/gpiizybff.sHtML

[Q30] 分组统计
来源：http://www.share.zdbjq.cn/Article/details/gqlcumoag.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://wap.fehbvm.com/Article/details/gsyjmsrsv.sHtML

[Q31] 分组后过滤
来源：http://wap.zdbjq.cn/Article/details/gfpkviksb.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://mobile.fehbvm.com/Article/details/gofcmpwqz.sHtML

[Q32] 分组拼接字符串
来源：http://www.share.zdbjq.cn/Article/details/gqxkprjfl.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://m.share.hesvh.cn/Article/details/gmyhdcybr.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://m.share.hesvh.cn/Article/details/gfuwjuazc.sHtML

[Q33] 多列分组
来源：http://blog.hesvh.cn/Article/details/gilejdxpp.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.blog.zdbjq.cn/Article/details/ghbvfwsve.sHtML

[Q34] 每组取第一条
来源：http://3g.fehbvm.com/Article/details/giiaygzrm.sHtML

SELECT * FROM (
来源：http://www.m.share.hesvh.cn/Article/details/gfgdrgehx.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://3g.hesvh.cn/Article/details/gemdrkzcd.sHtML

) t WHERE rn = 1;
来源：http://www.blog.zdbjq.cn/Article/details/gdoxciwpq.sHtML

[Q35] 内连接
来源：http://www.blog.zdbjq.cn/Article/details/gkjjsjfop.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://m.share.fehbvm.com/Article/details/grqkxkxgz.sHtML

[Q36] 左连接
来源：http://baike.hesvh.cn/Article/details/gdjzrnrao.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.share.hesvh.cn/Article/details/gnsrzfeui.sHtML

[Q37] 右连接
来源：http://wap.zdbjq.cn/Article/details/gxycahqmy.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.share.fehbvm.com/Article/details/gqkupeatq.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://mobile.fehbvm.com/Article/details/ghlrmxfra.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://read.share.zdbjq.cn/Article/details/gmszooezo.sHtML

[Q39] 自连接（查上下级）
来源：http://www.share.hesvh.cn/Article/details/gxbanurlr.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://wap.hesvh.cn/Article/details/gthpthvyu.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://blog.fehbvm.com/Article/details/gatfrufgf.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://blog.zdbjq.cn/Article/details/giihyvnba.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://mobile.fehbvm.com/Article/details/gomicsjty.sHtML

[Q41] 多表连接
来源：http://www.m.share.hesvh.cn/Article/details/gvjzcofzf.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://3g.fehbvm.com/Article/details/gyucmilap.sHtML

JOIN users u ON u.id = o.user_id
来源：http://baike.fehbvm.com/Article/details/gsprouwon.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://3g.fehbvm.com/Article/details/gadnudxns.sHtML

[Q42] 连接条件附加过滤
来源：http://www.share.zdbjq.cn/Article/details/gmaombqfr.sHtML

SELECT u.name, o.amount FROM users u
来源：http://m.share.fehbvm.com/Article/details/gvaupkojo.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.share.zdbjq.cn/Article/details/gdtqubzlr.sHtML

[Q43] 标量子查询
来源：http://blog.fehbvm.com/Article/details/gdswcieco.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.m.share.zdbjq.cn/Article/details/grwblsvrz.sHtML

[Q44] IN 子查询
来源：http://wap.zdbjq.cn/Article/details/glfskyrah.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://wap.hesvh.cn/Article/details/givnkknia.sHtML

[Q45] EXISTS 判断存在
来源：http://www.m.share.hesvh.cn/Article/details/gyrbbpvzn.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.fehbvm.com/Article/details/gaitrdkgh.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://blog.hesvh.cn/Article/details/gmuxnpsdp.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.zdbjq.cn/Article/details/glnptzdgz.sHtML

[Q47] 与平均值比较
来源：http://baike.fehbvm.com/Article/details/gtmryjccv.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.blog.fehbvm.com/Article/details/guqrlbkcv.sHtML

[Q48] CTE 公用表表达式
来源：http://blog.zdbjq.cn/Article/details/glhezrtfd.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.blog.zdbjq.cn/Article/details/grqrnurro.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://read.share.zdbjq.cn/Article/details/gmnkdlrzt.sHtML

[Q49] 更新单行
来源：http://read.share.fehbvm.com/Article/details/gxwkqlwgo.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.m.share.zdbjq.cn/Article/details/glcfgmjbr.sHtML

[Q50] 批量更新
来源：http://m.share.zdbjq.cn/Article/details/gksznpgsz.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://m.share.fehbvm.com/Article/details/gnbwcjrpa.sHtML

[Q51] 用子查询更新
来源：http://mobile.hesvh.cn/Article/details/gujzlbtoq.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.blog.hesvh.cn/Article/details/gmkkcfmxb.sHtML

[Q52] 删除指定行
来源：http://www.share.fehbvm.com/Article/details/gmmuqjyhu.sHtML

DELETE FROM users WHERE id = 10;
来源：http://baike.zdbjq.cn/Article/details/gezakopdk.sHtML

[Q53] 按条件删除
来源：http://mobile.zdbjq.cn/Article/details/gatdvmukj.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.m.share.zdbjq.cn/Article/details/gtinugkmk.sHtML

[Q54] 清空表
来源：http://3g.hesvh.cn/Article/details/gsyxqvtxk.sHtML

TRUNCATE TABLE logs;
来源：http://www.blog.zdbjq.cn/Article/details/gtxhmapwn.sHtML

[Q55] 排名（并列占位）
来源：http://m.share.fehbvm.com/Article/details/gevvubiru.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://mobile.fehbvm.com/Article/details/gngzkkphg.sHtML

[Q56] 密集排名（并列不占位）
来源：http://baike.hesvh.cn/Article/details/gbizwuhrz.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.blog.fehbvm.com/Article/details/gihymmhhc.sHtML

[Q57] 行号
来源：http://www.blog.hesvh.cn/Article/details/gfpdwtrup.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://baike.zdbjq.cn/Article/details/gorowasem.sHtML

[Q58] 累计求和
来源：http://m.share.hesvh.cn/Article/details/gkkhjfnsu.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.blog.fehbvm.com/Article/details/gyrcrikgw.sHtML

[Q59] 分组内累计
来源：http://wap.hesvh.cn/Article/details/gsqoujzcc.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://baike.zdbjq.cn/Article/details/gbtrphrmr.sHtML

[Q60] 取上一行 / 下一行
来源：http://baike.hesvh.cn/Article/details/gonnwtfza.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.blog.fehbvm.com/Article/details/ghbnijtkm.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.share.hesvh.cn/Article/details/gxocesqwo.sHtML

[Q61] 移动平均
来源：http://blog.zdbjq.cn/Article/details/gbwzejjhq.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://m.share.zdbjq.cn/Article/details/gfyigkldi.sHtML

[Q62] 分组占比
来源：http://mobile.zdbjq.cn/Article/details/gghczbhlb.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://3g.fehbvm.com/Article/details/gqctcjmbt.sHtML

[Q63] 开启事务
来源：http://mobile.hesvh.cn/Article/details/gtzklncxw.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://read.share.zdbjq.cn/Article/details/ggotahzhj.sHtML

[Q64] 提交事务
来源：http://m.share.fehbvm.com/Article/details/gfqqnrosy.sHtML

COMMIT;
来源：http://www.blog.hesvh.cn/Article/details/gscnhgpdf.sHtML

[Q65] 回滚事务
来源：http://blog.fehbvm.com/Article/details/gvybqncvt.sHtML

ROLLBACK;
来源：http://blog.zdbjq.cn/Article/details/gxspfblfn.sHtML

[Q66] 行锁查询
来源：http://3g.fehbvm.com/Article/details/gsxarymwq.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.share.fehbvm.com/Article/details/gawhgmqud.sHtML

[Q67] 设置隔离级别
来源：http://www.share.zdbjq.cn/Article/details/gianbroxb.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://baike.hesvh.cn/Article/details/gqyhqanqn.sHtML

[Q68] 保存点
来源：http://read.share.zdbjq.cn/Article/details/gyguvcqsv.sHtML

SAVEPOINT sp1;
来源：http://www.m.share.fehbvm.com/Article/details/gpnhojtbu.sHtML

ROLLBACK TO sp1;
来源：http://baike.hesvh.cn/Article/details/gzcbhiumv.sHtML

[Q69] 查看执行计划
来源：http://www.share.fehbvm.com/Article/details/gvhkvyqkn.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.share.zdbjq.cn/Article/details/goltffops.sHtML

[Q70] 更新统计信息
来源：http://www.blog.zdbjq.cn/Article/details/gphieyers.sHtML

ANALYZE TABLE users;
来源：http://m.share.fehbvm.com/Article/details/gzzryaxbu.sHtML

[Q71] 查看建表语句
来源：http://read.share.zdbjq.cn/Article/details/gpyitcwna.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://read.share.fehbvm.com/Article/details/gsoqwiivd.sHtML

[Q72] 查看索引
来源：http://www.m.share.hesvh.cn/Article/details/gmbqtvqdp.sHtML

SHOW INDEX FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gfwboodxt.sHtML

[Q73] 查看表状态
来源：http://read.share.zdbjq.cn/Article/details/gjnmlmwty.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://3g.zdbjq.cn/Article/details/gqhckhfjj.sHtML

[Q74] 强制使用索引
来源：http://read.share.hesvh.cn/Article/details/gamrkafsg.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://mobile.fehbvm.com/Article/details/gnsmjhico.sHtML

[Q75] 日期格式化
来源：http://wap.hesvh.cn/Article/details/gxxfarxcy.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.blog.hesvh.cn/Article/details/gtsgjqexl.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.blog.zdbjq.cn/Article/details/gekgziupn.sHtML

[Q76] 按天统计
来源：http://read.share.zdbjq.cn/Article/details/gmqdnpqdp.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.blog.fehbvm.com/Article/details/gqbtrppiz.sHtML

[Q77] 时间加减
来源：http://www.blog.fehbvm.com/Article/details/gxwoenfzl.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://wap.hesvh.cn/Article/details/gnjvfywmo.sHtML

[Q78] 当前时间
来源：http://www.share.hesvh.cn/Article/details/gdbdpsjez.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://mobile.zdbjq.cn/Article/details/gsbqimsnr.sHtML

[Q79] 字符串拼接
来源：http://www.m.share.hesvh.cn/Article/details/gmnxvsogt.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://read.share.zdbjq.cn/Article/details/gzegvpaqh.sHtML

[Q80] 字符串截取
来源：http://www.share.hesvh.cn/Article/details/grdavbsmz.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gosvfukro.sHtML

[Q81] 字符串替换
来源：http://mobile.hesvh.cn/Article/details/gvshbrcsf.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gyvleblju.sHtML

[Q82] 字符长度与字节长度
来源：http://www.share.zdbjq.cn/Article/details/gydqxggkt.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gagrbkyst.sHtML

[Q83] 大小写转换
来源：http://mobile.hesvh.cn/Article/details/gvqwhmexs.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://m.share.fehbvm.com/Article/details/gxlrfjhqt.sHtML

[Q84] 去除首尾空格
来源：http://read.share.zdbjq.cn/Article/details/gmqzabaze.sHtML

SELECT TRIM(name) FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gegjcwkby.sHtML

[Q85] 数值取整
来源：http://baike.zdbjq.cn/Article/details/gtvcmlclr.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://m.share.fehbvm.com/Article/details/gebbkczrx.sHtML

[Q86] 读取 JSON 字段
来源：http://wap.zdbjq.cn/Article/details/gsszlstgz.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://wap.fehbvm.com/Article/details/ggdlbmicf.sHtML

[Q87] JSON 字段做条件
来源：http://blog.hesvh.cn/Article/details/gcqjllfco.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://m.share.zdbjq.cn/Article/details/gsufxojnk.sHtML

[Q88] 行转列（条件聚合）
来源：http://3g.zdbjq.cn/Article/details/gogynrhpb.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://m.share.fehbvm.com/Article/details/gcwlkorqk.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://wap.zdbjq.cn/Article/details/goipaaldg.sHtML

[Q89] 判断表是否存在
来源：http://www.blog.fehbvm.com/Article/details/grkwbwgyz.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://blog.fehbvm.com/Article/details/glcixfmbo.sHtML

[Q90] 生成序号列
来源：http://wap.hesvh.cn/Article/details/gzbqljvtp.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://read.share.zdbjq.cn/Article/details/gmtruitco.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gmlccvvxo.sHtML

R. Bash 专题
来源：http://mobile.zdbjq.cn/Article/details/gocsflbqt.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/grxzzibzu.sHtML

[R01] shebang 与严格模式
来源：http://www.blog.zdbjq.cn/Article/details/gppihruyc.sHtML

#!/usr/bin/env bash
来源：http://www.m.share.zdbjq.cn/Article/details/gzdxicwwz.sHtML

set -euo pipefail
来源：http://blog.hesvh.cn/Article/details/ghjvqcaou.sHtML

[R02] 变量赋值与使用
来源：http://www.share.hesvh.cn/Article/details/gkblfxthg.sHtML

name="Tom"; echo "$name"
来源：http://wap.zdbjq.cn/Article/details/ggsdjbgmz.sHtML

[R03] 只读变量
来源：http://www.blog.zdbjq.cn/Article/details/ghfhnnnxw.sHtML

readonly PI=3.14
来源：http://baike.hesvh.cn/Article/details/guganiheb.sHtML

[R04] 位置参数
来源：http://m.share.fehbvm.com/Article/details/ghtpjqkjy.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://baike.hesvh.cn/Article/details/gzloldrrj.sHtML

[R05] 参数默认值
来源：http://mobile.zdbjq.cn/Article/details/gpmuwzzqw.sHtML

name="${1:-default}"
来源：http://www.share.fehbvm.com/Article/details/gulgtnick.sHtML

[R06] 判断命令是否存在
来源：http://blog.fehbvm.com/Article/details/glooppyhg.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://3g.zdbjq.cn/Article/details/gxtbrukbw.sHtML

[R07] if 判断文件
来源：http://www.share.zdbjq.cn/Article/details/gzvkacdxv.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://read.share.fehbvm.com/Article/details/gixwrhnlo.sHtML

[R08] 数值比较
来源：http://blog.hesvh.cn/Article/details/gudlgslzn.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://baike.zdbjq.cn/Article/details/gwlzjtexb.sHtML

[R09] 字符串比较
来源：http://baike.zdbjq.cn/Article/details/gzgjkgbiw.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://read.share.zdbjq.cn/Article/details/ggvznsqjy.sHtML

[R10] 正则匹配
来源：http://read.share.hesvh.cn/Article/details/gguvzckao.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://3g.fehbvm.com/Article/details/gjkhnspcd.sHtML

[R11] case 多分支
来源：http://m.share.zdbjq.cn/Article/details/gynupewfp.sHtML

case "$1" in
来源：http://3g.hesvh.cn/Article/details/gkmvgsudq.sHtML

start) echo "启动" ;;
来源：http://mobile.hesvh.cn/Article/details/gpittjrmy.sHtML

stop)  echo "停止" ;;
来源：http://read.share.zdbjq.cn/Article/details/gsvoucnam.sHtML

*)     echo "未知命令" ;;
来源：http://www.m.share.hesvh.cn/Article/details/gsllcmfns.sHtML

esac
来源：http://read.share.fehbvm.com/Article/details/gbocimbdj.sHtML

[R12] for 遍历文件
来源：http://mobile.zdbjq.cn/Article/details/gbayjzcql.sHtML

for f in *.txt; do echo "$f"; done
来源：http://read.share.zdbjq.cn/Article/details/gjxkstosz.sHtML

[R13] for 计数循环
来源：http://baike.hesvh.cn/Article/details/grceolaaz.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://wap.hesvh.cn/Article/details/gfmgdivna.sHtML

[R14] C 风格 for
来源：http://mobile.hesvh.cn/Article/details/giizgurdx.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://mobile.fehbvm.com/Article/details/glektoqcs.sHtML

[R15] while 逐行读文件
来源：http://mobile.fehbvm.com/Article/details/gblucqkro.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://read.share.zdbjq.cn/Article/details/giquexxfe.sHtML

[R16] until 等待条件
来源：http://www.share.hesvh.cn/Article/details/gkblmsrrh.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://baike.hesvh.cn/Article/details/gawlzadkt.sHtML

[R17] 数组定义与取值
来源：http://3g.fehbvm.com/Article/details/girxdnoou.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.m.share.hesvh.cn/Article/details/glmgedcxa.sHtML

[R18] 遍历数组
来源：http://www.m.share.zdbjq.cn/Article/details/gwcrkymdh.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.blog.fehbvm.com/Article/details/gfadadrbz.sHtML

[R19] 数组长度
来源：http://baike.zdbjq.cn/Article/details/gcazplniq.sHtML

echo "${#arr[@]}"
来源：http://blog.hesvh.cn/Article/details/gzdghnvlq.sHtML

[R20] 关联数组（字典）
来源：http://mobile.fehbvm.com/Article/details/gylnwmfno.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.blog.zdbjq.cn/Article/details/gebmrhbmd.sHtML

[R21] 字符串长度
来源：http://3g.fehbvm.com/Article/details/grsfighzm.sHtML

echo "${#s}"
来源：http://www.m.share.zdbjq.cn/Article/details/gzpktlnuw.sHtML

[R22] 截取子串
来源：http://www.share.fehbvm.com/Article/details/gjmdtmjly.sHtML

echo "${s:0:5}"
来源：http://baike.hesvh.cn/Article/details/gtwzvooae.sHtML

[R23] 字符串替换
来源：http://3g.zdbjq.cn/Article/details/gktqcctvo.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.share.fehbvm.com/Article/details/gqlesfarc.sHtML

[R24] 大小写转换
来源：http://wap.fehbvm.com/Article/details/gkyrmbqiu.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://m.share.hesvh.cn/Article/details/gdswhvgbv.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.share.fehbvm.com/Article/details/grtapumot.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.m.share.zdbjq.cn/Article/details/gxdsfflff.sHtML

[R26] 命令替换
来源：http://wap.hesvh.cn/Article/details/gdsmbstkk.sHtML

now=$(date +%F); echo "$now"
来源：http://blog.zdbjq.cn/Article/details/gscixyqtn.sHtML

[R27] 算术展开
来源：http://m.share.hesvh.cn/Article/details/gojhphayk.sHtML

echo $((1 + 2 * 3))
来源：http://read.share.hesvh.cn/Article/details/glebuyrjk.sHtML

[R28] 浮点运算
来源：http://3g.fehbvm.com/Article/details/gfomkczbz.sHtML

echo "scale=2; 10/3" | bc
来源：http://read.share.hesvh.cn/Article/details/gpgvykrdg.sHtML

[R29] 定义函数
来源：http://m.share.hesvh.cn/Article/details/gejvwfrug.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.m.share.hesvh.cn/Article/details/gfrvwbjtx.sHtML

[R30] 函数返回状态码
来源：http://blog.fehbvm.com/Article/details/gfpczpqje.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://read.share.zdbjq.cn/Article/details/grtocbnij.sHtML

[R31] 局部变量
来源：http://www.blog.zdbjq.cn/Article/details/gkqtdauug.sHtML

f() { local x=1; echo "$x"; }
来源：http://baike.zdbjq.cn/Article/details/gxcahtkzi.sHtML

[R32] 参数个数校验
来源：http://3g.zdbjq.cn/Article/details/gkkllatzc.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://3g.hesvh.cn/Article/details/gmtfhxshv.sHtML

[R33] 捕获错误并提示行号
来源：http://read.share.zdbjq.cn/Article/details/gwdzwycuw.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://m.share.hesvh.cn/Article/details/gkzigfodq.sHtML

[R34] 退出时清理
来源：http://www.m.share.hesvh.cn/Article/details/gvpzkcjnb.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://m.share.hesvh.cn/Article/details/gwmhvxlhf.sHtML

[R35] 后台执行并等待
来源：http://3g.fehbvm.com/Article/details/gowfatxef.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://baike.zdbjq.cn/Article/details/gsjvsgyom.sHtML

[R36] 并发执行多个任务
来源：http://mobile.fehbvm.com/Article/details/gcsxetalk.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.share.hesvh.cn/Article/details/gufkeaihy.sHtML

[R37] 把输出赋给变量
来源：http://3g.zdbjq.cn/Article/details/goormyjvm.sHtML

files=$(ls -1)
来源：http://mobile.fehbvm.com/Article/details/gztiuwyqn.sHtML

[R38] 管道串联
来源：http://baike.hesvh.cn/Article/details/gofvexgpq.sHtML

cat a.txt | grep -i error | wc -l
来源：http://3g.fehbvm.com/Article/details/gusomltjq.sHtML

[R39] 重定向标准输出与错误
来源：http://baike.zdbjq.cn/Article/details/gmrnduady.sHtML


<!-- 参考信息 -->