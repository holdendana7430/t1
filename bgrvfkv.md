代发 wailian999

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpvtjecjd.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.fanxiaobao.xyz/Article/details/gdoyjjska.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.fanxiaobao.xyz/Article/details/gzsnkusix.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.fanxiaobao.xyz/Article/details/guqpmggqh.sHtML

Java: list.size();  map.size();  s.length()
来源：http://blog.fanxiaobao.xyz/Article/details/gskezhkie.sHtML

Go:   len(arr);  len(m)
来源：http://m.share.fanxiaobao.xyz/Article/details/glmrfrwne.sHtML

Ruby: x.length;  x.size
来源：http://www.share.fanxiaobao.xyz/Article/details/gjmmdjyoe.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://m.share.fanxiaobao.xyz/Article/details/gkeehzdli.sHtML

[P05] 判断两个对象内容是否相等
来源：http://baike.fanxiaobao.xyz/Article/details/gamooznjn.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://mobile.fanxiaobao.xyz/Article/details/genaywscc.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://wap.fanxiaobao.xyz/Article/details/gkpycpptc.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://blog.fanxiaobao.xyz/Article/details/glyjqfhpa.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://m.share.fanxiaobao.xyz/Article/details/gmmqpnuew.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://baike.fanxiaobao.xyz/Article/details/ghicnbjsn.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://wap.fanxiaobao.xyz/Article/details/geaciwwmp.sHtML

Ruby: a == b
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gytvifgrc.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsmubzqpc.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://mobile.fanxiaobao.xyz/Article/details/grgiyddmy.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://3g.fanxiaobao.xyz/Article/details/gdxvkyfil.sHtML

PHP:  if (empty($x)) {}
来源：http://3g.fanxiaobao.xyz/Article/details/gafqvzegg.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.share.fanxiaobao.xyz/Article/details/gvdsxhxyq.sHtML

TS:   if (x == null) {}
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvsckyqgx.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.share.fanxiaobao.xyz/Article/details/gfqlbtraa.sHtML

Go:   if x == nil {}
来源：http://3g.fanxiaobao.xyz/Article/details/gwhwxzwcm.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goercuxhb.sHtML

C#:   if (x is null) {}
来源：http://3g.fanxiaobao.xyz/Article/details/grnlctyck.sHtML

[P07] 防抖与节流
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gguiokwod.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdjsvclyk.sHtML

PHP:  // 手写时间戳比较
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbkkyyvhc.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gooypryyt.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.fanxiaobao.xyz/Article/details/gmhxdtlfr.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://wap.fanxiaobao.xyz/Article/details/gibiytmdf.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsiiyrdjf.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://read.share.fanxiaobao.xyz/Article/details/gkvurrazi.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://blog.fanxiaobao.xyz/Article/details/gwvxpscfq.sHtML

[P08] 处理浮点精度问题
来源：http://read.share.fanxiaobao.xyz/Article/details/gkkopbpmj.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://3g.fanxiaobao.xyz/Article/details/glayqtboc.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://wap.fanxiaobao.xyz/Article/details/ghgtpnvbt.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://mobile.fanxiaobao.xyz/Article/details/gssxanigl.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://blog.fanxiaobao.xyz/Article/details/ghdjydpbb.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://read.share.fanxiaobao.xyz/Article/details/gcpenegil.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://3g.fanxiaobao.xyz/Article/details/gkgolatvo.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.share.fanxiaobao.xyz/Article/details/gfesawcij.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://wap.fanxiaobao.xyz/Article/details/gkbvmnerq.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gceyyimsx.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.share.fanxiaobao.xyz/Article/details/galyqmtvq.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gveeiqber.sHtML

[Q01] 创建表
来源：http://blog.fanxiaobao.xyz/Article/details/gpbaygkfl.sHtML

CREATE TABLE users (
来源：http://blog.fanxiaobao.xyz/Article/details/grnidmqjb.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.fanxiaobao.xyz/Article/details/gvtfqndpk.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.share.fanxiaobao.xyz/Article/details/gqbqjkeqt.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.blog.fanxiaobao.xyz/Article/details/gypnaqopx.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://m.share.fanxiaobao.xyz/Article/details/gnocmbxka.sHtML

);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzxnlovry.sHtML

[Q02] 创建带外键的表
来源：http://baike.fanxiaobao.xyz/Article/details/glsaalhxw.sHtML

CREATE TABLE orders (
来源：http://baike.fanxiaobao.xyz/Article/details/ghpnweisu.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtdipykst.sHtML

user_id INT NOT NULL,
来源：http://www.share.fanxiaobao.xyz/Article/details/gloiljrqq.sHtML

amount DECIMAL(10, 2),
来源：http://baike.fanxiaobao.xyz/Article/details/gnjijedsc.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.share.fanxiaobao.xyz/Article/details/gtlismaxp.sHtML

);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbtnvbtio.sHtML

[Q03] 增加列
来源：http://read.share.fanxiaobao.xyz/Article/details/glemclfqi.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://mobile.fanxiaobao.xyz/Article/details/gtzadipzf.sHtML

[Q04] 修改列类型
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjjlctfws.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://wap.fanxiaobao.xyz/Article/details/gnlbyvoqo.sHtML

[Q05] 重命名列
来源：http://www.share.fanxiaobao.xyz/Article/details/ghldonckt.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://wap.fanxiaobao.xyz/Article/details/goqwgwxwa.sHtML

[Q06] 删除列
来源：http://baike.fanxiaobao.xyz/Article/details/gwpkvaktk.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.share.fanxiaobao.xyz/Article/details/gmaobbean.sHtML

[Q07] 删除表
来源：http://www.share.fanxiaobao.xyz/Article/details/gworfvdsv.sHtML

DROP TABLE IF EXISTS orders;
来源：http://mobile.fanxiaobao.xyz/Article/details/gsjoeakwy.sHtML

[Q08] 创建普通索引
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggjhxgmiy.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://m.share.fanxiaobao.xyz/Article/details/gaovsowle.sHtML

[Q09] 创建唯一索引
来源：http://blog.fanxiaobao.xyz/Article/details/getivpdyy.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.share.fanxiaobao.xyz/Article/details/gfpmlnjat.sHtML

[Q10] 插入单行
来源：http://wap.fanxiaobao.xyz/Article/details/gvrpktacu.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghbqpsglz.sHtML

[Q11] 一次插入多行
来源：http://m.share.fanxiaobao.xyz/Article/details/gxcfncamw.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://mobile.fanxiaobao.xyz/Article/details/gxcnsjosg.sHtML

[Q12] 插入后取自增 ID
来源：http://www.blog.fanxiaobao.xyz/Article/details/gocamjtyh.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://m.share.fanxiaobao.xyz/Article/details/gifbnrppv.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://wap.fanxiaobao.xyz/Article/details/gfivsotbj.sHtML

[Q13] 忽略重复插入
来源：http://read.share.fanxiaobao.xyz/Article/details/gtorcxmih.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://baike.fanxiaobao.xyz/Article/details/gwthqzrmi.sHtML

[Q14] 存在则更新（upsert）
来源：http://m.share.fanxiaobao.xyz/Article/details/goaxftrdl.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://mobile.fanxiaobao.xyz/Article/details/gwxxdmguf.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://baike.fanxiaobao.xyz/Article/details/ggkhzknpx.sHtML

[Q15] 查询全部
来源：http://www.blog.fanxiaobao.xyz/Article/details/gummcuyzz.sHtML

SELECT * FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gejwphczj.sHtML

[Q16] 查询指定列
来源：http://www.share.fanxiaobao.xyz/Article/details/gjglshzen.sHtML

SELECT id, name FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gogmdqgwy.sHtML

[Q17] 条件查询
来源：http://www.share.fanxiaobao.xyz/Article/details/gbqijutjx.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmtowjwbk.sHtML

[Q18] 模糊匹配
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gatmqkjot.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://3g.fanxiaobao.xyz/Article/details/gmupzlaev.sHtML

[Q19] 范围查询
来源：http://wap.fanxiaobao.xyz/Article/details/gfzqjreka.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://baike.fanxiaobao.xyz/Article/details/gkhwwhrxw.sHtML

[Q20] IN 列表
来源：http://baike.fanxiaobao.xyz/Article/details/goztsfbcd.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://mobile.fanxiaobao.xyz/Article/details/gdjakrmbw.sHtML

[Q21] 空值判断
来源：http://read.share.fanxiaobao.xyz/Article/details/gelpqdbkc.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://blog.fanxiaobao.xyz/Article/details/ginpdqzzy.sHtML

[Q22] 排序
来源：http://read.share.fanxiaobao.xyz/Article/details/gbxydrums.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://baike.fanxiaobao.xyz/Article/details/gxuzxtwgc.sHtML

[Q23] 分页
来源：http://wap.fanxiaobao.xyz/Article/details/gyxafehen.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://baike.fanxiaobao.xyz/Article/details/gjmupuzpk.sHtML

[Q24] 去重
来源：http://m.share.fanxiaobao.xyz/Article/details/gwxkvmmvd.sHtML

SELECT DISTINCT city FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gyjlinslr.sHtML

[Q25] 只取前 N 条
来源：http://wap.fanxiaobao.xyz/Article/details/gzeeuzufx.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://wap.fanxiaobao.xyz/Article/details/gcbmkzvcn.sHtML

[Q26] 计数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gamjkmzbb.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpfjodjxe.sHtML

[Q27] 条件计数
来源：http://www.blog.fanxiaobao.xyz/Article/details/glpqkkefj.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/ginbkwtfm.sHtML

[Q28] 求和与平均
来源：http://mobile.fanxiaobao.xyz/Article/details/gubvcbvqa.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.share.fanxiaobao.xyz/Article/details/gdyzwnfbw.sHtML

[Q29] 最大最小值
来源：http://wap.fanxiaobao.xyz/Article/details/ggezvsuri.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gxbgalzcd.sHtML

[Q30] 分组统计
来源：http://baike.fanxiaobao.xyz/Article/details/gvxtgycmi.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://read.share.fanxiaobao.xyz/Article/details/ggvaxyzcl.sHtML

[Q31] 分组后过滤
来源：http://www.blog.fanxiaobao.xyz/Article/details/gajhqphqg.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://mobile.fanxiaobao.xyz/Article/details/gkarhqjea.sHtML

[Q32] 分组拼接字符串
来源：http://baike.fanxiaobao.xyz/Article/details/gosuuspcz.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwnsfshxk.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.blog.fanxiaobao.xyz/Article/details/gabmmhitr.sHtML

[Q33] 多列分组
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjkityvit.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://wap.fanxiaobao.xyz/Article/details/gszvwghln.sHtML

[Q34] 每组取第一条
来源：http://wap.fanxiaobao.xyz/Article/details/godqinxlw.sHtML

SELECT * FROM (
来源：http://www.share.fanxiaobao.xyz/Article/details/glyyjxvdp.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://3g.fanxiaobao.xyz/Article/details/gvnemovyx.sHtML

) t WHERE rn = 1;
来源：http://wap.fanxiaobao.xyz/Article/details/grkpeiwsc.sHtML

[Q35] 内连接
来源：http://blog.fanxiaobao.xyz/Article/details/gvfredfmr.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://mobile.fanxiaobao.xyz/Article/details/ggyclfwxf.sHtML

[Q36] 左连接
来源：http://www.share.fanxiaobao.xyz/Article/details/gvboshqow.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://baike.fanxiaobao.xyz/Article/details/glkradvbp.sHtML

[Q37] 右连接
来源：http://www.blog.fanxiaobao.xyz/Article/details/gezzpxqgu.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzesesybj.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://read.share.fanxiaobao.xyz/Article/details/gcxqonlfz.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gajecbdek.sHtML

[Q39] 自连接（查上下级）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/getuafykr.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://blog.fanxiaobao.xyz/Article/details/ganazdzje.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghgqmeaeg.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://wap.fanxiaobao.xyz/Article/details/grrikoqfd.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://mobile.fanxiaobao.xyz/Article/details/gfqyijhqe.sHtML

[Q41] 多表连接
来源：http://wap.fanxiaobao.xyz/Article/details/gbbcafykk.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://baike.fanxiaobao.xyz/Article/details/gbdowavrf.sHtML

JOIN users u ON u.id = o.user_id
来源：http://baike.fanxiaobao.xyz/Article/details/gkrqkwfyi.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://wap.fanxiaobao.xyz/Article/details/gzhexkqmc.sHtML

[Q42] 连接条件附加过滤
来源：http://www.share.fanxiaobao.xyz/Article/details/gylxiwlgf.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqqtzquop.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsdazppuu.sHtML

[Q43] 标量子查询
来源：http://3g.fanxiaobao.xyz/Article/details/gicuxnpff.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwgqceyap.sHtML

[Q44] IN 子查询
来源：http://read.share.fanxiaobao.xyz/Article/details/gpggnlokj.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://wap.fanxiaobao.xyz/Article/details/gucwewzqn.sHtML

[Q45] EXISTS 判断存在
来源：http://3g.fanxiaobao.xyz/Article/details/gelnunvry.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.fanxiaobao.xyz/Article/details/guswroocn.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.share.fanxiaobao.xyz/Article/details/gremrgpsv.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.fanxiaobao.xyz/Article/details/gpadgdddn.sHtML

[Q47] 与平均值比较
来源：http://wap.fanxiaobao.xyz/Article/details/gdawzlkag.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcjtyqsjc.sHtML

[Q48] CTE 公用表表达式
来源：http://read.share.fanxiaobao.xyz/Article/details/gkcqiaxre.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://blog.fanxiaobao.xyz/Article/details/gwheoxsif.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://blog.fanxiaobao.xyz/Article/details/givyheyyw.sHtML

[Q49] 更新单行
来源：http://read.share.fanxiaobao.xyz/Article/details/gtspbikfd.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.share.fanxiaobao.xyz/Article/details/giqrlshxm.sHtML

[Q50] 批量更新
来源：http://3g.fanxiaobao.xyz/Article/details/gkjwuuise.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsbquexaf.sHtML

[Q51] 用子查询更新
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtxamozhh.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.share.fanxiaobao.xyz/Article/details/ggfymyiqq.sHtML

[Q52] 删除指定行
来源：http://blog.fanxiaobao.xyz/Article/details/grmnyxmnx.sHtML

DELETE FROM users WHERE id = 10;
来源：http://blog.fanxiaobao.xyz/Article/details/ggdbqyzau.sHtML

[Q53] 按条件删除
来源：http://read.share.fanxiaobao.xyz/Article/details/ghjraueyd.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://m.share.fanxiaobao.xyz/Article/details/gxsqribxu.sHtML

[Q54] 清空表
来源：http://read.share.fanxiaobao.xyz/Article/details/gbxhcehwq.sHtML

TRUNCATE TABLE logs;
来源：http://mobile.fanxiaobao.xyz/Article/details/gygpznfbf.sHtML

[Q55] 排名（并列占位）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqgdziuxg.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.share.fanxiaobao.xyz/Article/details/gbbezqccq.sHtML

[Q56] 密集排名（并列不占位）
来源：http://baike.fanxiaobao.xyz/Article/details/giucwuweq.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://mobile.fanxiaobao.xyz/Article/details/ghrgcipnt.sHtML

[Q57] 行号
来源：http://wap.fanxiaobao.xyz/Article/details/gjhnhomdf.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/grrvsirra.sHtML

[Q58] 累计求和
来源：http://mobile.fanxiaobao.xyz/Article/details/gjlonknwj.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.blog.fanxiaobao.xyz/Article/details/glejtqmzt.sHtML

[Q59] 分组内累计
来源：http://mobile.fanxiaobao.xyz/Article/details/gkjruygvd.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://baike.fanxiaobao.xyz/Article/details/gfxbgeoss.sHtML

[Q60] 取上一行 / 下一行
来源：http://m.share.fanxiaobao.xyz/Article/details/glsypqavc.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://m.share.fanxiaobao.xyz/Article/details/goodftvpl.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://wap.fanxiaobao.xyz/Article/details/gnqsftvks.sHtML

[Q61] 移动平均
来源：http://mobile.fanxiaobao.xyz/Article/details/gophgygqm.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://blog.fanxiaobao.xyz/Article/details/gmognyeso.sHtML

[Q62] 分组占比
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkryrzpya.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://m.share.fanxiaobao.xyz/Article/details/gykfaxkys.sHtML

[Q63] 开启事务
来源：http://www.share.fanxiaobao.xyz/Article/details/gaprmlmrr.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://m.share.fanxiaobao.xyz/Article/details/gnekshavl.sHtML

[Q64] 提交事务
来源：http://m.share.fanxiaobao.xyz/Article/details/gssncxttp.sHtML

COMMIT;
来源：http://wap.fanxiaobao.xyz/Article/details/gwdbadebn.sHtML

[Q65] 回滚事务
来源：http://www.share.fanxiaobao.xyz/Article/details/gmjparbyk.sHtML

ROLLBACK;
来源：http://wap.fanxiaobao.xyz/Article/details/grxdfeltj.sHtML

[Q66] 行锁查询
来源：http://blog.fanxiaobao.xyz/Article/details/giqzczsum.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://m.share.fanxiaobao.xyz/Article/details/gtduidinf.sHtML

[Q67] 设置隔离级别
来源：http://m.share.fanxiaobao.xyz/Article/details/gorulxbnd.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://read.share.fanxiaobao.xyz/Article/details/gwsfoectw.sHtML

[Q68] 保存点
来源：http://3g.fanxiaobao.xyz/Article/details/gmmreulbp.sHtML

SAVEPOINT sp1;
来源：http://read.share.fanxiaobao.xyz/Article/details/gahycpgem.sHtML

ROLLBACK TO sp1;
来源：http://baike.fanxiaobao.xyz/Article/details/gkdmhtgwp.sHtML

[Q69] 查看执行计划
来源：http://mobile.fanxiaobao.xyz/Article/details/ggdhujfsw.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbxzrtkyz.sHtML

[Q70] 更新统计信息
来源：http://3g.fanxiaobao.xyz/Article/details/gyglohabe.sHtML

ANALYZE TABLE users;
来源：http://baike.fanxiaobao.xyz/Article/details/grbacpvsm.sHtML

[Q71] 查看建表语句
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghwcwnufv.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://read.share.fanxiaobao.xyz/Article/details/gexfifqlt.sHtML

[Q72] 查看索引
来源：http://www.blog.fanxiaobao.xyz/Article/details/gojvwvvxj.sHtML

SHOW INDEX FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gmpjfnpto.sHtML

[Q73] 查看表状态
来源：http://read.share.fanxiaobao.xyz/Article/details/gnztxerly.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://3g.fanxiaobao.xyz/Article/details/gguvhmyjr.sHtML

[Q74] 强制使用索引
来源：http://www.share.fanxiaobao.xyz/Article/details/gonqxvere.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://read.share.fanxiaobao.xyz/Article/details/ghmdenwuk.sHtML

[Q75] 日期格式化
来源：http://baike.fanxiaobao.xyz/Article/details/gqkokzmdi.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://m.share.fanxiaobao.xyz/Article/details/gcyqgfsvj.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://wap.fanxiaobao.xyz/Article/details/giqstgfcl.sHtML

[Q76] 按天统计
来源：http://3g.fanxiaobao.xyz/Article/details/gbyyathye.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.share.fanxiaobao.xyz/Article/details/gblygdttw.sHtML

[Q77] 时间加减
来源：http://www.share.fanxiaobao.xyz/Article/details/glqklgysf.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvgnbhidu.sHtML

[Q78] 当前时间
来源：http://blog.fanxiaobao.xyz/Article/details/gynwsgnbs.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://m.share.fanxiaobao.xyz/Article/details/gjojmxswg.sHtML

[Q79] 字符串拼接
来源：http://3g.fanxiaobao.xyz/Article/details/gesevukhe.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.share.fanxiaobao.xyz/Article/details/gjkpkpolv.sHtML

[Q80] 字符串截取
来源：http://mobile.fanxiaobao.xyz/Article/details/gdlsasgpb.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gdbvxlucv.sHtML

[Q81] 字符串替换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcghxwbuc.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gpkxgmjah.sHtML

[Q82] 字符长度与字节长度
来源：http://baike.fanxiaobao.xyz/Article/details/gdtgqudqv.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/grudsswuc.sHtML

[Q83] 大小写转换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gljvsiodc.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gazwojwct.sHtML

[Q84] 去除首尾空格
来源：http://blog.fanxiaobao.xyz/Article/details/gzrnmecxz.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/guwoniowt.sHtML

[Q85] 数值取整
来源：http://m.share.fanxiaobao.xyz/Article/details/gqywikofe.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://baike.fanxiaobao.xyz/Article/details/gxjfuioel.sHtML

[Q86] 读取 JSON 字段
来源：http://read.share.fanxiaobao.xyz/Article/details/guhefqaeh.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://mobile.fanxiaobao.xyz/Article/details/gjyxvnppk.sHtML

[Q87] JSON 字段做条件
来源：http://m.share.fanxiaobao.xyz/Article/details/gdrazpdko.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://wap.fanxiaobao.xyz/Article/details/gtneicsar.sHtML

[Q88] 行转列（条件聚合）
来源：http://read.share.fanxiaobao.xyz/Article/details/gfxwgpwue.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gitmzbnrz.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvaobqfqn.sHtML

[Q89] 判断表是否存在
来源：http://m.share.fanxiaobao.xyz/Article/details/gzgrjsogc.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://wap.fanxiaobao.xyz/Article/details/ggcjnurkt.sHtML

[Q90] 生成序号列
来源：http://blog.fanxiaobao.xyz/Article/details/gicgblbrd.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://3g.fanxiaobao.xyz/Article/details/gttmyewvi.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gioxulvjl.sHtML

R. Bash 专题
来源：http://blog.fanxiaobao.xyz/Article/details/gtuepopag.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gfrrctqko.sHtML

[R01] shebang 与严格模式
来源：http://wap.fanxiaobao.xyz/Article/details/gsngnihab.sHtML

#!/usr/bin/env bash
来源：http://read.share.fanxiaobao.xyz/Article/details/gufwtezbe.sHtML

set -euo pipefail
来源：http://3g.fanxiaobao.xyz/Article/details/gdodruzce.sHtML

[R02] 变量赋值与使用
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxpcekjec.sHtML

name="Tom"; echo "$name"
来源：http://wap.fanxiaobao.xyz/Article/details/gataylbck.sHtML

[R03] 只读变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gzlbokbzx.sHtML

readonly PI=3.14
来源：http://m.share.fanxiaobao.xyz/Article/details/gtgyhetwo.sHtML

[R04] 位置参数
来源：http://mobile.fanxiaobao.xyz/Article/details/gipwbvmvu.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gitjytnbc.sHtML

[R05] 参数默认值
来源：http://www.share.fanxiaobao.xyz/Article/details/gsmrlrwjw.sHtML

name="${1:-default}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggmhqfmkr.sHtML

[R06] 判断命令是否存在
来源：http://blog.fanxiaobao.xyz/Article/details/glwdynqjs.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gkeeamule.sHtML

[R07] if 判断文件
来源：http://baike.fanxiaobao.xyz/Article/details/gnhcrxuyr.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glcsqesfl.sHtML

[R08] 数值比较
来源：http://wap.fanxiaobao.xyz/Article/details/gyjppdabb.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpwzlwimk.sHtML

[R09] 字符串比较
来源：http://3g.fanxiaobao.xyz/Article/details/guctxhtrk.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://wap.fanxiaobao.xyz/Article/details/gajppnxtf.sHtML

[R10] 正则匹配
来源：http://baike.fanxiaobao.xyz/Article/details/grsbkshsj.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gceeqbsno.sHtML

[R11] case 多分支
来源：http://baike.fanxiaobao.xyz/Article/details/gshepvrnb.sHtML

case "$1" in
来源：http://3g.fanxiaobao.xyz/Article/details/gebcfvskm.sHtML

start) echo "启动" ;;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gllqirugf.sHtML

stop)  echo "停止" ;;
来源：http://baike.fanxiaobao.xyz/Article/details/gpiwsfqbr.sHtML

*)     echo "未知命令" ;;
来源：http://3g.fanxiaobao.xyz/Article/details/gvbzcqhxn.sHtML

esac
来源：http://baike.fanxiaobao.xyz/Article/details/grknuhdzl.sHtML

[R12] for 遍历文件
来源：http://3g.fanxiaobao.xyz/Article/details/gurshhrdx.sHtML

for f in *.txt; do echo "$f"; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gvlirzizb.sHtML

[R13] for 计数循环
来源：http://m.share.fanxiaobao.xyz/Article/details/gtpqjsntn.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdovthoyu.sHtML

[R14] C 风格 for
来源：http://wap.fanxiaobao.xyz/Article/details/glqclvdzu.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://blog.fanxiaobao.xyz/Article/details/goveqjmrv.sHtML

[R15] while 逐行读文件
来源：http://baike.fanxiaobao.xyz/Article/details/grbtltagm.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjcggxyzj.sHtML

[R16] until 等待条件
来源：http://www.share.fanxiaobao.xyz/Article/details/gbkcbozvu.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpwjimbww.sHtML

[R17] 数组定义与取值
来源：http://www.blog.fanxiaobao.xyz/Article/details/gilayqjdy.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://3g.fanxiaobao.xyz/Article/details/gisqshbfp.sHtML

[R18] 遍历数组
来源：http://blog.fanxiaobao.xyz/Article/details/gtmhcxjzz.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://wap.fanxiaobao.xyz/Article/details/glxjqpair.sHtML

[R19] 数组长度
来源：http://read.share.fanxiaobao.xyz/Article/details/gzbqddiom.sHtML

echo "${#arr[@]}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gzxrofzsa.sHtML

[R20] 关联数组（字典）
来源：http://blog.fanxiaobao.xyz/Article/details/gveppolvf.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://blog.fanxiaobao.xyz/Article/details/gqcjpyzre.sHtML

[R21] 字符串长度
来源：http://www.share.fanxiaobao.xyz/Article/details/grqgadcrm.sHtML


<!-- 参考信息 -->