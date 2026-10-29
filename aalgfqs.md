代发 wailian999

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://wap.zdbjq.cn/Article/details/gtufmbaqw.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://wap.fehbvm.com/Article/details/gjtxkkkau.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://baike.fehbvm.com/Article/details/gargovytv.sHtML

PHP:  if (empty($x)) {}
来源：http://blog.fehbvm.com/Article/details/gisgrgyyj.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://m.share.hesvh.cn/Article/details/ghebhkddk.sHtML

TS:   if (x == null) {}
来源：http://www.share.zdbjq.cn/Article/details/gixhltfqo.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.m.share.hesvh.cn/Article/details/gpdwlokrz.sHtML

Go:   if x == nil {}
来源：http://wap.fehbvm.com/Article/details/gaejrrkbp.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://read.share.hesvh.cn/Article/details/gjmmtqktg.sHtML

C#:   if (x is null) {}
来源：http://baike.zdbjq.cn/Article/details/gtfybelgw.sHtML

[P07] 防抖与节流
来源：http://wap.hesvh.cn/Article/details/gpokfycxu.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://blog.fehbvm.com/Article/details/gkxqnuewm.sHtML

PHP:  // 手写时间戳比较
来源：http://www.share.fehbvm.com/Article/details/gwuzkwbrl.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.fehbvm.com/Article/details/gspqldtrv.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.hesvh.cn/Article/details/gspozjsyc.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://baike.zdbjq.cn/Article/details/gwjmozycq.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://3g.fehbvm.com/Article/details/gqlhtkazr.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.share.fehbvm.com/Article/details/gqobsxcly.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.blog.zdbjq.cn/Article/details/glpzvpmvh.sHtML

[P08] 处理浮点精度问题
来源：http://3g.fehbvm.com/Article/details/gztgcnipq.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://baike.fehbvm.com/Article/details/gdfggkaso.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.share.fehbvm.com/Article/details/gcoxxgdia.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.m.share.fehbvm.com/Article/details/gmnyzrkcl.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.blog.fehbvm.com/Article/details/gtfldtvzr.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.m.share.hesvh.cn/Article/details/gineqjike.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://mobile.fehbvm.com/Article/details/giwgikfpp.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://m.share.hesvh.cn/Article/details/gsddsislv.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.share.zdbjq.cn/Article/details/gvcwiqdiu.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gvfsryohl.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://blog.hesvh.cn/Article/details/gvneogyvx.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gkwpyyhjf.sHtML

[Q01] 创建表
来源：http://m.share.fehbvm.com/Article/details/gfhhbkvyo.sHtML

CREATE TABLE users (
来源：http://baike.zdbjq.cn/Article/details/glkmlwlhz.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.fehbvm.com/Article/details/gbnwyhkee.sHtML

name VARCHAR(50) NOT NULL,
来源：http://blog.hesvh.cn/Article/details/geqpiyrbz.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.share.hesvh.cn/Article/details/gzfxxmhby.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.m.share.fehbvm.com/Article/details/gicceylog.sHtML

);
来源：http://m.share.zdbjq.cn/Article/details/goqcejcyr.sHtML

[Q02] 创建带外键的表
来源：http://read.share.fehbvm.com/Article/details/guttxixsk.sHtML

CREATE TABLE orders (
来源：http://3g.zdbjq.cn/Article/details/glbxmxgyk.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.zdbjq.cn/Article/details/gaqwlwrvl.sHtML

user_id INT NOT NULL,
来源：http://wap.hesvh.cn/Article/details/gozxlbxqs.sHtML

amount DECIMAL(10, 2),
来源：http://blog.fehbvm.com/Article/details/gxipbozdd.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://read.share.zdbjq.cn/Article/details/gpttlfrvt.sHtML

);
来源：http://www.m.share.fehbvm.com/Article/details/gabbjlgvs.sHtML

[Q03] 增加列
来源：http://read.share.hesvh.cn/Article/details/ggxdmnqai.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://blog.fehbvm.com/Article/details/gzoxdwwff.sHtML

[Q04] 修改列类型
来源：http://m.share.zdbjq.cn/Article/details/gcahuhbip.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://m.share.zdbjq.cn/Article/details/gfisndvrs.sHtML

[Q05] 重命名列
来源：http://baike.zdbjq.cn/Article/details/gmlwqsrxk.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://wap.fehbvm.com/Article/details/gdjpchvcs.sHtML

[Q06] 删除列
来源：http://read.share.zdbjq.cn/Article/details/grjezdmij.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://read.share.hesvh.cn/Article/details/gaeeontee.sHtML

[Q07] 删除表
来源：http://3g.hesvh.cn/Article/details/gfgmyvgth.sHtML

DROP TABLE IF EXISTS orders;
来源：http://blog.hesvh.cn/Article/details/glavdkdml.sHtML

[Q08] 创建普通索引
来源：http://m.share.fehbvm.com/Article/details/gjfpfwryi.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://baike.hesvh.cn/Article/details/gczshvcpj.sHtML

[Q09] 创建唯一索引
来源：http://3g.zdbjq.cn/Article/details/gourkcjcu.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://baike.zdbjq.cn/Article/details/gsvzclkss.sHtML

[Q10] 插入单行
来源：http://m.share.zdbjq.cn/Article/details/gkoncoxmk.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.share.fehbvm.com/Article/details/gzfnthevf.sHtML

[Q11] 一次插入多行
来源：http://wap.zdbjq.cn/Article/details/gfzcuataz.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://blog.zdbjq.cn/Article/details/gklqxyauj.sHtML

[Q12] 插入后取自增 ID
来源：http://m.share.hesvh.cn/Article/details/gqbjxtail.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.m.share.fehbvm.com/Article/details/gvgxeajjs.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://mobile.zdbjq.cn/Article/details/gxkotyyxh.sHtML

[Q13] 忽略重复插入
来源：http://www.share.zdbjq.cn/Article/details/gvxfnxoyp.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://read.share.hesvh.cn/Article/details/gorbyxhef.sHtML

[Q14] 存在则更新（upsert）
来源：http://mobile.fehbvm.com/Article/details/gdrbbakjd.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://read.share.zdbjq.cn/Article/details/gsfvzrydu.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://mobile.zdbjq.cn/Article/details/gbuhsfjtl.sHtML

[Q15] 查询全部
来源：http://www.blog.fehbvm.com/Article/details/gdwsohkeb.sHtML

SELECT * FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gxgkfcwfq.sHtML

[Q16] 查询指定列
来源：http://www.m.share.fehbvm.com/Article/details/gsdmjdmpr.sHtML

SELECT id, name FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gnwwcezyc.sHtML

[Q17] 条件查询
来源：http://www.share.zdbjq.cn/Article/details/gkxqklpsh.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://m.share.hesvh.cn/Article/details/gofhzdwlh.sHtML

[Q18] 模糊匹配
来源：http://blog.zdbjq.cn/Article/details/gzfklrjzi.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://read.share.fehbvm.com/Article/details/gsledushg.sHtML

[Q19] 范围查询
来源：http://mobile.zdbjq.cn/Article/details/gcxnzmpuu.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://blog.fehbvm.com/Article/details/gsiddjgtm.sHtML

[Q20] IN 列表
来源：http://mobile.fehbvm.com/Article/details/gavtqoudw.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://wap.fehbvm.com/Article/details/gohmfkdty.sHtML

[Q21] 空值判断
来源：http://baike.zdbjq.cn/Article/details/gclyixswv.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.share.zdbjq.cn/Article/details/ggcqsijdm.sHtML

[Q22] 排序
来源：http://wap.fehbvm.com/Article/details/gffxcvnvw.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://3g.fehbvm.com/Article/details/ghmzfwoqa.sHtML

[Q23] 分页
来源：http://www.m.share.hesvh.cn/Article/details/ggcsegozx.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://m.share.zdbjq.cn/Article/details/gwnflpimz.sHtML

[Q24] 去重
来源：http://www.m.share.hesvh.cn/Article/details/gajswsdnd.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.share.fehbvm.com/Article/details/gbhuktbsw.sHtML

[Q25] 只取前 N 条
来源：http://www.m.share.fehbvm.com/Article/details/glwmkpxew.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://3g.hesvh.cn/Article/details/gnvuzxlig.sHtML

[Q26] 计数
来源：http://baike.fehbvm.com/Article/details/gabuajsfh.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gnksbleql.sHtML

[Q27] 条件计数
来源：http://www.blog.fehbvm.com/Article/details/gaazdpjnb.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gaqstxfir.sHtML

[Q28] 求和与平均
来源：http://m.share.zdbjq.cn/Article/details/ggxfcgjvl.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.m.share.zdbjq.cn/Article/details/gqdnzvvrw.sHtML

[Q29] 最大最小值
来源：http://3g.hesvh.cn/Article/details/gjohpvhph.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://blog.fehbvm.com/Article/details/gaismltow.sHtML

[Q30] 分组统计
来源：http://read.share.hesvh.cn/Article/details/gprwaudap.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.m.share.hesvh.cn/Article/details/gdlvsxnsv.sHtML

[Q31] 分组后过滤
来源：http://www.share.fehbvm.com/Article/details/goosbmmec.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://blog.hesvh.cn/Article/details/grcsrbpil.sHtML

[Q32] 分组拼接字符串
来源：http://read.share.fehbvm.com/Article/details/gltebnykt.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://3g.fehbvm.com/Article/details/gkrrxxnqj.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://baike.hesvh.cn/Article/details/gcmxzeowd.sHtML

[Q33] 多列分组
来源：http://blog.fehbvm.com/Article/details/ggfvykqwq.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.m.share.zdbjq.cn/Article/details/garjqretm.sHtML

[Q34] 每组取第一条
来源：http://mobile.zdbjq.cn/Article/details/ghbdweodi.sHtML

SELECT * FROM (
来源：http://baike.zdbjq.cn/Article/details/gegzpswvk.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://m.share.zdbjq.cn/Article/details/gedmbdzje.sHtML

) t WHERE rn = 1;
来源：http://blog.zdbjq.cn/Article/details/gexguzkjx.sHtML

[Q35] 内连接
来源：http://www.m.share.hesvh.cn/Article/details/glwtqqjiu.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://mobile.zdbjq.cn/Article/details/gdkhdauwp.sHtML

[Q36] 左连接
来源：http://baike.zdbjq.cn/Article/details/gsvvbnasy.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://mobile.hesvh.cn/Article/details/gkfchkrvb.sHtML

[Q37] 右连接
来源：http://m.share.zdbjq.cn/Article/details/gnjjdzziy.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://read.share.zdbjq.cn/Article/details/gbchbqjaw.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://3g.hesvh.cn/Article/details/ghepiiqpv.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.blog.hesvh.cn/Article/details/gfajroqok.sHtML

[Q39] 自连接（查上下级）
来源：http://www.blog.hesvh.cn/Article/details/gocmzrget.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.m.share.zdbjq.cn/Article/details/gvykhtcye.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.blog.zdbjq.cn/Article/details/gkrmxumkp.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://baike.fehbvm.com/Article/details/gtqbgurio.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://wap.zdbjq.cn/Article/details/gjmnuirwu.sHtML

[Q41] 多表连接
来源：http://baike.fehbvm.com/Article/details/gnrjxxaal.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://read.share.fehbvm.com/Article/details/gcntpsrqk.sHtML

JOIN users u ON u.id = o.user_id
来源：http://baike.fehbvm.com/Article/details/gwgwgbksn.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://3g.hesvh.cn/Article/details/gxhpqxkfo.sHtML

[Q42] 连接条件附加过滤
来源：http://3g.fehbvm.com/Article/details/gjwqcjzja.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.blog.zdbjq.cn/Article/details/gqxxptrmm.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.m.share.fehbvm.com/Article/details/grzofkimr.sHtML

[Q43] 标量子查询
来源：http://www.m.share.hesvh.cn/Article/details/gmbmmnnwm.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://3g.zdbjq.cn/Article/details/gcehiqcuv.sHtML

[Q44] IN 子查询
来源：http://read.share.zdbjq.cn/Article/details/gnifqxkjp.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://m.share.fehbvm.com/Article/details/gxdnxhxma.sHtML

[Q45] EXISTS 判断存在
来源：http://baike.hesvh.cn/Article/details/girqhrjeq.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.hesvh.cn/Article/details/gixrhkqyb.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.m.share.fehbvm.com/Article/details/gbyszryhq.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.hesvh.cn/Article/details/gmshhzwoa.sHtML

[Q47] 与平均值比较
来源：http://www.share.hesvh.cn/Article/details/gevvmsbds.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.share.fehbvm.com/Article/details/gnmegkehn.sHtML

[Q48] CTE 公用表表达式
来源：http://m.share.hesvh.cn/Article/details/gbqhmmoct.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://read.share.fehbvm.com/Article/details/gvntzlush.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://mobile.fehbvm.com/Article/details/geibgvtxg.sHtML

[Q49] 更新单行
来源：http://wap.fehbvm.com/Article/details/gcdddvrql.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.share.fehbvm.com/Article/details/gerbwtmcd.sHtML

[Q50] 批量更新
来源：http://www.m.share.zdbjq.cn/Article/details/gsekietln.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://wap.zdbjq.cn/Article/details/gpggzcarh.sHtML

[Q51] 用子查询更新
来源：http://wap.zdbjq.cn/Article/details/gaxmxznds.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://wap.zdbjq.cn/Article/details/geaxuwtzg.sHtML

[Q52] 删除指定行
来源：http://wap.fehbvm.com/Article/details/grplrwibx.sHtML

DELETE FROM users WHERE id = 10;
来源：http://blog.zdbjq.cn/Article/details/gefggqixy.sHtML

[Q53] 按条件删除
来源：http://m.share.fehbvm.com/Article/details/gleymtkpf.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://m.share.zdbjq.cn/Article/details/gbfitppiu.sHtML

[Q54] 清空表
来源：http://m.share.fehbvm.com/Article/details/gsanoadzv.sHtML

TRUNCATE TABLE logs;
来源：http://m.share.zdbjq.cn/Article/details/gcigmxcdl.sHtML

[Q55] 排名（并列占位）
来源：http://baike.hesvh.cn/Article/details/gvsqzmzmr.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://m.share.fehbvm.com/Article/details/grmwrvuxz.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.blog.fehbvm.com/Article/details/grecrjyba.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://wap.zdbjq.cn/Article/details/gsmmfdeml.sHtML

[Q57] 行号
来源：http://mobile.hesvh.cn/Article/details/gsjtfpnpf.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://wap.zdbjq.cn/Article/details/gzibrqlng.sHtML

[Q58] 累计求和
来源：http://blog.hesvh.cn/Article/details/gpiscgjay.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://blog.hesvh.cn/Article/details/gxenhhflk.sHtML

[Q59] 分组内累计
来源：http://mobile.zdbjq.cn/Article/details/gvxskdwdt.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://read.share.zdbjq.cn/Article/details/gxufwkapr.sHtML

[Q60] 取上一行 / 下一行
来源：http://mobile.fehbvm.com/Article/details/ghxwlswxh.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://read.share.fehbvm.com/Article/details/geqsljrcp.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.blog.fehbvm.com/Article/details/gstgxyvoh.sHtML

[Q61] 移动平均
来源：http://www.blog.hesvh.cn/Article/details/ggeneghad.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://mobile.fehbvm.com/Article/details/gsmglkorm.sHtML

[Q62] 分组占比
来源：http://www.m.share.hesvh.cn/Article/details/gxuaskxez.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://wap.fehbvm.com/Article/details/ghczoccos.sHtML

[Q63] 开启事务
来源：http://baike.zdbjq.cn/Article/details/gptbzqdcz.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://m.share.zdbjq.cn/Article/details/gnojeksoc.sHtML

[Q64] 提交事务
来源：http://mobile.zdbjq.cn/Article/details/gdnnyxggo.sHtML

COMMIT;
来源：http://read.share.zdbjq.cn/Article/details/gacubuerv.sHtML

[Q65] 回滚事务
来源：http://3g.hesvh.cn/Article/details/grnlgppwg.sHtML

ROLLBACK;
来源：http://www.blog.hesvh.cn/Article/details/gvteicrwo.sHtML

[Q66] 行锁查询
来源：http://blog.fehbvm.com/Article/details/gtlmukrnn.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.m.share.fehbvm.com/Article/details/guhvazoiy.sHtML

[Q67] 设置隔离级别
来源：http://3g.zdbjq.cn/Article/details/gbkytuodk.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.blog.hesvh.cn/Article/details/ghxokcste.sHtML

[Q68] 保存点
来源：http://blog.fehbvm.com/Article/details/gaydywhir.sHtML

SAVEPOINT sp1;
来源：http://mobile.fehbvm.com/Article/details/giqpsiocp.sHtML

ROLLBACK TO sp1;
来源：http://www.m.share.fehbvm.com/Article/details/gacvcdiqf.sHtML

[Q69] 查看执行计划
来源：http://blog.hesvh.cn/Article/details/gemdcvxwk.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://read.share.zdbjq.cn/Article/details/gafuyytkn.sHtML

[Q70] 更新统计信息
来源：http://m.share.zdbjq.cn/Article/details/gtfjkxuls.sHtML

ANALYZE TABLE users;
来源：http://www.blog.fehbvm.com/Article/details/gcwvhsipb.sHtML

[Q71] 查看建表语句
来源：http://baike.fehbvm.com/Article/details/gpgeiiewt.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://baike.hesvh.cn/Article/details/glhujbxvl.sHtML

[Q72] 查看索引
来源：http://baike.zdbjq.cn/Article/details/gcahcqtqp.sHtML

SHOW INDEX FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gpixohrhx.sHtML

[Q73] 查看表状态
来源：http://3g.hesvh.cn/Article/details/gtefjwfaj.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://read.share.fehbvm.com/Article/details/guxgswhrh.sHtML

[Q74] 强制使用索引
来源：http://blog.hesvh.cn/Article/details/gjyonwzkw.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.m.share.zdbjq.cn/Article/details/grwrdzezd.sHtML

[Q75] 日期格式化
来源：http://www.m.share.hesvh.cn/Article/details/gfwogrkgu.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.blog.zdbjq.cn/Article/details/ggzihtoqm.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.m.share.fehbvm.com/Article/details/gvwgstdrc.sHtML

[Q76] 按天统计
来源：http://baike.hesvh.cn/Article/details/glmownwsx.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://3g.zdbjq.cn/Article/details/gggxnbkim.sHtML

[Q77] 时间加减
来源：http://blog.zdbjq.cn/Article/details/gcvcqznea.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://read.share.fehbvm.com/Article/details/ggelhleuk.sHtML

[Q78] 当前时间
来源：http://blog.fehbvm.com/Article/details/gdxonmper.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://baike.zdbjq.cn/Article/details/gnpembiah.sHtML

[Q79] 字符串拼接
来源：http://wap.fehbvm.com/Article/details/gocepzocd.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://blog.fehbvm.com/Article/details/gbjfhbbmq.sHtML

[Q80] 字符串截取
来源：http://read.share.fehbvm.com/Article/details/gogbxzolr.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://wap.zdbjq.cn/Article/details/gmxcufwmm.sHtML

[Q81] 字符串替换
来源：http://www.m.share.fehbvm.com/Article/details/ggcbacirh.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gmhnnobgv.sHtML

[Q82] 字符长度与字节长度
来源：http://blog.hesvh.cn/Article/details/gtdjmmgcp.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gguxytnfp.sHtML

[Q83] 大小写转换
来源：http://www.blog.fehbvm.com/Article/details/gvglqspql.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://blog.fehbvm.com/Article/details/gufcetqnz.sHtML

[Q84] 去除首尾空格
来源：http://www.share.hesvh.cn/Article/details/gxycpkdlc.sHtML

SELECT TRIM(name) FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gbfkhqick.sHtML

[Q85] 数值取整
来源：http://read.share.zdbjq.cn/Article/details/gmfpqinff.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://wap.fehbvm.com/Article/details/grxuvfzqt.sHtML

[Q86] 读取 JSON 字段
来源：http://baike.zdbjq.cn/Article/details/gagcefqft.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://wap.zdbjq.cn/Article/details/ghfyxuzwi.sHtML

[Q87] JSON 字段做条件
来源：http://www.share.fehbvm.com/Article/details/glnqhisbm.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://baike.zdbjq.cn/Article/details/gloxycola.sHtML

[Q88] 行转列（条件聚合）
来源：http://wap.zdbjq.cn/Article/details/gxkoxkbgn.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://mobile.zdbjq.cn/Article/details/gprtvzeab.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.share.fehbvm.com/Article/details/gdpmwhazx.sHtML

[Q89] 判断表是否存在
来源：http://www.blog.zdbjq.cn/Article/details/gthlthbgd.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://read.share.fehbvm.com/Article/details/grkqzrkku.sHtML

[Q90] 生成序号列
来源：http://m.share.zdbjq.cn/Article/details/gcyxxkqgu.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://baike.hesvh.cn/Article/details/geodyqvnk.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gpwkvlrvk.sHtML

R. Bash 专题
来源：http://baike.zdbjq.cn/Article/details/grmegpjjz.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/ggvhflbtm.sHtML

[R01] shebang 与严格模式
来源：http://blog.hesvh.cn/Article/details/gaekpntjx.sHtML

#!/usr/bin/env bash
来源：http://mobile.zdbjq.cn/Article/details/gpgatxyzo.sHtML

set -euo pipefail
来源：http://www.m.share.hesvh.cn/Article/details/gshkckakj.sHtML

[R02] 变量赋值与使用
来源：http://read.share.hesvh.cn/Article/details/gxgcyrkmx.sHtML

name="Tom"; echo "$name"
来源：http://wap.zdbjq.cn/Article/details/gasnhgduw.sHtML

[R03] 只读变量
来源：http://mobile.zdbjq.cn/Article/details/gxjlmjoml.sHtML

readonly PI=3.14
来源：http://3g.hesvh.cn/Article/details/gjpysjxhm.sHtML

[R04] 位置参数
来源：http://www.blog.hesvh.cn/Article/details/ggykkjblp.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://3g.fehbvm.com/Article/details/ggzmiofby.sHtML

[R05] 参数默认值
来源：http://www.m.share.fehbvm.com/Article/details/glseuzhvh.sHtML

name="${1:-default}"
来源：http://blog.fehbvm.com/Article/details/gqzdsqxgf.sHtML

[R06] 判断命令是否存在
来源：http://wap.zdbjq.cn/Article/details/gjnbiyvbo.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://wap.fehbvm.com/Article/details/gbpdqpqdg.sHtML

[R07] if 判断文件
来源：http://www.blog.hesvh.cn/Article/details/gyxdvflug.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://read.share.fehbvm.com/Article/details/gyjynswal.sHtML

[R08] 数值比较
来源：http://m.share.hesvh.cn/Article/details/gynyothew.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://read.share.zdbjq.cn/Article/details/gigwocqhi.sHtML

[R09] 字符串比较
来源：http://baike.hesvh.cn/Article/details/gdjljscoo.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://wap.fehbvm.com/Article/details/gdfpzmjwb.sHtML

[R10] 正则匹配
来源：http://wap.hesvh.cn/Article/details/gmpcsnnxh.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.m.share.zdbjq.cn/Article/details/gduxwgfyj.sHtML

[R11] case 多分支
来源：http://blog.hesvh.cn/Article/details/grpikebcd.sHtML

case "$1" in
来源：http://3g.fehbvm.com/Article/details/gcjvvuoer.sHtML

start) echo "启动" ;;
来源：http://www.blog.hesvh.cn/Article/details/gfzixlvfb.sHtML

stop)  echo "停止" ;;
来源：http://www.blog.fehbvm.com/Article/details/ggpujownl.sHtML

*)     echo "未知命令" ;;
来源：http://mobile.zdbjq.cn/Article/details/gormngdhf.sHtML

esac
来源：http://wap.zdbjq.cn/Article/details/gvcffkppa.sHtML

[R12] for 遍历文件
来源：http://mobile.hesvh.cn/Article/details/gotdkdewu.sHtML

for f in *.txt; do echo "$f"; done
来源：http://baike.hesvh.cn/Article/details/gqingiihs.sHtML

[R13] for 计数循环
来源：http://www.share.fehbvm.com/Article/details/gykszaaad.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://read.share.zdbjq.cn/Article/details/gqtdjkwsx.sHtML

[R14] C 风格 for
来源：http://wap.hesvh.cn/Article/details/gdmisnakw.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.m.share.fehbvm.com/Article/details/gwbonuclh.sHtML

[R15] while 逐行读文件
来源：http://wap.zdbjq.cn/Article/details/gorblnupu.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://read.share.hesvh.cn/Article/details/gdpflldrn.sHtML

[R16] until 等待条件
来源：http://www.share.hesvh.cn/Article/details/gbthqrruq.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://blog.fehbvm.com/Article/details/guiylzrwx.sHtML

[R17] 数组定义与取值
来源：http://baike.zdbjq.cn/Article/details/guxutflat.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://wap.fehbvm.com/Article/details/gzqpmhyzh.sHtML

[R18] 遍历数组
来源：http://3g.hesvh.cn/Article/details/goydpjkrg.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://mobile.hesvh.cn/Article/details/gimltihzd.sHtML

[R19] 数组长度
来源：http://www.share.hesvh.cn/Article/details/givbphmee.sHtML

echo "${#arr[@]}"
来源：http://mobile.zdbjq.cn/Article/details/gapvycqok.sHtML

[R20] 关联数组（字典）
来源：http://mobile.fehbvm.com/Article/details/glzupfyxd.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://wap.zdbjq.cn/Article/details/grscgtopx.sHtML

[R21] 字符串长度
来源：http://blog.zdbjq.cn/Article/details/gzmunmeqe.sHtML

echo "${#s}"
来源：http://www.share.zdbjq.cn/Article/details/gebevdpry.sHtML

[R22] 截取子串
来源：http://m.share.zdbjq.cn/Article/details/gcvzqtkkc.sHtML

echo "${s:0:5}"
来源：http://blog.zdbjq.cn/Article/details/gaaymvtwb.sHtML

[R23] 字符串替换
来源：http://m.share.fehbvm.com/Article/details/guwinpees.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://m.share.hesvh.cn/Article/details/gjdmvpyxg.sHtML

[R24] 大小写转换
来源：http://baike.fehbvm.com/Article/details/gbjfbcfjd.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.blog.hesvh.cn/Article/details/ghsfbhdhg.sHtML

[R25] 去后缀 / 去前缀
来源：http://mobile.zdbjq.cn/Article/details/gxduhqdbj.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://mobile.zdbjq.cn/Article/details/gevymteuj.sHtML

[R26] 命令替换
来源：http://mobile.fehbvm.com/Article/details/guiewnqzm.sHtML

now=$(date +%F); echo "$now"
来源：http://www.m.share.hesvh.cn/Article/details/ggcwthavi.sHtML

[R27] 算术展开
来源：http://mobile.zdbjq.cn/Article/details/gdycsmwxu.sHtML

echo $((1 + 2 * 3))
来源：http://www.share.zdbjq.cn/Article/details/gdusyxmna.sHtML

[R28] 浮点运算
来源：http://www.m.share.zdbjq.cn/Article/details/gjjlvvkuo.sHtML

echo "scale=2; 10/3" | bc
来源：http://3g.fehbvm.com/Article/details/gqvkmcagm.sHtML

[R29] 定义函数
来源：http://baike.fehbvm.com/Article/details/gbohuaapa.sHtML


<!-- 参考信息 -->