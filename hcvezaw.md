代发 wailian999

[P01] 生成 UUID
来源：http://3g.hesvh.cn/Article/details/gfemghwgt.sHtML

Py:   str(uuid.uuid4())
来源：http://www.blog.hesvh.cn/Article/details/ggfajyfnz.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://wap.hesvh.cn/Article/details/gkpijycol.sHtML

JS:   crypto.randomUUID()
来源：http://baike.hesvh.cn/Article/details/grojkvxwn.sHtML

TS:   crypto.randomUUID()
来源：http://m.share.zdbjq.cn/Article/details/gppvmnupz.sHtML

Java: UUID.randomUUID().toString()
来源：http://blog.hesvh.cn/Article/details/gbqpzhvga.sHtML

Go:   // 用 github.com/google/uuid
来源：http://blog.fehbvm.com/Article/details/gsgjxrvch.sHtML

Ruby: SecureRandom.uuid
来源：http://mobile.zdbjq.cn/Article/details/gjyrlsbij.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://m.share.fehbvm.com/Article/details/gobqgrznf.sHtML

[P02] MD5 / SHA256 摘要
来源：http://wap.fehbvm.com/Article/details/gkjsdrhes.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://3g.zdbjq.cn/Article/details/gkgsbukdu.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://3g.fehbvm.com/Article/details/gkhhnlonq.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://3g.hesvh.cn/Article/details/gvpqjsttq.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.share.hesvh.cn/Article/details/glxourmwm.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://wap.hesvh.cn/Article/details/gepwtqxcj.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.m.share.fehbvm.com/Article/details/gbscikluv.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://baike.fehbvm.com/Article/details/gjbuverak.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://m.share.zdbjq.cn/Article/details/gywllhkck.sHtML

[P03] 生成短随机字符串
来源：http://baike.fehbvm.com/Article/details/gpbzeckfj.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.share.zdbjq.cn/Article/details/ghfuoxcbu.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.share.hesvh.cn/Article/details/grfvwgayx.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.zdbjq.cn/Article/details/gxezcpqrr.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.fehbvm.com/Article/details/gcnbqnazx.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.m.share.hesvh.cn/Article/details/gsjgangtu.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://read.share.hesvh.cn/Article/details/gazxojkia.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://baike.fehbvm.com/Article/details/gqtwpsqrn.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://wap.fehbvm.com/Article/details/gcqyvdcvn.sHtML

[P04] 求长度
来源：http://www.m.share.hesvh.cn/Article/details/gziialoyy.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://3g.fehbvm.com/Article/details/gjsewuhhf.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.share.hesvh.cn/Article/details/ggirsynvh.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.hesvh.cn/Article/details/gcmpvcezw.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.zdbjq.cn/Article/details/glckqpwky.sHtML

Java: list.size();  map.size();  s.length()
来源：http://m.share.fehbvm.com/Article/details/gkpiwnkli.sHtML

Go:   len(arr);  len(m)
来源：http://www.blog.fehbvm.com/Article/details/gqtqvdafv.sHtML

Ruby: x.length;  x.size
来源：http://www.m.share.hesvh.cn/Article/details/gqexlceip.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.share.hesvh.cn/Article/details/gveoljrex.sHtML

[P05] 判断两个对象内容是否相等
来源：http://read.share.hesvh.cn/Article/details/gkrspvctx.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://mobile.hesvh.cn/Article/details/gczsoiapy.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://baike.hesvh.cn/Article/details/gigaxwddw.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://blog.zdbjq.cn/Article/details/gammjmqdc.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://m.share.fehbvm.com/Article/details/gkgxkfvrz.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://baike.zdbjq.cn/Article/details/gnmquehxf.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://mobile.hesvh.cn/Article/details/gxxeumsie.sHtML

Ruby: a == b
来源：http://blog.zdbjq.cn/Article/details/gneexfieu.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://mobile.hesvh.cn/Article/details/gpltemmps.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://m.share.fehbvm.com/Article/details/gdirovpzv.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://mobile.hesvh.cn/Article/details/gaogngtpg.sHtML

PHP:  if (empty($x)) {}
来源：http://3g.hesvh.cn/Article/details/ggplmjddb.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.m.share.zdbjq.cn/Article/details/gwucqppkz.sHtML

TS:   if (x == null) {}
来源：http://wap.fehbvm.com/Article/details/gutqnbago.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://blog.hesvh.cn/Article/details/gmjzemeqb.sHtML

Go:   if x == nil {}
来源：http://wap.zdbjq.cn/Article/details/gzsmacfld.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://baike.hesvh.cn/Article/details/gasicyieh.sHtML

C#:   if (x is null) {}
来源：http://www.share.fehbvm.com/Article/details/gkumvxnth.sHtML

[P07] 防抖与节流
来源：http://wap.fehbvm.com/Article/details/glhdorijk.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.share.hesvh.cn/Article/details/gyfmhkkhi.sHtML

PHP:  // 手写时间戳比较
来源：http://blog.hesvh.cn/Article/details/gkmzsjvfm.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.fehbvm.com/Article/details/gqdwxfnal.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.fehbvm.com/Article/details/gaptmqxsf.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://m.share.fehbvm.com/Article/details/gfovjvyyt.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://wap.fehbvm.com/Article/details/ggnwundfk.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://read.share.hesvh.cn/Article/details/gsptfufyv.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://blog.zdbjq.cn/Article/details/gdqlttdym.sHtML

[P08] 处理浮点精度问题
来源：http://blog.zdbjq.cn/Article/details/gcycbuumk.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://m.share.fehbvm.com/Article/details/gvxwzmbvg.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://mobile.fehbvm.com/Article/details/geuawqvev.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://3g.fehbvm.com/Article/details/gflnuoexa.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://m.share.fehbvm.com/Article/details/gvevvbilk.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://m.share.hesvh.cn/Article/details/gdhjhphhc.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://blog.hesvh.cn/Article/details/gwpxfhzld.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.m.share.hesvh.cn/Article/details/gezbhzxbb.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://mobile.zdbjq.cn/Article/details/gddjtlvdp.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/grgezorfi.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.blog.fehbvm.com/Article/details/gzpspvbrr.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gbbjoerwy.sHtML

[Q01] 创建表
来源：http://www.m.share.zdbjq.cn/Article/details/guezfpubn.sHtML

CREATE TABLE users (
来源：http://3g.fehbvm.com/Article/details/gtnmsiecj.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.hesvh.cn/Article/details/gfndwvkfw.sHtML

name VARCHAR(50) NOT NULL,
来源：http://wap.zdbjq.cn/Article/details/gzcnaoodn.sHtML

email VARCHAR(100) UNIQUE,
来源：http://baike.hesvh.cn/Article/details/gqdpyxxvf.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://read.share.fehbvm.com/Article/details/gfsmtlmnz.sHtML

);
来源：http://blog.fehbvm.com/Article/details/gehesmqoq.sHtML

[Q02] 创建带外键的表
来源：http://www.m.share.fehbvm.com/Article/details/glrvguzec.sHtML

CREATE TABLE orders (
来源：http://www.blog.zdbjq.cn/Article/details/gkzvttwoq.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.share.hesvh.cn/Article/details/gcbykceoj.sHtML

user_id INT NOT NULL,
来源：http://wap.hesvh.cn/Article/details/gmdsqsqor.sHtML

amount DECIMAL(10, 2),
来源：http://blog.fehbvm.com/Article/details/gmtuuimfl.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.share.hesvh.cn/Article/details/gakpusbpg.sHtML

);
来源：http://wap.zdbjq.cn/Article/details/gbpoyeuqh.sHtML

[Q03] 增加列
来源：http://3g.fehbvm.com/Article/details/gelooqnii.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://mobile.fehbvm.com/Article/details/gukszfqcs.sHtML

[Q04] 修改列类型
来源：http://wap.fehbvm.com/Article/details/gtpoqatjj.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://wap.zdbjq.cn/Article/details/gczyuwezv.sHtML

[Q05] 重命名列
来源：http://blog.hesvh.cn/Article/details/gpgnsqyqf.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://baike.fehbvm.com/Article/details/gwcrdcqbm.sHtML

[Q06] 删除列
来源：http://www.m.share.zdbjq.cn/Article/details/ghgaaophy.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://3g.zdbjq.cn/Article/details/gqoxxoeqo.sHtML

[Q07] 删除表
来源：http://blog.zdbjq.cn/Article/details/gzuajbwhb.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.share.zdbjq.cn/Article/details/gzjiguebp.sHtML

[Q08] 创建普通索引
来源：http://baike.hesvh.cn/Article/details/gptkzlvwf.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.m.share.hesvh.cn/Article/details/gcqhqlygk.sHtML

[Q09] 创建唯一索引
来源：http://blog.fehbvm.com/Article/details/gglemqecg.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.blog.zdbjq.cn/Article/details/gtodktkxx.sHtML

[Q10] 插入单行
来源：http://blog.fehbvm.com/Article/details/grikqvadv.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://baike.fehbvm.com/Article/details/gciauvhid.sHtML

[Q11] 一次插入多行
来源：http://www.blog.zdbjq.cn/Article/details/glizyyxqi.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.m.share.fehbvm.com/Article/details/gbqnrmdpj.sHtML

[Q12] 插入后取自增 ID
来源：http://m.share.hesvh.cn/Article/details/gkcerapqu.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://mobile.hesvh.cn/Article/details/gyzijomwc.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://mobile.zdbjq.cn/Article/details/gthyezkqi.sHtML

[Q13] 忽略重复插入
来源：http://read.share.zdbjq.cn/Article/details/grbglwept.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://read.share.zdbjq.cn/Article/details/gugypuvdq.sHtML

[Q14] 存在则更新（upsert）
来源：http://mobile.fehbvm.com/Article/details/gvghpcvyl.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://m.share.hesvh.cn/Article/details/gjgozpnng.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.blog.zdbjq.cn/Article/details/gwtdlxcoc.sHtML

[Q15] 查询全部
来源：http://www.blog.zdbjq.cn/Article/details/gbknmfyks.sHtML

SELECT * FROM users;
来源：http://3g.hesvh.cn/Article/details/glfgqrxkg.sHtML

[Q16] 查询指定列
来源：http://mobile.hesvh.cn/Article/details/gnvmhjetb.sHtML

SELECT id, name FROM users;
来源：http://m.share.fehbvm.com/Article/details/gajhfvhag.sHtML

[Q17] 条件查询
来源：http://www.share.fehbvm.com/Article/details/gswlijadf.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.share.hesvh.cn/Article/details/gramfhdlt.sHtML

[Q18] 模糊匹配
来源：http://wap.hesvh.cn/Article/details/guzjqkhxh.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://mobile.hesvh.cn/Article/details/gsukwmaxn.sHtML

[Q19] 范围查询
来源：http://mobile.fehbvm.com/Article/details/gjgjlrwqh.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.m.share.fehbvm.com/Article/details/gqoszioki.sHtML

[Q20] IN 列表
来源：http://read.share.hesvh.cn/Article/details/giljvzqdz.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://3g.hesvh.cn/Article/details/gkjxqbfqc.sHtML

[Q21] 空值判断
来源：http://www.blog.hesvh.cn/Article/details/guboylkqr.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://read.share.fehbvm.com/Article/details/gfekdyzme.sHtML

[Q22] 排序
来源：http://www.m.share.hesvh.cn/Article/details/gqrgsoznb.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://baike.fehbvm.com/Article/details/gvkronwcx.sHtML

[Q23] 分页
来源：http://www.m.share.zdbjq.cn/Article/details/gtuwzldee.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://read.share.zdbjq.cn/Article/details/gjgxkvgdx.sHtML

[Q24] 去重
来源：http://m.share.hesvh.cn/Article/details/gzlcmqwwm.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gcucbotym.sHtML

[Q25] 只取前 N 条
来源：http://www.blog.fehbvm.com/Article/details/geofpanpx.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.share.zdbjq.cn/Article/details/gtuhvfwww.sHtML

[Q26] 计数
来源：http://www.share.zdbjq.cn/Article/details/gcgsdevgi.sHtML

SELECT COUNT(*) FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gbnaawofi.sHtML

[Q27] 条件计数
来源：http://mobile.fehbvm.com/Article/details/gkpluysgo.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gyupgcpnw.sHtML

[Q28] 求和与平均
来源：http://www.m.share.zdbjq.cn/Article/details/gcrvyxdug.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.m.share.fehbvm.com/Article/details/griylvesx.sHtML

[Q29] 最大最小值
来源：http://3g.fehbvm.com/Article/details/gocivokpz.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.share.zdbjq.cn/Article/details/grnwzlahy.sHtML

[Q30] 分组统计
来源：http://www.m.share.hesvh.cn/Article/details/gkjunuuuc.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://wap.hesvh.cn/Article/details/gjnliibtm.sHtML

[Q31] 分组后过滤
来源：http://mobile.zdbjq.cn/Article/details/gkajvkymd.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://mobile.hesvh.cn/Article/details/gktnmdivy.sHtML

[Q32] 分组拼接字符串
来源：http://3g.hesvh.cn/Article/details/ghctufdjw.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.blog.fehbvm.com/Article/details/gkkdfvshy.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://wap.hesvh.cn/Article/details/goavaoovp.sHtML

[Q33] 多列分组
来源：http://m.share.hesvh.cn/Article/details/gjyzetmop.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://m.share.hesvh.cn/Article/details/gswgmojkm.sHtML

[Q34] 每组取第一条
来源：http://read.share.fehbvm.com/Article/details/gkyrdzeem.sHtML

SELECT * FROM (
来源：http://www.blog.fehbvm.com/Article/details/gyimipzgd.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://m.share.hesvh.cn/Article/details/gxhjfiusy.sHtML

) t WHERE rn = 1;
来源：http://www.share.zdbjq.cn/Article/details/gvtxogqbm.sHtML

[Q35] 内连接
来源：http://www.blog.hesvh.cn/Article/details/gyvczedyu.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.hesvh.cn/Article/details/gfnedmsqb.sHtML

[Q36] 左连接
来源：http://m.share.zdbjq.cn/Article/details/gscqagcef.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://baike.fehbvm.com/Article/details/gipejxrri.sHtML

[Q37] 右连接
来源：http://blog.zdbjq.cn/Article/details/gqbrkdfls.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://wap.hesvh.cn/Article/details/gezzdrpcg.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://wap.hesvh.cn/Article/details/gztrnqtic.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://baike.hesvh.cn/Article/details/gnszdcepp.sHtML

[Q39] 自连接（查上下级）
来源：http://www.blog.fehbvm.com/Article/details/geimjjute.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.share.hesvh.cn/Article/details/ghuaiamlo.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.m.share.fehbvm.com/Article/details/gzadkkigk.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://m.share.zdbjq.cn/Article/details/gnrnlicyz.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.share.hesvh.cn/Article/details/ghhoiiipq.sHtML

[Q41] 多表连接
来源：http://wap.fehbvm.com/Article/details/gsxcyqjul.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://3g.fehbvm.com/Article/details/gqddbxuro.sHtML

JOIN users u ON u.id = o.user_id
来源：http://mobile.hesvh.cn/Article/details/gmurhmlmd.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://m.share.zdbjq.cn/Article/details/gfygsfdbm.sHtML

[Q42] 连接条件附加过滤
来源：http://www.m.share.fehbvm.com/Article/details/gflvmhwxi.sHtML

SELECT u.name, o.amount FROM users u
来源：http://read.share.fehbvm.com/Article/details/gqgnhcqvv.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://blog.fehbvm.com/Article/details/gkpcglzac.sHtML

[Q43] 标量子查询
来源：http://baike.zdbjq.cn/Article/details/gxnxpnfdl.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://wap.zdbjq.cn/Article/details/gqdxgmirf.sHtML

[Q44] IN 子查询
来源：http://wap.hesvh.cn/Article/details/gynusqjny.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://baike.zdbjq.cn/Article/details/gjryxofve.sHtML

[Q45] EXISTS 判断存在
来源：http://www.blog.hesvh.cn/Article/details/gcssphxaq.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.hesvh.cn/Article/details/gnkfwvxll.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://baike.zdbjq.cn/Article/details/geqytjzsp.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.fehbvm.com/Article/details/gurpdiktl.sHtML

[Q47] 与平均值比较
来源：http://blog.fehbvm.com/Article/details/glullgcnc.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.m.share.fehbvm.com/Article/details/gvwaancuy.sHtML

[Q48] CTE 公用表表达式
来源：http://blog.hesvh.cn/Article/details/gjiywlxpv.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://mobile.fehbvm.com/Article/details/gfgmuuevo.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://m.share.fehbvm.com/Article/details/gedqcnvki.sHtML

[Q49] 更新单行
来源：http://www.share.zdbjq.cn/Article/details/galzboqoz.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.m.share.hesvh.cn/Article/details/gmquakmyi.sHtML

[Q50] 批量更新
来源：http://m.share.zdbjq.cn/Article/details/gwpxelgvu.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://3g.hesvh.cn/Article/details/gmziigqdn.sHtML

[Q51] 用子查询更新
来源：http://blog.zdbjq.cn/Article/details/gusbiuxtb.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://mobile.fehbvm.com/Article/details/gzucxnnkk.sHtML

[Q52] 删除指定行
来源：http://3g.fehbvm.com/Article/details/gwpttbniv.sHtML

DELETE FROM users WHERE id = 10;
来源：http://m.share.hesvh.cn/Article/details/gdppcrqqr.sHtML

[Q53] 按条件删除
来源：http://www.share.fehbvm.com/Article/details/gfusuxaxc.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.blog.hesvh.cn/Article/details/gdyjndqcl.sHtML

[Q54] 清空表
来源：http://wap.fehbvm.com/Article/details/gjoqudefr.sHtML

TRUNCATE TABLE logs;
来源：http://mobile.fehbvm.com/Article/details/ginpcooyv.sHtML

[Q55] 排名（并列占位）
来源：http://www.share.zdbjq.cn/Article/details/ggnujahmx.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://baike.hesvh.cn/Article/details/gvegfwjmz.sHtML

[Q56] 密集排名（并列不占位）
来源：http://baike.fehbvm.com/Article/details/gnoescdnn.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.share.fehbvm.com/Article/details/gtyvshjmw.sHtML

[Q57] 行号
来源：http://www.blog.hesvh.cn/Article/details/gidnoztep.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gwuyybyce.sHtML

[Q58] 累计求和
来源：http://www.share.fehbvm.com/Article/details/gturphweg.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.blog.fehbvm.com/Article/details/gjhodpavu.sHtML

[Q59] 分组内累计
来源：http://www.m.share.zdbjq.cn/Article/details/gmcelrcku.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://m.share.hesvh.cn/Article/details/gptanzjvl.sHtML

[Q60] 取上一行 / 下一行
来源：http://baike.zdbjq.cn/Article/details/gvzargryt.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://3g.zdbjq.cn/Article/details/gfydzwtvu.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://blog.zdbjq.cn/Article/details/glwgyfflb.sHtML

[Q61] 移动平均
来源：http://3g.fehbvm.com/Article/details/gkpiwywzn.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://wap.hesvh.cn/Article/details/gydyekrfs.sHtML

[Q62] 分组占比
来源：http://baike.fehbvm.com/Article/details/gvvpvbflh.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://wap.hesvh.cn/Article/details/gogggvfpb.sHtML

[Q63] 开启事务
来源：http://www.blog.fehbvm.com/Article/details/gcutuflzg.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://3g.fehbvm.com/Article/details/ghtveaeys.sHtML

[Q64] 提交事务
来源：http://wap.fehbvm.com/Article/details/gsmgqtdvk.sHtML

COMMIT;
来源：http://mobile.hesvh.cn/Article/details/gietxvojp.sHtML

[Q65] 回滚事务
来源：http://m.share.fehbvm.com/Article/details/gmiiygtek.sHtML

ROLLBACK;
来源：http://baike.zdbjq.cn/Article/details/gvffwyfbq.sHtML

[Q66] 行锁查询
来源：http://3g.zdbjq.cn/Article/details/gipcjwcgm.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://baike.hesvh.cn/Article/details/gerggjbnv.sHtML

[Q67] 设置隔离级别
来源：http://read.share.hesvh.cn/Article/details/gobccnxgf.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.m.share.fehbvm.com/Article/details/genpjhung.sHtML

[Q68] 保存点
来源：http://www.blog.zdbjq.cn/Article/details/guqyuvfxw.sHtML

SAVEPOINT sp1;
来源：http://www.share.zdbjq.cn/Article/details/gtpbqefqf.sHtML

ROLLBACK TO sp1;
来源：http://blog.fehbvm.com/Article/details/gwimpgezb.sHtML

[Q69] 查看执行计划
来源：http://www.m.share.fehbvm.com/Article/details/gswkodgto.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://m.share.hesvh.cn/Article/details/gwubzmoef.sHtML

[Q70] 更新统计信息
来源：http://mobile.zdbjq.cn/Article/details/gnnkkiqkp.sHtML

ANALYZE TABLE users;
来源：http://wap.hesvh.cn/Article/details/grddbuifi.sHtML

[Q71] 查看建表语句
来源：http://wap.hesvh.cn/Article/details/gycshbctz.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.m.share.zdbjq.cn/Article/details/gofjwhxwb.sHtML

[Q72] 查看索引
来源：http://read.share.fehbvm.com/Article/details/gxikqofhn.sHtML

SHOW INDEX FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gidqucdlx.sHtML

[Q73] 查看表状态
来源：http://m.share.hesvh.cn/Article/details/gauxyowoh.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://3g.hesvh.cn/Article/details/gqufnsfbw.sHtML

[Q74] 强制使用索引
来源：http://mobile.hesvh.cn/Article/details/gpphnwiby.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://baike.fehbvm.com/Article/details/gfmxhnjda.sHtML

[Q75] 日期格式化
来源：http://wap.fehbvm.com/Article/details/gzecamxwk.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://blog.zdbjq.cn/Article/details/gpprhpvlz.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://wap.hesvh.cn/Article/details/gcojazsej.sHtML

[Q76] 按天统计
来源：http://blog.zdbjq.cn/Article/details/gtqlvebvo.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.m.share.fehbvm.com/Article/details/govswftjr.sHtML

[Q77] 时间加减
来源：http://www.m.share.fehbvm.com/Article/details/gmnagqhwi.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://mobile.hesvh.cn/Article/details/ggudpvifd.sHtML

[Q78] 当前时间
来源：http://3g.zdbjq.cn/Article/details/ghzzvmrba.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://blog.fehbvm.com/Article/details/gfnmeidzq.sHtML

[Q79] 字符串拼接
来源：http://www.blog.zdbjq.cn/Article/details/gdblnwjxe.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://blog.hesvh.cn/Article/details/gzyuqqbuw.sHtML

[Q80] 字符串截取
来源：http://www.m.share.hesvh.cn/Article/details/gwoaeuowa.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.share.fehbvm.com/Article/details/gbhmaujmt.sHtML

[Q81] 字符串替换
来源：http://blog.zdbjq.cn/Article/details/gtkzyrgmd.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://blog.zdbjq.cn/Article/details/grjnexxrj.sHtML

[Q82] 字符长度与字节长度
来源：http://www.blog.fehbvm.com/Article/details/gbhrybybv.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://blog.zdbjq.cn/Article/details/gkdljdnly.sHtML

[Q83] 大小写转换
来源：http://mobile.hesvh.cn/Article/details/geoxxhxis.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://3g.hesvh.cn/Article/details/gfmvfqqyz.sHtML

[Q84] 去除首尾空格
来源：http://m.share.fehbvm.com/Article/details/gzcgchwwp.sHtML

SELECT TRIM(name) FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gnkcmrizo.sHtML

[Q85] 数值取整
来源：http://blog.zdbjq.cn/Article/details/gkjsheisu.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://m.share.fehbvm.com/Article/details/gznzvpaep.sHtML

[Q86] 读取 JSON 字段
来源：http://blog.zdbjq.cn/Article/details/goqwjwumc.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://m.share.hesvh.cn/Article/details/gzpabvbuj.sHtML

[Q87] JSON 字段做条件
来源：http://wap.fehbvm.com/Article/details/ggedarbit.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://baike.zdbjq.cn/Article/details/gwvvoamvb.sHtML

[Q88] 行转列（条件聚合）
来源：http://wap.zdbjq.cn/Article/details/gyrfqgqgy.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://m.share.fehbvm.com/Article/details/gxbcxgkjc.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://3g.zdbjq.cn/Article/details/gpoegzimb.sHtML

[Q89] 判断表是否存在
来源：http://wap.fehbvm.com/Article/details/ghcdezfsf.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://mobile.fehbvm.com/Article/details/glkypsjys.sHtML

[Q90] 生成序号列
来源：http://m.share.hesvh.cn/Article/details/gjwhlqvrw.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://read.share.fehbvm.com/Article/details/grnfrnfln.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gelbboony.sHtML

R. Bash 专题
来源：http://wap.hesvh.cn/Article/details/gmzbwonxe.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gsfzuujaf.sHtML

[R01] shebang 与严格模式
来源：http://m.share.fehbvm.com/Article/details/golzomdgu.sHtML

#!/usr/bin/env bash
来源：http://www.share.zdbjq.cn/Article/details/gragqtdnn.sHtML

set -euo pipefail
来源：http://3g.hesvh.cn/Article/details/gxfhsbhpd.sHtML

[R02] 变量赋值与使用
来源：http://read.share.hesvh.cn/Article/details/gepacures.sHtML

name="Tom"; echo "$name"
来源：http://baike.hesvh.cn/Article/details/gkvgsgnih.sHtML

[R03] 只读变量
来源：http://wap.hesvh.cn/Article/details/gmmxxewmq.sHtML

readonly PI=3.14
来源：http://www.share.zdbjq.cn/Article/details/gqvmplfts.sHtML

[R04] 位置参数
来源：http://3g.fehbvm.com/Article/details/gxnqnmwwd.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://baike.fehbvm.com/Article/details/gzrdrzsqc.sHtML

[R05] 参数默认值
来源：http://www.blog.fehbvm.com/Article/details/gwkhhuens.sHtML

name="${1:-default}"
来源：http://www.share.fehbvm.com/Article/details/glzfzporj.sHtML

[R06] 判断命令是否存在
来源：http://wap.hesvh.cn/Article/details/gedpkrxfw.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://wap.hesvh.cn/Article/details/gtnlwritv.sHtML

[R07] if 判断文件
来源：http://blog.fehbvm.com/Article/details/gpdjdbkiu.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://3g.fehbvm.com/Article/details/gwbpwvuel.sHtML

[R08] 数值比较
来源：http://mobile.fehbvm.com/Article/details/guhqlfvlr.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://blog.zdbjq.cn/Article/details/glkrlyjrc.sHtML

[R09] 字符串比较
来源：http://read.share.fehbvm.com/Article/details/ganxkupcj.sHtML


<!-- 参考信息 -->