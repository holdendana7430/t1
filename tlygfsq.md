代发 wailian999

C#:   Parallel.For
来源：http://3g.zdbjq.cn/Article/details/gczescokp.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gwihxztfv.sHtML

P. 常用工具函数
来源：http://www.blog.fehbvm.com/Article/details/gfecoxmiy.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/guuctaocc.sHtML

[P01] 生成 UUID
来源：http://mobile.fehbvm.com/Article/details/gbkjxbxgd.sHtML

Py:   str(uuid.uuid4())
来源：http://3g.hesvh.cn/Article/details/gtizzcqau.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://mobile.fehbvm.com/Article/details/gxnmtjhhv.sHtML

JS:   crypto.randomUUID()
来源：http://baike.fehbvm.com/Article/details/gvbkhawgz.sHtML

TS:   crypto.randomUUID()
来源：http://blog.hesvh.cn/Article/details/gijkdqjrk.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.blog.fehbvm.com/Article/details/gmjkbrtcu.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.share.hesvh.cn/Article/details/gqermpxae.sHtML

Ruby: SecureRandom.uuid
来源：http://www.blog.hesvh.cn/Article/details/gtwiyohhr.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://wap.fehbvm.com/Article/details/gynbnoopy.sHtML

[P02] MD5 / SHA256 摘要
来源：http://read.share.fehbvm.com/Article/details/gztjfabhe.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://m.share.fehbvm.com/Article/details/gahkjieqa.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://m.share.zdbjq.cn/Article/details/gtbmvdioz.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://read.share.hesvh.cn/Article/details/gsazskhwd.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://wap.hesvh.cn/Article/details/gkeabyvnj.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://mobile.zdbjq.cn/Article/details/gcacsttdb.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://mobile.fehbvm.com/Article/details/goxstanvs.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://wap.fehbvm.com/Article/details/glvlddggc.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.m.share.fehbvm.com/Article/details/ghkenmufo.sHtML

[P03] 生成短随机字符串
来源：http://m.share.fehbvm.com/Article/details/gaaivwtmr.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://baike.fehbvm.com/Article/details/gshjnowan.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.share.hesvh.cn/Article/details/grahnpixy.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://3g.hesvh.cn/Article/details/gqozdohkj.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.zdbjq.cn/Article/details/gaafcicmx.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.share.fehbvm.com/Article/details/gfkgzzauo.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://baike.zdbjq.cn/Article/details/gcavuhtmc.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://baike.zdbjq.cn/Article/details/gkifydezw.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://baike.hesvh.cn/Article/details/gcfruoxel.sHtML

[P04] 求长度
来源：http://www.blog.fehbvm.com/Article/details/gcuoumdip.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://blog.fehbvm.com/Article/details/gxtesjjtg.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.zdbjq.cn/Article/details/gzjvchugm.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.zdbjq.cn/Article/details/gbbnlpxji.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.hesvh.cn/Article/details/gxkotogxl.sHtML

Java: list.size();  map.size();  s.length()
来源：http://wap.fehbvm.com/Article/details/gylwaunqo.sHtML

Go:   len(arr);  len(m)
来源：http://blog.fehbvm.com/Article/details/gonkcbxkg.sHtML

Ruby: x.length;  x.size
来源：http://blog.hesvh.cn/Article/details/gqnqavkuh.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://3g.fehbvm.com/Article/details/gzcaeoliq.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.m.share.zdbjq.cn/Article/details/grxmfprpq.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.share.fehbvm.com/Article/details/gqtcfwhjt.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://mobile.zdbjq.cn/Article/details/gbtgaojji.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://3g.hesvh.cn/Article/details/gpxjrfnhf.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://3g.zdbjq.cn/Article/details/grfrnygso.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.share.hesvh.cn/Article/details/gamzqqqel.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://3g.zdbjq.cn/Article/details/gvbeykkkw.sHtML

Ruby: a == b
来源：http://blog.hesvh.cn/Article/details/gbbpuybwp.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.blog.fehbvm.com/Article/details/gwhmqymcq.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://m.share.fehbvm.com/Article/details/gqaftpzln.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://baike.zdbjq.cn/Article/details/gglbktasa.sHtML

PHP:  if (empty($x)) {}
来源：http://mobile.fehbvm.com/Article/details/gupwullpt.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.blog.fehbvm.com/Article/details/gjcnlvnyw.sHtML

TS:   if (x == null) {}
来源：http://3g.fehbvm.com/Article/details/gvawccsqo.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://3g.zdbjq.cn/Article/details/gzkyoxcvr.sHtML

Go:   if x == nil {}
来源：http://wap.hesvh.cn/Article/details/gldtijszs.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://mobile.fehbvm.com/Article/details/gzkubcwgo.sHtML

C#:   if (x is null) {}
来源：http://3g.zdbjq.cn/Article/details/gfksjjfny.sHtML

[P07] 防抖与节流
来源：http://www.share.fehbvm.com/Article/details/gpicjgwpf.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.blog.hesvh.cn/Article/details/gygbzhqpu.sHtML

PHP:  // 手写时间戳比较
来源：http://wap.fehbvm.com/Article/details/gpeuaquri.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.hesvh.cn/Article/details/gfszmzxeb.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.fehbvm.com/Article/details/glonbldid.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://read.share.zdbjq.cn/Article/details/gxsfubueb.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.share.fehbvm.com/Article/details/gjqylweqj.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.m.share.zdbjq.cn/Article/details/gslrmgxro.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://blog.fehbvm.com/Article/details/gqziyfxbz.sHtML

[P08] 处理浮点精度问题
来源：http://mobile.hesvh.cn/Article/details/gzxfmthwl.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.m.share.hesvh.cn/Article/details/gcjaxjjbb.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://3g.fehbvm.com/Article/details/gideoonvp.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://m.share.fehbvm.com/Article/details/godobhmyq.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.share.zdbjq.cn/Article/details/gbogefifm.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://baike.zdbjq.cn/Article/details/gawkdpgbf.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://wap.zdbjq.cn/Article/details/gwkymkiae.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.blog.zdbjq.cn/Article/details/gteqgraac.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.m.share.fehbvm.com/Article/details/gulettbmr.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gbmalakod.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://baike.fehbvm.com/Article/details/gwxsalkwe.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gnuckqake.sHtML

[Q01] 创建表
来源：http://www.share.hesvh.cn/Article/details/guztoolra.sHtML

CREATE TABLE users (
来源：http://3g.zdbjq.cn/Article/details/gqgeaixbt.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.hesvh.cn/Article/details/gnjeblzkh.sHtML

name VARCHAR(50) NOT NULL,
来源：http://baike.hesvh.cn/Article/details/gbekbjsgx.sHtML

email VARCHAR(100) UNIQUE,
来源：http://read.share.fehbvm.com/Article/details/gwkeiitbn.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://baike.fehbvm.com/Article/details/gzzpheevn.sHtML

);
来源：http://baike.fehbvm.com/Article/details/gykzjjoxj.sHtML

[Q02] 创建带外键的表
来源：http://www.share.hesvh.cn/Article/details/gkeuhzjff.sHtML

CREATE TABLE orders (
来源：http://www.m.share.fehbvm.com/Article/details/gaqntchjr.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.fehbvm.com/Article/details/gqbauvain.sHtML

user_id INT NOT NULL,
来源：http://mobile.hesvh.cn/Article/details/gqsobgxoy.sHtML

amount DECIMAL(10, 2),
来源：http://baike.fehbvm.com/Article/details/gmbwctwap.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://mobile.hesvh.cn/Article/details/gvsgmfltk.sHtML

);
来源：http://www.share.zdbjq.cn/Article/details/gegttjdvk.sHtML

[Q03] 增加列
来源：http://m.share.hesvh.cn/Article/details/grssxqywa.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://blog.fehbvm.com/Article/details/gvcoksgac.sHtML

[Q04] 修改列类型
来源：http://www.blog.hesvh.cn/Article/details/gyjqqymkg.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://blog.fehbvm.com/Article/details/glmhnbmdd.sHtML

[Q05] 重命名列
来源：http://blog.hesvh.cn/Article/details/gthfprsyz.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.blog.hesvh.cn/Article/details/ggjlcxjuo.sHtML

[Q06] 删除列
来源：http://www.share.fehbvm.com/Article/details/grubnafwt.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://mobile.zdbjq.cn/Article/details/gbseochpn.sHtML

[Q07] 删除表
来源：http://wap.fehbvm.com/Article/details/gydfvfxla.sHtML

DROP TABLE IF EXISTS orders;
来源：http://baike.hesvh.cn/Article/details/ghyybksza.sHtML

[Q08] 创建普通索引
来源：http://3g.hesvh.cn/Article/details/gwufdovlf.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://read.share.fehbvm.com/Article/details/ggefvwgvd.sHtML

[Q09] 创建唯一索引
来源：http://3g.hesvh.cn/Article/details/gqjcykyig.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.blog.fehbvm.com/Article/details/gtiiqctcg.sHtML

[Q10] 插入单行
来源：http://3g.hesvh.cn/Article/details/gxehwrxuj.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.share.zdbjq.cn/Article/details/giouscvog.sHtML

[Q11] 一次插入多行
来源：http://mobile.hesvh.cn/Article/details/gztjnhdlw.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://mobile.fehbvm.com/Article/details/gblxvbfgq.sHtML

[Q12] 插入后取自增 ID
来源：http://read.share.fehbvm.com/Article/details/gwiqyjqzb.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.m.share.zdbjq.cn/Article/details/ggmrlawvi.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://blog.fehbvm.com/Article/details/gabwcqksx.sHtML

[Q13] 忽略重复插入
来源：http://3g.hesvh.cn/Article/details/gqljuohrg.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://blog.fehbvm.com/Article/details/gakwwlqpg.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.blog.fehbvm.com/Article/details/gwmftvosh.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.blog.fehbvm.com/Article/details/garmucxzy.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.m.share.hesvh.cn/Article/details/gugiyjgvm.sHtML

[Q15] 查询全部
来源：http://wap.hesvh.cn/Article/details/gflkgsruq.sHtML

SELECT * FROM users;
来源：http://wap.fehbvm.com/Article/details/gslxbsufz.sHtML

[Q16] 查询指定列
来源：http://blog.fehbvm.com/Article/details/gfhnnbfbl.sHtML

SELECT id, name FROM users;
来源：http://m.share.hesvh.cn/Article/details/gifzlbnwf.sHtML

[Q17] 条件查询
来源：http://read.share.zdbjq.cn/Article/details/gnryxdqka.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.m.share.hesvh.cn/Article/details/gtzuqsasd.sHtML

[Q18] 模糊匹配
来源：http://read.share.zdbjq.cn/Article/details/ghiwqoecd.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://mobile.fehbvm.com/Article/details/gjhcgbdoi.sHtML

[Q19] 范围查询
来源：http://blog.hesvh.cn/Article/details/guoxovtki.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://wap.fehbvm.com/Article/details/gsnijmwih.sHtML

[Q20] IN 列表
来源：http://wap.fehbvm.com/Article/details/gcsllrcmz.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://blog.zdbjq.cn/Article/details/gsxlynndd.sHtML

[Q21] 空值判断
来源：http://www.blog.zdbjq.cn/Article/details/gnzyeemoo.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://3g.zdbjq.cn/Article/details/ghsdpacti.sHtML

[Q22] 排序
来源：http://m.share.fehbvm.com/Article/details/gdtixvuel.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://wap.hesvh.cn/Article/details/gxtjojotu.sHtML

[Q23] 分页
来源：http://www.share.hesvh.cn/Article/details/gnejrvnuc.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.m.share.zdbjq.cn/Article/details/gviqewnyw.sHtML

[Q24] 去重
来源：http://3g.fehbvm.com/Article/details/gpdgtjidv.sHtML

SELECT DISTINCT city FROM users;
来源：http://3g.hesvh.cn/Article/details/gvkjdfvos.sHtML

[Q25] 只取前 N 条
来源：http://blog.zdbjq.cn/Article/details/gxwkhotwl.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://read.share.hesvh.cn/Article/details/gqumqlgmg.sHtML

[Q26] 计数
来源：http://blog.fehbvm.com/Article/details/gqdzmipwx.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gzkbzsudp.sHtML

[Q27] 条件计数
来源：http://baike.hesvh.cn/Article/details/gliacykfu.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://baike.fehbvm.com/Article/details/gjqquzrrj.sHtML

[Q28] 求和与平均
来源：http://3g.hesvh.cn/Article/details/gzdrhpjqp.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.share.fehbvm.com/Article/details/gpnmhjbhu.sHtML

[Q29] 最大最小值
来源：http://www.m.share.fehbvm.com/Article/details/gmarqcjtg.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://baike.hesvh.cn/Article/details/gvmppwfco.sHtML

[Q30] 分组统计
来源：http://www.m.share.hesvh.cn/Article/details/gnkbedxsg.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://blog.fehbvm.com/Article/details/gwlvkafsj.sHtML

[Q31] 分组后过滤
来源：http://wap.zdbjq.cn/Article/details/gsvvxolzy.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://read.share.zdbjq.cn/Article/details/grhkjfmfd.sHtML

[Q32] 分组拼接字符串
来源：http://blog.hesvh.cn/Article/details/genthgvjy.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://read.share.zdbjq.cn/Article/details/gezxqqiii.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://m.share.zdbjq.cn/Article/details/gcpqwjvoq.sHtML

[Q33] 多列分组
来源：http://m.share.hesvh.cn/Article/details/gvunoamtf.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://3g.zdbjq.cn/Article/details/gluywyqpr.sHtML

[Q34] 每组取第一条
来源：http://3g.zdbjq.cn/Article/details/gieuolnek.sHtML

SELECT * FROM (
来源：http://www.blog.hesvh.cn/Article/details/gffhhlcqf.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.m.share.zdbjq.cn/Article/details/gdgjuojdd.sHtML

) t WHERE rn = 1;
来源：http://m.share.fehbvm.com/Article/details/grfctbztu.sHtML

[Q35] 内连接
来源：http://mobile.fehbvm.com/Article/details/gbwfuqewh.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://m.share.fehbvm.com/Article/details/guvxbcveh.sHtML

[Q36] 左连接
来源：http://www.blog.fehbvm.com/Article/details/gbgamgjck.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://3g.zdbjq.cn/Article/details/gaoyvqwxy.sHtML

[Q37] 右连接
来源：http://read.share.fehbvm.com/Article/details/ggcuelrlf.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.m.share.hesvh.cn/Article/details/gcjbyfaye.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://3g.fehbvm.com/Article/details/gmmzzsjds.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://baike.hesvh.cn/Article/details/gibvzifvm.sHtML

[Q39] 自连接（查上下级）
来源：http://www.blog.fehbvm.com/Article/details/grokgevze.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://read.share.fehbvm.com/Article/details/gzmrgldmm.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://mobile.fehbvm.com/Article/details/gjjdvuead.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://baike.fehbvm.com/Article/details/gwmsxqlef.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.share.zdbjq.cn/Article/details/gjlgzwfva.sHtML

[Q41] 多表连接
来源：http://www.blog.zdbjq.cn/Article/details/gmvadzrrw.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.share.hesvh.cn/Article/details/gcpmdtwtd.sHtML

JOIN users u ON u.id = o.user_id
来源：http://blog.zdbjq.cn/Article/details/gemidmhak.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.m.share.zdbjq.cn/Article/details/gqbkbjqpf.sHtML

[Q42] 连接条件附加过滤
来源：http://m.share.zdbjq.cn/Article/details/ghoafbhuo.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.blog.zdbjq.cn/Article/details/gtwukzjig.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://blog.zdbjq.cn/Article/details/gnpoovefh.sHtML

[Q43] 标量子查询
来源：http://www.share.zdbjq.cn/Article/details/gjtgoakui.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.blog.hesvh.cn/Article/details/gtrcwjikt.sHtML

[Q44] IN 子查询
来源：http://3g.hesvh.cn/Article/details/gfuhdmegh.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://m.share.hesvh.cn/Article/details/givxlyvqy.sHtML

[Q45] EXISTS 判断存在
来源：http://mobile.zdbjq.cn/Article/details/gotndgvoh.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.zdbjq.cn/Article/details/gtoxlylwy.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://read.share.zdbjq.cn/Article/details/gefhwcipu.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.hesvh.cn/Article/details/guvjuqiah.sHtML

[Q47] 与平均值比较
来源：http://blog.zdbjq.cn/Article/details/gaimdpymd.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://wap.fehbvm.com/Article/details/gaiotyhdq.sHtML

[Q48] CTE 公用表表达式
来源：http://3g.fehbvm.com/Article/details/gbwnsfmlh.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://mobile.fehbvm.com/Article/details/gmszfasvj.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.share.fehbvm.com/Article/details/gjghohzxd.sHtML

[Q49] 更新单行
来源：http://blog.hesvh.cn/Article/details/gfzuasvli.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://mobile.zdbjq.cn/Article/details/gectrlqjd.sHtML

[Q50] 批量更新
来源：http://www.m.share.hesvh.cn/Article/details/gwjibkxgs.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.m.share.hesvh.cn/Article/details/gzxkfrmeh.sHtML

[Q51] 用子查询更新
来源：http://3g.zdbjq.cn/Article/details/gchvlrjnm.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://3g.hesvh.cn/Article/details/gnvwdgjji.sHtML

[Q52] 删除指定行
来源：http://3g.hesvh.cn/Article/details/gxmtlmiyv.sHtML

DELETE FROM users WHERE id = 10;
来源：http://m.share.zdbjq.cn/Article/details/goswffeeu.sHtML

[Q53] 按条件删除
来源：http://blog.fehbvm.com/Article/details/gwiacokmp.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://mobile.zdbjq.cn/Article/details/gdbmmdbbm.sHtML

[Q54] 清空表
来源：http://3g.hesvh.cn/Article/details/gundejyew.sHtML

TRUNCATE TABLE logs;
来源：http://m.share.zdbjq.cn/Article/details/gyimiyhip.sHtML

[Q55] 排名（并列占位）
来源：http://wap.hesvh.cn/Article/details/gpzmlhwur.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://3g.fehbvm.com/Article/details/giqjikxgo.sHtML

[Q56] 密集排名（并列不占位）
来源：http://blog.fehbvm.com/Article/details/gbouiaytx.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://wap.fehbvm.com/Article/details/galoqlqzv.sHtML

[Q57] 行号
来源：http://blog.fehbvm.com/Article/details/gnjxfnquo.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://m.share.fehbvm.com/Article/details/gmvbzatjy.sHtML

[Q58] 累计求和
来源：http://m.share.hesvh.cn/Article/details/gjsqttztj.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://3g.fehbvm.com/Article/details/gkzjsiqgv.sHtML

[Q59] 分组内累计
来源：http://www.blog.zdbjq.cn/Article/details/gygbkemvw.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://blog.fehbvm.com/Article/details/gqeeaicxv.sHtML

[Q60] 取上一行 / 下一行
来源：http://mobile.hesvh.cn/Article/details/gnpxuejdi.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://baike.fehbvm.com/Article/details/giaulsode.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.share.hesvh.cn/Article/details/gsbjlzfbb.sHtML

[Q61] 移动平均
来源：http://wap.zdbjq.cn/Article/details/ggofvufiz.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://read.share.zdbjq.cn/Article/details/grfpozbvd.sHtML

[Q62] 分组占比
来源：http://read.share.fehbvm.com/Article/details/grzmdxcud.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://baike.zdbjq.cn/Article/details/guaveluql.sHtML

[Q63] 开启事务
来源：http://www.m.share.fehbvm.com/Article/details/gdupkomxl.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://wap.zdbjq.cn/Article/details/glirbkyaf.sHtML

[Q64] 提交事务
来源：http://read.share.fehbvm.com/Article/details/gdjtiqari.sHtML

COMMIT;
来源：http://read.share.hesvh.cn/Article/details/ghpmubqem.sHtML

[Q65] 回滚事务
来源：http://wap.hesvh.cn/Article/details/ghbvhvwsy.sHtML

ROLLBACK;
来源：http://www.share.fehbvm.com/Article/details/gkklncoax.sHtML

[Q66] 行锁查询
来源：http://read.share.fehbvm.com/Article/details/glgigzcfs.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://blog.hesvh.cn/Article/details/gqkrvfdlt.sHtML

[Q67] 设置隔离级别
来源：http://blog.zdbjq.cn/Article/details/gychzilhk.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.share.zdbjq.cn/Article/details/guydtpaqh.sHtML

[Q68] 保存点
来源：http://wap.fehbvm.com/Article/details/gzkusbqix.sHtML

SAVEPOINT sp1;
来源：http://blog.fehbvm.com/Article/details/guihrtbrb.sHtML

ROLLBACK TO sp1;
来源：http://baike.fehbvm.com/Article/details/gjpeurnnb.sHtML

[Q69] 查看执行计划
来源：http://www.share.zdbjq.cn/Article/details/gzserauaw.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.blog.zdbjq.cn/Article/details/gsbvbgcsm.sHtML

[Q70] 更新统计信息
来源：http://m.share.zdbjq.cn/Article/details/gycryfega.sHtML

ANALYZE TABLE users;
来源：http://read.share.hesvh.cn/Article/details/gwruaqoab.sHtML

[Q71] 查看建表语句
来源：http://wap.fehbvm.com/Article/details/gwatikprd.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.m.share.hesvh.cn/Article/details/gtmxplslm.sHtML

[Q72] 查看索引
来源：http://www.share.fehbvm.com/Article/details/gmhhvyogr.sHtML

SHOW INDEX FROM users;
来源：http://read.share.hesvh.cn/Article/details/gjzcdxkgn.sHtML

[Q73] 查看表状态
来源：http://read.share.hesvh.cn/Article/details/gcyritdvq.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.m.share.fehbvm.com/Article/details/gbutondvh.sHtML

[Q74] 强制使用索引
来源：http://mobile.zdbjq.cn/Article/details/godawgyxq.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://blog.hesvh.cn/Article/details/gbkbvlvtq.sHtML

[Q75] 日期格式化
来源：http://blog.fehbvm.com/Article/details/gerdhmebs.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.share.zdbjq.cn/Article/details/gupxlsdkb.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.share.hesvh.cn/Article/details/garbkizvc.sHtML

[Q76] 按天统计
来源：http://m.share.hesvh.cn/Article/details/gwzfkerja.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://m.share.hesvh.cn/Article/details/gezsalkmr.sHtML

[Q77] 时间加减
来源：http://www.blog.hesvh.cn/Article/details/gklifyywt.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://blog.hesvh.cn/Article/details/gnahyqgbm.sHtML

[Q78] 当前时间
来源：http://www.m.share.hesvh.cn/Article/details/gzfdjobcb.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://blog.hesvh.cn/Article/details/gxzaalhmq.sHtML

[Q79] 字符串拼接
来源：http://www.share.zdbjq.cn/Article/details/gabzcwfeo.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://mobile.fehbvm.com/Article/details/gsamxjqgj.sHtML

[Q80] 字符串截取
来源：http://baike.zdbjq.cn/Article/details/gptxjzzjr.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/giczwxvea.sHtML

[Q81] 字符串替换
来源：http://read.share.hesvh.cn/Article/details/gjdgkqcoj.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://mobile.fehbvm.com/Article/details/gmflfpcnk.sHtML

[Q82] 字符长度与字节长度
来源：http://wap.fehbvm.com/Article/details/gxgfdadog.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://mobile.hesvh.cn/Article/details/ggigkvfaf.sHtML

[Q83] 大小写转换
来源：http://3g.zdbjq.cn/Article/details/gkjansxlb.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gloodydcr.sHtML

[Q84] 去除首尾空格
来源：http://m.share.fehbvm.com/Article/details/gexgbikme.sHtML

SELECT TRIM(name) FROM users;
来源：http://3g.fehbvm.com/Article/details/gtsbetzvz.sHtML

[Q85] 数值取整
来源：http://m.share.hesvh.cn/Article/details/gdsqlrxkp.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.blog.fehbvm.com/Article/details/gjnqyjzza.sHtML

[Q86] 读取 JSON 字段
来源：http://m.share.zdbjq.cn/Article/details/gjjwrxfjb.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://blog.hesvh.cn/Article/details/gmrwnmdup.sHtML

[Q87] JSON 字段做条件
来源：http://www.blog.zdbjq.cn/Article/details/gsvgwunti.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://wap.hesvh.cn/Article/details/gcxfldeuy.sHtML

[Q88] 行转列（条件聚合）
来源：http://mobile.fehbvm.com/Article/details/gpjlwtobr.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://baike.zdbjq.cn/Article/details/gqjlojuli.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://baike.zdbjq.cn/Article/details/gikmjsego.sHtML

[Q89] 判断表是否存在
来源：http://www.m.share.zdbjq.cn/Article/details/grpagrkqa.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://m.share.fehbvm.com/Article/details/gsqzkjorj.sHtML

[Q90] 生成序号列
来源：http://www.m.share.fehbvm.com/Article/details/gjxizbuts.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://read.share.zdbjq.cn/Article/details/gdfgeudif.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gtrkkqzrg.sHtML

R. Bash 专题
来源：http://www.share.fehbvm.com/Article/details/gwcwkwgve.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gxsdftpsk.sHtML

[R01] shebang 与严格模式
来源：http://www.share.fehbvm.com/Article/details/gzypudprn.sHtML

#!/usr/bin/env bash
来源：http://www.blog.hesvh.cn/Article/details/gwdmdrolz.sHtML

set -euo pipefail
来源：http://blog.hesvh.cn/Article/details/gwagogtzt.sHtML

[R02] 变量赋值与使用
来源：http://baike.zdbjq.cn/Article/details/gxnlejukz.sHtML

name="Tom"; echo "$name"
来源：http://mobile.zdbjq.cn/Article/details/gbikgafdy.sHtML

[R03] 只读变量
来源：http://wap.fehbvm.com/Article/details/glnnnjonj.sHtML

readonly PI=3.14
来源：http://m.share.fehbvm.com/Article/details/gvkxaimua.sHtML

[R04] 位置参数
来源：http://3g.zdbjq.cn/Article/details/gthazruoj.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.m.share.fehbvm.com/Article/details/gqxilodxn.sHtML

[R05] 参数默认值
来源：http://www.blog.fehbvm.com/Article/details/geiiunnqf.sHtML

name="${1:-default}"
来源：http://3g.fehbvm.com/Article/details/gzyempjhb.sHtML

[R06] 判断命令是否存在
来源：http://www.blog.zdbjq.cn/Article/details/gktiwrmoc.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://wap.zdbjq.cn/Article/details/gysuogaks.sHtML

[R07] if 判断文件
来源：http://www.m.share.zdbjq.cn/Article/details/gnqazaiqs.sHtML


<!-- 参考信息 -->