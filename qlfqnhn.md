代发 wailian999

[P01] 生成 UUID
来源：http://m.share.fehbvm.com/Article/details/gjsmtxsas.sHtML

Py:   str(uuid.uuid4())
来源：http://mobile.zdbjq.cn/Article/details/gqrfwupdj.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.m.share.fehbvm.com/Article/details/gkgfdxkty.sHtML

JS:   crypto.randomUUID()
来源：http://www.m.share.fehbvm.com/Article/details/gqgmqnkki.sHtML

TS:   crypto.randomUUID()
来源：http://blog.zdbjq.cn/Article/details/ggwlmuybv.sHtML

Java: UUID.randomUUID().toString()
来源：http://m.share.zdbjq.cn/Article/details/glxhlbfej.sHtML

Go:   // 用 github.com/google/uuid
来源：http://read.share.fehbvm.com/Article/details/gwpdptbeu.sHtML

Ruby: SecureRandom.uuid
来源：http://mobile.fehbvm.com/Article/details/gwhrckito.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://3g.fehbvm.com/Article/details/gznvoyeao.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.m.share.hesvh.cn/Article/details/gafisralt.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.share.fehbvm.com/Article/details/gwtdlebia.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://mobile.zdbjq.cn/Article/details/gabohvheo.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://blog.fehbvm.com/Article/details/gbuilvrcp.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.blog.zdbjq.cn/Article/details/gkovieuqr.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://blog.zdbjq.cn/Article/details/gedzawtlq.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://m.share.fehbvm.com/Article/details/geifluyjc.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://blog.zdbjq.cn/Article/details/gvvvedndi.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://mobile.zdbjq.cn/Article/details/glziotdcj.sHtML

[P03] 生成短随机字符串
来源：http://blog.fehbvm.com/Article/details/gxyffynyd.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://mobile.fehbvm.com/Article/details/gygwglgdp.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://blog.zdbjq.cn/Article/details/gycvrnfwd.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.fehbvm.com/Article/details/gtcvihrmf.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.hesvh.cn/Article/details/gbwzpfpgx.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://read.share.hesvh.cn/Article/details/gnachctkw.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://wap.hesvh.cn/Article/details/gmvvkacuk.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.blog.hesvh.cn/Article/details/gnxxcioli.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://3g.hesvh.cn/Article/details/ghyploush.sHtML

[P04] 求长度
来源：http://read.share.hesvh.cn/Article/details/grgrobpoc.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.m.share.zdbjq.cn/Article/details/givkeotgc.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.zdbjq.cn/Article/details/gpdwlghpo.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mobile.hesvh.cn/Article/details/gdsjojiml.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.fehbvm.com/Article/details/gtyktnfcu.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.m.share.zdbjq.cn/Article/details/gadiquhvz.sHtML

Go:   len(arr);  len(m)
来源：http://wap.zdbjq.cn/Article/details/gsrvbcwmm.sHtML

Ruby: x.length;  x.size
来源：http://wap.fehbvm.com/Article/details/gtnkdwvsi.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://blog.hesvh.cn/Article/details/gpztwabto.sHtML

[P05] 判断两个对象内容是否相等
来源：http://mobile.fehbvm.com/Article/details/gyzkbbqyk.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://wap.zdbjq.cn/Article/details/giapaxguu.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://m.share.zdbjq.cn/Article/details/gprhdfimd.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://m.share.zdbjq.cn/Article/details/gbeflbvro.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://mobile.zdbjq.cn/Article/details/gvsnssdhj.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://3g.fehbvm.com/Article/details/gyitmphds.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://baike.fehbvm.com/Article/details/gwxzlhydl.sHtML

Ruby: a == b
来源：http://www.share.zdbjq.cn/Article/details/gulrufngn.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://read.share.zdbjq.cn/Article/details/gmgdnwpfz.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.blog.zdbjq.cn/Article/details/gfnfbmlpt.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://wap.fehbvm.com/Article/details/gkljhrivx.sHtML

PHP:  if (empty($x)) {}
来源：http://mobile.fehbvm.com/Article/details/gvjskvstp.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://wap.hesvh.cn/Article/details/giwjrzsmk.sHtML

TS:   if (x == null) {}
来源：http://wap.zdbjq.cn/Article/details/ggwbfsjki.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://m.share.hesvh.cn/Article/details/ggkpqrjrr.sHtML

Go:   if x == nil {}
来源：http://baike.fehbvm.com/Article/details/gsgucuhfo.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://read.share.zdbjq.cn/Article/details/geukxqhuj.sHtML

C#:   if (x is null) {}
来源：http://wap.zdbjq.cn/Article/details/golchqjve.sHtML

[P07] 防抖与节流
来源：http://3g.hesvh.cn/Article/details/gkptqndfa.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://blog.fehbvm.com/Article/details/gduhhhtzi.sHtML

PHP:  // 手写时间戳比较
来源：http://3g.zdbjq.cn/Article/details/gzgbjmxrq.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.fehbvm.com/Article/details/gedgdetdm.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.hesvh.cn/Article/details/gfscnailb.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.m.share.fehbvm.com/Article/details/gdwnbcurp.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://3g.fehbvm.com/Article/details/gdapuloyi.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://3g.hesvh.cn/Article/details/gbsotnsfd.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://wap.fehbvm.com/Article/details/gtmmidpzm.sHtML

[P08] 处理浮点精度问题
来源：http://mobile.fehbvm.com/Article/details/gflflixip.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://3g.zdbjq.cn/Article/details/glkjwzvxu.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://3g.zdbjq.cn/Article/details/guxxmtalf.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.blog.fehbvm.com/Article/details/gtloewarm.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://m.share.hesvh.cn/Article/details/gmycefkme.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://3g.hesvh.cn/Article/details/gzdziyjrk.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://mobile.fehbvm.com/Article/details/gypxcstki.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://blog.fehbvm.com/Article/details/gapvfuinw.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://wap.hesvh.cn/Article/details/gthbsyshw.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/ghgrkgelg.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.share.zdbjq.cn/Article/details/gcsmfmcww.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gjdnqbtdl.sHtML

[Q01] 创建表
来源：http://www.m.share.zdbjq.cn/Article/details/gezioznvp.sHtML

CREATE TABLE users (
来源：http://www.share.zdbjq.cn/Article/details/gnchrtqtp.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.fehbvm.com/Article/details/givvnyybt.sHtML

name VARCHAR(50) NOT NULL,
来源：http://mobile.zdbjq.cn/Article/details/gwcoqbwrm.sHtML

email VARCHAR(100) UNIQUE,
来源：http://baike.zdbjq.cn/Article/details/gvmnfkcfi.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.blog.zdbjq.cn/Article/details/gdfeataen.sHtML

);
来源：http://baike.fehbvm.com/Article/details/gwauvggnb.sHtML

[Q02] 创建带外键的表
来源：http://www.blog.zdbjq.cn/Article/details/ggwvfxhvb.sHtML

CREATE TABLE orders (
来源：http://www.m.share.zdbjq.cn/Article/details/goptpynsm.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.hesvh.cn/Article/details/ggzcqcwzm.sHtML

user_id INT NOT NULL,
来源：http://read.share.zdbjq.cn/Article/details/grnftnuha.sHtML

amount DECIMAL(10, 2),
来源：http://www.m.share.fehbvm.com/Article/details/gowekozgk.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://wap.hesvh.cn/Article/details/gioeclnxp.sHtML

);
来源：http://read.share.zdbjq.cn/Article/details/gcsuhtfas.sHtML

[Q03] 增加列
来源：http://wap.zdbjq.cn/Article/details/gozzzczmz.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://read.share.hesvh.cn/Article/details/gobadzuar.sHtML

[Q04] 修改列类型
来源：http://www.m.share.hesvh.cn/Article/details/gingnfdnr.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://m.share.hesvh.cn/Article/details/gafdblpih.sHtML

[Q05] 重命名列
来源：http://wap.zdbjq.cn/Article/details/ghfolmujc.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://mobile.hesvh.cn/Article/details/grhwixusv.sHtML

[Q06] 删除列
来源：http://baike.hesvh.cn/Article/details/gfwcjfmkt.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://3g.zdbjq.cn/Article/details/glvziwttx.sHtML

[Q07] 删除表
来源：http://wap.zdbjq.cn/Article/details/gshtowgoo.sHtML

DROP TABLE IF EXISTS orders;
来源：http://blog.fehbvm.com/Article/details/gbfqlhabm.sHtML

[Q08] 创建普通索引
来源：http://baike.zdbjq.cn/Article/details/gtbvghmfx.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.blog.hesvh.cn/Article/details/ghkxwtydl.sHtML

[Q09] 创建唯一索引
来源：http://wap.fehbvm.com/Article/details/gvbwghgqk.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://baike.hesvh.cn/Article/details/gfvqgdivw.sHtML

[Q10] 插入单行
来源：http://read.share.fehbvm.com/Article/details/gccgmxdju.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://m.share.hesvh.cn/Article/details/gwgtbhecp.sHtML

[Q11] 一次插入多行
来源：http://www.m.share.hesvh.cn/Article/details/gxlcwirea.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://m.share.zdbjq.cn/Article/details/gaeyxxtgw.sHtML

[Q12] 插入后取自增 ID
来源：http://www.share.zdbjq.cn/Article/details/gapvxgtgx.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://read.share.hesvh.cn/Article/details/gjjsbpirh.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://m.share.fehbvm.com/Article/details/gymqgvntr.sHtML

[Q13] 忽略重复插入
来源：http://mobile.fehbvm.com/Article/details/gtyinnztx.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://wap.zdbjq.cn/Article/details/gvwtxwftc.sHtML

[Q14] 存在则更新（upsert）
来源：http://3g.zdbjq.cn/Article/details/gslhzcstm.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://3g.hesvh.cn/Article/details/gpqkgktup.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.m.share.fehbvm.com/Article/details/gngtdhlwb.sHtML

[Q15] 查询全部
来源：http://blog.hesvh.cn/Article/details/gegkbsufr.sHtML

SELECT * FROM users;
来源：http://mobile.hesvh.cn/Article/details/geiasvtdp.sHtML

[Q16] 查询指定列
来源：http://mobile.hesvh.cn/Article/details/gfwmxvdlv.sHtML

SELECT id, name FROM users;
来源：http://3g.zdbjq.cn/Article/details/gxotbtwxy.sHtML

[Q17] 条件查询
来源：http://3g.hesvh.cn/Article/details/gonrxhspn.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.m.share.hesvh.cn/Article/details/gwxyflznt.sHtML

[Q18] 模糊匹配
来源：http://wap.zdbjq.cn/Article/details/gfnuxtakc.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://baike.fehbvm.com/Article/details/gukdguzth.sHtML

[Q19] 范围查询
来源：http://www.share.hesvh.cn/Article/details/gazfpzhrd.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.m.share.hesvh.cn/Article/details/gkrhxnqak.sHtML

[Q20] IN 列表
来源：http://read.share.fehbvm.com/Article/details/gfrsztmye.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://mobile.zdbjq.cn/Article/details/gcotuvxfl.sHtML

[Q21] 空值判断
来源：http://read.share.hesvh.cn/Article/details/gykwrynrx.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.share.hesvh.cn/Article/details/gawkzkxhl.sHtML

[Q22] 排序
来源：http://baike.zdbjq.cn/Article/details/ghmdnqnnw.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://baike.hesvh.cn/Article/details/gziyuilwj.sHtML

[Q23] 分页
来源：http://baike.zdbjq.cn/Article/details/gotrmsnhy.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://mobile.hesvh.cn/Article/details/gcwiorjjb.sHtML

[Q24] 去重
来源：http://www.blog.zdbjq.cn/Article/details/ggisjfyyj.sHtML

SELECT DISTINCT city FROM users;
来源：http://blog.fehbvm.com/Article/details/gkuxbqxdu.sHtML

[Q25] 只取前 N 条
来源：http://wap.zdbjq.cn/Article/details/gksiuczsb.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.blog.zdbjq.cn/Article/details/gslnchnrb.sHtML

[Q26] 计数
来源：http://www.blog.zdbjq.cn/Article/details/gxxwztkbd.sHtML

SELECT COUNT(*) FROM users;
来源：http://blog.hesvh.cn/Article/details/gpykpmwzc.sHtML

[Q27] 条件计数
来源：http://www.m.share.zdbjq.cn/Article/details/gtugddvnk.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://wap.zdbjq.cn/Article/details/gefclvlfj.sHtML

[Q28] 求和与平均
来源：http://www.blog.hesvh.cn/Article/details/gzxeweust.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://blog.zdbjq.cn/Article/details/geucdrhts.sHtML

[Q29] 最大最小值
来源：http://baike.hesvh.cn/Article/details/gxkombexg.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gttgfwfll.sHtML

[Q30] 分组统计
来源：http://wap.fehbvm.com/Article/details/gosptqxiy.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://m.share.hesvh.cn/Article/details/grorxkauk.sHtML

[Q31] 分组后过滤
来源：http://3g.zdbjq.cn/Article/details/gvmhmmebp.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://m.share.hesvh.cn/Article/details/glftvyabx.sHtML

[Q32] 分组拼接字符串
来源：http://wap.zdbjq.cn/Article/details/gnpatqond.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://wap.zdbjq.cn/Article/details/ggiocrafp.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://m.share.zdbjq.cn/Article/details/gytcmzjjb.sHtML

[Q33] 多列分组
来源：http://m.share.hesvh.cn/Article/details/gktuthprb.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://3g.hesvh.cn/Article/details/gcptbtynu.sHtML

[Q34] 每组取第一条
来源：http://mobile.zdbjq.cn/Article/details/gicttyyxk.sHtML

SELECT * FROM (
来源：http://www.m.share.hesvh.cn/Article/details/gxdfktkkl.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://blog.fehbvm.com/Article/details/guggvssxj.sHtML

) t WHERE rn = 1;
来源：http://www.share.zdbjq.cn/Article/details/gntjpxgcx.sHtML

[Q35] 内连接
来源：http://www.blog.hesvh.cn/Article/details/gqbrvidve.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://read.share.hesvh.cn/Article/details/gxzppbwyb.sHtML

[Q36] 左连接
来源：http://mobile.zdbjq.cn/Article/details/gdgyekvfh.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://mobile.hesvh.cn/Article/details/gvdodgtgt.sHtML

[Q37] 右连接
来源：http://blog.zdbjq.cn/Article/details/guhsotfhx.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://baike.zdbjq.cn/Article/details/gnlsgsuuy.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.share.hesvh.cn/Article/details/gsraxznlj.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.share.hesvh.cn/Article/details/gaklzkglm.sHtML

[Q39] 自连接（查上下级）
来源：http://read.share.fehbvm.com/Article/details/gkydtptym.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.share.fehbvm.com/Article/details/gudqhkwmd.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://baike.zdbjq.cn/Article/details/gnnyrkjiz.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.blog.zdbjq.cn/Article/details/gfdvsmmlq.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.blog.hesvh.cn/Article/details/glsspplzp.sHtML

[Q41] 多表连接
来源：http://blog.hesvh.cn/Article/details/gcdlsinvn.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://3g.zdbjq.cn/Article/details/gkfzcjcqy.sHtML

JOIN users u ON u.id = o.user_id
来源：http://blog.fehbvm.com/Article/details/gznnvmtft.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.m.share.hesvh.cn/Article/details/gdeeudwpb.sHtML

[Q42] 连接条件附加过滤
来源：http://www.m.share.fehbvm.com/Article/details/googbqauq.sHtML

SELECT u.name, o.amount FROM users u
来源：http://m.share.hesvh.cn/Article/details/gwqiqnfog.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://blog.fehbvm.com/Article/details/gsjnrqkmx.sHtML

[Q43] 标量子查询
来源：http://3g.hesvh.cn/Article/details/gmdactplo.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://wap.hesvh.cn/Article/details/gbaqmmjob.sHtML

[Q44] IN 子查询
来源：http://blog.hesvh.cn/Article/details/gqrleotce.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://m.share.hesvh.cn/Article/details/gwvvyvxdy.sHtML

[Q45] EXISTS 判断存在
来源：http://www.share.fehbvm.com/Article/details/gtfnzgzdf.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.zdbjq.cn/Article/details/gqtpzmrkf.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.m.share.fehbvm.com/Article/details/gxxrzuarr.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.fehbvm.com/Article/details/glzxmnktd.sHtML

[Q47] 与平均值比较
来源：http://read.share.zdbjq.cn/Article/details/gwdsjypji.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://mobile.zdbjq.cn/Article/details/grropgnko.sHtML

[Q48] CTE 公用表表达式
来源：http://www.share.zdbjq.cn/Article/details/gccwktqjh.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://blog.zdbjq.cn/Article/details/gllbpaytc.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.blog.hesvh.cn/Article/details/gscqjiqhn.sHtML

[Q49] 更新单行
来源：http://wap.hesvh.cn/Article/details/gertolhiv.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.blog.fehbvm.com/Article/details/guqjcpjcp.sHtML

[Q50] 批量更新
来源：http://read.share.fehbvm.com/Article/details/gomzjtvyx.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.share.fehbvm.com/Article/details/gzymqhkhn.sHtML

[Q51] 用子查询更新
来源：http://baike.zdbjq.cn/Article/details/gbxnkabht.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://mobile.hesvh.cn/Article/details/grwjtbwjt.sHtML

[Q52] 删除指定行
来源：http://3g.fehbvm.com/Article/details/gqoixsovd.sHtML

DELETE FROM users WHERE id = 10;
来源：http://wap.fehbvm.com/Article/details/gvvlcydxr.sHtML

[Q53] 按条件删除
来源：http://wap.fehbvm.com/Article/details/gjhsyepxe.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://m.share.zdbjq.cn/Article/details/gmrghmjoz.sHtML

[Q54] 清空表
来源：http://m.share.zdbjq.cn/Article/details/gdufnlcqx.sHtML

TRUNCATE TABLE logs;
来源：http://blog.hesvh.cn/Article/details/geuxrwqyn.sHtML

[Q55] 排名（并列占位）
来源：http://blog.fehbvm.com/Article/details/gttaamxtq.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.share.hesvh.cn/Article/details/gnayndazu.sHtML

[Q56] 密集排名（并列不占位）
来源：http://mobile.fehbvm.com/Article/details/gkscmavma.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.share.zdbjq.cn/Article/details/gfjkottdb.sHtML

[Q57] 行号
来源：http://mobile.zdbjq.cn/Article/details/gwfhxcxfo.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gnfcznwhy.sHtML

[Q58] 累计求和
来源：http://baike.fehbvm.com/Article/details/gveoeqjzz.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://read.share.fehbvm.com/Article/details/gsvxdwmxv.sHtML

[Q59] 分组内累计
来源：http://wap.hesvh.cn/Article/details/gyvpubsbq.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://3g.fehbvm.com/Article/details/gidofkmqj.sHtML

[Q60] 取上一行 / 下一行
来源：http://m.share.fehbvm.com/Article/details/gmryibkgw.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://read.share.fehbvm.com/Article/details/grqoadfeb.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://read.share.hesvh.cn/Article/details/gwcqseckb.sHtML

[Q61] 移动平均
来源：http://m.share.zdbjq.cn/Article/details/ggfzzkcez.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://mobile.zdbjq.cn/Article/details/gtwqlcbze.sHtML

[Q62] 分组占比
来源：http://mobile.hesvh.cn/Article/details/geetxjifz.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://baike.hesvh.cn/Article/details/gzwoqywcu.sHtML

[Q63] 开启事务
来源：http://www.m.share.zdbjq.cn/Article/details/gxmeojqwh.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://blog.fehbvm.com/Article/details/gulkwznmt.sHtML

[Q64] 提交事务
来源：http://read.share.zdbjq.cn/Article/details/gjxyyocnz.sHtML

COMMIT;
来源：http://www.blog.fehbvm.com/Article/details/gyekdogcr.sHtML

[Q65] 回滚事务
来源：http://read.share.hesvh.cn/Article/details/grqtmgqfi.sHtML

ROLLBACK;
来源：http://www.share.zdbjq.cn/Article/details/gtmxctmbf.sHtML

[Q66] 行锁查询
来源：http://www.blog.hesvh.cn/Article/details/gczmjfxvy.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.blog.zdbjq.cn/Article/details/gaufiyfkr.sHtML

[Q67] 设置隔离级别
来源：http://wap.hesvh.cn/Article/details/gisdaameq.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.share.zdbjq.cn/Article/details/gvdsgvyey.sHtML

[Q68] 保存点
来源：http://wap.zdbjq.cn/Article/details/gacukhawi.sHtML

SAVEPOINT sp1;
来源：http://blog.hesvh.cn/Article/details/gdbrzhyhf.sHtML

ROLLBACK TO sp1;
来源：http://www.m.share.fehbvm.com/Article/details/gdavvoqew.sHtML

[Q69] 查看执行计划
来源：http://www.blog.fehbvm.com/Article/details/gzfernpsd.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://wap.fehbvm.com/Article/details/gbzvudepa.sHtML

[Q70] 更新统计信息
来源：http://mobile.zdbjq.cn/Article/details/gdprkzvcc.sHtML

ANALYZE TABLE users;
来源：http://3g.hesvh.cn/Article/details/gdysmsgpo.sHtML

[Q71] 查看建表语句
来源：http://www.m.share.fehbvm.com/Article/details/gglspbtqt.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.share.hesvh.cn/Article/details/gxpwqtpzy.sHtML

[Q72] 查看索引
来源：http://baike.hesvh.cn/Article/details/gecwnmqdd.sHtML

SHOW INDEX FROM users;
来源：http://3g.fehbvm.com/Article/details/gulkzujdn.sHtML

[Q73] 查看表状态
来源：http://wap.fehbvm.com/Article/details/gtdpaswly.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://m.share.hesvh.cn/Article/details/gysogbtpb.sHtML

[Q74] 强制使用索引
来源：http://wap.hesvh.cn/Article/details/gkkxhvunz.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://baike.zdbjq.cn/Article/details/gpapqhuvg.sHtML

[Q75] 日期格式化
来源：http://3g.fehbvm.com/Article/details/gwkpduaab.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://mobile.hesvh.cn/Article/details/gahbaofxo.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://baike.fehbvm.com/Article/details/guycatsrx.sHtML

[Q76] 按天统计
来源：http://mobile.zdbjq.cn/Article/details/gwkykgits.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://baike.fehbvm.com/Article/details/gadojoaaa.sHtML

[Q77] 时间加减
来源：http://wap.zdbjq.cn/Article/details/gnxnrcdkh.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://mobile.fehbvm.com/Article/details/gcerzeduv.sHtML

[Q78] 当前时间
来源：http://wap.hesvh.cn/Article/details/gnlnqlnet.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://wap.hesvh.cn/Article/details/gesoyzxpi.sHtML

[Q79] 字符串拼接
来源：http://read.share.zdbjq.cn/Article/details/glqnufykk.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://baike.hesvh.cn/Article/details/gfvhernal.sHtML

[Q80] 字符串截取
来源：http://baike.hesvh.cn/Article/details/ghzvzqpat.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://3g.zdbjq.cn/Article/details/gblqocpri.sHtML

[Q81] 字符串替换
来源：http://blog.zdbjq.cn/Article/details/grjlvzciz.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://read.share.hesvh.cn/Article/details/ggdgnmlju.sHtML

[Q82] 字符长度与字节长度
来源：http://wap.zdbjq.cn/Article/details/ghhwwujmt.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://wap.fehbvm.com/Article/details/gjehldhjv.sHtML

[Q83] 大小写转换
来源：http://www.m.share.hesvh.cn/Article/details/gvbcoffoi.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://baike.hesvh.cn/Article/details/gduwescbh.sHtML

[Q84] 去除首尾空格
来源：http://baike.fehbvm.com/Article/details/gjtlrafqo.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.share.hesvh.cn/Article/details/gjcrrydoh.sHtML

[Q85] 数值取整
来源：http://www.share.zdbjq.cn/Article/details/gopetylkx.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://m.share.zdbjq.cn/Article/details/gruuucgaz.sHtML

[Q86] 读取 JSON 字段
来源：http://mobile.hesvh.cn/Article/details/glyjqtath.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.share.fehbvm.com/Article/details/guwzfdsnc.sHtML

[Q87] JSON 字段做条件
来源：http://www.blog.zdbjq.cn/Article/details/gvnvtbafx.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.blog.hesvh.cn/Article/details/gxrppykeo.sHtML

[Q88] 行转列（条件聚合）
来源：http://baike.hesvh.cn/Article/details/grnuipcmv.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.share.zdbjq.cn/Article/details/gjpypuury.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gltinpojw.sHtML

[Q89] 判断表是否存在
来源：http://3g.zdbjq.cn/Article/details/gttssvwsz.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://3g.zdbjq.cn/Article/details/gjlyxtwbs.sHtML

[Q90] 生成序号列
来源：http://baike.hesvh.cn/Article/details/gbjglmado.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.share.hesvh.cn/Article/details/gfccntkyx.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/ghcxniyxi.sHtML

R. Bash 专题
来源：http://baike.fehbvm.com/Article/details/gexbsiusv.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/ghvphijwx.sHtML

[R01] shebang 与严格模式
来源：http://blog.fehbvm.com/Article/details/gitzlvitd.sHtML

#!/usr/bin/env bash
来源：http://www.m.share.fehbvm.com/Article/details/goyfxnntl.sHtML

set -euo pipefail
来源：http://m.share.hesvh.cn/Article/details/gqmvybzjj.sHtML

[R02] 变量赋值与使用
来源：http://www.share.hesvh.cn/Article/details/gwsthmici.sHtML

name="Tom"; echo "$name"
来源：http://baike.zdbjq.cn/Article/details/gxbftimkk.sHtML

[R03] 只读变量
来源：http://wap.zdbjq.cn/Article/details/gqelvisgq.sHtML

readonly PI=3.14
来源：http://wap.hesvh.cn/Article/details/gdlmycyyj.sHtML

[R04] 位置参数
来源：http://read.share.hesvh.cn/Article/details/gcnsdpicy.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://3g.zdbjq.cn/Article/details/gjunumxph.sHtML

[R05] 参数默认值
来源：http://baike.hesvh.cn/Article/details/giedlckdc.sHtML

name="${1:-default}"
来源：http://www.m.share.fehbvm.com/Article/details/ghlvheejg.sHtML

[R06] 判断命令是否存在
来源：http://blog.zdbjq.cn/Article/details/gvtxgglju.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://blog.zdbjq.cn/Article/details/gmyvstfzj.sHtML

[R07] if 判断文件
来源：http://m.share.zdbjq.cn/Article/details/gyjvxnwsu.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://wap.hesvh.cn/Article/details/gnpuepwzz.sHtML

[R08] 数值比较
来源：http://baike.zdbjq.cn/Article/details/gvecjnyza.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.share.zdbjq.cn/Article/details/gfuzrbmtn.sHtML

[R09] 字符串比较
来源：http://read.share.hesvh.cn/Article/details/gvjeffoem.sHtML


<!-- 参考信息 -->