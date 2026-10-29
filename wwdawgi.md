代发 wailian999

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://3g.zdbjq.cn/Article/details/gbtecvscy.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://mobile.hesvh.cn/Article/details/ggdqenupt.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://read.share.fehbvm.com/Article/details/gmwmgihft.sHtML

PHP:  if (empty($x)) {}
来源：http://wap.hesvh.cn/Article/details/gvgncyqjq.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://baike.zdbjq.cn/Article/details/gywlgdclv.sHtML

TS:   if (x == null) {}
来源：http://blog.hesvh.cn/Article/details/gdumdqslc.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://baike.fehbvm.com/Article/details/gxyjljczz.sHtML

Go:   if x == nil {}
来源：http://www.blog.hesvh.cn/Article/details/geoupgqnq.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://blog.fehbvm.com/Article/details/gglmonvyq.sHtML

C#:   if (x is null) {}
来源：http://m.share.hesvh.cn/Article/details/glxecslql.sHtML

[P07] 防抖与节流
来源：http://www.share.zdbjq.cn/Article/details/gusejixjf.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://read.share.hesvh.cn/Article/details/gdjofbapt.sHtML

PHP:  // 手写时间戳比较
来源：http://www.m.share.zdbjq.cn/Article/details/gdutaznwk.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.zdbjq.cn/Article/details/gvurjzknu.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.zdbjq.cn/Article/details/gtuqyephr.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://mobile.zdbjq.cn/Article/details/gdqcfryiy.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://m.share.hesvh.cn/Article/details/gvizhwjnc.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.m.share.fehbvm.com/Article/details/ggcsprvkq.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://3g.zdbjq.cn/Article/details/gacszzmzh.sHtML

[P08] 处理浮点精度问题
来源：http://www.m.share.fehbvm.com/Article/details/gxxmerels.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://wap.hesvh.cn/Article/details/gjpnmcwkw.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://read.share.hesvh.cn/Article/details/ggsajncyq.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://wap.fehbvm.com/Article/details/gfoszeblt.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://blog.zdbjq.cn/Article/details/gkgmrrcpz.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.blog.fehbvm.com/Article/details/gnxfiygvr.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://baike.hesvh.cn/Article/details/ggmerlqoz.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://read.share.zdbjq.cn/Article/details/gjsbqvztk.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.share.zdbjq.cn/Article/details/gdzcqdxap.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gukxkqxdb.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://blog.hesvh.cn/Article/details/gasiopcso.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gmsekpuec.sHtML

[Q01] 创建表
来源：http://read.share.zdbjq.cn/Article/details/gpyghgpar.sHtML

CREATE TABLE users (
来源：http://read.share.zdbjq.cn/Article/details/gakvlmnhe.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.hesvh.cn/Article/details/gkrpmbrix.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.m.share.hesvh.cn/Article/details/gmpdifais.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.share.zdbjq.cn/Article/details/gxnqpvlsr.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://3g.zdbjq.cn/Article/details/gdhvtoipx.sHtML

);
来源：http://www.share.zdbjq.cn/Article/details/gdipdiqwb.sHtML

[Q02] 创建带外键的表
来源：http://m.share.zdbjq.cn/Article/details/gdopzmaok.sHtML

CREATE TABLE orders (
来源：http://www.blog.hesvh.cn/Article/details/gopvwosei.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.zdbjq.cn/Article/details/gorzoclmh.sHtML

user_id INT NOT NULL,
来源：http://read.share.zdbjq.cn/Article/details/gyrvjugvx.sHtML

amount DECIMAL(10, 2),
来源：http://www.share.zdbjq.cn/Article/details/gddrmdyvp.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.share.fehbvm.com/Article/details/goczqcnjh.sHtML

);
来源：http://blog.hesvh.cn/Article/details/gpuumchul.sHtML

[Q03] 增加列
来源：http://blog.fehbvm.com/Article/details/gyeqcttcx.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.share.zdbjq.cn/Article/details/gfpqejpyz.sHtML

[Q04] 修改列类型
来源：http://m.share.zdbjq.cn/Article/details/gedfjfnsl.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.blog.fehbvm.com/Article/details/gskjijmxq.sHtML

[Q05] 重命名列
来源：http://m.share.hesvh.cn/Article/details/gkllizbod.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://3g.zdbjq.cn/Article/details/gfivjxwdk.sHtML

[Q06] 删除列
来源：http://m.share.zdbjq.cn/Article/details/gybzceqdj.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.share.fehbvm.com/Article/details/gktvurary.sHtML

[Q07] 删除表
来源：http://www.share.hesvh.cn/Article/details/gonsgznry.sHtML

DROP TABLE IF EXISTS orders;
来源：http://mobile.hesvh.cn/Article/details/gbjqnfpwb.sHtML

[Q08] 创建普通索引
来源：http://www.m.share.fehbvm.com/Article/details/gxzfervpw.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.share.zdbjq.cn/Article/details/gdfhgdgop.sHtML

[Q09] 创建唯一索引
来源：http://baike.zdbjq.cn/Article/details/gepzeupbx.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://m.share.fehbvm.com/Article/details/gdykpuzsy.sHtML

[Q10] 插入单行
来源：http://m.share.hesvh.cn/Article/details/glwltidrr.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.blog.hesvh.cn/Article/details/gplficzgk.sHtML

[Q11] 一次插入多行
来源：http://www.blog.fehbvm.com/Article/details/grbivnvoq.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.share.fehbvm.com/Article/details/gnpihtayl.sHtML

[Q12] 插入后取自增 ID
来源：http://blog.zdbjq.cn/Article/details/gvtkxhtdn.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://baike.zdbjq.cn/Article/details/gxsdtyuqh.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://baike.zdbjq.cn/Article/details/gaebnfrrn.sHtML

[Q13] 忽略重复插入
来源：http://wap.hesvh.cn/Article/details/gyhxraksj.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://m.share.zdbjq.cn/Article/details/gnmumyxmz.sHtML

[Q14] 存在则更新（upsert）
来源：http://3g.fehbvm.com/Article/details/gmebfuxoj.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.blog.zdbjq.cn/Article/details/gpagpsstt.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.blog.fehbvm.com/Article/details/gtldkhnkq.sHtML

[Q15] 查询全部
来源：http://blog.hesvh.cn/Article/details/gtykrjgsa.sHtML

SELECT * FROM users;
来源：http://wap.fehbvm.com/Article/details/gkvsntifm.sHtML

[Q16] 查询指定列
来源：http://www.m.share.hesvh.cn/Article/details/gvcsvhjer.sHtML

SELECT id, name FROM users;
来源：http://baike.fehbvm.com/Article/details/gpanqcszy.sHtML

[Q17] 条件查询
来源：http://m.share.hesvh.cn/Article/details/gjfvdohjx.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://read.share.zdbjq.cn/Article/details/gsyepcxph.sHtML

[Q18] 模糊匹配
来源：http://www.share.fehbvm.com/Article/details/gyfzwuayy.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://baike.fehbvm.com/Article/details/gesngityr.sHtML

[Q19] 范围查询
来源：http://mobile.fehbvm.com/Article/details/glysjjwrn.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://read.share.fehbvm.com/Article/details/goetxepul.sHtML

[Q20] IN 列表
来源：http://mobile.zdbjq.cn/Article/details/gntnlbgei.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.share.zdbjq.cn/Article/details/gupmhqiiv.sHtML

[Q21] 空值判断
来源：http://blog.hesvh.cn/Article/details/ghcesxhiz.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.m.share.hesvh.cn/Article/details/golykofby.sHtML

[Q22] 排序
来源：http://m.share.zdbjq.cn/Article/details/gmgawydfc.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.blog.zdbjq.cn/Article/details/gqkaevulf.sHtML

[Q23] 分页
来源：http://www.share.fehbvm.com/Article/details/gzarvnxah.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://3g.fehbvm.com/Article/details/gcyxftjvd.sHtML

[Q24] 去重
来源：http://wap.zdbjq.cn/Article/details/gppplcdvt.sHtML

SELECT DISTINCT city FROM users;
来源：http://mobile.hesvh.cn/Article/details/grqnlkrae.sHtML

[Q25] 只取前 N 条
来源：http://read.share.zdbjq.cn/Article/details/gnasyoujv.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.share.fehbvm.com/Article/details/gigypunqa.sHtML

[Q26] 计数
来源：http://www.share.hesvh.cn/Article/details/gufubotpu.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gqwhliphk.sHtML

[Q27] 条件计数
来源：http://3g.hesvh.cn/Article/details/gqtcxpdra.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://mobile.hesvh.cn/Article/details/gksujclwf.sHtML

[Q28] 求和与平均
来源：http://mobile.hesvh.cn/Article/details/gshmcrylj.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.blog.fehbvm.com/Article/details/gngyylfct.sHtML

[Q29] 最大最小值
来源：http://www.share.fehbvm.com/Article/details/gyzwdqwbm.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://wap.fehbvm.com/Article/details/graajipvt.sHtML

[Q30] 分组统计
来源：http://3g.fehbvm.com/Article/details/gxoajxfnj.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.m.share.fehbvm.com/Article/details/gjahmsowr.sHtML

[Q31] 分组后过滤
来源：http://www.share.fehbvm.com/Article/details/gnlyyjrrj.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://3g.zdbjq.cn/Article/details/gjrvceqoz.sHtML

[Q32] 分组拼接字符串
来源：http://baike.hesvh.cn/Article/details/gwywqdkic.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://blog.fehbvm.com/Article/details/gtgpfyzxr.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.m.share.fehbvm.com/Article/details/gkltsjesx.sHtML

[Q33] 多列分组
来源：http://3g.hesvh.cn/Article/details/gqoylfvzz.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://blog.fehbvm.com/Article/details/gbkmxhijm.sHtML

[Q34] 每组取第一条
来源：http://www.blog.hesvh.cn/Article/details/goiinhykj.sHtML

SELECT * FROM (
来源：http://www.share.zdbjq.cn/Article/details/gtlmsldau.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://mobile.zdbjq.cn/Article/details/gevikqahd.sHtML

) t WHERE rn = 1;
来源：http://3g.zdbjq.cn/Article/details/gxzntjdnt.sHtML

[Q35] 内连接
来源：http://wap.zdbjq.cn/Article/details/goksjyduq.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.fehbvm.com/Article/details/gonilpqws.sHtML

[Q36] 左连接
来源：http://www.share.hesvh.cn/Article/details/gvrupjunj.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://blog.hesvh.cn/Article/details/gtspjtyhs.sHtML

[Q37] 右连接
来源：http://wap.zdbjq.cn/Article/details/gdwhsjtpx.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://wap.zdbjq.cn/Article/details/gkemprbog.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.m.share.fehbvm.com/Article/details/gnsyynnim.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://m.share.zdbjq.cn/Article/details/gybsoocno.sHtML

[Q39] 自连接（查上下级）
来源：http://baike.zdbjq.cn/Article/details/gfwxgyeic.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.m.share.hesvh.cn/Article/details/ghxblniov.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://baike.zdbjq.cn/Article/details/guansyjuk.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://baike.hesvh.cn/Article/details/gmvzipvgf.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://wap.zdbjq.cn/Article/details/gjybxiyfe.sHtML

[Q41] 多表连接
来源：http://baike.fehbvm.com/Article/details/gqfgoofhi.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.share.fehbvm.com/Article/details/gybrmdjkd.sHtML

JOIN users u ON u.id = o.user_id
来源：http://m.share.fehbvm.com/Article/details/ghdtjsrno.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://read.share.zdbjq.cn/Article/details/gkjsodoev.sHtML

[Q42] 连接条件附加过滤
来源：http://baike.zdbjq.cn/Article/details/gdyalxvez.sHtML

SELECT u.name, o.amount FROM users u
来源：http://mobile.fehbvm.com/Article/details/gljgezczs.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://mobile.zdbjq.cn/Article/details/gqlfizmgo.sHtML

[Q43] 标量子查询
来源：http://read.share.zdbjq.cn/Article/details/gdvtbgtex.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://m.share.zdbjq.cn/Article/details/gbwlzlccu.sHtML

[Q44] IN 子查询
来源：http://mobile.hesvh.cn/Article/details/gydiwlzhj.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.m.share.zdbjq.cn/Article/details/gqmxsxmbv.sHtML

[Q45] EXISTS 判断存在
来源：http://blog.hesvh.cn/Article/details/galhgweaj.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.hesvh.cn/Article/details/gqhaoylai.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://wap.hesvh.cn/Article/details/gzbmyfueu.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.fehbvm.com/Article/details/gfhpoqxuf.sHtML

[Q47] 与平均值比较
来源：http://www.blog.hesvh.cn/Article/details/gpsjjrokk.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://mobile.fehbvm.com/Article/details/gomvhhfrc.sHtML

[Q48] CTE 公用表表达式
来源：http://blog.fehbvm.com/Article/details/gfyxqfrxd.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://mobile.hesvh.cn/Article/details/goftomzpq.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.share.fehbvm.com/Article/details/gaqqvtkva.sHtML

[Q49] 更新单行
来源：http://mobile.hesvh.cn/Article/details/glczxeafa.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://m.share.fehbvm.com/Article/details/gpjdbilgs.sHtML

[Q50] 批量更新
来源：http://www.share.hesvh.cn/Article/details/gbwfkipoh.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://baike.hesvh.cn/Article/details/gdjytpmxr.sHtML

[Q51] 用子查询更新
来源：http://baike.zdbjq.cn/Article/details/gfhemiany.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://baike.hesvh.cn/Article/details/gzelttqas.sHtML

[Q52] 删除指定行
来源：http://www.m.share.fehbvm.com/Article/details/ggjovwtqx.sHtML

DELETE FROM users WHERE id = 10;
来源：http://read.share.fehbvm.com/Article/details/gngdnyvok.sHtML

[Q53] 按条件删除
来源：http://blog.fehbvm.com/Article/details/gzllynsif.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.m.share.zdbjq.cn/Article/details/gldppzmqw.sHtML

[Q54] 清空表
来源：http://3g.fehbvm.com/Article/details/gefaozvpu.sHtML

TRUNCATE TABLE logs;
来源：http://baike.hesvh.cn/Article/details/gxasrobxw.sHtML

[Q55] 排名（并列占位）
来源：http://blog.zdbjq.cn/Article/details/gmgixisjh.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.blog.zdbjq.cn/Article/details/goagwqcqb.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.m.share.fehbvm.com/Article/details/gjvzyhwvt.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://baike.fehbvm.com/Article/details/glewfhahd.sHtML

[Q57] 行号
来源：http://www.m.share.fehbvm.com/Article/details/glcqyjpix.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gdeozzuly.sHtML

[Q58] 累计求和
来源：http://mobile.hesvh.cn/Article/details/gyyinprzw.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://mobile.fehbvm.com/Article/details/gdoabuwuw.sHtML

[Q59] 分组内累计
来源：http://3g.fehbvm.com/Article/details/gldjzellr.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://baike.zdbjq.cn/Article/details/gfkxdwatp.sHtML

[Q60] 取上一行 / 下一行
来源：http://wap.fehbvm.com/Article/details/gcsoxqznn.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://read.share.hesvh.cn/Article/details/gbdfllojf.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://wap.hesvh.cn/Article/details/gfvhedogj.sHtML

[Q61] 移动平均
来源：http://www.share.fehbvm.com/Article/details/gzdphgptg.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.blog.hesvh.cn/Article/details/gbksxjrvs.sHtML

[Q62] 分组占比
来源：http://www.share.fehbvm.com/Article/details/glzhhngen.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://read.share.hesvh.cn/Article/details/gehsscuxx.sHtML

[Q63] 开启事务
来源：http://www.share.zdbjq.cn/Article/details/gdybdegin.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://m.share.fehbvm.com/Article/details/gdhvjniyv.sHtML

[Q64] 提交事务
来源：http://www.share.hesvh.cn/Article/details/gjcmqmijp.sHtML

COMMIT;
来源：http://blog.hesvh.cn/Article/details/gyfncoltd.sHtML

[Q65] 回滚事务
来源：http://read.share.fehbvm.com/Article/details/gxgvmatku.sHtML

ROLLBACK;
来源：http://www.share.zdbjq.cn/Article/details/gqmkgclja.sHtML

[Q66] 行锁查询
来源：http://wap.zdbjq.cn/Article/details/gwjjyfxnj.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://wap.fehbvm.com/Article/details/gyprkwwyu.sHtML

[Q67] 设置隔离级别
来源：http://blog.fehbvm.com/Article/details/gpmywwmpr.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://mobile.zdbjq.cn/Article/details/gjdpzqgpb.sHtML

[Q68] 保存点
来源：http://read.share.zdbjq.cn/Article/details/gfyosqjih.sHtML

SAVEPOINT sp1;
来源：http://www.m.share.hesvh.cn/Article/details/gxjuhoidb.sHtML

ROLLBACK TO sp1;
来源：http://baike.hesvh.cn/Article/details/gskfonodx.sHtML

[Q69] 查看执行计划
来源：http://wap.zdbjq.cn/Article/details/gcrqpfbom.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://blog.zdbjq.cn/Article/details/gnexihqkn.sHtML

[Q70] 更新统计信息
来源：http://www.blog.zdbjq.cn/Article/details/glzudzkpn.sHtML

ANALYZE TABLE users;
来源：http://blog.fehbvm.com/Article/details/guvdfarzd.sHtML

[Q71] 查看建表语句
来源：http://m.share.fehbvm.com/Article/details/gzcicjygp.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.m.share.hesvh.cn/Article/details/ggtttxudc.sHtML

[Q72] 查看索引
来源：http://www.m.share.fehbvm.com/Article/details/gtonalzgd.sHtML

SHOW INDEX FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gwstlsxfi.sHtML

[Q73] 查看表状态
来源：http://www.blog.fehbvm.com/Article/details/glgcfkkfz.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://3g.hesvh.cn/Article/details/gycjbmskh.sHtML

[Q74] 强制使用索引
来源：http://read.share.zdbjq.cn/Article/details/gdehfeqen.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://blog.hesvh.cn/Article/details/gxmjqbjds.sHtML

[Q75] 日期格式化
来源：http://mobile.hesvh.cn/Article/details/gosxlbzps.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://baike.fehbvm.com/Article/details/glytaxpon.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://baike.zdbjq.cn/Article/details/gtfkwwxji.sHtML

[Q76] 按天统计
来源：http://baike.fehbvm.com/Article/details/gkrfgzyix.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.blog.hesvh.cn/Article/details/gnsyxuadh.sHtML

[Q77] 时间加减
来源：http://read.share.fehbvm.com/Article/details/gipsmdznp.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://3g.fehbvm.com/Article/details/gbepatcpe.sHtML

[Q78] 当前时间
来源：http://www.blog.hesvh.cn/Article/details/gvnhjfyvz.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://m.share.hesvh.cn/Article/details/gmehvptsk.sHtML

[Q79] 字符串拼接
来源：http://baike.fehbvm.com/Article/details/gvagdqava.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://m.share.zdbjq.cn/Article/details/gcohctxkk.sHtML

[Q80] 字符串截取
来源：http://read.share.fehbvm.com/Article/details/guplajljf.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gmqtirmpv.sHtML

[Q81] 字符串替换
来源：http://mobile.zdbjq.cn/Article/details/gxogdyxfv.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://read.share.zdbjq.cn/Article/details/giwpgelrs.sHtML

[Q82] 字符长度与字节长度
来源：http://www.blog.fehbvm.com/Article/details/gsvxkmfod.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://wap.zdbjq.cn/Article/details/gflkkvrfq.sHtML

[Q83] 大小写转换
来源：http://baike.fehbvm.com/Article/details/gjzxteeli.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://mobile.fehbvm.com/Article/details/glsczopxo.sHtML

[Q84] 去除首尾空格
来源：http://www.blog.fehbvm.com/Article/details/guxerhdud.sHtML

SELECT TRIM(name) FROM users;
来源：http://baike.hesvh.cn/Article/details/gzswnwyjq.sHtML

[Q85] 数值取整
来源：http://www.m.share.zdbjq.cn/Article/details/gjapbwnbk.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://blog.fehbvm.com/Article/details/ghrkkutvy.sHtML

[Q86] 读取 JSON 字段
来源：http://wap.hesvh.cn/Article/details/grrkdxeyg.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://mobile.zdbjq.cn/Article/details/gplbkmmuc.sHtML

[Q87] JSON 字段做条件
来源：http://mobile.zdbjq.cn/Article/details/glnpdoqud.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://m.share.fehbvm.com/Article/details/gbnqmfphz.sHtML

[Q88] 行转列（条件聚合）
来源：http://blog.fehbvm.com/Article/details/gjxohajql.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://blog.hesvh.cn/Article/details/gvloklufr.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gsbjpijsu.sHtML

[Q89] 判断表是否存在
来源：http://www.m.share.zdbjq.cn/Article/details/gjqusmlob.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.share.fehbvm.com/Article/details/gghtycuru.sHtML

[Q90] 生成序号列
来源：http://m.share.fehbvm.com/Article/details/gntutvccx.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://wap.hesvh.cn/Article/details/gtamempjt.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/golxdkwng.sHtML

R. Bash 专题
来源：http://blog.fehbvm.com/Article/details/glvicylyl.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gnizkvjqz.sHtML

[R01] shebang 与严格模式
来源：http://3g.hesvh.cn/Article/details/gzzhzxtug.sHtML

#!/usr/bin/env bash
来源：http://www.share.fehbvm.com/Article/details/glghuurgg.sHtML

set -euo pipefail
来源：http://m.share.zdbjq.cn/Article/details/ggkzwbmxd.sHtML

[R02] 变量赋值与使用
来源：http://www.m.share.fehbvm.com/Article/details/gxcacnmyh.sHtML

name="Tom"; echo "$name"
来源：http://baike.zdbjq.cn/Article/details/ghdptlflb.sHtML

[R03] 只读变量
来源：http://3g.zdbjq.cn/Article/details/gcsezgsyk.sHtML

readonly PI=3.14
来源：http://blog.hesvh.cn/Article/details/gskwxujgp.sHtML

[R04] 位置参数
来源：http://read.share.hesvh.cn/Article/details/gctytfcng.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://wap.fehbvm.com/Article/details/gotqvtaql.sHtML

[R05] 参数默认值
来源：http://baike.fehbvm.com/Article/details/gagmddkta.sHtML

name="${1:-default}"
来源：http://mobile.hesvh.cn/Article/details/gpvhyyqdg.sHtML

[R06] 判断命令是否存在
来源：http://m.share.fehbvm.com/Article/details/gdsafmlyr.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://mobile.zdbjq.cn/Article/details/gynfwrsgc.sHtML

[R07] if 判断文件
来源：http://blog.fehbvm.com/Article/details/gypwiuktk.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://mobile.zdbjq.cn/Article/details/gmhiecxfs.sHtML

[R08] 数值比较
来源：http://wap.hesvh.cn/Article/details/gnqselcoh.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://blog.hesvh.cn/Article/details/gsozqarhq.sHtML

[R09] 字符串比较
来源：http://www.share.zdbjq.cn/Article/details/gcatuwtvb.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://baike.zdbjq.cn/Article/details/ghgefeyho.sHtML

[R10] 正则匹配
来源：http://m.share.zdbjq.cn/Article/details/gaydusfdh.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://baike.zdbjq.cn/Article/details/gkzjonzhe.sHtML

[R11] case 多分支
来源：http://www.share.fehbvm.com/Article/details/gzimdyvfv.sHtML

case "$1" in
来源：http://www.m.share.fehbvm.com/Article/details/gwyntkvft.sHtML

start) echo "启动" ;;
来源：http://www.m.share.fehbvm.com/Article/details/gstptkubp.sHtML

stop)  echo "停止" ;;
来源：http://www.blog.fehbvm.com/Article/details/gehlrkjlf.sHtML

*)     echo "未知命令" ;;
来源：http://m.share.hesvh.cn/Article/details/gdjnisxkl.sHtML

esac
来源：http://www.blog.hesvh.cn/Article/details/gtcqzjlxs.sHtML

[R12] for 遍历文件
来源：http://read.share.fehbvm.com/Article/details/garsbccyk.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.blog.hesvh.cn/Article/details/gvekrxitt.sHtML

[R13] for 计数循环
来源：http://3g.hesvh.cn/Article/details/gvcvvkbox.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://3g.fehbvm.com/Article/details/gptebliid.sHtML

[R14] C 风格 for
来源：http://www.m.share.hesvh.cn/Article/details/gghvcnyel.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://mobile.zdbjq.cn/Article/details/guvjbnrzi.sHtML

[R15] while 逐行读文件
来源：http://read.share.fehbvm.com/Article/details/gjdpixwdn.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.m.share.zdbjq.cn/Article/details/gmgpsdtdn.sHtML

[R16] until 等待条件
来源：http://3g.hesvh.cn/Article/details/gepxiqepb.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://mobile.zdbjq.cn/Article/details/ghcyehbsa.sHtML

[R17] 数组定义与取值
来源：http://3g.hesvh.cn/Article/details/gplrbpzcu.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://blog.zdbjq.cn/Article/details/gqcvkbhlj.sHtML

[R18] 遍历数组
来源：http://www.blog.zdbjq.cn/Article/details/ggpobbrah.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://mobile.hesvh.cn/Article/details/gkreqouap.sHtML

[R19] 数组长度
来源：http://blog.fehbvm.com/Article/details/gllkqoypl.sHtML

echo "${#arr[@]}"
来源：http://read.share.hesvh.cn/Article/details/ggcilpsaj.sHtML

[R20] 关联数组（字典）
来源：http://3g.fehbvm.com/Article/details/gxffnhekh.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://mobile.hesvh.cn/Article/details/gdwmbrjjs.sHtML

[R21] 字符串长度
来源：http://www.share.fehbvm.com/Article/details/gxshfqigi.sHtML

echo "${#s}"
来源：http://www.m.share.zdbjq.cn/Article/details/gmpbugpxq.sHtML

[R22] 截取子串
来源：http://3g.fehbvm.com/Article/details/glqhmdqlz.sHtML

echo "${s:0:5}"
来源：http://www.m.share.hesvh.cn/Article/details/gniajydfd.sHtML

[R23] 字符串替换
来源：http://mobile.hesvh.cn/Article/details/grecaejzl.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.share.hesvh.cn/Article/details/gywfsdmgm.sHtML

[R24] 大小写转换
来源：http://www.blog.zdbjq.cn/Article/details/gyydhlerm.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://3g.hesvh.cn/Article/details/giaapgkpl.sHtML

[R25] 去后缀 / 去前缀
来源：http://blog.hesvh.cn/Article/details/gtrknxkel.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.m.share.hesvh.cn/Article/details/gjaflczkf.sHtML

[R26] 命令替换
来源：http://mobile.zdbjq.cn/Article/details/gxixvwtbu.sHtML

now=$(date +%F); echo "$now"
来源：http://www.m.share.zdbjq.cn/Article/details/gzrkeakca.sHtML

[R27] 算术展开
来源：http://www.m.share.zdbjq.cn/Article/details/gfxdydjyi.sHtML

echo $((1 + 2 * 3))
来源：http://m.share.zdbjq.cn/Article/details/gmovpydsg.sHtML

[R28] 浮点运算
来源：http://mobile.zdbjq.cn/Article/details/gwsvishlc.sHtML

echo "scale=2; 10/3" | bc
来源：http://m.share.zdbjq.cn/Article/details/gvvjsrkjm.sHtML

[R29] 定义函数
来源：http://baike.hesvh.cn/Article/details/gzqgheeyq.sHtML


<!-- 参考信息 -->