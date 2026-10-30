代发 wailian999

Py:   len(x)            # 字符串、列表、字典通用
来源：http://baike.hesvh.cn/Article/details/gderehybx.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.fehbvm.com/Article/details/gjyajatpb.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.zdbjq.cn/Article/details/gvbpzftja.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.hesvh.cn/Article/details/gvubxlode.sHtML

Java: list.size();  map.size();  s.length()
来源：http://blog.hesvh.cn/Article/details/gwdsnimtx.sHtML

Go:   len(arr);  len(m)
来源：http://www.m.share.hesvh.cn/Article/details/gwpwyztmf.sHtML

Ruby: x.length;  x.size
来源：http://mobile.fehbvm.com/Article/details/gushmnmyl.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://m.share.hesvh.cn/Article/details/gibkdmvrx.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.m.share.hesvh.cn/Article/details/gxdbkpoos.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.m.share.hesvh.cn/Article/details/gfkcmwcyi.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://m.share.fehbvm.com/Article/details/ggtrlgxvy.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://m.share.zdbjq.cn/Article/details/gtoqomsbv.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.zdbjq.cn/Article/details/gkptlzxrf.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://baike.zdbjq.cn/Article/details/gochoosjg.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.blog.hesvh.cn/Article/details/gjmnhwuzv.sHtML

Ruby: a == b
来源：http://www.m.share.fehbvm.com/Article/details/gmignlolo.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://wap.zdbjq.cn/Article/details/ghihswmog.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://wap.zdbjq.cn/Article/details/gfvcvcyxo.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://3g.fehbvm.com/Article/details/gjrypwqdd.sHtML

PHP:  if (empty($x)) {}
来源：http://www.m.share.fehbvm.com/Article/details/gxnczhbgo.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.m.share.hesvh.cn/Article/details/gqmmslltn.sHtML

TS:   if (x == null) {}
来源：http://www.blog.fehbvm.com/Article/details/gbyvdbcjy.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.share.zdbjq.cn/Article/details/gphjldpgz.sHtML

Go:   if x == nil {}
来源：http://baike.fehbvm.com/Article/details/geicxfgfr.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://m.share.zdbjq.cn/Article/details/gdkkwfhed.sHtML

C#:   if (x is null) {}
来源：http://baike.zdbjq.cn/Article/details/gkvrrdokz.sHtML

[P07] 防抖与节流
来源：http://m.share.fehbvm.com/Article/details/gbrfvdglb.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://blog.zdbjq.cn/Article/details/gpaoalmjv.sHtML

PHP:  // 手写时间戳比较
来源：http://www.share.hesvh.cn/Article/details/gagoyxxuz.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.fehbvm.com/Article/details/gngxevzrp.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.fehbvm.com/Article/details/gedmyjkya.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://mobile.hesvh.cn/Article/details/gbwaqrakw.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.share.hesvh.cn/Article/details/gjnkhowes.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://wap.fehbvm.com/Article/details/gldeokgyr.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://wap.fehbvm.com/Article/details/ghoejjwps.sHtML

[P08] 处理浮点精度问题
来源：http://www.m.share.zdbjq.cn/Article/details/gjqbkjody.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://mobile.hesvh.cn/Article/details/gfnjgbkra.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://baike.zdbjq.cn/Article/details/gcxgvszyp.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://read.share.fehbvm.com/Article/details/gqanwrxme.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://m.share.hesvh.cn/Article/details/gxziojzab.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://3g.hesvh.cn/Article/details/giuybjlfk.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://wap.fehbvm.com/Article/details/gdrffezfz.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://mobile.hesvh.cn/Article/details/gismzhzey.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://baike.zdbjq.cn/Article/details/gfllqtsjz.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gevlffkag.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.blog.zdbjq.cn/Article/details/ghbgowdzb.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/giiujppbe.sHtML

[Q01] 创建表
来源：http://baike.hesvh.cn/Article/details/gltekrqlt.sHtML

CREATE TABLE users (
来源：http://www.m.share.hesvh.cn/Article/details/gvpfaisga.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.fehbvm.com/Article/details/gaeldweak.sHtML

name VARCHAR(50) NOT NULL,
来源：http://baike.zdbjq.cn/Article/details/gqjqstjuj.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.m.share.zdbjq.cn/Article/details/gputjcpgk.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://m.share.zdbjq.cn/Article/details/gzmcwczwj.sHtML

);
来源：http://3g.hesvh.cn/Article/details/gezildhyk.sHtML

[Q02] 创建带外键的表
来源：http://read.share.fehbvm.com/Article/details/glewlthor.sHtML

CREATE TABLE orders (
来源：http://baike.fehbvm.com/Article/details/gnnznvskh.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.zdbjq.cn/Article/details/gjgunvkli.sHtML

user_id INT NOT NULL,
来源：http://3g.hesvh.cn/Article/details/gyoxghcih.sHtML

amount DECIMAL(10, 2),
来源：http://wap.zdbjq.cn/Article/details/gqlkpodjq.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://blog.hesvh.cn/Article/details/gikhwxqyg.sHtML

);
来源：http://3g.hesvh.cn/Article/details/gcttywziq.sHtML

[Q03] 增加列
来源：http://www.share.hesvh.cn/Article/details/giqdlwejv.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.m.share.zdbjq.cn/Article/details/gwpziayzo.sHtML

[Q04] 修改列类型
来源：http://mobile.fehbvm.com/Article/details/gyburhwfh.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://blog.zdbjq.cn/Article/details/gendjbhnw.sHtML

[Q05] 重命名列
来源：http://blog.fehbvm.com/Article/details/gvrdfniqq.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://3g.hesvh.cn/Article/details/gaobpicxx.sHtML

[Q06] 删除列
来源：http://m.share.hesvh.cn/Article/details/gzljpuzpi.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.blog.zdbjq.cn/Article/details/gmeysgwnv.sHtML

[Q07] 删除表
来源：http://baike.fehbvm.com/Article/details/gmgxviyxf.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.share.zdbjq.cn/Article/details/gzoqsrphm.sHtML

[Q08] 创建普通索引
来源：http://baike.fehbvm.com/Article/details/gvuqtxjok.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://blog.hesvh.cn/Article/details/gxvexieiz.sHtML

[Q09] 创建唯一索引
来源：http://blog.zdbjq.cn/Article/details/gcudaabxs.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://m.share.zdbjq.cn/Article/details/gxqcyxsoe.sHtML

[Q10] 插入单行
来源：http://www.share.zdbjq.cn/Article/details/gjxzufhmo.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://blog.hesvh.cn/Article/details/gpizpcmqh.sHtML

[Q11] 一次插入多行
来源：http://wap.zdbjq.cn/Article/details/gxhbtusjs.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://blog.zdbjq.cn/Article/details/gdrwfcmax.sHtML

[Q12] 插入后取自增 ID
来源：http://m.share.fehbvm.com/Article/details/gyoursbqi.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://blog.zdbjq.cn/Article/details/ggaobualu.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.m.share.zdbjq.cn/Article/details/gmuukpzpk.sHtML

[Q13] 忽略重复插入
来源：http://baike.fehbvm.com/Article/details/gzqqhbifp.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://blog.fehbvm.com/Article/details/gthbdhypq.sHtML

[Q14] 存在则更新（upsert）
来源：http://read.share.zdbjq.cn/Article/details/gzlvfexeu.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://read.share.fehbvm.com/Article/details/gelgnnjow.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://baike.zdbjq.cn/Article/details/grswldfhp.sHtML

[Q15] 查询全部
来源：http://baike.zdbjq.cn/Article/details/gaxrzajuh.sHtML

SELECT * FROM users;
来源：http://wap.hesvh.cn/Article/details/geeaosdow.sHtML

[Q16] 查询指定列
来源：http://baike.zdbjq.cn/Article/details/gnyyuuzem.sHtML

SELECT id, name FROM users;
来源：http://wap.hesvh.cn/Article/details/gcehajvdb.sHtML

[Q17] 条件查询
来源：http://m.share.hesvh.cn/Article/details/gmglrmbce.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://wap.fehbvm.com/Article/details/gloowttua.sHtML

[Q18] 模糊匹配
来源：http://baike.zdbjq.cn/Article/details/gkyyrqqzf.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://mobile.hesvh.cn/Article/details/gjjdueuph.sHtML

[Q19] 范围查询
来源：http://www.m.share.hesvh.cn/Article/details/ggjtwbwyx.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://read.share.hesvh.cn/Article/details/gtdmwgcoa.sHtML

[Q20] IN 列表
来源：http://wap.fehbvm.com/Article/details/gidivoktb.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://m.share.hesvh.cn/Article/details/gzkceqtuu.sHtML

[Q21] 空值判断
来源：http://baike.fehbvm.com/Article/details/ghalvihzc.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://wap.fehbvm.com/Article/details/gcopzekiy.sHtML

[Q22] 排序
来源：http://mobile.fehbvm.com/Article/details/gykazjaaz.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.m.share.zdbjq.cn/Article/details/gphkmomln.sHtML

[Q23] 分页
来源：http://www.blog.fehbvm.com/Article/details/glvufgjjc.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://blog.hesvh.cn/Article/details/gwocerkkg.sHtML

[Q24] 去重
来源：http://m.share.zdbjq.cn/Article/details/gziilhsrv.sHtML

SELECT DISTINCT city FROM users;
来源：http://baike.zdbjq.cn/Article/details/gbgkaqywh.sHtML

[Q25] 只取前 N 条
来源：http://baike.hesvh.cn/Article/details/gewzlpodk.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://3g.zdbjq.cn/Article/details/gtzbzgkug.sHtML

[Q26] 计数
来源：http://m.share.hesvh.cn/Article/details/gbodyluya.sHtML

SELECT COUNT(*) FROM users;
来源：http://baike.zdbjq.cn/Article/details/gibhxpfdj.sHtML

[Q27] 条件计数
来源：http://m.share.fehbvm.com/Article/details/ghprapaow.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://baike.fehbvm.com/Article/details/gpsasciky.sHtML

[Q28] 求和与平均
来源：http://wap.fehbvm.com/Article/details/ghysxjril.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://baike.hesvh.cn/Article/details/gnywidneq.sHtML

[Q29] 最大最小值
来源：http://wap.zdbjq.cn/Article/details/gbxkrrlpl.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.share.hesvh.cn/Article/details/gqqxdmdyh.sHtML

[Q30] 分组统计
来源：http://wap.hesvh.cn/Article/details/guvowfnev.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.blog.zdbjq.cn/Article/details/goguhcmcz.sHtML

[Q31] 分组后过滤
来源：http://m.share.zdbjq.cn/Article/details/gdqompyhm.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://blog.fehbvm.com/Article/details/gzrsgdvhc.sHtML

[Q32] 分组拼接字符串
来源：http://wap.hesvh.cn/Article/details/gdesvzhpx.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://baike.zdbjq.cn/Article/details/gjzhcdach.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.blog.hesvh.cn/Article/details/gakcworbs.sHtML

[Q33] 多列分组
来源：http://mobile.zdbjq.cn/Article/details/gqapilldg.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://blog.fehbvm.com/Article/details/gwshnxklq.sHtML

[Q34] 每组取第一条
来源：http://blog.hesvh.cn/Article/details/gtmlcwiec.sHtML

SELECT * FROM (
来源：http://baike.zdbjq.cn/Article/details/gdmwdbgdq.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://m.share.zdbjq.cn/Article/details/gcrtnhugx.sHtML

) t WHERE rn = 1;
来源：http://m.share.hesvh.cn/Article/details/gdxguanmh.sHtML

[Q35] 内连接
来源：http://3g.fehbvm.com/Article/details/gbzdrzwof.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://baike.zdbjq.cn/Article/details/gqjjbdqtz.sHtML

[Q36] 左连接
来源：http://wap.hesvh.cn/Article/details/gkbcnrrxt.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.zdbjq.cn/Article/details/gwytksfpq.sHtML

[Q37] 右连接
来源：http://www.blog.zdbjq.cn/Article/details/gczhycpll.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://baike.zdbjq.cn/Article/details/gurtlvgdn.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.m.share.hesvh.cn/Article/details/gtmkbkutn.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.share.fehbvm.com/Article/details/gcgqtkzel.sHtML

[Q39] 自连接（查上下级）
来源：http://baike.fehbvm.com/Article/details/gayccabff.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.blog.fehbvm.com/Article/details/grlfuqztd.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.m.share.fehbvm.com/Article/details/gigpicnws.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.m.share.hesvh.cn/Article/details/grplywgrh.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.blog.hesvh.cn/Article/details/gpoommhun.sHtML

[Q41] 多表连接
来源：http://baike.hesvh.cn/Article/details/gfzpcrkpz.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://3g.fehbvm.com/Article/details/gurphbqek.sHtML

JOIN users u ON u.id = o.user_id
来源：http://blog.fehbvm.com/Article/details/gguxeexdx.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://m.share.hesvh.cn/Article/details/gdzpefpbz.sHtML

[Q42] 连接条件附加过滤
来源：http://www.blog.zdbjq.cn/Article/details/gltjajwpv.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.share.zdbjq.cn/Article/details/gtrfhzstw.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://read.share.fehbvm.com/Article/details/gbowvyerq.sHtML

[Q43] 标量子查询
来源：http://3g.zdbjq.cn/Article/details/gnflktton.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.blog.hesvh.cn/Article/details/gcwpvkfei.sHtML

[Q44] IN 子查询
来源：http://wap.hesvh.cn/Article/details/gqoczzqgf.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.blog.fehbvm.com/Article/details/gfvfkqqqw.sHtML

[Q45] EXISTS 判断存在
来源：http://www.blog.hesvh.cn/Article/details/gnpjshffs.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.fehbvm.com/Article/details/gakqvwblb.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://wap.zdbjq.cn/Article/details/gnevonwjk.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.fehbvm.com/Article/details/ghdardwoa.sHtML

[Q47] 与平均值比较
来源：http://www.blog.zdbjq.cn/Article/details/gfcakrkle.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.blog.fehbvm.com/Article/details/gigrrnlof.sHtML

[Q48] CTE 公用表表达式
来源：http://baike.hesvh.cn/Article/details/gnyglwpei.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://baike.zdbjq.cn/Article/details/gdkandlkz.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://read.share.fehbvm.com/Article/details/gicomgtig.sHtML

[Q49] 更新单行
来源：http://www.share.hesvh.cn/Article/details/gikhqhdrg.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://m.share.fehbvm.com/Article/details/gyecxodrg.sHtML

[Q50] 批量更新
来源：http://m.share.fehbvm.com/Article/details/glbhskuvf.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://mobile.zdbjq.cn/Article/details/gwirnajua.sHtML

[Q51] 用子查询更新
来源：http://blog.zdbjq.cn/Article/details/gjzxgcily.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.blog.zdbjq.cn/Article/details/gbzifxeba.sHtML

[Q52] 删除指定行
来源：http://www.blog.zdbjq.cn/Article/details/gcqbunpyl.sHtML

DELETE FROM users WHERE id = 10;
来源：http://mobile.fehbvm.com/Article/details/gnbwdqmso.sHtML

[Q53] 按条件删除
来源：http://wap.fehbvm.com/Article/details/geoxqiihp.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.share.fehbvm.com/Article/details/greneldtl.sHtML

[Q54] 清空表
来源：http://blog.hesvh.cn/Article/details/gfzukubtf.sHtML

TRUNCATE TABLE logs;
来源：http://wap.hesvh.cn/Article/details/gmtnhmqka.sHtML

[Q55] 排名（并列占位）
来源：http://blog.fehbvm.com/Article/details/glaapzhhj.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.m.share.hesvh.cn/Article/details/gpaauagil.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.m.share.fehbvm.com/Article/details/gnflqjyex.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://m.share.zdbjq.cn/Article/details/ghybqhatu.sHtML

[Q57] 行号
来源：http://www.m.share.fehbvm.com/Article/details/grqzyhfmf.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://m.share.fehbvm.com/Article/details/gzskxxluw.sHtML

[Q58] 累计求和
来源：http://www.blog.zdbjq.cn/Article/details/gpwmlovqn.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://3g.fehbvm.com/Article/details/gtkjnyoyg.sHtML

[Q59] 分组内累计
来源：http://read.share.zdbjq.cn/Article/details/ghfublflc.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://read.share.zdbjq.cn/Article/details/gifkjvwze.sHtML

[Q60] 取上一行 / 下一行
来源：http://read.share.zdbjq.cn/Article/details/gnnjfqotn.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://mobile.zdbjq.cn/Article/details/gatoaqsev.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.m.share.zdbjq.cn/Article/details/gbojxavcd.sHtML

[Q61] 移动平均
来源：http://www.share.fehbvm.com/Article/details/gasdqphqf.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://blog.zdbjq.cn/Article/details/gtvaahujw.sHtML

[Q62] 分组占比
来源：http://mobile.zdbjq.cn/Article/details/gzijnywxv.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://mobile.hesvh.cn/Article/details/gyfshyiwo.sHtML

[Q63] 开启事务
来源：http://baike.hesvh.cn/Article/details/gkozsjxdc.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.m.share.hesvh.cn/Article/details/ghlrrntqn.sHtML

[Q64] 提交事务
来源：http://www.blog.zdbjq.cn/Article/details/ggzgjufor.sHtML

COMMIT;
来源：http://wap.hesvh.cn/Article/details/gocubvimz.sHtML

[Q65] 回滚事务
来源：http://www.m.share.hesvh.cn/Article/details/gobvvmlat.sHtML

ROLLBACK;
来源：http://www.blog.zdbjq.cn/Article/details/gmdugluqa.sHtML

[Q66] 行锁查询
来源：http://read.share.hesvh.cn/Article/details/gmhppuxtb.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://blog.zdbjq.cn/Article/details/gqsekxteo.sHtML

[Q67] 设置隔离级别
来源：http://www.share.hesvh.cn/Article/details/gbebgdrqf.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://wap.hesvh.cn/Article/details/gwrtofyto.sHtML

[Q68] 保存点
来源：http://m.share.fehbvm.com/Article/details/gvrnoioir.sHtML

SAVEPOINT sp1;
来源：http://3g.fehbvm.com/Article/details/geufranru.sHtML

ROLLBACK TO sp1;
来源：http://blog.zdbjq.cn/Article/details/gkausefam.sHtML

[Q69] 查看执行计划
来源：http://read.share.hesvh.cn/Article/details/gylqijqpr.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://3g.hesvh.cn/Article/details/gjfgtrcfb.sHtML

[Q70] 更新统计信息
来源：http://mobile.zdbjq.cn/Article/details/gqsstctrm.sHtML

ANALYZE TABLE users;
来源：http://3g.hesvh.cn/Article/details/gfxsoprjo.sHtML

[Q71] 查看建表语句
来源：http://m.share.fehbvm.com/Article/details/gmqxmezkm.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.m.share.hesvh.cn/Article/details/gyyxsvgfs.sHtML

[Q72] 查看索引
来源：http://mobile.fehbvm.com/Article/details/gxanjnbdh.sHtML

SHOW INDEX FROM users;
来源：http://wap.hesvh.cn/Article/details/ghhozykdu.sHtML

[Q73] 查看表状态
来源：http://www.share.fehbvm.com/Article/details/gbxzwixvq.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://wap.fehbvm.com/Article/details/gvlijwkin.sHtML

[Q74] 强制使用索引
来源：http://www.share.hesvh.cn/Article/details/ggfjuacru.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.m.share.hesvh.cn/Article/details/gpbideccy.sHtML

[Q75] 日期格式化
来源：http://www.m.share.hesvh.cn/Article/details/gsgfypnmi.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://read.share.hesvh.cn/Article/details/gdgyxgdjl.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://baike.zdbjq.cn/Article/details/gaugcdljl.sHtML

[Q76] 按天统计
来源：http://blog.zdbjq.cn/Article/details/gvgweoeof.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://blog.fehbvm.com/Article/details/gkafjxzen.sHtML

[Q77] 时间加减
来源：http://3g.hesvh.cn/Article/details/gdwpzsbks.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.blog.zdbjq.cn/Article/details/ggbetfqfk.sHtML

[Q78] 当前时间
来源：http://blog.hesvh.cn/Article/details/gampjvzfk.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://baike.hesvh.cn/Article/details/gmcmjrxjo.sHtML

[Q79] 字符串拼接
来源：http://3g.fehbvm.com/Article/details/gzpizbgdz.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://read.share.zdbjq.cn/Article/details/goicavcbc.sHtML

[Q80] 字符串截取
来源：http://wap.hesvh.cn/Article/details/gbqigezxm.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://baike.zdbjq.cn/Article/details/ggrvgoeqn.sHtML

[Q81] 字符串替换
来源：http://blog.hesvh.cn/Article/details/gwuntlduh.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gmycntcap.sHtML

[Q82] 字符长度与字节长度
来源：http://baike.hesvh.cn/Article/details/gyemznubd.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gqruzsmly.sHtML

[Q83] 大小写转换
来源：http://www.blog.hesvh.cn/Article/details/gwtxzqfeu.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://3g.hesvh.cn/Article/details/grwnefndb.sHtML

[Q84] 去除首尾空格
来源：http://www.blog.hesvh.cn/Article/details/gyabctitj.sHtML

SELECT TRIM(name) FROM users;
来源：http://baike.hesvh.cn/Article/details/giucrjhwp.sHtML

[Q85] 数值取整
来源：http://3g.fehbvm.com/Article/details/guvxfbahv.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://baike.zdbjq.cn/Article/details/gmfqtdrkc.sHtML

[Q86] 读取 JSON 字段
来源：http://www.m.share.zdbjq.cn/Article/details/gwsrlbarw.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://wap.fehbvm.com/Article/details/gplybjwbj.sHtML

[Q87] JSON 字段做条件
来源：http://wap.fehbvm.com/Article/details/gkeknkjtk.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://baike.zdbjq.cn/Article/details/gahtkmtfy.sHtML

[Q88] 行转列（条件聚合）
来源：http://blog.zdbjq.cn/Article/details/gsjzhtmyo.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.blog.fehbvm.com/Article/details/gfryhjtmj.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://wap.hesvh.cn/Article/details/ghuhvvkkm.sHtML

[Q89] 判断表是否存在
来源：http://mobile.zdbjq.cn/Article/details/geshwekid.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://mobile.fehbvm.com/Article/details/gsufktjfs.sHtML

[Q90] 生成序号列
来源：http://read.share.zdbjq.cn/Article/details/gvkikqwzc.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://m.share.zdbjq.cn/Article/details/getghomil.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/geryjgwxu.sHtML

R. Bash 专题
来源：http://baike.zdbjq.cn/Article/details/ggabmqvco.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gpbhlzgol.sHtML

[R01] shebang 与严格模式
来源：http://mobile.zdbjq.cn/Article/details/glzrcevdp.sHtML

#!/usr/bin/env bash
来源：http://baike.hesvh.cn/Article/details/gclwrlzfv.sHtML

set -euo pipefail
来源：http://www.share.hesvh.cn/Article/details/ghsdmqflw.sHtML

[R02] 变量赋值与使用
来源：http://mobile.hesvh.cn/Article/details/geisxhrsl.sHtML

name="Tom"; echo "$name"
来源：http://3g.zdbjq.cn/Article/details/glbhytsvc.sHtML

[R03] 只读变量
来源：http://www.blog.fehbvm.com/Article/details/gwslwewwq.sHtML

readonly PI=3.14
来源：http://www.share.hesvh.cn/Article/details/giocsjisj.sHtML

[R04] 位置参数
来源：http://3g.hesvh.cn/Article/details/gilqecvdk.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://m.share.hesvh.cn/Article/details/gwjvwnadu.sHtML

[R05] 参数默认值
来源：http://www.blog.fehbvm.com/Article/details/gdsqintrk.sHtML

name="${1:-default}"
来源：http://blog.fehbvm.com/Article/details/gvdyzwafx.sHtML

[R06] 判断命令是否存在
来源：http://3g.hesvh.cn/Article/details/gjgkvyzfz.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://m.share.zdbjq.cn/Article/details/gxxsgasnf.sHtML

[R07] if 判断文件
来源：http://read.share.hesvh.cn/Article/details/gsuphsmmv.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://wap.fehbvm.com/Article/details/gkpxiclcg.sHtML

[R08] 数值比较
来源：http://3g.hesvh.cn/Article/details/gqizhjuxk.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.share.hesvh.cn/Article/details/gzxwdqwlu.sHtML

[R09] 字符串比较
来源：http://mobile.zdbjq.cn/Article/details/gkccqucna.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.blog.hesvh.cn/Article/details/gvcggwfer.sHtML

[R10] 正则匹配
来源：http://mobile.zdbjq.cn/Article/details/gezlwdxhw.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.m.share.zdbjq.cn/Article/details/geuyugshi.sHtML

[R11] case 多分支
来源：http://www.m.share.fehbvm.com/Article/details/gnfnlpihf.sHtML

case "$1" in
来源：http://read.share.zdbjq.cn/Article/details/gotkqhrbp.sHtML

start) echo "启动" ;;
来源：http://wap.hesvh.cn/Article/details/gfewtgmkr.sHtML

stop)  echo "停止" ;;
来源：http://mobile.zdbjq.cn/Article/details/glzfkacii.sHtML

*)     echo "未知命令" ;;
来源：http://www.share.hesvh.cn/Article/details/gtrhihtru.sHtML

esac
来源：http://www.blog.zdbjq.cn/Article/details/gnfhepdyt.sHtML

[R12] for 遍历文件
来源：http://www.blog.fehbvm.com/Article/details/ghowypzax.sHtML

for f in *.txt; do echo "$f"; done
来源：http://blog.hesvh.cn/Article/details/gphdqjlmj.sHtML

[R13] for 计数循环
来源：http://baike.fehbvm.com/Article/details/grpxzvjdb.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.share.fehbvm.com/Article/details/gsuindnbt.sHtML

[R14] C 风格 for
来源：http://mobile.hesvh.cn/Article/details/gzdusqnrp.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.share.zdbjq.cn/Article/details/gsegglqze.sHtML

[R15] while 逐行读文件
来源：http://www.blog.hesvh.cn/Article/details/gankekkuu.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://read.share.zdbjq.cn/Article/details/ghwhhakei.sHtML

[R16] until 等待条件
来源：http://www.m.share.fehbvm.com/Article/details/gwdegemkb.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://3g.hesvh.cn/Article/details/glsptbvoz.sHtML

[R17] 数组定义与取值
来源：http://www.share.zdbjq.cn/Article/details/gojahjjfm.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://3g.fehbvm.com/Article/details/gtaelsjmy.sHtML

[R18] 遍历数组
来源：http://mobile.fehbvm.com/Article/details/gmjjckplz.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.m.share.zdbjq.cn/Article/details/gxeaoeeae.sHtML

[R19] 数组长度
来源：http://3g.fehbvm.com/Article/details/gnfxpuxfa.sHtML

echo "${#arr[@]}"
来源：http://wap.zdbjq.cn/Article/details/gxflgtylr.sHtML

[R20] 关联数组（字典）
来源：http://baike.zdbjq.cn/Article/details/gzsjezein.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://3g.zdbjq.cn/Article/details/ggxlcbuta.sHtML

[R21] 字符串长度
来源：http://wap.fehbvm.com/Article/details/glqgzhfry.sHtML


<!-- 参考信息 -->