代发 wailian999

[P05] 判断两个对象内容是否相等
来源：http://www.m.share.fehbvm.com/Article/details/guyoodqqd.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://read.share.fehbvm.com/Article/details/ghfqirkyo.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://mobile.fehbvm.com/Article/details/gzpvlpjff.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://read.share.hesvh.cn/Article/details/gbfolqpdc.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://read.share.zdbjq.cn/Article/details/giwpeepek.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://3g.hesvh.cn/Article/details/ghonekryf.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://mobile.hesvh.cn/Article/details/gbaeiqbcg.sHtML

Ruby: a == b
来源：http://read.share.hesvh.cn/Article/details/geaanbdck.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.blog.zdbjq.cn/Article/details/gknavfvcd.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://blog.fehbvm.com/Article/details/gqhwcdgmi.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.blog.zdbjq.cn/Article/details/gpjvoacpp.sHtML

PHP:  if (empty($x)) {}
来源：http://blog.zdbjq.cn/Article/details/gwhcrhwme.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://wap.hesvh.cn/Article/details/gjwqvzrnm.sHtML

TS:   if (x == null) {}
来源：http://mobile.fehbvm.com/Article/details/gvayzipht.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.m.share.fehbvm.com/Article/details/gghkkqtqr.sHtML

Go:   if x == nil {}
来源：http://m.share.hesvh.cn/Article/details/ggknshzzs.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://baike.fehbvm.com/Article/details/gssooptim.sHtML

C#:   if (x is null) {}
来源：http://www.blog.zdbjq.cn/Article/details/gnawsjjsn.sHtML

[P07] 防抖与节流
来源：http://mobile.zdbjq.cn/Article/details/gdodpvwot.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.m.share.hesvh.cn/Article/details/gftyvcxlv.sHtML

PHP:  // 手写时间戳比较
来源：http://baike.fehbvm.com/Article/details/gigcqptyf.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.zdbjq.cn/Article/details/gaswvaamo.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.fehbvm.com/Article/details/gknvtncyt.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://wap.fehbvm.com/Article/details/gbduoxxxd.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://baike.fehbvm.com/Article/details/gkwfwmnjz.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://baike.fehbvm.com/Article/details/ghrahgdnc.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://baike.hesvh.cn/Article/details/gnrdtakus.sHtML

[P08] 处理浮点精度问题
来源：http://www.blog.fehbvm.com/Article/details/gwjqzklkw.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://wap.fehbvm.com/Article/details/gvekontvb.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://mobile.hesvh.cn/Article/details/gjtiueukj.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://baike.hesvh.cn/Article/details/gkechajwg.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://mobile.fehbvm.com/Article/details/gbvykkopv.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.blog.hesvh.cn/Article/details/gpkiiovqp.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://wap.fehbvm.com/Article/details/gqutkylyh.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://mobile.zdbjq.cn/Article/details/gezrgmetx.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://baike.fehbvm.com/Article/details/gqddnrsfo.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gnglldstk.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.m.share.zdbjq.cn/Article/details/gamniebki.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gutntqzqb.sHtML

[Q01] 创建表
来源：http://www.share.hesvh.cn/Article/details/gggkxnhnl.sHtML

CREATE TABLE users (
来源：http://www.m.share.fehbvm.com/Article/details/gnqlychcg.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.zdbjq.cn/Article/details/gdwfyidpz.sHtML

name VARCHAR(50) NOT NULL,
来源：http://m.share.fehbvm.com/Article/details/gvbmdivcy.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.blog.zdbjq.cn/Article/details/glltfrxwa.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://wap.zdbjq.cn/Article/details/geiisaime.sHtML

);
来源：http://wap.hesvh.cn/Article/details/gxanmelfm.sHtML

[Q02] 创建带外键的表
来源：http://m.share.hesvh.cn/Article/details/gygqmmbgx.sHtML

CREATE TABLE orders (
来源：http://read.share.zdbjq.cn/Article/details/gunwstfbj.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.zdbjq.cn/Article/details/gpgczgbyp.sHtML

user_id INT NOT NULL,
来源：http://www.m.share.zdbjq.cn/Article/details/gtizdkdky.sHtML

amount DECIMAL(10, 2),
来源：http://blog.zdbjq.cn/Article/details/gmxqmhgsu.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://m.share.hesvh.cn/Article/details/gdtyroobt.sHtML

);
来源：http://baike.zdbjq.cn/Article/details/gdhscwihp.sHtML

[Q03] 增加列
来源：http://read.share.fehbvm.com/Article/details/gydfgppjk.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://mobile.fehbvm.com/Article/details/gtuuqbocf.sHtML

[Q04] 修改列类型
来源：http://www.m.share.fehbvm.com/Article/details/grifmnkqa.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.m.share.zdbjq.cn/Article/details/gjcrhzonf.sHtML

[Q05] 重命名列
来源：http://www.share.hesvh.cn/Article/details/gmxvdezes.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://m.share.zdbjq.cn/Article/details/ggoaheuvj.sHtML

[Q06] 删除列
来源：http://read.share.fehbvm.com/Article/details/golbkksrm.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://wap.zdbjq.cn/Article/details/gqsznzuqv.sHtML

[Q07] 删除表
来源：http://read.share.fehbvm.com/Article/details/gpgyrcxob.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.blog.fehbvm.com/Article/details/gmqbywodx.sHtML

[Q08] 创建普通索引
来源：http://wap.hesvh.cn/Article/details/gvitjolqs.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.m.share.fehbvm.com/Article/details/gnhautndm.sHtML

[Q09] 创建唯一索引
来源：http://www.share.hesvh.cn/Article/details/gpnefemen.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://baike.zdbjq.cn/Article/details/gmcxrroix.sHtML

[Q10] 插入单行
来源：http://www.m.share.fehbvm.com/Article/details/gwdaphktv.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://mobile.fehbvm.com/Article/details/gecixcefs.sHtML

[Q11] 一次插入多行
来源：http://read.share.hesvh.cn/Article/details/gjeycvstj.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://blog.zdbjq.cn/Article/details/gmrpvqrpp.sHtML

[Q12] 插入后取自增 ID
来源：http://www.m.share.fehbvm.com/Article/details/gqwgcekzb.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://mobile.fehbvm.com/Article/details/gkygnpoyt.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.blog.fehbvm.com/Article/details/gvieqzlkq.sHtML

[Q13] 忽略重复插入
来源：http://blog.zdbjq.cn/Article/details/gefqzvzpm.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://3g.fehbvm.com/Article/details/gsqpmxpup.sHtML

[Q14] 存在则更新（upsert）
来源：http://blog.zdbjq.cn/Article/details/gofhkvndh.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://blog.hesvh.cn/Article/details/gvtqpkbtx.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://read.share.hesvh.cn/Article/details/gffgkfpde.sHtML

[Q15] 查询全部
来源：http://blog.zdbjq.cn/Article/details/gokamvers.sHtML

SELECT * FROM users;
来源：http://blog.zdbjq.cn/Article/details/gnvpqjomg.sHtML

[Q16] 查询指定列
来源：http://mobile.zdbjq.cn/Article/details/gdgwbjpyg.sHtML

SELECT id, name FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gmsprqgzv.sHtML

[Q17] 条件查询
来源：http://3g.zdbjq.cn/Article/details/gckthzeov.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.m.share.zdbjq.cn/Article/details/gmmvbsqha.sHtML

[Q18] 模糊匹配
来源：http://blog.zdbjq.cn/Article/details/gbyqgyigg.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://3g.fehbvm.com/Article/details/ghfbphouz.sHtML

[Q19] 范围查询
来源：http://wap.hesvh.cn/Article/details/gpcilmuov.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://baike.zdbjq.cn/Article/details/garcbtgah.sHtML

[Q20] IN 列表
来源：http://www.blog.hesvh.cn/Article/details/gbrajhzel.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://read.share.fehbvm.com/Article/details/glkxlgoyr.sHtML

[Q21] 空值判断
来源：http://wap.zdbjq.cn/Article/details/gnowypaeu.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.blog.hesvh.cn/Article/details/guhenxbxa.sHtML

[Q22] 排序
来源：http://mobile.zdbjq.cn/Article/details/ggtrhwfsg.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.m.share.hesvh.cn/Article/details/gotloidzs.sHtML

[Q23] 分页
来源：http://m.share.hesvh.cn/Article/details/gjebymmsc.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://wap.hesvh.cn/Article/details/gfvriivnh.sHtML

[Q24] 去重
来源：http://read.share.zdbjq.cn/Article/details/ggxqogocv.sHtML

SELECT DISTINCT city FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gekikexwj.sHtML

[Q25] 只取前 N 条
来源：http://blog.zdbjq.cn/Article/details/gpjtqbjdn.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://blog.zdbjq.cn/Article/details/ggrdpcxwy.sHtML

[Q26] 计数
来源：http://www.share.zdbjq.cn/Article/details/gngyxsqhd.sHtML

SELECT COUNT(*) FROM users;
来源：http://baike.fehbvm.com/Article/details/gopheroin.sHtML

[Q27] 条件计数
来源：http://blog.hesvh.cn/Article/details/gagdsyxdy.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.share.hesvh.cn/Article/details/gwgutlugu.sHtML

[Q28] 求和与平均
来源：http://www.blog.fehbvm.com/Article/details/gcheglupq.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.m.share.fehbvm.com/Article/details/glhklcbew.sHtML

[Q29] 最大最小值
来源：http://m.share.zdbjq.cn/Article/details/gkuaezfgj.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://wap.zdbjq.cn/Article/details/gdlkgihya.sHtML

[Q30] 分组统计
来源：http://m.share.zdbjq.cn/Article/details/gvxjjxnyp.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.share.hesvh.cn/Article/details/gfomayfev.sHtML

[Q31] 分组后过滤
来源：http://www.m.share.hesvh.cn/Article/details/gnshiezhl.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.blog.fehbvm.com/Article/details/giehvtzfi.sHtML

[Q32] 分组拼接字符串
来源：http://blog.fehbvm.com/Article/details/godqvolmn.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://baike.fehbvm.com/Article/details/gtdjecrtc.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://3g.fehbvm.com/Article/details/gcfwrtlsm.sHtML

[Q33] 多列分组
来源：http://www.m.share.zdbjq.cn/Article/details/gmxtjrjru.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.blog.hesvh.cn/Article/details/gwbwofqep.sHtML

[Q34] 每组取第一条
来源：http://wap.fehbvm.com/Article/details/gqxzpihts.sHtML

SELECT * FROM (
来源：http://www.m.share.hesvh.cn/Article/details/gpphjpyfs.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://baike.fehbvm.com/Article/details/gpufoqdkv.sHtML

) t WHERE rn = 1;
来源：http://www.share.zdbjq.cn/Article/details/gripdtmta.sHtML

[Q35] 内连接
来源：http://read.share.hesvh.cn/Article/details/gqposqzqm.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://m.share.zdbjq.cn/Article/details/gkbdwdmqo.sHtML

[Q36] 左连接
来源：http://www.m.share.fehbvm.com/Article/details/gxlvnepdq.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://wap.fehbvm.com/Article/details/gxfrgjrmo.sHtML

[Q37] 右连接
来源：http://mobile.hesvh.cn/Article/details/gkwzmdllg.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.blog.hesvh.cn/Article/details/grhipxxmm.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.m.share.fehbvm.com/Article/details/geqhwseiq.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.m.share.hesvh.cn/Article/details/gqadpxquv.sHtML

[Q39] 自连接（查上下级）
来源：http://read.share.fehbvm.com/Article/details/gaaegfsou.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://wap.hesvh.cn/Article/details/grftoxhhd.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://m.share.zdbjq.cn/Article/details/gxacecykd.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.blog.zdbjq.cn/Article/details/gpvidsiqj.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://mobile.zdbjq.cn/Article/details/gxayjqxnj.sHtML

[Q41] 多表连接
来源：http://baike.zdbjq.cn/Article/details/gfmwruprx.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://read.share.fehbvm.com/Article/details/gkkkpqbht.sHtML

JOIN users u ON u.id = o.user_id
来源：http://m.share.fehbvm.com/Article/details/gjkjijwho.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.m.share.hesvh.cn/Article/details/gpfzfzfdl.sHtML

[Q42] 连接条件附加过滤
来源：http://m.share.hesvh.cn/Article/details/gqcgxehnj.sHtML

SELECT u.name, o.amount FROM users u
来源：http://blog.zdbjq.cn/Article/details/gguvzpvvs.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.share.hesvh.cn/Article/details/glbilrrlc.sHtML

[Q43] 标量子查询
来源：http://m.share.hesvh.cn/Article/details/gudynlcyk.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://baike.fehbvm.com/Article/details/gbbjzcdzb.sHtML

[Q44] IN 子查询
来源：http://www.m.share.zdbjq.cn/Article/details/gnqluvbeq.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.blog.hesvh.cn/Article/details/gabwxscgg.sHtML

[Q45] EXISTS 判断存在
来源：http://baike.fehbvm.com/Article/details/gkxlbtjqw.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.hesvh.cn/Article/details/gdwaaulpm.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.blog.hesvh.cn/Article/details/gjglwooug.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.zdbjq.cn/Article/details/gbhiioerd.sHtML

[Q47] 与平均值比较
来源：http://read.share.zdbjq.cn/Article/details/ggknuwayd.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://baike.hesvh.cn/Article/details/golpuolbw.sHtML

[Q48] CTE 公用表表达式
来源：http://www.m.share.hesvh.cn/Article/details/gnwoqoped.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://baike.zdbjq.cn/Article/details/ghbnnnvkx.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.blog.zdbjq.cn/Article/details/ghwtiocku.sHtML

[Q49] 更新单行
来源：http://www.blog.fehbvm.com/Article/details/gqstspjzh.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.m.share.hesvh.cn/Article/details/gfkzpdfau.sHtML

[Q50] 批量更新
来源：http://baike.hesvh.cn/Article/details/gbetsupbf.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://baike.fehbvm.com/Article/details/grnpeoroq.sHtML

[Q51] 用子查询更新
来源：http://read.share.hesvh.cn/Article/details/gwkxsmcit.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://3g.zdbjq.cn/Article/details/gpwgkwxck.sHtML

[Q52] 删除指定行
来源：http://read.share.fehbvm.com/Article/details/gxomqseat.sHtML

DELETE FROM users WHERE id = 10;
来源：http://wap.hesvh.cn/Article/details/gvaoygvee.sHtML

[Q53] 按条件删除
来源：http://wap.fehbvm.com/Article/details/gsfbvslqg.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://wap.hesvh.cn/Article/details/gxfkssbrz.sHtML

[Q54] 清空表
来源：http://mobile.hesvh.cn/Article/details/ggsaxgwah.sHtML

TRUNCATE TABLE logs;
来源：http://www.m.share.fehbvm.com/Article/details/gezeniovt.sHtML

[Q55] 排名（并列占位）
来源：http://blog.zdbjq.cn/Article/details/gaxqzeaph.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://baike.fehbvm.com/Article/details/grlwiplfn.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.share.zdbjq.cn/Article/details/gkvirudgo.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.blog.hesvh.cn/Article/details/guhxzamcj.sHtML

[Q57] 行号
来源：http://www.blog.hesvh.cn/Article/details/gykvuwcwt.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.share.hesvh.cn/Article/details/gdesxzrmf.sHtML

[Q58] 累计求和
来源：http://www.share.zdbjq.cn/Article/details/gpgugwrty.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://mobile.zdbjq.cn/Article/details/gznyjbqvd.sHtML

[Q59] 分组内累计
来源：http://m.share.hesvh.cn/Article/details/gmuzhncfl.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://wap.zdbjq.cn/Article/details/gsquhftvu.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.m.share.fehbvm.com/Article/details/gsgvisvcl.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://blog.zdbjq.cn/Article/details/gpyekogkx.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.share.zdbjq.cn/Article/details/gcuqjuunm.sHtML

[Q61] 移动平均
来源：http://read.share.hesvh.cn/Article/details/gcsridjnr.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://wap.fehbvm.com/Article/details/gzjcvgpeb.sHtML

[Q62] 分组占比
来源：http://baike.fehbvm.com/Article/details/gmneuilir.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://read.share.hesvh.cn/Article/details/ghyoegcad.sHtML

[Q63] 开启事务
来源：http://wap.hesvh.cn/Article/details/gabdyswdo.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://baike.fehbvm.com/Article/details/gtilcbwof.sHtML

[Q64] 提交事务
来源：http://www.share.hesvh.cn/Article/details/gutgpbhib.sHtML

COMMIT;
来源：http://www.blog.hesvh.cn/Article/details/gfzxrjxky.sHtML

[Q65] 回滚事务
来源：http://www.share.fehbvm.com/Article/details/gwqmcrlok.sHtML

ROLLBACK;
来源：http://blog.hesvh.cn/Article/details/gkncwkssy.sHtML

[Q66] 行锁查询
来源：http://m.share.hesvh.cn/Article/details/gxthzmeyk.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://m.share.hesvh.cn/Article/details/gbxzeddix.sHtML

[Q67] 设置隔离级别
来源：http://3g.zdbjq.cn/Article/details/gdkhjtvpf.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://mobile.zdbjq.cn/Article/details/gqalsjdkc.sHtML

[Q68] 保存点
来源：http://3g.zdbjq.cn/Article/details/grepznntg.sHtML

SAVEPOINT sp1;
来源：http://blog.hesvh.cn/Article/details/gtftkuyig.sHtML

ROLLBACK TO sp1;
来源：http://blog.fehbvm.com/Article/details/gzeyhpugg.sHtML

[Q69] 查看执行计划
来源：http://www.share.hesvh.cn/Article/details/gbnvzxdjf.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://read.share.fehbvm.com/Article/details/gldgbbafe.sHtML

[Q70] 更新统计信息
来源：http://read.share.hesvh.cn/Article/details/gjgwazyah.sHtML

ANALYZE TABLE users;
来源：http://m.share.fehbvm.com/Article/details/gwjatlxej.sHtML

[Q71] 查看建表语句
来源：http://www.m.share.hesvh.cn/Article/details/gwlrpnuxy.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.blog.zdbjq.cn/Article/details/gomufvbdp.sHtML

[Q72] 查看索引
来源：http://baike.zdbjq.cn/Article/details/gbauwbtoa.sHtML

SHOW INDEX FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gsnfpvhka.sHtML

[Q73] 查看表状态
来源：http://mobile.zdbjq.cn/Article/details/gxkuvglan.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://m.share.fehbvm.com/Article/details/grzglqvor.sHtML

[Q74] 强制使用索引
来源：http://www.blog.hesvh.cn/Article/details/griwhcope.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.share.hesvh.cn/Article/details/gigafkwcj.sHtML

[Q75] 日期格式化
来源：http://www.m.share.fehbvm.com/Article/details/gwqgmbbwe.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://blog.fehbvm.com/Article/details/gzjffgmki.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://read.share.hesvh.cn/Article/details/gvapflnrx.sHtML

[Q76] 按天统计
来源：http://m.share.fehbvm.com/Article/details/gntgoflmu.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://mobile.zdbjq.cn/Article/details/gsgtgvqzp.sHtML

[Q77] 时间加减
来源：http://baike.hesvh.cn/Article/details/gkbavbgdv.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.blog.zdbjq.cn/Article/details/girdzxucd.sHtML

[Q78] 当前时间
来源：http://read.share.fehbvm.com/Article/details/ggssmkrnb.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://wap.hesvh.cn/Article/details/gibewjqhg.sHtML

[Q79] 字符串拼接
来源：http://read.share.hesvh.cn/Article/details/gxokdpqko.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://mobile.zdbjq.cn/Article/details/gobbpwjza.sHtML

[Q80] 字符串截取
来源：http://mobile.zdbjq.cn/Article/details/gqosbzsgx.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://wap.zdbjq.cn/Article/details/gzdxwjwxl.sHtML

[Q81] 字符串替换
来源：http://blog.zdbjq.cn/Article/details/gxmsmwtyq.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gtnfdmnlj.sHtML

[Q82] 字符长度与字节长度
来源：http://read.share.fehbvm.com/Article/details/gjvvsudbm.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://blog.zdbjq.cn/Article/details/gojosxkxf.sHtML

[Q83] 大小写转换
来源：http://mobile.fehbvm.com/Article/details/gksjdnomy.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gsxeqeywn.sHtML

[Q84] 去除首尾空格
来源：http://blog.fehbvm.com/Article/details/gvygovwld.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gsckgfumz.sHtML

[Q85] 数值取整
来源：http://www.m.share.zdbjq.cn/Article/details/gtdlsbndv.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://m.share.fehbvm.com/Article/details/gbtvdlhcs.sHtML

[Q86] 读取 JSON 字段
来源：http://wap.hesvh.cn/Article/details/gvtzjipor.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://blog.hesvh.cn/Article/details/gpufrlvtv.sHtML

[Q87] JSON 字段做条件
来源：http://m.share.fehbvm.com/Article/details/gqifspofb.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://read.share.zdbjq.cn/Article/details/gvscrzpcf.sHtML

[Q88] 行转列（条件聚合）
来源：http://wap.hesvh.cn/Article/details/gfvkzkvql.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.m.share.zdbjq.cn/Article/details/gyjresxbl.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://wap.fehbvm.com/Article/details/gmlsjepqt.sHtML

[Q89] 判断表是否存在
来源：http://m.share.zdbjq.cn/Article/details/gjqlosvlz.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://baike.zdbjq.cn/Article/details/gslbuayjr.sHtML

[Q90] 生成序号列
来源：http://mobile.hesvh.cn/Article/details/ghwpawesh.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://baike.hesvh.cn/Article/details/goalkqtnm.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/ghgyqqmke.sHtML

R. Bash 专题
来源：http://mobile.hesvh.cn/Article/details/gczrnfdxy.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gduhgpxsh.sHtML

[R01] shebang 与严格模式
来源：http://mobile.zdbjq.cn/Article/details/gnywticgp.sHtML

#!/usr/bin/env bash
来源：http://www.m.share.fehbvm.com/Article/details/grgbejuhh.sHtML

set -euo pipefail
来源：http://www.share.hesvh.cn/Article/details/grssycszv.sHtML

[R02] 变量赋值与使用
来源：http://m.share.zdbjq.cn/Article/details/gpcbhoyjk.sHtML

name="Tom"; echo "$name"
来源：http://blog.zdbjq.cn/Article/details/gcdpxzkvc.sHtML

[R03] 只读变量
来源：http://www.blog.hesvh.cn/Article/details/gnvardlsn.sHtML

readonly PI=3.14
来源：http://blog.zdbjq.cn/Article/details/gzqurfoih.sHtML

[R04] 位置参数
来源：http://read.share.hesvh.cn/Article/details/gfodxwvve.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.share.zdbjq.cn/Article/details/glvkimwqn.sHtML

[R05] 参数默认值
来源：http://www.m.share.fehbvm.com/Article/details/gkukmitxp.sHtML

name="${1:-default}"
来源：http://www.share.fehbvm.com/Article/details/gpdbbgxxo.sHtML

[R06] 判断命令是否存在
来源：http://wap.zdbjq.cn/Article/details/ggefruhdc.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.blog.zdbjq.cn/Article/details/gahaievpv.sHtML

[R07] if 判断文件
来源：http://mobile.fehbvm.com/Article/details/gjngkbyan.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.m.share.hesvh.cn/Article/details/gwkycmdto.sHtML

[R08] 数值比较
来源：http://3g.fehbvm.com/Article/details/gjysbfuli.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://mobile.hesvh.cn/Article/details/gimccrkwo.sHtML

[R09] 字符串比较
来源：http://blog.hesvh.cn/Article/details/gapqcettz.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://wap.fehbvm.com/Article/details/gxxnlphbj.sHtML

[R10] 正则匹配
来源：http://www.blog.zdbjq.cn/Article/details/ghlfdgnzs.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://baike.fehbvm.com/Article/details/gnxnecemb.sHtML

[R11] case 多分支
来源：http://read.share.hesvh.cn/Article/details/gkknlykfv.sHtML

case "$1" in
来源：http://blog.fehbvm.com/Article/details/gjoqikfsc.sHtML

start) echo "启动" ;;
来源：http://blog.fehbvm.com/Article/details/ghdemogxp.sHtML

stop)  echo "停止" ;;
来源：http://blog.zdbjq.cn/Article/details/gbwutyick.sHtML

*)     echo "未知命令" ;;
来源：http://www.share.fehbvm.com/Article/details/gkbhcofpw.sHtML

esac
来源：http://baike.fehbvm.com/Article/details/gxguxrlve.sHtML

[R12] for 遍历文件
来源：http://mobile.fehbvm.com/Article/details/gvgqsvesv.sHtML

for f in *.txt; do echo "$f"; done
来源：http://wap.fehbvm.com/Article/details/gzpihstqh.sHtML

[R13] for 计数循环
来源：http://www.m.share.hesvh.cn/Article/details/ginfsbkes.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://wap.fehbvm.com/Article/details/giyjvheel.sHtML

[R14] C 风格 for
来源：http://mobile.zdbjq.cn/Article/details/guhqqnmly.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://read.share.zdbjq.cn/Article/details/gvckbkyjx.sHtML

[R15] while 逐行读文件
来源：http://mobile.zdbjq.cn/Article/details/gzlpfgerv.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://blog.fehbvm.com/Article/details/gqukejnmy.sHtML

[R16] until 等待条件
来源：http://mobile.hesvh.cn/Article/details/gqsmbivhh.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.m.share.fehbvm.com/Article/details/gibwwmlde.sHtML

[R17] 数组定义与取值
来源：http://www.share.fehbvm.com/Article/details/gpcfonlsb.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://mobile.zdbjq.cn/Article/details/gpoihvahj.sHtML

[R18] 遍历数组
来源：http://read.share.fehbvm.com/Article/details/gmrragcnu.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://read.share.zdbjq.cn/Article/details/gnbfrcvlr.sHtML

[R19] 数组长度
来源：http://mobile.zdbjq.cn/Article/details/gzwclnusb.sHtML

echo "${#arr[@]}"
来源：http://www.share.fehbvm.com/Article/details/gkpyojkju.sHtML

[R20] 关联数组（字典）
来源：http://www.m.share.hesvh.cn/Article/details/gwqekclor.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.blog.hesvh.cn/Article/details/galidmuae.sHtML

[R21] 字符串长度
来源：http://www.share.fehbvm.com/Article/details/ghtxtzokj.sHtML

echo "${#s}"
来源：http://www.share.fehbvm.com/Article/details/gienpehlf.sHtML

[R22] 截取子串
来源：http://www.m.share.hesvh.cn/Article/details/gqcpjqxwz.sHtML

echo "${s:0:5}"
来源：http://www.blog.fehbvm.com/Article/details/gwigecqql.sHtML

[R23] 字符串替换
来源：http://baike.fehbvm.com/Article/details/gmqrknzfs.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://mobile.hesvh.cn/Article/details/gcgwncqzz.sHtML

[R24] 大小写转换
来源：http://3g.fehbvm.com/Article/details/gkgjtddjy.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.share.zdbjq.cn/Article/details/gjhbbddrh.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.m.share.hesvh.cn/Article/details/gicbhjekz.sHtML


<!-- 参考信息 -->