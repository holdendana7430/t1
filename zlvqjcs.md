代发 wailian999

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://mobile.fanxiaobao.xyz/Article/details/gmcsozihz.sHtML

TS:   if (x == null) {}
来源：http://www.blog.fanxiaobao.xyz/Article/details/guvrkpfof.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://read.share.fanxiaobao.xyz/Article/details/gzuncqtpy.sHtML

Go:   if x == nil {}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glvxhpeot.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://mobile.fanxiaobao.xyz/Article/details/glpmpbkgf.sHtML

C#:   if (x is null) {}
来源：http://blog.fanxiaobao.xyz/Article/details/grvvhqcvi.sHtML

[P07] 防抖与节流
来源：http://m.share.fanxiaobao.xyz/Article/details/gcnsakzcx.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://baike.fanxiaobao.xyz/Article/details/gbasgieab.sHtML

PHP:  // 手写时间戳比较
来源：http://baike.fanxiaobao.xyz/Article/details/ggshqqivy.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnemokzrh.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.fanxiaobao.xyz/Article/details/gnwgfjcah.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnkzuprpc.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://read.share.fanxiaobao.xyz/Article/details/gazscbnui.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmdkijdde.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.share.fanxiaobao.xyz/Article/details/gqnbftort.sHtML

[P08] 处理浮点精度问题
来源：http://blog.fanxiaobao.xyz/Article/details/grvyqtwvb.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://blog.fanxiaobao.xyz/Article/details/genrirtcz.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://3g.fanxiaobao.xyz/Article/details/gpnimrjsa.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://mobile.fanxiaobao.xyz/Article/details/gguuprqea.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://read.share.fanxiaobao.xyz/Article/details/gaazoahgx.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://read.share.fanxiaobao.xyz/Article/details/gdpvyjrxd.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://mobile.fanxiaobao.xyz/Article/details/gtkqilnfq.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://blog.fanxiaobao.xyz/Article/details/gpwtcbcqa.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://blog.fanxiaobao.xyz/Article/details/gsyjywxvd.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gycxbqvvv.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaajwscta.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gedaojyvx.sHtML

[Q01] 创建表
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjbgdphha.sHtML

CREATE TABLE users (
来源：http://baike.fanxiaobao.xyz/Article/details/geingdowd.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.share.fanxiaobao.xyz/Article/details/gsnaafdvq.sHtML

name VARCHAR(50) NOT NULL,
来源：http://3g.fanxiaobao.xyz/Article/details/gylxavojw.sHtML

email VARCHAR(100) UNIQUE,
来源：http://mobile.fanxiaobao.xyz/Article/details/gemglzkyq.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://wap.fanxiaobao.xyz/Article/details/grgcqucte.sHtML

);
来源：http://m.share.fanxiaobao.xyz/Article/details/glxinsmis.sHtML

[Q02] 创建带外键的表
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtnpihney.sHtML

CREATE TABLE orders (
来源：http://blog.fanxiaobao.xyz/Article/details/ghaanrsaa.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.fanxiaobao.xyz/Article/details/gdgimmtsa.sHtML

user_id INT NOT NULL,
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbgloaqfj.sHtML

amount DECIMAL(10, 2),
来源：http://www.share.fanxiaobao.xyz/Article/details/gvwccwjpv.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://blog.fanxiaobao.xyz/Article/details/gxmpnycts.sHtML

);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmupaqmta.sHtML

[Q03] 增加列
来源：http://www.share.fanxiaobao.xyz/Article/details/gusbawnyk.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://baike.fanxiaobao.xyz/Article/details/gpbaicczo.sHtML

[Q04] 修改列类型
来源：http://blog.fanxiaobao.xyz/Article/details/ghepgragh.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://read.share.fanxiaobao.xyz/Article/details/gpenltpxe.sHtML

[Q05] 重命名列
来源：http://www.share.fanxiaobao.xyz/Article/details/gfoocxolm.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://mobile.fanxiaobao.xyz/Article/details/gsbejwhsv.sHtML

[Q06] 删除列
来源：http://m.share.fanxiaobao.xyz/Article/details/gslwxgqkl.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://blog.fanxiaobao.xyz/Article/details/gozfdoxim.sHtML

[Q07] 删除表
来源：http://wap.fanxiaobao.xyz/Article/details/glcaucmpf.sHtML

DROP TABLE IF EXISTS orders;
来源：http://baike.fanxiaobao.xyz/Article/details/gcudomzsx.sHtML

[Q08] 创建普通索引
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gviowvffu.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://read.share.fanxiaobao.xyz/Article/details/gwgdopuri.sHtML

[Q09] 创建唯一索引
来源：http://www.share.fanxiaobao.xyz/Article/details/gfdarfxpu.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gatmpbeqs.sHtML

[Q10] 插入单行
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpasjpuzv.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://blog.fanxiaobao.xyz/Article/details/ggbwjzpvb.sHtML

[Q11] 一次插入多行
来源：http://baike.fanxiaobao.xyz/Article/details/gskmnhnwd.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://baike.fanxiaobao.xyz/Article/details/goikckazf.sHtML

[Q12] 插入后取自增 ID
来源：http://www.share.fanxiaobao.xyz/Article/details/gdxveeadj.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://mobile.fanxiaobao.xyz/Article/details/gnpbhnldr.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxvlcvksa.sHtML

[Q13] 忽略重复插入
来源：http://www.share.fanxiaobao.xyz/Article/details/gvupssijy.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://3g.fanxiaobao.xyz/Article/details/gnrsjmpdu.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggpspomua.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://m.share.fanxiaobao.xyz/Article/details/gnddquhjt.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyogisahx.sHtML

[Q15] 查询全部
来源：http://wap.fanxiaobao.xyz/Article/details/gsbpwxnne.sHtML

SELECT * FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/ggicetddd.sHtML

[Q16] 查询指定列
来源：http://blog.fanxiaobao.xyz/Article/details/guavfumwz.sHtML

SELECT id, name FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gisjihdfi.sHtML

[Q17] 条件查询
来源：http://baike.fanxiaobao.xyz/Article/details/gaanqbgkl.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkvdocurm.sHtML

[Q18] 模糊匹配
来源：http://www.blog.fanxiaobao.xyz/Article/details/geqgokhvm.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfqmebyua.sHtML

[Q19] 范围查询
来源：http://www.share.fanxiaobao.xyz/Article/details/gcgpgvcse.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://read.share.fanxiaobao.xyz/Article/details/gpzqhneuq.sHtML

[Q20] IN 列表
来源：http://blog.fanxiaobao.xyz/Article/details/gutrsttoe.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gptydvdya.sHtML

[Q21] 空值判断
来源：http://wap.fanxiaobao.xyz/Article/details/gpocxqjzu.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.blog.fanxiaobao.xyz/Article/details/giriqsqsa.sHtML

[Q22] 排序
来源：http://www.share.fanxiaobao.xyz/Article/details/gthwloeph.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://3g.fanxiaobao.xyz/Article/details/gwtmjhfpa.sHtML

[Q23] 分页
来源：http://read.share.fanxiaobao.xyz/Article/details/gqhwmlcqh.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://baike.fanxiaobao.xyz/Article/details/giaoyopwi.sHtML

[Q24] 去重
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glhafaqcz.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzqcwzjvj.sHtML

[Q25] 只取前 N 条
来源：http://blog.fanxiaobao.xyz/Article/details/gegxkiyau.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.share.fanxiaobao.xyz/Article/details/gwbvpvpoc.sHtML

[Q26] 计数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzsyttamh.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gavclcami.sHtML

[Q27] 条件计数
来源：http://3g.fanxiaobao.xyz/Article/details/gxtlprnww.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfcfxmqws.sHtML

[Q28] 求和与平均
来源：http://wap.fanxiaobao.xyz/Article/details/gnbbnfwoh.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://m.share.fanxiaobao.xyz/Article/details/gfpiizzbm.sHtML

[Q29] 最大最小值
来源：http://www.share.fanxiaobao.xyz/Article/details/gcfstvkcn.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gbygzfzii.sHtML

[Q30] 分组统计
来源：http://m.share.fanxiaobao.xyz/Article/details/gbtovjzgp.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://wap.fanxiaobao.xyz/Article/details/gkgqotgno.sHtML

[Q31] 分组后过滤
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwharhgit.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.share.fanxiaobao.xyz/Article/details/ghvpqlmxh.sHtML

[Q32] 分组拼接字符串
来源：http://wap.fanxiaobao.xyz/Article/details/gtszbzxwc.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://read.share.fanxiaobao.xyz/Article/details/gyblfpnid.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gndtyiedz.sHtML

[Q33] 多列分组
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyarnhujo.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://blog.fanxiaobao.xyz/Article/details/gdwpafuaa.sHtML

[Q34] 每组取第一条
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdnqgsocc.sHtML

SELECT * FROM (
来源：http://wap.fanxiaobao.xyz/Article/details/gwztxadcc.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://blog.fanxiaobao.xyz/Article/details/gylpxrzww.sHtML

) t WHERE rn = 1;
来源：http://www.share.fanxiaobao.xyz/Article/details/gmvzuaxvz.sHtML

[Q35] 内连接
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtytlujjx.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gobmmthcb.sHtML

[Q36] 左连接
来源：http://wap.fanxiaobao.xyz/Article/details/gorhenrvu.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://baike.fanxiaobao.xyz/Article/details/gvvttjiyt.sHtML

[Q37] 右连接
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzdpobdap.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmumroler.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://mobile.fanxiaobao.xyz/Article/details/gkbzniihd.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghtxipcfo.sHtML

[Q39] 自连接（查上下级）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/govyjsaez.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://wap.fanxiaobao.xyz/Article/details/ggzkmeuca.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://m.share.fanxiaobao.xyz/Article/details/gikovuyls.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://wap.fanxiaobao.xyz/Article/details/glsexjfgn.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://m.share.fanxiaobao.xyz/Article/details/gkofzxgyn.sHtML

[Q41] 多表连接
来源：http://blog.fanxiaobao.xyz/Article/details/gcvteeaod.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvmjqlbrg.sHtML

JOIN users u ON u.id = o.user_id
来源：http://mobile.fanxiaobao.xyz/Article/details/gvnprbfss.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://baike.fanxiaobao.xyz/Article/details/gwtxrnxdr.sHtML

[Q42] 连接条件附加过滤
来源：http://3g.fanxiaobao.xyz/Article/details/gfzfzdkei.sHtML

SELECT u.name, o.amount FROM users u
来源：http://mobile.fanxiaobao.xyz/Article/details/gftqiwyhg.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://m.share.fanxiaobao.xyz/Article/details/ggpeuekcy.sHtML

[Q43] 标量子查询
来源：http://m.share.fanxiaobao.xyz/Article/details/gmovskdmb.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggsaablfb.sHtML

[Q44] IN 子查询
来源：http://www.share.fanxiaobao.xyz/Article/details/gxupvadhh.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://wap.fanxiaobao.xyz/Article/details/gsaqhnzve.sHtML

[Q45] EXISTS 判断存在
来源：http://read.share.fanxiaobao.xyz/Article/details/gkislupvd.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gexgfodas.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://wap.fanxiaobao.xyz/Article/details/gilosnhpd.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.fanxiaobao.xyz/Article/details/gsikgdyza.sHtML

[Q47] 与平均值比较
来源：http://blog.fanxiaobao.xyz/Article/details/gpvyodxef.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://mobile.fanxiaobao.xyz/Article/details/gaspwhtpc.sHtML

[Q48] CTE 公用表表达式
来源：http://wap.fanxiaobao.xyz/Article/details/gybwxjjnx.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.share.fanxiaobao.xyz/Article/details/gxugadznd.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://3g.fanxiaobao.xyz/Article/details/gbtbzgyja.sHtML

[Q49] 更新单行
来源：http://mobile.fanxiaobao.xyz/Article/details/gdegutglz.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://read.share.fanxiaobao.xyz/Article/details/ghczaitag.sHtML

[Q50] 批量更新
来源：http://mobile.fanxiaobao.xyz/Article/details/gbopuqjam.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.share.fanxiaobao.xyz/Article/details/gbccuhdfv.sHtML

[Q51] 用子查询更新
来源：http://www.blog.fanxiaobao.xyz/Article/details/geoluqixr.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://m.share.fanxiaobao.xyz/Article/details/geltvyubu.sHtML

[Q52] 删除指定行
来源：http://baike.fanxiaobao.xyz/Article/details/gcokxtnmw.sHtML

DELETE FROM users WHERE id = 10;
来源：http://3g.fanxiaobao.xyz/Article/details/gqgezsxwk.sHtML

[Q53] 按条件删除
来源：http://m.share.fanxiaobao.xyz/Article/details/gunyouuvr.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://mobile.fanxiaobao.xyz/Article/details/gaknppcps.sHtML

[Q54] 清空表
来源：http://read.share.fanxiaobao.xyz/Article/details/gzhtndunf.sHtML

TRUNCATE TABLE logs;
来源：http://baike.fanxiaobao.xyz/Article/details/guvxpfnte.sHtML

[Q55] 排名（并列占位）
来源：http://3g.fanxiaobao.xyz/Article/details/govbnlioj.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://m.share.fanxiaobao.xyz/Article/details/gejugpyrb.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.share.fanxiaobao.xyz/Article/details/giedtpqgy.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://wap.fanxiaobao.xyz/Article/details/gjzjbjeiy.sHtML

[Q57] 行号
来源：http://baike.fanxiaobao.xyz/Article/details/gkvkjybuy.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gzstfmuip.sHtML

[Q58] 累计求和
来源：http://baike.fanxiaobao.xyz/Article/details/gzylvxind.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://3g.fanxiaobao.xyz/Article/details/gcnjaepyc.sHtML

[Q59] 分组内累计
来源：http://mobile.fanxiaobao.xyz/Article/details/goeswaapd.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://wap.fanxiaobao.xyz/Article/details/glnupqsdf.sHtML

[Q60] 取上一行 / 下一行
来源：http://blog.fanxiaobao.xyz/Article/details/gwzhifjfw.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://baike.fanxiaobao.xyz/Article/details/gccthcoeu.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvfjgffra.sHtML

[Q61] 移动平均
来源：http://www.share.fanxiaobao.xyz/Article/details/ggkproctr.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://m.share.fanxiaobao.xyz/Article/details/gdedexuxy.sHtML

[Q62] 分组占比
来源：http://blog.fanxiaobao.xyz/Article/details/ggjbrztjm.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://m.share.fanxiaobao.xyz/Article/details/grsignkey.sHtML

[Q63] 开启事务
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjlwckiur.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://mobile.fanxiaobao.xyz/Article/details/gyapudkvm.sHtML

[Q64] 提交事务
来源：http://wap.fanxiaobao.xyz/Article/details/ggrtcxswi.sHtML

COMMIT;
来源：http://m.share.fanxiaobao.xyz/Article/details/gtlhuqzdi.sHtML

[Q65] 回滚事务
来源：http://blog.fanxiaobao.xyz/Article/details/gipgtogry.sHtML

ROLLBACK;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqcxverma.sHtML

[Q66] 行锁查询
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtzmbqjjg.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://read.share.fanxiaobao.xyz/Article/details/gmmcqjrns.sHtML

[Q67] 设置隔离级别
来源：http://baike.fanxiaobao.xyz/Article/details/ghzmzlaaz.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.share.fanxiaobao.xyz/Article/details/gcfqzrncq.sHtML

[Q68] 保存点
来源：http://mobile.fanxiaobao.xyz/Article/details/gmqgrfexd.sHtML

SAVEPOINT sp1;
来源：http://blog.fanxiaobao.xyz/Article/details/gxhyncobz.sHtML

ROLLBACK TO sp1;
来源：http://m.share.fanxiaobao.xyz/Article/details/guodpqxvk.sHtML

[Q69] 查看执行计划
来源：http://baike.fanxiaobao.xyz/Article/details/getlglzof.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://3g.fanxiaobao.xyz/Article/details/gmgwphvhc.sHtML

[Q70] 更新统计信息
来源：http://baike.fanxiaobao.xyz/Article/details/gvdsvfbar.sHtML

ANALYZE TABLE users;
来源：http://baike.fanxiaobao.xyz/Article/details/glmjecjlj.sHtML

[Q71] 查看建表语句
来源：http://m.share.fanxiaobao.xyz/Article/details/gtemelfye.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://read.share.fanxiaobao.xyz/Article/details/gkgglmnbj.sHtML

[Q72] 查看索引
来源：http://mobile.fanxiaobao.xyz/Article/details/gzkvusfrd.sHtML

SHOW INDEX FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/goceedhox.sHtML

[Q73] 查看表状态
来源：http://baike.fanxiaobao.xyz/Article/details/gshqybgfy.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmltlssxq.sHtML

[Q74] 强制使用索引
来源：http://m.share.fanxiaobao.xyz/Article/details/ghrsatvjl.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://wap.fanxiaobao.xyz/Article/details/gboppthyq.sHtML

[Q75] 日期格式化
来源：http://baike.fanxiaobao.xyz/Article/details/gnpysumxa.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://blog.fanxiaobao.xyz/Article/details/ggrxfnnlm.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://baike.fanxiaobao.xyz/Article/details/gibmnixhw.sHtML

[Q76] 按天统计
来源：http://www.share.fanxiaobao.xyz/Article/details/gpqfhwary.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gihogysxh.sHtML

[Q77] 时间加减
来源：http://baike.fanxiaobao.xyz/Article/details/ginzvvmxb.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://wap.fanxiaobao.xyz/Article/details/grvaldyao.sHtML

[Q78] 当前时间
来源：http://www.share.fanxiaobao.xyz/Article/details/ggmzlisva.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.share.fanxiaobao.xyz/Article/details/gixkmyzkx.sHtML

[Q79] 字符串拼接
来源：http://3g.fanxiaobao.xyz/Article/details/gumpjnzdv.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://mobile.fanxiaobao.xyz/Article/details/gyzqozhtm.sHtML

[Q80] 字符串截取
来源：http://read.share.fanxiaobao.xyz/Article/details/ghrngqoqr.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/geqqttgca.sHtML

[Q81] 字符串替换
来源：http://mobile.fanxiaobao.xyz/Article/details/gdahmjxos.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gbvnzuxbk.sHtML

[Q82] 字符长度与字节长度
来源：http://3g.fanxiaobao.xyz/Article/details/guvfmzpoa.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gijpnzfhf.sHtML

[Q83] 大小写转换
来源：http://www.blog.fanxiaobao.xyz/Article/details/grqyjczdl.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gupfvccjy.sHtML

[Q84] 去除首尾空格
来源：http://blog.fanxiaobao.xyz/Article/details/guikdnpac.sHtML

SELECT TRIM(name) FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gevunosbt.sHtML

[Q85] 数值取整
来源：http://read.share.fanxiaobao.xyz/Article/details/gmtcgonkk.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://3g.fanxiaobao.xyz/Article/details/gxrhogrjy.sHtML

[Q86] 读取 JSON 字段
来源：http://m.share.fanxiaobao.xyz/Article/details/gzpgeogyx.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://blog.fanxiaobao.xyz/Article/details/goxwxsakg.sHtML

[Q87] JSON 字段做条件
来源：http://baike.fanxiaobao.xyz/Article/details/glfnobzfk.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://m.share.fanxiaobao.xyz/Article/details/gwosatbac.sHtML

[Q88] 行转列（条件聚合）
来源：http://3g.fanxiaobao.xyz/Article/details/gjkncqkje.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://read.share.fanxiaobao.xyz/Article/details/gltiemxvb.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxcodeuqh.sHtML

[Q89] 判断表是否存在
来源：http://blog.fanxiaobao.xyz/Article/details/gmbhkwrmn.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://wap.fanxiaobao.xyz/Article/details/gcidcofpn.sHtML

[Q90] 生成序号列
来源：http://blog.fanxiaobao.xyz/Article/details/gfugjaxtg.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://blog.fanxiaobao.xyz/Article/details/gaogvadqw.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqbnimubc.sHtML

R. Bash 专题
来源：http://blog.fanxiaobao.xyz/Article/details/gzzoxocuv.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gipkbyswl.sHtML

[R01] shebang 与严格模式
来源：http://3g.fanxiaobao.xyz/Article/details/gujzitaff.sHtML

#!/usr/bin/env bash
来源：http://m.share.fanxiaobao.xyz/Article/details/gexnpknot.sHtML

set -euo pipefail
来源：http://3g.fanxiaobao.xyz/Article/details/gmwtsdkcz.sHtML

[R02] 变量赋值与使用
来源：http://www.share.fanxiaobao.xyz/Article/details/gnzvzuvug.sHtML

name="Tom"; echo "$name"
来源：http://www.blog.fanxiaobao.xyz/Article/details/grvbpljwl.sHtML

[R03] 只读变量
来源：http://read.share.fanxiaobao.xyz/Article/details/gpvdqjpjz.sHtML

readonly PI=3.14
来源：http://blog.fanxiaobao.xyz/Article/details/gjalfyfll.sHtML

[R04] 位置参数
来源：http://wap.fanxiaobao.xyz/Article/details/gelyqoaob.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://blog.fanxiaobao.xyz/Article/details/gdwjsphra.sHtML

[R05] 参数默认值
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsalladqf.sHtML

name="${1:-default}"
来源：http://baike.fanxiaobao.xyz/Article/details/gtpcfcbpd.sHtML

[R06] 判断命令是否存在
来源：http://blog.fanxiaobao.xyz/Article/details/gqmcomwnb.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gzarveyvd.sHtML

[R07] if 判断文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gmeppyhzg.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.share.fanxiaobao.xyz/Article/details/giclmqbpq.sHtML

[R08] 数值比较
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gugvcbdcq.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.share.fanxiaobao.xyz/Article/details/gljhistvh.sHtML

[R09] 字符串比较
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grqhvceyy.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://wap.fanxiaobao.xyz/Article/details/grvokasqq.sHtML

[R10] 正则匹配
来源：http://wap.fanxiaobao.xyz/Article/details/gqsatwxbm.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://baike.fanxiaobao.xyz/Article/details/gksxsflbx.sHtML

[R11] case 多分支
来源：http://wap.fanxiaobao.xyz/Article/details/guuxhgues.sHtML

case "$1" in
来源：http://blog.fanxiaobao.xyz/Article/details/gwokqwkhx.sHtML

start) echo "启动" ;;
来源：http://read.share.fanxiaobao.xyz/Article/details/glpbzjtra.sHtML

stop)  echo "停止" ;;
来源：http://mobile.fanxiaobao.xyz/Article/details/gdoquqoyb.sHtML

*)     echo "未知命令" ;;
来源：http://www.share.fanxiaobao.xyz/Article/details/gwawyfprl.sHtML

esac
来源：http://baike.fanxiaobao.xyz/Article/details/gmfwslaxe.sHtML

[R12] for 遍历文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gltlvngid.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.share.fanxiaobao.xyz/Article/details/guqmqktzp.sHtML

[R13] for 计数循环
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnysinjwx.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://read.share.fanxiaobao.xyz/Article/details/glhuwgmbz.sHtML

[R14] C 风格 for
来源：http://wap.fanxiaobao.xyz/Article/details/goszwgjij.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkdpomawo.sHtML

[R15] while 逐行读文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gscsmksoi.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gcgxchyhn.sHtML

[R16] until 等待条件
来源：http://blog.fanxiaobao.xyz/Article/details/gtfuulgjv.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://blog.fanxiaobao.xyz/Article/details/gnwluizfy.sHtML

[R17] 数组定义与取值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grjccqjsp.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://blog.fanxiaobao.xyz/Article/details/gpnyxntfo.sHtML

[R18] 遍历数组
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gogfiiwru.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gjtnptggu.sHtML

[R19] 数组长度
来源：http://www.blog.fanxiaobao.xyz/Article/details/goevgqctc.sHtML

echo "${#arr[@]}"
来源：http://baike.fanxiaobao.xyz/Article/details/gwvyzsiiv.sHtML

[R20] 关联数组（字典）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gremjfwty.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gypffcwvq.sHtML

[R21] 字符串长度
来源：http://www.share.fanxiaobao.xyz/Article/details/gumorfpfi.sHtML

echo "${#s}"
来源：http://blog.fanxiaobao.xyz/Article/details/gactenrzp.sHtML

[R22] 截取子串
来源：http://3g.fanxiaobao.xyz/Article/details/gcstyapid.sHtML

echo "${s:0:5}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gkolejric.sHtML

[R23] 字符串替换
来源：http://read.share.fanxiaobao.xyz/Article/details/ghroivhsj.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://3g.fanxiaobao.xyz/Article/details/gubbtunzn.sHtML

[R24] 大小写转换
来源：http://mobile.fanxiaobao.xyz/Article/details/gxquufdal.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://blog.fanxiaobao.xyz/Article/details/gsnbafwil.sHtML

[R25] 去后缀 / 去前缀
来源：http://wap.fanxiaobao.xyz/Article/details/ggkpzgguc.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://blog.fanxiaobao.xyz/Article/details/gqhtjdhsp.sHtML

[R26] 命令替换
来源：http://baike.fanxiaobao.xyz/Article/details/gcsywccev.sHtML

now=$(date +%F); echo "$now"
来源：http://3g.fanxiaobao.xyz/Article/details/gpmmqtbfr.sHtML

[R27] 算术展开
来源：http://www.blog.fanxiaobao.xyz/Article/details/gctvflikb.sHtML

echo $((1 + 2 * 3))
来源：http://m.share.fanxiaobao.xyz/Article/details/gzqvkdcrb.sHtML

[R28] 浮点运算
来源：http://read.share.fanxiaobao.xyz/Article/details/gchfhybxx.sHtML

echo "scale=2; 10/3" | bc
来源：http://m.share.fanxiaobao.xyz/Article/details/glrjqajfu.sHtML

[R29] 定义函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gaohguvdo.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggpmnnvaz.sHtML

[R30] 函数返回状态码
来源：http://wap.fanxiaobao.xyz/Article/details/glszchulp.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://baike.fanxiaobao.xyz/Article/details/giwhbwrgb.sHtML

[R31] 局部变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gadawkyau.sHtML


<!-- 参考信息 -->