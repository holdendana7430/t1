代发 wailian999

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://m.share.fehbvm.com/Article/details/guaiqtfmy.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://m.share.hesvh.cn/Article/details/gzgxegbkq.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.blog.fehbvm.com/Article/details/gddyxyrop.sHtML

PHP:  if (empty($x)) {}
来源：http://wap.hesvh.cn/Article/details/giieqbhkb.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.blog.fehbvm.com/Article/details/gaiofmrro.sHtML

TS:   if (x == null) {}
来源：http://baike.fehbvm.com/Article/details/gqtgpfsow.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.share.hesvh.cn/Article/details/gmdhvcpyp.sHtML

Go:   if x == nil {}
来源：http://wap.zdbjq.cn/Article/details/gnzqlhwqp.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://m.share.fehbvm.com/Article/details/gvarfxxqg.sHtML

C#:   if (x is null) {}
来源：http://mobile.fehbvm.com/Article/details/gbfgzzjae.sHtML

[P07] 防抖与节流
来源：http://www.blog.fehbvm.com/Article/details/gnkxmguuc.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://m.share.zdbjq.cn/Article/details/gdkfvxhyc.sHtML

PHP:  // 手写时间戳比较
来源：http://baike.hesvh.cn/Article/details/ggjmleoxl.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.hesvh.cn/Article/details/genxjiwni.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.zdbjq.cn/Article/details/gnghpalsp.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://mobile.fehbvm.com/Article/details/gclsuttnp.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.m.share.hesvh.cn/Article/details/ghasgylbh.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.share.fehbvm.com/Article/details/gmjnjwihf.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.m.share.fehbvm.com/Article/details/ghmxojqvz.sHtML

[P08] 处理浮点精度问题
来源：http://3g.hesvh.cn/Article/details/grjriashk.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.blog.fehbvm.com/Article/details/gmctyxrax.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://blog.zdbjq.cn/Article/details/gcdnvzmks.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.m.share.hesvh.cn/Article/details/gjgqkblok.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://read.share.zdbjq.cn/Article/details/gxigwyegm.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.blog.fehbvm.com/Article/details/gsxbvyeey.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.m.share.hesvh.cn/Article/details/gztacgrwq.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://m.share.hesvh.cn/Article/details/gfjucogvc.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.share.zdbjq.cn/Article/details/gkelkqzyp.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/giskneajz.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://m.share.hesvh.cn/Article/details/gwjrcitbe.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gzntbedox.sHtML

[Q01] 创建表
来源：http://m.share.zdbjq.cn/Article/details/gzydygbdt.sHtML

CREATE TABLE users (
来源：http://baike.hesvh.cn/Article/details/gyhggjqgk.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.fehbvm.com/Article/details/gjomutgss.sHtML

name VARCHAR(50) NOT NULL,
来源：http://3g.hesvh.cn/Article/details/geocvujeq.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.m.share.zdbjq.cn/Article/details/gnmlisphc.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.share.fehbvm.com/Article/details/gvuytzafm.sHtML

);
来源：http://wap.fehbvm.com/Article/details/gthtcchgq.sHtML

[Q02] 创建带外键的表
来源：http://blog.hesvh.cn/Article/details/gmwpfxigd.sHtML

CREATE TABLE orders (
来源：http://m.share.zdbjq.cn/Article/details/gfosmjibo.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.share.zdbjq.cn/Article/details/gxzqaclol.sHtML

user_id INT NOT NULL,
来源：http://blog.hesvh.cn/Article/details/gkxsempay.sHtML

amount DECIMAL(10, 2),
来源：http://www.blog.fehbvm.com/Article/details/gvmprfkra.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://wap.fehbvm.com/Article/details/gdtwhuwdj.sHtML

);
来源：http://wap.zdbjq.cn/Article/details/gckxfkwkq.sHtML

[Q03] 增加列
来源：http://www.share.fehbvm.com/Article/details/gfaxydxob.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.blog.fehbvm.com/Article/details/gfnifplpv.sHtML

[Q04] 修改列类型
来源：http://mobile.fehbvm.com/Article/details/gtpnugusp.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.share.hesvh.cn/Article/details/gdgrzyiyo.sHtML

[Q05] 重命名列
来源：http://wap.fehbvm.com/Article/details/gudeylrgi.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://mobile.hesvh.cn/Article/details/gnojpylra.sHtML

[Q06] 删除列
来源：http://wap.hesvh.cn/Article/details/gehriaenb.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://read.share.fehbvm.com/Article/details/gaqmhkzwy.sHtML

[Q07] 删除表
来源：http://www.m.share.zdbjq.cn/Article/details/gefulqfnx.sHtML

DROP TABLE IF EXISTS orders;
来源：http://read.share.zdbjq.cn/Article/details/gkjlizuak.sHtML

[Q08] 创建普通索引
来源：http://www.blog.zdbjq.cn/Article/details/gzkewqjud.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://m.share.fehbvm.com/Article/details/gbqezrfmv.sHtML

[Q09] 创建唯一索引
来源：http://read.share.fehbvm.com/Article/details/gcnceijqd.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://blog.fehbvm.com/Article/details/gzeyykkki.sHtML

[Q10] 插入单行
来源：http://3g.fehbvm.com/Article/details/gzzuknnwk.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://3g.fehbvm.com/Article/details/gkloctiga.sHtML

[Q11] 一次插入多行
来源：http://read.share.zdbjq.cn/Article/details/gxiaquklu.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://wap.fehbvm.com/Article/details/gyddqtxdw.sHtML

[Q12] 插入后取自增 ID
来源：http://blog.fehbvm.com/Article/details/gkybhspik.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.blog.hesvh.cn/Article/details/gdgwsalgb.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://mobile.zdbjq.cn/Article/details/grpzpcops.sHtML

[Q13] 忽略重复插入
来源：http://wap.fehbvm.com/Article/details/ghksoljbg.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://blog.fehbvm.com/Article/details/gqndclrzv.sHtML

[Q14] 存在则更新（upsert）
来源：http://3g.fehbvm.com/Article/details/guhsifxbz.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://wap.zdbjq.cn/Article/details/gisjlshfx.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://read.share.zdbjq.cn/Article/details/gcaxryoiq.sHtML

[Q15] 查询全部
来源：http://www.m.share.fehbvm.com/Article/details/ghlpuwuol.sHtML

SELECT * FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gsszgqjvh.sHtML

[Q16] 查询指定列
来源：http://m.share.hesvh.cn/Article/details/gypqymazw.sHtML

SELECT id, name FROM users;
来源：http://3g.hesvh.cn/Article/details/gjqmlnigs.sHtML

[Q17] 条件查询
来源：http://blog.fehbvm.com/Article/details/gvudotmjr.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://m.share.zdbjq.cn/Article/details/goqsrlkdo.sHtML

[Q18] 模糊匹配
来源：http://www.m.share.fehbvm.com/Article/details/grwcfbmos.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.share.hesvh.cn/Article/details/ginxevzdq.sHtML

[Q19] 范围查询
来源：http://blog.zdbjq.cn/Article/details/gjlmfehzt.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://wap.zdbjq.cn/Article/details/gcengatve.sHtML

[Q20] IN 列表
来源：http://wap.fehbvm.com/Article/details/gyuolmmnc.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://3g.fehbvm.com/Article/details/ggiwykylf.sHtML

[Q21] 空值判断
来源：http://wap.hesvh.cn/Article/details/gfmqseubx.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://m.share.zdbjq.cn/Article/details/griarjbwy.sHtML

[Q22] 排序
来源：http://mobile.hesvh.cn/Article/details/gyaqmfzdg.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://m.share.zdbjq.cn/Article/details/gqxpsqgwn.sHtML

[Q23] 分页
来源：http://www.blog.zdbjq.cn/Article/details/gzijweuxf.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://baike.fehbvm.com/Article/details/gwtrsqeis.sHtML

[Q24] 去重
来源：http://www.m.share.fehbvm.com/Article/details/gdnnvfojt.sHtML

SELECT DISTINCT city FROM users;
来源：http://m.share.fehbvm.com/Article/details/gwfitdrfu.sHtML

[Q25] 只取前 N 条
来源：http://www.m.share.fehbvm.com/Article/details/ghceovfgd.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://3g.zdbjq.cn/Article/details/gtmbcttzz.sHtML

[Q26] 计数
来源：http://wap.hesvh.cn/Article/details/gmvzhxywi.sHtML

SELECT COUNT(*) FROM users;
来源：http://m.share.fehbvm.com/Article/details/gvqqnpegd.sHtML

[Q27] 条件计数
来源：http://www.m.share.hesvh.cn/Article/details/ggfjawjyv.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://3g.fehbvm.com/Article/details/glqhdrwjw.sHtML

[Q28] 求和与平均
来源：http://www.m.share.hesvh.cn/Article/details/gexccehcx.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://3g.hesvh.cn/Article/details/gmyfsmhyf.sHtML

[Q29] 最大最小值
来源：http://wap.zdbjq.cn/Article/details/gjpijmcyr.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gkxstvumx.sHtML

[Q30] 分组统计
来源：http://www.share.zdbjq.cn/Article/details/grywvikiz.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.blog.hesvh.cn/Article/details/gmybaimji.sHtML

[Q31] 分组后过滤
来源：http://baike.zdbjq.cn/Article/details/gtnerukok.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.blog.zdbjq.cn/Article/details/grnpqpfjb.sHtML

[Q32] 分组拼接字符串
来源：http://baike.zdbjq.cn/Article/details/gpvqemtaj.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.blog.zdbjq.cn/Article/details/guzfawzrp.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.share.hesvh.cn/Article/details/glcywxgqr.sHtML

[Q33] 多列分组
来源：http://read.share.zdbjq.cn/Article/details/gvllrprvl.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://wap.zdbjq.cn/Article/details/gcsdleqfb.sHtML

[Q34] 每组取第一条
来源：http://www.share.fehbvm.com/Article/details/gicwgkitc.sHtML

SELECT * FROM (
来源：http://read.share.fehbvm.com/Article/details/gyneendsl.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://wap.fehbvm.com/Article/details/ggjbdofwe.sHtML

) t WHERE rn = 1;
来源：http://mobile.zdbjq.cn/Article/details/glipfnwgl.sHtML

[Q35] 内连接
来源：http://www.m.share.fehbvm.com/Article/details/gktjdxirg.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.fehbvm.com/Article/details/gqbthrpue.sHtML

[Q36] 左连接
来源：http://mobile.fehbvm.com/Article/details/gtcxxlefk.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://m.share.fehbvm.com/Article/details/gvgfbebji.sHtML

[Q37] 右连接
来源：http://read.share.hesvh.cn/Article/details/gqhnwwcrc.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://read.share.fehbvm.com/Article/details/gunthfnne.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://wap.fehbvm.com/Article/details/gindxoxpz.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://read.share.hesvh.cn/Article/details/gmhmdkgog.sHtML

[Q39] 自连接（查上下级）
来源：http://blog.zdbjq.cn/Article/details/gucebflzb.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://wap.zdbjq.cn/Article/details/gjbskbqhm.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://blog.hesvh.cn/Article/details/gtzrceoxp.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://wap.hesvh.cn/Article/details/gwhrshcxq.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.blog.zdbjq.cn/Article/details/gnzfnizoo.sHtML

[Q41] 多表连接
来源：http://baike.hesvh.cn/Article/details/gxtqgbvhp.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://m.share.fehbvm.com/Article/details/gqcklwovi.sHtML

JOIN users u ON u.id = o.user_id
来源：http://m.share.hesvh.cn/Article/details/gswyxcrdn.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.m.share.hesvh.cn/Article/details/gfpjzumfw.sHtML

[Q42] 连接条件附加过滤
来源：http://wap.hesvh.cn/Article/details/gxmamcckd.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.share.hesvh.cn/Article/details/gucaadrej.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://3g.zdbjq.cn/Article/details/grgkzpcfs.sHtML

[Q43] 标量子查询
来源：http://read.share.fehbvm.com/Article/details/gwvqodmoo.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://baike.fehbvm.com/Article/details/ggblpzzgw.sHtML

[Q44] IN 子查询
来源：http://mobile.zdbjq.cn/Article/details/gaeylbyvp.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.share.zdbjq.cn/Article/details/gvmhbmfcu.sHtML

[Q45] EXISTS 判断存在
来源：http://read.share.zdbjq.cn/Article/details/gnocxtqml.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.zdbjq.cn/Article/details/gjsgocmzg.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://mobile.fehbvm.com/Article/details/gvwwbwlzm.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.zdbjq.cn/Article/details/goqamvhgf.sHtML

[Q47] 与平均值比较
来源：http://www.share.zdbjq.cn/Article/details/gjasuxuak.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://mobile.fehbvm.com/Article/details/gpuhtiahi.sHtML

[Q48] CTE 公用表表达式
来源：http://3g.zdbjq.cn/Article/details/gktmpwaya.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://blog.zdbjq.cn/Article/details/gbgfachux.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.blog.hesvh.cn/Article/details/gsuzxmjev.sHtML

[Q49] 更新单行
来源：http://www.share.fehbvm.com/Article/details/glijqyacw.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://mobile.hesvh.cn/Article/details/getqfnpyn.sHtML

[Q50] 批量更新
来源：http://wap.hesvh.cn/Article/details/gzfoknauj.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.m.share.fehbvm.com/Article/details/ggvoazgyg.sHtML

[Q51] 用子查询更新
来源：http://wap.zdbjq.cn/Article/details/gcrdgyryq.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://blog.fehbvm.com/Article/details/gltnrbccs.sHtML

[Q52] 删除指定行
来源：http://baike.fehbvm.com/Article/details/gwyvsptai.sHtML

DELETE FROM users WHERE id = 10;
来源：http://baike.hesvh.cn/Article/details/gixjbnbyl.sHtML

[Q53] 按条件删除
来源：http://m.share.zdbjq.cn/Article/details/gjmhzpvse.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://3g.hesvh.cn/Article/details/goswzuzkj.sHtML

[Q54] 清空表
来源：http://blog.fehbvm.com/Article/details/gfyzsociy.sHtML

TRUNCATE TABLE logs;
来源：http://m.share.zdbjq.cn/Article/details/gdkecdfki.sHtML

[Q55] 排名（并列占位）
来源：http://m.share.zdbjq.cn/Article/details/grkzeqpei.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://baike.hesvh.cn/Article/details/gypwcztil.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.share.fehbvm.com/Article/details/gfzpqukzm.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.m.share.hesvh.cn/Article/details/gqtunrggp.sHtML

[Q57] 行号
来源：http://mobile.fehbvm.com/Article/details/giabgaxvz.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://wap.fehbvm.com/Article/details/gvqoafnvc.sHtML

[Q58] 累计求和
来源：http://mobile.zdbjq.cn/Article/details/goxrbrxni.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://m.share.zdbjq.cn/Article/details/gvntregan.sHtML

[Q59] 分组内累计
来源：http://m.share.hesvh.cn/Article/details/gjohsdcvs.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://m.share.fehbvm.com/Article/details/gxadvtfei.sHtML

[Q60] 取上一行 / 下一行
来源：http://mobile.hesvh.cn/Article/details/gstfqrwvf.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://read.share.fehbvm.com/Article/details/gtedqsoqy.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://wap.zdbjq.cn/Article/details/glctkhwgf.sHtML

[Q61] 移动平均
来源：http://wap.hesvh.cn/Article/details/ghfrhdsku.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://m.share.zdbjq.cn/Article/details/gbwttiiwd.sHtML

[Q62] 分组占比
来源：http://m.share.zdbjq.cn/Article/details/gmkalrqfz.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://wap.hesvh.cn/Article/details/gaduqdfap.sHtML

[Q63] 开启事务
来源：http://baike.zdbjq.cn/Article/details/gfjdckuse.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://blog.zdbjq.cn/Article/details/gffvaijsb.sHtML

[Q64] 提交事务
来源：http://www.share.hesvh.cn/Article/details/gtflcgilf.sHtML

COMMIT;
来源：http://mobile.hesvh.cn/Article/details/guocytflh.sHtML

[Q65] 回滚事务
来源：http://www.blog.hesvh.cn/Article/details/gogmquxnc.sHtML

ROLLBACK;
来源：http://blog.hesvh.cn/Article/details/geidlfdyn.sHtML

[Q66] 行锁查询
来源：http://read.share.fehbvm.com/Article/details/gcxfljwyd.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.share.fehbvm.com/Article/details/ginvfrvix.sHtML

[Q67] 设置隔离级别
来源：http://baike.fehbvm.com/Article/details/gmnwewmhq.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://mobile.zdbjq.cn/Article/details/gfzgvrvjf.sHtML

[Q68] 保存点
来源：http://mobile.hesvh.cn/Article/details/ghvpawxdr.sHtML

SAVEPOINT sp1;
来源：http://wap.fehbvm.com/Article/details/gcfxpzybo.sHtML

ROLLBACK TO sp1;
来源：http://read.share.fehbvm.com/Article/details/gsilkrtds.sHtML

[Q69] 查看执行计划
来源：http://blog.fehbvm.com/Article/details/gdmjrgaqq.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://mobile.fehbvm.com/Article/details/gjvfxfdwp.sHtML

[Q70] 更新统计信息
来源：http://wap.zdbjq.cn/Article/details/grevlsnjy.sHtML

ANALYZE TABLE users;
来源：http://mobile.zdbjq.cn/Article/details/gxmknaysz.sHtML

[Q71] 查看建表语句
来源：http://www.blog.hesvh.cn/Article/details/gjppbdgwk.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://3g.hesvh.cn/Article/details/gdcfgbcgt.sHtML

[Q72] 查看索引
来源：http://3g.fehbvm.com/Article/details/gxwamaxzv.sHtML

SHOW INDEX FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gqiqhjqim.sHtML

[Q73] 查看表状态
来源：http://blog.zdbjq.cn/Article/details/gbymlxvsc.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.share.fehbvm.com/Article/details/guecyerbe.sHtML

[Q74] 强制使用索引
来源：http://www.m.share.zdbjq.cn/Article/details/gpsirljin.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://baike.fehbvm.com/Article/details/gutjklnka.sHtML

[Q75] 日期格式化
来源：http://read.share.hesvh.cn/Article/details/gtjewjbzl.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://3g.hesvh.cn/Article/details/gtujvoexy.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://3g.hesvh.cn/Article/details/gxjuntotr.sHtML

[Q76] 按天统计
来源：http://3g.fehbvm.com/Article/details/gfuzqzqpm.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://read.share.zdbjq.cn/Article/details/gynucyhgc.sHtML

[Q77] 时间加减
来源：http://m.share.zdbjq.cn/Article/details/gdnajxvlx.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.blog.hesvh.cn/Article/details/gxypuexpv.sHtML

[Q78] 当前时间
来源：http://www.blog.fehbvm.com/Article/details/gsnqdpzpa.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.blog.fehbvm.com/Article/details/gheeqefkm.sHtML

[Q79] 字符串拼接
来源：http://baike.hesvh.cn/Article/details/griuvewjj.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://m.share.fehbvm.com/Article/details/gvfpbosap.sHtML

[Q80] 字符串截取
来源：http://blog.zdbjq.cn/Article/details/gqmuqitgt.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://wap.zdbjq.cn/Article/details/gtnqzikry.sHtML

[Q81] 字符串替换
来源：http://www.m.share.fehbvm.com/Article/details/gebpvtaax.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gvhpbqhlx.sHtML

[Q82] 字符长度与字节长度
来源：http://blog.hesvh.cn/Article/details/geozkujnt.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://baike.fehbvm.com/Article/details/gdtfxilxk.sHtML

[Q83] 大小写转换
来源：http://blog.zdbjq.cn/Article/details/grqscoacf.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://wap.zdbjq.cn/Article/details/gdhkcekgd.sHtML

[Q84] 去除首尾空格
来源：http://www.blog.zdbjq.cn/Article/details/gfmlxpyvo.sHtML

SELECT TRIM(name) FROM users;
来源：http://blog.fehbvm.com/Article/details/gfppzgfxo.sHtML

[Q85] 数值取整
来源：http://www.m.share.zdbjq.cn/Article/details/gizmkgtts.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://mobile.hesvh.cn/Article/details/gqvpbmekh.sHtML

[Q86] 读取 JSON 字段
来源：http://mobile.zdbjq.cn/Article/details/geldtbpav.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://blog.hesvh.cn/Article/details/ghiuwewap.sHtML

[Q87] JSON 字段做条件
来源：http://www.share.hesvh.cn/Article/details/gvbebjjao.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.m.share.zdbjq.cn/Article/details/gquhrsefd.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.blog.zdbjq.cn/Article/details/gjgtisqgy.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://blog.zdbjq.cn/Article/details/ghfljnyem.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://mobile.fehbvm.com/Article/details/gxiklpmca.sHtML

[Q89] 判断表是否存在
来源：http://3g.fehbvm.com/Article/details/gmdsnytay.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.share.hesvh.cn/Article/details/grlltlsju.sHtML

[Q90] 生成序号列
来源：http://read.share.fehbvm.com/Article/details/gztwvmowx.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.blog.fehbvm.com/Article/details/gbpwswygb.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gksekggdt.sHtML

R. Bash 专题
来源：http://www.share.fehbvm.com/Article/details/giikratjt.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gifmzpews.sHtML

[R01] shebang 与严格模式
来源：http://m.share.fehbvm.com/Article/details/gxspqkwea.sHtML

#!/usr/bin/env bash
来源：http://3g.hesvh.cn/Article/details/gmfxqifxn.sHtML

set -euo pipefail
来源：http://m.share.fehbvm.com/Article/details/gpevsshyn.sHtML

[R02] 变量赋值与使用
来源：http://baike.zdbjq.cn/Article/details/gusswtgnl.sHtML

name="Tom"; echo "$name"
来源：http://www.share.fehbvm.com/Article/details/gawpmunvn.sHtML

[R03] 只读变量
来源：http://blog.fehbvm.com/Article/details/gruiibnny.sHtML

readonly PI=3.14
来源：http://3g.hesvh.cn/Article/details/giwwzdokr.sHtML

[R04] 位置参数
来源：http://www.share.zdbjq.cn/Article/details/gwjpzcbji.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://3g.fehbvm.com/Article/details/gtkjtvnio.sHtML

[R05] 参数默认值
来源：http://www.m.share.hesvh.cn/Article/details/gjwmrdbnc.sHtML

name="${1:-default}"
来源：http://baike.fehbvm.com/Article/details/grztafizs.sHtML

[R06] 判断命令是否存在
来源：http://baike.fehbvm.com/Article/details/ghdmsuafo.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://blog.zdbjq.cn/Article/details/gwuulfary.sHtML

[R07] if 判断文件
来源：http://www.m.share.fehbvm.com/Article/details/gnubocuuo.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.blog.hesvh.cn/Article/details/grkmpyoke.sHtML

[R08] 数值比较
来源：http://www.blog.fehbvm.com/Article/details/guvytthrm.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://m.share.zdbjq.cn/Article/details/gqyyiemyy.sHtML

[R09] 字符串比较
来源：http://wap.hesvh.cn/Article/details/gsxctygjk.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.share.zdbjq.cn/Article/details/gmadvqpfm.sHtML

[R10] 正则匹配
来源：http://www.blog.fehbvm.com/Article/details/gkngxoalz.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.share.zdbjq.cn/Article/details/gwhhszihu.sHtML

[R11] case 多分支
来源：http://www.blog.hesvh.cn/Article/details/gjlrnqfhv.sHtML

case "$1" in
来源：http://blog.zdbjq.cn/Article/details/gdfojfqbu.sHtML

start) echo "启动" ;;
来源：http://read.share.hesvh.cn/Article/details/gqyuhxbih.sHtML

stop)  echo "停止" ;;
来源：http://3g.hesvh.cn/Article/details/gikqpzuvw.sHtML

*)     echo "未知命令" ;;
来源：http://3g.fehbvm.com/Article/details/gbhhushex.sHtML

esac
来源：http://read.share.fehbvm.com/Article/details/guumraqgd.sHtML

[R12] for 遍历文件
来源：http://baike.fehbvm.com/Article/details/gqfhqgafk.sHtML

for f in *.txt; do echo "$f"; done
来源：http://m.share.hesvh.cn/Article/details/gmebesmmo.sHtML

[R13] for 计数循环
来源：http://www.blog.zdbjq.cn/Article/details/glljhfwep.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://blog.hesvh.cn/Article/details/gdizauapq.sHtML

[R14] C 风格 for
来源：http://www.m.share.hesvh.cn/Article/details/gcobgqfjk.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://baike.fehbvm.com/Article/details/gjxiltcmq.sHtML

[R15] while 逐行读文件
来源：http://www.blog.zdbjq.cn/Article/details/ghkgdgmee.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://baike.zdbjq.cn/Article/details/gckkaqzsx.sHtML

[R16] until 等待条件
来源：http://baike.hesvh.cn/Article/details/gbokdgcvq.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://wap.fehbvm.com/Article/details/gbtmejycg.sHtML

[R17] 数组定义与取值
来源：http://read.share.zdbjq.cn/Article/details/gugychtbb.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://mobile.hesvh.cn/Article/details/gxvnfkpkt.sHtML

[R18] 遍历数组
来源：http://read.share.zdbjq.cn/Article/details/gkxncrkbr.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.blog.hesvh.cn/Article/details/gvipgzpks.sHtML

[R19] 数组长度
来源：http://3g.zdbjq.cn/Article/details/gqrfcmbiu.sHtML

echo "${#arr[@]}"
来源：http://mobile.fehbvm.com/Article/details/gmpegojuh.sHtML

[R20] 关联数组（字典）
来源：http://mobile.fehbvm.com/Article/details/gtindkdvn.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.share.hesvh.cn/Article/details/gwbhjpihq.sHtML

[R21] 字符串长度
来源：http://www.share.fehbvm.com/Article/details/gbdxhapfo.sHtML

echo "${#s}"
来源：http://mobile.fehbvm.com/Article/details/gdcbiefjs.sHtML

[R22] 截取子串
来源：http://read.share.zdbjq.cn/Article/details/gdledzpzy.sHtML

echo "${s:0:5}"
来源：http://mobile.fehbvm.com/Article/details/gubrrxeqt.sHtML

[R23] 字符串替换
来源：http://www.blog.fehbvm.com/Article/details/grxcoxxwg.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://m.share.zdbjq.cn/Article/details/gzezjoaat.sHtML

[R24] 大小写转换
来源：http://3g.zdbjq.cn/Article/details/gxpulkopv.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://m.share.hesvh.cn/Article/details/giafkctvo.sHtML

[R25] 去后缀 / 去前缀
来源：http://m.share.zdbjq.cn/Article/details/goxdjfjzv.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://3g.zdbjq.cn/Article/details/gwjdbincx.sHtML

[R26] 命令替换
来源：http://mobile.fehbvm.com/Article/details/gcnxvsybb.sHtML

now=$(date +%F); echo "$now"
来源：http://read.share.hesvh.cn/Article/details/gguqllyux.sHtML

[R27] 算术展开
来源：http://www.share.hesvh.cn/Article/details/ggoetqmfz.sHtML

echo $((1 + 2 * 3))
来源：http://blog.fehbvm.com/Article/details/gjuexqwgt.sHtML

[R28] 浮点运算
来源：http://read.share.hesvh.cn/Article/details/gemyewzxp.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.share.zdbjq.cn/Article/details/gzplrlhws.sHtML

[R29] 定义函数
来源：http://www.share.zdbjq.cn/Article/details/gmounbdxw.sHtML


<!-- 参考信息 -->