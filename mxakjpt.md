代发 wailian999

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://3g.fehbvm.com/Article/details/gubebzbux.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://3g.zdbjq.cn/Article/details/gnfnjzksx.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.share.zdbjq.cn/Article/details/gxhnhvxpd.sHtML

[P04] 求长度
来源：http://3g.hesvh.cn/Article/details/gwemtzlpf.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://baike.hesvh.cn/Article/details/ggumuiajn.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.fehbvm.com/Article/details/ghqofjsvh.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.zdbjq.cn/Article/details/goulorcug.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.zdbjq.cn/Article/details/gmoghhuox.sHtML

Java: list.size();  map.size();  s.length()
来源：http://mobile.fehbvm.com/Article/details/gnlbkdqrg.sHtML

Go:   len(arr);  len(m)
来源：http://wap.zdbjq.cn/Article/details/gdzsgzdvd.sHtML

Ruby: x.length;  x.size
来源：http://read.share.hesvh.cn/Article/details/gqcubxdvw.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://blog.fehbvm.com/Article/details/gzxbwglgg.sHtML

[P05] 判断两个对象内容是否相等
来源：http://mobile.fehbvm.com/Article/details/gypgdgzoz.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://read.share.hesvh.cn/Article/details/gmkjmfoaz.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.share.fehbvm.com/Article/details/goxkdoswa.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://3g.zdbjq.cn/Article/details/gigezxvxs.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://baike.hesvh.cn/Article/details/gniabtqeg.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://mobile.zdbjq.cn/Article/details/gjtgskfoo.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.share.zdbjq.cn/Article/details/gydibhago.sHtML

Ruby: a == b
来源：http://baike.hesvh.cn/Article/details/gwjxwhzie.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.blog.hesvh.cn/Article/details/gmpflmptm.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.blog.hesvh.cn/Article/details/golafhdqu.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.m.share.fehbvm.com/Article/details/grtynxexh.sHtML

PHP:  if (empty($x)) {}
来源：http://3g.fehbvm.com/Article/details/gayaktijv.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://blog.hesvh.cn/Article/details/gnejydabh.sHtML

TS:   if (x == null) {}
来源：http://wap.hesvh.cn/Article/details/gshloyvly.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.m.share.hesvh.cn/Article/details/gyjchrgye.sHtML

Go:   if x == nil {}
来源：http://3g.hesvh.cn/Article/details/ggouutsob.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://baike.hesvh.cn/Article/details/gajxnwomz.sHtML

C#:   if (x is null) {}
来源：http://m.share.fehbvm.com/Article/details/gqmpbksbm.sHtML

[P07] 防抖与节流
来源：http://www.m.share.hesvh.cn/Article/details/ggbyuxxft.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.share.fehbvm.com/Article/details/gblcfcavj.sHtML

PHP:  // 手写时间戳比较
来源：http://www.blog.hesvh.cn/Article/details/gyuiznhoq.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.fehbvm.com/Article/details/gxzapbbmj.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.hesvh.cn/Article/details/gndbumdcb.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://blog.fehbvm.com/Article/details/glmbusfcq.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.blog.fehbvm.com/Article/details/ghvzssmyw.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://wap.hesvh.cn/Article/details/geiexgjqi.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://baike.zdbjq.cn/Article/details/gvmnunjqy.sHtML

[P08] 处理浮点精度问题
来源：http://mobile.fehbvm.com/Article/details/ghkrxmloa.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://mobile.hesvh.cn/Article/details/gzbibxujp.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://mobile.hesvh.cn/Article/details/gfdsmgymy.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.share.fehbvm.com/Article/details/ghbyhayor.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://blog.fehbvm.com/Article/details/gtgqpouts.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://read.share.hesvh.cn/Article/details/gqcccwrzm.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://blog.hesvh.cn/Article/details/gjqgnofoh.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://wap.hesvh.cn/Article/details/gocxxmwgs.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://mobile.fehbvm.com/Article/details/gcmxqsnwu.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/ggbascpwa.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://m.share.zdbjq.cn/Article/details/gqwwqxplj.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gwvolmwpt.sHtML

[Q01] 创建表
来源：http://mobile.hesvh.cn/Article/details/gikievcra.sHtML

CREATE TABLE users (
来源：http://m.share.zdbjq.cn/Article/details/ggtdysilq.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.zdbjq.cn/Article/details/gnohdpabk.sHtML

name VARCHAR(50) NOT NULL,
来源：http://blog.hesvh.cn/Article/details/gqghiojwe.sHtML

email VARCHAR(100) UNIQUE,
来源：http://m.share.hesvh.cn/Article/details/gzgaqjrdp.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://blog.zdbjq.cn/Article/details/ggfkjbjjj.sHtML

);
来源：http://3g.hesvh.cn/Article/details/gytcexdjz.sHtML

[Q02] 创建带外键的表
来源：http://www.share.fehbvm.com/Article/details/gtnfjmefn.sHtML

CREATE TABLE orders (
来源：http://baike.fehbvm.com/Article/details/gawcdkpti.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.hesvh.cn/Article/details/geeqbfynl.sHtML

user_id INT NOT NULL,
来源：http://www.m.share.fehbvm.com/Article/details/gkluzqupr.sHtML

amount DECIMAL(10, 2),
来源：http://m.share.zdbjq.cn/Article/details/godfwzwbv.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://blog.hesvh.cn/Article/details/gzuswwhms.sHtML

);
来源：http://m.share.zdbjq.cn/Article/details/ghavxachq.sHtML

[Q03] 增加列
来源：http://read.share.zdbjq.cn/Article/details/gmbftvnml.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.m.share.zdbjq.cn/Article/details/gshslfsug.sHtML

[Q04] 修改列类型
来源：http://www.share.zdbjq.cn/Article/details/gnkcjmhda.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.blog.zdbjq.cn/Article/details/gpqwhaaux.sHtML

[Q05] 重命名列
来源：http://read.share.fehbvm.com/Article/details/gbuqdguhf.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.m.share.fehbvm.com/Article/details/geeqonphn.sHtML

[Q06] 删除列
来源：http://m.share.zdbjq.cn/Article/details/grkshpkdl.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://3g.fehbvm.com/Article/details/gbiqiatjd.sHtML

[Q07] 删除表
来源：http://www.blog.hesvh.cn/Article/details/gpwmzlghn.sHtML

DROP TABLE IF EXISTS orders;
来源：http://3g.hesvh.cn/Article/details/gvsyguquj.sHtML

[Q08] 创建普通索引
来源：http://wap.zdbjq.cn/Article/details/ggafzwbsc.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.m.share.zdbjq.cn/Article/details/gvggntjqu.sHtML

[Q09] 创建唯一索引
来源：http://blog.hesvh.cn/Article/details/gfcdtboty.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://m.share.hesvh.cn/Article/details/gmghnfdsf.sHtML

[Q10] 插入单行
来源：http://m.share.hesvh.cn/Article/details/gsdgqhgdf.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.blog.hesvh.cn/Article/details/gkjtdafoa.sHtML

[Q11] 一次插入多行
来源：http://www.blog.fehbvm.com/Article/details/gurrsbgpu.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://m.share.hesvh.cn/Article/details/geddksxmk.sHtML

[Q12] 插入后取自增 ID
来源：http://baike.hesvh.cn/Article/details/gyguydcub.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.m.share.fehbvm.com/Article/details/ggoahcemi.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://blog.fehbvm.com/Article/details/gogtisvjr.sHtML

[Q13] 忽略重复插入
来源：http://wap.fehbvm.com/Article/details/gzqgxsapq.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://baike.fehbvm.com/Article/details/gkyjknbwh.sHtML

[Q14] 存在则更新（upsert）
来源：http://m.share.zdbjq.cn/Article/details/gyqtbsxif.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.m.share.zdbjq.cn/Article/details/gskyzwvrn.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://mobile.fehbvm.com/Article/details/gcpfbfjqw.sHtML

[Q15] 查询全部
来源：http://www.share.fehbvm.com/Article/details/gghredvgp.sHtML

SELECT * FROM users;
来源：http://mobile.fehbvm.com/Article/details/gsrismfmd.sHtML

[Q16] 查询指定列
来源：http://blog.fehbvm.com/Article/details/gyaqcmhpi.sHtML

SELECT id, name FROM users;
来源：http://blog.fehbvm.com/Article/details/gqnoiedhl.sHtML

[Q17] 条件查询
来源：http://www.share.fehbvm.com/Article/details/ggtodfwin.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://blog.fehbvm.com/Article/details/ghartgvcd.sHtML

[Q18] 模糊匹配
来源：http://baike.zdbjq.cn/Article/details/gxmwqfvtp.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.share.fehbvm.com/Article/details/gwrsqrxys.sHtML

[Q19] 范围查询
来源：http://www.share.hesvh.cn/Article/details/gtljntwbu.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://wap.hesvh.cn/Article/details/gteeikqns.sHtML

[Q20] IN 列表
来源：http://www.share.zdbjq.cn/Article/details/gxdzcluic.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://blog.hesvh.cn/Article/details/gzjfcpcyu.sHtML

[Q21] 空值判断
来源：http://baike.hesvh.cn/Article/details/gsvizijfd.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://m.share.hesvh.cn/Article/details/gnyadknxw.sHtML

[Q22] 排序
来源：http://www.share.hesvh.cn/Article/details/ggsixjmbl.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://blog.fehbvm.com/Article/details/gjmqikmbr.sHtML

[Q23] 分页
来源：http://m.share.fehbvm.com/Article/details/gmhwzqvuz.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://3g.fehbvm.com/Article/details/glycxpiuj.sHtML

[Q24] 去重
来源：http://mobile.fehbvm.com/Article/details/grtrdmwua.sHtML

SELECT DISTINCT city FROM users;
来源：http://m.share.zdbjq.cn/Article/details/ginmovsaq.sHtML

[Q25] 只取前 N 条
来源：http://wap.fehbvm.com/Article/details/gsersgymx.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://baike.fehbvm.com/Article/details/gzxpcigpb.sHtML

[Q26] 计数
来源：http://mobile.zdbjq.cn/Article/details/guatzbkfr.sHtML

SELECT COUNT(*) FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gvcwvjdjy.sHtML

[Q27] 条件计数
来源：http://wap.hesvh.cn/Article/details/gzkpzuoko.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gmujvtjof.sHtML

[Q28] 求和与平均
来源：http://www.m.share.zdbjq.cn/Article/details/gafdrmjfy.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://mobile.zdbjq.cn/Article/details/gqziwsbyy.sHtML

[Q29] 最大最小值
来源：http://3g.fehbvm.com/Article/details/gvmsxacgu.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://wap.fehbvm.com/Article/details/glcfdrkdf.sHtML

[Q30] 分组统计
来源：http://www.blog.hesvh.cn/Article/details/gunyitwij.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://wap.zdbjq.cn/Article/details/gsuyrxarg.sHtML

[Q31] 分组后过滤
来源：http://3g.zdbjq.cn/Article/details/gdpjnlbgr.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://baike.hesvh.cn/Article/details/gndyjxvyq.sHtML

[Q32] 分组拼接字符串
来源：http://mobile.zdbjq.cn/Article/details/gmajsvzih.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.m.share.hesvh.cn/Article/details/geycwbzkq.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.blog.fehbvm.com/Article/details/gmvwaukcm.sHtML

[Q33] 多列分组
来源：http://www.blog.fehbvm.com/Article/details/gcyuquayk.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.m.share.hesvh.cn/Article/details/glswvksnq.sHtML

[Q34] 每组取第一条
来源：http://3g.fehbvm.com/Article/details/gpubqlvvf.sHtML

SELECT * FROM (
来源：http://read.share.hesvh.cn/Article/details/gshpuzlhj.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://mobile.hesvh.cn/Article/details/glfjkmptg.sHtML

) t WHERE rn = 1;
来源：http://wap.zdbjq.cn/Article/details/gpldygokt.sHtML

[Q35] 内连接
来源：http://3g.zdbjq.cn/Article/details/gyawuzccg.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://mobile.fehbvm.com/Article/details/gwhcytmaz.sHtML

[Q36] 左连接
来源：http://www.share.hesvh.cn/Article/details/geegdeciz.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://blog.fehbvm.com/Article/details/gtiifbzsj.sHtML

[Q37] 右连接
来源：http://3g.zdbjq.cn/Article/details/geauazuup.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://wap.fehbvm.com/Article/details/ghtruiltp.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://wap.zdbjq.cn/Article/details/gzrexnhqz.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.blog.zdbjq.cn/Article/details/gafozpynt.sHtML

[Q39] 自连接（查上下级）
来源：http://wap.fehbvm.com/Article/details/ghxdggwcd.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://blog.fehbvm.com/Article/details/ghpolelyh.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://read.share.fehbvm.com/Article/details/gwmpgkqss.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://blog.hesvh.cn/Article/details/guhczpnon.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://blog.fehbvm.com/Article/details/gtnugzfqq.sHtML

[Q41] 多表连接
来源：http://mobile.hesvh.cn/Article/details/gervadilz.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.blog.hesvh.cn/Article/details/glyqcdbmh.sHtML

JOIN users u ON u.id = o.user_id
来源：http://3g.hesvh.cn/Article/details/gencjkvwr.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://m.share.zdbjq.cn/Article/details/gqbeuamvi.sHtML

[Q42] 连接条件附加过滤
来源：http://www.m.share.zdbjq.cn/Article/details/gbaqukdxi.sHtML

SELECT u.name, o.amount FROM users u
来源：http://baike.hesvh.cn/Article/details/guzwfynbd.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://blog.fehbvm.com/Article/details/gsogzksvl.sHtML

[Q43] 标量子查询
来源：http://blog.fehbvm.com/Article/details/gviqwqfco.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://wap.hesvh.cn/Article/details/gqtfwihcy.sHtML

[Q44] IN 子查询
来源：http://www.share.hesvh.cn/Article/details/ghiwbpinu.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.share.zdbjq.cn/Article/details/gtxvmtlkm.sHtML

[Q45] EXISTS 判断存在
来源：http://www.m.share.hesvh.cn/Article/details/gfczlbrjd.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.hesvh.cn/Article/details/gsjciqjli.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://mobile.fehbvm.com/Article/details/grgzdsdod.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.fehbvm.com/Article/details/gdbwywxmn.sHtML

[Q47] 与平均值比较
来源：http://wap.fehbvm.com/Article/details/gebmorswb.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.share.hesvh.cn/Article/details/gifbkoksy.sHtML

[Q48] CTE 公用表表达式
来源：http://read.share.zdbjq.cn/Article/details/gxhfcdion.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://m.share.zdbjq.cn/Article/details/gaafexxnd.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.m.share.fehbvm.com/Article/details/gxtcnizsd.sHtML

[Q49] 更新单行
来源：http://read.share.zdbjq.cn/Article/details/gwpbatmol.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://read.share.zdbjq.cn/Article/details/ginmoiplj.sHtML

[Q50] 批量更新
来源：http://m.share.zdbjq.cn/Article/details/geddwmshx.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.m.share.zdbjq.cn/Article/details/gzstcajwn.sHtML

[Q51] 用子查询更新
来源：http://mobile.fehbvm.com/Article/details/gvimvislx.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://blog.zdbjq.cn/Article/details/glocufxav.sHtML

[Q52] 删除指定行
来源：http://mobile.hesvh.cn/Article/details/gtuyclzcn.sHtML

DELETE FROM users WHERE id = 10;
来源：http://blog.fehbvm.com/Article/details/gbkcyvtzv.sHtML

[Q53] 按条件删除
来源：http://3g.hesvh.cn/Article/details/gxpdikzze.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://m.share.zdbjq.cn/Article/details/gcdhdchyh.sHtML

[Q54] 清空表
来源：http://read.share.fehbvm.com/Article/details/gegdekvza.sHtML

TRUNCATE TABLE logs;
来源：http://blog.zdbjq.cn/Article/details/gokmpylox.sHtML

[Q55] 排名（并列占位）
来源：http://blog.zdbjq.cn/Article/details/gcexvzzlc.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://3g.hesvh.cn/Article/details/glotxldcy.sHtML

[Q56] 密集排名（并列不占位）
来源：http://wap.zdbjq.cn/Article/details/gbtfjzmwd.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://3g.fehbvm.com/Article/details/gkewxwiuz.sHtML

[Q57] 行号
来源：http://3g.hesvh.cn/Article/details/gkjdmtxqg.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gkfvpbnuu.sHtML

[Q58] 累计求和
来源：http://wap.zdbjq.cn/Article/details/gpvogazog.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://read.share.fehbvm.com/Article/details/gcsrdaxad.sHtML

[Q59] 分组内累计
来源：http://3g.fehbvm.com/Article/details/gedvodxwv.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://wap.zdbjq.cn/Article/details/glvweyijx.sHtML

[Q60] 取上一行 / 下一行
来源：http://mobile.hesvh.cn/Article/details/griaglecm.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://m.share.hesvh.cn/Article/details/gezwpkddu.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://3g.fehbvm.com/Article/details/gpfgfsqpy.sHtML

[Q61] 移动平均
来源：http://wap.hesvh.cn/Article/details/gzuxkregj.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://read.share.hesvh.cn/Article/details/gmrmxrxmx.sHtML

[Q62] 分组占比
来源：http://read.share.hesvh.cn/Article/details/gaxxcdltk.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.share.hesvh.cn/Article/details/gxpsenlqx.sHtML

[Q63] 开启事务
来源：http://www.m.share.fehbvm.com/Article/details/grrbgsouv.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://wap.zdbjq.cn/Article/details/gtcqhbigl.sHtML

[Q64] 提交事务
来源：http://3g.zdbjq.cn/Article/details/guejdtwcr.sHtML

COMMIT;
来源：http://read.share.zdbjq.cn/Article/details/glttgokwe.sHtML

[Q65] 回滚事务
来源：http://m.share.fehbvm.com/Article/details/gweivxumf.sHtML

ROLLBACK;
来源：http://read.share.fehbvm.com/Article/details/gclktuhgq.sHtML

[Q66] 行锁查询
来源：http://3g.hesvh.cn/Article/details/gukzpmmfk.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://wap.zdbjq.cn/Article/details/gjarjnmwp.sHtML

[Q67] 设置隔离级别
来源：http://3g.zdbjq.cn/Article/details/gujntvaic.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.m.share.zdbjq.cn/Article/details/gubyruqlh.sHtML

[Q68] 保存点
来源：http://www.m.share.fehbvm.com/Article/details/gjdkmvwam.sHtML

SAVEPOINT sp1;
来源：http://mobile.zdbjq.cn/Article/details/gfeldtpzw.sHtML

ROLLBACK TO sp1;
来源：http://www.blog.hesvh.cn/Article/details/gkxqzaqlz.sHtML

[Q69] 查看执行计划
来源：http://wap.fehbvm.com/Article/details/gzteomahr.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://blog.fehbvm.com/Article/details/gagdvicuu.sHtML

[Q70] 更新统计信息
来源：http://www.m.share.fehbvm.com/Article/details/grayawhia.sHtML

ANALYZE TABLE users;
来源：http://m.share.fehbvm.com/Article/details/gyjhdfnhr.sHtML

[Q71] 查看建表语句
来源：http://3g.zdbjq.cn/Article/details/gzgewphun.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.share.hesvh.cn/Article/details/guvnkqxfv.sHtML

[Q72] 查看索引
来源：http://m.share.hesvh.cn/Article/details/gbbaqtxjj.sHtML

SHOW INDEX FROM users;
来源：http://www.share.fehbvm.com/Article/details/gszjrbxjn.sHtML

[Q73] 查看表状态
来源：http://www.blog.fehbvm.com/Article/details/gldzifugg.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.m.share.fehbvm.com/Article/details/gtcrjdfsv.sHtML

[Q74] 强制使用索引
来源：http://www.share.fehbvm.com/Article/details/gzyrwipfa.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://3g.zdbjq.cn/Article/details/gbileqvbb.sHtML

[Q75] 日期格式化
来源：http://www.share.zdbjq.cn/Article/details/gszsminzg.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.blog.hesvh.cn/Article/details/gyunhuehg.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://baike.hesvh.cn/Article/details/gqdgwffxe.sHtML

[Q76] 按天统计
来源：http://blog.zdbjq.cn/Article/details/ggufvjugv.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.share.fehbvm.com/Article/details/gcfgowjdg.sHtML

[Q77] 时间加减
来源：http://www.blog.fehbvm.com/Article/details/ghmmmukxq.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://read.share.zdbjq.cn/Article/details/gokntwawc.sHtML

[Q78] 当前时间
来源：http://blog.fehbvm.com/Article/details/gfgdtbgqo.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://blog.zdbjq.cn/Article/details/gzsffqolf.sHtML

[Q79] 字符串拼接
来源：http://mobile.hesvh.cn/Article/details/gxihyabqb.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.m.share.hesvh.cn/Article/details/gkuapojie.sHtML

[Q80] 字符串截取
来源：http://www.blog.zdbjq.cn/Article/details/gmnbyalic.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gzoofewgx.sHtML

[Q81] 字符串替换
来源：http://m.share.fehbvm.com/Article/details/gnoyanyge.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.share.hesvh.cn/Article/details/gfspuvaau.sHtML

[Q82] 字符长度与字节长度
来源：http://www.blog.hesvh.cn/Article/details/gytjizlwi.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://wap.zdbjq.cn/Article/details/gpojvarem.sHtML

[Q83] 大小写转换
来源：http://read.share.zdbjq.cn/Article/details/gpgznhcjm.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://blog.hesvh.cn/Article/details/gddbvnbtq.sHtML

[Q84] 去除首尾空格
来源：http://read.share.hesvh.cn/Article/details/gebhzxwmi.sHtML

SELECT TRIM(name) FROM users;
来源：http://m.share.hesvh.cn/Article/details/ghnovqeru.sHtML

[Q85] 数值取整
来源：http://3g.hesvh.cn/Article/details/gblfkyiul.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.m.share.fehbvm.com/Article/details/grxptejue.sHtML

[Q86] 读取 JSON 字段
来源：http://3g.hesvh.cn/Article/details/gnjhldyqo.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://m.share.zdbjq.cn/Article/details/gvfjetevf.sHtML

[Q87] JSON 字段做条件
来源：http://mobile.hesvh.cn/Article/details/gtjvleblm.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://mobile.fehbvm.com/Article/details/gkpupvnid.sHtML

[Q88] 行转列（条件聚合）
来源：http://blog.hesvh.cn/Article/details/giupqjdid.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.blog.zdbjq.cn/Article/details/gfbvcmuew.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://mobile.fehbvm.com/Article/details/ghznqxgpd.sHtML

[Q89] 判断表是否存在
来源：http://3g.hesvh.cn/Article/details/ggcyfylpr.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.blog.hesvh.cn/Article/details/gzbcpvnbb.sHtML

[Q90] 生成序号列
来源：http://www.m.share.hesvh.cn/Article/details/gxkfcevue.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.blog.hesvh.cn/Article/details/gnmdillca.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gnvidarmd.sHtML

R. Bash 专题
来源：http://wap.fehbvm.com/Article/details/goskknqgf.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gnkpwbxcc.sHtML

[R01] shebang 与严格模式
来源：http://mobile.fehbvm.com/Article/details/gjptokmso.sHtML

#!/usr/bin/env bash
来源：http://baike.hesvh.cn/Article/details/gzevpvoiv.sHtML

set -euo pipefail
来源：http://wap.fehbvm.com/Article/details/gxahurcgq.sHtML

[R02] 变量赋值与使用
来源：http://www.m.share.fehbvm.com/Article/details/gsdwwonqe.sHtML

name="Tom"; echo "$name"
来源：http://www.m.share.fehbvm.com/Article/details/gxhsslgtm.sHtML

[R03] 只读变量
来源：http://mobile.zdbjq.cn/Article/details/gatyecfmr.sHtML

readonly PI=3.14
来源：http://www.blog.zdbjq.cn/Article/details/gzsvyfygp.sHtML

[R04] 位置参数
来源：http://wap.hesvh.cn/Article/details/gvwlezedm.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.m.share.hesvh.cn/Article/details/gnqjxknfe.sHtML

[R05] 参数默认值
来源：http://mobile.fehbvm.com/Article/details/gwsrgxuly.sHtML

name="${1:-default}"
来源：http://read.share.fehbvm.com/Article/details/ggfnuhfoh.sHtML

[R06] 判断命令是否存在
来源：http://www.m.share.zdbjq.cn/Article/details/glhrxhyrh.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.blog.hesvh.cn/Article/details/gtlyjisti.sHtML

[R07] if 判断文件
来源：http://m.share.fehbvm.com/Article/details/gzurowdpm.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://mobile.zdbjq.cn/Article/details/gwjiqaqup.sHtML

[R08] 数值比较
来源：http://blog.fehbvm.com/Article/details/gohbsdprt.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.m.share.zdbjq.cn/Article/details/gwmdjkane.sHtML

[R09] 字符串比较
来源：http://baike.hesvh.cn/Article/details/glcatlwzu.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://read.share.zdbjq.cn/Article/details/gnkgffzhg.sHtML

[R10] 正则匹配
来源：http://blog.zdbjq.cn/Article/details/gdpphpxir.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://m.share.zdbjq.cn/Article/details/gujbpoafo.sHtML

[R11] case 多分支
来源：http://m.share.fehbvm.com/Article/details/gbahxlmri.sHtML

case "$1" in
来源：http://baike.hesvh.cn/Article/details/gumwneahf.sHtML

start) echo "启动" ;;
来源：http://www.share.hesvh.cn/Article/details/gkjlwrjwr.sHtML

stop)  echo "停止" ;;
来源：http://www.m.share.hesvh.cn/Article/details/glzkyurqn.sHtML

*)     echo "未知命令" ;;
来源：http://blog.fehbvm.com/Article/details/ggxygfzly.sHtML

esac
来源：http://mobile.zdbjq.cn/Article/details/gqlvqacli.sHtML

[R12] for 遍历文件
来源：http://m.share.hesvh.cn/Article/details/gmuhmvxni.sHtML

for f in *.txt; do echo "$f"; done
来源：http://mobile.hesvh.cn/Article/details/gkgpphpgz.sHtML

[R13] for 计数循环
来源：http://read.share.zdbjq.cn/Article/details/geueqypui.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.m.share.hesvh.cn/Article/details/gyylnzmnw.sHtML

[R14] C 风格 for
来源：http://www.m.share.fehbvm.com/Article/details/ggcvuipzf.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://baike.zdbjq.cn/Article/details/ggtsbtkja.sHtML

[R15] while 逐行读文件
来源：http://www.blog.fehbvm.com/Article/details/gzjzgxpii.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://baike.zdbjq.cn/Article/details/gjnzijrnd.sHtML

[R16] until 等待条件
来源：http://baike.fehbvm.com/Article/details/gbmxotcyw.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.blog.fehbvm.com/Article/details/gyrdrrgdw.sHtML

[R17] 数组定义与取值
来源：http://3g.hesvh.cn/Article/details/goczcfzsk.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.m.share.hesvh.cn/Article/details/gxgmihtah.sHtML

[R18] 遍历数组
来源：http://blog.fehbvm.com/Article/details/gucpayqqq.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://3g.fehbvm.com/Article/details/glkbiuiou.sHtML

[R19] 数组长度
来源：http://www.share.fehbvm.com/Article/details/goplxmica.sHtML


<!-- 参考信息 -->