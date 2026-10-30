代发 wailian999

Py:   len(x)            # 字符串、列表、字典通用
来源：http://baike.zdbjq.cn/Article/details/gfnjdovzh.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.zdbjq.cn/Article/details/gdphxhmao.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.zdbjq.cn/Article/details/gdelwranq.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.hesvh.cn/Article/details/gddosayyd.sHtML

Java: list.size();  map.size();  s.length()
来源：http://baike.fehbvm.com/Article/details/gfuzyegev.sHtML

Go:   len(arr);  len(m)
来源：http://www.blog.fehbvm.com/Article/details/gdshvmmnp.sHtML

Ruby: x.length;  x.size
来源：http://blog.zdbjq.cn/Article/details/gbdcpardo.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://read.share.fehbvm.com/Article/details/gyyoskwwx.sHtML

[P05] 判断两个对象内容是否相等
来源：http://read.share.zdbjq.cn/Article/details/gpgxgpdsr.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.share.fehbvm.com/Article/details/groghvpbd.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://m.share.fehbvm.com/Article/details/gflbjzyqd.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://blog.fehbvm.com/Article/details/glqwkuakw.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://baike.fehbvm.com/Article/details/gbosujqqa.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://m.share.zdbjq.cn/Article/details/gqtjgiuol.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://m.share.zdbjq.cn/Article/details/gytuedltn.sHtML

Ruby: a == b
来源：http://baike.fehbvm.com/Article/details/gqyearpwe.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.blog.hesvh.cn/Article/details/gvfeaeist.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://wap.fehbvm.com/Article/details/gcniparhw.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://3g.hesvh.cn/Article/details/goylwojnt.sHtML

PHP:  if (empty($x)) {}
来源：http://www.share.fehbvm.com/Article/details/gbqwrxgsr.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://baike.hesvh.cn/Article/details/gulykzzkk.sHtML

TS:   if (x == null) {}
来源：http://www.blog.hesvh.cn/Article/details/gxtwamkmi.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://wap.hesvh.cn/Article/details/gesfxoxur.sHtML

Go:   if x == nil {}
来源：http://3g.hesvh.cn/Article/details/gzdsplxfi.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://3g.fehbvm.com/Article/details/gmmxqxfmb.sHtML

C#:   if (x is null) {}
来源：http://m.share.fehbvm.com/Article/details/gillgasod.sHtML

[P07] 防抖与节流
来源：http://www.blog.hesvh.cn/Article/details/gwijulcrt.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://read.share.hesvh.cn/Article/details/ghaakvcmq.sHtML

PHP:  // 手写时间戳比较
来源：http://www.m.share.hesvh.cn/Article/details/gfbdydpoj.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.zdbjq.cn/Article/details/gcrnfuqnt.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.hesvh.cn/Article/details/gyiqvbyoe.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://mobile.hesvh.cn/Article/details/ggdavbwws.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.blog.fehbvm.com/Article/details/gkrcmceul.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://3g.fehbvm.com/Article/details/gqeztkakm.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://wap.zdbjq.cn/Article/details/gqaenegfq.sHtML

[P08] 处理浮点精度问题
来源：http://www.share.fehbvm.com/Article/details/gpkddbdzp.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://3g.hesvh.cn/Article/details/gjgyyzxvm.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://blog.hesvh.cn/Article/details/gapyshzcu.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://read.share.zdbjq.cn/Article/details/gwtpkfejw.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.blog.fehbvm.com/Article/details/gcxbpjkdm.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://3g.zdbjq.cn/Article/details/grhwhofmt.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://m.share.zdbjq.cn/Article/details/gysgmdodj.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.m.share.fehbvm.com/Article/details/gazshzmlu.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.share.hesvh.cn/Article/details/gsyigbpbw.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gdgekfhvi.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://baike.hesvh.cn/Article/details/gwnvcqhxj.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/guwotvqdz.sHtML

[Q01] 创建表
来源：http://read.share.fehbvm.com/Article/details/ghfmvkejq.sHtML

CREATE TABLE users (
来源：http://read.share.fehbvm.com/Article/details/gbzacfzrc.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.zdbjq.cn/Article/details/gidicbejl.sHtML

name VARCHAR(50) NOT NULL,
来源：http://wap.hesvh.cn/Article/details/glmostgit.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.m.share.fehbvm.com/Article/details/gnlckeedk.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.blog.hesvh.cn/Article/details/geshikaem.sHtML

);
来源：http://www.share.hesvh.cn/Article/details/ggrouhqvl.sHtML

[Q02] 创建带外键的表
来源：http://blog.zdbjq.cn/Article/details/gljrgwung.sHtML

CREATE TABLE orders (
来源：http://wap.hesvh.cn/Article/details/gbczcsuti.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.fehbvm.com/Article/details/gplnhvuaf.sHtML

user_id INT NOT NULL,
来源：http://blog.zdbjq.cn/Article/details/gyuvdkcir.sHtML

amount DECIMAL(10, 2),
来源：http://read.share.zdbjq.cn/Article/details/gdeveptag.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://blog.fehbvm.com/Article/details/gczqvskrt.sHtML

);
来源：http://baike.fehbvm.com/Article/details/grotxkkuq.sHtML

[Q03] 增加列
来源：http://m.share.hesvh.cn/Article/details/geskoxrjw.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.blog.fehbvm.com/Article/details/gfcurlzxl.sHtML

[Q04] 修改列类型
来源：http://baike.fehbvm.com/Article/details/ggedbseiy.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://blog.fehbvm.com/Article/details/gwloxaopw.sHtML

[Q05] 重命名列
来源：http://www.share.zdbjq.cn/Article/details/gezjvlptm.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.m.share.hesvh.cn/Article/details/gqxjvkrdz.sHtML

[Q06] 删除列
来源：http://blog.fehbvm.com/Article/details/ghuvmmbmu.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.share.hesvh.cn/Article/details/goojjbagr.sHtML

[Q07] 删除表
来源：http://baike.zdbjq.cn/Article/details/gcibpdvrn.sHtML

DROP TABLE IF EXISTS orders;
来源：http://3g.fehbvm.com/Article/details/ganvsmatg.sHtML

[Q08] 创建普通索引
来源：http://www.m.share.hesvh.cn/Article/details/gsxiuseip.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://m.share.hesvh.cn/Article/details/gyhzhowna.sHtML

[Q09] 创建唯一索引
来源：http://mobile.zdbjq.cn/Article/details/gycoccbca.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.blog.fehbvm.com/Article/details/gaagfblpn.sHtML

[Q10] 插入单行
来源：http://3g.hesvh.cn/Article/details/guakigxyb.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://mobile.hesvh.cn/Article/details/geqqqvigj.sHtML

[Q11] 一次插入多行
来源：http://read.share.fehbvm.com/Article/details/gyvmtspil.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://blog.fehbvm.com/Article/details/gbcjdphyb.sHtML

[Q12] 插入后取自增 ID
来源：http://baike.fehbvm.com/Article/details/gdsqbkdlm.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://m.share.hesvh.cn/Article/details/gnthnhhsf.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://3g.fehbvm.com/Article/details/gtovgjizn.sHtML

[Q13] 忽略重复插入
来源：http://www.m.share.fehbvm.com/Article/details/gswzauhbc.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://read.share.fehbvm.com/Article/details/gwalqmsly.sHtML

[Q14] 存在则更新（upsert）
来源：http://3g.fehbvm.com/Article/details/gxlpixciv.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://blog.fehbvm.com/Article/details/gxatteque.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://wap.zdbjq.cn/Article/details/gvnpgwhua.sHtML

[Q15] 查询全部
来源：http://m.share.zdbjq.cn/Article/details/glgzixjhf.sHtML

SELECT * FROM users;
来源：http://read.share.fehbvm.com/Article/details/gsxfnjtrc.sHtML

[Q16] 查询指定列
来源：http://mobile.fehbvm.com/Article/details/gmenrjezc.sHtML

SELECT id, name FROM users;
来源：http://mobile.fehbvm.com/Article/details/gqxwyltpd.sHtML

[Q17] 条件查询
来源：http://www.m.share.zdbjq.cn/Article/details/gqbcxavaq.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://wap.hesvh.cn/Article/details/gbfxmjnjh.sHtML

[Q18] 模糊匹配
来源：http://m.share.fehbvm.com/Article/details/glplvmvzo.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.m.share.hesvh.cn/Article/details/gqpovnfnd.sHtML

[Q19] 范围查询
来源：http://3g.fehbvm.com/Article/details/gbwxoijsi.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://m.share.zdbjq.cn/Article/details/gyiymzpew.sHtML

[Q20] IN 列表
来源：http://baike.hesvh.cn/Article/details/gufpmhmwq.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://mobile.fehbvm.com/Article/details/grqfgkbvb.sHtML

[Q21] 空值判断
来源：http://www.blog.fehbvm.com/Article/details/giibcgxwn.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://blog.hesvh.cn/Article/details/gufuedthe.sHtML

[Q22] 排序
来源：http://baike.fehbvm.com/Article/details/gxnwohqle.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://3g.zdbjq.cn/Article/details/gkbnlbeao.sHtML

[Q23] 分页
来源：http://m.share.hesvh.cn/Article/details/gsshcypfu.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://wap.zdbjq.cn/Article/details/gmcvwxnqm.sHtML

[Q24] 去重
来源：http://m.share.hesvh.cn/Article/details/gltsctnyu.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gvqstkzxi.sHtML

[Q25] 只取前 N 条
来源：http://blog.hesvh.cn/Article/details/gqgtuqvil.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.m.share.fehbvm.com/Article/details/gleuyxmuv.sHtML

[Q26] 计数
来源：http://baike.zdbjq.cn/Article/details/gtdemxdun.sHtML

SELECT COUNT(*) FROM users;
来源：http://3g.fehbvm.com/Article/details/gqysbeoxx.sHtML

[Q27] 条件计数
来源：http://www.blog.hesvh.cn/Article/details/gcncelhoq.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://m.share.fehbvm.com/Article/details/gerhaallb.sHtML

[Q28] 求和与平均
来源：http://blog.zdbjq.cn/Article/details/gycghfitv.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.share.hesvh.cn/Article/details/gzusjkwxg.sHtML

[Q29] 最大最小值
来源：http://www.m.share.hesvh.cn/Article/details/gmkzjcnfj.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.share.fehbvm.com/Article/details/gglbmezqu.sHtML

[Q30] 分组统计
来源：http://mobile.fehbvm.com/Article/details/gncqsbkhk.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.blog.zdbjq.cn/Article/details/gsankacbq.sHtML

[Q31] 分组后过滤
来源：http://blog.fehbvm.com/Article/details/gfabsdgvn.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.m.share.hesvh.cn/Article/details/gmpmprcnt.sHtML

[Q32] 分组拼接字符串
来源：http://www.blog.fehbvm.com/Article/details/gnvsnrgqn.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://baike.fehbvm.com/Article/details/glegcseam.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://read.share.fehbvm.com/Article/details/gzgmabuod.sHtML

[Q33] 多列分组
来源：http://www.share.zdbjq.cn/Article/details/gsyupitfp.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://blog.zdbjq.cn/Article/details/grduzqgwr.sHtML

[Q34] 每组取第一条
来源：http://baike.zdbjq.cn/Article/details/gzvgqjzmx.sHtML

SELECT * FROM (
来源：http://m.share.fehbvm.com/Article/details/gysoapugi.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://wap.fehbvm.com/Article/details/gyhagynnx.sHtML

) t WHERE rn = 1;
来源：http://www.share.fehbvm.com/Article/details/gvdaervvk.sHtML

[Q35] 内连接
来源：http://baike.fehbvm.com/Article/details/gzwbgolld.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://blog.zdbjq.cn/Article/details/gratlqpzw.sHtML

[Q36] 左连接
来源：http://read.share.fehbvm.com/Article/details/gtalittue.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://wap.fehbvm.com/Article/details/gkeqlctdo.sHtML

[Q37] 右连接
来源：http://www.share.hesvh.cn/Article/details/gjbesuzxf.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://read.share.hesvh.cn/Article/details/gfzwfpdqx.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://read.share.zdbjq.cn/Article/details/gqsbafrkb.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://blog.fehbvm.com/Article/details/gksnbwgfd.sHtML

[Q39] 自连接（查上下级）
来源：http://3g.hesvh.cn/Article/details/gixnahdvc.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://3g.hesvh.cn/Article/details/gzyxgdqaz.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://read.share.fehbvm.com/Article/details/ghmglysqz.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.blog.zdbjq.cn/Article/details/gekfegmus.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://3g.hesvh.cn/Article/details/glhbwigog.sHtML

[Q41] 多表连接
来源：http://www.m.share.hesvh.cn/Article/details/gbxisdenq.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://m.share.hesvh.cn/Article/details/gbreuopnr.sHtML

JOIN users u ON u.id = o.user_id
来源：http://m.share.hesvh.cn/Article/details/gwdxgesac.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://read.share.zdbjq.cn/Article/details/gzwyisqjx.sHtML

[Q42] 连接条件附加过滤
来源：http://wap.hesvh.cn/Article/details/glsrihfcr.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.m.share.fehbvm.com/Article/details/gevuajtkh.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://m.share.hesvh.cn/Article/details/ghegbwyom.sHtML

[Q43] 标量子查询
来源：http://read.share.hesvh.cn/Article/details/gbazzdkky.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://m.share.hesvh.cn/Article/details/gkhvnedvk.sHtML

[Q44] IN 子查询
来源：http://www.blog.zdbjq.cn/Article/details/gvwojjvfz.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://m.share.fehbvm.com/Article/details/gcsyvbruc.sHtML

[Q45] EXISTS 判断存在
来源：http://baike.fehbvm.com/Article/details/gidlbijif.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.fehbvm.com/Article/details/gpswcedlr.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.m.share.hesvh.cn/Article/details/gonhkctjj.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.zdbjq.cn/Article/details/gbbhyipax.sHtML

[Q47] 与平均值比较
来源：http://baike.hesvh.cn/Article/details/gwlovbbic.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://m.share.zdbjq.cn/Article/details/gezcxawuf.sHtML

[Q48] CTE 公用表表达式
来源：http://read.share.fehbvm.com/Article/details/gkrvrvwbl.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://blog.zdbjq.cn/Article/details/gunyvdbcf.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://read.share.zdbjq.cn/Article/details/ggmhybhul.sHtML

[Q49] 更新单行
来源：http://blog.hesvh.cn/Article/details/gboqhbwfq.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://blog.zdbjq.cn/Article/details/geeaxwjac.sHtML

[Q50] 批量更新
来源：http://wap.hesvh.cn/Article/details/gdeyakieq.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://wap.fehbvm.com/Article/details/gubdwhpgh.sHtML

[Q51] 用子查询更新
来源：http://blog.zdbjq.cn/Article/details/govirmjww.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://mobile.hesvh.cn/Article/details/gwdflezvf.sHtML

[Q52] 删除指定行
来源：http://mobile.zdbjq.cn/Article/details/gaseesixb.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.m.share.hesvh.cn/Article/details/gkehexdca.sHtML

[Q53] 按条件删除
来源：http://blog.fehbvm.com/Article/details/grqwmgaxk.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://mobile.fehbvm.com/Article/details/guyrupaca.sHtML

[Q54] 清空表
来源：http://www.m.share.zdbjq.cn/Article/details/ggrmkzrjf.sHtML

TRUNCATE TABLE logs;
来源：http://www.blog.zdbjq.cn/Article/details/gozbylkxa.sHtML

[Q55] 排名（并列占位）
来源：http://baike.zdbjq.cn/Article/details/gfslnzvor.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.m.share.zdbjq.cn/Article/details/gcfidatsr.sHtML

[Q56] 密集排名（并列不占位）
来源：http://blog.hesvh.cn/Article/details/gphezinwr.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://blog.zdbjq.cn/Article/details/gjbvmyjjb.sHtML

[Q57] 行号
来源：http://www.m.share.hesvh.cn/Article/details/gmujnkkrc.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gonyuhgyh.sHtML

[Q58] 累计求和
来源：http://www.blog.zdbjq.cn/Article/details/gcwhakgib.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://baike.zdbjq.cn/Article/details/glwnsknbr.sHtML

[Q59] 分组内累计
来源：http://baike.hesvh.cn/Article/details/gcwijfknn.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.m.share.zdbjq.cn/Article/details/gfyhlpbaw.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.blog.hesvh.cn/Article/details/ggwpymmgi.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.m.share.zdbjq.cn/Article/details/gzqabaggd.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.blog.hesvh.cn/Article/details/giphtqimn.sHtML

[Q61] 移动平均
来源：http://read.share.zdbjq.cn/Article/details/gmhcpbsbg.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.blog.hesvh.cn/Article/details/gxwejshyo.sHtML

[Q62] 分组占比
来源：http://3g.zdbjq.cn/Article/details/ghdsqucjv.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://read.share.fehbvm.com/Article/details/grprutxvy.sHtML

[Q63] 开启事务
来源：http://www.share.hesvh.cn/Article/details/gmhbbvzdt.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://wap.zdbjq.cn/Article/details/gdkayjdru.sHtML

[Q64] 提交事务
来源：http://www.blog.fehbvm.com/Article/details/gpwdpzlkw.sHtML

COMMIT;
来源：http://www.blog.zdbjq.cn/Article/details/gazqlpyek.sHtML

[Q65] 回滚事务
来源：http://www.blog.hesvh.cn/Article/details/gqtgdlfsg.sHtML

ROLLBACK;
来源：http://www.m.share.hesvh.cn/Article/details/gvwsgzjwc.sHtML

[Q66] 行锁查询
来源：http://www.m.share.zdbjq.cn/Article/details/giavxhpsx.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://read.share.fehbvm.com/Article/details/gmjfssang.sHtML

[Q67] 设置隔离级别
来源：http://baike.fehbvm.com/Article/details/gpzqnjllq.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://mobile.hesvh.cn/Article/details/gaixsjxfx.sHtML

[Q68] 保存点
来源：http://read.share.fehbvm.com/Article/details/ggzxyoehj.sHtML

SAVEPOINT sp1;
来源：http://blog.hesvh.cn/Article/details/gwnlgcmex.sHtML

ROLLBACK TO sp1;
来源：http://m.share.hesvh.cn/Article/details/gamfmcesp.sHtML

[Q69] 查看执行计划
来源：http://wap.fehbvm.com/Article/details/grvnqszwa.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.blog.hesvh.cn/Article/details/ggowhshhn.sHtML

[Q70] 更新统计信息
来源：http://www.share.zdbjq.cn/Article/details/grnipsqmh.sHtML

ANALYZE TABLE users;
来源：http://mobile.hesvh.cn/Article/details/gxnsgmcma.sHtML

[Q71] 查看建表语句
来源：http://m.share.fehbvm.com/Article/details/gmrbfrivr.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://mobile.fehbvm.com/Article/details/gizppzjsm.sHtML

[Q72] 查看索引
来源：http://www.share.fehbvm.com/Article/details/grynlirzw.sHtML

SHOW INDEX FROM users;
来源：http://wap.zdbjq.cn/Article/details/geksiuxmf.sHtML

[Q73] 查看表状态
来源：http://3g.fehbvm.com/Article/details/gjefmeyce.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.share.hesvh.cn/Article/details/gxugsycuz.sHtML

[Q74] 强制使用索引
来源：http://www.share.hesvh.cn/Article/details/gxjzqwjtv.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://3g.zdbjq.cn/Article/details/gmwzswrfe.sHtML

[Q75] 日期格式化
来源：http://www.share.zdbjq.cn/Article/details/glcesopvf.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://m.share.zdbjq.cn/Article/details/gqfuissmy.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://m.share.fehbvm.com/Article/details/guajyrdzx.sHtML

[Q76] 按天统计
来源：http://wap.hesvh.cn/Article/details/gkiiewady.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://read.share.fehbvm.com/Article/details/giutjvjpn.sHtML

[Q77] 时间加减
来源：http://www.blog.zdbjq.cn/Article/details/grsvzcygr.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://m.share.zdbjq.cn/Article/details/gbfoyqvlq.sHtML

[Q78] 当前时间
来源：http://blog.fehbvm.com/Article/details/gijaoqqkc.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://blog.zdbjq.cn/Article/details/gjezglshr.sHtML

[Q79] 字符串拼接
来源：http://www.blog.hesvh.cn/Article/details/gxltycmml.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://baike.zdbjq.cn/Article/details/gyoabxued.sHtML

[Q80] 字符串截取
来源：http://3g.fehbvm.com/Article/details/gkvygtcyr.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://blog.fehbvm.com/Article/details/gkvevuenk.sHtML

[Q81] 字符串替换
来源：http://baike.fehbvm.com/Article/details/gkfxoctbs.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://wap.hesvh.cn/Article/details/gcumlbykt.sHtML

[Q82] 字符长度与字节长度
来源：http://www.blog.hesvh.cn/Article/details/gsaycqata.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.share.hesvh.cn/Article/details/gnxkabbie.sHtML

[Q83] 大小写转换
来源：http://www.m.share.fehbvm.com/Article/details/gfnclrfao.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gmkfmgswf.sHtML

[Q84] 去除首尾空格
来源：http://mobile.hesvh.cn/Article/details/gzijwxjja.sHtML

SELECT TRIM(name) FROM users;
来源：http://3g.hesvh.cn/Article/details/gvepmfocn.sHtML

[Q85] 数值取整
来源：http://blog.zdbjq.cn/Article/details/gyzkdpuqc.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.m.share.zdbjq.cn/Article/details/gxbxofnmb.sHtML

[Q86] 读取 JSON 字段
来源：http://m.share.zdbjq.cn/Article/details/gfcdozgpb.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://wap.zdbjq.cn/Article/details/grwxeqdpn.sHtML

[Q87] JSON 字段做条件
来源：http://read.share.hesvh.cn/Article/details/goufqrorn.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.m.share.fehbvm.com/Article/details/gerxtgvzu.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.m.share.hesvh.cn/Article/details/gcwdrixfo.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://read.share.fehbvm.com/Article/details/gsynwvdwc.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gavstmruj.sHtML

[Q89] 判断表是否存在
来源：http://wap.hesvh.cn/Article/details/gpjskapjh.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://read.share.hesvh.cn/Article/details/ggvxlriaa.sHtML

[Q90] 生成序号列
来源：http://3g.fehbvm.com/Article/details/gvjizcete.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.blog.fehbvm.com/Article/details/gujyvsqnf.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gaetkycpv.sHtML

R. Bash 专题
来源：http://baike.zdbjq.cn/Article/details/gqwjwzpuy.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gysjrkbfk.sHtML

[R01] shebang 与严格模式
来源：http://blog.fehbvm.com/Article/details/gklzmhfiz.sHtML

#!/usr/bin/env bash
来源：http://baike.zdbjq.cn/Article/details/gzcphbzwm.sHtML

set -euo pipefail
来源：http://mobile.fehbvm.com/Article/details/gveytndhq.sHtML

[R02] 变量赋值与使用
来源：http://read.share.fehbvm.com/Article/details/gsenvisut.sHtML

name="Tom"; echo "$name"
来源：http://baike.zdbjq.cn/Article/details/gbcljdgwf.sHtML

[R03] 只读变量
来源：http://www.blog.fehbvm.com/Article/details/gfrbhpsao.sHtML

readonly PI=3.14
来源：http://m.share.hesvh.cn/Article/details/gshumkcxj.sHtML

[R04] 位置参数
来源：http://3g.hesvh.cn/Article/details/gfntdqxfz.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://wap.fehbvm.com/Article/details/gcysptcvl.sHtML

[R05] 参数默认值
来源：http://wap.zdbjq.cn/Article/details/gwqrrueeq.sHtML

name="${1:-default}"
来源：http://wap.fehbvm.com/Article/details/gkpeovntj.sHtML

[R06] 判断命令是否存在
来源：http://mobile.fehbvm.com/Article/details/gdkasiwhz.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.share.zdbjq.cn/Article/details/gqrwaavkv.sHtML

[R07] if 判断文件
来源：http://m.share.fehbvm.com/Article/details/ghacrqvdo.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://wap.zdbjq.cn/Article/details/gltudtjlc.sHtML

[R08] 数值比较
来源：http://read.share.fehbvm.com/Article/details/gdweazjme.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://read.share.fehbvm.com/Article/details/geqdluhkf.sHtML

[R09] 字符串比较
来源：http://m.share.zdbjq.cn/Article/details/ghpshwahw.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://wap.fehbvm.com/Article/details/guoftamsp.sHtML

[R10] 正则匹配
来源：http://mobile.zdbjq.cn/Article/details/gsllwvmmg.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://blog.hesvh.cn/Article/details/gvldmxypb.sHtML

[R11] case 多分支
来源：http://m.share.zdbjq.cn/Article/details/gwwxdrgyk.sHtML

case "$1" in
来源：http://www.blog.fehbvm.com/Article/details/gclidrnnb.sHtML

start) echo "启动" ;;
来源：http://3g.hesvh.cn/Article/details/gpwqvoakj.sHtML

stop)  echo "停止" ;;
来源：http://m.share.zdbjq.cn/Article/details/guqvcczzl.sHtML

*)     echo "未知命令" ;;
来源：http://read.share.hesvh.cn/Article/details/gqdmnzikz.sHtML

esac
来源：http://blog.zdbjq.cn/Article/details/gykyszjnd.sHtML

[R12] for 遍历文件
来源：http://www.share.hesvh.cn/Article/details/gwurdrdlc.sHtML

for f in *.txt; do echo "$f"; done
来源：http://baike.zdbjq.cn/Article/details/gmykyvvfk.sHtML

[R13] for 计数循环
来源：http://baike.zdbjq.cn/Article/details/grgbbvrvs.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://3g.zdbjq.cn/Article/details/gjgvzxryy.sHtML

[R14] C 风格 for
来源：http://read.share.fehbvm.com/Article/details/gqqiawmzv.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://wap.hesvh.cn/Article/details/gzjuaazxl.sHtML

[R15] while 逐行读文件
来源：http://mobile.fehbvm.com/Article/details/gpuajgdkd.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://wap.fehbvm.com/Article/details/guuybvhmg.sHtML

[R16] until 等待条件
来源：http://www.m.share.zdbjq.cn/Article/details/ghcnabpoj.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://blog.fehbvm.com/Article/details/gucobyinl.sHtML

[R17] 数组定义与取值
来源：http://mobile.hesvh.cn/Article/details/gtmchpsbk.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://mobile.hesvh.cn/Article/details/ghxykfwox.sHtML

[R18] 遍历数组
来源：http://3g.fehbvm.com/Article/details/gbrkazmsu.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.blog.zdbjq.cn/Article/details/gyutdgdxz.sHtML

[R19] 数组长度
来源：http://read.share.hesvh.cn/Article/details/gzducqyhu.sHtML

echo "${#arr[@]}"
来源：http://www.blog.hesvh.cn/Article/details/gpyzvlfpe.sHtML

[R20] 关联数组（字典）
来源：http://www.m.share.fehbvm.com/Article/details/gahquctfa.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://read.share.zdbjq.cn/Article/details/gvggyawau.sHtML

[R21] 字符串长度
来源：http://wap.hesvh.cn/Article/details/gbhplwlbx.sHtML


<!-- 参考信息 -->