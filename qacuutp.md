代发 wailian999

TS:   crypto.randomUUID()
来源：http://baike.hesvh.cn/Article/details/gwkdlfrxp.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.blog.fehbvm.com/Article/details/gbkjsmnmu.sHtML

Go:   // 用 github.com/google/uuid
来源：http://read.share.hesvh.cn/Article/details/gmhbrqsok.sHtML

Ruby: SecureRandom.uuid
来源：http://m.share.hesvh.cn/Article/details/gocvlxcki.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.share.zdbjq.cn/Article/details/gsjdyaihc.sHtML

[P02] MD5 / SHA256 摘要
来源：http://wap.hesvh.cn/Article/details/gbywklrxs.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://m.share.hesvh.cn/Article/details/gvgfvsaku.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://3g.fehbvm.com/Article/details/gdmgwrugx.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://baike.fehbvm.com/Article/details/gkvqkvqwd.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://mobile.fehbvm.com/Article/details/gmuspsquk.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://blog.fehbvm.com/Article/details/gnlgukgmb.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.share.fehbvm.com/Article/details/gyrnzaiko.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://blog.fehbvm.com/Article/details/gwfafqogd.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.share.zdbjq.cn/Article/details/gbqkniwyc.sHtML

[P03] 生成短随机字符串
来源：http://m.share.hesvh.cn/Article/details/gfegckgpk.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://wap.hesvh.cn/Article/details/gtiplhfbe.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://3g.hesvh.cn/Article/details/gzghfvrjx.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.zdbjq.cn/Article/details/gdzhqzvxv.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.fehbvm.com/Article/details/gpzkakayj.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://baike.fehbvm.com/Article/details/gvtskxorq.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://blog.fehbvm.com/Article/details/gtmfjatne.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://baike.zdbjq.cn/Article/details/ggwdxlyoc.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.share.hesvh.cn/Article/details/gqknudzof.sHtML

[P04] 求长度
来源：http://3g.zdbjq.cn/Article/details/gbhntxhks.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://blog.fehbvm.com/Article/details/gvqbdinqt.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.hesvh.cn/Article/details/gtrsvhkkm.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.fehbvm.com/Article/details/gghinlwkz.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.hesvh.cn/Article/details/gdgrcpzcu.sHtML

Java: list.size();  map.size();  s.length()
来源：http://3g.zdbjq.cn/Article/details/gdiqrggcr.sHtML

Go:   len(arr);  len(m)
来源：http://wap.zdbjq.cn/Article/details/gkbbgrtrq.sHtML

Ruby: x.length;  x.size
来源：http://m.share.fehbvm.com/Article/details/gupflprkg.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://mobile.hesvh.cn/Article/details/grwqjrzbp.sHtML

[P05] 判断两个对象内容是否相等
来源：http://m.share.fehbvm.com/Article/details/gbxcrbwdn.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://3g.fehbvm.com/Article/details/gefvpuhnk.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://read.share.fehbvm.com/Article/details/gykkirmic.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://3g.fehbvm.com/Article/details/gqjjhwduq.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://wap.fehbvm.com/Article/details/gfaoesogn.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://baike.hesvh.cn/Article/details/gfobutnev.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://mobile.fehbvm.com/Article/details/gylcmiauz.sHtML

Ruby: a == b
来源：http://baike.fehbvm.com/Article/details/ggrlmnwyx.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://3g.fehbvm.com/Article/details/gauqpgmka.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.blog.hesvh.cn/Article/details/gxiceicwx.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.m.share.hesvh.cn/Article/details/gwpycozzk.sHtML

PHP:  if (empty($x)) {}
来源：http://mobile.fehbvm.com/Article/details/glcpfdejs.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://baike.fehbvm.com/Article/details/gcdyuekxg.sHtML

TS:   if (x == null) {}
来源：http://3g.zdbjq.cn/Article/details/gtnmlopnx.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://wap.hesvh.cn/Article/details/gkksiowze.sHtML

Go:   if x == nil {}
来源：http://3g.hesvh.cn/Article/details/gspmpmrgn.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.share.fehbvm.com/Article/details/gqvynkfya.sHtML

C#:   if (x is null) {}
来源：http://read.share.zdbjq.cn/Article/details/gewqmblha.sHtML

[P07] 防抖与节流
来源：http://wap.hesvh.cn/Article/details/ghuyplnjk.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.m.share.fehbvm.com/Article/details/gxfnukyan.sHtML

PHP:  // 手写时间戳比较
来源：http://m.share.fehbvm.com/Article/details/grrgvegos.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.hesvh.cn/Article/details/gbfsbznzm.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.fehbvm.com/Article/details/gqpsilrrp.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.blog.zdbjq.cn/Article/details/gmvflysfs.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://mobile.zdbjq.cn/Article/details/gnvgehylc.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://blog.zdbjq.cn/Article/details/gevyeodxr.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://3g.zdbjq.cn/Article/details/gxeerbvse.sHtML

[P08] 处理浮点精度问题
来源：http://www.m.share.fehbvm.com/Article/details/gavnlsmkq.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://read.share.hesvh.cn/Article/details/glezcmdbk.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://read.share.fehbvm.com/Article/details/gfzzgajmk.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.m.share.fehbvm.com/Article/details/gthsbwblh.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://read.share.hesvh.cn/Article/details/gqfwcnpon.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.share.fehbvm.com/Article/details/gnphlogfa.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://blog.zdbjq.cn/Article/details/giohhcwxh.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.m.share.hesvh.cn/Article/details/glcsyfwap.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://3g.zdbjq.cn/Article/details/gpeembzjq.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gwhwtujum.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://read.share.zdbjq.cn/Article/details/gwfbppwqx.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gthsgakih.sHtML

[Q01] 创建表
来源：http://blog.zdbjq.cn/Article/details/gvtncochm.sHtML

CREATE TABLE users (
来源：http://read.share.fehbvm.com/Article/details/grsgmhkvy.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.fehbvm.com/Article/details/gjndzdimg.sHtML

name VARCHAR(50) NOT NULL,
来源：http://mobile.hesvh.cn/Article/details/ghlvsotup.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.blog.fehbvm.com/Article/details/gjlqnlbth.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://read.share.zdbjq.cn/Article/details/gojpwclop.sHtML

);
来源：http://m.share.fehbvm.com/Article/details/gwyeaongw.sHtML

[Q02] 创建带外键的表
来源：http://3g.zdbjq.cn/Article/details/goxbonkbw.sHtML

CREATE TABLE orders (
来源：http://www.m.share.fehbvm.com/Article/details/gaawwluxf.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://mobile.fehbvm.com/Article/details/gqbzqcfaw.sHtML

user_id INT NOT NULL,
来源：http://www.m.share.fehbvm.com/Article/details/gmgxiwsnn.sHtML

amount DECIMAL(10, 2),
来源：http://mobile.hesvh.cn/Article/details/gyalsbuiv.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.share.fehbvm.com/Article/details/gfdwzbikt.sHtML

);
来源：http://mobile.hesvh.cn/Article/details/gfmewnude.sHtML

[Q03] 增加列
来源：http://mobile.fehbvm.com/Article/details/gvpsdvqrx.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://blog.hesvh.cn/Article/details/gqhbbwgnf.sHtML

[Q04] 修改列类型
来源：http://wap.hesvh.cn/Article/details/gxxjgfaml.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://wap.fehbvm.com/Article/details/gvvcjjrat.sHtML

[Q05] 重命名列
来源：http://mobile.fehbvm.com/Article/details/grsqufmpr.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://read.share.fehbvm.com/Article/details/glvdsrxex.sHtML

[Q06] 删除列
来源：http://baike.hesvh.cn/Article/details/gxxunagil.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://blog.fehbvm.com/Article/details/gltjcahxu.sHtML

[Q07] 删除表
来源：http://baike.fehbvm.com/Article/details/gqntdhojz.sHtML

DROP TABLE IF EXISTS orders;
来源：http://3g.zdbjq.cn/Article/details/ggxsrlyqt.sHtML

[Q08] 创建普通索引
来源：http://baike.hesvh.cn/Article/details/gkdsncsnx.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://blog.hesvh.cn/Article/details/gzlxbdtht.sHtML

[Q09] 创建唯一索引
来源：http://3g.zdbjq.cn/Article/details/gsuztggyi.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://m.share.hesvh.cn/Article/details/gjbeliadq.sHtML

[Q10] 插入单行
来源：http://mobile.hesvh.cn/Article/details/gmnefhucl.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.share.zdbjq.cn/Article/details/gnlzzwkch.sHtML

[Q11] 一次插入多行
来源：http://www.blog.hesvh.cn/Article/details/gdgbxrkhm.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://mobile.hesvh.cn/Article/details/ghuetvevx.sHtML

[Q12] 插入后取自增 ID
来源：http://blog.fehbvm.com/Article/details/gwzwxymfr.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://wap.fehbvm.com/Article/details/gvcmrbyap.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.share.hesvh.cn/Article/details/gyaqfcejb.sHtML

[Q13] 忽略重复插入
来源：http://www.blog.fehbvm.com/Article/details/gvnieyybq.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://baike.zdbjq.cn/Article/details/gmevumcif.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.share.fehbvm.com/Article/details/gcmbwthll.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://3g.hesvh.cn/Article/details/goldsegnf.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://m.share.hesvh.cn/Article/details/gpgdgzauq.sHtML

[Q15] 查询全部
来源：http://www.blog.hesvh.cn/Article/details/gcrlhvvjl.sHtML

SELECT * FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gomcuugrq.sHtML

[Q16] 查询指定列
来源：http://m.share.hesvh.cn/Article/details/gqsgkstoo.sHtML

SELECT id, name FROM users;
来源：http://3g.zdbjq.cn/Article/details/glzwfhrdb.sHtML

[Q17] 条件查询
来源：http://baike.fehbvm.com/Article/details/gjbnqmlox.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://baike.hesvh.cn/Article/details/gngkzbeoj.sHtML

[Q18] 模糊匹配
来源：http://mobile.zdbjq.cn/Article/details/gckymcnho.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://m.share.zdbjq.cn/Article/details/gnqzhfihk.sHtML

[Q19] 范围查询
来源：http://www.share.hesvh.cn/Article/details/gmfmsjsqf.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://3g.zdbjq.cn/Article/details/gcbontqqq.sHtML

[Q20] IN 列表
来源：http://www.m.share.zdbjq.cn/Article/details/goobkqxpj.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://3g.zdbjq.cn/Article/details/giqlqwgzm.sHtML

[Q21] 空值判断
来源：http://read.share.fehbvm.com/Article/details/gggrhcebg.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://baike.hesvh.cn/Article/details/giocckdik.sHtML

[Q22] 排序
来源：http://read.share.fehbvm.com/Article/details/gecqbbolg.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://3g.fehbvm.com/Article/details/gjlzmrmcs.sHtML

[Q23] 分页
来源：http://wap.hesvh.cn/Article/details/gkmfymvmg.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.blog.hesvh.cn/Article/details/gauqwbrxo.sHtML

[Q24] 去重
来源：http://wap.zdbjq.cn/Article/details/gevbidnwn.sHtML

SELECT DISTINCT city FROM users;
来源：http://wap.hesvh.cn/Article/details/gsgwonzgq.sHtML

[Q25] 只取前 N 条
来源：http://blog.fehbvm.com/Article/details/gzxcyazxs.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://wap.hesvh.cn/Article/details/gfbudxojk.sHtML

[Q26] 计数
来源：http://m.share.hesvh.cn/Article/details/gopcflbly.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gzmuqqyfi.sHtML

[Q27] 条件计数
来源：http://baike.fehbvm.com/Article/details/grahkqwyk.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gvdgnktdj.sHtML

[Q28] 求和与平均
来源：http://wap.zdbjq.cn/Article/details/gtgfvoars.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.m.share.zdbjq.cn/Article/details/galscirbb.sHtML

[Q29] 最大最小值
来源：http://www.blog.fehbvm.com/Article/details/griajaihf.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://blog.zdbjq.cn/Article/details/grrakyliy.sHtML

[Q30] 分组统计
来源：http://3g.fehbvm.com/Article/details/gllavyeqq.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://read.share.fehbvm.com/Article/details/ghjzsqwps.sHtML

[Q31] 分组后过滤
来源：http://www.m.share.fehbvm.com/Article/details/gqfwipvhy.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://mobile.hesvh.cn/Article/details/gzwczpnme.sHtML

[Q32] 分组拼接字符串
来源：http://3g.zdbjq.cn/Article/details/gxzpilumo.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://wap.fehbvm.com/Article/details/gvnfgdkww.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://blog.fehbvm.com/Article/details/gjxnijjeu.sHtML

[Q33] 多列分组
来源：http://blog.zdbjq.cn/Article/details/gzteqaqzd.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.share.fehbvm.com/Article/details/gjspaxabn.sHtML

[Q34] 每组取第一条
来源：http://wap.fehbvm.com/Article/details/gsyovcpxo.sHtML

SELECT * FROM (
来源：http://wap.fehbvm.com/Article/details/grrjnygny.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://mobile.fehbvm.com/Article/details/gfpfcidbz.sHtML

) t WHERE rn = 1;
来源：http://blog.hesvh.cn/Article/details/ghyyrqiaq.sHtML

[Q35] 内连接
来源：http://m.share.fehbvm.com/Article/details/gslesvfpg.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.fehbvm.com/Article/details/griacvypr.sHtML

[Q36] 左连接
来源：http://3g.zdbjq.cn/Article/details/gvlyipsqb.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://baike.zdbjq.cn/Article/details/gnyftmrop.sHtML

[Q37] 右连接
来源：http://wap.hesvh.cn/Article/details/gydjtyckv.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.share.hesvh.cn/Article/details/gmonfcdii.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://blog.zdbjq.cn/Article/details/gqznrgewe.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.m.share.hesvh.cn/Article/details/gzpycauro.sHtML

[Q39] 自连接（查上下级）
来源：http://read.share.fehbvm.com/Article/details/gfjayuwio.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://blog.fehbvm.com/Article/details/gjyoppklr.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.share.fehbvm.com/Article/details/gmfwjoveu.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://mobile.hesvh.cn/Article/details/gnkidyoxo.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://mobile.fehbvm.com/Article/details/goqamjcwl.sHtML

[Q41] 多表连接
来源：http://www.m.share.hesvh.cn/Article/details/gymdeylfb.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://mobile.hesvh.cn/Article/details/gvvhukmyp.sHtML

JOIN users u ON u.id = o.user_id
来源：http://baike.fehbvm.com/Article/details/gsqgkggfg.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://m.share.hesvh.cn/Article/details/golwcsweh.sHtML

[Q42] 连接条件附加过滤
来源：http://www.share.zdbjq.cn/Article/details/gwmdzshcv.sHtML

SELECT u.name, o.amount FROM users u
来源：http://wap.hesvh.cn/Article/details/ghqunmoam.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://blog.hesvh.cn/Article/details/gebsxijvd.sHtML

[Q43] 标量子查询
来源：http://3g.hesvh.cn/Article/details/ghxyehtia.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://m.share.hesvh.cn/Article/details/gnvlawseu.sHtML

[Q44] IN 子查询
来源：http://www.m.share.hesvh.cn/Article/details/gvfrkxlfd.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://3g.hesvh.cn/Article/details/gijdrswyj.sHtML

[Q45] EXISTS 判断存在
来源：http://www.share.hesvh.cn/Article/details/glkvzfpum.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.fehbvm.com/Article/details/gqhjattkl.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.share.fehbvm.com/Article/details/glekxroup.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.fehbvm.com/Article/details/gwquvatll.sHtML

[Q47] 与平均值比较
来源：http://baike.fehbvm.com/Article/details/gtuckhgeh.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://blog.zdbjq.cn/Article/details/gtacxfnok.sHtML

[Q48] CTE 公用表表达式
来源：http://www.share.fehbvm.com/Article/details/gnrprgutc.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.m.share.zdbjq.cn/Article/details/gufaeknux.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://wap.zdbjq.cn/Article/details/gvanbboeh.sHtML

[Q49] 更新单行
来源：http://3g.fehbvm.com/Article/details/gnnvjurds.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.m.share.hesvh.cn/Article/details/gypsqwvoi.sHtML

[Q50] 批量更新
来源：http://3g.zdbjq.cn/Article/details/gwlkhyncq.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://blog.hesvh.cn/Article/details/gajvpzutn.sHtML

[Q51] 用子查询更新
来源：http://www.share.hesvh.cn/Article/details/glkeryoig.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.m.share.fehbvm.com/Article/details/gtavcvmun.sHtML

[Q52] 删除指定行
来源：http://www.m.share.fehbvm.com/Article/details/gmhusjhxm.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.blog.fehbvm.com/Article/details/gimeeigyq.sHtML

[Q53] 按条件删除
来源：http://m.share.hesvh.cn/Article/details/gwohlibzr.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.share.zdbjq.cn/Article/details/glyxngulx.sHtML

[Q54] 清空表
来源：http://m.share.zdbjq.cn/Article/details/gingvhaco.sHtML

TRUNCATE TABLE logs;
来源：http://mobile.zdbjq.cn/Article/details/gsqegrqjh.sHtML

[Q55] 排名（并列占位）
来源：http://wap.zdbjq.cn/Article/details/giicpvleu.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://mobile.hesvh.cn/Article/details/gqzgvttnt.sHtML

[Q56] 密集排名（并列不占位）
来源：http://m.share.fehbvm.com/Article/details/gdkzcpawe.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://mobile.hesvh.cn/Article/details/gcdxlimle.sHtML

[Q57] 行号
来源：http://wap.hesvh.cn/Article/details/ghuqerylp.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://blog.hesvh.cn/Article/details/grykzbbrt.sHtML

[Q58] 累计求和
来源：http://3g.hesvh.cn/Article/details/guvmtqvox.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://baike.fehbvm.com/Article/details/glnvbzxsb.sHtML

[Q59] 分组内累计
来源：http://mobile.fehbvm.com/Article/details/gaculnkwr.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.share.hesvh.cn/Article/details/gklmholyi.sHtML

[Q60] 取上一行 / 下一行
来源：http://baike.zdbjq.cn/Article/details/gdxvtdfyr.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.m.share.fehbvm.com/Article/details/gsbenamyr.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://mobile.zdbjq.cn/Article/details/gnojhqdmg.sHtML

[Q61] 移动平均
来源：http://www.share.fehbvm.com/Article/details/gdmdmdsjn.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://3g.hesvh.cn/Article/details/gaoqlmccf.sHtML

[Q62] 分组占比
来源：http://baike.hesvh.cn/Article/details/ggrgkobko.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://wap.zdbjq.cn/Article/details/gnafwkhnd.sHtML

[Q63] 开启事务
来源：http://read.share.zdbjq.cn/Article/details/gssztvump.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://3g.hesvh.cn/Article/details/gnymvovqq.sHtML

[Q64] 提交事务
来源：http://wap.zdbjq.cn/Article/details/gulwbevwj.sHtML

COMMIT;
来源：http://www.share.fehbvm.com/Article/details/gcizuhajs.sHtML

[Q65] 回滚事务
来源：http://read.share.zdbjq.cn/Article/details/gmyxgybzg.sHtML

ROLLBACK;
来源：http://wap.zdbjq.cn/Article/details/ggpwpdrij.sHtML

[Q66] 行锁查询
来源：http://www.share.zdbjq.cn/Article/details/gzszpmvkm.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.share.zdbjq.cn/Article/details/gwnygdbfq.sHtML

[Q67] 设置隔离级别
来源：http://3g.fehbvm.com/Article/details/gxwbanpda.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://m.share.fehbvm.com/Article/details/gyykvltxe.sHtML

[Q68] 保存点
来源：http://baike.zdbjq.cn/Article/details/gjghldpon.sHtML

SAVEPOINT sp1;
来源：http://www.share.hesvh.cn/Article/details/gzhnqpqlx.sHtML

ROLLBACK TO sp1;
来源：http://www.blog.zdbjq.cn/Article/details/gfybocryk.sHtML

[Q69] 查看执行计划
来源：http://m.share.hesvh.cn/Article/details/glqhbnhpl.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://mobile.hesvh.cn/Article/details/gthfsarlp.sHtML

[Q70] 更新统计信息
来源：http://www.m.share.hesvh.cn/Article/details/gkdvyxhyy.sHtML

ANALYZE TABLE users;
来源：http://www.m.share.fehbvm.com/Article/details/gxbaloonr.sHtML

[Q71] 查看建表语句
来源：http://baike.fehbvm.com/Article/details/gtnorhjkv.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.blog.zdbjq.cn/Article/details/gppntsdiq.sHtML

[Q72] 查看索引
来源：http://www.blog.fehbvm.com/Article/details/ggdyqxbwu.sHtML

SHOW INDEX FROM users;
来源：http://www.share.fehbvm.com/Article/details/gpcbwmrrh.sHtML

[Q73] 查看表状态
来源：http://www.blog.fehbvm.com/Article/details/gngvjnsmj.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.share.hesvh.cn/Article/details/gmtlrydvw.sHtML

[Q74] 强制使用索引
来源：http://www.blog.hesvh.cn/Article/details/gxxlolqcf.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://baike.zdbjq.cn/Article/details/gktdxpgff.sHtML

[Q75] 日期格式化
来源：http://m.share.hesvh.cn/Article/details/gygblbkfz.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://mobile.zdbjq.cn/Article/details/gavykwjsb.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.m.share.hesvh.cn/Article/details/guvlypben.sHtML

[Q76] 按天统计
来源：http://www.blog.zdbjq.cn/Article/details/guxjtfqhu.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://3g.hesvh.cn/Article/details/gcqefrxlm.sHtML

[Q77] 时间加减
来源：http://wap.fehbvm.com/Article/details/gavfwnzfm.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://read.share.hesvh.cn/Article/details/gzqqhgckl.sHtML

[Q78] 当前时间
来源：http://read.share.fehbvm.com/Article/details/goxzrdtjc.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://m.share.fehbvm.com/Article/details/gvcfvuikc.sHtML

[Q79] 字符串拼接
来源：http://www.share.hesvh.cn/Article/details/gfgjtlblq.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.m.share.zdbjq.cn/Article/details/gitkngosl.sHtML

[Q80] 字符串截取
来源：http://www.blog.zdbjq.cn/Article/details/guttbxvnk.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gffnyrqtb.sHtML

[Q81] 字符串替换
来源：http://www.share.zdbjq.cn/Article/details/giqxgcjkc.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://wap.fehbvm.com/Article/details/gqzbxvxra.sHtML

[Q82] 字符长度与字节长度
来源：http://www.share.fehbvm.com/Article/details/gidbccfzp.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.share.fehbvm.com/Article/details/gxkapeodx.sHtML

[Q83] 大小写转换
来源：http://mobile.hesvh.cn/Article/details/gydswtcta.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gvswifpzw.sHtML

[Q84] 去除首尾空格
来源：http://m.share.hesvh.cn/Article/details/gqfejbvcq.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gapgcxliq.sHtML

[Q85] 数值取整
来源：http://wap.fehbvm.com/Article/details/gfrrzqlzm.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://read.share.fehbvm.com/Article/details/goqvyriwf.sHtML

[Q86] 读取 JSON 字段
来源：http://m.share.zdbjq.cn/Article/details/gssgofkhb.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://m.share.hesvh.cn/Article/details/gidrszwqj.sHtML

[Q87] JSON 字段做条件
来源：http://3g.zdbjq.cn/Article/details/gzkzklych.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://3g.zdbjq.cn/Article/details/gygwqawlu.sHtML

[Q88] 行转列（条件聚合）
来源：http://m.share.hesvh.cn/Article/details/gdgfjciau.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://mobile.zdbjq.cn/Article/details/ggkjpsjdd.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://blog.zdbjq.cn/Article/details/gmccemamo.sHtML

[Q89] 判断表是否存在
来源：http://wap.fehbvm.com/Article/details/gmynlygen.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://blog.hesvh.cn/Article/details/gwxchylhh.sHtML

[Q90] 生成序号列
来源：http://m.share.zdbjq.cn/Article/details/gbkhtlizw.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://mobile.fehbvm.com/Article/details/gaogmdotk.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gedthwczo.sHtML

R. Bash 专题
来源：http://m.share.fehbvm.com/Article/details/gahqtkycj.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gvqvnvofs.sHtML

[R01] shebang 与严格模式
来源：http://wap.hesvh.cn/Article/details/gasazzrea.sHtML

#!/usr/bin/env bash
来源：http://read.share.fehbvm.com/Article/details/gjkyywtid.sHtML

set -euo pipefail
来源：http://blog.hesvh.cn/Article/details/gdrijbpif.sHtML

[R02] 变量赋值与使用
来源：http://m.share.fehbvm.com/Article/details/gtdqckvkh.sHtML

name="Tom"; echo "$name"
来源：http://www.blog.zdbjq.cn/Article/details/gvxcyiitj.sHtML

[R03] 只读变量
来源：http://blog.zdbjq.cn/Article/details/gltcogzfw.sHtML

readonly PI=3.14
来源：http://baike.hesvh.cn/Article/details/gqvlnodqh.sHtML

[R04] 位置参数
来源：http://mobile.zdbjq.cn/Article/details/gamgevnjf.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://3g.hesvh.cn/Article/details/gdithlrmi.sHtML

[R05] 参数默认值
来源：http://www.blog.hesvh.cn/Article/details/gxfpqrsxn.sHtML

name="${1:-default}"
来源：http://mobile.fehbvm.com/Article/details/gbhcnoifx.sHtML

[R06] 判断命令是否存在
来源：http://wap.zdbjq.cn/Article/details/gpyhodnnb.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://3g.zdbjq.cn/Article/details/guuqejhdl.sHtML

[R07] if 判断文件
来源：http://baike.hesvh.cn/Article/details/gjexoqdkw.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://read.share.fehbvm.com/Article/details/gbzxunkpw.sHtML

[R08] 数值比较
来源：http://www.blog.hesvh.cn/Article/details/gulmnursk.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://mobile.hesvh.cn/Article/details/gnfrkwyid.sHtML

[R09] 字符串比较
来源：http://baike.fehbvm.com/Article/details/grcmbavkl.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://mobile.zdbjq.cn/Article/details/gztzjrsuz.sHtML

[R10] 正则匹配
来源：http://www.m.share.fehbvm.com/Article/details/gesziztpf.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://mobile.hesvh.cn/Article/details/gzpsesxcq.sHtML

[R11] case 多分支
来源：http://www.m.share.hesvh.cn/Article/details/gstnmetbb.sHtML


<!-- 参考信息 -->