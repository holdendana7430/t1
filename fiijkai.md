代发 wailian999

C#:   Guid.NewGuid().ToString()
来源：http://blog.zdbjq.cn/Article/details/grhlfuwwh.sHtML

[P02] MD5 / SHA256 摘要
来源：http://m.share.hesvh.cn/Article/details/gezdxnyem.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.share.zdbjq.cn/Article/details/gehqxusmh.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://blog.fehbvm.com/Article/details/gjwlcprpv.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.blog.fehbvm.com/Article/details/gxszrhcob.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.blog.hesvh.cn/Article/details/gopdmewxm.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://mobile.hesvh.cn/Article/details/golndsgof.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://3g.zdbjq.cn/Article/details/gysfahays.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://3g.zdbjq.cn/Article/details/gtxugxitd.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://baike.fehbvm.com/Article/details/gibipisyt.sHtML

[P03] 生成短随机字符串
来源：http://3g.zdbjq.cn/Article/details/gyeamcxpf.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://3g.zdbjq.cn/Article/details/getfudsai.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://3g.fehbvm.com/Article/details/gebrkaelr.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.fehbvm.com/Article/details/gnlcpzjcl.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.fehbvm.com/Article/details/geultrokm.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://baike.zdbjq.cn/Article/details/gehrnsxln.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://m.share.zdbjq.cn/Article/details/gfjreowzj.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://baike.hesvh.cn/Article/details/ggthvptyt.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://read.share.fehbvm.com/Article/details/gjtblowwv.sHtML

[P04] 求长度
来源：http://www.m.share.hesvh.cn/Article/details/ggxaocvhy.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.blog.fehbvm.com/Article/details/gdepygnpw.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.fehbvm.com/Article/details/ghyaxesds.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.fehbvm.com/Article/details/geowokafc.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.fehbvm.com/Article/details/guraofwxw.sHtML

Java: list.size();  map.size();  s.length()
来源：http://m.share.zdbjq.cn/Article/details/glvooikgf.sHtML

Go:   len(arr);  len(m)
来源：http://m.share.zdbjq.cn/Article/details/gixjorhfd.sHtML

Ruby: x.length;  x.size
来源：http://wap.fehbvm.com/Article/details/glowqhtrj.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://3g.fehbvm.com/Article/details/gtbnwzlfh.sHtML

[P05] 判断两个对象内容是否相等
来源：http://read.share.zdbjq.cn/Article/details/gryqzlsjm.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://baike.hesvh.cn/Article/details/gfgodngou.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://m.share.hesvh.cn/Article/details/gwddnyosa.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://baike.zdbjq.cn/Article/details/gskbkdwda.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://read.share.fehbvm.com/Article/details/goykjyslj.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.blog.zdbjq.cn/Article/details/gimcjfgtl.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://mobile.hesvh.cn/Article/details/gfzukcsry.sHtML

Ruby: a == b
来源：http://www.share.hesvh.cn/Article/details/gievceike.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.share.zdbjq.cn/Article/details/gdfocwmvt.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.m.share.fehbvm.com/Article/details/gcpetyzpv.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.m.share.zdbjq.cn/Article/details/grxlhdhcn.sHtML

PHP:  if (empty($x)) {}
来源：http://blog.zdbjq.cn/Article/details/glxjxljkf.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.blog.fehbvm.com/Article/details/gwemfvjfg.sHtML

TS:   if (x == null) {}
来源：http://wap.fehbvm.com/Article/details/gosgmnrup.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://blog.hesvh.cn/Article/details/gdlhzgwvf.sHtML

Go:   if x == nil {}
来源：http://mobile.hesvh.cn/Article/details/gqpfxtdlv.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://m.share.zdbjq.cn/Article/details/gtojqynxx.sHtML

C#:   if (x is null) {}
来源：http://www.m.share.hesvh.cn/Article/details/gsvuhuqfj.sHtML

[P07] 防抖与节流
来源：http://m.share.fehbvm.com/Article/details/gkaqnqiro.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://wap.hesvh.cn/Article/details/gxpirqrbs.sHtML

PHP:  // 手写时间戳比较
来源：http://blog.hesvh.cn/Article/details/gkoplspgu.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.hesvh.cn/Article/details/gndhdvltu.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.hesvh.cn/Article/details/ghxgtcqan.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.blog.fehbvm.com/Article/details/gmftjhwtt.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://baike.hesvh.cn/Article/details/gwpqjzrmc.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.share.fehbvm.com/Article/details/gxdlgcayt.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://mobile.fehbvm.com/Article/details/gqqcyqccp.sHtML

[P08] 处理浮点精度问题
来源：http://mobile.zdbjq.cn/Article/details/gdntdybkp.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.blog.zdbjq.cn/Article/details/gqkmvortg.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.share.hesvh.cn/Article/details/gjeofdybc.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://m.share.zdbjq.cn/Article/details/gyigcaocu.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://read.share.zdbjq.cn/Article/details/gelgxjuda.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://blog.fehbvm.com/Article/details/gttjvphit.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://mobile.zdbjq.cn/Article/details/gxzgpjsrv.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.blog.zdbjq.cn/Article/details/gvkdakeru.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://read.share.fehbvm.com/Article/details/gvjzimccu.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gxnstvnox.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.blog.zdbjq.cn/Article/details/ghiwdywjy.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/garglxyee.sHtML

[Q01] 创建表
来源：http://mobile.fehbvm.com/Article/details/gbtuhrium.sHtML

CREATE TABLE users (
来源：http://www.share.hesvh.cn/Article/details/grppoevab.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.hesvh.cn/Article/details/gqthuuvoj.sHtML

name VARCHAR(50) NOT NULL,
来源：http://m.share.zdbjq.cn/Article/details/gwjofzscm.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.m.share.hesvh.cn/Article/details/gbrcvgzre.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://wap.zdbjq.cn/Article/details/gklirzsru.sHtML

);
来源：http://baike.zdbjq.cn/Article/details/gkysopibf.sHtML

[Q02] 创建带外键的表
来源：http://blog.hesvh.cn/Article/details/gdlnypvqu.sHtML

CREATE TABLE orders (
来源：http://baike.fehbvm.com/Article/details/ghlaejxgj.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.hesvh.cn/Article/details/guzxschfb.sHtML

user_id INT NOT NULL,
来源：http://m.share.zdbjq.cn/Article/details/ggqkuzgus.sHtML

amount DECIMAL(10, 2),
来源：http://blog.fehbvm.com/Article/details/gpaebtjmf.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.m.share.zdbjq.cn/Article/details/goorqhdmr.sHtML

);
来源：http://www.blog.zdbjq.cn/Article/details/gwkdjnosx.sHtML

[Q03] 增加列
来源：http://baike.fehbvm.com/Article/details/gwlkwmgoq.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://mobile.hesvh.cn/Article/details/gcwknmsrk.sHtML

[Q04] 修改列类型
来源：http://3g.zdbjq.cn/Article/details/gwjbnaehm.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.blog.fehbvm.com/Article/details/gcdvsksdj.sHtML

[Q05] 重命名列
来源：http://m.share.zdbjq.cn/Article/details/gsacgclkr.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://read.share.fehbvm.com/Article/details/grwzdnmut.sHtML

[Q06] 删除列
来源：http://m.share.fehbvm.com/Article/details/gmekngskd.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://m.share.hesvh.cn/Article/details/gxfzmcyes.sHtML

[Q07] 删除表
来源：http://baike.fehbvm.com/Article/details/glwbhtafk.sHtML

DROP TABLE IF EXISTS orders;
来源：http://wap.hesvh.cn/Article/details/gcphigjdg.sHtML

[Q08] 创建普通索引
来源：http://m.share.zdbjq.cn/Article/details/glyccqerm.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://blog.hesvh.cn/Article/details/ghrsgsget.sHtML

[Q09] 创建唯一索引
来源：http://m.share.zdbjq.cn/Article/details/gvccgmnum.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://baike.hesvh.cn/Article/details/goeuvthhf.sHtML

[Q10] 插入单行
来源：http://www.share.hesvh.cn/Article/details/gcmdptily.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.share.hesvh.cn/Article/details/gecvfmbaq.sHtML

[Q11] 一次插入多行
来源：http://3g.hesvh.cn/Article/details/gatogmkxn.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://mobile.hesvh.cn/Article/details/gcntsxzzc.sHtML

[Q12] 插入后取自增 ID
来源：http://www.blog.fehbvm.com/Article/details/gzcfexdwv.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.share.hesvh.cn/Article/details/ggdpevvbg.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://baike.hesvh.cn/Article/details/gsxgkdvan.sHtML

[Q13] 忽略重复插入
来源：http://blog.fehbvm.com/Article/details/grjfphrpb.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.m.share.fehbvm.com/Article/details/gunqllwyn.sHtML

[Q14] 存在则更新（upsert）
来源：http://blog.fehbvm.com/Article/details/gtzwlvuou.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://mobile.fehbvm.com/Article/details/gxgopmrbw.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.share.fehbvm.com/Article/details/gwcvfwqet.sHtML

[Q15] 查询全部
来源：http://wap.fehbvm.com/Article/details/gdptjvyqb.sHtML

SELECT * FROM users;
来源：http://3g.zdbjq.cn/Article/details/gteoruofc.sHtML

[Q16] 查询指定列
来源：http://3g.zdbjq.cn/Article/details/gxtahwxwq.sHtML

SELECT id, name FROM users;
来源：http://m.share.hesvh.cn/Article/details/gxcaufvad.sHtML

[Q17] 条件查询
来源：http://read.share.zdbjq.cn/Article/details/gsonucowc.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://baike.hesvh.cn/Article/details/gxhammdee.sHtML

[Q18] 模糊匹配
来源：http://www.blog.zdbjq.cn/Article/details/gupykkcob.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://m.share.zdbjq.cn/Article/details/gcvdultte.sHtML

[Q19] 范围查询
来源：http://www.share.fehbvm.com/Article/details/gfbykgyyj.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://mobile.hesvh.cn/Article/details/gwcitkrgm.sHtML

[Q20] IN 列表
来源：http://mobile.hesvh.cn/Article/details/gejsreqtr.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://m.share.zdbjq.cn/Article/details/gkuakzujy.sHtML

[Q21] 空值判断
来源：http://m.share.hesvh.cn/Article/details/gticziihn.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://read.share.hesvh.cn/Article/details/gwtcgfeol.sHtML

[Q22] 排序
来源：http://read.share.fehbvm.com/Article/details/gqeguihse.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.share.fehbvm.com/Article/details/ggeseaowd.sHtML

[Q23] 分页
来源：http://m.share.fehbvm.com/Article/details/gfnqrkpus.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://blog.fehbvm.com/Article/details/gbqneqyfc.sHtML

[Q24] 去重
来源：http://www.share.fehbvm.com/Article/details/gocusqmoi.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gncmdmoor.sHtML

[Q25] 只取前 N 条
来源：http://wap.zdbjq.cn/Article/details/ggmblwefq.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://read.share.zdbjq.cn/Article/details/gkyabtkwu.sHtML

[Q26] 计数
来源：http://mobile.fehbvm.com/Article/details/gtvvkqufd.sHtML

SELECT COUNT(*) FROM users;
来源：http://baike.fehbvm.com/Article/details/gwthtsyja.sHtML

[Q27] 条件计数
来源：http://www.m.share.fehbvm.com/Article/details/goblgjiwa.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://read.share.hesvh.cn/Article/details/gpcreltdo.sHtML

[Q28] 求和与平均
来源：http://3g.zdbjq.cn/Article/details/gjadeoahp.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://blog.zdbjq.cn/Article/details/gwbcjafds.sHtML

[Q29] 最大最小值
来源：http://www.m.share.hesvh.cn/Article/details/gkvyjcvnk.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gfgsjswfe.sHtML

[Q30] 分组统计
来源：http://3g.fehbvm.com/Article/details/gojeynydq.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.share.hesvh.cn/Article/details/gewcjaipb.sHtML

[Q31] 分组后过滤
来源：http://www.share.fehbvm.com/Article/details/gbofjcixs.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://m.share.zdbjq.cn/Article/details/gnhttfweo.sHtML

[Q32] 分组拼接字符串
来源：http://read.share.zdbjq.cn/Article/details/gyadrbcdx.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://mobile.zdbjq.cn/Article/details/godcuotxj.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://wap.fehbvm.com/Article/details/gnjljlayn.sHtML

[Q33] 多列分组
来源：http://read.share.zdbjq.cn/Article/details/gzghnmuyb.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://blog.fehbvm.com/Article/details/gjmxabuhz.sHtML

[Q34] 每组取第一条
来源：http://wap.fehbvm.com/Article/details/glheobpyl.sHtML

SELECT * FROM (
来源：http://mobile.hesvh.cn/Article/details/gtcdegzxl.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.share.hesvh.cn/Article/details/gopkptblk.sHtML

) t WHERE rn = 1;
来源：http://read.share.zdbjq.cn/Article/details/gdmupttxs.sHtML

[Q35] 内连接
来源：http://baike.zdbjq.cn/Article/details/grpgjncyv.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.zdbjq.cn/Article/details/gnodgocva.sHtML

[Q36] 左连接
来源：http://read.share.fehbvm.com/Article/details/gjhjijmko.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://m.share.fehbvm.com/Article/details/gzoncynbt.sHtML

[Q37] 右连接
来源：http://www.share.zdbjq.cn/Article/details/gigeelsnt.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://m.share.zdbjq.cn/Article/details/gikgqklcx.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://wap.fehbvm.com/Article/details/ggbwojflg.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.share.fehbvm.com/Article/details/gizphgoco.sHtML

[Q39] 自连接（查上下级）
来源：http://3g.fehbvm.com/Article/details/grwmbcwez.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.share.zdbjq.cn/Article/details/gyjwrpbtn.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.blog.zdbjq.cn/Article/details/gwigbozsw.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.blog.zdbjq.cn/Article/details/gaegxqxaz.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.m.share.fehbvm.com/Article/details/gxladljeo.sHtML

[Q41] 多表连接
来源：http://m.share.hesvh.cn/Article/details/gjffnyjuq.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://wap.hesvh.cn/Article/details/ggfypgckz.sHtML

JOIN users u ON u.id = o.user_id
来源：http://baike.fehbvm.com/Article/details/grlccstpb.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://read.share.hesvh.cn/Article/details/gnnrmktdt.sHtML

[Q42] 连接条件附加过滤
来源：http://m.share.zdbjq.cn/Article/details/gycuadcfe.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.m.share.zdbjq.cn/Article/details/grpzohtmf.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://baike.fehbvm.com/Article/details/gqucqvfma.sHtML

[Q43] 标量子查询
来源：http://m.share.hesvh.cn/Article/details/guqjxfscv.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.blog.hesvh.cn/Article/details/gitcjbrpj.sHtML

[Q44] IN 子查询
来源：http://baike.fehbvm.com/Article/details/gryrwbbko.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://3g.hesvh.cn/Article/details/gawosoekg.sHtML

[Q45] EXISTS 判断存在
来源：http://read.share.hesvh.cn/Article/details/gdrksomrv.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.hesvh.cn/Article/details/gydpbwokf.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://blog.zdbjq.cn/Article/details/gjrdaomib.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.fehbvm.com/Article/details/gtimliwqv.sHtML

[Q47] 与平均值比较
来源：http://mobile.hesvh.cn/Article/details/gfmwtwumh.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://3g.fehbvm.com/Article/details/gkbqrbprw.sHtML

[Q48] CTE 公用表表达式
来源：http://www.m.share.hesvh.cn/Article/details/gxptieacp.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://mobile.hesvh.cn/Article/details/gsxjjhdux.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.m.share.zdbjq.cn/Article/details/gsvgjmzon.sHtML

[Q49] 更新单行
来源：http://baike.fehbvm.com/Article/details/gbseqgucm.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://blog.hesvh.cn/Article/details/gczyyrcfo.sHtML

[Q50] 批量更新
来源：http://www.m.share.hesvh.cn/Article/details/gvjzyavet.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://read.share.hesvh.cn/Article/details/gopwbjnxu.sHtML

[Q51] 用子查询更新
来源：http://www.m.share.fehbvm.com/Article/details/gpepbpisu.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://read.share.hesvh.cn/Article/details/gohozwawu.sHtML

[Q52] 删除指定行
来源：http://m.share.hesvh.cn/Article/details/grpmefvow.sHtML

DELETE FROM users WHERE id = 10;
来源：http://baike.zdbjq.cn/Article/details/gmnwsdfnx.sHtML

[Q53] 按条件删除
来源：http://www.share.hesvh.cn/Article/details/gfdpjghca.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://read.share.hesvh.cn/Article/details/gdoqvdnmo.sHtML

[Q54] 清空表
来源：http://www.blog.fehbvm.com/Article/details/gjuyfeafs.sHtML

TRUNCATE TABLE logs;
来源：http://m.share.fehbvm.com/Article/details/gwncssgdu.sHtML

[Q55] 排名（并列占位）
来源：http://www.blog.fehbvm.com/Article/details/gonsnqhdb.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://mobile.hesvh.cn/Article/details/gpuaglvnb.sHtML

[Q56] 密集排名（并列不占位）
来源：http://baike.fehbvm.com/Article/details/gmudaqviu.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://blog.fehbvm.com/Article/details/gsqslnvmm.sHtML

[Q57] 行号
来源：http://blog.fehbvm.com/Article/details/gicjxqljh.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://3g.zdbjq.cn/Article/details/gxpgqxhnt.sHtML

[Q58] 累计求和
来源：http://m.share.fehbvm.com/Article/details/gfwexghlu.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.share.zdbjq.cn/Article/details/ghfutwwmj.sHtML

[Q59] 分组内累计
来源：http://www.blog.zdbjq.cn/Article/details/giexmvhho.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://3g.hesvh.cn/Article/details/gvtyctsew.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.blog.zdbjq.cn/Article/details/gwohgzuvm.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.m.share.fehbvm.com/Article/details/gkpilayqq.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://m.share.zdbjq.cn/Article/details/glpmrknqe.sHtML

[Q61] 移动平均
来源：http://baike.fehbvm.com/Article/details/ghicbdfti.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://m.share.fehbvm.com/Article/details/gfkirwskf.sHtML

[Q62] 分组占比
来源：http://wap.hesvh.cn/Article/details/glzvgmvmb.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.blog.hesvh.cn/Article/details/gkpkzuxjf.sHtML

[Q63] 开启事务
来源：http://mobile.fehbvm.com/Article/details/glnzevpxb.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://baike.hesvh.cn/Article/details/gozcncoyr.sHtML

[Q64] 提交事务
来源：http://wap.zdbjq.cn/Article/details/gycvglakj.sHtML

COMMIT;
来源：http://www.share.zdbjq.cn/Article/details/gdwrrcqet.sHtML

[Q65] 回滚事务
来源：http://blog.fehbvm.com/Article/details/ghelizpgd.sHtML

ROLLBACK;
来源：http://wap.fehbvm.com/Article/details/goswmivfs.sHtML

[Q66] 行锁查询
来源：http://3g.fehbvm.com/Article/details/gznjyhpgw.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.share.zdbjq.cn/Article/details/gzcfcwbfc.sHtML

[Q67] 设置隔离级别
来源：http://mobile.fehbvm.com/Article/details/gmjlroomh.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.blog.fehbvm.com/Article/details/gjyrwuxez.sHtML

[Q68] 保存点
来源：http://blog.fehbvm.com/Article/details/gouertbou.sHtML

SAVEPOINT sp1;
来源：http://www.blog.hesvh.cn/Article/details/gadlhctjk.sHtML

ROLLBACK TO sp1;
来源：http://www.m.share.fehbvm.com/Article/details/gqvshqgvm.sHtML

[Q69] 查看执行计划
来源：http://3g.fehbvm.com/Article/details/gnnpunvcm.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://m.share.hesvh.cn/Article/details/gxwesuria.sHtML

[Q70] 更新统计信息
来源：http://read.share.hesvh.cn/Article/details/gbvbtieoc.sHtML

ANALYZE TABLE users;
来源：http://3g.hesvh.cn/Article/details/ggwfphaps.sHtML

[Q71] 查看建表语句
来源：http://m.share.fehbvm.com/Article/details/gfmktvfmt.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.m.share.hesvh.cn/Article/details/gomwgbebd.sHtML

[Q72] 查看索引
来源：http://www.m.share.fehbvm.com/Article/details/geqcfljah.sHtML

SHOW INDEX FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gscsmarnc.sHtML

[Q73] 查看表状态
来源：http://baike.zdbjq.cn/Article/details/gqukmnpwp.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://blog.zdbjq.cn/Article/details/gxluwcnfq.sHtML

[Q74] 强制使用索引
来源：http://m.share.fehbvm.com/Article/details/gsadksuui.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://m.share.fehbvm.com/Article/details/gfzagxzrs.sHtML

[Q75] 日期格式化
来源：http://wap.hesvh.cn/Article/details/ghrxhxqoo.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://read.share.fehbvm.com/Article/details/grknacdiz.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://baike.fehbvm.com/Article/details/gyhsxlswa.sHtML

[Q76] 按天统计
来源：http://m.share.fehbvm.com/Article/details/gzhcoyhau.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://blog.zdbjq.cn/Article/details/gkcnmkanr.sHtML

[Q77] 时间加减
来源：http://www.m.share.fehbvm.com/Article/details/geltxzbmi.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://3g.hesvh.cn/Article/details/gznxwlfxa.sHtML

[Q78] 当前时间
来源：http://blog.zdbjq.cn/Article/details/gjgbnvtyu.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.m.share.fehbvm.com/Article/details/ghzzfvfpx.sHtML

[Q79] 字符串拼接
来源：http://blog.fehbvm.com/Article/details/gasbfyooa.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://baike.fehbvm.com/Article/details/grsdofvdm.sHtML

[Q80] 字符串截取
来源：http://blog.zdbjq.cn/Article/details/gzomcstqs.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://wap.hesvh.cn/Article/details/gzttsvbqp.sHtML

[Q81] 字符串替换
来源：http://mobile.hesvh.cn/Article/details/gjrijazly.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gwatiwmfx.sHtML

[Q82] 字符长度与字节长度
来源：http://baike.zdbjq.cn/Article/details/govwciogk.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://3g.fehbvm.com/Article/details/gclscodqv.sHtML

[Q83] 大小写转换
来源：http://www.blog.fehbvm.com/Article/details/guxfpmymk.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://3g.hesvh.cn/Article/details/grexyapdz.sHtML

[Q84] 去除首尾空格
来源：http://blog.hesvh.cn/Article/details/gsbvgkzvz.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gmilbwykk.sHtML

[Q85] 数值取整
来源：http://mobile.hesvh.cn/Article/details/grftnbjlx.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://mobile.hesvh.cn/Article/details/gewhsnvjk.sHtML

[Q86] 读取 JSON 字段
来源：http://read.share.hesvh.cn/Article/details/gkreaaniv.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://mobile.hesvh.cn/Article/details/guqztbnvh.sHtML

[Q87] JSON 字段做条件
来源：http://3g.zdbjq.cn/Article/details/gaifsdpbc.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://blog.zdbjq.cn/Article/details/gqwfnpygu.sHtML

[Q88] 行转列（条件聚合）
来源：http://mobile.hesvh.cn/Article/details/gxgqfpxqc.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.m.share.hesvh.cn/Article/details/gytztjrld.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.share.hesvh.cn/Article/details/gmhjrohpw.sHtML

[Q89] 判断表是否存在
来源：http://blog.hesvh.cn/Article/details/glffzftkp.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.share.zdbjq.cn/Article/details/gvfdwrekq.sHtML

[Q90] 生成序号列
来源：http://blog.hesvh.cn/Article/details/gmcbgttgy.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://wap.hesvh.cn/Article/details/gnmsvcmrg.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gmcslqmcw.sHtML

R. Bash 专题
来源：http://m.share.fehbvm.com/Article/details/gdiavqjoh.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gabivhkzq.sHtML

[R01] shebang 与严格模式
来源：http://www.blog.fehbvm.com/Article/details/glczaipch.sHtML

#!/usr/bin/env bash
来源：http://www.m.share.fehbvm.com/Article/details/gyrqicnxh.sHtML

set -euo pipefail
来源：http://www.blog.hesvh.cn/Article/details/gpoprqqvn.sHtML

[R02] 变量赋值与使用
来源：http://m.share.hesvh.cn/Article/details/gfwlrvdge.sHtML

name="Tom"; echo "$name"
来源：http://mobile.hesvh.cn/Article/details/gjbbpacxd.sHtML

[R03] 只读变量
来源：http://www.blog.fehbvm.com/Article/details/gzsjwmljc.sHtML

readonly PI=3.14
来源：http://3g.fehbvm.com/Article/details/gsjpfgucw.sHtML

[R04] 位置参数
来源：http://read.share.hesvh.cn/Article/details/grjgaielz.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.share.hesvh.cn/Article/details/gumwoijwg.sHtML

[R05] 参数默认值
来源：http://mobile.hesvh.cn/Article/details/gcwcuggdq.sHtML

name="${1:-default}"
来源：http://mobile.fehbvm.com/Article/details/gyndngjly.sHtML

[R06] 判断命令是否存在
来源：http://wap.hesvh.cn/Article/details/gksybjqaw.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://blog.fehbvm.com/Article/details/gdgugrqkb.sHtML

[R07] if 判断文件
来源：http://wap.fehbvm.com/Article/details/gplcizidr.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://baike.hesvh.cn/Article/details/gahqmvbji.sHtML

[R08] 数值比较
来源：http://baike.hesvh.cn/Article/details/gxjbfzuqd.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://3g.fehbvm.com/Article/details/glqjfxhvw.sHtML

[R09] 字符串比较
来源：http://wap.fehbvm.com/Article/details/gocgeuslu.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://mobile.zdbjq.cn/Article/details/gdlfvvxot.sHtML

[R10] 正则匹配
来源：http://www.blog.zdbjq.cn/Article/details/gubzelidq.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://baike.hesvh.cn/Article/details/gzadxbgki.sHtML

[R11] case 多分支
来源：http://www.blog.hesvh.cn/Article/details/ghokotfzm.sHtML

case "$1" in
来源：http://mobile.zdbjq.cn/Article/details/gjkbmcyvi.sHtML

start) echo "启动" ;;
来源：http://blog.hesvh.cn/Article/details/gcsaexxgo.sHtML

stop)  echo "停止" ;;
来源：http://www.blog.zdbjq.cn/Article/details/gfpewvzpp.sHtML

*)     echo "未知命令" ;;
来源：http://www.share.fehbvm.com/Article/details/gmieuiznv.sHtML


<!-- 参考信息 -->