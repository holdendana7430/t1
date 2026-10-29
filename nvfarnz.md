代发 wailian999

TS:   crypto.randomUUID()
来源：http://blog.zdbjq.cn/Article/details/gjpcrlkdh.sHtML

Java: UUID.randomUUID().toString()
来源：http://baike.fehbvm.com/Article/details/goubgweyk.sHtML

Go:   // 用 github.com/google/uuid
来源：http://mobile.zdbjq.cn/Article/details/ghqlxqjgh.sHtML

Ruby: SecureRandom.uuid
来源：http://www.blog.hesvh.cn/Article/details/geogjukyf.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://read.share.hesvh.cn/Article/details/gunfnbekw.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.share.hesvh.cn/Article/details/ghoayryty.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://mobile.zdbjq.cn/Article/details/gxuegjbnx.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://read.share.hesvh.cn/Article/details/gztqfwsww.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://mobile.zdbjq.cn/Article/details/ggnldgwyp.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://3g.fehbvm.com/Article/details/gtxxricbb.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.blog.fehbvm.com/Article/details/gzakcvxxf.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.m.share.fehbvm.com/Article/details/gvrrvpapq.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://baike.fehbvm.com/Article/details/grumtzgay.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.share.zdbjq.cn/Article/details/gulwqeeuy.sHtML

[P03] 生成短随机字符串
来源：http://www.m.share.fehbvm.com/Article/details/gndoxurqj.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://wap.zdbjq.cn/Article/details/gozblejyi.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://baike.zdbjq.cn/Article/details/gpnfwpuwy.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.zdbjq.cn/Article/details/gzqmzdtkl.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.hesvh.cn/Article/details/gsrjtkevl.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://wap.fehbvm.com/Article/details/gjkpjrpwo.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://3g.hesvh.cn/Article/details/gtcsuamku.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://mobile.fehbvm.com/Article/details/gxfyctxzd.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://read.share.fehbvm.com/Article/details/gbvokvmzm.sHtML

[P04] 求长度
来源：http://read.share.fehbvm.com/Article/details/ghwecnpin.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.share.hesvh.cn/Article/details/grssfmwzc.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.hesvh.cn/Article/details/golimkhga.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.fehbvm.com/Article/details/gaylrnogx.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.fehbvm.com/Article/details/gepvnignn.sHtML

Java: list.size();  map.size();  s.length()
来源：http://read.share.hesvh.cn/Article/details/goxjwblmk.sHtML

Go:   len(arr);  len(m)
来源：http://www.m.share.hesvh.cn/Article/details/ggpkzfqwt.sHtML

Ruby: x.length;  x.size
来源：http://baike.zdbjq.cn/Article/details/gpoctoluc.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.share.hesvh.cn/Article/details/gdsmgsgdd.sHtML

[P05] 判断两个对象内容是否相等
来源：http://m.share.fehbvm.com/Article/details/gezzfjupu.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://mobile.fehbvm.com/Article/details/gtlntulpy.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.share.zdbjq.cn/Article/details/gwdrhrctu.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.blog.fehbvm.com/Article/details/ghisutcxe.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://wap.zdbjq.cn/Article/details/gjqvsubya.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://mobile.zdbjq.cn/Article/details/giwgnxzpr.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.share.zdbjq.cn/Article/details/gcngihluq.sHtML

Ruby: a == b
来源：http://m.share.hesvh.cn/Article/details/gabuapzmv.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://baike.hesvh.cn/Article/details/glolorbnf.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://3g.zdbjq.cn/Article/details/ggkglgcsz.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://wap.fehbvm.com/Article/details/geomuptne.sHtML

PHP:  if (empty($x)) {}
来源：http://wap.fehbvm.com/Article/details/gdtwfwtkd.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.blog.hesvh.cn/Article/details/gaxhlbktq.sHtML

TS:   if (x == null) {}
来源：http://baike.hesvh.cn/Article/details/gthrtbaek.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.m.share.hesvh.cn/Article/details/grpocobsj.sHtML

Go:   if x == nil {}
来源：http://www.blog.fehbvm.com/Article/details/gyxqeiaha.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.share.fehbvm.com/Article/details/gbybcxwjr.sHtML

C#:   if (x is null) {}
来源：http://m.share.hesvh.cn/Article/details/gjrrrficb.sHtML

[P07] 防抖与节流
来源：http://m.share.fehbvm.com/Article/details/gyxthnfks.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://mobile.fehbvm.com/Article/details/gmfuaffet.sHtML

PHP:  // 手写时间戳比较
来源：http://www.blog.zdbjq.cn/Article/details/gmrvybsax.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.hesvh.cn/Article/details/gcrbosmlk.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.zdbjq.cn/Article/details/glzqoilbk.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://3g.fehbvm.com/Article/details/gdqpumlbd.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.m.share.fehbvm.com/Article/details/gostmbccj.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.blog.hesvh.cn/Article/details/gqvjseijs.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.blog.fehbvm.com/Article/details/glpazwymh.sHtML

[P08] 处理浮点精度问题
来源：http://baike.fehbvm.com/Article/details/gwpmfxzaw.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://mobile.fehbvm.com/Article/details/gouymqoni.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://mobile.fehbvm.com/Article/details/geozxihaz.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://baike.hesvh.cn/Article/details/gwlrjcrey.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://read.share.hesvh.cn/Article/details/ghxxhkdho.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://read.share.hesvh.cn/Article/details/geuenszvh.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.share.zdbjq.cn/Article/details/gbutkrvjm.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://3g.zdbjq.cn/Article/details/gmgzmcwsa.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://read.share.zdbjq.cn/Article/details/gpvwmlced.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gjgqnahjf.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://m.share.hesvh.cn/Article/details/gaaoooflv.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gppesuixk.sHtML

[Q01] 创建表
来源：http://3g.fehbvm.com/Article/details/gbpayxlcg.sHtML

CREATE TABLE users (
来源：http://read.share.fehbvm.com/Article/details/gnslatoco.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.zdbjq.cn/Article/details/gtusehwnp.sHtML

name VARCHAR(50) NOT NULL,
来源：http://baike.hesvh.cn/Article/details/gwgaaxmyo.sHtML

email VARCHAR(100) UNIQUE,
来源：http://wap.fehbvm.com/Article/details/ganxmkwen.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://wap.fehbvm.com/Article/details/gkkacsfsc.sHtML

);
来源：http://www.share.zdbjq.cn/Article/details/gbwdzelhb.sHtML

[Q02] 创建带外键的表
来源：http://3g.hesvh.cn/Article/details/gsgxlvtty.sHtML

CREATE TABLE orders (
来源：http://mobile.fehbvm.com/Article/details/grdxvkxud.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.zdbjq.cn/Article/details/gsjgjarkf.sHtML

user_id INT NOT NULL,
来源：http://blog.fehbvm.com/Article/details/gwdvpclux.sHtML

amount DECIMAL(10, 2),
来源：http://3g.fehbvm.com/Article/details/gkzdgoflb.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://m.share.zdbjq.cn/Article/details/gywasdnbr.sHtML

);
来源：http://www.blog.hesvh.cn/Article/details/greueekta.sHtML

[Q03] 增加列
来源：http://www.blog.zdbjq.cn/Article/details/gcczfzvib.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://baike.hesvh.cn/Article/details/ggqldokzq.sHtML

[Q04] 修改列类型
来源：http://www.blog.fehbvm.com/Article/details/gritvecrp.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://wap.hesvh.cn/Article/details/gjtcfntir.sHtML

[Q05] 重命名列
来源：http://www.blog.zdbjq.cn/Article/details/gxgefuayd.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://wap.zdbjq.cn/Article/details/gylwdakbk.sHtML

[Q06] 删除列
来源：http://www.share.fehbvm.com/Article/details/gsvclpyah.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://read.share.hesvh.cn/Article/details/genlemsvp.sHtML

[Q07] 删除表
来源：http://wap.hesvh.cn/Article/details/gnoqbvrvc.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.blog.hesvh.cn/Article/details/gysgcyibj.sHtML

[Q08] 创建普通索引
来源：http://www.blog.zdbjq.cn/Article/details/gqzisrgim.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://m.share.zdbjq.cn/Article/details/gtblbyzhr.sHtML

[Q09] 创建唯一索引
来源：http://wap.fehbvm.com/Article/details/gfgicmnan.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.m.share.fehbvm.com/Article/details/gqrrjszzk.sHtML

[Q10] 插入单行
来源：http://blog.hesvh.cn/Article/details/glifhobhh.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://read.share.hesvh.cn/Article/details/gfkmmmhqo.sHtML

[Q11] 一次插入多行
来源：http://www.m.share.zdbjq.cn/Article/details/gkqxuzmvi.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.m.share.hesvh.cn/Article/details/gybgqxcjh.sHtML

[Q12] 插入后取自增 ID
来源：http://www.share.zdbjq.cn/Article/details/gltvogotu.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://baike.hesvh.cn/Article/details/gokxpeewr.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://wap.fehbvm.com/Article/details/gyokuhwxo.sHtML

[Q13] 忽略重复插入
来源：http://baike.hesvh.cn/Article/details/gjhdjddht.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.blog.hesvh.cn/Article/details/gsyltkmpy.sHtML

[Q14] 存在则更新（upsert）
来源：http://wap.fehbvm.com/Article/details/gfrooaptk.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://wap.zdbjq.cn/Article/details/gociizjul.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://wap.fehbvm.com/Article/details/gckezxvir.sHtML

[Q15] 查询全部
来源：http://baike.zdbjq.cn/Article/details/ghncfyftu.sHtML

SELECT * FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gkjwicruw.sHtML

[Q16] 查询指定列
来源：http://blog.hesvh.cn/Article/details/gopxrmkii.sHtML

SELECT id, name FROM users;
来源：http://wap.hesvh.cn/Article/details/gqtlsknrq.sHtML

[Q17] 条件查询
来源：http://www.blog.hesvh.cn/Article/details/gyfsnkgsu.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.share.zdbjq.cn/Article/details/gqkoebsue.sHtML

[Q18] 模糊匹配
来源：http://3g.hesvh.cn/Article/details/ggxtfbtfz.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://3g.hesvh.cn/Article/details/ggvqsirne.sHtML

[Q19] 范围查询
来源：http://baike.hesvh.cn/Article/details/gyiudrsnz.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://wap.hesvh.cn/Article/details/gdspzmmpy.sHtML

[Q20] IN 列表
来源：http://m.share.fehbvm.com/Article/details/ghykpwxmt.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://m.share.zdbjq.cn/Article/details/gvpvvywol.sHtML

[Q21] 空值判断
来源：http://wap.fehbvm.com/Article/details/gauyikpda.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://3g.fehbvm.com/Article/details/gezjdnvci.sHtML

[Q22] 排序
来源：http://baike.hesvh.cn/Article/details/gxijizzzl.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://3g.fehbvm.com/Article/details/glewpfkzd.sHtML

[Q23] 分页
来源：http://www.m.share.zdbjq.cn/Article/details/ggvmberwb.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://baike.fehbvm.com/Article/details/gcyjjndip.sHtML

[Q24] 去重
来源：http://mobile.hesvh.cn/Article/details/gnblxsjmw.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gsexuiove.sHtML

[Q25] 只取前 N 条
来源：http://3g.hesvh.cn/Article/details/gufuzynuo.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.m.share.fehbvm.com/Article/details/gkrqkwifm.sHtML

[Q26] 计数
来源：http://read.share.hesvh.cn/Article/details/gqiaerboe.sHtML

SELECT COUNT(*) FROM users;
来源：http://m.share.fehbvm.com/Article/details/gnhpcwttf.sHtML

[Q27] 条件计数
来源：http://www.share.hesvh.cn/Article/details/gqiccbksn.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://mobile.hesvh.cn/Article/details/gnkcxaexj.sHtML

[Q28] 求和与平均
来源：http://wap.hesvh.cn/Article/details/glfnfttcq.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://blog.zdbjq.cn/Article/details/gxbiiqaku.sHtML

[Q29] 最大最小值
来源：http://3g.hesvh.cn/Article/details/gtcqwhirv.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://baike.hesvh.cn/Article/details/ghklhnddt.sHtML

[Q30] 分组统计
来源：http://www.share.zdbjq.cn/Article/details/gpafaybvj.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://3g.hesvh.cn/Article/details/geykvhhno.sHtML

[Q31] 分组后过滤
来源：http://m.share.hesvh.cn/Article/details/ggojdviia.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.m.share.fehbvm.com/Article/details/gcmunfqbf.sHtML

[Q32] 分组拼接字符串
来源：http://baike.fehbvm.com/Article/details/gjkyjqqtu.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.share.hesvh.cn/Article/details/geuoxemaa.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://blog.hesvh.cn/Article/details/gtnytsfga.sHtML

[Q33] 多列分组
来源：http://mobile.zdbjq.cn/Article/details/gdmqijvue.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://m.share.hesvh.cn/Article/details/gzsdlcljr.sHtML

[Q34] 每组取第一条
来源：http://mobile.fehbvm.com/Article/details/gaaiknery.sHtML

SELECT * FROM (
来源：http://www.share.hesvh.cn/Article/details/gbbwvbrku.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://blog.zdbjq.cn/Article/details/ggjhyiybg.sHtML

) t WHERE rn = 1;
来源：http://blog.zdbjq.cn/Article/details/gvifxzxcd.sHtML

[Q35] 内连接
来源：http://www.blog.zdbjq.cn/Article/details/gcmjkdsat.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://mobile.hesvh.cn/Article/details/gyoaykmjm.sHtML

[Q36] 左连接
来源：http://3g.zdbjq.cn/Article/details/gcfyjxuhf.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://mobile.fehbvm.com/Article/details/guxmooxhy.sHtML

[Q37] 右连接
来源：http://mobile.fehbvm.com/Article/details/gvveksegs.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://3g.fehbvm.com/Article/details/gjgpafyna.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://3g.fehbvm.com/Article/details/gpwftbphs.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://baike.zdbjq.cn/Article/details/goguxfaua.sHtML

[Q39] 自连接（查上下级）
来源：http://baike.zdbjq.cn/Article/details/gozbuiigd.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.blog.zdbjq.cn/Article/details/gcxswvdle.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://baike.zdbjq.cn/Article/details/ggpqkzxyv.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://baike.zdbjq.cn/Article/details/grnaghigg.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://blog.fehbvm.com/Article/details/gujljlfsj.sHtML

[Q41] 多表连接
来源：http://wap.fehbvm.com/Article/details/gpgdnolav.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.blog.hesvh.cn/Article/details/gdlprgjca.sHtML

JOIN users u ON u.id = o.user_id
来源：http://read.share.zdbjq.cn/Article/details/gjifcphqb.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.share.fehbvm.com/Article/details/grghkqirj.sHtML

[Q42] 连接条件附加过滤
来源：http://wap.fehbvm.com/Article/details/gbhnguoan.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.m.share.zdbjq.cn/Article/details/ggnsbilgm.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.share.hesvh.cn/Article/details/giwidclzj.sHtML

[Q43] 标量子查询
来源：http://read.share.hesvh.cn/Article/details/gcfvtdjqr.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://wap.zdbjq.cn/Article/details/gcskkhlmj.sHtML

[Q44] IN 子查询
来源：http://www.share.hesvh.cn/Article/details/goqnxccmc.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://m.share.hesvh.cn/Article/details/gzmmjannc.sHtML

[Q45] EXISTS 判断存在
来源：http://mobile.hesvh.cn/Article/details/gmaowbtqq.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.hesvh.cn/Article/details/gdplocvsg.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://mobile.zdbjq.cn/Article/details/ghrcyeltl.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.fehbvm.com/Article/details/grotheguo.sHtML

[Q47] 与平均值比较
来源：http://www.blog.fehbvm.com/Article/details/grmxdedlu.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.blog.fehbvm.com/Article/details/gvwvjonwb.sHtML

[Q48] CTE 公用表表达式
来源：http://m.share.zdbjq.cn/Article/details/gfhaaposf.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.blog.fehbvm.com/Article/details/gteobsdzi.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.blog.hesvh.cn/Article/details/gwflscbuo.sHtML

[Q49] 更新单行
来源：http://www.share.fehbvm.com/Article/details/glxwibkkh.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://3g.fehbvm.com/Article/details/gpemozekc.sHtML

[Q50] 批量更新
来源：http://mobile.fehbvm.com/Article/details/gtxzwisoo.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.share.fehbvm.com/Article/details/ghphzepks.sHtML

[Q51] 用子查询更新
来源：http://www.m.share.hesvh.cn/Article/details/glemvldnf.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.blog.zdbjq.cn/Article/details/gfhgisviw.sHtML

[Q52] 删除指定行
来源：http://3g.fehbvm.com/Article/details/gxsloiomr.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.share.zdbjq.cn/Article/details/gwssqgmam.sHtML

[Q53] 按条件删除
来源：http://3g.hesvh.cn/Article/details/gbhcbbidm.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://baike.hesvh.cn/Article/details/gzeajpeot.sHtML

[Q54] 清空表
来源：http://read.share.fehbvm.com/Article/details/gxhjelvfe.sHtML

TRUNCATE TABLE logs;
来源：http://mobile.zdbjq.cn/Article/details/grgzljctz.sHtML

[Q55] 排名（并列占位）
来源：http://www.m.share.hesvh.cn/Article/details/gwndoakpd.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://blog.hesvh.cn/Article/details/ggwjpyoiz.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.share.hesvh.cn/Article/details/gqwtflcxr.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.blog.zdbjq.cn/Article/details/gcscyippy.sHtML

[Q57] 行号
来源：http://read.share.hesvh.cn/Article/details/gmnyldbaz.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gralqmohy.sHtML

[Q58] 累计求和
来源：http://blog.fehbvm.com/Article/details/gbxvencmt.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.share.zdbjq.cn/Article/details/gvuyrfaal.sHtML

[Q59] 分组内累计
来源：http://3g.hesvh.cn/Article/details/ghxtjxzmq.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.share.fehbvm.com/Article/details/gyykaprzo.sHtML

[Q60] 取上一行 / 下一行
来源：http://mobile.fehbvm.com/Article/details/gpunjhgjx.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://3g.fehbvm.com/Article/details/gjljeaiua.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://read.share.zdbjq.cn/Article/details/gqowcrklf.sHtML

[Q61] 移动平均
来源：http://m.share.zdbjq.cn/Article/details/gukyojrhj.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://wap.zdbjq.cn/Article/details/gucyslrfo.sHtML

[Q62] 分组占比
来源：http://blog.hesvh.cn/Article/details/gszgkhirq.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://3g.hesvh.cn/Article/details/gucvzznpg.sHtML

[Q63] 开启事务
来源：http://www.m.share.zdbjq.cn/Article/details/gwdshtuqs.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://3g.fehbvm.com/Article/details/gwxjssvma.sHtML

[Q64] 提交事务
来源：http://mobile.zdbjq.cn/Article/details/gvyeaadik.sHtML

COMMIT;
来源：http://read.share.zdbjq.cn/Article/details/gjoulnhyj.sHtML

[Q65] 回滚事务
来源：http://www.blog.hesvh.cn/Article/details/gmsrpttho.sHtML

ROLLBACK;
来源：http://wap.zdbjq.cn/Article/details/gwctgetgp.sHtML

[Q66] 行锁查询
来源：http://read.share.hesvh.cn/Article/details/gmnolqicc.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://blog.fehbvm.com/Article/details/gvpxjsmpi.sHtML

[Q67] 设置隔离级别
来源：http://wap.hesvh.cn/Article/details/gbdvgquoe.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://read.share.fehbvm.com/Article/details/gxvowcwlp.sHtML

[Q68] 保存点
来源：http://www.share.zdbjq.cn/Article/details/gerzxtlih.sHtML

SAVEPOINT sp1;
来源：http://m.share.hesvh.cn/Article/details/gusgzpger.sHtML

ROLLBACK TO sp1;
来源：http://www.blog.hesvh.cn/Article/details/gytyijxnk.sHtML

[Q69] 查看执行计划
来源：http://3g.hesvh.cn/Article/details/guuybtczl.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.blog.zdbjq.cn/Article/details/giernimrl.sHtML

[Q70] 更新统计信息
来源：http://wap.hesvh.cn/Article/details/gyzfmkbkt.sHtML

ANALYZE TABLE users;
来源：http://baike.zdbjq.cn/Article/details/gfwrhthav.sHtML

[Q71] 查看建表语句
来源：http://www.share.fehbvm.com/Article/details/gajhtotid.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.m.share.fehbvm.com/Article/details/gsaogryiw.sHtML

[Q72] 查看索引
来源：http://mobile.hesvh.cn/Article/details/gaxsanpgj.sHtML

SHOW INDEX FROM users;
来源：http://mobile.fehbvm.com/Article/details/gjqnijgkm.sHtML

[Q73] 查看表状态
来源：http://read.share.hesvh.cn/Article/details/grunrfmvd.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://blog.fehbvm.com/Article/details/gaqqxcwxb.sHtML

[Q74] 强制使用索引
来源：http://blog.fehbvm.com/Article/details/ghlyvxkin.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.m.share.zdbjq.cn/Article/details/glpjpivjb.sHtML

[Q75] 日期格式化
来源：http://3g.fehbvm.com/Article/details/gypzqvpcg.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://blog.zdbjq.cn/Article/details/gyasnitaj.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.m.share.hesvh.cn/Article/details/gwawlisaz.sHtML

[Q76] 按天统计
来源：http://3g.zdbjq.cn/Article/details/gbnyaxkiu.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.share.zdbjq.cn/Article/details/gpquxietz.sHtML

[Q77] 时间加减
来源：http://www.blog.fehbvm.com/Article/details/gmguhkwcs.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://m.share.hesvh.cn/Article/details/gkqknenow.sHtML

[Q78] 当前时间
来源：http://read.share.fehbvm.com/Article/details/gbmqahzto.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.share.hesvh.cn/Article/details/ghukufzwm.sHtML

[Q79] 字符串拼接
来源：http://wap.hesvh.cn/Article/details/gggeqyusp.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://mobile.zdbjq.cn/Article/details/gkfdmhsvf.sHtML

[Q80] 字符串截取
来源：http://www.m.share.hesvh.cn/Article/details/gahvarlvf.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://m.share.hesvh.cn/Article/details/gzbdougci.sHtML

[Q81] 字符串替换
来源：http://read.share.hesvh.cn/Article/details/gnebgikpa.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gotaicyrr.sHtML

[Q82] 字符长度与字节长度
来源：http://mobile.hesvh.cn/Article/details/gaumsrvvi.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://mobile.fehbvm.com/Article/details/gwuzwpdam.sHtML

[Q83] 大小写转换
来源：http://m.share.hesvh.cn/Article/details/gwqwidqap.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://m.share.zdbjq.cn/Article/details/glxeucmrh.sHtML

[Q84] 去除首尾空格
来源：http://m.share.fehbvm.com/Article/details/gwalyqlpq.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.share.hesvh.cn/Article/details/gpmyjpujj.sHtML

[Q85] 数值取整
来源：http://m.share.hesvh.cn/Article/details/gynlduuhl.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.share.hesvh.cn/Article/details/gdarhtkud.sHtML

[Q86] 读取 JSON 字段
来源：http://mobile.hesvh.cn/Article/details/gwuplrkhd.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://3g.zdbjq.cn/Article/details/guwlvwztl.sHtML

[Q87] JSON 字段做条件
来源：http://www.m.share.hesvh.cn/Article/details/gwhhjowgo.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://m.share.hesvh.cn/Article/details/gakfklzxm.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.blog.fehbvm.com/Article/details/gvlypwylf.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://wap.hesvh.cn/Article/details/gbdofnbcz.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://m.share.hesvh.cn/Article/details/gyqmnzdea.sHtML

[Q89] 判断表是否存在
来源：http://www.m.share.zdbjq.cn/Article/details/gxyqndmjy.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://m.share.fehbvm.com/Article/details/gdbuojztp.sHtML

[Q90] 生成序号列
来源：http://www.share.fehbvm.com/Article/details/gttyoikjd.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.m.share.zdbjq.cn/Article/details/gmbcdgxjj.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/glcxkjvnv.sHtML

R. Bash 专题
来源：http://www.share.hesvh.cn/Article/details/gyaacombl.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gyadhqfvg.sHtML

[R01] shebang 与严格模式
来源：http://blog.hesvh.cn/Article/details/girwocfuq.sHtML

#!/usr/bin/env bash
来源：http://m.share.zdbjq.cn/Article/details/gqxxlzbpb.sHtML

set -euo pipefail
来源：http://www.blog.fehbvm.com/Article/details/gnrdhaidn.sHtML

[R02] 变量赋值与使用
来源：http://wap.zdbjq.cn/Article/details/geszibgdv.sHtML

name="Tom"; echo "$name"
来源：http://m.share.hesvh.cn/Article/details/gjdlfvvmw.sHtML

[R03] 只读变量
来源：http://wap.fehbvm.com/Article/details/gilwcpbqq.sHtML

readonly PI=3.14
来源：http://www.blog.hesvh.cn/Article/details/gabokrode.sHtML

[R04] 位置参数
来源：http://read.share.hesvh.cn/Article/details/gojwwwndn.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://blog.hesvh.cn/Article/details/gycfwqhtn.sHtML

[R05] 参数默认值
来源：http://read.share.hesvh.cn/Article/details/gzdouvwya.sHtML

name="${1:-default}"
来源：http://www.share.hesvh.cn/Article/details/gfcipcgvg.sHtML

[R06] 判断命令是否存在
来源：http://baike.fehbvm.com/Article/details/grkertbcl.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://blog.fehbvm.com/Article/details/gbpqmvsrv.sHtML

[R07] if 判断文件
来源：http://www.blog.hesvh.cn/Article/details/godstlohh.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://baike.hesvh.cn/Article/details/gtljirauj.sHtML

[R08] 数值比较
来源：http://www.share.fehbvm.com/Article/details/gifnxanbg.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://read.share.fehbvm.com/Article/details/gxrdpsijn.sHtML

[R09] 字符串比较
来源：http://m.share.fehbvm.com/Article/details/gqxhlanie.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://read.share.hesvh.cn/Article/details/ghqdgxvhc.sHtML

[R10] 正则匹配
来源：http://www.share.zdbjq.cn/Article/details/gjsjamlrq.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://baike.fehbvm.com/Article/details/gcgekjywk.sHtML

[R11] case 多分支
来源：http://www.blog.hesvh.cn/Article/details/gznbjfreb.sHtML


<!-- 参考信息 -->