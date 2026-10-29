代发 wailian999

PHP:  // 手写时间戳比较
来源：http://baike.fehbvm.com/Article/details/gbryywpxv.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.fehbvm.com/Article/details/glmaqxycg.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.zdbjq.cn/Article/details/gztydymjv.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://m.share.hesvh.cn/Article/details/ghqijlkbl.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.m.share.hesvh.cn/Article/details/gnzgmhozj.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://wap.zdbjq.cn/Article/details/gdsrxqabn.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://mobile.hesvh.cn/Article/details/ggtxjeyca.sHtML

[P08] 处理浮点精度问题
来源：http://blog.fehbvm.com/Article/details/ghrmanqtl.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.m.share.hesvh.cn/Article/details/glsqngvpr.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.m.share.fehbvm.com/Article/details/gsxkfajzl.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.share.zdbjq.cn/Article/details/gpuvlsppg.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://blog.fehbvm.com/Article/details/gwettslyb.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://read.share.zdbjq.cn/Article/details/gvsljwxal.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.share.zdbjq.cn/Article/details/gyvoqgqzp.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.m.share.hesvh.cn/Article/details/gyazmfmfb.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://wap.fehbvm.com/Article/details/gkshfykhd.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/ghfcubhdl.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://m.share.hesvh.cn/Article/details/gpquglini.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gtewqbgwr.sHtML

[Q01] 创建表
来源：http://m.share.fehbvm.com/Article/details/glovndfcj.sHtML

CREATE TABLE users (
来源：http://3g.hesvh.cn/Article/details/gjobpuzlm.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.hesvh.cn/Article/details/ghbwrpnyq.sHtML

name VARCHAR(50) NOT NULL,
来源：http://wap.hesvh.cn/Article/details/ghmxztcab.sHtML

email VARCHAR(100) UNIQUE,
来源：http://read.share.fehbvm.com/Article/details/gvgdawmfb.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://wap.hesvh.cn/Article/details/goktwikxb.sHtML

);
来源：http://mobile.hesvh.cn/Article/details/gnghinxxb.sHtML

[Q02] 创建带外键的表
来源：http://wap.zdbjq.cn/Article/details/gjcusutbv.sHtML

CREATE TABLE orders (
来源：http://wap.hesvh.cn/Article/details/gcknaejyl.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://mobile.hesvh.cn/Article/details/gzkafsmyv.sHtML

user_id INT NOT NULL,
来源：http://www.share.hesvh.cn/Article/details/gmhdfpqvc.sHtML

amount DECIMAL(10, 2),
来源：http://3g.fehbvm.com/Article/details/gqdsrecpt.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://3g.hesvh.cn/Article/details/gafxvmirq.sHtML

);
来源：http://www.blog.fehbvm.com/Article/details/gbzyardvr.sHtML

[Q03] 增加列
来源：http://www.share.hesvh.cn/Article/details/gaaisafpm.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.blog.zdbjq.cn/Article/details/grxhzizyb.sHtML

[Q04] 修改列类型
来源：http://blog.fehbvm.com/Article/details/grhdfufed.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.m.share.zdbjq.cn/Article/details/gkjzeilei.sHtML

[Q05] 重命名列
来源：http://3g.hesvh.cn/Article/details/gdqlrvbyo.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://3g.fehbvm.com/Article/details/gdgivipmf.sHtML

[Q06] 删除列
来源：http://wap.zdbjq.cn/Article/details/gjjirgdvc.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://blog.hesvh.cn/Article/details/ggthfaubw.sHtML

[Q07] 删除表
来源：http://wap.hesvh.cn/Article/details/gmmooqltt.sHtML

DROP TABLE IF EXISTS orders;
来源：http://wap.hesvh.cn/Article/details/gcezybogi.sHtML

[Q08] 创建普通索引
来源：http://www.m.share.fehbvm.com/Article/details/gbzsjrwuy.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.m.share.hesvh.cn/Article/details/gxjnylctk.sHtML

[Q09] 创建唯一索引
来源：http://read.share.hesvh.cn/Article/details/gdykibuqe.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://mobile.zdbjq.cn/Article/details/gzjlwxuon.sHtML

[Q10] 插入单行
来源：http://www.m.share.fehbvm.com/Article/details/gqfqqfldr.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.share.hesvh.cn/Article/details/gpmbltety.sHtML

[Q11] 一次插入多行
来源：http://3g.fehbvm.com/Article/details/gelophsxc.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://3g.fehbvm.com/Article/details/gnwjdnkww.sHtML

[Q12] 插入后取自增 ID
来源：http://www.m.share.fehbvm.com/Article/details/gxqxognmp.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://baike.zdbjq.cn/Article/details/gsbujtpqx.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.share.fehbvm.com/Article/details/gtnhgdjla.sHtML

[Q13] 忽略重复插入
来源：http://www.blog.fehbvm.com/Article/details/glywhprbg.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://m.share.zdbjq.cn/Article/details/geyznlaal.sHtML

[Q14] 存在则更新（upsert）
来源：http://mobile.zdbjq.cn/Article/details/glcqsdjbp.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://mobile.hesvh.cn/Article/details/gsrdzvgwk.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://blog.zdbjq.cn/Article/details/gyxswwowr.sHtML

[Q15] 查询全部
来源：http://blog.hesvh.cn/Article/details/gbyxrnfhj.sHtML

SELECT * FROM users;
来源：http://3g.fehbvm.com/Article/details/gcsqwdjeo.sHtML

[Q16] 查询指定列
来源：http://m.share.zdbjq.cn/Article/details/gcfmxsfhr.sHtML

SELECT id, name FROM users;
来源：http://mobile.fehbvm.com/Article/details/gjhfdcfrh.sHtML

[Q17] 条件查询
来源：http://www.blog.zdbjq.cn/Article/details/gdvitqriq.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.blog.fehbvm.com/Article/details/gozpsatbh.sHtML

[Q18] 模糊匹配
来源：http://blog.fehbvm.com/Article/details/gecuihvbv.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://wap.zdbjq.cn/Article/details/gcedgjshw.sHtML

[Q19] 范围查询
来源：http://read.share.fehbvm.com/Article/details/gdxzupkvx.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://m.share.hesvh.cn/Article/details/gvevdatbu.sHtML

[Q20] IN 列表
来源：http://baike.hesvh.cn/Article/details/gipfkvfrx.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://3g.hesvh.cn/Article/details/gkgrsihbv.sHtML

[Q21] 空值判断
来源：http://www.share.zdbjq.cn/Article/details/gwtbjuawf.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://wap.hesvh.cn/Article/details/gifjuetdd.sHtML

[Q22] 排序
来源：http://wap.hesvh.cn/Article/details/gfhkxoxid.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://blog.fehbvm.com/Article/details/gjegvwvwl.sHtML

[Q23] 分页
来源：http://3g.zdbjq.cn/Article/details/gnixyayni.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://3g.zdbjq.cn/Article/details/gahfdejkg.sHtML

[Q24] 去重
来源：http://m.share.fehbvm.com/Article/details/glluxzcck.sHtML

SELECT DISTINCT city FROM users;
来源：http://baike.fehbvm.com/Article/details/gynycnorj.sHtML

[Q25] 只取前 N 条
来源：http://www.blog.fehbvm.com/Article/details/gkllvfjad.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://baike.fehbvm.com/Article/details/gddacvlhq.sHtML

[Q26] 计数
来源：http://baike.fehbvm.com/Article/details/gfuwzijfk.sHtML

SELECT COUNT(*) FROM users;
来源：http://wap.fehbvm.com/Article/details/goosnuqgb.sHtML

[Q27] 条件计数
来源：http://mobile.fehbvm.com/Article/details/gieemffwa.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gbltqgqzs.sHtML

[Q28] 求和与平均
来源：http://www.m.share.hesvh.cn/Article/details/gdpjflerf.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://m.share.hesvh.cn/Article/details/goieyxjyn.sHtML

[Q29] 最大最小值
来源：http://www.blog.fehbvm.com/Article/details/gntjrewjy.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://wap.zdbjq.cn/Article/details/gxvoxkrpf.sHtML

[Q30] 分组统计
来源：http://blog.zdbjq.cn/Article/details/gbzqzdkxo.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://m.share.hesvh.cn/Article/details/gajavxoqh.sHtML

[Q31] 分组后过滤
来源：http://blog.hesvh.cn/Article/details/gjvoogtns.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://mobile.fehbvm.com/Article/details/gxztxavsv.sHtML

[Q32] 分组拼接字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gzfzlzgqz.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://3g.fehbvm.com/Article/details/gmubiqjky.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://3g.hesvh.cn/Article/details/gwsyhkdvd.sHtML

[Q33] 多列分组
来源：http://blog.fehbvm.com/Article/details/gzzypclfh.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://read.share.fehbvm.com/Article/details/gbdccscss.sHtML

[Q34] 每组取第一条
来源：http://baike.fehbvm.com/Article/details/gwrrlempv.sHtML

SELECT * FROM (
来源：http://blog.fehbvm.com/Article/details/glbfkqcpc.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://baike.zdbjq.cn/Article/details/gzaoribky.sHtML

) t WHERE rn = 1;
来源：http://m.share.zdbjq.cn/Article/details/gcsnokgau.sHtML

[Q35] 内连接
来源：http://baike.fehbvm.com/Article/details/gyihwmdoy.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.fehbvm.com/Article/details/goboogzoc.sHtML

[Q36] 左连接
来源：http://www.m.share.hesvh.cn/Article/details/germbdswk.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://3g.hesvh.cn/Article/details/gomymgebt.sHtML

[Q37] 右连接
来源：http://3g.hesvh.cn/Article/details/guwfcfwau.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://baike.hesvh.cn/Article/details/gddcgfend.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://wap.fehbvm.com/Article/details/gxqtqolks.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://blog.fehbvm.com/Article/details/ggkvastib.sHtML

[Q39] 自连接（查上下级）
来源：http://baike.zdbjq.cn/Article/details/gydebwsek.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://read.share.hesvh.cn/Article/details/gmhudwcvq.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://read.share.zdbjq.cn/Article/details/guvsbukgd.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://m.share.hesvh.cn/Article/details/gdyulnrvi.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://wap.fehbvm.com/Article/details/guwdovikc.sHtML

[Q41] 多表连接
来源：http://3g.fehbvm.com/Article/details/gbwbckmnw.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.m.share.zdbjq.cn/Article/details/goqiqjhbq.sHtML

JOIN users u ON u.id = o.user_id
来源：http://read.share.zdbjq.cn/Article/details/gocpyborg.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://read.share.zdbjq.cn/Article/details/ggloytigm.sHtML

[Q42] 连接条件附加过滤
来源：http://www.share.hesvh.cn/Article/details/gtvlylnwt.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.m.share.zdbjq.cn/Article/details/gqeqdpkpj.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://mobile.hesvh.cn/Article/details/gelegacnm.sHtML

[Q43] 标量子查询
来源：http://blog.fehbvm.com/Article/details/gflkimikk.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://m.share.fehbvm.com/Article/details/gryzxgfyi.sHtML

[Q44] IN 子查询
来源：http://3g.fehbvm.com/Article/details/gvhwnihyr.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://mobile.fehbvm.com/Article/details/gczfldywc.sHtML

[Q45] EXISTS 判断存在
来源：http://baike.zdbjq.cn/Article/details/gpclqofjj.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.hesvh.cn/Article/details/gbumprvjw.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://baike.fehbvm.com/Article/details/grfptftqw.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.zdbjq.cn/Article/details/gferczukv.sHtML

[Q47] 与平均值比较
来源：http://wap.fehbvm.com/Article/details/gbiiuavws.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://mobile.hesvh.cn/Article/details/ginjvbpdy.sHtML

[Q48] CTE 公用表表达式
来源：http://www.m.share.fehbvm.com/Article/details/gnwoxiswg.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://read.share.hesvh.cn/Article/details/gfuryujiy.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://blog.fehbvm.com/Article/details/gksjizgnz.sHtML

[Q49] 更新单行
来源：http://m.share.hesvh.cn/Article/details/gaskktnld.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://mobile.fehbvm.com/Article/details/gjsdwzfqf.sHtML

[Q50] 批量更新
来源：http://www.share.zdbjq.cn/Article/details/gxnssibuy.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://3g.hesvh.cn/Article/details/grzaaboni.sHtML

[Q51] 用子查询更新
来源：http://read.share.fehbvm.com/Article/details/gjutbygnv.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://wap.fehbvm.com/Article/details/gfvrcmvnx.sHtML

[Q52] 删除指定行
来源：http://www.m.share.fehbvm.com/Article/details/gnyinxnxe.sHtML

DELETE FROM users WHERE id = 10;
来源：http://3g.fehbvm.com/Article/details/gdirqhdrn.sHtML

[Q53] 按条件删除
来源：http://baike.fehbvm.com/Article/details/gyzkqosfq.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.m.share.zdbjq.cn/Article/details/gmrywsoxq.sHtML

[Q54] 清空表
来源：http://m.share.fehbvm.com/Article/details/gmkiyfwrc.sHtML

TRUNCATE TABLE logs;
来源：http://m.share.zdbjq.cn/Article/details/gysnizvzz.sHtML

[Q55] 排名（并列占位）
来源：http://mobile.zdbjq.cn/Article/details/gsgnxhqxa.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.share.zdbjq.cn/Article/details/gczfpzwnb.sHtML

[Q56] 密集排名（并列不占位）
来源：http://baike.fehbvm.com/Article/details/gidztmcyt.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://wap.hesvh.cn/Article/details/gocniulzn.sHtML

[Q57] 行号
来源：http://blog.fehbvm.com/Article/details/ggtliedbf.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://blog.zdbjq.cn/Article/details/gtimvxhbn.sHtML

[Q58] 累计求和
来源：http://blog.fehbvm.com/Article/details/gwoxdiebv.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.share.hesvh.cn/Article/details/grsxygclq.sHtML

[Q59] 分组内累计
来源：http://mobile.hesvh.cn/Article/details/grrmrylwr.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://mobile.fehbvm.com/Article/details/gbyusnkut.sHtML

[Q60] 取上一行 / 下一行
来源：http://m.share.fehbvm.com/Article/details/gpidejmii.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://baike.fehbvm.com/Article/details/gmbvccjbp.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://wap.hesvh.cn/Article/details/grvyttucz.sHtML

[Q61] 移动平均
来源：http://wap.hesvh.cn/Article/details/gndwbnmtk.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://blog.fehbvm.com/Article/details/gbumamaso.sHtML

[Q62] 分组占比
来源：http://blog.fehbvm.com/Article/details/gpstegapx.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://read.share.fehbvm.com/Article/details/gybwfiwcy.sHtML

[Q63] 开启事务
来源：http://www.blog.zdbjq.cn/Article/details/ghjcsiwpo.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://m.share.zdbjq.cn/Article/details/gudtujcno.sHtML

[Q64] 提交事务
来源：http://www.blog.hesvh.cn/Article/details/gazentsnl.sHtML

COMMIT;
来源：http://read.share.hesvh.cn/Article/details/gazvfpanb.sHtML

[Q65] 回滚事务
来源：http://wap.zdbjq.cn/Article/details/gvhusqcmd.sHtML

ROLLBACK;
来源：http://www.share.hesvh.cn/Article/details/gehczmxlb.sHtML

[Q66] 行锁查询
来源：http://baike.zdbjq.cn/Article/details/gmcquivaq.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.share.zdbjq.cn/Article/details/gankudfjc.sHtML

[Q67] 设置隔离级别
来源：http://mobile.hesvh.cn/Article/details/glofthflg.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://mobile.zdbjq.cn/Article/details/gthycmykp.sHtML

[Q68] 保存点
来源：http://3g.fehbvm.com/Article/details/gijpmlutt.sHtML

SAVEPOINT sp1;
来源：http://baike.hesvh.cn/Article/details/gfpeetwpo.sHtML

ROLLBACK TO sp1;
来源：http://baike.hesvh.cn/Article/details/gcqedtces.sHtML

[Q69] 查看执行计划
来源：http://www.m.share.zdbjq.cn/Article/details/gssrkhvfn.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://mobile.zdbjq.cn/Article/details/gfcihsoje.sHtML

[Q70] 更新统计信息
来源：http://baike.fehbvm.com/Article/details/gsbkliaib.sHtML

ANALYZE TABLE users;
来源：http://read.share.zdbjq.cn/Article/details/gsnqwrvzk.sHtML

[Q71] 查看建表语句
来源：http://wap.fehbvm.com/Article/details/gsflcxicl.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://m.share.fehbvm.com/Article/details/gtckaoogb.sHtML

[Q72] 查看索引
来源：http://www.blog.fehbvm.com/Article/details/gumvwsfoh.sHtML

SHOW INDEX FROM users;
来源：http://www.share.hesvh.cn/Article/details/gumvfehxn.sHtML

[Q73] 查看表状态
来源：http://read.share.zdbjq.cn/Article/details/gcuutxsnv.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.blog.fehbvm.com/Article/details/gkwidcsgs.sHtML

[Q74] 强制使用索引
来源：http://read.share.fehbvm.com/Article/details/gyyydozqy.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://read.share.zdbjq.cn/Article/details/glzxygbjs.sHtML

[Q75] 日期格式化
来源：http://www.blog.zdbjq.cn/Article/details/gclexgezq.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://3g.zdbjq.cn/Article/details/gnpjkrtxr.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://m.share.zdbjq.cn/Article/details/gvtstzjgx.sHtML

[Q76] 按天统计
来源：http://blog.fehbvm.com/Article/details/glrpukddd.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://wap.fehbvm.com/Article/details/gzrrvpnby.sHtML

[Q77] 时间加减
来源：http://www.share.hesvh.cn/Article/details/gayeydboj.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://m.share.zdbjq.cn/Article/details/gytjwrohq.sHtML

[Q78] 当前时间
来源：http://www.blog.zdbjq.cn/Article/details/gfmlwojuy.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://wap.zdbjq.cn/Article/details/gkmthgnfu.sHtML

[Q79] 字符串拼接
来源：http://www.m.share.fehbvm.com/Article/details/gckbgzkxl.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.blog.zdbjq.cn/Article/details/gnnyafavz.sHtML

[Q80] 字符串截取
来源：http://www.share.fehbvm.com/Article/details/gxgaopcad.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/giirgwywx.sHtML

[Q81] 字符串替换
来源：http://www.m.share.zdbjq.cn/Article/details/gakbmrzds.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gocmsbcbr.sHtML

[Q82] 字符长度与字节长度
来源：http://www.share.zdbjq.cn/Article/details/gumcykjnp.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://blog.fehbvm.com/Article/details/gvekylfwt.sHtML

[Q83] 大小写转换
来源：http://baike.hesvh.cn/Article/details/gpwcsvkoz.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gpifwsttb.sHtML

[Q84] 去除首尾空格
来源：http://www.share.hesvh.cn/Article/details/guawekvsy.sHtML

SELECT TRIM(name) FROM users;
来源：http://baike.fehbvm.com/Article/details/gzmhpucsn.sHtML

[Q85] 数值取整
来源：http://www.blog.hesvh.cn/Article/details/glxraczpf.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://3g.zdbjq.cn/Article/details/gizefmwfp.sHtML

[Q86] 读取 JSON 字段
来源：http://baike.fehbvm.com/Article/details/gjjiqhawu.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://baike.hesvh.cn/Article/details/gaatbfadt.sHtML

[Q87] JSON 字段做条件
来源：http://www.m.share.zdbjq.cn/Article/details/gbnxbikvr.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://blog.hesvh.cn/Article/details/gctzvyffx.sHtML

[Q88] 行转列（条件聚合）
来源：http://blog.fehbvm.com/Article/details/gtrfmnghb.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://blog.zdbjq.cn/Article/details/gpizsfrhz.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://m.share.fehbvm.com/Article/details/gpyasnfna.sHtML

[Q89] 判断表是否存在
来源：http://3g.zdbjq.cn/Article/details/gzidtwgef.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://baike.hesvh.cn/Article/details/ggfyeahgq.sHtML

[Q90] 生成序号列
来源：http://wap.zdbjq.cn/Article/details/gbrhuxqlr.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://baike.fehbvm.com/Article/details/gnwlyawid.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gfyunpcqr.sHtML

R. Bash 专题
来源：http://www.share.fehbvm.com/Article/details/gsannokij.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gyukwqmpt.sHtML

[R01] shebang 与严格模式
来源：http://www.blog.fehbvm.com/Article/details/gcpgjgpgp.sHtML

#!/usr/bin/env bash
来源：http://www.blog.hesvh.cn/Article/details/gwtwbsjsr.sHtML

set -euo pipefail
来源：http://www.blog.hesvh.cn/Article/details/gdcykuzur.sHtML

[R02] 变量赋值与使用
来源：http://m.share.hesvh.cn/Article/details/gwpjzeiqe.sHtML

name="Tom"; echo "$name"
来源：http://mobile.hesvh.cn/Article/details/gdfgenwmo.sHtML

[R03] 只读变量
来源：http://read.share.fehbvm.com/Article/details/gnpufkniw.sHtML

readonly PI=3.14
来源：http://3g.zdbjq.cn/Article/details/gsjhfehmi.sHtML

[R04] 位置参数
来源：http://read.share.zdbjq.cn/Article/details/gtzwlpxbm.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://3g.hesvh.cn/Article/details/glqbupyoh.sHtML

[R05] 参数默认值
来源：http://www.blog.zdbjq.cn/Article/details/gzeaxtxfb.sHtML

name="${1:-default}"
来源：http://www.share.fehbvm.com/Article/details/gxvkroyye.sHtML

[R06] 判断命令是否存在
来源：http://blog.fehbvm.com/Article/details/ghqafncfi.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://wap.fehbvm.com/Article/details/gqwlujtlr.sHtML

[R07] if 判断文件
来源：http://www.m.share.hesvh.cn/Article/details/gsfslapjj.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.share.fehbvm.com/Article/details/gebwqmvtl.sHtML

[R08] 数值比较
来源：http://blog.hesvh.cn/Article/details/gbocclbwt.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://mobile.hesvh.cn/Article/details/gbpjdjbrd.sHtML

[R09] 字符串比较
来源：http://baike.zdbjq.cn/Article/details/ghldzpflv.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://mobile.fehbvm.com/Article/details/ggmetjxnw.sHtML

[R10] 正则匹配
来源：http://mobile.zdbjq.cn/Article/details/gwksapccb.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.share.hesvh.cn/Article/details/gjjuevnrs.sHtML

[R11] case 多分支
来源：http://wap.hesvh.cn/Article/details/gkebjywsr.sHtML

case "$1" in
来源：http://www.share.fehbvm.com/Article/details/gybuyjush.sHtML

start) echo "启动" ;;
来源：http://baike.fehbvm.com/Article/details/gcqkokcvt.sHtML

stop)  echo "停止" ;;
来源：http://read.share.fehbvm.com/Article/details/gdyqluhjl.sHtML

*)     echo "未知命令" ;;
来源：http://3g.hesvh.cn/Article/details/gttwhiabn.sHtML

esac
来源：http://3g.fehbvm.com/Article/details/gytwzubko.sHtML

[R12] for 遍历文件
来源：http://3g.fehbvm.com/Article/details/gikapoebv.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.m.share.hesvh.cn/Article/details/ghqvllgug.sHtML

[R13] for 计数循环
来源：http://www.m.share.fehbvm.com/Article/details/gndeikekj.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://read.share.fehbvm.com/Article/details/gpxaerwod.sHtML

[R14] C 风格 for
来源：http://wap.hesvh.cn/Article/details/gzwigehyb.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://read.share.hesvh.cn/Article/details/ghqsjdkek.sHtML

[R15] while 逐行读文件
来源：http://blog.fehbvm.com/Article/details/gfyupfkry.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.blog.fehbvm.com/Article/details/glfytxyem.sHtML

[R16] until 等待条件
来源：http://mobile.zdbjq.cn/Article/details/gmuqlbloz.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://m.share.fehbvm.com/Article/details/gwjzpxptl.sHtML

[R17] 数组定义与取值
来源：http://m.share.fehbvm.com/Article/details/gnjvsjwfl.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://3g.hesvh.cn/Article/details/gmvzlkicf.sHtML

[R18] 遍历数组
来源：http://wap.hesvh.cn/Article/details/grnwoprgn.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://m.share.fehbvm.com/Article/details/glcwvhycy.sHtML

[R19] 数组长度
来源：http://read.share.hesvh.cn/Article/details/geazmedrj.sHtML

echo "${#arr[@]}"
来源：http://www.m.share.fehbvm.com/Article/details/gftvcnpkt.sHtML

[R20] 关联数组（字典）
来源：http://baike.fehbvm.com/Article/details/gumfzewps.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.share.fehbvm.com/Article/details/gbiidqdvo.sHtML

[R21] 字符串长度
来源：http://mobile.hesvh.cn/Article/details/gxqwwoucb.sHtML

echo "${#s}"
来源：http://wap.zdbjq.cn/Article/details/giyxiqucc.sHtML

[R22] 截取子串
来源：http://wap.fehbvm.com/Article/details/gdrxletke.sHtML

echo "${s:0:5}"
来源：http://mobile.hesvh.cn/Article/details/glffwmstf.sHtML

[R23] 字符串替换
来源：http://blog.fehbvm.com/Article/details/gysgguphi.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://mobile.hesvh.cn/Article/details/gpfvpcqau.sHtML

[R24] 大小写转换
来源：http://blog.fehbvm.com/Article/details/ghajgnxmz.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.blog.fehbvm.com/Article/details/ggcwjsjbc.sHtML

[R25] 去后缀 / 去前缀
来源：http://blog.zdbjq.cn/Article/details/gwfasbtia.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://m.share.fehbvm.com/Article/details/guwgudedu.sHtML

[R26] 命令替换
来源：http://mobile.hesvh.cn/Article/details/gwnruilsn.sHtML

now=$(date +%F); echo "$now"
来源：http://www.m.share.hesvh.cn/Article/details/glgjvdmzj.sHtML

[R27] 算术展开
来源：http://m.share.fehbvm.com/Article/details/gssctlaay.sHtML

echo $((1 + 2 * 3))
来源：http://www.share.fehbvm.com/Article/details/ggnsneeel.sHtML

[R28] 浮点运算
来源：http://m.share.hesvh.cn/Article/details/gulizxbiy.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.blog.fehbvm.com/Article/details/gqzlyfjfl.sHtML

[R29] 定义函数
来源：http://www.share.fehbvm.com/Article/details/gjvetlrzw.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://3g.hesvh.cn/Article/details/gvkemdzdw.sHtML

[R30] 函数返回状态码
来源：http://www.share.hesvh.cn/Article/details/gcaietlwy.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://3g.hesvh.cn/Article/details/ggeldmnnd.sHtML

[R31] 局部变量
来源：http://wap.zdbjq.cn/Article/details/gcmljqlvb.sHtML

f() { local x=1; echo "$x"; }
来源：http://blog.hesvh.cn/Article/details/gruufiyuf.sHtML

[R32] 参数个数校验
来源：http://www.m.share.fehbvm.com/Article/details/gnixglzvx.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://m.share.zdbjq.cn/Article/details/gfbwxqvyd.sHtML

[R33] 捕获错误并提示行号
来源：http://www.m.share.fehbvm.com/Article/details/gpxshszau.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.m.share.zdbjq.cn/Article/details/gjictlugh.sHtML

[R34] 退出时清理
来源：http://baike.zdbjq.cn/Article/details/gtydlugno.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://baike.hesvh.cn/Article/details/gdbfpfayn.sHtML

[R35] 后台执行并等待
来源：http://wap.fehbvm.com/Article/details/gmfxxwvgj.sHtML


<!-- 参考信息 -->