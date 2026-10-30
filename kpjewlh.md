代发 wailian999

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.blog.zdbjq.cn/Article/details/gigdoikyy.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://wap.zdbjq.cn/Article/details/guqrgrkti.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://m.share.zdbjq.cn/Article/details/gybrtbqav.sHtML

[P04] 求长度
来源：http://wap.fehbvm.com/Article/details/gypnswueb.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://blog.hesvh.cn/Article/details/goxaipqld.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.zdbjq.cn/Article/details/gkggzueth.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.hesvh.cn/Article/details/gydjbfxfx.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.fehbvm.com/Article/details/giknyuojv.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.blog.fehbvm.com/Article/details/gogzzjpaz.sHtML

Go:   len(arr);  len(m)
来源：http://wap.fehbvm.com/Article/details/gfoljuelo.sHtML

Ruby: x.length;  x.size
来源：http://3g.hesvh.cn/Article/details/gcnnegwjj.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.share.hesvh.cn/Article/details/gxtkoslvi.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.share.hesvh.cn/Article/details/gpjsrfoyh.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://3g.zdbjq.cn/Article/details/gpsjgpfjc.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://wap.hesvh.cn/Article/details/gwxburgsy.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://m.share.hesvh.cn/Article/details/gmkvxpihr.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://baike.fehbvm.com/Article/details/gwewxenfm.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://baike.zdbjq.cn/Article/details/gmtadbwkb.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://blog.fehbvm.com/Article/details/gmilrxdlz.sHtML

Ruby: a == b
来源：http://www.blog.fehbvm.com/Article/details/guicjnavr.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://read.share.hesvh.cn/Article/details/gizbmjupw.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.m.share.zdbjq.cn/Article/details/gfzukpfkc.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://3g.fehbvm.com/Article/details/grmlhiggt.sHtML

PHP:  if (empty($x)) {}
来源：http://read.share.zdbjq.cn/Article/details/gyemrclhk.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://blog.hesvh.cn/Article/details/grkxpgnha.sHtML

TS:   if (x == null) {}
来源：http://blog.zdbjq.cn/Article/details/grceoxwbe.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://m.share.hesvh.cn/Article/details/ghuefumsr.sHtML

Go:   if x == nil {}
来源：http://3g.zdbjq.cn/Article/details/gnqwknftv.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://wap.fehbvm.com/Article/details/ghreuaxls.sHtML

C#:   if (x is null) {}
来源：http://mobile.fehbvm.com/Article/details/gglaqfgjr.sHtML

[P07] 防抖与节流
来源：http://www.m.share.fehbvm.com/Article/details/gvdqhoily.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://wap.zdbjq.cn/Article/details/gbtjmlvbg.sHtML

PHP:  // 手写时间戳比较
来源：http://baike.zdbjq.cn/Article/details/gkmrvwdub.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.hesvh.cn/Article/details/goquiybns.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.hesvh.cn/Article/details/gadrzcafz.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.share.hesvh.cn/Article/details/gqeoofpza.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://wap.hesvh.cn/Article/details/gkynbujco.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://baike.hesvh.cn/Article/details/gohzntonx.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.share.fehbvm.com/Article/details/gcukxvhrj.sHtML

[P08] 处理浮点精度问题
来源：http://baike.zdbjq.cn/Article/details/gendumvfi.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://baike.hesvh.cn/Article/details/goqtgaeiq.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://mobile.fehbvm.com/Article/details/gmosmmxll.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://wap.fehbvm.com/Article/details/gpmjiiyqy.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://wap.zdbjq.cn/Article/details/ggpdmaaut.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://wap.zdbjq.cn/Article/details/gomqqhluq.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://read.share.hesvh.cn/Article/details/gulbmpbst.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://m.share.fehbvm.com/Article/details/gpvsreren.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://3g.fehbvm.com/Article/details/gosllslpf.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gqwlliwaa.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://baike.zdbjq.cn/Article/details/gaslvchfz.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gznrfpjkh.sHtML

[Q01] 创建表
来源：http://baike.hesvh.cn/Article/details/gpvyzgzga.sHtML

CREATE TABLE users (
来源：http://www.share.zdbjq.cn/Article/details/gmcdxmpvs.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://mobile.fehbvm.com/Article/details/gmxcjlwoy.sHtML

name VARCHAR(50) NOT NULL,
来源：http://3g.zdbjq.cn/Article/details/gpavhpwef.sHtML

email VARCHAR(100) UNIQUE,
来源：http://3g.fehbvm.com/Article/details/gjtwfpyzz.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://3g.fehbvm.com/Article/details/ghxbvhimz.sHtML

);
来源：http://mobile.hesvh.cn/Article/details/gwavedkuf.sHtML

[Q02] 创建带外键的表
来源：http://www.blog.fehbvm.com/Article/details/gpfhjxnqk.sHtML

CREATE TABLE orders (
来源：http://www.m.share.zdbjq.cn/Article/details/gmbhydfph.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.hesvh.cn/Article/details/gckqqjttj.sHtML

user_id INT NOT NULL,
来源：http://mobile.zdbjq.cn/Article/details/garylymet.sHtML

amount DECIMAL(10, 2),
来源：http://www.m.share.fehbvm.com/Article/details/gidtmitik.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.blog.fehbvm.com/Article/details/gkbhwqgyx.sHtML

);
来源：http://www.share.zdbjq.cn/Article/details/gxefelmzr.sHtML

[Q03] 增加列
来源：http://www.m.share.zdbjq.cn/Article/details/ggbqzmdei.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://mobile.fehbvm.com/Article/details/gecahlzkv.sHtML

[Q04] 修改列类型
来源：http://baike.fehbvm.com/Article/details/gpoxmrdkx.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://m.share.fehbvm.com/Article/details/gkbqsltoz.sHtML

[Q05] 重命名列
来源：http://baike.zdbjq.cn/Article/details/gwmtwuauk.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://blog.hesvh.cn/Article/details/gyacrspbe.sHtML

[Q06] 删除列
来源：http://read.share.fehbvm.com/Article/details/gtdbfhqpb.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.m.share.fehbvm.com/Article/details/grkcoikpt.sHtML

[Q07] 删除表
来源：http://blog.zdbjq.cn/Article/details/gxvlbpgxb.sHtML

DROP TABLE IF EXISTS orders;
来源：http://mobile.fehbvm.com/Article/details/gwifspmop.sHtML

[Q08] 创建普通索引
来源：http://www.m.share.zdbjq.cn/Article/details/gjmmbeief.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://3g.hesvh.cn/Article/details/gjmoquxuq.sHtML

[Q09] 创建唯一索引
来源：http://m.share.hesvh.cn/Article/details/gwimrhawo.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://blog.fehbvm.com/Article/details/gbbxcisdy.sHtML

[Q10] 插入单行
来源：http://wap.hesvh.cn/Article/details/gmzdrreeo.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://3g.zdbjq.cn/Article/details/ghqrvsmxq.sHtML

[Q11] 一次插入多行
来源：http://m.share.fehbvm.com/Article/details/gvuvvispe.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://baike.hesvh.cn/Article/details/gblxbflxg.sHtML

[Q12] 插入后取自增 ID
来源：http://www.share.hesvh.cn/Article/details/grxjdrsim.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.share.zdbjq.cn/Article/details/gnouybgga.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://blog.hesvh.cn/Article/details/gwdvbcvau.sHtML

[Q13] 忽略重复插入
来源：http://read.share.hesvh.cn/Article/details/grwcanqti.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.m.share.zdbjq.cn/Article/details/gmfsbimkw.sHtML

[Q14] 存在则更新（upsert）
来源：http://read.share.hesvh.cn/Article/details/grqzbyjql.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://mobile.zdbjq.cn/Article/details/gvujjijzz.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.m.share.hesvh.cn/Article/details/gozhpwlex.sHtML

[Q15] 查询全部
来源：http://m.share.fehbvm.com/Article/details/gnqjrfitv.sHtML

SELECT * FROM users;
来源：http://3g.hesvh.cn/Article/details/gzztwymua.sHtML

[Q16] 查询指定列
来源：http://blog.zdbjq.cn/Article/details/ghpagkqdy.sHtML

SELECT id, name FROM users;
来源：http://blog.hesvh.cn/Article/details/gvlfzfklt.sHtML

[Q17] 条件查询
来源：http://blog.fehbvm.com/Article/details/ghwzptvfv.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://read.share.zdbjq.cn/Article/details/gyosasgky.sHtML

[Q18] 模糊匹配
来源：http://baike.hesvh.cn/Article/details/gxioghgdb.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://mobile.hesvh.cn/Article/details/gbwdbwvrg.sHtML

[Q19] 范围查询
来源：http://mobile.fehbvm.com/Article/details/gwgozgyrh.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://wap.fehbvm.com/Article/details/ggcbltpkk.sHtML

[Q20] IN 列表
来源：http://www.m.share.hesvh.cn/Article/details/gzpjhnbjf.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://wap.fehbvm.com/Article/details/gfrvvhtiz.sHtML

[Q21] 空值判断
来源：http://3g.zdbjq.cn/Article/details/gblllktym.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://m.share.fehbvm.com/Article/details/gzbexpljg.sHtML

[Q22] 排序
来源：http://baike.zdbjq.cn/Article/details/gjtpujtqg.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.blog.zdbjq.cn/Article/details/gqjeailwe.sHtML

[Q23] 分页
来源：http://mobile.fehbvm.com/Article/details/gyzrysxpc.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.share.hesvh.cn/Article/details/gqdlxafyi.sHtML

[Q24] 去重
来源：http://www.m.share.hesvh.cn/Article/details/gsuwedori.sHtML

SELECT DISTINCT city FROM users;
来源：http://read.share.fehbvm.com/Article/details/gjwrksiuq.sHtML

[Q25] 只取前 N 条
来源：http://www.blog.hesvh.cn/Article/details/gctqpuynu.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.m.share.zdbjq.cn/Article/details/gluupfhab.sHtML

[Q26] 计数
来源：http://www.blog.hesvh.cn/Article/details/gruqiuqqj.sHtML

SELECT COUNT(*) FROM users;
来源：http://m.share.fehbvm.com/Article/details/gqobqatar.sHtML

[Q27] 条件计数
来源：http://mobile.hesvh.cn/Article/details/gkqezpenj.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://baike.fehbvm.com/Article/details/gclxdmkxm.sHtML

[Q28] 求和与平均
来源：http://www.m.share.zdbjq.cn/Article/details/ghjdxjkxa.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://mobile.zdbjq.cn/Article/details/gjziwrign.sHtML

[Q29] 最大最小值
来源：http://www.share.zdbjq.cn/Article/details/gmavizaln.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.blog.hesvh.cn/Article/details/glceyvppz.sHtML

[Q30] 分组统计
来源：http://wap.fehbvm.com/Article/details/gbemvwfrf.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.blog.fehbvm.com/Article/details/gvucwdigh.sHtML

[Q31] 分组后过滤
来源：http://blog.hesvh.cn/Article/details/gwiqrbxzd.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.blog.hesvh.cn/Article/details/ggvdaiorn.sHtML

[Q32] 分组拼接字符串
来源：http://read.share.hesvh.cn/Article/details/gizdgbgde.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.share.hesvh.cn/Article/details/gkhpfwwvg.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://blog.fehbvm.com/Article/details/gacnnncyz.sHtML

[Q33] 多列分组
来源：http://wap.zdbjq.cn/Article/details/gashzefah.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://mobile.zdbjq.cn/Article/details/gujyqwzgy.sHtML

[Q34] 每组取第一条
来源：http://www.share.hesvh.cn/Article/details/gdtliypvv.sHtML

SELECT * FROM (
来源：http://wap.hesvh.cn/Article/details/gmubvjvaf.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.blog.fehbvm.com/Article/details/ggexfrypu.sHtML

) t WHERE rn = 1;
来源：http://read.share.zdbjq.cn/Article/details/grvwetfxp.sHtML

[Q35] 内连接
来源：http://www.m.share.zdbjq.cn/Article/details/gocvqivct.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://baike.fehbvm.com/Article/details/gtxiktzuh.sHtML

[Q36] 左连接
来源：http://read.share.zdbjq.cn/Article/details/gvpoohmmr.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.zdbjq.cn/Article/details/gehyzqspl.sHtML

[Q37] 右连接
来源：http://read.share.zdbjq.cn/Article/details/glxkabwws.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://3g.fehbvm.com/Article/details/gyxqausbq.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://3g.fehbvm.com/Article/details/gsyiucimf.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://3g.fehbvm.com/Article/details/giqrkmtmy.sHtML

[Q39] 自连接（查上下级）
来源：http://mobile.zdbjq.cn/Article/details/giirfoafy.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://mobile.hesvh.cn/Article/details/gsoxscclq.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://baike.fehbvm.com/Article/details/gagxpuzem.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.share.hesvh.cn/Article/details/gvtombkou.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.share.zdbjq.cn/Article/details/gcuucvady.sHtML

[Q41] 多表连接
来源：http://www.share.zdbjq.cn/Article/details/gakblnltg.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://baike.fehbvm.com/Article/details/gdshmvvjl.sHtML

JOIN users u ON u.id = o.user_id
来源：http://wap.hesvh.cn/Article/details/gwjqgiwjb.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://3g.fehbvm.com/Article/details/gqjiobggc.sHtML

[Q42] 连接条件附加过滤
来源：http://m.share.zdbjq.cn/Article/details/gphxqbrcr.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.m.share.hesvh.cn/Article/details/gnxeqbziv.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.share.fehbvm.com/Article/details/gwpnbeihs.sHtML

[Q43] 标量子查询
来源：http://mobile.fehbvm.com/Article/details/gyaookeet.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://baike.zdbjq.cn/Article/details/gcevhttfn.sHtML

[Q44] IN 子查询
来源：http://www.share.zdbjq.cn/Article/details/gjizghhjs.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://wap.hesvh.cn/Article/details/gpafozllm.sHtML

[Q45] EXISTS 判断存在
来源：http://wap.fehbvm.com/Article/details/gxmvsjesj.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.zdbjq.cn/Article/details/gmuccshvl.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://read.share.fehbvm.com/Article/details/gzmrejqfx.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.fehbvm.com/Article/details/gjaixodlo.sHtML

[Q47] 与平均值比较
来源：http://www.share.zdbjq.cn/Article/details/gdqjvwucf.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://mobile.hesvh.cn/Article/details/gbcelpxyx.sHtML

[Q48] CTE 公用表表达式
来源：http://m.share.hesvh.cn/Article/details/gsgaotyri.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.blog.zdbjq.cn/Article/details/gxmypdmil.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.share.fehbvm.com/Article/details/gmnzqloez.sHtML

[Q49] 更新单行
来源：http://www.m.share.hesvh.cn/Article/details/gylnpzuep.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.blog.hesvh.cn/Article/details/gkfefbacr.sHtML

[Q50] 批量更新
来源：http://mobile.fehbvm.com/Article/details/ghmabhfec.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://m.share.fehbvm.com/Article/details/gowzufukd.sHtML

[Q51] 用子查询更新
来源：http://www.share.hesvh.cn/Article/details/gjkprmjcg.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.share.zdbjq.cn/Article/details/gtqdwsjsd.sHtML

[Q52] 删除指定行
来源：http://mobile.zdbjq.cn/Article/details/gkmzupcmm.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.m.share.zdbjq.cn/Article/details/glronyrho.sHtML

[Q53] 按条件删除
来源：http://wap.zdbjq.cn/Article/details/gxpyakykg.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://read.share.fehbvm.com/Article/details/gmrswuxax.sHtML

[Q54] 清空表
来源：http://baike.zdbjq.cn/Article/details/gyzxprguw.sHtML

TRUNCATE TABLE logs;
来源：http://mobile.fehbvm.com/Article/details/gkrexalnt.sHtML

[Q55] 排名（并列占位）
来源：http://m.share.hesvh.cn/Article/details/gdbpexaus.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://3g.hesvh.cn/Article/details/gwyxurofu.sHtML

[Q56] 密集排名（并列不占位）
来源：http://baike.zdbjq.cn/Article/details/gumcllhdt.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://mobile.hesvh.cn/Article/details/grezymflg.sHtML

[Q57] 行号
来源：http://wap.zdbjq.cn/Article/details/gmvhoivst.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://wap.hesvh.cn/Article/details/gsxpemmqi.sHtML

[Q58] 累计求和
来源：http://m.share.hesvh.cn/Article/details/gluzuozdy.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.share.fehbvm.com/Article/details/gvccdlpjb.sHtML

[Q59] 分组内累计
来源：http://www.m.share.zdbjq.cn/Article/details/gmlfdantg.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://read.share.hesvh.cn/Article/details/gnbgyysps.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.blog.hesvh.cn/Article/details/ggyrwizos.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://3g.zdbjq.cn/Article/details/gdqufevxc.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://blog.zdbjq.cn/Article/details/gwujzlsdm.sHtML

[Q61] 移动平均
来源：http://baike.fehbvm.com/Article/details/gpglqpmvg.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://baike.fehbvm.com/Article/details/gngingbgn.sHtML

[Q62] 分组占比
来源：http://www.share.zdbjq.cn/Article/details/goooifbvr.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://mobile.fehbvm.com/Article/details/gkpluelvu.sHtML

[Q63] 开启事务
来源：http://m.share.zdbjq.cn/Article/details/gygatdwxf.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://m.share.fehbvm.com/Article/details/grvnwtmup.sHtML

[Q64] 提交事务
来源：http://baike.hesvh.cn/Article/details/gfxzyapah.sHtML

COMMIT;
来源：http://www.m.share.zdbjq.cn/Article/details/grqocueyu.sHtML

[Q65] 回滚事务
来源：http://mobile.hesvh.cn/Article/details/gmcdedvbd.sHtML

ROLLBACK;
来源：http://baike.fehbvm.com/Article/details/gestnrsti.sHtML

[Q66] 行锁查询
来源：http://blog.zdbjq.cn/Article/details/gtvtnhvtd.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://mobile.hesvh.cn/Article/details/gcrjogwzm.sHtML

[Q67] 设置隔离级别
来源：http://blog.fehbvm.com/Article/details/gmgbglsrf.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://baike.hesvh.cn/Article/details/gpovypewk.sHtML

[Q68] 保存点
来源：http://www.m.share.hesvh.cn/Article/details/gaijyzlin.sHtML

SAVEPOINT sp1;
来源：http://m.share.zdbjq.cn/Article/details/gssbtdnfy.sHtML

ROLLBACK TO sp1;
来源：http://read.share.fehbvm.com/Article/details/gwrisvxyf.sHtML

[Q69] 查看执行计划
来源：http://www.share.hesvh.cn/Article/details/gdqumlhls.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://read.share.hesvh.cn/Article/details/gwzwakzli.sHtML

[Q70] 更新统计信息
来源：http://www.blog.hesvh.cn/Article/details/ggbhgcweb.sHtML

ANALYZE TABLE users;
来源：http://3g.zdbjq.cn/Article/details/gsqbjjzsa.sHtML

[Q71] 查看建表语句
来源：http://wap.hesvh.cn/Article/details/gqylnkqyt.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.m.share.fehbvm.com/Article/details/gyazupztp.sHtML

[Q72] 查看索引
来源：http://blog.zdbjq.cn/Article/details/gcpqzllnr.sHtML

SHOW INDEX FROM users;
来源：http://3g.hesvh.cn/Article/details/gkhgiqcmy.sHtML

[Q73] 查看表状态
来源：http://blog.hesvh.cn/Article/details/giqggiazb.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.m.share.zdbjq.cn/Article/details/gybwgknmm.sHtML

[Q74] 强制使用索引
来源：http://blog.zdbjq.cn/Article/details/gqxrkpbgc.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://3g.zdbjq.cn/Article/details/gthzjhpqk.sHtML

[Q75] 日期格式化
来源：http://wap.hesvh.cn/Article/details/gbuyyjzkm.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://mobile.fehbvm.com/Article/details/gzwcmmshs.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://read.share.fehbvm.com/Article/details/grgtxvman.sHtML

[Q76] 按天统计
来源：http://mobile.fehbvm.com/Article/details/gyeetubxb.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://read.share.hesvh.cn/Article/details/gaszviepf.sHtML

[Q77] 时间加减
来源：http://wap.fehbvm.com/Article/details/grmkknzee.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://wap.zdbjq.cn/Article/details/gwlrlgcuy.sHtML

[Q78] 当前时间
来源：http://blog.zdbjq.cn/Article/details/gymptfgmn.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://mobile.zdbjq.cn/Article/details/gninemtsd.sHtML

[Q79] 字符串拼接
来源：http://www.blog.zdbjq.cn/Article/details/gaziqipba.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://3g.fehbvm.com/Article/details/goohwbkyt.sHtML

[Q80] 字符串截取
来源：http://www.blog.fehbvm.com/Article/details/gvmzlrjyr.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gavjaegmn.sHtML

[Q81] 字符串替换
来源：http://m.share.fehbvm.com/Article/details/ghhvpyqmr.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gllfpezvd.sHtML

[Q82] 字符长度与字节长度
来源：http://blog.fehbvm.com/Article/details/gishvmvub.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://read.share.hesvh.cn/Article/details/gkfcygvac.sHtML

[Q83] 大小写转换
来源：http://mobile.hesvh.cn/Article/details/gxqoxbfzc.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.share.fehbvm.com/Article/details/glclrijpg.sHtML

[Q84] 去除首尾空格
来源：http://wap.hesvh.cn/Article/details/gbyfvwdza.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gbxievevt.sHtML

[Q85] 数值取整
来源：http://wap.hesvh.cn/Article/details/gmjzcsmam.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.blog.hesvh.cn/Article/details/gwkfintry.sHtML

[Q86] 读取 JSON 字段
来源：http://read.share.hesvh.cn/Article/details/gqrhyzjup.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://3g.zdbjq.cn/Article/details/glylrokbr.sHtML

[Q87] JSON 字段做条件
来源：http://www.share.fehbvm.com/Article/details/grachcowx.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.share.hesvh.cn/Article/details/gsnnuztzx.sHtML

[Q88] 行转列（条件聚合）
来源：http://wap.zdbjq.cn/Article/details/gdudfsmyy.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.share.hesvh.cn/Article/details/gwhttxujx.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://read.share.fehbvm.com/Article/details/gcmbfkpsu.sHtML

[Q89] 判断表是否存在
来源：http://wap.hesvh.cn/Article/details/gdxmrhhck.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://wap.zdbjq.cn/Article/details/gyisnameo.sHtML

[Q90] 生成序号列
来源：http://wap.hesvh.cn/Article/details/ggtnnncnn.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://read.share.zdbjq.cn/Article/details/gpiwkpamk.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gjngvhzto.sHtML

R. Bash 专题
来源：http://wap.zdbjq.cn/Article/details/ghmcfzkxh.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gyagwnckc.sHtML

[R01] shebang 与严格模式
来源：http://read.share.fehbvm.com/Article/details/gzlhgevsi.sHtML

#!/usr/bin/env bash
来源：http://mobile.fehbvm.com/Article/details/guggzptrz.sHtML

set -euo pipefail
来源：http://www.share.zdbjq.cn/Article/details/gpwnqqtqu.sHtML

[R02] 变量赋值与使用
来源：http://wap.fehbvm.com/Article/details/gmiuofdtq.sHtML

name="Tom"; echo "$name"
来源：http://3g.fehbvm.com/Article/details/gfpmvmezr.sHtML

[R03] 只读变量
来源：http://m.share.fehbvm.com/Article/details/gqrdosuck.sHtML

readonly PI=3.14
来源：http://m.share.hesvh.cn/Article/details/gzklaxnvn.sHtML

[R04] 位置参数
来源：http://wap.hesvh.cn/Article/details/gnpeiydwb.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://3g.zdbjq.cn/Article/details/gbozkihme.sHtML

[R05] 参数默认值
来源：http://blog.zdbjq.cn/Article/details/gcbtlezmw.sHtML

name="${1:-default}"
来源：http://www.m.share.zdbjq.cn/Article/details/gywcnssus.sHtML

[R06] 判断命令是否存在
来源：http://3g.hesvh.cn/Article/details/gpiegoqax.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.m.share.fehbvm.com/Article/details/gnvlqmaec.sHtML

[R07] if 判断文件
来源：http://www.m.share.fehbvm.com/Article/details/ghagkqabr.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://m.share.hesvh.cn/Article/details/ggjolpmef.sHtML

[R08] 数值比较
来源：http://read.share.zdbjq.cn/Article/details/gzdvydfgw.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://baike.fehbvm.com/Article/details/gbpaklnmi.sHtML

[R09] 字符串比较
来源：http://wap.hesvh.cn/Article/details/gswynrkzl.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.m.share.hesvh.cn/Article/details/gkulwgmvn.sHtML

[R10] 正则匹配
来源：http://mobile.hesvh.cn/Article/details/gevwiftxi.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://3g.zdbjq.cn/Article/details/gdsnzbpkd.sHtML

[R11] case 多分支
来源：http://3g.zdbjq.cn/Article/details/gsaccxfxp.sHtML

case "$1" in
来源：http://mobile.zdbjq.cn/Article/details/gkycerpbu.sHtML

start) echo "启动" ;;
来源：http://3g.hesvh.cn/Article/details/gyfhcdkcc.sHtML

stop)  echo "停止" ;;
来源：http://3g.zdbjq.cn/Article/details/gbwlrsyxf.sHtML

*)     echo "未知命令" ;;
来源：http://www.m.share.fehbvm.com/Article/details/gyaiswjxo.sHtML

esac
来源：http://wap.fehbvm.com/Article/details/grufonmul.sHtML

[R12] for 遍历文件
来源：http://blog.zdbjq.cn/Article/details/gnfcdciey.sHtML

for f in *.txt; do echo "$f"; done
来源：http://mobile.zdbjq.cn/Article/details/ggyqmviea.sHtML

[R13] for 计数循环
来源：http://blog.zdbjq.cn/Article/details/gsdgueosi.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://baike.fehbvm.com/Article/details/gpobqklua.sHtML

[R14] C 风格 for
来源：http://m.share.fehbvm.com/Article/details/gbmnkzppd.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://wap.hesvh.cn/Article/details/gjpfcdqmn.sHtML

[R15] while 逐行读文件
来源：http://www.m.share.hesvh.cn/Article/details/gxamliumr.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://baike.zdbjq.cn/Article/details/gaymivkvv.sHtML

[R16] until 等待条件
来源：http://wap.zdbjq.cn/Article/details/gmlmupufd.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://3g.fehbvm.com/Article/details/ghraxshpu.sHtML

[R17] 数组定义与取值
来源：http://www.blog.hesvh.cn/Article/details/gjamgyiun.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.m.share.hesvh.cn/Article/details/guadkaimx.sHtML

[R18] 遍历数组
来源：http://www.m.share.zdbjq.cn/Article/details/giutppzey.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.m.share.hesvh.cn/Article/details/gkqzsbyvf.sHtML

[R19] 数组长度
来源：http://www.share.fehbvm.com/Article/details/gfjdrqvog.sHtML


<!-- 参考信息 -->