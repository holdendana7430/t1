代发 wailian999

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.share.fehbvm.com/Article/details/gbexavwil.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://read.share.hesvh.cn/Article/details/gjthislqr.sHtML

[P03] 生成短随机字符串
来源：http://mobile.hesvh.cn/Article/details/gfkqhobgt.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.m.share.zdbjq.cn/Article/details/gqlbqlduj.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.share.fehbvm.com/Article/details/gjovgujyy.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.hesvh.cn/Article/details/gkrtqahxs.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.zdbjq.cn/Article/details/gtbunmlgy.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.m.share.fehbvm.com/Article/details/gazvjaagj.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.m.share.fehbvm.com/Article/details/gokdxmzbc.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://wap.zdbjq.cn/Article/details/gxmnaeloc.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://mobile.hesvh.cn/Article/details/gmhnrtykq.sHtML

[P04] 求长度
来源：http://mobile.hesvh.cn/Article/details/giokblrck.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://read.share.hesvh.cn/Article/details/gegsqtqur.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.share.fehbvm.com/Article/details/gsckpwyqg.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.zdbjq.cn/Article/details/ggletdtof.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.hesvh.cn/Article/details/ggzckersl.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.blog.fehbvm.com/Article/details/gfmqluuad.sHtML

Go:   len(arr);  len(m)
来源：http://wap.fehbvm.com/Article/details/ghefhthet.sHtML

Ruby: x.length;  x.size
来源：http://www.blog.zdbjq.cn/Article/details/gkttglnrs.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://blog.fehbvm.com/Article/details/gsomlwzaf.sHtML

[P05] 判断两个对象内容是否相等
来源：http://wap.hesvh.cn/Article/details/gjhzcxloo.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.blog.hesvh.cn/Article/details/gheoxsqyj.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.share.hesvh.cn/Article/details/gtxanhdmi.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://read.share.hesvh.cn/Article/details/gnriwcxkd.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://mobile.zdbjq.cn/Article/details/gnhsmqfmb.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://3g.fehbvm.com/Article/details/gxbcfmmmk.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.m.share.zdbjq.cn/Article/details/gvvtukhin.sHtML

Ruby: a == b
来源：http://mobile.zdbjq.cn/Article/details/gultmvmqj.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.blog.zdbjq.cn/Article/details/ggzqlstpt.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.blog.fehbvm.com/Article/details/gbisshlio.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://blog.hesvh.cn/Article/details/gvijpatsf.sHtML

PHP:  if (empty($x)) {}
来源：http://3g.hesvh.cn/Article/details/gugydpjvs.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.blog.hesvh.cn/Article/details/gxfzlqfnf.sHtML

TS:   if (x == null) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gwnqpdcki.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://baike.hesvh.cn/Article/details/gdaygdwon.sHtML

Go:   if x == nil {}
来源：http://mobile.hesvh.cn/Article/details/gnitwyzec.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://wap.hesvh.cn/Article/details/gtzskxday.sHtML

C#:   if (x is null) {}
来源：http://mobile.fehbvm.com/Article/details/gwegxuzla.sHtML

[P07] 防抖与节流
来源：http://www.share.fehbvm.com/Article/details/gyqkyixpm.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.m.share.hesvh.cn/Article/details/gkegixzok.sHtML

PHP:  // 手写时间戳比较
来源：http://mobile.fehbvm.com/Article/details/glodpzlmn.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.zdbjq.cn/Article/details/gzpicrwqg.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.fehbvm.com/Article/details/gmjdbujwb.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://mobile.zdbjq.cn/Article/details/gfnqcyics.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.share.hesvh.cn/Article/details/gkslimcoe.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://m.share.hesvh.cn/Article/details/gfafanqdj.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://baike.hesvh.cn/Article/details/gqgnchfbj.sHtML

[P08] 处理浮点精度问题
来源：http://read.share.hesvh.cn/Article/details/gnpmroffs.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.m.share.zdbjq.cn/Article/details/gvcwmhqbm.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.m.share.zdbjq.cn/Article/details/gwgciwtix.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://m.share.zdbjq.cn/Article/details/gyqgydgna.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.blog.zdbjq.cn/Article/details/gxetuyitg.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.share.fehbvm.com/Article/details/gpgjfitbu.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://wap.hesvh.cn/Article/details/gmvmvookp.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://m.share.fehbvm.com/Article/details/guiozeevn.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.m.share.zdbjq.cn/Article/details/giltafsyt.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/ggoozezfq.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://blog.fehbvm.com/Article/details/gdfobrbms.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gdtqkccei.sHtML

[Q01] 创建表
来源：http://read.share.hesvh.cn/Article/details/guhmrhzqz.sHtML

CREATE TABLE users (
来源：http://3g.fehbvm.com/Article/details/gjrhmzirg.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.hesvh.cn/Article/details/ghtxttsoz.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.m.share.hesvh.cn/Article/details/gmeismcdn.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.blog.zdbjq.cn/Article/details/gxbiwvblr.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://blog.fehbvm.com/Article/details/gprmbitad.sHtML

);
来源：http://blog.hesvh.cn/Article/details/gpbwmkqpu.sHtML

[Q02] 创建带外键的表
来源：http://wap.zdbjq.cn/Article/details/gbkbwbssj.sHtML

CREATE TABLE orders (
来源：http://www.blog.zdbjq.cn/Article/details/ghxtjvgpf.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.zdbjq.cn/Article/details/gixvjupef.sHtML

user_id INT NOT NULL,
来源：http://3g.fehbvm.com/Article/details/gkavtiftz.sHtML

amount DECIMAL(10, 2),
来源：http://blog.zdbjq.cn/Article/details/gpdqnsqnb.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://m.share.fehbvm.com/Article/details/giwlhbouw.sHtML

);
来源：http://www.blog.zdbjq.cn/Article/details/gvhqeftot.sHtML

[Q03] 增加列
来源：http://mobile.fehbvm.com/Article/details/gnddcahxy.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.blog.zdbjq.cn/Article/details/gmxufnblu.sHtML

[Q04] 修改列类型
来源：http://read.share.fehbvm.com/Article/details/gbozpwjfk.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://baike.fehbvm.com/Article/details/gxfrepxmf.sHtML

[Q05] 重命名列
来源：http://read.share.fehbvm.com/Article/details/ggfubjmhn.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://3g.zdbjq.cn/Article/details/gfwjvfvod.sHtML

[Q06] 删除列
来源：http://read.share.hesvh.cn/Article/details/gsybqpkls.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.blog.fehbvm.com/Article/details/gktuwpszb.sHtML

[Q07] 删除表
来源：http://wap.hesvh.cn/Article/details/ggiubmtjz.sHtML

DROP TABLE IF EXISTS orders;
来源：http://read.share.hesvh.cn/Article/details/gcohpovco.sHtML

[Q08] 创建普通索引
来源：http://blog.zdbjq.cn/Article/details/gdagomiaq.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.m.share.zdbjq.cn/Article/details/goyakmawk.sHtML

[Q09] 创建唯一索引
来源：http://3g.fehbvm.com/Article/details/gmhhhhabd.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://baike.fehbvm.com/Article/details/guhtcjxio.sHtML

[Q10] 插入单行
来源：http://mobile.zdbjq.cn/Article/details/glgmmufsv.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://baike.hesvh.cn/Article/details/gfitouath.sHtML

[Q11] 一次插入多行
来源：http://www.share.zdbjq.cn/Article/details/gcgmuxwjx.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://blog.zdbjq.cn/Article/details/ggmevbona.sHtML

[Q12] 插入后取自增 ID
来源：http://3g.zdbjq.cn/Article/details/gotdopopd.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://read.share.zdbjq.cn/Article/details/gpzpphhbp.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://read.share.fehbvm.com/Article/details/gsgsvhzru.sHtML

[Q13] 忽略重复插入
来源：http://3g.hesvh.cn/Article/details/gazwwibpc.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://m.share.zdbjq.cn/Article/details/gmpwsriun.sHtML

[Q14] 存在则更新（upsert）
来源：http://m.share.fehbvm.com/Article/details/gmzvqnxyp.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.m.share.hesvh.cn/Article/details/gmivhjvne.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://3g.fehbvm.com/Article/details/gvqttzpdg.sHtML

[Q15] 查询全部
来源：http://www.share.hesvh.cn/Article/details/glpqedhnk.sHtML

SELECT * FROM users;
来源：http://baike.hesvh.cn/Article/details/ggkgyukde.sHtML

[Q16] 查询指定列
来源：http://read.share.zdbjq.cn/Article/details/gtnvejios.sHtML

SELECT id, name FROM users;
来源：http://www.share.hesvh.cn/Article/details/gnqcfenmw.sHtML

[Q17] 条件查询
来源：http://m.share.hesvh.cn/Article/details/guukctlxs.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://3g.fehbvm.com/Article/details/gvbfhfqbg.sHtML

[Q18] 模糊匹配
来源：http://www.blog.zdbjq.cn/Article/details/gtquwbrco.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://3g.zdbjq.cn/Article/details/gekkazonm.sHtML

[Q19] 范围查询
来源：http://mobile.zdbjq.cn/Article/details/gnwcbiepc.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://mobile.fehbvm.com/Article/details/gmitorlyg.sHtML

[Q20] IN 列表
来源：http://www.m.share.fehbvm.com/Article/details/glbisgoii.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://3g.fehbvm.com/Article/details/gqiyryyig.sHtML

[Q21] 空值判断
来源：http://baike.hesvh.cn/Article/details/gdqudnyre.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.m.share.zdbjq.cn/Article/details/gkslqywfy.sHtML

[Q22] 排序
来源：http://baike.zdbjq.cn/Article/details/gzccuwbne.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://m.share.zdbjq.cn/Article/details/gebgcjnga.sHtML

[Q23] 分页
来源：http://www.m.share.zdbjq.cn/Article/details/gzzgzqnuw.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.share.zdbjq.cn/Article/details/grqtttkym.sHtML

[Q24] 去重
来源：http://mobile.zdbjq.cn/Article/details/gpvdgceni.sHtML

SELECT DISTINCT city FROM users;
来源：http://wap.zdbjq.cn/Article/details/gsykokrvn.sHtML

[Q25] 只取前 N 条
来源：http://www.share.hesvh.cn/Article/details/germnulcb.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://m.share.hesvh.cn/Article/details/gdaucovfg.sHtML

[Q26] 计数
来源：http://blog.zdbjq.cn/Article/details/gewzvjntx.sHtML

SELECT COUNT(*) FROM users;
来源：http://baike.fehbvm.com/Article/details/gmyizlvsj.sHtML

[Q27] 条件计数
来源：http://blog.fehbvm.com/Article/details/gapdmdusu.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gfxynvbme.sHtML

[Q28] 求和与平均
来源：http://www.share.hesvh.cn/Article/details/gdpivahbl.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://read.share.fehbvm.com/Article/details/gxinzbfvg.sHtML

[Q29] 最大最小值
来源：http://www.blog.zdbjq.cn/Article/details/gmlvbsszc.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://read.share.fehbvm.com/Article/details/ghtwkmyic.sHtML

[Q30] 分组统计
来源：http://www.blog.fehbvm.com/Article/details/gnjuyvyau.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://mobile.zdbjq.cn/Article/details/ghekybbtj.sHtML

[Q31] 分组后过滤
来源：http://m.share.fehbvm.com/Article/details/gdbcyvvdv.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.m.share.zdbjq.cn/Article/details/geikymdqa.sHtML

[Q32] 分组拼接字符串
来源：http://www.share.zdbjq.cn/Article/details/gfvsbaspd.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://m.share.fehbvm.com/Article/details/giragenfu.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://m.share.hesvh.cn/Article/details/grurpuymb.sHtML

[Q33] 多列分组
来源：http://www.blog.zdbjq.cn/Article/details/gkirkpmzm.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://read.share.hesvh.cn/Article/details/gzoqyqjag.sHtML

[Q34] 每组取第一条
来源：http://www.share.hesvh.cn/Article/details/gmzoaajsr.sHtML

SELECT * FROM (
来源：http://mobile.fehbvm.com/Article/details/ggodnmrbt.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://3g.hesvh.cn/Article/details/gppkaolty.sHtML

) t WHERE rn = 1;
来源：http://mobile.hesvh.cn/Article/details/gtvwqknya.sHtML

[Q35] 内连接
来源：http://read.share.zdbjq.cn/Article/details/gbjuqktuf.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.zdbjq.cn/Article/details/gnbakelcf.sHtML

[Q36] 左连接
来源：http://www.share.zdbjq.cn/Article/details/gxjzkfrkg.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://baike.zdbjq.cn/Article/details/gvsldiipi.sHtML

[Q37] 右连接
来源：http://baike.fehbvm.com/Article/details/glmfhlkio.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://3g.hesvh.cn/Article/details/gaxaqsjeb.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.m.share.zdbjq.cn/Article/details/gzretersy.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.blog.fehbvm.com/Article/details/giujvrpmr.sHtML

[Q39] 自连接（查上下级）
来源：http://read.share.zdbjq.cn/Article/details/ggypmfdcb.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://3g.zdbjq.cn/Article/details/gpxrbmqql.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://3g.zdbjq.cn/Article/details/gaetfvtja.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.blog.fehbvm.com/Article/details/gfvlpubxk.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://m.share.hesvh.cn/Article/details/gznesfunf.sHtML

[Q41] 多表连接
来源：http://mobile.zdbjq.cn/Article/details/gkkgduuez.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://read.share.fehbvm.com/Article/details/gvznlwblh.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.m.share.fehbvm.com/Article/details/gnknuomte.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.share.hesvh.cn/Article/details/gizxawifp.sHtML

[Q42] 连接条件附加过滤
来源：http://www.share.zdbjq.cn/Article/details/gczsclhtz.sHtML

SELECT u.name, o.amount FROM users u
来源：http://wap.zdbjq.cn/Article/details/gonrzozpn.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.share.hesvh.cn/Article/details/gcddfypkw.sHtML

[Q43] 标量子查询
来源：http://wap.zdbjq.cn/Article/details/gzdcugrnj.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://read.share.hesvh.cn/Article/details/gqitoecfc.sHtML

[Q44] IN 子查询
来源：http://mobile.fehbvm.com/Article/details/glxdlsvke.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://read.share.fehbvm.com/Article/details/gytrahjcx.sHtML

[Q45] EXISTS 判断存在
来源：http://wap.fehbvm.com/Article/details/gqhdhspzt.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.hesvh.cn/Article/details/gnvtxjtpi.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://baike.fehbvm.com/Article/details/gzbqtawzm.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.fehbvm.com/Article/details/gmeqmhcts.sHtML

[Q47] 与平均值比较
来源：http://www.share.fehbvm.com/Article/details/gpjtmxwsz.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://blog.hesvh.cn/Article/details/gzpvupwcy.sHtML

[Q48] CTE 公用表表达式
来源：http://www.share.zdbjq.cn/Article/details/givsoyqaa.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.blog.hesvh.cn/Article/details/gwpigrrub.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.blog.fehbvm.com/Article/details/goqwfbqsn.sHtML

[Q49] 更新单行
来源：http://www.blog.fehbvm.com/Article/details/gflmnbhhu.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://wap.hesvh.cn/Article/details/gmcaljmve.sHtML

[Q50] 批量更新
来源：http://mobile.zdbjq.cn/Article/details/gbrplpyza.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://read.share.fehbvm.com/Article/details/gutzlckjm.sHtML

[Q51] 用子查询更新
来源：http://3g.zdbjq.cn/Article/details/gypoxqmco.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://baike.fehbvm.com/Article/details/gztvuzozq.sHtML

[Q52] 删除指定行
来源：http://www.m.share.zdbjq.cn/Article/details/gkqmvkrbs.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.m.share.zdbjq.cn/Article/details/gvwsvwqus.sHtML

[Q53] 按条件删除
来源：http://read.share.hesvh.cn/Article/details/gbetualdl.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://blog.fehbvm.com/Article/details/grlhbynyk.sHtML

[Q54] 清空表
来源：http://mobile.zdbjq.cn/Article/details/gpbvfrvkc.sHtML

TRUNCATE TABLE logs;
来源：http://www.share.fehbvm.com/Article/details/gnlydjbxj.sHtML

[Q55] 排名（并列占位）
来源：http://www.m.share.hesvh.cn/Article/details/gypdighxu.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.blog.hesvh.cn/Article/details/gdjfhzxhu.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.blog.zdbjq.cn/Article/details/gtvnajaco.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://read.share.hesvh.cn/Article/details/gwmxgjtfd.sHtML

[Q57] 行号
来源：http://www.m.share.fehbvm.com/Article/details/gxptuwxtp.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gzjenveoc.sHtML

[Q58] 累计求和
来源：http://wap.zdbjq.cn/Article/details/gakjjnujl.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.m.share.zdbjq.cn/Article/details/gzgglseih.sHtML

[Q59] 分组内累计
来源：http://m.share.fehbvm.com/Article/details/gxdupdcep.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://mobile.fehbvm.com/Article/details/glekcpbpv.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.m.share.fehbvm.com/Article/details/glrndwnuw.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://3g.zdbjq.cn/Article/details/gixpgvpys.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://wap.fehbvm.com/Article/details/gveyxbgfz.sHtML

[Q61] 移动平均
来源：http://www.blog.hesvh.cn/Article/details/grxeqnaxs.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://mobile.hesvh.cn/Article/details/gnadynyvw.sHtML

[Q62] 分组占比
来源：http://mobile.zdbjq.cn/Article/details/gqxatjzlt.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://baike.hesvh.cn/Article/details/gwlazwaug.sHtML

[Q63] 开启事务
来源：http://baike.fehbvm.com/Article/details/gblpcqowi.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://3g.hesvh.cn/Article/details/gvtbiarku.sHtML

[Q64] 提交事务
来源：http://baike.zdbjq.cn/Article/details/ggtdfgoit.sHtML

COMMIT;
来源：http://3g.hesvh.cn/Article/details/glxalrjsi.sHtML

[Q65] 回滚事务
来源：http://m.share.hesvh.cn/Article/details/gvunettnj.sHtML

ROLLBACK;
来源：http://m.share.fehbvm.com/Article/details/gfuynlnfp.sHtML

[Q66] 行锁查询
来源：http://wap.fehbvm.com/Article/details/gxezgdvff.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.m.share.fehbvm.com/Article/details/guwqbhhwi.sHtML

[Q67] 设置隔离级别
来源：http://www.m.share.zdbjq.cn/Article/details/ggmwtasks.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.m.share.hesvh.cn/Article/details/gaqhqnfpj.sHtML

[Q68] 保存点
来源：http://www.share.zdbjq.cn/Article/details/gsnrkrpdx.sHtML

SAVEPOINT sp1;
来源：http://m.share.fehbvm.com/Article/details/gzhpleldu.sHtML

ROLLBACK TO sp1;
来源：http://m.share.zdbjq.cn/Article/details/gcmbwmsyj.sHtML

[Q69] 查看执行计划
来源：http://blog.zdbjq.cn/Article/details/gghryxcpn.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://blog.hesvh.cn/Article/details/gapfocjdm.sHtML

[Q70] 更新统计信息
来源：http://www.m.share.zdbjq.cn/Article/details/gvxjttlgi.sHtML

ANALYZE TABLE users;
来源：http://www.share.fehbvm.com/Article/details/ghlwnzywr.sHtML

[Q71] 查看建表语句
来源：http://www.m.share.hesvh.cn/Article/details/ggjyhuxtm.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://m.share.zdbjq.cn/Article/details/gsmxufddp.sHtML

[Q72] 查看索引
来源：http://baike.hesvh.cn/Article/details/gfmgwavco.sHtML

SHOW INDEX FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gbadkegzw.sHtML

[Q73] 查看表状态
来源：http://baike.zdbjq.cn/Article/details/gmntzipux.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://m.share.fehbvm.com/Article/details/gomebwibh.sHtML

[Q74] 强制使用索引
来源：http://3g.fehbvm.com/Article/details/gvhgfvdfe.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://3g.fehbvm.com/Article/details/gwiudhetv.sHtML

[Q75] 日期格式化
来源：http://mobile.fehbvm.com/Article/details/gaypsjmcb.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://baike.hesvh.cn/Article/details/gffaezwjt.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://read.share.fehbvm.com/Article/details/genmhfwpv.sHtML

[Q76] 按天统计
来源：http://mobile.fehbvm.com/Article/details/gpxmvgvcw.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://read.share.hesvh.cn/Article/details/geuhvojmd.sHtML

[Q77] 时间加减
来源：http://m.share.hesvh.cn/Article/details/gicadruxw.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://m.share.hesvh.cn/Article/details/gthnyhahe.sHtML

[Q78] 当前时间
来源：http://read.share.fehbvm.com/Article/details/gadgeyqet.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://m.share.fehbvm.com/Article/details/giwtnjele.sHtML

[Q79] 字符串拼接
来源：http://www.m.share.zdbjq.cn/Article/details/gelvlanrk.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://m.share.zdbjq.cn/Article/details/gkfxaawyn.sHtML

[Q80] 字符串截取
来源：http://baike.zdbjq.cn/Article/details/gyqkvxpvo.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gqzuoitjv.sHtML

[Q81] 字符串替换
来源：http://www.m.share.fehbvm.com/Article/details/gdphzyqup.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://blog.fehbvm.com/Article/details/gzkyyvlfw.sHtML

[Q82] 字符长度与字节长度
来源：http://baike.zdbjq.cn/Article/details/grqpghxtj.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://blog.zdbjq.cn/Article/details/gzeomhvkd.sHtML

[Q83] 大小写转换
来源：http://mobile.hesvh.cn/Article/details/gvqiayeqi.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://mobile.zdbjq.cn/Article/details/glympaiwp.sHtML

[Q84] 去除首尾空格
来源：http://read.share.fehbvm.com/Article/details/gfyzlozml.sHtML

SELECT TRIM(name) FROM users;
来源：http://3g.fehbvm.com/Article/details/gtmllryux.sHtML

[Q85] 数值取整
来源：http://www.m.share.fehbvm.com/Article/details/gwknufcgn.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://wap.fehbvm.com/Article/details/gaobkvybt.sHtML

[Q86] 读取 JSON 字段
来源：http://blog.zdbjq.cn/Article/details/gtrhgepxo.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.m.share.zdbjq.cn/Article/details/gnamixpdy.sHtML

[Q87] JSON 字段做条件
来源：http://www.blog.fehbvm.com/Article/details/gxffkaagj.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.share.hesvh.cn/Article/details/godskcplv.sHtML

[Q88] 行转列（条件聚合）
来源：http://mobile.fehbvm.com/Article/details/geyhkwgdr.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.share.zdbjq.cn/Article/details/ggeqmxgwa.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://wap.zdbjq.cn/Article/details/gzrhghrow.sHtML

[Q89] 判断表是否存在
来源：http://baike.zdbjq.cn/Article/details/glagwiwqj.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://baike.zdbjq.cn/Article/details/gptalnfmw.sHtML

[Q90] 生成序号列
来源：http://blog.fehbvm.com/Article/details/ghkjmyigt.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.blog.hesvh.cn/Article/details/gaznslymk.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gtgbdrejn.sHtML

R. Bash 专题
来源：http://3g.zdbjq.cn/Article/details/gsapcgfbh.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gnebhvobo.sHtML

[R01] shebang 与严格模式
来源：http://read.share.hesvh.cn/Article/details/giissnuor.sHtML

#!/usr/bin/env bash
来源：http://www.share.zdbjq.cn/Article/details/gmpnbcije.sHtML

set -euo pipefail
来源：http://www.m.share.fehbvm.com/Article/details/gcvzxokyo.sHtML

[R02] 变量赋值与使用
来源：http://mobile.hesvh.cn/Article/details/grurtfshv.sHtML

name="Tom"; echo "$name"
来源：http://3g.fehbvm.com/Article/details/gnczgpyhs.sHtML

[R03] 只读变量
来源：http://www.m.share.hesvh.cn/Article/details/gneoksugl.sHtML

readonly PI=3.14
来源：http://3g.hesvh.cn/Article/details/gitfkzrtc.sHtML

[R04] 位置参数
来源：http://www.m.share.zdbjq.cn/Article/details/guelfinnp.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://3g.fehbvm.com/Article/details/gmqhyymlo.sHtML

[R05] 参数默认值
来源：http://www.share.hesvh.cn/Article/details/gevgcvrkd.sHtML

name="${1:-default}"
来源：http://wap.hesvh.cn/Article/details/gfaklnatd.sHtML

[R06] 判断命令是否存在
来源：http://baike.zdbjq.cn/Article/details/gddowhngh.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.blog.fehbvm.com/Article/details/grymnawnc.sHtML

[R07] if 判断文件
来源：http://blog.fehbvm.com/Article/details/gtpvwmgpb.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://m.share.hesvh.cn/Article/details/gegisorwq.sHtML

[R08] 数值比较
来源：http://baike.zdbjq.cn/Article/details/gpiypqvwz.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://read.share.fehbvm.com/Article/details/goityeupk.sHtML

[R09] 字符串比较
来源：http://baike.hesvh.cn/Article/details/ghjytqwey.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://read.share.fehbvm.com/Article/details/gezhebwoc.sHtML

[R10] 正则匹配
来源：http://3g.hesvh.cn/Article/details/gkrofbjrl.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://baike.fehbvm.com/Article/details/gfqfirtxd.sHtML

[R11] case 多分支
来源：http://www.blog.hesvh.cn/Article/details/guzkfnncr.sHtML

case "$1" in
来源：http://m.share.hesvh.cn/Article/details/gdagwozul.sHtML

start) echo "启动" ;;
来源：http://baike.hesvh.cn/Article/details/gqbinxooh.sHtML

stop)  echo "停止" ;;
来源：http://www.share.fehbvm.com/Article/details/gkpuiqmsv.sHtML

*)     echo "未知命令" ;;
来源：http://www.m.share.hesvh.cn/Article/details/gtzamuavu.sHtML

esac
来源：http://www.m.share.zdbjq.cn/Article/details/gpcamzsor.sHtML

[R12] for 遍历文件
来源：http://m.share.zdbjq.cn/Article/details/gababbapw.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.m.share.fehbvm.com/Article/details/gtxglgwrj.sHtML

[R13] for 计数循环
来源：http://www.m.share.zdbjq.cn/Article/details/ghxqbjnnp.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://baike.zdbjq.cn/Article/details/gvyagckca.sHtML

[R14] C 风格 for
来源：http://blog.hesvh.cn/Article/details/gxgsjyfca.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://m.share.hesvh.cn/Article/details/gbtkcmyfw.sHtML

[R15] while 逐行读文件
来源：http://www.share.hesvh.cn/Article/details/gfiknfays.sHtML


<!-- 参考信息 -->