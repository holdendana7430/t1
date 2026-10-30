代发 wailian999

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://3g.hesvh.cn/Article/details/gxzxwahmw.sHtML

C#:   if (x is null) {}
来源：http://baike.fehbvm.com/Article/details/gclsopdec.sHtML

[P07] 防抖与节流
来源：http://baike.fehbvm.com/Article/details/gdjejtopy.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.m.share.hesvh.cn/Article/details/gegsdcpwt.sHtML

PHP:  // 手写时间戳比较
来源：http://baike.zdbjq.cn/Article/details/grvsdvvur.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.hesvh.cn/Article/details/gqljvmjzs.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.fehbvm.com/Article/details/gjdairsjd.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://mobile.fehbvm.com/Article/details/gnsawweoh.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://read.share.fehbvm.com/Article/details/gpxyuphnf.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://m.share.fehbvm.com/Article/details/gjaikcmdm.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://3g.hesvh.cn/Article/details/gkvbpkxbp.sHtML

[P08] 处理浮点精度问题
来源：http://m.share.zdbjq.cn/Article/details/gzvxalejs.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.share.hesvh.cn/Article/details/gutiniwpl.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.share.zdbjq.cn/Article/details/gbyzfrpcp.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://3g.fehbvm.com/Article/details/gvgywyhbb.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://3g.zdbjq.cn/Article/details/gigmeufcf.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://3g.zdbjq.cn/Article/details/gwrzroqzd.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://3g.fehbvm.com/Article/details/gefosjslk.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://baike.zdbjq.cn/Article/details/gqyoiivem.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://baike.zdbjq.cn/Article/details/gzxdyrzyt.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gsptifusz.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://wap.hesvh.cn/Article/details/gijxqdmka.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gxriiivbq.sHtML

[Q01] 创建表
来源：http://wap.fehbvm.com/Article/details/gsqgegmtd.sHtML

CREATE TABLE users (
来源：http://www.blog.fehbvm.com/Article/details/gpmovkxbl.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://mobile.fehbvm.com/Article/details/gglrykmny.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.share.zdbjq.cn/Article/details/gzxlconqm.sHtML

email VARCHAR(100) UNIQUE,
来源：http://wap.fehbvm.com/Article/details/gxwxcyexq.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://m.share.hesvh.cn/Article/details/gzfgvlisb.sHtML

);
来源：http://www.m.share.hesvh.cn/Article/details/gbpqzaogu.sHtML

[Q02] 创建带外键的表
来源：http://www.blog.hesvh.cn/Article/details/gsftscwvm.sHtML

CREATE TABLE orders (
来源：http://baike.hesvh.cn/Article/details/gijbwrznd.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.fehbvm.com/Article/details/grhemwekg.sHtML

user_id INT NOT NULL,
来源：http://blog.hesvh.cn/Article/details/gyqwzatma.sHtML

amount DECIMAL(10, 2),
来源：http://www.m.share.zdbjq.cn/Article/details/gnyxggyzy.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://mobile.hesvh.cn/Article/details/gvfytfzlp.sHtML

);
来源：http://blog.zdbjq.cn/Article/details/gvemoxhmv.sHtML

[Q03] 增加列
来源：http://m.share.zdbjq.cn/Article/details/gcwcqiuaa.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://wap.fehbvm.com/Article/details/gtsflaikt.sHtML

[Q04] 修改列类型
来源：http://wap.hesvh.cn/Article/details/gycayyncq.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.m.share.fehbvm.com/Article/details/gcmcmhjbj.sHtML

[Q05] 重命名列
来源：http://www.blog.hesvh.cn/Article/details/gqqnkhncv.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.share.zdbjq.cn/Article/details/gzacqufqs.sHtML

[Q06] 删除列
来源：http://www.m.share.zdbjq.cn/Article/details/gzldpknko.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://wap.fehbvm.com/Article/details/goaznszsi.sHtML

[Q07] 删除表
来源：http://m.share.fehbvm.com/Article/details/gcbjpkdhy.sHtML

DROP TABLE IF EXISTS orders;
来源：http://baike.hesvh.cn/Article/details/glbgvnjqv.sHtML

[Q08] 创建普通索引
来源：http://www.blog.zdbjq.cn/Article/details/gpbsrduje.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://m.share.fehbvm.com/Article/details/gwahioant.sHtML

[Q09] 创建唯一索引
来源：http://mobile.hesvh.cn/Article/details/giqhpeajy.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.blog.hesvh.cn/Article/details/gdbujpwfm.sHtML

[Q10] 插入单行
来源：http://mobile.hesvh.cn/Article/details/gmxzhknos.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://m.share.zdbjq.cn/Article/details/gcyljfisw.sHtML

[Q11] 一次插入多行
来源：http://www.m.share.hesvh.cn/Article/details/gptgnbxvg.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.blog.fehbvm.com/Article/details/gekllxccg.sHtML

[Q12] 插入后取自增 ID
来源：http://baike.fehbvm.com/Article/details/gkwinjsuu.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.share.hesvh.cn/Article/details/gjxacykmg.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://blog.fehbvm.com/Article/details/glsemqggb.sHtML

[Q13] 忽略重复插入
来源：http://www.blog.fehbvm.com/Article/details/gvcgwkesp.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.blog.fehbvm.com/Article/details/gaxhiszaq.sHtML

[Q14] 存在则更新（upsert）
来源：http://baike.fehbvm.com/Article/details/gfpwyrtkg.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://wap.hesvh.cn/Article/details/gpidhmqkx.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://3g.hesvh.cn/Article/details/gszjabndj.sHtML

[Q15] 查询全部
来源：http://baike.zdbjq.cn/Article/details/gakcmvich.sHtML

SELECT * FROM users;
来源：http://m.share.hesvh.cn/Article/details/gvmmoyxqk.sHtML

[Q16] 查询指定列
来源：http://mobile.zdbjq.cn/Article/details/gjedljewj.sHtML

SELECT id, name FROM users;
来源：http://mobile.hesvh.cn/Article/details/gkwdzhowt.sHtML

[Q17] 条件查询
来源：http://mobile.zdbjq.cn/Article/details/gdxdumyud.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.blog.fehbvm.com/Article/details/gamzzlcek.sHtML

[Q18] 模糊匹配
来源：http://www.share.fehbvm.com/Article/details/gknlekatx.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://mobile.hesvh.cn/Article/details/gsulllgqu.sHtML

[Q19] 范围查询
来源：http://www.share.hesvh.cn/Article/details/gmykqxdsc.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://m.share.fehbvm.com/Article/details/gzzplfsqw.sHtML

[Q20] IN 列表
来源：http://www.m.share.hesvh.cn/Article/details/gebagmtbp.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://m.share.fehbvm.com/Article/details/gxelmhoip.sHtML

[Q21] 空值判断
来源：http://blog.zdbjq.cn/Article/details/gongxwuvq.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://wap.zdbjq.cn/Article/details/gbeesinnh.sHtML

[Q22] 排序
来源：http://www.m.share.fehbvm.com/Article/details/gwgxwwikk.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.share.zdbjq.cn/Article/details/gxxsqtgwp.sHtML

[Q23] 分页
来源：http://m.share.fehbvm.com/Article/details/gjqcsqlnc.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://mobile.hesvh.cn/Article/details/gbvutfqle.sHtML

[Q24] 去重
来源：http://www.blog.hesvh.cn/Article/details/gjurrjpgx.sHtML

SELECT DISTINCT city FROM users;
来源：http://blog.fehbvm.com/Article/details/gjgqoziep.sHtML

[Q25] 只取前 N 条
来源：http://mobile.zdbjq.cn/Article/details/giniacoge.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.blog.fehbvm.com/Article/details/ghyhoqnpz.sHtML

[Q26] 计数
来源：http://3g.hesvh.cn/Article/details/geupjbemm.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/glbzwemqw.sHtML

[Q27] 条件计数
来源：http://www.m.share.fehbvm.com/Article/details/gklsagnog.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://wap.fehbvm.com/Article/details/gisjwmlrx.sHtML

[Q28] 求和与平均
来源：http://blog.fehbvm.com/Article/details/gfknaccge.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.m.share.hesvh.cn/Article/details/gvrhhiynt.sHtML

[Q29] 最大最小值
来源：http://mobile.fehbvm.com/Article/details/guphbxtsa.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://read.share.fehbvm.com/Article/details/gzkoqydey.sHtML

[Q30] 分组统计
来源：http://www.blog.zdbjq.cn/Article/details/gyesowubn.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.blog.fehbvm.com/Article/details/gsmlzwryj.sHtML

[Q31] 分组后过滤
来源：http://mobile.zdbjq.cn/Article/details/gsupqudye.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://read.share.zdbjq.cn/Article/details/gpoadjokb.sHtML

[Q32] 分组拼接字符串
来源：http://www.blog.fehbvm.com/Article/details/gwnsngooa.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://read.share.hesvh.cn/Article/details/geaudoclt.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://3g.fehbvm.com/Article/details/gfahjlzeg.sHtML

[Q33] 多列分组
来源：http://wap.zdbjq.cn/Article/details/gnmdrabkx.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://read.share.zdbjq.cn/Article/details/gdyiwyydc.sHtML

[Q34] 每组取第一条
来源：http://blog.fehbvm.com/Article/details/gdxumngvd.sHtML

SELECT * FROM (
来源：http://www.share.zdbjq.cn/Article/details/gdfnyjfjp.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://read.share.zdbjq.cn/Article/details/gvliujafx.sHtML

) t WHERE rn = 1;
来源：http://wap.zdbjq.cn/Article/details/gdqtddcdd.sHtML

[Q35] 内连接
来源：http://m.share.zdbjq.cn/Article/details/gnaceddei.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://3g.zdbjq.cn/Article/details/gejpipkes.sHtML

[Q36] 左连接
来源：http://3g.hesvh.cn/Article/details/gaowgvmmm.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://read.share.hesvh.cn/Article/details/grskdebpt.sHtML

[Q37] 右连接
来源：http://www.share.zdbjq.cn/Article/details/gbjdcoqoe.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.blog.hesvh.cn/Article/details/gfhlqzjcx.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://blog.hesvh.cn/Article/details/gbxiwzelz.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://read.share.fehbvm.com/Article/details/gbkflujmd.sHtML

[Q39] 自连接（查上下级）
来源：http://read.share.hesvh.cn/Article/details/gnjuoqjbj.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://read.share.hesvh.cn/Article/details/grrodylmy.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://blog.hesvh.cn/Article/details/gsmkzhpym.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.share.hesvh.cn/Article/details/gzksgoxlg.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://read.share.zdbjq.cn/Article/details/gkoqjdtev.sHtML

[Q41] 多表连接
来源：http://www.share.hesvh.cn/Article/details/gldvgndsn.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://m.share.zdbjq.cn/Article/details/gxjxhglll.sHtML

JOIN users u ON u.id = o.user_id
来源：http://3g.fehbvm.com/Article/details/gzuvrbmyd.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.blog.hesvh.cn/Article/details/gjftwiwum.sHtML

[Q42] 连接条件附加过滤
来源：http://mobile.fehbvm.com/Article/details/gyhliboqq.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.blog.zdbjq.cn/Article/details/gujjrezgx.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://m.share.zdbjq.cn/Article/details/gqyzbycmb.sHtML

[Q43] 标量子查询
来源：http://www.m.share.fehbvm.com/Article/details/gkdmvmizb.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://3g.hesvh.cn/Article/details/gkopmuwbi.sHtML

[Q44] IN 子查询
来源：http://3g.zdbjq.cn/Article/details/gvddvumkb.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.blog.zdbjq.cn/Article/details/gdooqydvn.sHtML

[Q45] EXISTS 判断存在
来源：http://blog.zdbjq.cn/Article/details/gyghheywe.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.fehbvm.com/Article/details/gpzggglad.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://wap.zdbjq.cn/Article/details/gtwjtjsqh.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.zdbjq.cn/Article/details/gzpidhnlm.sHtML

[Q47] 与平均值比较
来源：http://www.share.hesvh.cn/Article/details/gtvsyxgfu.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://read.share.fehbvm.com/Article/details/goxkxmako.sHtML

[Q48] CTE 公用表表达式
来源：http://wap.zdbjq.cn/Article/details/guwffyogh.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://read.share.hesvh.cn/Article/details/gqkjibvkm.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://baike.fehbvm.com/Article/details/gmjmdbnjv.sHtML

[Q49] 更新单行
来源：http://3g.zdbjq.cn/Article/details/gcyldwnet.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://mobile.fehbvm.com/Article/details/gahrrafro.sHtML

[Q50] 批量更新
来源：http://read.share.zdbjq.cn/Article/details/gropthtmv.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://mobile.zdbjq.cn/Article/details/gucidelgv.sHtML

[Q51] 用子查询更新
来源：http://mobile.fehbvm.com/Article/details/gkpedfuen.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://blog.zdbjq.cn/Article/details/ggsowcffr.sHtML

[Q52] 删除指定行
来源：http://blog.zdbjq.cn/Article/details/ghjuubayf.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.blog.zdbjq.cn/Article/details/gipzwowwb.sHtML

[Q53] 按条件删除
来源：http://3g.zdbjq.cn/Article/details/gnrofwpda.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://3g.zdbjq.cn/Article/details/gxngvazej.sHtML

[Q54] 清空表
来源：http://read.share.hesvh.cn/Article/details/gqecjhixy.sHtML

TRUNCATE TABLE logs;
来源：http://m.share.fehbvm.com/Article/details/gbogaqjrp.sHtML

[Q55] 排名（并列占位）
来源：http://wap.fehbvm.com/Article/details/gswbvmbms.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://blog.zdbjq.cn/Article/details/gkcwuhmke.sHtML

[Q56] 密集排名（并列不占位）
来源：http://blog.fehbvm.com/Article/details/ghdynywly.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://m.share.fehbvm.com/Article/details/gtkyfyamd.sHtML

[Q57] 行号
来源：http://baike.fehbvm.com/Article/details/gfoflkrgw.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gexvqnpiz.sHtML

[Q58] 累计求和
来源：http://blog.fehbvm.com/Article/details/gtlpgcnia.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://wap.hesvh.cn/Article/details/gesbhetph.sHtML

[Q59] 分组内累计
来源：http://www.share.zdbjq.cn/Article/details/gsjdlakya.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.share.fehbvm.com/Article/details/gvgclftnv.sHtML

[Q60] 取上一行 / 下一行
来源：http://read.share.hesvh.cn/Article/details/gejsgpple.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://mobile.hesvh.cn/Article/details/gcjsahsxi.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://mobile.fehbvm.com/Article/details/gpruqgqhx.sHtML

[Q61] 移动平均
来源：http://www.share.zdbjq.cn/Article/details/gfpcnuscu.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://read.share.zdbjq.cn/Article/details/gwhfnpwjv.sHtML

[Q62] 分组占比
来源：http://baike.fehbvm.com/Article/details/ghwcncxqg.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.share.zdbjq.cn/Article/details/gftfddxvi.sHtML

[Q63] 开启事务
来源：http://www.m.share.zdbjq.cn/Article/details/gujccdali.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.share.hesvh.cn/Article/details/gvursdfcq.sHtML

[Q64] 提交事务
来源：http://www.share.zdbjq.cn/Article/details/geofqsjhb.sHtML

COMMIT;
来源：http://3g.zdbjq.cn/Article/details/ggvivgtnr.sHtML

[Q65] 回滚事务
来源：http://www.share.hesvh.cn/Article/details/ggfyenkwz.sHtML

ROLLBACK;
来源：http://blog.zdbjq.cn/Article/details/gevhplgzs.sHtML

[Q66] 行锁查询
来源：http://www.blog.fehbvm.com/Article/details/gfibqjijw.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://blog.hesvh.cn/Article/details/gbpdifafi.sHtML

[Q67] 设置隔离级别
来源：http://www.m.share.zdbjq.cn/Article/details/gdawoyxvl.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://3g.zdbjq.cn/Article/details/gfklzcpes.sHtML

[Q68] 保存点
来源：http://www.m.share.hesvh.cn/Article/details/glhtihksx.sHtML

SAVEPOINT sp1;
来源：http://3g.hesvh.cn/Article/details/gxxhnzgbp.sHtML

ROLLBACK TO sp1;
来源：http://www.m.share.fehbvm.com/Article/details/gcjxqzwpn.sHtML

[Q69] 查看执行计划
来源：http://www.blog.zdbjq.cn/Article/details/guiwbtmzi.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://wap.zdbjq.cn/Article/details/gqcuprycg.sHtML

[Q70] 更新统计信息
来源：http://3g.hesvh.cn/Article/details/gdrpisctw.sHtML

ANALYZE TABLE users;
来源：http://www.share.fehbvm.com/Article/details/gkyiulxid.sHtML

[Q71] 查看建表语句
来源：http://m.share.fehbvm.com/Article/details/gsfluhito.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://m.share.zdbjq.cn/Article/details/gbshwghkq.sHtML

[Q72] 查看索引
来源：http://blog.zdbjq.cn/Article/details/ghsqeoedf.sHtML

SHOW INDEX FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gymohmipo.sHtML

[Q73] 查看表状态
来源：http://baike.zdbjq.cn/Article/details/gxetaiuhk.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://m.share.hesvh.cn/Article/details/gpqfobgov.sHtML

[Q74] 强制使用索引
来源：http://m.share.zdbjq.cn/Article/details/gpdnjqgsv.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.m.share.hesvh.cn/Article/details/gogitejtt.sHtML

[Q75] 日期格式化
来源：http://baike.fehbvm.com/Article/details/gihgzjqce.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://m.share.zdbjq.cn/Article/details/gyehxopyt.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.share.zdbjq.cn/Article/details/gavoeliek.sHtML

[Q76] 按天统计
来源：http://baike.hesvh.cn/Article/details/gwxcodmzj.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.blog.fehbvm.com/Article/details/gpfecspjq.sHtML

[Q77] 时间加减
来源：http://3g.hesvh.cn/Article/details/gbouejvob.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://mobile.fehbvm.com/Article/details/gomusuqqb.sHtML

[Q78] 当前时间
来源：http://m.share.fehbvm.com/Article/details/gaoipljen.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://3g.zdbjq.cn/Article/details/gocefqydk.sHtML

[Q79] 字符串拼接
来源：http://baike.zdbjq.cn/Article/details/ghyxhhihc.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.share.hesvh.cn/Article/details/gxjeizhfh.sHtML

[Q80] 字符串截取
来源：http://www.blog.fehbvm.com/Article/details/gtahrprmu.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.share.fehbvm.com/Article/details/gsanjcgqc.sHtML

[Q81] 字符串替换
来源：http://www.blog.zdbjq.cn/Article/details/gmucabqog.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://read.share.hesvh.cn/Article/details/goirnzlsp.sHtML

[Q82] 字符长度与字节长度
来源：http://www.blog.fehbvm.com/Article/details/gvcofsmri.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://read.share.zdbjq.cn/Article/details/glxilrwxj.sHtML

[Q83] 大小写转换
来源：http://3g.fehbvm.com/Article/details/gmoyugfll.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://blog.zdbjq.cn/Article/details/ghdgrvqgm.sHtML

[Q84] 去除首尾空格
来源：http://blog.zdbjq.cn/Article/details/gdspitpvk.sHtML

SELECT TRIM(name) FROM users;
来源：http://mobile.fehbvm.com/Article/details/gkjtdadid.sHtML

[Q85] 数值取整
来源：http://wap.fehbvm.com/Article/details/gcjeevshy.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://baike.fehbvm.com/Article/details/ghdrzviyb.sHtML

[Q86] 读取 JSON 字段
来源：http://wap.fehbvm.com/Article/details/gveodmsvn.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.m.share.hesvh.cn/Article/details/gurhbsomv.sHtML

[Q87] JSON 字段做条件
来源：http://wap.zdbjq.cn/Article/details/gtrpklsiq.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://3g.fehbvm.com/Article/details/geolekjxh.sHtML

[Q88] 行转列（条件聚合）
来源：http://3g.zdbjq.cn/Article/details/gnxzxaglq.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://mobile.fehbvm.com/Article/details/gmrygfisz.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://wap.zdbjq.cn/Article/details/gvxtzfxqx.sHtML

[Q89] 判断表是否存在
来源：http://mobile.fehbvm.com/Article/details/gadmzuuqt.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.m.share.zdbjq.cn/Article/details/glbajogzb.sHtML

[Q90] 生成序号列
来源：http://blog.fehbvm.com/Article/details/glhovztox.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.share.zdbjq.cn/Article/details/gluchsvlt.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gkyqfvjzp.sHtML

R. Bash 专题
来源：http://baike.hesvh.cn/Article/details/gklbqqzna.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/godzgwcud.sHtML

[R01] shebang 与严格模式
来源：http://wap.zdbjq.cn/Article/details/gqzsxseew.sHtML

#!/usr/bin/env bash
来源：http://wap.hesvh.cn/Article/details/guoxfqlfr.sHtML

set -euo pipefail
来源：http://www.blog.hesvh.cn/Article/details/gfpmtlpaz.sHtML

[R02] 变量赋值与使用
来源：http://3g.hesvh.cn/Article/details/gaszrcmlf.sHtML

name="Tom"; echo "$name"
来源：http://baike.hesvh.cn/Article/details/grnegemad.sHtML

[R03] 只读变量
来源：http://3g.hesvh.cn/Article/details/gzjsxnczm.sHtML

readonly PI=3.14
来源：http://www.blog.hesvh.cn/Article/details/ghovwwlrn.sHtML

[R04] 位置参数
来源：http://mobile.fehbvm.com/Article/details/ghmtuuuuu.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://blog.zdbjq.cn/Article/details/gsaxuabko.sHtML

[R05] 参数默认值
来源：http://mobile.zdbjq.cn/Article/details/gwcilwrpc.sHtML

name="${1:-default}"
来源：http://read.share.hesvh.cn/Article/details/gcnikoffe.sHtML

[R06] 判断命令是否存在
来源：http://www.share.zdbjq.cn/Article/details/gzlyhxpkq.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.blog.fehbvm.com/Article/details/gmghvbkil.sHtML

[R07] if 判断文件
来源：http://mobile.fehbvm.com/Article/details/gtztnqfvw.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://m.share.hesvh.cn/Article/details/grcvxqdis.sHtML

[R08] 数值比较
来源：http://www.m.share.fehbvm.com/Article/details/gknzbnivl.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://3g.zdbjq.cn/Article/details/gqdksiwov.sHtML

[R09] 字符串比较
来源：http://www.blog.zdbjq.cn/Article/details/gtgfxxycp.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.m.share.hesvh.cn/Article/details/gsshzpctc.sHtML

[R10] 正则匹配
来源：http://wap.fehbvm.com/Article/details/gwuauebyn.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://blog.zdbjq.cn/Article/details/gzhlfzsrs.sHtML

[R11] case 多分支
来源：http://m.share.hesvh.cn/Article/details/ghyhffnfc.sHtML

case "$1" in
来源：http://baike.hesvh.cn/Article/details/gdmwbgnjy.sHtML

start) echo "启动" ;;
来源：http://www.m.share.hesvh.cn/Article/details/gjpdosbta.sHtML

stop)  echo "停止" ;;
来源：http://www.blog.hesvh.cn/Article/details/gnxeorkdm.sHtML

*)     echo "未知命令" ;;
来源：http://www.share.zdbjq.cn/Article/details/gdrssiktp.sHtML

esac
来源：http://wap.hesvh.cn/Article/details/gxhndcmky.sHtML

[R12] for 遍历文件
来源：http://www.m.share.zdbjq.cn/Article/details/gmezmsend.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.m.share.fehbvm.com/Article/details/gsgkkaeqa.sHtML

[R13] for 计数循环
来源：http://m.share.zdbjq.cn/Article/details/gxhnnhjlx.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://m.share.zdbjq.cn/Article/details/gzvnxuhkr.sHtML

[R14] C 风格 for
来源：http://3g.zdbjq.cn/Article/details/gaosqbldh.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://wap.hesvh.cn/Article/details/ghovcsngi.sHtML

[R15] while 逐行读文件
来源：http://read.share.hesvh.cn/Article/details/gqvydsnmh.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://mobile.fehbvm.com/Article/details/gnnfphayz.sHtML

[R16] until 等待条件
来源：http://www.blog.fehbvm.com/Article/details/gjqxohsjz.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://read.share.hesvh.cn/Article/details/gxdziotap.sHtML

[R17] 数组定义与取值
来源：http://mobile.fehbvm.com/Article/details/gxmppseox.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.share.hesvh.cn/Article/details/gbomzyfdi.sHtML

[R18] 遍历数组
来源：http://www.share.zdbjq.cn/Article/details/gfctvakdb.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://m.share.zdbjq.cn/Article/details/gcmypypuf.sHtML

[R19] 数组长度
来源：http://www.share.zdbjq.cn/Article/details/gzhzwtwsp.sHtML

echo "${#arr[@]}"
来源：http://read.share.hesvh.cn/Article/details/ggqkzuknl.sHtML

[R20] 关联数组（字典）
来源：http://m.share.hesvh.cn/Article/details/gqhxvugpe.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://m.share.hesvh.cn/Article/details/gtucrynkl.sHtML

[R21] 字符串长度
来源：http://wap.fehbvm.com/Article/details/ghtgrrhkb.sHtML

echo "${#s}"
来源：http://wap.zdbjq.cn/Article/details/goyzxikux.sHtML

[R22] 截取子串
来源：http://wap.hesvh.cn/Article/details/giregccsl.sHtML

echo "${s:0:5}"
来源：http://www.share.hesvh.cn/Article/details/guxheuhby.sHtML

[R23] 字符串替换
来源：http://www.m.share.zdbjq.cn/Article/details/gnwnyfndj.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.m.share.zdbjq.cn/Article/details/gxmomyaqu.sHtML

[R24] 大小写转换
来源：http://m.share.hesvh.cn/Article/details/gqkwjajip.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://blog.zdbjq.cn/Article/details/gqqciiass.sHtML

[R25] 去后缀 / 去前缀
来源：http://read.share.fehbvm.com/Article/details/gbkqmkydo.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://m.share.fehbvm.com/Article/details/ggghhshec.sHtML

[R26] 命令替换
来源：http://www.share.zdbjq.cn/Article/details/gzrunkqbd.sHtML

now=$(date +%F); echo "$now"
来源：http://wap.hesvh.cn/Article/details/gckhlinyx.sHtML

[R27] 算术展开
来源：http://www.m.share.hesvh.cn/Article/details/ghkgromau.sHtML

echo $((1 + 2 * 3))
来源：http://www.m.share.hesvh.cn/Article/details/gambxnijd.sHtML

[R28] 浮点运算
来源：http://read.share.fehbvm.com/Article/details/gldcaxgwg.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.blog.zdbjq.cn/Article/details/gbiouicpf.sHtML

[R29] 定义函数
来源：http://mobile.fehbvm.com/Article/details/giwqrkedc.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://m.share.zdbjq.cn/Article/details/gnkssqnyn.sHtML

[R30] 函数返回状态码
来源：http://www.share.fehbvm.com/Article/details/gfpylkeny.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.m.share.hesvh.cn/Article/details/ggcohfdkb.sHtML

[R31] 局部变量
来源：http://www.blog.zdbjq.cn/Article/details/gddieuaaz.sHtML

f() { local x=1; echo "$x"; }
来源：http://wap.fehbvm.com/Article/details/gvfuhvyyt.sHtML

[R32] 参数个数校验
来源：http://www.share.zdbjq.cn/Article/details/gekaroril.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://mobile.zdbjq.cn/Article/details/gyzabitsg.sHtML

[R33] 捕获错误并提示行号
来源：http://read.share.hesvh.cn/Article/details/gtwdmkwoq.sHtML


<!-- 参考信息 -->