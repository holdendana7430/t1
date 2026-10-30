代发 wailian999

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.fehbvm.com/Article/details/gvzlmnziu.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://read.share.zdbjq.cn/Article/details/gydpxqbkd.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://mobile.hesvh.cn/Article/details/gcxrrpxan.sHtML

Ruby: a == b
来源：http://wap.fehbvm.com/Article/details/gvjylzbyv.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://baike.zdbjq.cn/Article/details/gdcpdgwry.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://read.share.hesvh.cn/Article/details/gsjysnimv.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://wap.hesvh.cn/Article/details/gjrsduwcg.sHtML

PHP:  if (empty($x)) {}
来源：http://baike.hesvh.cn/Article/details/gopwyxkfo.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.m.share.fehbvm.com/Article/details/gjmcaxask.sHtML

TS:   if (x == null) {}
来源：http://mobile.zdbjq.cn/Article/details/golkrpsuo.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.m.share.fehbvm.com/Article/details/gjoeytcid.sHtML

Go:   if x == nil {}
来源：http://read.share.zdbjq.cn/Article/details/gkfwpzkab.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://read.share.zdbjq.cn/Article/details/gilzcjaud.sHtML

C#:   if (x is null) {}
来源：http://m.share.hesvh.cn/Article/details/gmdelnfje.sHtML

[P07] 防抖与节流
来源：http://www.share.zdbjq.cn/Article/details/gmkxipabh.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://3g.hesvh.cn/Article/details/gdovrhekm.sHtML

PHP:  // 手写时间戳比较
来源：http://wap.hesvh.cn/Article/details/gnuhikhlr.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.fehbvm.com/Article/details/gffxqpnve.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.hesvh.cn/Article/details/gjnkgjkxa.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://blog.zdbjq.cn/Article/details/gojnjwxzv.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.share.fehbvm.com/Article/details/gmjzsxjcm.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.m.share.zdbjq.cn/Article/details/gfzkggweh.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.share.zdbjq.cn/Article/details/grlmmfefl.sHtML

[P08] 处理浮点精度问题
来源：http://3g.zdbjq.cn/Article/details/gxmqxpsjd.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://wap.hesvh.cn/Article/details/grbwyihyt.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://blog.hesvh.cn/Article/details/gbfabahgo.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://m.share.hesvh.cn/Article/details/gvwklvvpv.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://wap.hesvh.cn/Article/details/gjivdtehk.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://3g.zdbjq.cn/Article/details/gmsanpkom.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://blog.fehbvm.com/Article/details/gxqhtnteu.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://wap.hesvh.cn/Article/details/gcttckhqd.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.blog.zdbjq.cn/Article/details/gjyywqcuo.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gveaknyhe.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.share.hesvh.cn/Article/details/ggknzedgs.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gynyvrcze.sHtML

[Q01] 创建表
来源：http://read.share.hesvh.cn/Article/details/gplxblszk.sHtML

CREATE TABLE users (
来源：http://blog.fehbvm.com/Article/details/gfnittrhm.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.hesvh.cn/Article/details/ghtufrkjs.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.blog.fehbvm.com/Article/details/gwfwnlwrz.sHtML

email VARCHAR(100) UNIQUE,
来源：http://read.share.fehbvm.com/Article/details/gmhghfzbl.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.blog.zdbjq.cn/Article/details/gfyfkbfee.sHtML

);
来源：http://wap.hesvh.cn/Article/details/gdwqhxqta.sHtML

[Q02] 创建带外键的表
来源：http://blog.zdbjq.cn/Article/details/ghwobwuwb.sHtML

CREATE TABLE orders (
来源：http://baike.hesvh.cn/Article/details/grdairqoy.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.zdbjq.cn/Article/details/gkvffuykv.sHtML

user_id INT NOT NULL,
来源：http://www.share.fehbvm.com/Article/details/glhjmnjki.sHtML

amount DECIMAL(10, 2),
来源：http://blog.fehbvm.com/Article/details/ghaifmtni.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.m.share.zdbjq.cn/Article/details/gnikkczdq.sHtML

);
来源：http://mobile.zdbjq.cn/Article/details/gosvbbwgc.sHtML

[Q03] 增加列
来源：http://www.blog.zdbjq.cn/Article/details/gajfskgpf.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://blog.hesvh.cn/Article/details/gufjrwwzc.sHtML

[Q04] 修改列类型
来源：http://wap.zdbjq.cn/Article/details/giarpdlcb.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://wap.hesvh.cn/Article/details/gpxjkdopf.sHtML

[Q05] 重命名列
来源：http://blog.hesvh.cn/Article/details/gqpksmfzu.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://blog.fehbvm.com/Article/details/gwbwndmcn.sHtML

[Q06] 删除列
来源：http://read.share.fehbvm.com/Article/details/gxrrcnxbz.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.m.share.zdbjq.cn/Article/details/gawtcpqht.sHtML

[Q07] 删除表
来源：http://baike.hesvh.cn/Article/details/grxdcgstm.sHtML

DROP TABLE IF EXISTS orders;
来源：http://mobile.fehbvm.com/Article/details/gkiepwavt.sHtML

[Q08] 创建普通索引
来源：http://mobile.zdbjq.cn/Article/details/gxvcryhge.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://mobile.hesvh.cn/Article/details/gfsbdoxwh.sHtML

[Q09] 创建唯一索引
来源：http://blog.zdbjq.cn/Article/details/gahfzffng.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.m.share.fehbvm.com/Article/details/ghzwwkvrj.sHtML

[Q10] 插入单行
来源：http://www.blog.zdbjq.cn/Article/details/gyrmntsmw.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://read.share.fehbvm.com/Article/details/gqqergrzm.sHtML

[Q11] 一次插入多行
来源：http://3g.zdbjq.cn/Article/details/gtwogaigf.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://baike.hesvh.cn/Article/details/gukbjtone.sHtML

[Q12] 插入后取自增 ID
来源：http://3g.hesvh.cn/Article/details/gznhvkhrf.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.blog.hesvh.cn/Article/details/grgomejat.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://3g.hesvh.cn/Article/details/gogdmsepe.sHtML

[Q13] 忽略重复插入
来源：http://baike.fehbvm.com/Article/details/grepgeaqo.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://wap.zdbjq.cn/Article/details/grphevnaf.sHtML

[Q14] 存在则更新（upsert）
来源：http://blog.zdbjq.cn/Article/details/gakgfvtit.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://baike.fehbvm.com/Article/details/gikuwelwa.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.m.share.hesvh.cn/Article/details/giscfmggq.sHtML

[Q15] 查询全部
来源：http://wap.hesvh.cn/Article/details/goducqpdw.sHtML

SELECT * FROM users;
来源：http://m.share.hesvh.cn/Article/details/gormzvdhx.sHtML

[Q16] 查询指定列
来源：http://www.blog.hesvh.cn/Article/details/gkvoltpsa.sHtML

SELECT id, name FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/ganobzfiv.sHtML

[Q17] 条件查询
来源：http://blog.fehbvm.com/Article/details/gxqbvzjum.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://mobile.hesvh.cn/Article/details/goshjqbji.sHtML

[Q18] 模糊匹配
来源：http://www.share.hesvh.cn/Article/details/gmuzxsela.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://wap.zdbjq.cn/Article/details/gcwbkucxt.sHtML

[Q19] 范围查询
来源：http://baike.fehbvm.com/Article/details/gswsiiuga.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://read.share.fehbvm.com/Article/details/gmrbqcsad.sHtML

[Q20] IN 列表
来源：http://baike.zdbjq.cn/Article/details/gpeizvbqd.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.share.fehbvm.com/Article/details/grlexkgmq.sHtML

[Q21] 空值判断
来源：http://3g.hesvh.cn/Article/details/gyrzghakq.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://3g.zdbjq.cn/Article/details/gzrblbewc.sHtML

[Q22] 排序
来源：http://mobile.fehbvm.com/Article/details/gwngtwxse.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://mobile.zdbjq.cn/Article/details/gncectdwt.sHtML

[Q23] 分页
来源：http://m.share.zdbjq.cn/Article/details/gxzmzxjkd.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://baike.fehbvm.com/Article/details/gkkwnzxrd.sHtML

[Q24] 去重
来源：http://mobile.fehbvm.com/Article/details/glcdcdsub.sHtML

SELECT DISTINCT city FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gkhkwxuft.sHtML

[Q25] 只取前 N 条
来源：http://baike.hesvh.cn/Article/details/gdpfysalo.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://read.share.zdbjq.cn/Article/details/gbejcempb.sHtML

[Q26] 计数
来源：http://3g.zdbjq.cn/Article/details/gqcmmuyje.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.blog.hesvh.cn/Article/details/grtaayhou.sHtML

[Q27] 条件计数
来源：http://3g.fehbvm.com/Article/details/ggfdbflyr.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gtviphdmq.sHtML

[Q28] 求和与平均
来源：http://3g.fehbvm.com/Article/details/gcqtnhykd.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://read.share.fehbvm.com/Article/details/gkosupymh.sHtML

[Q29] 最大最小值
来源：http://mobile.zdbjq.cn/Article/details/ghmgslbyh.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://wap.fehbvm.com/Article/details/ghsumydrj.sHtML

[Q30] 分组统计
来源：http://mobile.zdbjq.cn/Article/details/giciscdjy.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://wap.fehbvm.com/Article/details/gmdmbmmnm.sHtML

[Q31] 分组后过滤
来源：http://wap.zdbjq.cn/Article/details/ggzxqpivl.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://mobile.hesvh.cn/Article/details/gsokvacdw.sHtML

[Q32] 分组拼接字符串
来源：http://baike.hesvh.cn/Article/details/gxhpumsfm.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.m.share.fehbvm.com/Article/details/gtnropait.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://mobile.fehbvm.com/Article/details/gjocyywpm.sHtML

[Q33] 多列分组
来源：http://3g.fehbvm.com/Article/details/gxhoilqxs.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://mobile.fehbvm.com/Article/details/gnfzwvpms.sHtML

[Q34] 每组取第一条
来源：http://www.share.hesvh.cn/Article/details/gewuhlixi.sHtML

SELECT * FROM (
来源：http://www.share.fehbvm.com/Article/details/gnppxcomg.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://m.share.fehbvm.com/Article/details/gbazlttnt.sHtML

) t WHERE rn = 1;
来源：http://read.share.fehbvm.com/Article/details/guerutufp.sHtML

[Q35] 内连接
来源：http://www.blog.fehbvm.com/Article/details/gcrazlrbi.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://m.share.zdbjq.cn/Article/details/gstelzkdh.sHtML

[Q36] 左连接
来源：http://blog.zdbjq.cn/Article/details/gfxotyrfx.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://wap.zdbjq.cn/Article/details/gioulrpzx.sHtML

[Q37] 右连接
来源：http://blog.zdbjq.cn/Article/details/gwezsrzix.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.share.fehbvm.com/Article/details/gbwxdcbgi.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.blog.zdbjq.cn/Article/details/gxkojgqjm.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.blog.hesvh.cn/Article/details/gymofwvff.sHtML

[Q39] 自连接（查上下级）
来源：http://baike.fehbvm.com/Article/details/gmkjvlepf.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://baike.fehbvm.com/Article/details/gkdixubrt.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://3g.hesvh.cn/Article/details/gutephped.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.blog.fehbvm.com/Article/details/gxclywyad.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.blog.fehbvm.com/Article/details/gjrrcuhop.sHtML

[Q41] 多表连接
来源：http://3g.fehbvm.com/Article/details/gorbjylzk.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.blog.zdbjq.cn/Article/details/gyvjiqlgv.sHtML

JOIN users u ON u.id = o.user_id
来源：http://read.share.zdbjq.cn/Article/details/gxgwqcniq.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.m.share.hesvh.cn/Article/details/gywyqnzrn.sHtML

[Q42] 连接条件附加过滤
来源：http://www.share.zdbjq.cn/Article/details/gswdqzujl.sHtML

SELECT u.name, o.amount FROM users u
来源：http://mobile.fehbvm.com/Article/details/gvpausmqw.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.share.zdbjq.cn/Article/details/gbbtfgilg.sHtML

[Q43] 标量子查询
来源：http://mobile.zdbjq.cn/Article/details/goileirxy.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.blog.fehbvm.com/Article/details/gyxprxbwe.sHtML

[Q44] IN 子查询
来源：http://m.share.zdbjq.cn/Article/details/gyganbiih.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://wap.hesvh.cn/Article/details/gkriczvqk.sHtML

[Q45] EXISTS 判断存在
来源：http://3g.fehbvm.com/Article/details/gwuzsthgg.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.fehbvm.com/Article/details/gsitewqpd.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.share.hesvh.cn/Article/details/guhabvzra.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.hesvh.cn/Article/details/gxcldnnki.sHtML

[Q47] 与平均值比较
来源：http://3g.hesvh.cn/Article/details/ghxyzside.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://wap.zdbjq.cn/Article/details/gghlllmcc.sHtML

[Q48] CTE 公用表表达式
来源：http://mobile.hesvh.cn/Article/details/gzxuxbgxg.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://m.share.zdbjq.cn/Article/details/gmowtgqby.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://wap.hesvh.cn/Article/details/gxnpiocfq.sHtML

[Q49] 更新单行
来源：http://read.share.fehbvm.com/Article/details/gvcjtivud.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://3g.zdbjq.cn/Article/details/gxkhozjrm.sHtML

[Q50] 批量更新
来源：http://blog.zdbjq.cn/Article/details/gekhtjnmg.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://mobile.zdbjq.cn/Article/details/gigvcpvya.sHtML

[Q51] 用子查询更新
来源：http://3g.zdbjq.cn/Article/details/gkvvvgyzu.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://mobile.zdbjq.cn/Article/details/gudfmoejd.sHtML

[Q52] 删除指定行
来源：http://www.share.fehbvm.com/Article/details/gdpnsrjbt.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.blog.hesvh.cn/Article/details/gfpscjoiw.sHtML

[Q53] 按条件删除
来源：http://read.share.hesvh.cn/Article/details/grkadsxar.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.m.share.zdbjq.cn/Article/details/giqtniwjx.sHtML

[Q54] 清空表
来源：http://www.share.fehbvm.com/Article/details/gryqsydzw.sHtML

TRUNCATE TABLE logs;
来源：http://blog.fehbvm.com/Article/details/gldqnyfho.sHtML

[Q55] 排名（并列占位）
来源：http://blog.zdbjq.cn/Article/details/ggmwrhsvf.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://m.share.hesvh.cn/Article/details/gbhdgactz.sHtML

[Q56] 密集排名（并列不占位）
来源：http://m.share.hesvh.cn/Article/details/goowzeaxw.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://mobile.fehbvm.com/Article/details/guwyenpeh.sHtML

[Q57] 行号
来源：http://blog.zdbjq.cn/Article/details/gimoamdsu.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://mobile.hesvh.cn/Article/details/gnarjihsg.sHtML

[Q58] 累计求和
来源：http://www.m.share.fehbvm.com/Article/details/gdspmdfex.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://baike.zdbjq.cn/Article/details/gqlvxczxw.sHtML

[Q59] 分组内累计
来源：http://read.share.fehbvm.com/Article/details/gbmdrqdha.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.share.zdbjq.cn/Article/details/gqpfdcezq.sHtML

[Q60] 取上一行 / 下一行
来源：http://mobile.fehbvm.com/Article/details/gzwqjjdzm.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://3g.zdbjq.cn/Article/details/gsoxdfrxv.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://mobile.zdbjq.cn/Article/details/gkymhbefw.sHtML

[Q61] 移动平均
来源：http://www.m.share.hesvh.cn/Article/details/gbwpxxjcq.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://wap.hesvh.cn/Article/details/gepfwsrfy.sHtML

[Q62] 分组占比
来源：http://www.m.share.zdbjq.cn/Article/details/gqyabsiee.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://mobile.zdbjq.cn/Article/details/gtvxcgdfn.sHtML

[Q63] 开启事务
来源：http://baike.fehbvm.com/Article/details/gwonwhvgb.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://baike.hesvh.cn/Article/details/gchvtvoph.sHtML

[Q64] 提交事务
来源：http://3g.zdbjq.cn/Article/details/gjxwfoyql.sHtML

COMMIT;
来源：http://blog.fehbvm.com/Article/details/gdbwhhgur.sHtML

[Q65] 回滚事务
来源：http://www.share.hesvh.cn/Article/details/gcvylbciu.sHtML

ROLLBACK;
来源：http://3g.fehbvm.com/Article/details/gtovmkjcq.sHtML

[Q66] 行锁查询
来源：http://blog.fehbvm.com/Article/details/gsoqtxtox.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://wap.hesvh.cn/Article/details/gdrjxgryo.sHtML

[Q67] 设置隔离级别
来源：http://mobile.zdbjq.cn/Article/details/glxirtgmt.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://3g.hesvh.cn/Article/details/gtqlpicoj.sHtML

[Q68] 保存点
来源：http://blog.zdbjq.cn/Article/details/gwmszzmjm.sHtML

SAVEPOINT sp1;
来源：http://read.share.hesvh.cn/Article/details/gqpryglws.sHtML

ROLLBACK TO sp1;
来源：http://3g.hesvh.cn/Article/details/gjkntndah.sHtML

[Q69] 查看执行计划
来源：http://baike.hesvh.cn/Article/details/gcltdjors.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.m.share.fehbvm.com/Article/details/gljptqjyy.sHtML

[Q70] 更新统计信息
来源：http://mobile.zdbjq.cn/Article/details/greyrjaas.sHtML

ANALYZE TABLE users;
来源：http://blog.hesvh.cn/Article/details/ggyqrsyxw.sHtML

[Q71] 查看建表语句
来源：http://www.blog.fehbvm.com/Article/details/gjgktwlbe.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://read.share.hesvh.cn/Article/details/gndsuluma.sHtML

[Q72] 查看索引
来源：http://read.share.zdbjq.cn/Article/details/gawhdvbkq.sHtML

SHOW INDEX FROM users;
来源：http://read.share.hesvh.cn/Article/details/gpweaimou.sHtML

[Q73] 查看表状态
来源：http://baike.fehbvm.com/Article/details/giuamdgai.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://mobile.hesvh.cn/Article/details/gxhqecdpr.sHtML

[Q74] 强制使用索引
来源：http://www.blog.zdbjq.cn/Article/details/gabjkoccv.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.m.share.hesvh.cn/Article/details/gvdqsvrvv.sHtML

[Q75] 日期格式化
来源：http://www.share.hesvh.cn/Article/details/ghviqbeku.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://3g.fehbvm.com/Article/details/gldtpjlka.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://blog.zdbjq.cn/Article/details/gdvnrrgzz.sHtML

[Q76] 按天统计
来源：http://www.share.hesvh.cn/Article/details/gnitvdoor.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.m.share.fehbvm.com/Article/details/gzjmmppua.sHtML

[Q77] 时间加减
来源：http://www.m.share.zdbjq.cn/Article/details/gbobavfvw.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://mobile.fehbvm.com/Article/details/gcdgwnuhq.sHtML

[Q78] 当前时间
来源：http://mobile.zdbjq.cn/Article/details/guxrdtkbb.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://mobile.zdbjq.cn/Article/details/ghffagtgz.sHtML

[Q79] 字符串拼接
来源：http://www.blog.fehbvm.com/Article/details/ghvmvdmbr.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.share.hesvh.cn/Article/details/gvnvhaypw.sHtML

[Q80] 字符串截取
来源：http://www.share.zdbjq.cn/Article/details/girxzasle.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://baike.zdbjq.cn/Article/details/guviklcwc.sHtML

[Q81] 字符串替换
来源：http://mobile.fehbvm.com/Article/details/guywrjckj.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://mobile.fehbvm.com/Article/details/ggeiagbvf.sHtML

[Q82] 字符长度与字节长度
来源：http://blog.fehbvm.com/Article/details/gqsozpvnb.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://3g.zdbjq.cn/Article/details/gyksdjgom.sHtML

[Q83] 大小写转换
来源：http://blog.zdbjq.cn/Article/details/gdxclvucn.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.share.fehbvm.com/Article/details/gcernbddn.sHtML

[Q84] 去除首尾空格
来源：http://baike.fehbvm.com/Article/details/gcwgnacjo.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gencqzfxr.sHtML

[Q85] 数值取整
来源：http://blog.zdbjq.cn/Article/details/glrezjrbk.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.blog.zdbjq.cn/Article/details/geokjlwte.sHtML

[Q86] 读取 JSON 字段
来源：http://wap.hesvh.cn/Article/details/gswzdeifi.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://read.share.fehbvm.com/Article/details/gcaxjuulu.sHtML

[Q87] JSON 字段做条件
来源：http://baike.hesvh.cn/Article/details/gbdmyhuvn.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://blog.zdbjq.cn/Article/details/gwwmpiafe.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.blog.fehbvm.com/Article/details/gynbdgdtg.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.blog.fehbvm.com/Article/details/gbxujhmut.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://blog.fehbvm.com/Article/details/gppzzdafi.sHtML

[Q89] 判断表是否存在
来源：http://www.m.share.fehbvm.com/Article/details/godrennhk.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://3g.zdbjq.cn/Article/details/gcrcwijdf.sHtML

[Q90] 生成序号列
来源：http://www.m.share.fehbvm.com/Article/details/gwarvpbrb.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://mobile.hesvh.cn/Article/details/gdgxcempt.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gbggydwxs.sHtML

R. Bash 专题
来源：http://www.blog.zdbjq.cn/Article/details/gflnmfpar.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/goobrrdyj.sHtML

[R01] shebang 与严格模式
来源：http://baike.hesvh.cn/Article/details/ghwxeqbvq.sHtML

#!/usr/bin/env bash
来源：http://blog.fehbvm.com/Article/details/gejoemstr.sHtML

set -euo pipefail
来源：http://3g.zdbjq.cn/Article/details/gtbohjgmo.sHtML

[R02] 变量赋值与使用
来源：http://read.share.hesvh.cn/Article/details/ghkxgjsjq.sHtML

name="Tom"; echo "$name"
来源：http://blog.zdbjq.cn/Article/details/gnwhiwfkh.sHtML

[R03] 只读变量
来源：http://blog.fehbvm.com/Article/details/ghzhxexds.sHtML

readonly PI=3.14
来源：http://www.share.fehbvm.com/Article/details/gbghassmd.sHtML

[R04] 位置参数
来源：http://3g.hesvh.cn/Article/details/gpmxcabhn.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://m.share.fehbvm.com/Article/details/gzxgikxkc.sHtML

[R05] 参数默认值
来源：http://read.share.zdbjq.cn/Article/details/gmumhcvpa.sHtML

name="${1:-default}"
来源：http://wap.hesvh.cn/Article/details/gqldzixgo.sHtML

[R06] 判断命令是否存在
来源：http://www.m.share.fehbvm.com/Article/details/gexyurelk.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.m.share.hesvh.cn/Article/details/gecmkofni.sHtML

[R07] if 判断文件
来源：http://www.share.hesvh.cn/Article/details/gmbcdjuro.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://blog.hesvh.cn/Article/details/gikifeond.sHtML

[R08] 数值比较
来源：http://www.share.zdbjq.cn/Article/details/gkqfbneiq.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://read.share.hesvh.cn/Article/details/gapmxvprx.sHtML

[R09] 字符串比较
来源：http://wap.zdbjq.cn/Article/details/gzmfpcenk.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://3g.hesvh.cn/Article/details/gbvaohifl.sHtML

[R10] 正则匹配
来源：http://www.blog.fehbvm.com/Article/details/gfuktndfg.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://3g.zdbjq.cn/Article/details/gjnawpjpj.sHtML

[R11] case 多分支
来源：http://mobile.zdbjq.cn/Article/details/gupviaoco.sHtML

case "$1" in
来源：http://3g.hesvh.cn/Article/details/gsutimqlb.sHtML

start) echo "启动" ;;
来源：http://blog.zdbjq.cn/Article/details/gnjqbhvlv.sHtML

stop)  echo "停止" ;;
来源：http://www.m.share.hesvh.cn/Article/details/gajxriakx.sHtML

*)     echo "未知命令" ;;
来源：http://blog.hesvh.cn/Article/details/gdojbdjsw.sHtML

esac
来源：http://3g.zdbjq.cn/Article/details/gdokztqbe.sHtML

[R12] for 遍历文件
来源：http://m.share.zdbjq.cn/Article/details/gwczqvjwc.sHtML

for f in *.txt; do echo "$f"; done
来源：http://blog.hesvh.cn/Article/details/geybwcuuj.sHtML

[R13] for 计数循环
来源：http://read.share.hesvh.cn/Article/details/gjdvredpl.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://baike.zdbjq.cn/Article/details/ggzmumhtt.sHtML

[R14] C 风格 for
来源：http://wap.zdbjq.cn/Article/details/gwelwrkhy.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://wap.hesvh.cn/Article/details/gfzzmrmzt.sHtML

[R15] while 逐行读文件
来源：http://wap.zdbjq.cn/Article/details/gtkwrzpeb.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://m.share.fehbvm.com/Article/details/gzifzxzsw.sHtML

[R16] until 等待条件
来源：http://wap.fehbvm.com/Article/details/gmvlsajji.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://3g.hesvh.cn/Article/details/gkpztwbri.sHtML

[R17] 数组定义与取值
来源：http://read.share.fehbvm.com/Article/details/gzlckqbrg.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://blog.fehbvm.com/Article/details/gftdedeho.sHtML

[R18] 遍历数组
来源：http://www.blog.hesvh.cn/Article/details/gosyoogwk.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://wap.fehbvm.com/Article/details/gwhndtkcd.sHtML

[R19] 数组长度
来源：http://baike.fehbvm.com/Article/details/gcdlbtjmm.sHtML

echo "${#arr[@]}"
来源：http://www.blog.fehbvm.com/Article/details/gxixzmyxh.sHtML

[R20] 关联数组（字典）
来源：http://www.m.share.fehbvm.com/Article/details/gfnkqiawm.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://blog.hesvh.cn/Article/details/gktepsgrt.sHtML

[R21] 字符串长度
来源：http://wap.hesvh.cn/Article/details/gobsniojz.sHtML

echo "${#s}"
来源：http://www.share.fehbvm.com/Article/details/gxiirxjcf.sHtML

[R22] 截取子串
来源：http://blog.hesvh.cn/Article/details/gfkzbkjms.sHtML

echo "${s:0:5}"
来源：http://m.share.fehbvm.com/Article/details/gfqaaxwze.sHtML

[R23] 字符串替换
来源：http://wap.zdbjq.cn/Article/details/gtnsligge.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://mobile.zdbjq.cn/Article/details/ghnfdmwdo.sHtML

[R24] 大小写转换
来源：http://wap.zdbjq.cn/Article/details/gsyxvfhzs.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.share.zdbjq.cn/Article/details/ghmlcwkil.sHtML

[R25] 去后缀 / 去前缀
来源：http://mobile.hesvh.cn/Article/details/graoajiyu.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.blog.zdbjq.cn/Article/details/gmrgfdhnc.sHtML

[R26] 命令替换
来源：http://3g.zdbjq.cn/Article/details/gszbinbxh.sHtML

now=$(date +%F); echo "$now"
来源：http://www.share.fehbvm.com/Article/details/gyhjktxvj.sHtML

[R27] 算术展开
来源：http://mobile.hesvh.cn/Article/details/glfiqtwuo.sHtML


<!-- 参考信息 -->