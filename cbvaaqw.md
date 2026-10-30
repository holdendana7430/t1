代发 wailian999

PHP:  // 手写时间戳比较
来源：http://baike.fehbvm.com/Article/details/gpljdnoei.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.fehbvm.com/Article/details/giswhmoqm.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.zdbjq.cn/Article/details/gueaoeasu.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://wap.fehbvm.com/Article/details/goeigcshe.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://blog.hesvh.cn/Article/details/gknnpwjfk.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://read.share.fehbvm.com/Article/details/gcfuqivew.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.share.hesvh.cn/Article/details/gwykgbpvh.sHtML

[P08] 处理浮点精度问题
来源：http://read.share.zdbjq.cn/Article/details/gufiqnaod.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://baike.zdbjq.cn/Article/details/gjpjpvakt.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://blog.fehbvm.com/Article/details/giwgdtbhi.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://read.share.hesvh.cn/Article/details/ghjkjoarv.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.share.fehbvm.com/Article/details/gviyfrdzv.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://wap.fehbvm.com/Article/details/gbuhpcuix.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.share.fehbvm.com/Article/details/gpdvpvhfm.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.blog.hesvh.cn/Article/details/gbhtpscks.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.m.share.fehbvm.com/Article/details/gllgnvknu.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gbxlzepos.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.blog.fehbvm.com/Article/details/gljwcrwfu.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gnjcxdufb.sHtML

[Q01] 创建表
来源：http://www.blog.fehbvm.com/Article/details/gjnwibzvw.sHtML

CREATE TABLE users (
来源：http://blog.zdbjq.cn/Article/details/ggzvjdnhn.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.fehbvm.com/Article/details/gbmeuqpcr.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.share.fehbvm.com/Article/details/gtyjojycm.sHtML

email VARCHAR(100) UNIQUE,
来源：http://m.share.hesvh.cn/Article/details/gmzrkvncp.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.share.zdbjq.cn/Article/details/ghgbnjtom.sHtML

);
来源：http://www.share.fehbvm.com/Article/details/gbhilqsbh.sHtML

[Q02] 创建带外键的表
来源：http://m.share.fehbvm.com/Article/details/gpirgmofb.sHtML

CREATE TABLE orders (
来源：http://www.share.hesvh.cn/Article/details/gsfslxlfp.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.share.zdbjq.cn/Article/details/gwqcloiqm.sHtML

user_id INT NOT NULL,
来源：http://www.blog.hesvh.cn/Article/details/gpqukscjl.sHtML

amount DECIMAL(10, 2),
来源：http://m.share.zdbjq.cn/Article/details/gyhtpooir.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://m.share.fehbvm.com/Article/details/gofwnzzlb.sHtML

);
来源：http://wap.zdbjq.cn/Article/details/ghufkwdbe.sHtML

[Q03] 增加列
来源：http://m.share.hesvh.cn/Article/details/gvhlorukj.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://mobile.hesvh.cn/Article/details/gwtfdlahv.sHtML

[Q04] 修改列类型
来源：http://3g.zdbjq.cn/Article/details/gykfvxybq.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://read.share.zdbjq.cn/Article/details/gowmcjhgr.sHtML

[Q05] 重命名列
来源：http://read.share.zdbjq.cn/Article/details/gayudaipq.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.share.fehbvm.com/Article/details/gulsziazd.sHtML

[Q06] 删除列
来源：http://www.share.zdbjq.cn/Article/details/gdlkjyyzb.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://blog.fehbvm.com/Article/details/gbtdbdzaq.sHtML

[Q07] 删除表
来源：http://www.share.fehbvm.com/Article/details/giahjawgc.sHtML

DROP TABLE IF EXISTS orders;
来源：http://m.share.hesvh.cn/Article/details/gpsgdmfup.sHtML

[Q08] 创建普通索引
来源：http://wap.fehbvm.com/Article/details/gmrqzmart.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://mobile.fehbvm.com/Article/details/grsfqkfdv.sHtML

[Q09] 创建唯一索引
来源：http://3g.fehbvm.com/Article/details/gkzyyqlzo.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.share.fehbvm.com/Article/details/geyjakpzm.sHtML

[Q10] 插入单行
来源：http://wap.hesvh.cn/Article/details/gldfakwsk.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://m.share.hesvh.cn/Article/details/gpadcuhqu.sHtML

[Q11] 一次插入多行
来源：http://mobile.hesvh.cn/Article/details/gplqucksd.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.blog.fehbvm.com/Article/details/gwqvpieki.sHtML

[Q12] 插入后取自增 ID
来源：http://mobile.fehbvm.com/Article/details/ghmajkooj.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.share.zdbjq.cn/Article/details/gryxdneeb.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.share.fehbvm.com/Article/details/gfsyumkzc.sHtML

[Q13] 忽略重复插入
来源：http://m.share.hesvh.cn/Article/details/gcwqdkprg.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://read.share.hesvh.cn/Article/details/gxdzqaazu.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.share.fehbvm.com/Article/details/gwvnnxxob.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://mobile.zdbjq.cn/Article/details/gedpyczhv.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://baike.zdbjq.cn/Article/details/ggmfsjdnc.sHtML

[Q15] 查询全部
来源：http://wap.zdbjq.cn/Article/details/gscoaqcos.sHtML

SELECT * FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gjbmcnbbq.sHtML

[Q16] 查询指定列
来源：http://read.share.zdbjq.cn/Article/details/goafnauxh.sHtML

SELECT id, name FROM users;
来源：http://baike.fehbvm.com/Article/details/ggbgxpgim.sHtML

[Q17] 条件查询
来源：http://read.share.fehbvm.com/Article/details/gqexdnmec.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.m.share.zdbjq.cn/Article/details/gkwranbvd.sHtML

[Q18] 模糊匹配
来源：http://blog.hesvh.cn/Article/details/gjpybsfjg.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://m.share.hesvh.cn/Article/details/gfctarwez.sHtML

[Q19] 范围查询
来源：http://3g.fehbvm.com/Article/details/gubusldie.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.share.hesvh.cn/Article/details/gssvsvdzy.sHtML

[Q20] IN 列表
来源：http://mobile.zdbjq.cn/Article/details/gkpjuvsbn.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://mobile.hesvh.cn/Article/details/gsqolnmnv.sHtML

[Q21] 空值判断
来源：http://3g.fehbvm.com/Article/details/gayfmlkve.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.blog.zdbjq.cn/Article/details/gfuhevbaf.sHtML

[Q22] 排序
来源：http://mobile.fehbvm.com/Article/details/gyfomqjnk.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://wap.zdbjq.cn/Article/details/gvsgkrfnu.sHtML

[Q23] 分页
来源：http://mobile.fehbvm.com/Article/details/gpfanpbhp.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://baike.hesvh.cn/Article/details/glpehiurq.sHtML

[Q24] 去重
来源：http://blog.hesvh.cn/Article/details/gfnxkgsym.sHtML

SELECT DISTINCT city FROM users;
来源：http://wap.fehbvm.com/Article/details/glnodzqbg.sHtML

[Q25] 只取前 N 条
来源：http://wap.zdbjq.cn/Article/details/ggvdoammc.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://mobile.hesvh.cn/Article/details/gvjieuduq.sHtML

[Q26] 计数
来源：http://blog.hesvh.cn/Article/details/gjoxlhnnm.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gzpgirwsa.sHtML

[Q27] 条件计数
来源：http://read.share.fehbvm.com/Article/details/gsnevlfsj.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gmorbajlm.sHtML

[Q28] 求和与平均
来源：http://blog.fehbvm.com/Article/details/goxzcpjvx.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.share.fehbvm.com/Article/details/gksymodqd.sHtML

[Q29] 最大最小值
来源：http://mobile.zdbjq.cn/Article/details/gsitkkgvy.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://blog.hesvh.cn/Article/details/gmulpujjx.sHtML

[Q30] 分组统计
来源：http://wap.fehbvm.com/Article/details/gnpequhnz.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://wap.hesvh.cn/Article/details/gagwpwfob.sHtML

[Q31] 分组后过滤
来源：http://3g.fehbvm.com/Article/details/gdhkflonl.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.blog.fehbvm.com/Article/details/gbupxeepx.sHtML

[Q32] 分组拼接字符串
来源：http://wap.zdbjq.cn/Article/details/gsqdmaobg.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.blog.fehbvm.com/Article/details/gnxeezkcm.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://m.share.fehbvm.com/Article/details/gjcxlzryx.sHtML

[Q33] 多列分组
来源：http://mobile.zdbjq.cn/Article/details/gplfqtnkh.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://read.share.zdbjq.cn/Article/details/gytdfsris.sHtML

[Q34] 每组取第一条
来源：http://mobile.hesvh.cn/Article/details/gvpczbtiv.sHtML

SELECT * FROM (
来源：http://m.share.fehbvm.com/Article/details/gredmexyt.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://mobile.fehbvm.com/Article/details/givprhbsl.sHtML

) t WHERE rn = 1;
来源：http://blog.fehbvm.com/Article/details/gpuppgxal.sHtML

[Q35] 内连接
来源：http://3g.fehbvm.com/Article/details/gqflrtbds.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://mobile.zdbjq.cn/Article/details/gtsxniqlf.sHtML

[Q36] 左连接
来源：http://www.share.fehbvm.com/Article/details/gqsgfloxh.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.share.fehbvm.com/Article/details/gkeexbwyl.sHtML

[Q37] 右连接
来源：http://www.m.share.zdbjq.cn/Article/details/gizqfbypo.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://read.share.hesvh.cn/Article/details/gfxohlpdt.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://mobile.fehbvm.com/Article/details/gwkacagvr.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.blog.fehbvm.com/Article/details/gtulhuopr.sHtML

[Q39] 自连接（查上下级）
来源：http://www.share.hesvh.cn/Article/details/gfpbuatzk.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://3g.fehbvm.com/Article/details/gpwnhjgqv.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.m.share.zdbjq.cn/Article/details/gxdcsltuc.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://m.share.fehbvm.com/Article/details/gajkvfyyk.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://blog.hesvh.cn/Article/details/glnxeenda.sHtML

[Q41] 多表连接
来源：http://www.share.fehbvm.com/Article/details/goelqhvyw.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.blog.fehbvm.com/Article/details/gyifqfpho.sHtML

JOIN users u ON u.id = o.user_id
来源：http://baike.zdbjq.cn/Article/details/gxotsfmcp.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://mobile.hesvh.cn/Article/details/gqnistqjq.sHtML

[Q42] 连接条件附加过滤
来源：http://m.share.fehbvm.com/Article/details/gynerljaf.sHtML

SELECT u.name, o.amount FROM users u
来源：http://wap.zdbjq.cn/Article/details/guqrygnjm.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.share.hesvh.cn/Article/details/gdfvhvwpl.sHtML

[Q43] 标量子查询
来源：http://blog.hesvh.cn/Article/details/gfdknsoql.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://wap.zdbjq.cn/Article/details/gmihfdrrz.sHtML

[Q44] IN 子查询
来源：http://3g.fehbvm.com/Article/details/gbfamkiax.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://blog.hesvh.cn/Article/details/gwuknmody.sHtML

[Q45] EXISTS 判断存在
来源：http://mobile.hesvh.cn/Article/details/gkknlyvej.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.zdbjq.cn/Article/details/gvwqvxlnw.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://blog.zdbjq.cn/Article/details/gyuljaasg.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.fehbvm.com/Article/details/gnnmeycag.sHtML

[Q47] 与平均值比较
来源：http://3g.zdbjq.cn/Article/details/gnomvuren.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://baike.zdbjq.cn/Article/details/gxwmyjnda.sHtML

[Q48] CTE 公用表表达式
来源：http://wap.hesvh.cn/Article/details/ghgrfumye.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.m.share.zdbjq.cn/Article/details/gtebzydyi.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://baike.fehbvm.com/Article/details/gabbigcsx.sHtML

[Q49] 更新单行
来源：http://mobile.zdbjq.cn/Article/details/gkajlktuk.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.m.share.hesvh.cn/Article/details/gawvuhxcq.sHtML

[Q50] 批量更新
来源：http://www.share.fehbvm.com/Article/details/gdfkeckbz.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.share.hesvh.cn/Article/details/gsxljbuzw.sHtML

[Q51] 用子查询更新
来源：http://www.blog.fehbvm.com/Article/details/gueegbjcq.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.blog.fehbvm.com/Article/details/guzclhjnd.sHtML

[Q52] 删除指定行
来源：http://mobile.hesvh.cn/Article/details/giztgemrr.sHtML

DELETE FROM users WHERE id = 10;
来源：http://mobile.hesvh.cn/Article/details/gntnjwliq.sHtML

[Q53] 按条件删除
来源：http://wap.fehbvm.com/Article/details/gxrdgpghx.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://baike.hesvh.cn/Article/details/gywqfbftd.sHtML

[Q54] 清空表
来源：http://3g.zdbjq.cn/Article/details/giikuweia.sHtML

TRUNCATE TABLE logs;
来源：http://read.share.fehbvm.com/Article/details/gasowajyi.sHtML

[Q55] 排名（并列占位）
来源：http://m.share.fehbvm.com/Article/details/gnayqwqhk.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.m.share.hesvh.cn/Article/details/grnkzehdc.sHtML

[Q56] 密集排名（并列不占位）
来源：http://mobile.hesvh.cn/Article/details/gqzuvlnod.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.m.share.fehbvm.com/Article/details/gssvjjgiq.sHtML

[Q57] 行号
来源：http://wap.fehbvm.com/Article/details/gpvkputtm.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://3g.zdbjq.cn/Article/details/gvvngktfz.sHtML

[Q58] 累计求和
来源：http://www.blog.zdbjq.cn/Article/details/gtrkhdapr.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://m.share.hesvh.cn/Article/details/gyexwrzcv.sHtML

[Q59] 分组内累计
来源：http://m.share.zdbjq.cn/Article/details/gzthqlhri.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://blog.zdbjq.cn/Article/details/gafbatwsp.sHtML

[Q60] 取上一行 / 下一行
来源：http://read.share.hesvh.cn/Article/details/gzvbsycpv.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://read.share.zdbjq.cn/Article/details/gtanqgvvc.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://wap.zdbjq.cn/Article/details/gyciuhjqp.sHtML

[Q61] 移动平均
来源：http://read.share.zdbjq.cn/Article/details/grzvejfce.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.blog.zdbjq.cn/Article/details/gigxgwrke.sHtML

[Q62] 分组占比
来源：http://blog.hesvh.cn/Article/details/ggnejnpiv.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://wap.zdbjq.cn/Article/details/gtnzqoxhw.sHtML

[Q63] 开启事务
来源：http://m.share.zdbjq.cn/Article/details/gkjmbdvxm.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://blog.hesvh.cn/Article/details/gxshuqzfc.sHtML

[Q64] 提交事务
来源：http://wap.zdbjq.cn/Article/details/glkdvwpjd.sHtML

COMMIT;
来源：http://baike.zdbjq.cn/Article/details/gixzftjyc.sHtML

[Q65] 回滚事务
来源：http://www.m.share.zdbjq.cn/Article/details/gurlibduv.sHtML

ROLLBACK;
来源：http://3g.fehbvm.com/Article/details/gahpiemuh.sHtML

[Q66] 行锁查询
来源：http://www.m.share.fehbvm.com/Article/details/gwwormads.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://read.share.hesvh.cn/Article/details/ggnrhpvqv.sHtML

[Q67] 设置隔离级别
来源：http://baike.hesvh.cn/Article/details/gveozrwja.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.share.hesvh.cn/Article/details/gknmyhxow.sHtML

[Q68] 保存点
来源：http://www.share.fehbvm.com/Article/details/gvhkjndvv.sHtML

SAVEPOINT sp1;
来源：http://www.m.share.fehbvm.com/Article/details/gnanoefei.sHtML

ROLLBACK TO sp1;
来源：http://mobile.zdbjq.cn/Article/details/gaqleovrf.sHtML

[Q69] 查看执行计划
来源：http://3g.zdbjq.cn/Article/details/gneldqdwq.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://read.share.zdbjq.cn/Article/details/gcphdybdx.sHtML

[Q70] 更新统计信息
来源：http://baike.zdbjq.cn/Article/details/gxqvnfmjf.sHtML

ANALYZE TABLE users;
来源：http://wap.hesvh.cn/Article/details/gqmeztmvk.sHtML

[Q71] 查看建表语句
来源：http://www.blog.hesvh.cn/Article/details/gtfmljgvc.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.blog.hesvh.cn/Article/details/grqgljhkl.sHtML

[Q72] 查看索引
来源：http://baike.fehbvm.com/Article/details/gffxrsxwn.sHtML

SHOW INDEX FROM users;
来源：http://read.share.zdbjq.cn/Article/details/ghekahxqx.sHtML

[Q73] 查看表状态
来源：http://3g.hesvh.cn/Article/details/gfuyrcycd.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.blog.fehbvm.com/Article/details/gzawcfgmm.sHtML

[Q74] 强制使用索引
来源：http://blog.hesvh.cn/Article/details/gfqodwvli.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://blog.fehbvm.com/Article/details/gciukbonw.sHtML

[Q75] 日期格式化
来源：http://baike.fehbvm.com/Article/details/gubhrmofu.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://blog.fehbvm.com/Article/details/gtegsirnh.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://3g.zdbjq.cn/Article/details/geyuawrwm.sHtML

[Q76] 按天统计
来源：http://www.share.zdbjq.cn/Article/details/gwtmhewwa.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://m.share.hesvh.cn/Article/details/gtvmrdpbs.sHtML

[Q77] 时间加减
来源：http://3g.zdbjq.cn/Article/details/gfdbueiqw.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.share.hesvh.cn/Article/details/gkznslagf.sHtML

[Q78] 当前时间
来源：http://baike.hesvh.cn/Article/details/gotnkbnfh.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.blog.hesvh.cn/Article/details/gaggaxlhz.sHtML

[Q79] 字符串拼接
来源：http://read.share.fehbvm.com/Article/details/gdkkmtjou.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.blog.hesvh.cn/Article/details/gehrtedwg.sHtML

[Q80] 字符串截取
来源：http://www.share.zdbjq.cn/Article/details/gdeidlzns.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://3g.hesvh.cn/Article/details/geyshrptq.sHtML

[Q81] 字符串替换
来源：http://baike.fehbvm.com/Article/details/gvegewpwv.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gstgbvalw.sHtML

[Q82] 字符长度与字节长度
来源：http://www.m.share.hesvh.cn/Article/details/gpzhkpxzw.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://baike.fehbvm.com/Article/details/ghccgsjvo.sHtML

[Q83] 大小写转换
来源：http://wap.fehbvm.com/Article/details/gbsknshcj.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://3g.hesvh.cn/Article/details/gnwdajzak.sHtML

[Q84] 去除首尾空格
来源：http://blog.zdbjq.cn/Article/details/gewihtrre.sHtML

SELECT TRIM(name) FROM users;
来源：http://wap.fehbvm.com/Article/details/gdbjyivet.sHtML

[Q85] 数值取整
来源：http://www.blog.fehbvm.com/Article/details/gkqsfrucl.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://mobile.zdbjq.cn/Article/details/gvvnvutfq.sHtML

[Q86] 读取 JSON 字段
来源：http://www.m.share.zdbjq.cn/Article/details/grbtffiyw.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://mobile.fehbvm.com/Article/details/gjspnfrmj.sHtML

[Q87] JSON 字段做条件
来源：http://www.share.zdbjq.cn/Article/details/gwxvikiio.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://read.share.zdbjq.cn/Article/details/gkrvaypkj.sHtML

[Q88] 行转列（条件聚合）
来源：http://blog.zdbjq.cn/Article/details/gpdwbodwq.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.blog.zdbjq.cn/Article/details/gcwtvawgy.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://wap.fehbvm.com/Article/details/ggeacjazr.sHtML

[Q89] 判断表是否存在
来源：http://mobile.hesvh.cn/Article/details/gtzsiecrk.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.blog.hesvh.cn/Article/details/gmkhrtbrj.sHtML

[Q90] 生成序号列
来源：http://www.blog.fehbvm.com/Article/details/gbxzqqdkz.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://wap.hesvh.cn/Article/details/gnoiofsll.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gwdqoeozs.sHtML

R. Bash 专题
来源：http://blog.hesvh.cn/Article/details/gqeyvftlk.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gkrfpbltc.sHtML

[R01] shebang 与严格模式
来源：http://baike.zdbjq.cn/Article/details/gxgkullpw.sHtML

#!/usr/bin/env bash
来源：http://www.m.share.fehbvm.com/Article/details/gacplznof.sHtML

set -euo pipefail
来源：http://baike.fehbvm.com/Article/details/geweomoam.sHtML

[R02] 变量赋值与使用
来源：http://read.share.fehbvm.com/Article/details/gidpyulrz.sHtML

name="Tom"; echo "$name"
来源：http://www.m.share.zdbjq.cn/Article/details/grajdhymi.sHtML

[R03] 只读变量
来源：http://mobile.zdbjq.cn/Article/details/gxegdbhsa.sHtML

readonly PI=3.14
来源：http://3g.hesvh.cn/Article/details/gbzueogow.sHtML

[R04] 位置参数
来源：http://wap.fehbvm.com/Article/details/glfnjchwh.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://read.share.hesvh.cn/Article/details/gnuotpmou.sHtML

[R05] 参数默认值
来源：http://www.m.share.zdbjq.cn/Article/details/grxwcchqb.sHtML

name="${1:-default}"
来源：http://wap.zdbjq.cn/Article/details/gitalhosr.sHtML

[R06] 判断命令是否存在
来源：http://baike.zdbjq.cn/Article/details/gavkieakx.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://blog.fehbvm.com/Article/details/gjlsvsxif.sHtML

[R07] if 判断文件
来源：http://wap.zdbjq.cn/Article/details/grboinpvn.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://blog.fehbvm.com/Article/details/gtcgohwov.sHtML

[R08] 数值比较
来源：http://read.share.hesvh.cn/Article/details/gclvjfrwn.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://mobile.hesvh.cn/Article/details/gbwqzayki.sHtML

[R09] 字符串比较
来源：http://www.m.share.hesvh.cn/Article/details/glhukjrgd.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://wap.zdbjq.cn/Article/details/gvkqhrbih.sHtML

[R10] 正则匹配
来源：http://www.blog.fehbvm.com/Article/details/gfzzcjbod.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.blog.hesvh.cn/Article/details/golhcfayg.sHtML

[R11] case 多分支
来源：http://www.m.share.zdbjq.cn/Article/details/gkuofdvtw.sHtML

case "$1" in
来源：http://read.share.hesvh.cn/Article/details/gngzoodgq.sHtML

start) echo "启动" ;;
来源：http://www.blog.hesvh.cn/Article/details/gepcwmvip.sHtML

stop)  echo "停止" ;;
来源：http://wap.zdbjq.cn/Article/details/gziuzaale.sHtML

*)     echo "未知命令" ;;
来源：http://wap.fehbvm.com/Article/details/gbjitjcwl.sHtML

esac
来源：http://wap.zdbjq.cn/Article/details/gueuuwxig.sHtML

[R12] for 遍历文件
来源：http://mobile.zdbjq.cn/Article/details/gayvcwooh.sHtML

for f in *.txt; do echo "$f"; done
来源：http://baike.hesvh.cn/Article/details/gbhqxqjpm.sHtML

[R13] for 计数循环
来源：http://mobile.fehbvm.com/Article/details/gdefuvtkn.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://wap.fehbvm.com/Article/details/gwinfavtq.sHtML

[R14] C 风格 for
来源：http://3g.zdbjq.cn/Article/details/gaesdfpql.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://baike.fehbvm.com/Article/details/gbnqfuvft.sHtML

[R15] while 逐行读文件
来源：http://www.share.zdbjq.cn/Article/details/gpokusddd.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://mobile.zdbjq.cn/Article/details/glpthctdw.sHtML

[R16] until 等待条件
来源：http://www.share.fehbvm.com/Article/details/gnsihbvuv.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.blog.hesvh.cn/Article/details/gcuhazdyq.sHtML

[R17] 数组定义与取值
来源：http://www.share.hesvh.cn/Article/details/glhpamgnf.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://3g.zdbjq.cn/Article/details/gofusplit.sHtML

[R18] 遍历数组
来源：http://wap.zdbjq.cn/Article/details/gabcnxfhu.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://mobile.zdbjq.cn/Article/details/gvgwflvjc.sHtML

[R19] 数组长度
来源：http://www.blog.fehbvm.com/Article/details/gkbvgybtd.sHtML

echo "${#arr[@]}"
来源：http://mobile.hesvh.cn/Article/details/geidyybvu.sHtML

[R20] 关联数组（字典）
来源：http://www.share.hesvh.cn/Article/details/gocyxgspa.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://3g.fehbvm.com/Article/details/gjkrihtcx.sHtML

[R21] 字符串长度
来源：http://www.share.zdbjq.cn/Article/details/gqeolnutq.sHtML

echo "${#s}"
来源：http://www.blog.hesvh.cn/Article/details/gqatkohgr.sHtML

[R22] 截取子串
来源：http://www.blog.zdbjq.cn/Article/details/gfcklshnw.sHtML

echo "${s:0:5}"
来源：http://www.blog.zdbjq.cn/Article/details/geyqgnvws.sHtML

[R23] 字符串替换
来源：http://wap.zdbjq.cn/Article/details/gfcjrrbye.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://m.share.fehbvm.com/Article/details/gjdrdwohy.sHtML

[R24] 大小写转换
来源：http://wap.fehbvm.com/Article/details/gkbldgslf.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://read.share.fehbvm.com/Article/details/gazdkcwqq.sHtML

[R25] 去后缀 / 去前缀
来源：http://3g.hesvh.cn/Article/details/gfbvdzkxw.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://read.share.hesvh.cn/Article/details/gcolvimpe.sHtML

[R26] 命令替换
来源：http://baike.fehbvm.com/Article/details/gpzanylyv.sHtML

now=$(date +%F); echo "$now"
来源：http://mobile.fehbvm.com/Article/details/gjhmdarkw.sHtML

[R27] 算术展开
来源：http://www.blog.zdbjq.cn/Article/details/gophpoxag.sHtML

echo $((1 + 2 * 3))
来源：http://3g.fehbvm.com/Article/details/gdfqfwieg.sHtML

[R28] 浮点运算
来源：http://wap.hesvh.cn/Article/details/gwzjpucvr.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.blog.zdbjq.cn/Article/details/gbjvukdaw.sHtML

[R29] 定义函数
来源：http://wap.fehbvm.com/Article/details/gbaqvoojy.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://blog.zdbjq.cn/Article/details/gsuutnqzi.sHtML

[R30] 函数返回状态码
来源：http://baike.fehbvm.com/Article/details/glqbqmjcm.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://m.share.zdbjq.cn/Article/details/gezoahsew.sHtML

[R31] 局部变量
来源：http://wap.fehbvm.com/Article/details/gqzosmrow.sHtML

f() { local x=1; echo "$x"; }
来源：http://3g.hesvh.cn/Article/details/gbddqfprm.sHtML

[R32] 参数个数校验
来源：http://wap.hesvh.cn/Article/details/gskhvdkre.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://read.share.hesvh.cn/Article/details/gsdqovinq.sHtML

[R33] 捕获错误并提示行号
来源：http://baike.zdbjq.cn/Article/details/gzqoxsoic.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.m.share.fehbvm.com/Article/details/gwcdceuyu.sHtML

[R34] 退出时清理
来源：http://3g.fehbvm.com/Article/details/gbdvtednk.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.share.fehbvm.com/Article/details/gzdskgolv.sHtML

[R35] 后台执行并等待
来源：http://www.blog.hesvh.cn/Article/details/gciztcmjo.sHtML


<!-- 参考信息 -->