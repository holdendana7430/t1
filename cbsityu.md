代发 wailian999

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.blog.zdbjq.cn/Article/details/gutuiusdk.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.share.hesvh.cn/Article/details/gvrktknmv.sHtML

[P03] 生成短随机字符串
来源：http://m.share.hesvh.cn/Article/details/gwbzjlogu.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://3g.fehbvm.com/Article/details/gqkgzkdkr.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://3g.hesvh.cn/Article/details/goncqzomc.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.zdbjq.cn/Article/details/gouondhtq.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.fehbvm.com/Article/details/grwhspuio.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://baike.hesvh.cn/Article/details/gsyvufbuz.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.blog.zdbjq.cn/Article/details/gzishbxyr.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://m.share.zdbjq.cn/Article/details/gluveuaqd.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://m.share.zdbjq.cn/Article/details/gdmbzsuru.sHtML

[P04] 求长度
来源：http://baike.fehbvm.com/Article/details/gunmkocpn.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://wap.hesvh.cn/Article/details/gxkifyamu.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.hesvh.cn/Article/details/gcmgpdbfu.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mobile.zdbjq.cn/Article/details/gekatqzdc.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.fehbvm.com/Article/details/ggdtmewiu.sHtML

Java: list.size();  map.size();  s.length()
来源：http://3g.fehbvm.com/Article/details/gpgcdxvve.sHtML

Go:   len(arr);  len(m)
来源：http://www.blog.zdbjq.cn/Article/details/gubtbbbod.sHtML

Ruby: x.length;  x.size
来源：http://read.share.fehbvm.com/Article/details/gplojlipg.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://wap.fehbvm.com/Article/details/gxghncevs.sHtML

[P05] 判断两个对象内容是否相等
来源：http://read.share.hesvh.cn/Article/details/gbjxjtbtk.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://baike.fehbvm.com/Article/details/gbvkjpjgr.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://baike.hesvh.cn/Article/details/gnefokzme.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.blog.fehbvm.com/Article/details/gvlhbqisn.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://m.share.hesvh.cn/Article/details/gmwkatlhi.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://blog.zdbjq.cn/Article/details/gigccdejg.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.blog.hesvh.cn/Article/details/gbmopdlgt.sHtML

Ruby: a == b
来源：http://www.m.share.hesvh.cn/Article/details/gzlwymusg.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://baike.fehbvm.com/Article/details/gshlasuwc.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://read.share.zdbjq.cn/Article/details/gekyzviwb.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://baike.fehbvm.com/Article/details/goirhbeyw.sHtML

PHP:  if (empty($x)) {}
来源：http://www.share.fehbvm.com/Article/details/gavcqslkp.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.blog.hesvh.cn/Article/details/gbeinskpp.sHtML

TS:   if (x == null) {}
来源：http://www.share.zdbjq.cn/Article/details/guailyztk.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://mobile.zdbjq.cn/Article/details/gsurbftgv.sHtML

Go:   if x == nil {}
来源：http://mobile.zdbjq.cn/Article/details/gbwlsgoip.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.m.share.hesvh.cn/Article/details/glljlajui.sHtML

C#:   if (x is null) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gvadsygkk.sHtML

[P07] 防抖与节流
来源：http://www.share.zdbjq.cn/Article/details/gczqopzqm.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.m.share.fehbvm.com/Article/details/gpmhwqsoo.sHtML

PHP:  // 手写时间戳比较
来源：http://www.blog.zdbjq.cn/Article/details/gkpvggmom.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.hesvh.cn/Article/details/gtpwuqlka.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.fehbvm.com/Article/details/grjhkjwmn.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.blog.hesvh.cn/Article/details/gstcetjfe.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://baike.zdbjq.cn/Article/details/gqdqagzip.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.m.share.fehbvm.com/Article/details/gcnfgcxfx.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://read.share.hesvh.cn/Article/details/guwqtcdbt.sHtML

[P08] 处理浮点精度问题
来源：http://www.blog.hesvh.cn/Article/details/goiagaetw.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://wap.hesvh.cn/Article/details/gphsyvlzs.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://blog.fehbvm.com/Article/details/gzdasjgzq.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://wap.fehbvm.com/Article/details/guodxjbey.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://m.share.zdbjq.cn/Article/details/gzvgrbhym.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.share.zdbjq.cn/Article/details/gynarvbwd.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.blog.hesvh.cn/Article/details/gonvdjgje.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://wap.zdbjq.cn/Article/details/gvmnqtcqw.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.share.fehbvm.com/Article/details/guaimlaaq.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gurpcscvl.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://3g.hesvh.cn/Article/details/gzrbamdjz.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gthgacags.sHtML

[Q01] 创建表
来源：http://wap.fehbvm.com/Article/details/gsveamhta.sHtML

CREATE TABLE users (
来源：http://www.m.share.zdbjq.cn/Article/details/gohkbjqdy.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.hesvh.cn/Article/details/gotumwxmv.sHtML

name VARCHAR(50) NOT NULL,
来源：http://wap.zdbjq.cn/Article/details/gwdrujoib.sHtML

email VARCHAR(100) UNIQUE,
来源：http://mobile.hesvh.cn/Article/details/ghubntvww.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.blog.hesvh.cn/Article/details/gvbkkwoot.sHtML

);
来源：http://wap.hesvh.cn/Article/details/gijeynneu.sHtML

[Q02] 创建带外键的表
来源：http://m.share.zdbjq.cn/Article/details/grichsydp.sHtML

CREATE TABLE orders (
来源：http://baike.zdbjq.cn/Article/details/ggvqbridz.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.share.zdbjq.cn/Article/details/glddvjapr.sHtML

user_id INT NOT NULL,
来源：http://read.share.zdbjq.cn/Article/details/gmdynlwmh.sHtML

amount DECIMAL(10, 2),
来源：http://www.m.share.zdbjq.cn/Article/details/gutxofzdq.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://m.share.zdbjq.cn/Article/details/gpplmeumq.sHtML

);
来源：http://wap.fehbvm.com/Article/details/gtygdewwe.sHtML

[Q03] 增加列
来源：http://blog.zdbjq.cn/Article/details/gxovwnywt.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://wap.fehbvm.com/Article/details/gutlxtjrr.sHtML

[Q04] 修改列类型
来源：http://blog.hesvh.cn/Article/details/gzcbududj.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://3g.hesvh.cn/Article/details/glvzhbocz.sHtML

[Q05] 重命名列
来源：http://read.share.zdbjq.cn/Article/details/gfewchyde.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.blog.fehbvm.com/Article/details/ggjvojdtf.sHtML

[Q06] 删除列
来源：http://blog.fehbvm.com/Article/details/gsuubearu.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.share.hesvh.cn/Article/details/gymtrhqoi.sHtML

[Q07] 删除表
来源：http://baike.zdbjq.cn/Article/details/gyadpzcew.sHtML

DROP TABLE IF EXISTS orders;
来源：http://3g.fehbvm.com/Article/details/grxovmyog.sHtML

[Q08] 创建普通索引
来源：http://www.m.share.hesvh.cn/Article/details/gsitpcrir.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://mobile.zdbjq.cn/Article/details/gqgngstbu.sHtML

[Q09] 创建唯一索引
来源：http://mobile.hesvh.cn/Article/details/grlppjiuv.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://blog.fehbvm.com/Article/details/gfbufxyeq.sHtML

[Q10] 插入单行
来源：http://m.share.fehbvm.com/Article/details/garvjfydy.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://blog.hesvh.cn/Article/details/ggoalxnhe.sHtML

[Q11] 一次插入多行
来源：http://baike.zdbjq.cn/Article/details/gujlfisqp.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.m.share.hesvh.cn/Article/details/ghgrmxopu.sHtML

[Q12] 插入后取自增 ID
来源：http://read.share.fehbvm.com/Article/details/gamnrgpyv.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://wap.zdbjq.cn/Article/details/gngfnghst.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://mobile.zdbjq.cn/Article/details/glxzqbvjz.sHtML

[Q13] 忽略重复插入
来源：http://blog.zdbjq.cn/Article/details/gcqpwelyl.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.blog.fehbvm.com/Article/details/gnqunenyh.sHtML

[Q14] 存在则更新（upsert）
来源：http://3g.fehbvm.com/Article/details/gqgzpmwnu.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://read.share.fehbvm.com/Article/details/gdtgyxfxo.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.share.zdbjq.cn/Article/details/gfssdeori.sHtML

[Q15] 查询全部
来源：http://www.share.zdbjq.cn/Article/details/gdbslvbpi.sHtML

SELECT * FROM users;
来源：http://blog.fehbvm.com/Article/details/gzperyqym.sHtML

[Q16] 查询指定列
来源：http://read.share.zdbjq.cn/Article/details/gpvhamezy.sHtML

SELECT id, name FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gfhsxusgl.sHtML

[Q17] 条件查询
来源：http://3g.fehbvm.com/Article/details/gidfuqrvd.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://blog.hesvh.cn/Article/details/gbigaaxva.sHtML

[Q18] 模糊匹配
来源：http://m.share.zdbjq.cn/Article/details/gxhauohsl.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.blog.zdbjq.cn/Article/details/gwwxjxpzs.sHtML

[Q19] 范围查询
来源：http://www.m.share.zdbjq.cn/Article/details/gxtdlbonm.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://blog.fehbvm.com/Article/details/gbkrvpptg.sHtML

[Q20] IN 列表
来源：http://www.share.hesvh.cn/Article/details/gsfknpblq.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://read.share.zdbjq.cn/Article/details/geuddccwh.sHtML

[Q21] 空值判断
来源：http://baike.hesvh.cn/Article/details/gomsraxaa.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://baike.hesvh.cn/Article/details/gbnngzsub.sHtML

[Q22] 排序
来源：http://www.m.share.zdbjq.cn/Article/details/gwukgqend.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://m.share.fehbvm.com/Article/details/gznzldbjp.sHtML

[Q23] 分页
来源：http://baike.hesvh.cn/Article/details/ggtvcigbu.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://read.share.hesvh.cn/Article/details/ghotvywrs.sHtML

[Q24] 去重
来源：http://3g.hesvh.cn/Article/details/gsnogsjim.sHtML

SELECT DISTINCT city FROM users;
来源：http://read.share.fehbvm.com/Article/details/gtpykcqrz.sHtML

[Q25] 只取前 N 条
来源：http://www.m.share.fehbvm.com/Article/details/goigskqzs.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://m.share.zdbjq.cn/Article/details/gmiteozbg.sHtML

[Q26] 计数
来源：http://www.blog.hesvh.cn/Article/details/gdpthqxcr.sHtML

SELECT COUNT(*) FROM users;
来源：http://blog.fehbvm.com/Article/details/gmbvdqdsi.sHtML

[Q27] 条件计数
来源：http://www.share.zdbjq.cn/Article/details/govjkrmcx.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://m.share.fehbvm.com/Article/details/garvmhymr.sHtML

[Q28] 求和与平均
来源：http://3g.fehbvm.com/Article/details/gplrtdvzq.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://m.share.hesvh.cn/Article/details/gjkdcsufn.sHtML

[Q29] 最大最小值
来源：http://www.m.share.fehbvm.com/Article/details/gddchycma.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://read.share.hesvh.cn/Article/details/gkauzyshu.sHtML

[Q30] 分组统计
来源：http://blog.hesvh.cn/Article/details/gukunfoqh.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.share.zdbjq.cn/Article/details/gxidiydwy.sHtML

[Q31] 分组后过滤
来源：http://www.m.share.fehbvm.com/Article/details/gvmefqbfj.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.m.share.hesvh.cn/Article/details/gpypweetv.sHtML

[Q32] 分组拼接字符串
来源：http://www.share.hesvh.cn/Article/details/gxcevnysg.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.m.share.hesvh.cn/Article/details/gfpdqpcoi.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://read.share.zdbjq.cn/Article/details/gznyjlisb.sHtML

[Q33] 多列分组
来源：http://blog.fehbvm.com/Article/details/gcxcrqmjy.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://m.share.zdbjq.cn/Article/details/gzwxrpkgu.sHtML

[Q34] 每组取第一条
来源：http://www.blog.fehbvm.com/Article/details/gitbmyago.sHtML

SELECT * FROM (
来源：http://blog.hesvh.cn/Article/details/gzzzqetaa.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://blog.fehbvm.com/Article/details/gkhipvskw.sHtML

) t WHERE rn = 1;
来源：http://www.m.share.fehbvm.com/Article/details/glpirulbv.sHtML

[Q35] 内连接
来源：http://blog.hesvh.cn/Article/details/ggdgjdmwu.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://baike.fehbvm.com/Article/details/gfofqadeu.sHtML

[Q36] 左连接
来源：http://3g.hesvh.cn/Article/details/guhhvayhm.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.share.fehbvm.com/Article/details/glqxetjpp.sHtML

[Q37] 右连接
来源：http://blog.zdbjq.cn/Article/details/ghedlvnsr.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://3g.fehbvm.com/Article/details/gfjonxxfe.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://baike.hesvh.cn/Article/details/gzvmgfpni.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://blog.zdbjq.cn/Article/details/gfrsfynpi.sHtML

[Q39] 自连接（查上下级）
来源：http://wap.hesvh.cn/Article/details/gswqjkxoh.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://3g.fehbvm.com/Article/details/gfcpgmbcr.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://wap.hesvh.cn/Article/details/gryndlcuy.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://read.share.hesvh.cn/Article/details/gbfgpzypv.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://mobile.zdbjq.cn/Article/details/ggxpvfphi.sHtML

[Q41] 多表连接
来源：http://blog.hesvh.cn/Article/details/gijpugrxv.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://m.share.zdbjq.cn/Article/details/gtufwqnzo.sHtML

JOIN users u ON u.id = o.user_id
来源：http://read.share.fehbvm.com/Article/details/gyvqkfgrq.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://read.share.fehbvm.com/Article/details/gxjhsqafp.sHtML

[Q42] 连接条件附加过滤
来源：http://3g.fehbvm.com/Article/details/gerefyyik.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.share.fehbvm.com/Article/details/gvrsonzep.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.share.hesvh.cn/Article/details/glfgnrffl.sHtML

[Q43] 标量子查询
来源：http://blog.hesvh.cn/Article/details/gusspdxks.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://3g.fehbvm.com/Article/details/gsmvedtxa.sHtML

[Q44] IN 子查询
来源：http://3g.zdbjq.cn/Article/details/gxrfbphjt.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.share.fehbvm.com/Article/details/gwebluqxf.sHtML

[Q45] EXISTS 判断存在
来源：http://www.blog.fehbvm.com/Article/details/gluozdvuq.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.fehbvm.com/Article/details/gwtuknert.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://mobile.fehbvm.com/Article/details/gfibnjtyh.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.hesvh.cn/Article/details/giwyckcyp.sHtML

[Q47] 与平均值比较
来源：http://3g.zdbjq.cn/Article/details/ggnznwanr.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://baike.zdbjq.cn/Article/details/gmflvzscv.sHtML

[Q48] CTE 公用表表达式
来源：http://mobile.fehbvm.com/Article/details/gzzmeibob.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://mobile.zdbjq.cn/Article/details/gldykszti.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://mobile.hesvh.cn/Article/details/gbvzdyofb.sHtML

[Q49] 更新单行
来源：http://www.share.fehbvm.com/Article/details/gqzxbbwlk.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.m.share.zdbjq.cn/Article/details/gmbmmhtvh.sHtML

[Q50] 批量更新
来源：http://www.blog.zdbjq.cn/Article/details/gdnwficnx.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://read.share.zdbjq.cn/Article/details/ghlvnaiug.sHtML

[Q51] 用子查询更新
来源：http://3g.fehbvm.com/Article/details/gikzlxsab.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://read.share.fehbvm.com/Article/details/gfyzpzeza.sHtML

[Q52] 删除指定行
来源：http://3g.zdbjq.cn/Article/details/gnocbkeml.sHtML

DELETE FROM users WHERE id = 10;
来源：http://3g.fehbvm.com/Article/details/gpxugabzr.sHtML

[Q53] 按条件删除
来源：http://blog.zdbjq.cn/Article/details/gmfwdpjow.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://blog.zdbjq.cn/Article/details/gyphcppls.sHtML

[Q54] 清空表
来源：http://www.blog.hesvh.cn/Article/details/grjtigcda.sHtML

TRUNCATE TABLE logs;
来源：http://mobile.hesvh.cn/Article/details/gibgqcadx.sHtML

[Q55] 排名（并列占位）
来源：http://baike.hesvh.cn/Article/details/gqxrgvjph.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://m.share.hesvh.cn/Article/details/grtfulesg.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.blog.fehbvm.com/Article/details/gzzefdfix.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://m.share.hesvh.cn/Article/details/gefyemttl.sHtML

[Q57] 行号
来源：http://blog.hesvh.cn/Article/details/glkxbzfqg.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.share.zdbjq.cn/Article/details/ghwnjhkgn.sHtML

[Q58] 累计求和
来源：http://wap.fehbvm.com/Article/details/gsicvahmh.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.m.share.hesvh.cn/Article/details/gerctgshd.sHtML

[Q59] 分组内累计
来源：http://baike.hesvh.cn/Article/details/gconpoepz.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://3g.zdbjq.cn/Article/details/gzlerbbol.sHtML

[Q60] 取上一行 / 下一行
来源：http://blog.fehbvm.com/Article/details/gsfwxrqak.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.blog.hesvh.cn/Article/details/gdcaihqcb.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://blog.fehbvm.com/Article/details/gonanchub.sHtML

[Q61] 移动平均
来源：http://mobile.fehbvm.com/Article/details/grpfbrbqj.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.m.share.fehbvm.com/Article/details/gefbkanvn.sHtML

[Q62] 分组占比
来源：http://wap.fehbvm.com/Article/details/gidudtonr.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://baike.fehbvm.com/Article/details/gjqnulefm.sHtML

[Q63] 开启事务
来源：http://wap.zdbjq.cn/Article/details/geoenfgja.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://3g.fehbvm.com/Article/details/geekaijar.sHtML

[Q64] 提交事务
来源：http://3g.fehbvm.com/Article/details/gymvbcrun.sHtML

COMMIT;
来源：http://read.share.zdbjq.cn/Article/details/geenlqpcv.sHtML

[Q65] 回滚事务
来源：http://mobile.hesvh.cn/Article/details/gmeqmilke.sHtML

ROLLBACK;
来源：http://www.m.share.hesvh.cn/Article/details/gcykpxrww.sHtML

[Q66] 行锁查询
来源：http://3g.hesvh.cn/Article/details/gkwowhopy.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.blog.fehbvm.com/Article/details/gpxbjjsck.sHtML

[Q67] 设置隔离级别
来源：http://read.share.hesvh.cn/Article/details/gqfscrycr.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://baike.fehbvm.com/Article/details/gbdmyfvpq.sHtML

[Q68] 保存点
来源：http://read.share.hesvh.cn/Article/details/gkjewjgsn.sHtML

SAVEPOINT sp1;
来源：http://wap.zdbjq.cn/Article/details/gnuokleko.sHtML

ROLLBACK TO sp1;
来源：http://wap.fehbvm.com/Article/details/gxczayfez.sHtML

[Q69] 查看执行计划
来源：http://m.share.fehbvm.com/Article/details/gaztzhrim.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://baike.zdbjq.cn/Article/details/gbrutiali.sHtML

[Q70] 更新统计信息
来源：http://www.blog.zdbjq.cn/Article/details/ghmexgluo.sHtML

ANALYZE TABLE users;
来源：http://www.blog.zdbjq.cn/Article/details/gpcrvknwy.sHtML

[Q71] 查看建表语句
来源：http://www.m.share.zdbjq.cn/Article/details/gifwjywde.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://mobile.fehbvm.com/Article/details/gljranmjt.sHtML

[Q72] 查看索引
来源：http://m.share.fehbvm.com/Article/details/gdbhiufpx.sHtML

SHOW INDEX FROM users;
来源：http://read.share.hesvh.cn/Article/details/gagcezssw.sHtML

[Q73] 查看表状态
来源：http://m.share.hesvh.cn/Article/details/grvmjpxjn.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://mobile.hesvh.cn/Article/details/gpnxzlnwa.sHtML

[Q74] 强制使用索引
来源：http://m.share.fehbvm.com/Article/details/grdjwivue.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://3g.zdbjq.cn/Article/details/ggutshknr.sHtML

[Q75] 日期格式化
来源：http://www.blog.hesvh.cn/Article/details/gdxnbpzfe.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://blog.zdbjq.cn/Article/details/gdgloqgyq.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://read.share.hesvh.cn/Article/details/gdqwgrdyh.sHtML

[Q76] 按天统计
来源：http://www.blog.zdbjq.cn/Article/details/gjdnkcepv.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://read.share.hesvh.cn/Article/details/gbovikcrj.sHtML

[Q77] 时间加减
来源：http://m.share.zdbjq.cn/Article/details/gyxsbiuze.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.blog.zdbjq.cn/Article/details/gpinoafuz.sHtML

[Q78] 当前时间
来源：http://mobile.zdbjq.cn/Article/details/gzqhhcjlj.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://mobile.hesvh.cn/Article/details/gwszmvcvk.sHtML

[Q79] 字符串拼接
来源：http://www.m.share.fehbvm.com/Article/details/gdomoouux.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.blog.fehbvm.com/Article/details/gfzevtkaz.sHtML

[Q80] 字符串截取
来源：http://www.m.share.hesvh.cn/Article/details/gbozexsls.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://read.share.zdbjq.cn/Article/details/groyfpxqy.sHtML

[Q81] 字符串替换
来源：http://www.m.share.fehbvm.com/Article/details/gnhwpqprd.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://wap.fehbvm.com/Article/details/gxnshrurs.sHtML

[Q82] 字符长度与字节长度
来源：http://mobile.fehbvm.com/Article/details/gpnzjbcim.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://3g.zdbjq.cn/Article/details/gxqnoweof.sHtML

[Q83] 大小写转换
来源：http://mobile.zdbjq.cn/Article/details/gvirdswdl.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://baike.zdbjq.cn/Article/details/gjlttxuuw.sHtML

[Q84] 去除首尾空格
来源：http://mobile.hesvh.cn/Article/details/gdrvlgfpu.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.share.zdbjq.cn/Article/details/guvanulqi.sHtML

[Q85] 数值取整
来源：http://read.share.hesvh.cn/Article/details/ggxzygjww.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://read.share.zdbjq.cn/Article/details/gxmczrilf.sHtML

[Q86] 读取 JSON 字段
来源：http://read.share.zdbjq.cn/Article/details/gtrfsycxe.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.share.zdbjq.cn/Article/details/gtitofoga.sHtML

[Q87] JSON 字段做条件
来源：http://mobile.fehbvm.com/Article/details/gxsacshtf.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://blog.zdbjq.cn/Article/details/gsdszzjen.sHtML

[Q88] 行转列（条件聚合）
来源：http://baike.zdbjq.cn/Article/details/gokwwgqzq.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://baike.zdbjq.cn/Article/details/gmmuhoary.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gfzhiedst.sHtML

[Q89] 判断表是否存在
来源：http://wap.hesvh.cn/Article/details/gmnrspjjd.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://blog.zdbjq.cn/Article/details/glxngqkfs.sHtML

[Q90] 生成序号列
来源：http://m.share.zdbjq.cn/Article/details/gayxslhxr.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://baike.hesvh.cn/Article/details/gggfflmdt.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gcshnsdta.sHtML

R. Bash 专题
来源：http://www.m.share.fehbvm.com/Article/details/ghcfbjnsm.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gukprxvpz.sHtML

[R01] shebang 与严格模式
来源：http://m.share.fehbvm.com/Article/details/ggqgsfdki.sHtML

#!/usr/bin/env bash
来源：http://mobile.fehbvm.com/Article/details/gtjscugpe.sHtML

set -euo pipefail
来源：http://baike.fehbvm.com/Article/details/gypkoibtu.sHtML

[R02] 变量赋值与使用
来源：http://www.blog.hesvh.cn/Article/details/gvzovcmly.sHtML

name="Tom"; echo "$name"
来源：http://wap.zdbjq.cn/Article/details/geiggbipc.sHtML

[R03] 只读变量
来源：http://www.share.fehbvm.com/Article/details/gttwymdby.sHtML

readonly PI=3.14
来源：http://www.share.fehbvm.com/Article/details/gwfcyrbqs.sHtML

[R04] 位置参数
来源：http://3g.hesvh.cn/Article/details/gwhhjkorp.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://mobile.zdbjq.cn/Article/details/gtubnihvd.sHtML

[R05] 参数默认值
来源：http://baike.hesvh.cn/Article/details/gnufirdui.sHtML

name="${1:-default}"
来源：http://read.share.fehbvm.com/Article/details/gngcmwybf.sHtML

[R06] 判断命令是否存在
来源：http://wap.hesvh.cn/Article/details/gmfznlvjb.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://read.share.hesvh.cn/Article/details/gbutkwzbl.sHtML

[R07] if 判断文件
来源：http://www.share.hesvh.cn/Article/details/gghpwyurj.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://m.share.fehbvm.com/Article/details/gjqawefmp.sHtML

[R08] 数值比较
来源：http://www.share.hesvh.cn/Article/details/grubdybmm.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://mobile.fehbvm.com/Article/details/guzahmupz.sHtML

[R09] 字符串比较
来源：http://www.blog.hesvh.cn/Article/details/grrzrviig.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://mobile.fehbvm.com/Article/details/gwitdyxrk.sHtML

[R10] 正则匹配
来源：http://mobile.zdbjq.cn/Article/details/gvtaahgah.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://baike.hesvh.cn/Article/details/gyxwohvxu.sHtML

[R11] case 多分支
来源：http://m.share.zdbjq.cn/Article/details/gjpvvgdpk.sHtML

case "$1" in
来源：http://mobile.fehbvm.com/Article/details/goxqrinby.sHtML

start) echo "启动" ;;
来源：http://blog.zdbjq.cn/Article/details/gckpbuctz.sHtML

stop)  echo "停止" ;;
来源：http://www.share.fehbvm.com/Article/details/glylisivz.sHtML

*)     echo "未知命令" ;;
来源：http://wap.fehbvm.com/Article/details/gonmldbfv.sHtML

esac
来源：http://blog.zdbjq.cn/Article/details/gqwywtcpc.sHtML

[R12] for 遍历文件
来源：http://m.share.zdbjq.cn/Article/details/gvgloqwve.sHtML

for f in *.txt; do echo "$f"; done
来源：http://baike.hesvh.cn/Article/details/gkqwojbmb.sHtML

[R13] for 计数循环
来源：http://read.share.zdbjq.cn/Article/details/glpdoxyoi.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://3g.fehbvm.com/Article/details/gokegfvro.sHtML

[R14] C 风格 for
来源：http://read.share.fehbvm.com/Article/details/gbetbnrsn.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.blog.zdbjq.cn/Article/details/golfkdqay.sHtML

[R15] while 逐行读文件
来源：http://read.share.fehbvm.com/Article/details/gbftbqmpo.sHtML


<!-- 参考信息 -->