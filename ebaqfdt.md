代发 wailian999

Ruby: Digest::SHA256.hexdigest(s)
来源：http://read.share.fehbvm.com/Article/details/gmsoblrfu.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.blog.hesvh.cn/Article/details/gvznfudbd.sHtML

[P03] 生成短随机字符串
来源：http://read.share.zdbjq.cn/Article/details/gvhrlihdo.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://wap.hesvh.cn/Article/details/gzvwhksyx.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.share.zdbjq.cn/Article/details/gxennlzxp.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.hesvh.cn/Article/details/gfyelcssu.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.hesvh.cn/Article/details/gookexsoh.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.share.hesvh.cn/Article/details/gnjcijfxg.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.share.hesvh.cn/Article/details/glmnkbnrs.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://wap.zdbjq.cn/Article/details/gilqkjiru.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://read.share.zdbjq.cn/Article/details/gzidvvrzx.sHtML

[P04] 求长度
来源：http://mobile.hesvh.cn/Article/details/gdlmghtwv.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://3g.hesvh.cn/Article/details/gqkhwvulh.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.share.fehbvm.com/Article/details/gllawvipk.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.hesvh.cn/Article/details/gtrpfcmcl.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.zdbjq.cn/Article/details/gypcgdtbi.sHtML

Java: list.size();  map.size();  s.length()
来源：http://3g.fehbvm.com/Article/details/gjblprnxa.sHtML

Go:   len(arr);  len(m)
来源：http://www.blog.fehbvm.com/Article/details/ggjfosjfi.sHtML

Ruby: x.length;  x.size
来源：http://m.share.fehbvm.com/Article/details/gtaicucsr.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.share.fehbvm.com/Article/details/gzxrpvuvr.sHtML

[P05] 判断两个对象内容是否相等
来源：http://3g.zdbjq.cn/Article/details/gxiewfcce.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://3g.fehbvm.com/Article/details/ghekhetfh.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.blog.fehbvm.com/Article/details/glnvfcjve.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://read.share.fehbvm.com/Article/details/gjbtlkwdw.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://wap.hesvh.cn/Article/details/gisbuqvje.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://m.share.fehbvm.com/Article/details/gkhizyyju.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.share.fehbvm.com/Article/details/gdzbajyfo.sHtML

Ruby: a == b
来源：http://www.share.zdbjq.cn/Article/details/gwadapzmr.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.share.hesvh.cn/Article/details/gruvlcugy.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://blog.fehbvm.com/Article/details/ggkyguzbk.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://3g.zdbjq.cn/Article/details/gtdcbotsv.sHtML

PHP:  if (empty($x)) {}
来源：http://baike.fehbvm.com/Article/details/gxadlmkhm.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://blog.zdbjq.cn/Article/details/gatdyypgs.sHtML

TS:   if (x == null) {}
来源：http://3g.zdbjq.cn/Article/details/gtmphyhhk.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.blog.fehbvm.com/Article/details/guwttpfva.sHtML

Go:   if x == nil {}
来源：http://mobile.fehbvm.com/Article/details/gxfflemca.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://read.share.hesvh.cn/Article/details/gfseqvbod.sHtML

C#:   if (x is null) {}
来源：http://www.share.zdbjq.cn/Article/details/geujaejna.sHtML

[P07] 防抖与节流
来源：http://wap.hesvh.cn/Article/details/gbxbmpsin.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://3g.hesvh.cn/Article/details/gdnvzelwy.sHtML

PHP:  // 手写时间戳比较
来源：http://3g.zdbjq.cn/Article/details/goeryrkbj.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.hesvh.cn/Article/details/gfkissjwp.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.zdbjq.cn/Article/details/ggpfvkbtd.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://mobile.hesvh.cn/Article/details/gjpsnayiz.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://baike.zdbjq.cn/Article/details/gnspupaxq.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://read.share.zdbjq.cn/Article/details/gmtipwziv.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://blog.zdbjq.cn/Article/details/gxxqncyhu.sHtML

[P08] 处理浮点精度问题
来源：http://3g.zdbjq.cn/Article/details/gdowxssgr.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://blog.fehbvm.com/Article/details/gvsbzankf.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://3g.fehbvm.com/Article/details/grleysbbr.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.m.share.zdbjq.cn/Article/details/gjsbmhmky.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://read.share.zdbjq.cn/Article/details/gpcicsmay.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://baike.hesvh.cn/Article/details/gzfvlemfw.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://blog.fehbvm.com/Article/details/gftmgqmqr.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://read.share.fehbvm.com/Article/details/ghcjgslsg.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.blog.fehbvm.com/Article/details/gcgjtxisl.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gufoczevu.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://blog.zdbjq.cn/Article/details/goarsswom.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gxnrmydek.sHtML

[Q01] 创建表
来源：http://www.blog.zdbjq.cn/Article/details/gfrvnbhry.sHtML

CREATE TABLE users (
来源：http://www.blog.hesvh.cn/Article/details/gqjazkahf.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.fehbvm.com/Article/details/gowjtrxlh.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.share.fehbvm.com/Article/details/gytxvdhxa.sHtML

email VARCHAR(100) UNIQUE,
来源：http://read.share.zdbjq.cn/Article/details/gkwpvttva.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://wap.zdbjq.cn/Article/details/gfwjpevoy.sHtML

);
来源：http://mobile.zdbjq.cn/Article/details/gupulmjhg.sHtML

[Q02] 创建带外键的表
来源：http://www.m.share.hesvh.cn/Article/details/gxejxiyod.sHtML

CREATE TABLE orders (
来源：http://www.blog.fehbvm.com/Article/details/gmdxxmlkx.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.hesvh.cn/Article/details/gfotvmnbb.sHtML

user_id INT NOT NULL,
来源：http://read.share.zdbjq.cn/Article/details/gkoidrzud.sHtML

amount DECIMAL(10, 2),
来源：http://wap.hesvh.cn/Article/details/gczdpjrhf.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://wap.fehbvm.com/Article/details/gwgopylxl.sHtML

);
来源：http://www.blog.zdbjq.cn/Article/details/gwxfkiinu.sHtML

[Q03] 增加列
来源：http://mobile.hesvh.cn/Article/details/glvpxrifc.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://m.share.fehbvm.com/Article/details/gshrtwigy.sHtML

[Q04] 修改列类型
来源：http://www.blog.hesvh.cn/Article/details/gobtzhujd.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://mobile.fehbvm.com/Article/details/gymanepie.sHtML

[Q05] 重命名列
来源：http://wap.fehbvm.com/Article/details/gobbkcihs.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.blog.fehbvm.com/Article/details/geoofhiat.sHtML

[Q06] 删除列
来源：http://www.blog.fehbvm.com/Article/details/gewegptbn.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.m.share.zdbjq.cn/Article/details/gntqwgieq.sHtML

[Q07] 删除表
来源：http://www.blog.hesvh.cn/Article/details/gevgpzuwi.sHtML

DROP TABLE IF EXISTS orders;
来源：http://wap.zdbjq.cn/Article/details/gvzmylevg.sHtML

[Q08] 创建普通索引
来源：http://www.share.hesvh.cn/Article/details/ghfnhroht.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.m.share.zdbjq.cn/Article/details/gkphhbbng.sHtML

[Q09] 创建唯一索引
来源：http://3g.zdbjq.cn/Article/details/gabkodhoi.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://blog.fehbvm.com/Article/details/gzzzfqwvq.sHtML

[Q10] 插入单行
来源：http://blog.zdbjq.cn/Article/details/grgcydbqn.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://wap.fehbvm.com/Article/details/gpxftjusf.sHtML

[Q11] 一次插入多行
来源：http://www.m.share.hesvh.cn/Article/details/gxychgbzc.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.share.hesvh.cn/Article/details/gdkqmqxxl.sHtML

[Q12] 插入后取自增 ID
来源：http://mobile.zdbjq.cn/Article/details/gprkfovcr.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.blog.fehbvm.com/Article/details/gdsxdbnbe.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.share.hesvh.cn/Article/details/gqmgordix.sHtML

[Q13] 忽略重复插入
来源：http://wap.fehbvm.com/Article/details/geftfefdm.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://baike.hesvh.cn/Article/details/gfghtwekn.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.m.share.fehbvm.com/Article/details/gtvvbvsmy.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://baike.zdbjq.cn/Article/details/gsvghspwg.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://3g.hesvh.cn/Article/details/gyyzlnrkh.sHtML

[Q15] 查询全部
来源：http://m.share.fehbvm.com/Article/details/gxosycihf.sHtML

SELECT * FROM users;
来源：http://blog.fehbvm.com/Article/details/gjpcoxgwq.sHtML

[Q16] 查询指定列
来源：http://3g.fehbvm.com/Article/details/gqiuuvqjz.sHtML

SELECT id, name FROM users;
来源：http://mobile.zdbjq.cn/Article/details/glwtocdwq.sHtML

[Q17] 条件查询
来源：http://read.share.hesvh.cn/Article/details/gxeljhscd.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://read.share.zdbjq.cn/Article/details/grmysrsyr.sHtML

[Q18] 模糊匹配
来源：http://wap.zdbjq.cn/Article/details/gzwdiupak.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://mobile.zdbjq.cn/Article/details/gainwdjtv.sHtML

[Q19] 范围查询
来源：http://www.share.zdbjq.cn/Article/details/gfukzbafi.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://blog.hesvh.cn/Article/details/gxifczhjj.sHtML

[Q20] IN 列表
来源：http://blog.zdbjq.cn/Article/details/gdiuleayx.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://baike.fehbvm.com/Article/details/gbvpctece.sHtML

[Q21] 空值判断
来源：http://mobile.zdbjq.cn/Article/details/gmfjipxeg.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.blog.hesvh.cn/Article/details/gnbfjirmr.sHtML

[Q22] 排序
来源：http://read.share.fehbvm.com/Article/details/gnaqkwmyn.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://blog.zdbjq.cn/Article/details/gsalavypx.sHtML

[Q23] 分页
来源：http://read.share.fehbvm.com/Article/details/gsqbwfueo.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://blog.fehbvm.com/Article/details/gamybuhrc.sHtML

[Q24] 去重
来源：http://www.blog.fehbvm.com/Article/details/gjbfaleri.sHtML

SELECT DISTINCT city FROM users;
来源：http://m.share.fehbvm.com/Article/details/ghsxzsmqw.sHtML

[Q25] 只取前 N 条
来源：http://m.share.fehbvm.com/Article/details/gsteofmik.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://blog.fehbvm.com/Article/details/gfilqaqos.sHtML

[Q26] 计数
来源：http://baike.hesvh.cn/Article/details/gmcbapfla.sHtML

SELECT COUNT(*) FROM users;
来源：http://read.share.hesvh.cn/Article/details/gfriziihh.sHtML

[Q27] 条件计数
来源：http://www.m.share.hesvh.cn/Article/details/gisfobxca.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://mobile.zdbjq.cn/Article/details/ghfpczhio.sHtML

[Q28] 求和与平均
来源：http://read.share.zdbjq.cn/Article/details/gjvlanwlj.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://m.share.hesvh.cn/Article/details/gvlokbuju.sHtML

[Q29] 最大最小值
来源：http://wap.hesvh.cn/Article/details/ghfgcfzpd.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gqrkvseip.sHtML

[Q30] 分组统计
来源：http://3g.fehbvm.com/Article/details/gwgkwaelo.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.m.share.zdbjq.cn/Article/details/goevouniu.sHtML

[Q31] 分组后过滤
来源：http://read.share.zdbjq.cn/Article/details/gaqoiznoa.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.m.share.zdbjq.cn/Article/details/grkndlphn.sHtML

[Q32] 分组拼接字符串
来源：http://mobile.hesvh.cn/Article/details/gobcyefxh.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://m.share.fehbvm.com/Article/details/gjmxegeqz.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://read.share.hesvh.cn/Article/details/gclujjuwv.sHtML

[Q33] 多列分组
来源：http://blog.fehbvm.com/Article/details/gdcdttnkh.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.share.zdbjq.cn/Article/details/gzizpfydb.sHtML

[Q34] 每组取第一条
来源：http://www.share.fehbvm.com/Article/details/giyulqpxg.sHtML

SELECT * FROM (
来源：http://blog.zdbjq.cn/Article/details/gsidmdisk.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://baike.fehbvm.com/Article/details/gurlhzmni.sHtML

) t WHERE rn = 1;
来源：http://blog.zdbjq.cn/Article/details/gluhxstht.sHtML

[Q35] 内连接
来源：http://www.share.hesvh.cn/Article/details/gmlpzwdmu.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.hesvh.cn/Article/details/gnjpedidw.sHtML

[Q36] 左连接
来源：http://wap.zdbjq.cn/Article/details/gxqmyfokm.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://3g.hesvh.cn/Article/details/gzeirnhsv.sHtML

[Q37] 右连接
来源：http://mobile.zdbjq.cn/Article/details/gblbznpqe.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.blog.zdbjq.cn/Article/details/gtmytquwj.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.share.hesvh.cn/Article/details/glnkfiefs.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.m.share.zdbjq.cn/Article/details/gfjtedqmj.sHtML

[Q39] 自连接（查上下级）
来源：http://www.blog.fehbvm.com/Article/details/gixbhcduq.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://mobile.hesvh.cn/Article/details/gokbzbzng.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.m.share.zdbjq.cn/Article/details/gmgzcnrqd.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://m.share.hesvh.cn/Article/details/gdinojomq.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://mobile.hesvh.cn/Article/details/gjldynosj.sHtML

[Q41] 多表连接
来源：http://blog.fehbvm.com/Article/details/gutjmzlvz.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://3g.fehbvm.com/Article/details/gnazurliz.sHtML

JOIN users u ON u.id = o.user_id
来源：http://wap.fehbvm.com/Article/details/gcaohfctw.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.share.hesvh.cn/Article/details/gwnsdygym.sHtML

[Q42] 连接条件附加过滤
来源：http://m.share.hesvh.cn/Article/details/gjptszwro.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.blog.fehbvm.com/Article/details/geydwyygb.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://wap.zdbjq.cn/Article/details/gcjhkndyp.sHtML

[Q43] 标量子查询
来源：http://read.share.fehbvm.com/Article/details/gweaycddl.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.m.share.zdbjq.cn/Article/details/gummdjcpa.sHtML

[Q44] IN 子查询
来源：http://read.share.fehbvm.com/Article/details/grsymcwwe.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://m.share.fehbvm.com/Article/details/gwoijrpsn.sHtML

[Q45] EXISTS 判断存在
来源：http://www.m.share.hesvh.cn/Article/details/gjkxlnwvj.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.fehbvm.com/Article/details/gugbuzums.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://mobile.hesvh.cn/Article/details/gtogshony.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.hesvh.cn/Article/details/gjeihpfhw.sHtML

[Q47] 与平均值比较
来源：http://wap.hesvh.cn/Article/details/gpvdteuhl.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.share.zdbjq.cn/Article/details/gwlwcqvud.sHtML

[Q48] CTE 公用表表达式
来源：http://mobile.zdbjq.cn/Article/details/gfsfsazmn.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://mobile.fehbvm.com/Article/details/gtmiffwru.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://mobile.hesvh.cn/Article/details/gstgdkhsv.sHtML

[Q49] 更新单行
来源：http://www.share.fehbvm.com/Article/details/gscqvtbda.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://blog.zdbjq.cn/Article/details/gufoyntwc.sHtML

[Q50] 批量更新
来源：http://www.share.hesvh.cn/Article/details/gyskoczvw.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.blog.hesvh.cn/Article/details/guylbosvc.sHtML

[Q51] 用子查询更新
来源：http://www.share.hesvh.cn/Article/details/gmujmviqz.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://blog.fehbvm.com/Article/details/gikwbdzra.sHtML

[Q52] 删除指定行
来源：http://wap.fehbvm.com/Article/details/gowvtttfa.sHtML

DELETE FROM users WHERE id = 10;
来源：http://wap.hesvh.cn/Article/details/grzglwxio.sHtML

[Q53] 按条件删除
来源：http://www.share.hesvh.cn/Article/details/guvqnttit.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://baike.fehbvm.com/Article/details/gvmafznhc.sHtML

[Q54] 清空表
来源：http://m.share.zdbjq.cn/Article/details/gdmohwrgv.sHtML

TRUNCATE TABLE logs;
来源：http://3g.zdbjq.cn/Article/details/gmxgqnnkz.sHtML

[Q55] 排名（并列占位）
来源：http://3g.zdbjq.cn/Article/details/gvzeebcna.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://wap.hesvh.cn/Article/details/ghfuxlcru.sHtML

[Q56] 密集排名（并列不占位）
来源：http://baike.fehbvm.com/Article/details/gzanasiig.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://blog.fehbvm.com/Article/details/gvtkhqxou.sHtML

[Q57] 行号
来源：http://wap.fehbvm.com/Article/details/gyuricmhh.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gubepzqwa.sHtML

[Q58] 累计求和
来源：http://m.share.hesvh.cn/Article/details/gbnezfxvn.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://mobile.hesvh.cn/Article/details/gpdhvuwwa.sHtML

[Q59] 分组内累计
来源：http://blog.fehbvm.com/Article/details/gfgacatth.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://mobile.zdbjq.cn/Article/details/glcawbcxs.sHtML

[Q60] 取上一行 / 下一行
来源：http://3g.zdbjq.cn/Article/details/gdspvtgev.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://m.share.fehbvm.com/Article/details/gznnqyuvt.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.blog.hesvh.cn/Article/details/gfmlttcmu.sHtML

[Q61] 移动平均
来源：http://mobile.hesvh.cn/Article/details/gggugowkw.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://baike.hesvh.cn/Article/details/guamzzlks.sHtML

[Q62] 分组占比
来源：http://m.share.fehbvm.com/Article/details/gdaukqrzp.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.share.zdbjq.cn/Article/details/goxnesaue.sHtML

[Q63] 开启事务
来源：http://wap.fehbvm.com/Article/details/gveembiyo.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://mobile.zdbjq.cn/Article/details/giclwozec.sHtML

[Q64] 提交事务
来源：http://blog.zdbjq.cn/Article/details/guylczfjc.sHtML

COMMIT;
来源：http://blog.fehbvm.com/Article/details/gthzbgbgb.sHtML

[Q65] 回滚事务
来源：http://www.share.zdbjq.cn/Article/details/giuoadjzu.sHtML

ROLLBACK;
来源：http://www.share.zdbjq.cn/Article/details/gpohwibkd.sHtML

[Q66] 行锁查询
来源：http://blog.hesvh.cn/Article/details/gqrpvtspc.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.m.share.fehbvm.com/Article/details/ghjiizqyh.sHtML

[Q67] 设置隔离级别
来源：http://www.share.hesvh.cn/Article/details/gcmwymbjo.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://wap.fehbvm.com/Article/details/gdtbuecey.sHtML

[Q68] 保存点
来源：http://mobile.zdbjq.cn/Article/details/gjrdqzviy.sHtML

SAVEPOINT sp1;
来源：http://m.share.hesvh.cn/Article/details/gzsieiand.sHtML

ROLLBACK TO sp1;
来源：http://blog.fehbvm.com/Article/details/gsvkazjsi.sHtML

[Q69] 查看执行计划
来源：http://www.blog.hesvh.cn/Article/details/gmkelaqsy.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.m.share.fehbvm.com/Article/details/gwqpxlwci.sHtML

[Q70] 更新统计信息
来源：http://blog.zdbjq.cn/Article/details/gxnhbceol.sHtML

ANALYZE TABLE users;
来源：http://read.share.hesvh.cn/Article/details/gsoevmqlu.sHtML

[Q71] 查看建表语句
来源：http://www.share.fehbvm.com/Article/details/gvsubkkno.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://mobile.fehbvm.com/Article/details/gwcibxuyz.sHtML

[Q72] 查看索引
来源：http://read.share.fehbvm.com/Article/details/gfmtmeqqb.sHtML

SHOW INDEX FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gpupxkaxj.sHtML

[Q73] 查看表状态
来源：http://www.m.share.fehbvm.com/Article/details/goysyzlrv.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.m.share.zdbjq.cn/Article/details/gnentvlsm.sHtML

[Q74] 强制使用索引
来源：http://wap.zdbjq.cn/Article/details/gsubgkztn.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://blog.hesvh.cn/Article/details/ghlkcimxi.sHtML

[Q75] 日期格式化
来源：http://www.blog.hesvh.cn/Article/details/gawuiephl.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://3g.hesvh.cn/Article/details/gvfarmwgx.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.blog.fehbvm.com/Article/details/gcynvwolv.sHtML

[Q76] 按天统计
来源：http://read.share.fehbvm.com/Article/details/gvllwccuw.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.share.hesvh.cn/Article/details/gywzijtnu.sHtML

[Q77] 时间加减
来源：http://www.share.hesvh.cn/Article/details/gfeaohbev.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://mobile.zdbjq.cn/Article/details/goytdmzad.sHtML

[Q78] 当前时间
来源：http://read.share.zdbjq.cn/Article/details/gcrrvushk.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://mobile.fehbvm.com/Article/details/gnhthpgns.sHtML

[Q79] 字符串拼接
来源：http://read.share.zdbjq.cn/Article/details/gpyshimde.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.share.zdbjq.cn/Article/details/goyxzhfqk.sHtML

[Q80] 字符串截取
来源：http://3g.zdbjq.cn/Article/details/ghktrirfy.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://3g.hesvh.cn/Article/details/gcitovrjq.sHtML

[Q81] 字符串替换
来源：http://read.share.hesvh.cn/Article/details/gudnbrnhv.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://m.share.fehbvm.com/Article/details/gnnpkcmat.sHtML

[Q82] 字符长度与字节长度
来源：http://wap.zdbjq.cn/Article/details/gouybucig.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/grxwfqsnr.sHtML

[Q83] 大小写转换
来源：http://read.share.zdbjq.cn/Article/details/gcquignse.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://blog.hesvh.cn/Article/details/gkcxjoozc.sHtML

[Q84] 去除首尾空格
来源：http://blog.zdbjq.cn/Article/details/gerfyysur.sHtML

SELECT TRIM(name) FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gvhbxzffv.sHtML

[Q85] 数值取整
来源：http://blog.hesvh.cn/Article/details/gntwjtnze.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.m.share.hesvh.cn/Article/details/gmuxeghuk.sHtML

[Q86] 读取 JSON 字段
来源：http://mobile.zdbjq.cn/Article/details/gxxdaogos.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://blog.fehbvm.com/Article/details/gggzhioqn.sHtML

[Q87] JSON 字段做条件
来源：http://www.m.share.hesvh.cn/Article/details/gbbficfnc.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://baike.hesvh.cn/Article/details/gekdmmcja.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.m.share.fehbvm.com/Article/details/griyragzj.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://3g.hesvh.cn/Article/details/gzyfrknrf.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://mobile.fehbvm.com/Article/details/ggkjyurbc.sHtML

[Q89] 判断表是否存在
来源：http://www.share.fehbvm.com/Article/details/gmfwzrmlr.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.blog.zdbjq.cn/Article/details/ghhrovcvc.sHtML

[Q90] 生成序号列
来源：http://wap.fehbvm.com/Article/details/gdnuvvtpn.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://read.share.zdbjq.cn/Article/details/gzsbgteuv.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gcwayedtg.sHtML

R. Bash 专题
来源：http://mobile.zdbjq.cn/Article/details/gxthokcqm.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gtdwjumjy.sHtML

[R01] shebang 与严格模式
来源：http://baike.fehbvm.com/Article/details/gzteoileg.sHtML

#!/usr/bin/env bash
来源：http://read.share.zdbjq.cn/Article/details/gepbaeuzj.sHtML

set -euo pipefail
来源：http://baike.hesvh.cn/Article/details/gtneatcea.sHtML

[R02] 变量赋值与使用
来源：http://3g.fehbvm.com/Article/details/goksgwnoc.sHtML

name="Tom"; echo "$name"
来源：http://baike.zdbjq.cn/Article/details/gyvsmaoyy.sHtML

[R03] 只读变量
来源：http://blog.hesvh.cn/Article/details/gzpmlcyrn.sHtML

readonly PI=3.14
来源：http://wap.fehbvm.com/Article/details/gbevwoika.sHtML

[R04] 位置参数
来源：http://www.blog.hesvh.cn/Article/details/glntossqn.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.m.share.hesvh.cn/Article/details/gqsxzqseq.sHtML

[R05] 参数默认值
来源：http://www.share.fehbvm.com/Article/details/gflwwlnum.sHtML

name="${1:-default}"
来源：http://www.blog.zdbjq.cn/Article/details/gmsdtyifd.sHtML

[R06] 判断命令是否存在
来源：http://baike.hesvh.cn/Article/details/gpgxrapnw.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://baike.hesvh.cn/Article/details/gkhygjtyh.sHtML

[R07] if 判断文件
来源：http://mobile.fehbvm.com/Article/details/gdqihytlq.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://3g.hesvh.cn/Article/details/gwhwuosdy.sHtML

[R08] 数值比较
来源：http://blog.hesvh.cn/Article/details/ghbxacbbd.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://3g.hesvh.cn/Article/details/glyrktbuk.sHtML

[R09] 字符串比较
来源：http://www.m.share.zdbjq.cn/Article/details/gibfzdzxn.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://read.share.hesvh.cn/Article/details/gsjqtnrzc.sHtML

[R10] 正则匹配
来源：http://www.blog.hesvh.cn/Article/details/gyayxtqsl.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://baike.fehbvm.com/Article/details/gooattyru.sHtML

[R11] case 多分支
来源：http://wap.fehbvm.com/Article/details/gsjmedmqk.sHtML

case "$1" in
来源：http://3g.hesvh.cn/Article/details/gemkrziys.sHtML

start) echo "启动" ;;
来源：http://www.m.share.hesvh.cn/Article/details/glnhqjuyp.sHtML

stop)  echo "停止" ;;
来源：http://www.blog.hesvh.cn/Article/details/gkduiuujs.sHtML

*)     echo "未知命令" ;;
来源：http://www.share.fehbvm.com/Article/details/gzfvuuidi.sHtML

esac
来源：http://3g.hesvh.cn/Article/details/gmujkpqat.sHtML

[R12] for 遍历文件
来源：http://m.share.fehbvm.com/Article/details/ggzhdycxa.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.blog.hesvh.cn/Article/details/guwrrdpts.sHtML

[R13] for 计数循环
来源：http://www.m.share.fehbvm.com/Article/details/gbaiwxelr.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://read.share.zdbjq.cn/Article/details/gimnheuuj.sHtML

[R14] C 风格 for
来源：http://www.share.hesvh.cn/Article/details/glrswxgtm.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.blog.hesvh.cn/Article/details/gmvywemiq.sHtML

[R15] while 逐行读文件
来源：http://blog.fehbvm.com/Article/details/gjpmelhda.sHtML


<!-- 参考信息 -->