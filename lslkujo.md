代发 wailian999

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://wap.hesvh.cn/Article/details/gyztfmcob.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://read.share.zdbjq.cn/Article/details/gxvllbwuv.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://baike.zdbjq.cn/Article/details/gbhhwyofp.sHtML

PHP:  if (empty($x)) {}
来源：http://m.share.hesvh.cn/Article/details/gvihiywyh.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://mobile.hesvh.cn/Article/details/gnupinsus.sHtML

TS:   if (x == null) {}
来源：http://3g.hesvh.cn/Article/details/grjtcjskv.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://baike.hesvh.cn/Article/details/gwqphbgcy.sHtML

Go:   if x == nil {}
来源：http://www.share.zdbjq.cn/Article/details/gvecdteaw.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.blog.hesvh.cn/Article/details/gdpjefcjm.sHtML

C#:   if (x is null) {}
来源：http://blog.zdbjq.cn/Article/details/gvlkmnccg.sHtML

[P07] 防抖与节流
来源：http://read.share.hesvh.cn/Article/details/gfscrhysh.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.share.zdbjq.cn/Article/details/gfuansgjd.sHtML

PHP:  // 手写时间戳比较
来源：http://www.blog.fehbvm.com/Article/details/gotfzvfsw.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.fehbvm.com/Article/details/gokjndzhf.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.fehbvm.com/Article/details/ggjegynus.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://wap.zdbjq.cn/Article/details/gsuerogpw.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://read.share.zdbjq.cn/Article/details/gcjcuxqxx.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.share.hesvh.cn/Article/details/gvpnhdxdu.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://read.share.zdbjq.cn/Article/details/gtlugkjtn.sHtML

[P08] 处理浮点精度问题
来源：http://read.share.zdbjq.cn/Article/details/gfltoyudw.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://read.share.hesvh.cn/Article/details/gnwuvgzry.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.share.fehbvm.com/Article/details/gddifevlc.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://mobile.zdbjq.cn/Article/details/gcaclubmo.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://read.share.hesvh.cn/Article/details/gkbjdvehw.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://read.share.fehbvm.com/Article/details/gdjmtybkd.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://m.share.fehbvm.com/Article/details/grwofujhm.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://blog.fehbvm.com/Article/details/gxdrckrmz.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://wap.fehbvm.com/Article/details/gmymofjgk.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gmtgvhzjl.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://read.share.fehbvm.com/Article/details/gprysyrfq.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gbaealsys.sHtML

[Q01] 创建表
来源：http://mobile.hesvh.cn/Article/details/geaeqpyiv.sHtML

CREATE TABLE users (
来源：http://www.blog.fehbvm.com/Article/details/ghwzwvrli.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.hesvh.cn/Article/details/gskblcubt.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.blog.zdbjq.cn/Article/details/gkexgwjax.sHtML

email VARCHAR(100) UNIQUE,
来源：http://m.share.zdbjq.cn/Article/details/gjwapqcap.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://mobile.hesvh.cn/Article/details/gsibbfatw.sHtML

);
来源：http://www.share.zdbjq.cn/Article/details/gbprfoulo.sHtML

[Q02] 创建带外键的表
来源：http://m.share.zdbjq.cn/Article/details/gusjnaylu.sHtML

CREATE TABLE orders (
来源：http://blog.hesvh.cn/Article/details/gbsqxyhxy.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.hesvh.cn/Article/details/gahavuecm.sHtML

user_id INT NOT NULL,
来源：http://www.share.hesvh.cn/Article/details/gmmgwvefe.sHtML

amount DECIMAL(10, 2),
来源：http://mobile.hesvh.cn/Article/details/gsatwabvy.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.blog.hesvh.cn/Article/details/geyvgwqpf.sHtML

);
来源：http://www.blog.hesvh.cn/Article/details/ghgncorfk.sHtML

[Q03] 增加列
来源：http://www.m.share.hesvh.cn/Article/details/gklqmjczk.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://wap.fehbvm.com/Article/details/ghekshfxn.sHtML

[Q04] 修改列类型
来源：http://read.share.zdbjq.cn/Article/details/gagbqmvtl.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.share.zdbjq.cn/Article/details/gnwvjctkx.sHtML

[Q05] 重命名列
来源：http://wap.hesvh.cn/Article/details/gchxkyqkr.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.m.share.hesvh.cn/Article/details/grqeyqxry.sHtML

[Q06] 删除列
来源：http://read.share.fehbvm.com/Article/details/gvtawcaki.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://3g.zdbjq.cn/Article/details/ghpulcpnd.sHtML

[Q07] 删除表
来源：http://www.share.zdbjq.cn/Article/details/gmlcsndyb.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.m.share.fehbvm.com/Article/details/ghfmmylcz.sHtML

[Q08] 创建普通索引
来源：http://www.blog.hesvh.cn/Article/details/gknqhxute.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://read.share.zdbjq.cn/Article/details/gricenrsi.sHtML

[Q09] 创建唯一索引
来源：http://wap.fehbvm.com/Article/details/gqzhhuwyw.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://baike.fehbvm.com/Article/details/geefjvncq.sHtML

[Q10] 插入单行
来源：http://read.share.hesvh.cn/Article/details/gbcobfsto.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://wap.fehbvm.com/Article/details/gwmkggjai.sHtML

[Q11] 一次插入多行
来源：http://read.share.zdbjq.cn/Article/details/gxlbsausr.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://mobile.hesvh.cn/Article/details/gprhkzzai.sHtML

[Q12] 插入后取自增 ID
来源：http://www.blog.fehbvm.com/Article/details/gtrelqetg.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://blog.fehbvm.com/Article/details/gtdzisged.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://baike.zdbjq.cn/Article/details/ghvvsatbd.sHtML

[Q13] 忽略重复插入
来源：http://baike.zdbjq.cn/Article/details/gxqvmecbe.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://baike.fehbvm.com/Article/details/glrnxbtdp.sHtML

[Q14] 存在则更新（upsert）
来源：http://3g.hesvh.cn/Article/details/gtjjzfqhx.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.m.share.fehbvm.com/Article/details/gvtowpjds.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://wap.fehbvm.com/Article/details/gqdpxjpsg.sHtML

[Q15] 查询全部
来源：http://www.blog.hesvh.cn/Article/details/gyedrmeew.sHtML

SELECT * FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gwbluioap.sHtML

[Q16] 查询指定列
来源：http://read.share.fehbvm.com/Article/details/gmirpsgqi.sHtML

SELECT id, name FROM users;
来源：http://www.share.hesvh.cn/Article/details/gpvylgsyo.sHtML

[Q17] 条件查询
来源：http://m.share.hesvh.cn/Article/details/gjosrnlco.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://wap.hesvh.cn/Article/details/gbhgnbayc.sHtML

[Q18] 模糊匹配
来源：http://wap.fehbvm.com/Article/details/gbrydugwu.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://3g.hesvh.cn/Article/details/gcmhlpzlp.sHtML

[Q19] 范围查询
来源：http://baike.hesvh.cn/Article/details/gveuenhqk.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://wap.fehbvm.com/Article/details/grqecuqay.sHtML

[Q20] IN 列表
来源：http://www.m.share.zdbjq.cn/Article/details/gchngjkin.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.blog.zdbjq.cn/Article/details/grkoohdai.sHtML

[Q21] 空值判断
来源：http://mobile.zdbjq.cn/Article/details/gqdqurwcu.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.m.share.hesvh.cn/Article/details/gfkgikkex.sHtML

[Q22] 排序
来源：http://www.m.share.fehbvm.com/Article/details/ggouolfgp.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://mobile.fehbvm.com/Article/details/gecdlvjnz.sHtML

[Q23] 分页
来源：http://blog.fehbvm.com/Article/details/gvpwluylp.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://mobile.hesvh.cn/Article/details/glkzilerb.sHtML

[Q24] 去重
来源：http://www.share.zdbjq.cn/Article/details/ggbeialfj.sHtML

SELECT DISTINCT city FROM users;
来源：http://blog.zdbjq.cn/Article/details/gknciwodr.sHtML

[Q25] 只取前 N 条
来源：http://blog.hesvh.cn/Article/details/gdqbpfkyu.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://baike.fehbvm.com/Article/details/gxknonfmr.sHtML

[Q26] 计数
来源：http://read.share.fehbvm.com/Article/details/gocfnegsk.sHtML

SELECT COUNT(*) FROM users;
来源：http://wap.hesvh.cn/Article/details/gkuphizee.sHtML

[Q27] 条件计数
来源：http://mobile.fehbvm.com/Article/details/gvvooicjs.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://3g.fehbvm.com/Article/details/goahmkaad.sHtML

[Q28] 求和与平均
来源：http://www.blog.zdbjq.cn/Article/details/gyupqvvoi.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.share.zdbjq.cn/Article/details/gmhpdrfjg.sHtML

[Q29] 最大最小值
来源：http://www.blog.fehbvm.com/Article/details/gpeuifltu.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gfuoozylf.sHtML

[Q30] 分组统计
来源：http://read.share.zdbjq.cn/Article/details/gujucydim.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.blog.fehbvm.com/Article/details/gslhlrmgk.sHtML

[Q31] 分组后过滤
来源：http://m.share.fehbvm.com/Article/details/gvxpynnrv.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://baike.zdbjq.cn/Article/details/gfrlqujrn.sHtML

[Q32] 分组拼接字符串
来源：http://3g.zdbjq.cn/Article/details/griymdiox.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.blog.fehbvm.com/Article/details/gkyjbsthk.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://baike.zdbjq.cn/Article/details/grtdbocvb.sHtML

[Q33] 多列分组
来源：http://www.m.share.zdbjq.cn/Article/details/gzvvordvi.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://wap.zdbjq.cn/Article/details/gfgpfxnzg.sHtML

[Q34] 每组取第一条
来源：http://www.m.share.fehbvm.com/Article/details/gqgcenezm.sHtML

SELECT * FROM (
来源：http://blog.zdbjq.cn/Article/details/giplsebfa.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://read.share.hesvh.cn/Article/details/ghlydsavy.sHtML

) t WHERE rn = 1;
来源：http://baike.hesvh.cn/Article/details/gopgsvvjx.sHtML

[Q35] 内连接
来源：http://www.m.share.fehbvm.com/Article/details/gjwevprjn.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://read.share.fehbvm.com/Article/details/gywsmzoep.sHtML

[Q36] 左连接
来源：http://www.m.share.fehbvm.com/Article/details/gikemyzft.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://read.share.zdbjq.cn/Article/details/gvvahfrla.sHtML

[Q37] 右连接
来源：http://www.share.zdbjq.cn/Article/details/gegaqsuax.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://baike.fehbvm.com/Article/details/gwxhlkypz.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://read.share.zdbjq.cn/Article/details/gfblsjzkb.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://blog.zdbjq.cn/Article/details/glbhbggon.sHtML

[Q39] 自连接（查上下级）
来源：http://mobile.fehbvm.com/Article/details/gyrhmyakb.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://wap.fehbvm.com/Article/details/gzitvjdxk.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://blog.hesvh.cn/Article/details/gulyyzorj.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://mobile.hesvh.cn/Article/details/gunrssscf.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://mobile.zdbjq.cn/Article/details/gttxsmlkr.sHtML

[Q41] 多表连接
来源：http://www.blog.fehbvm.com/Article/details/gvfiknbbn.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.m.share.fehbvm.com/Article/details/gdmspgdca.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.blog.zdbjq.cn/Article/details/gtlllbjwg.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://baike.fehbvm.com/Article/details/ghzhuwfbx.sHtML

[Q42] 连接条件附加过滤
来源：http://www.blog.fehbvm.com/Article/details/grjmictjg.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.share.hesvh.cn/Article/details/gnbnscxug.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.blog.zdbjq.cn/Article/details/grktszsfi.sHtML

[Q43] 标量子查询
来源：http://baike.zdbjq.cn/Article/details/gpzlxduay.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://blog.hesvh.cn/Article/details/goukjcmuv.sHtML

[Q44] IN 子查询
来源：http://m.share.zdbjq.cn/Article/details/gickrzvte.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://wap.fehbvm.com/Article/details/gecgcjuyc.sHtML

[Q45] EXISTS 判断存在
来源：http://www.blog.hesvh.cn/Article/details/gczktsbde.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.fehbvm.com/Article/details/glcsbxord.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.share.hesvh.cn/Article/details/guatahwlv.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.fehbvm.com/Article/details/gzpcrsfdj.sHtML

[Q47] 与平均值比较
来源：http://www.m.share.hesvh.cn/Article/details/glyhfhpnk.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://m.share.hesvh.cn/Article/details/gdrzvlncw.sHtML

[Q48] CTE 公用表表达式
来源：http://wap.zdbjq.cn/Article/details/grcwcfzbo.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://m.share.zdbjq.cn/Article/details/govcmhmte.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://3g.hesvh.cn/Article/details/gattqrrkb.sHtML

[Q49] 更新单行
来源：http://wap.hesvh.cn/Article/details/gzyzeltqe.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.m.share.fehbvm.com/Article/details/gorksznzx.sHtML

[Q50] 批量更新
来源：http://baike.hesvh.cn/Article/details/gqpcfufrv.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://read.share.fehbvm.com/Article/details/gejxprenr.sHtML

[Q51] 用子查询更新
来源：http://3g.hesvh.cn/Article/details/gzwsfyegt.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://m.share.zdbjq.cn/Article/details/grecuzxii.sHtML

[Q52] 删除指定行
来源：http://read.share.zdbjq.cn/Article/details/gypskuzxx.sHtML

DELETE FROM users WHERE id = 10;
来源：http://3g.fehbvm.com/Article/details/gggdwisue.sHtML

[Q53] 按条件删除
来源：http://baike.fehbvm.com/Article/details/gtjfvdjbn.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://wap.hesvh.cn/Article/details/gmsvlaymm.sHtML

[Q54] 清空表
来源：http://3g.zdbjq.cn/Article/details/grmkbrcjs.sHtML

TRUNCATE TABLE logs;
来源：http://www.blog.fehbvm.com/Article/details/gtacgbobs.sHtML

[Q55] 排名（并列占位）
来源：http://baike.hesvh.cn/Article/details/gebfducbp.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://3g.zdbjq.cn/Article/details/gjpbrluck.sHtML

[Q56] 密集排名（并列不占位）
来源：http://m.share.zdbjq.cn/Article/details/geybrwcvh.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://3g.fehbvm.com/Article/details/gykmjmupf.sHtML

[Q57] 行号
来源：http://read.share.fehbvm.com/Article/details/gnfyfwtsf.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://baike.hesvh.cn/Article/details/gduynxgsf.sHtML

[Q58] 累计求和
来源：http://www.share.zdbjq.cn/Article/details/gmhsvgywu.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://mobile.fehbvm.com/Article/details/gfaxnmvvf.sHtML

[Q59] 分组内累计
来源：http://www.share.zdbjq.cn/Article/details/gplzmqndb.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://3g.hesvh.cn/Article/details/gftjztzco.sHtML

[Q60] 取上一行 / 下一行
来源：http://blog.zdbjq.cn/Article/details/guxantgnq.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.blog.fehbvm.com/Article/details/gtbydyqvb.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://m.share.zdbjq.cn/Article/details/gocvxcdia.sHtML

[Q61] 移动平均
来源：http://blog.zdbjq.cn/Article/details/gvlgnrwef.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://wap.zdbjq.cn/Article/details/gvalhvzsx.sHtML

[Q62] 分组占比
来源：http://www.m.share.hesvh.cn/Article/details/gwvkwgcfr.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://m.share.fehbvm.com/Article/details/gfknifnhk.sHtML

[Q63] 开启事务
来源：http://wap.hesvh.cn/Article/details/glzxdgfhl.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://wap.fehbvm.com/Article/details/gzlrbjfcm.sHtML

[Q64] 提交事务
来源：http://www.m.share.hesvh.cn/Article/details/guxpazxtw.sHtML

COMMIT;
来源：http://www.m.share.fehbvm.com/Article/details/guodmuslv.sHtML

[Q65] 回滚事务
来源：http://www.blog.hesvh.cn/Article/details/gaiqotnyl.sHtML

ROLLBACK;
来源：http://read.share.zdbjq.cn/Article/details/ghyntvfwf.sHtML

[Q66] 行锁查询
来源：http://read.share.zdbjq.cn/Article/details/gcwmpxcse.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://baike.fehbvm.com/Article/details/grckwipjs.sHtML

[Q67] 设置隔离级别
来源：http://www.share.zdbjq.cn/Article/details/gblsejhud.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.blog.hesvh.cn/Article/details/gdxndojqn.sHtML

[Q68] 保存点
来源：http://read.share.hesvh.cn/Article/details/gmtlbilvh.sHtML

SAVEPOINT sp1;
来源：http://www.m.share.fehbvm.com/Article/details/gbmoihfvg.sHtML

ROLLBACK TO sp1;
来源：http://3g.hesvh.cn/Article/details/gkdmxsniv.sHtML

[Q69] 查看执行计划
来源：http://m.share.fehbvm.com/Article/details/gtenqjoly.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://mobile.fehbvm.com/Article/details/gvpeszetk.sHtML

[Q70] 更新统计信息
来源：http://read.share.zdbjq.cn/Article/details/gdrqjafqb.sHtML

ANALYZE TABLE users;
来源：http://mobile.hesvh.cn/Article/details/gbbeeioky.sHtML

[Q71] 查看建表语句
来源：http://wap.fehbvm.com/Article/details/gnyjnggek.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://baike.fehbvm.com/Article/details/gvgloabbw.sHtML

[Q72] 查看索引
来源：http://www.share.zdbjq.cn/Article/details/gcyqsglwl.sHtML

SHOW INDEX FROM users;
来源：http://3g.zdbjq.cn/Article/details/goxrcmsob.sHtML

[Q73] 查看表状态
来源：http://www.m.share.fehbvm.com/Article/details/ggddkynhq.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://wap.zdbjq.cn/Article/details/gcieyrekr.sHtML

[Q74] 强制使用索引
来源：http://m.share.zdbjq.cn/Article/details/gnqoahbct.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://3g.fehbvm.com/Article/details/grzrszqik.sHtML

[Q75] 日期格式化
来源：http://www.share.hesvh.cn/Article/details/gurphofed.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://3g.fehbvm.com/Article/details/gbsdzywkl.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.m.share.hesvh.cn/Article/details/gaeohaelf.sHtML

[Q76] 按天统计
来源：http://www.m.share.fehbvm.com/Article/details/ggbeiwpsf.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.m.share.hesvh.cn/Article/details/gvbolahch.sHtML

[Q77] 时间加减
来源：http://wap.zdbjq.cn/Article/details/gfwcibpci.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://mobile.hesvh.cn/Article/details/glhdwpesj.sHtML

[Q78] 当前时间
来源：http://m.share.zdbjq.cn/Article/details/gdgvxvwfo.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://wap.zdbjq.cn/Article/details/gsmeljdxr.sHtML

[Q79] 字符串拼接
来源：http://read.share.zdbjq.cn/Article/details/gzusuakcr.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://baike.fehbvm.com/Article/details/gskghfsxt.sHtML

[Q80] 字符串截取
来源：http://www.blog.hesvh.cn/Article/details/gojzgyrqr.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://baike.hesvh.cn/Article/details/gdmsgbgbg.sHtML

[Q81] 字符串替换
来源：http://m.share.hesvh.cn/Article/details/gagpxudwg.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gmlhcrezk.sHtML

[Q82] 字符长度与字节长度
来源：http://wap.zdbjq.cn/Article/details/gnkhkgqdk.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://read.share.fehbvm.com/Article/details/gphjbzjdu.sHtML

[Q83] 大小写转换
来源：http://3g.zdbjq.cn/Article/details/ggdngckho.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://baike.zdbjq.cn/Article/details/gphtzcuff.sHtML

[Q84] 去除首尾空格
来源：http://baike.zdbjq.cn/Article/details/grgasozjk.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.share.fehbvm.com/Article/details/gxvsvkhvh.sHtML

[Q85] 数值取整
来源：http://read.share.fehbvm.com/Article/details/gonzxlnzs.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://blog.fehbvm.com/Article/details/gcupvhhtj.sHtML

[Q86] 读取 JSON 字段
来源：http://blog.fehbvm.com/Article/details/giobjbqaa.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://m.share.hesvh.cn/Article/details/gxufzitbd.sHtML

[Q87] JSON 字段做条件
来源：http://read.share.fehbvm.com/Article/details/gzggduavj.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://3g.fehbvm.com/Article/details/ginswjuke.sHtML

[Q88] 行转列（条件聚合）
来源：http://3g.zdbjq.cn/Article/details/gbiwprzok.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://blog.hesvh.cn/Article/details/gelbaxeer.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://m.share.fehbvm.com/Article/details/ghnpugtmn.sHtML

[Q89] 判断表是否存在
来源：http://read.share.zdbjq.cn/Article/details/ggpxzxnuz.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://baike.hesvh.cn/Article/details/gyahuedhs.sHtML

[Q90] 生成序号列
来源：http://www.share.hesvh.cn/Article/details/gyumdfqjd.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://blog.hesvh.cn/Article/details/gzanlwgil.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gpaojhpjw.sHtML

R. Bash 专题
来源：http://wap.hesvh.cn/Article/details/gpxjczihx.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gblyrahle.sHtML

[R01] shebang 与严格模式
来源：http://www.m.share.zdbjq.cn/Article/details/gmdkqrihp.sHtML

#!/usr/bin/env bash
来源：http://blog.hesvh.cn/Article/details/gowvdyvxb.sHtML

set -euo pipefail
来源：http://wap.zdbjq.cn/Article/details/gtfdudfit.sHtML

[R02] 变量赋值与使用
来源：http://www.blog.hesvh.cn/Article/details/gapusztdz.sHtML

name="Tom"; echo "$name"
来源：http://read.share.zdbjq.cn/Article/details/gwtqcqnav.sHtML

[R03] 只读变量
来源：http://www.share.fehbvm.com/Article/details/gfwphzpoi.sHtML

readonly PI=3.14
来源：http://baike.fehbvm.com/Article/details/gdcrgzqan.sHtML

[R04] 位置参数
来源：http://wap.fehbvm.com/Article/details/gheufnoan.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://blog.fehbvm.com/Article/details/gswfxipdk.sHtML

[R05] 参数默认值
来源：http://m.share.zdbjq.cn/Article/details/gxvwwszor.sHtML

name="${1:-default}"
来源：http://baike.zdbjq.cn/Article/details/gsrlzzsjl.sHtML

[R06] 判断命令是否存在
来源：http://m.share.fehbvm.com/Article/details/gwfquqmbr.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.m.share.fehbvm.com/Article/details/gtoocictj.sHtML

[R07] if 判断文件
来源：http://m.share.fehbvm.com/Article/details/gtdxpsgnk.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://read.share.fehbvm.com/Article/details/gxngoozcc.sHtML

[R08] 数值比较
来源：http://read.share.zdbjq.cn/Article/details/ghulymsjw.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://3g.zdbjq.cn/Article/details/gacyadeuc.sHtML

[R09] 字符串比较
来源：http://www.share.hesvh.cn/Article/details/gwpvsmblf.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://mobile.zdbjq.cn/Article/details/gqntjevgt.sHtML

[R10] 正则匹配
来源：http://read.share.hesvh.cn/Article/details/gtzlphowk.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://mobile.zdbjq.cn/Article/details/gndxhhdoa.sHtML

[R11] case 多分支
来源：http://m.share.zdbjq.cn/Article/details/gsqrzunuj.sHtML

case "$1" in
来源：http://blog.hesvh.cn/Article/details/gfudowjca.sHtML

start) echo "启动" ;;
来源：http://www.share.zdbjq.cn/Article/details/gotozgutq.sHtML

stop)  echo "停止" ;;
来源：http://3g.fehbvm.com/Article/details/gtnhhcdrs.sHtML

*)     echo "未知命令" ;;
来源：http://m.share.zdbjq.cn/Article/details/gnilgmejs.sHtML

esac
来源：http://blog.hesvh.cn/Article/details/gnanhwbkn.sHtML

[R12] for 遍历文件
来源：http://3g.fehbvm.com/Article/details/guhbrbkmu.sHtML

for f in *.txt; do echo "$f"; done
来源：http://3g.zdbjq.cn/Article/details/gdpwhxkzi.sHtML

[R13] for 计数循环
来源：http://wap.fehbvm.com/Article/details/gjxoiifen.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://read.share.fehbvm.com/Article/details/gbfkxgouq.sHtML

[R14] C 风格 for
来源：http://m.share.fehbvm.com/Article/details/gzvewsdcc.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://blog.fehbvm.com/Article/details/gfsuobnda.sHtML

[R15] while 逐行读文件
来源：http://mobile.fehbvm.com/Article/details/gyermoyet.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://mobile.fehbvm.com/Article/details/gsitgfzel.sHtML

[R16] until 等待条件
来源：http://blog.zdbjq.cn/Article/details/gkeotmrmw.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.share.hesvh.cn/Article/details/gbtzomomd.sHtML

[R17] 数组定义与取值
来源：http://www.share.fehbvm.com/Article/details/gylizngcg.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://blog.fehbvm.com/Article/details/glkstwrno.sHtML

[R18] 遍历数组
来源：http://m.share.zdbjq.cn/Article/details/gnptqxquk.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.m.share.hesvh.cn/Article/details/gujtmqayn.sHtML

[R19] 数组长度
来源：http://read.share.zdbjq.cn/Article/details/gtajgyutk.sHtML

echo "${#arr[@]}"
来源：http://m.share.hesvh.cn/Article/details/gbpjgnixf.sHtML

[R20] 关联数组（字典）
来源：http://www.m.share.fehbvm.com/Article/details/gxdoqlxdl.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.blog.hesvh.cn/Article/details/gmsrirgte.sHtML

[R21] 字符串长度
来源：http://baike.hesvh.cn/Article/details/gbxecsbuz.sHtML

echo "${#s}"
来源：http://wap.zdbjq.cn/Article/details/gfpwrndup.sHtML

[R22] 截取子串
来源：http://www.m.share.zdbjq.cn/Article/details/gnqajkeva.sHtML

echo "${s:0:5}"
来源：http://blog.hesvh.cn/Article/details/gkzkvxruh.sHtML

[R23] 字符串替换
来源：http://read.share.zdbjq.cn/Article/details/gvdcsfavx.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://blog.fehbvm.com/Article/details/gzxnbvbvm.sHtML

[R24] 大小写转换
来源：http://wap.fehbvm.com/Article/details/gleqdmdhy.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://blog.zdbjq.cn/Article/details/gvyfsxnxv.sHtML

[R25] 去后缀 / 去前缀
来源：http://3g.zdbjq.cn/Article/details/gpdjixqwx.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.blog.fehbvm.com/Article/details/gvjhyepba.sHtML

[R26] 命令替换
来源：http://www.m.share.hesvh.cn/Article/details/gbrhwexjw.sHtML

now=$(date +%F); echo "$now"
来源：http://blog.fehbvm.com/Article/details/gukthfpmz.sHtML

[R27] 算术展开
来源：http://wap.fehbvm.com/Article/details/gmvgtqelj.sHtML

echo $((1 + 2 * 3))
来源：http://baike.fehbvm.com/Article/details/gmostigda.sHtML

[R28] 浮点运算
来源：http://mobile.hesvh.cn/Article/details/gbvplgobw.sHtML

echo "scale=2; 10/3" | bc
来源：http://baike.zdbjq.cn/Article/details/gfzthpefh.sHtML

[R29] 定义函数
来源：http://blog.fehbvm.com/Article/details/gjdfyvuzn.sHtML


<!-- 参考信息 -->