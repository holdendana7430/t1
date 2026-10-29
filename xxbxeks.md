代发 wailian999

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://wap.hesvh.cn/Article/details/gmekwyaep.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.share.zdbjq.cn/Article/details/guynlwjsu.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.m.share.fehbvm.com/Article/details/geoxitbae.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://wap.zdbjq.cn/Article/details/gytijkody.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.m.share.fehbvm.com/Article/details/ggvywxxuj.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://mobile.zdbjq.cn/Article/details/grxunisxv.sHtML

[P03] 生成短随机字符串
来源：http://m.share.zdbjq.cn/Article/details/gczmjqgul.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://3g.zdbjq.cn/Article/details/gostrlwrj.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.share.hesvh.cn/Article/details/ggobegcdj.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.fehbvm.com/Article/details/gkxxrtqbs.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.zdbjq.cn/Article/details/gqttujfui.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://3g.fehbvm.com/Article/details/gfznjrgns.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://baike.zdbjq.cn/Article/details/gcqowmwvb.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.share.zdbjq.cn/Article/details/gostexcpr.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://wap.zdbjq.cn/Article/details/genwagwfc.sHtML

[P04] 求长度
来源：http://wap.hesvh.cn/Article/details/gtmzvltyv.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.blog.hesvh.cn/Article/details/gskdrygrg.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.zdbjq.cn/Article/details/ghrtxjulx.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.hesvh.cn/Article/details/giqbpvdib.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.zdbjq.cn/Article/details/giekframf.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.blog.hesvh.cn/Article/details/guaqsvvqo.sHtML

Go:   len(arr);  len(m)
来源：http://3g.fehbvm.com/Article/details/gosmjvhcj.sHtML

Ruby: x.length;  x.size
来源：http://mobile.hesvh.cn/Article/details/gfzraxhpk.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://3g.fehbvm.com/Article/details/gbxnxeyja.sHtML

[P05] 判断两个对象内容是否相等
来源：http://blog.fehbvm.com/Article/details/gyinozodr.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://blog.zdbjq.cn/Article/details/gmnebpzxa.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://m.share.fehbvm.com/Article/details/gmztcyndo.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://blog.hesvh.cn/Article/details/gdytfxlie.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://3g.hesvh.cn/Article/details/gnxkbdohg.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://mobile.hesvh.cn/Article/details/gdqewktkr.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://blog.fehbvm.com/Article/details/geecapgck.sHtML

Ruby: a == b
来源：http://blog.fehbvm.com/Article/details/gfgswmjoq.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.m.share.fehbvm.com/Article/details/gvjqvolvz.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://m.share.zdbjq.cn/Article/details/gvzrohwtr.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.share.zdbjq.cn/Article/details/gqzifnutk.sHtML

PHP:  if (empty($x)) {}
来源：http://read.share.zdbjq.cn/Article/details/glhojtgbm.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://wap.fehbvm.com/Article/details/gillljwni.sHtML

TS:   if (x == null) {}
来源：http://baike.hesvh.cn/Article/details/gvdkllsnu.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://wap.fehbvm.com/Article/details/gavhznsxl.sHtML

Go:   if x == nil {}
来源：http://www.m.share.zdbjq.cn/Article/details/grequmtgl.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://blog.hesvh.cn/Article/details/gspabovtj.sHtML

C#:   if (x is null) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gxdjxkrsb.sHtML

[P07] 防抖与节流
来源：http://blog.fehbvm.com/Article/details/goodzcfgf.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.m.share.hesvh.cn/Article/details/gedfermdx.sHtML

PHP:  // 手写时间戳比较
来源：http://www.m.share.hesvh.cn/Article/details/gvpwffrsn.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.zdbjq.cn/Article/details/gqtmvfwcb.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.zdbjq.cn/Article/details/gblmvdxti.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://blog.hesvh.cn/Article/details/giydgnbwh.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.m.share.zdbjq.cn/Article/details/gwrjaifbp.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://read.share.hesvh.cn/Article/details/gwqpzpbnj.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://m.share.fehbvm.com/Article/details/gewpwbohl.sHtML

[P08] 处理浮点精度问题
来源：http://m.share.hesvh.cn/Article/details/gyhceapen.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://baike.zdbjq.cn/Article/details/garicfhxk.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://mobile.hesvh.cn/Article/details/ghiqsmyie.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://m.share.zdbjq.cn/Article/details/ghdrvkoqk.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://m.share.hesvh.cn/Article/details/gfxrlqube.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://wap.hesvh.cn/Article/details/gvazoxldx.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://mobile.hesvh.cn/Article/details/gvogqiyoe.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.share.hesvh.cn/Article/details/gvggavtvd.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://3g.zdbjq.cn/Article/details/gbcrkslfk.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/guydmxmcq.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://wap.fehbvm.com/Article/details/gwvolkwvj.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/ghnrxcfjm.sHtML

[Q01] 创建表
来源：http://www.blog.fehbvm.com/Article/details/gzmdssnoi.sHtML

CREATE TABLE users (
来源：http://m.share.fehbvm.com/Article/details/glogxotyy.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.hesvh.cn/Article/details/gueseicdk.sHtML

name VARCHAR(50) NOT NULL,
来源：http://blog.fehbvm.com/Article/details/gfkyurqzj.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.m.share.hesvh.cn/Article/details/gpuaoovej.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://mobile.zdbjq.cn/Article/details/gzztjkfpg.sHtML

);
来源：http://wap.fehbvm.com/Article/details/gizqbvvpc.sHtML

[Q02] 创建带外键的表
来源：http://www.share.hesvh.cn/Article/details/gmmvppkmf.sHtML

CREATE TABLE orders (
来源：http://www.blog.hesvh.cn/Article/details/grypzjtxh.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.zdbjq.cn/Article/details/gghmidvwk.sHtML

user_id INT NOT NULL,
来源：http://www.share.hesvh.cn/Article/details/ghibowwho.sHtML

amount DECIMAL(10, 2),
来源：http://www.blog.zdbjq.cn/Article/details/gvqdgnhbw.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://baike.hesvh.cn/Article/details/glcqdbksi.sHtML

);
来源：http://baike.fehbvm.com/Article/details/gczhxaghk.sHtML

[Q03] 增加列
来源：http://www.m.share.hesvh.cn/Article/details/ghmizujgu.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://3g.hesvh.cn/Article/details/gpvvezmtj.sHtML

[Q04] 修改列类型
来源：http://baike.fehbvm.com/Article/details/gtqgdpqex.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.share.fehbvm.com/Article/details/gjfiqnpgq.sHtML

[Q05] 重命名列
来源：http://baike.fehbvm.com/Article/details/gimxcqehf.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://baike.hesvh.cn/Article/details/gswzxlwpz.sHtML

[Q06] 删除列
来源：http://www.m.share.hesvh.cn/Article/details/ghjdpkexm.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.blog.zdbjq.cn/Article/details/gfkymqijw.sHtML

[Q07] 删除表
来源：http://wap.hesvh.cn/Article/details/gaxgbdfnj.sHtML

DROP TABLE IF EXISTS orders;
来源：http://mobile.zdbjq.cn/Article/details/gluvkfgwr.sHtML

[Q08] 创建普通索引
来源：http://mobile.zdbjq.cn/Article/details/gbwbbevcr.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.m.share.zdbjq.cn/Article/details/gtramdfoc.sHtML

[Q09] 创建唯一索引
来源：http://mobile.zdbjq.cn/Article/details/gcwhmlzho.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.share.zdbjq.cn/Article/details/gyqsozrwl.sHtML

[Q10] 插入单行
来源：http://read.share.hesvh.cn/Article/details/gtjtvgiwk.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://m.share.hesvh.cn/Article/details/glmllyrel.sHtML

[Q11] 一次插入多行
来源：http://read.share.zdbjq.cn/Article/details/gcjrwgvah.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://read.share.zdbjq.cn/Article/details/gomeabozf.sHtML

[Q12] 插入后取自增 ID
来源：http://3g.hesvh.cn/Article/details/glskbieju.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://m.share.fehbvm.com/Article/details/gxmupozje.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://3g.fehbvm.com/Article/details/gjeygqlyn.sHtML

[Q13] 忽略重复插入
来源：http://blog.fehbvm.com/Article/details/gighpxydd.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://blog.fehbvm.com/Article/details/gfucpuhwi.sHtML

[Q14] 存在则更新（upsert）
来源：http://wap.zdbjq.cn/Article/details/gjawzyizt.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://m.share.hesvh.cn/Article/details/gcsltiyuh.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://baike.hesvh.cn/Article/details/gfiqpqqkx.sHtML

[Q15] 查询全部
来源：http://mobile.fehbvm.com/Article/details/gyludpyqe.sHtML

SELECT * FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gbefubyxk.sHtML

[Q16] 查询指定列
来源：http://www.m.share.zdbjq.cn/Article/details/gqyzurtql.sHtML

SELECT id, name FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gvflrrbwc.sHtML

[Q17] 条件查询
来源：http://mobile.hesvh.cn/Article/details/gohjuqpgc.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://wap.zdbjq.cn/Article/details/gzhpjsbxn.sHtML

[Q18] 模糊匹配
来源：http://www.blog.zdbjq.cn/Article/details/gupirjvyz.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.blog.hesvh.cn/Article/details/gjrlqglpi.sHtML

[Q19] 范围查询
来源：http://3g.fehbvm.com/Article/details/gckkcflfb.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://baike.fehbvm.com/Article/details/gshbccjut.sHtML

[Q20] IN 列表
来源：http://www.blog.fehbvm.com/Article/details/gwlolngda.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.m.share.hesvh.cn/Article/details/gxypfssnu.sHtML

[Q21] 空值判断
来源：http://wap.fehbvm.com/Article/details/gpozwszwo.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://baike.fehbvm.com/Article/details/gadvebdim.sHtML

[Q22] 排序
来源：http://read.share.zdbjq.cn/Article/details/glscvwegf.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://m.share.fehbvm.com/Article/details/gwrponela.sHtML

[Q23] 分页
来源：http://blog.zdbjq.cn/Article/details/gugepexvh.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://3g.zdbjq.cn/Article/details/gwxqmtwzo.sHtML

[Q24] 去重
来源：http://mobile.fehbvm.com/Article/details/gvxsvtuyl.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/guicrjglh.sHtML

[Q25] 只取前 N 条
来源：http://mobile.hesvh.cn/Article/details/geecstgaa.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.blog.zdbjq.cn/Article/details/gerwwubcg.sHtML

[Q26] 计数
来源：http://wap.fehbvm.com/Article/details/gtushchel.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gqvfwxpjl.sHtML

[Q27] 条件计数
来源：http://baike.hesvh.cn/Article/details/ghfinpwhv.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://read.share.fehbvm.com/Article/details/gduunbsfs.sHtML

[Q28] 求和与平均
来源：http://m.share.fehbvm.com/Article/details/gasfqaydc.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.m.share.hesvh.cn/Article/details/giwanwgrn.sHtML

[Q29] 最大最小值
来源：http://3g.hesvh.cn/Article/details/guykicdms.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.share.hesvh.cn/Article/details/gxqcvgauk.sHtML

[Q30] 分组统计
来源：http://read.share.zdbjq.cn/Article/details/gwodtefzh.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.m.share.zdbjq.cn/Article/details/gfvdgjifu.sHtML

[Q31] 分组后过滤
来源：http://m.share.zdbjq.cn/Article/details/gemichkmc.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.m.share.zdbjq.cn/Article/details/gxmzufepj.sHtML

[Q32] 分组拼接字符串
来源：http://blog.zdbjq.cn/Article/details/gnztpgnsy.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://m.share.hesvh.cn/Article/details/gqmsbmrrf.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.m.share.fehbvm.com/Article/details/ghiqhhetu.sHtML

[Q33] 多列分组
来源：http://www.blog.hesvh.cn/Article/details/ghldugeft.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://mobile.fehbvm.com/Article/details/gutibbxph.sHtML

[Q34] 每组取第一条
来源：http://read.share.fehbvm.com/Article/details/ggvgmiczd.sHtML

SELECT * FROM (
来源：http://www.share.hesvh.cn/Article/details/getrcmiff.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://blog.fehbvm.com/Article/details/gdrqoljdm.sHtML

) t WHERE rn = 1;
来源：http://wap.hesvh.cn/Article/details/gfladclbi.sHtML

[Q35] 内连接
来源：http://wap.zdbjq.cn/Article/details/gkbilxyho.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://mobile.zdbjq.cn/Article/details/gamiuzdjz.sHtML

[Q36] 左连接
来源：http://mobile.fehbvm.com/Article/details/gwojqdxhs.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://blog.zdbjq.cn/Article/details/gzgsvfaql.sHtML

[Q37] 右连接
来源：http://baike.zdbjq.cn/Article/details/gqbphbbej.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.m.share.hesvh.cn/Article/details/gygoiosse.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://m.share.fehbvm.com/Article/details/gsjsdxzxn.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://3g.hesvh.cn/Article/details/giltwaons.sHtML

[Q39] 自连接（查上下级）
来源：http://read.share.zdbjq.cn/Article/details/gqrwxdrhp.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://wap.zdbjq.cn/Article/details/gdjcnbxrv.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://read.share.fehbvm.com/Article/details/glsyzhrtg.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://blog.hesvh.cn/Article/details/ghkkgoteb.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://read.share.fehbvm.com/Article/details/ghhjqywnm.sHtML

[Q41] 多表连接
来源：http://www.share.fehbvm.com/Article/details/gufbiqqnb.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.share.zdbjq.cn/Article/details/gizzxkchn.sHtML

JOIN users u ON u.id = o.user_id
来源：http://baike.fehbvm.com/Article/details/gbxepqjxz.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://wap.zdbjq.cn/Article/details/gvhgnpqby.sHtML

[Q42] 连接条件附加过滤
来源：http://www.m.share.zdbjq.cn/Article/details/gmdzycydi.sHtML

SELECT u.name, o.amount FROM users u
来源：http://3g.hesvh.cn/Article/details/gncktoxaz.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://mobile.fehbvm.com/Article/details/gizzupjze.sHtML

[Q43] 标量子查询
来源：http://read.share.zdbjq.cn/Article/details/gwcbwthzi.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.blog.fehbvm.com/Article/details/gxjbrcnta.sHtML

[Q44] IN 子查询
来源：http://www.share.hesvh.cn/Article/details/gmuaztkna.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.m.share.zdbjq.cn/Article/details/gwljvmuym.sHtML

[Q45] EXISTS 判断存在
来源：http://blog.zdbjq.cn/Article/details/gtbqvwyzj.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.hesvh.cn/Article/details/grqvpgzgp.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://3g.hesvh.cn/Article/details/gsibsagjv.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.fehbvm.com/Article/details/gcchelcsu.sHtML

[Q47] 与平均值比较
来源：http://blog.zdbjq.cn/Article/details/gflhanyac.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://wap.fehbvm.com/Article/details/gctnhqwpp.sHtML

[Q48] CTE 公用表表达式
来源：http://www.m.share.fehbvm.com/Article/details/gcuerueou.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://mobile.zdbjq.cn/Article/details/gxgfbngoi.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://wap.hesvh.cn/Article/details/gmtoafhwv.sHtML

[Q49] 更新单行
来源：http://read.share.fehbvm.com/Article/details/gjlseqzqi.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://3g.fehbvm.com/Article/details/gontgsuxf.sHtML

[Q50] 批量更新
来源：http://blog.hesvh.cn/Article/details/gkvyduvko.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.blog.zdbjq.cn/Article/details/gigjzhfpz.sHtML

[Q51] 用子查询更新
来源：http://read.share.fehbvm.com/Article/details/gjaeclzci.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://blog.fehbvm.com/Article/details/gmkcvfnox.sHtML

[Q52] 删除指定行
来源：http://wap.zdbjq.cn/Article/details/gnyazgxku.sHtML

DELETE FROM users WHERE id = 10;
来源：http://baike.fehbvm.com/Article/details/gwqhjjyhg.sHtML

[Q53] 按条件删除
来源：http://blog.fehbvm.com/Article/details/ghmojpzbi.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://3g.hesvh.cn/Article/details/gfrasuidv.sHtML

[Q54] 清空表
来源：http://3g.zdbjq.cn/Article/details/gmpisswdp.sHtML

TRUNCATE TABLE logs;
来源：http://read.share.zdbjq.cn/Article/details/gqmmjrfhm.sHtML

[Q55] 排名（并列占位）
来源：http://read.share.fehbvm.com/Article/details/gqryzdsmn.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://baike.zdbjq.cn/Article/details/gxjclzvfs.sHtML

[Q56] 密集排名（并列不占位）
来源：http://m.share.zdbjq.cn/Article/details/gwszflbid.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.m.share.zdbjq.cn/Article/details/giezeghxm.sHtML

[Q57] 行号
来源：http://3g.fehbvm.com/Article/details/grdelswah.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gywqdxudq.sHtML

[Q58] 累计求和
来源：http://www.m.share.zdbjq.cn/Article/details/grbkpuauw.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.share.fehbvm.com/Article/details/gucdzqmhf.sHtML

[Q59] 分组内累计
来源：http://baike.fehbvm.com/Article/details/gyyrlztjz.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://read.share.zdbjq.cn/Article/details/gmktxffhs.sHtML

[Q60] 取上一行 / 下一行
来源：http://3g.fehbvm.com/Article/details/gbkhskltm.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://wap.hesvh.cn/Article/details/gujhhlohu.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://m.share.hesvh.cn/Article/details/gyiorfxzq.sHtML

[Q61] 移动平均
来源：http://3g.zdbjq.cn/Article/details/gukhxhqde.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://blog.hesvh.cn/Article/details/gcpsvuyxj.sHtML

[Q62] 分组占比
来源：http://mobile.zdbjq.cn/Article/details/gwgxpekih.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://wap.hesvh.cn/Article/details/gxscpzmjv.sHtML

[Q63] 开启事务
来源：http://3g.fehbvm.com/Article/details/gpdahujzv.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://read.share.zdbjq.cn/Article/details/gmrdwjbay.sHtML

[Q64] 提交事务
来源：http://m.share.zdbjq.cn/Article/details/gpbxnxhrf.sHtML

COMMIT;
来源：http://read.share.fehbvm.com/Article/details/gfmdnddea.sHtML

[Q65] 回滚事务
来源：http://mobile.hesvh.cn/Article/details/ggldypmvg.sHtML

ROLLBACK;
来源：http://www.blog.zdbjq.cn/Article/details/ggzqwbjhz.sHtML

[Q66] 行锁查询
来源：http://www.blog.hesvh.cn/Article/details/gwqzybuig.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://blog.fehbvm.com/Article/details/gsqvawvoc.sHtML

[Q67] 设置隔离级别
来源：http://3g.zdbjq.cn/Article/details/gfhiquziq.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://m.share.zdbjq.cn/Article/details/gjiupanlz.sHtML

[Q68] 保存点
来源：http://www.share.hesvh.cn/Article/details/gptyelprd.sHtML

SAVEPOINT sp1;
来源：http://blog.zdbjq.cn/Article/details/gitidkqbi.sHtML

ROLLBACK TO sp1;
来源：http://www.blog.hesvh.cn/Article/details/gsrgkryyw.sHtML

[Q69] 查看执行计划
来源：http://www.m.share.zdbjq.cn/Article/details/gvcnfzrzn.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://wap.hesvh.cn/Article/details/gfqhohrwe.sHtML

[Q70] 更新统计信息
来源：http://www.blog.fehbvm.com/Article/details/gxrtaskxj.sHtML

ANALYZE TABLE users;
来源：http://m.share.zdbjq.cn/Article/details/ghxagnivk.sHtML

[Q71] 查看建表语句
来源：http://m.share.hesvh.cn/Article/details/giwetkiit.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.blog.fehbvm.com/Article/details/gploiejds.sHtML

[Q72] 查看索引
来源：http://m.share.hesvh.cn/Article/details/ghddvnusb.sHtML

SHOW INDEX FROM users;
来源：http://3g.hesvh.cn/Article/details/gaqkusphz.sHtML

[Q73] 查看表状态
来源：http://m.share.hesvh.cn/Article/details/gyhrshkri.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://blog.zdbjq.cn/Article/details/gdsluqlda.sHtML

[Q74] 强制使用索引
来源：http://www.m.share.fehbvm.com/Article/details/gzggroort.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.blog.hesvh.cn/Article/details/gwkkwplke.sHtML

[Q75] 日期格式化
来源：http://3g.zdbjq.cn/Article/details/guomrmtzp.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://mobile.hesvh.cn/Article/details/gqggatckm.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://read.share.hesvh.cn/Article/details/gdjqzhvme.sHtML

[Q76] 按天统计
来源：http://read.share.zdbjq.cn/Article/details/gnxmufzgc.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://m.share.zdbjq.cn/Article/details/gimbebqic.sHtML

[Q77] 时间加减
来源：http://read.share.hesvh.cn/Article/details/gkhtjxcpm.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://mobile.zdbjq.cn/Article/details/gjclnykbr.sHtML

[Q78] 当前时间
来源：http://www.share.fehbvm.com/Article/details/gfpfyavtd.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.share.zdbjq.cn/Article/details/gebnknaks.sHtML

[Q79] 字符串拼接
来源：http://read.share.zdbjq.cn/Article/details/ghrmrbjfm.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://read.share.zdbjq.cn/Article/details/gzwinrykh.sHtML

[Q80] 字符串截取
来源：http://www.share.hesvh.cn/Article/details/gmqtanydt.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://baike.fehbvm.com/Article/details/gdjmhdalr.sHtML

[Q81] 字符串替换
来源：http://www.blog.zdbjq.cn/Article/details/gklfdhdsr.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://wap.hesvh.cn/Article/details/geyckyqmb.sHtML

[Q82] 字符长度与字节长度
来源：http://www.m.share.fehbvm.com/Article/details/gmdpjzshc.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://blog.hesvh.cn/Article/details/ghvcaxsba.sHtML

[Q83] 大小写转换
来源：http://wap.hesvh.cn/Article/details/gycravzql.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://wap.hesvh.cn/Article/details/gmzdhgbmp.sHtML

[Q84] 去除首尾空格
来源：http://baike.hesvh.cn/Article/details/gfflfqyze.sHtML

SELECT TRIM(name) FROM users;
来源：http://mobile.fehbvm.com/Article/details/gliicwyaq.sHtML

[Q85] 数值取整
来源：http://www.share.zdbjq.cn/Article/details/gbnsiiuln.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.share.hesvh.cn/Article/details/gpgaljccm.sHtML

[Q86] 读取 JSON 字段
来源：http://blog.fehbvm.com/Article/details/ggbylxfhi.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://blog.hesvh.cn/Article/details/gsnnstwuf.sHtML

[Q87] JSON 字段做条件
来源：http://m.share.zdbjq.cn/Article/details/gmkincoyw.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://read.share.zdbjq.cn/Article/details/gmiptsjap.sHtML

[Q88] 行转列（条件聚合）
来源：http://m.share.fehbvm.com/Article/details/gpfkykvix.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.blog.zdbjq.cn/Article/details/gnpltkgib.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://m.share.fehbvm.com/Article/details/gmhcedecm.sHtML

[Q89] 判断表是否存在
来源：http://baike.zdbjq.cn/Article/details/gjhwkqysh.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.share.fehbvm.com/Article/details/gsjopjmli.sHtML

[Q90] 生成序号列
来源：http://www.m.share.zdbjq.cn/Article/details/glhsfkote.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.blog.hesvh.cn/Article/details/grefsofbh.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gfakkcmxl.sHtML

R. Bash 专题
来源：http://blog.hesvh.cn/Article/details/gzctilywd.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gokdbmpyr.sHtML

[R01] shebang 与严格模式
来源：http://wap.zdbjq.cn/Article/details/gwjjbplkn.sHtML

#!/usr/bin/env bash
来源：http://mobile.hesvh.cn/Article/details/gpyoasmjy.sHtML

set -euo pipefail
来源：http://www.blog.zdbjq.cn/Article/details/giaatakmr.sHtML

[R02] 变量赋值与使用
来源：http://read.share.fehbvm.com/Article/details/gmqwupywz.sHtML

name="Tom"; echo "$name"
来源：http://3g.fehbvm.com/Article/details/gldtqaeab.sHtML

[R03] 只读变量
来源：http://wap.zdbjq.cn/Article/details/ghalamuip.sHtML

readonly PI=3.14
来源：http://3g.fehbvm.com/Article/details/ghxknbuty.sHtML

[R04] 位置参数
来源：http://wap.fehbvm.com/Article/details/gmnzwedob.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://read.share.zdbjq.cn/Article/details/gsgkhdhzv.sHtML

[R05] 参数默认值
来源：http://baike.zdbjq.cn/Article/details/gniwpfhti.sHtML

name="${1:-default}"
来源：http://blog.zdbjq.cn/Article/details/gsqefemzn.sHtML

[R06] 判断命令是否存在
来源：http://www.share.fehbvm.com/Article/details/gxzjkshpb.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://read.share.hesvh.cn/Article/details/gtenzgamq.sHtML

[R07] if 判断文件
来源：http://3g.hesvh.cn/Article/details/gibkeknds.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://mobile.fehbvm.com/Article/details/gowrpkfey.sHtML

[R08] 数值比较
来源：http://www.blog.zdbjq.cn/Article/details/gkrgghobz.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://3g.zdbjq.cn/Article/details/gxbigofjs.sHtML

[R09] 字符串比较
来源：http://www.blog.zdbjq.cn/Article/details/grwgagrzx.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.blog.hesvh.cn/Article/details/gscjvhizh.sHtML

[R10] 正则匹配
来源：http://blog.zdbjq.cn/Article/details/gucrdalfu.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://read.share.zdbjq.cn/Article/details/gbiynoacj.sHtML

[R11] case 多分支
来源：http://baike.zdbjq.cn/Article/details/guzdlgtvd.sHtML

case "$1" in
来源：http://wap.fehbvm.com/Article/details/grvaugash.sHtML

start) echo "启动" ;;
来源：http://www.blog.hesvh.cn/Article/details/gvttyzere.sHtML

stop)  echo "停止" ;;
来源：http://baike.zdbjq.cn/Article/details/goejixqne.sHtML

*)     echo "未知命令" ;;
来源：http://mobile.fehbvm.com/Article/details/gprowjcre.sHtML

esac
来源：http://mobile.fehbvm.com/Article/details/gcfnxcghb.sHtML

[R12] for 遍历文件
来源：http://baike.hesvh.cn/Article/details/gesveusdy.sHtML

for f in *.txt; do echo "$f"; done
来源：http://3g.zdbjq.cn/Article/details/grikqevzx.sHtML

[R13] for 计数循环
来源：http://baike.hesvh.cn/Article/details/gmmjdcjaj.sHtML


<!-- 参考信息 -->