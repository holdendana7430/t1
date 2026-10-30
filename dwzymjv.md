代发 wailian999

C#:   Parallel.For
来源：http://wap.fehbvm.com/Article/details/gwezpmcvt.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gwbsquehf.sHtML

P. 常用工具函数
来源：http://www.share.hesvh.cn/Article/details/gwvwccivi.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gnhcqqnxa.sHtML

[P01] 生成 UUID
来源：http://www.m.share.fehbvm.com/Article/details/gfnvnnadm.sHtML

Py:   str(uuid.uuid4())
来源：http://www.blog.zdbjq.cn/Article/details/geyhvwmse.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.share.fehbvm.com/Article/details/gincbbocc.sHtML

JS:   crypto.randomUUID()
来源：http://3g.zdbjq.cn/Article/details/glrzozjwy.sHtML

TS:   crypto.randomUUID()
来源：http://www.m.share.fehbvm.com/Article/details/glgrxkzwu.sHtML

Java: UUID.randomUUID().toString()
来源：http://blog.zdbjq.cn/Article/details/gorcloynt.sHtML

Go:   // 用 github.com/google/uuid
来源：http://3g.zdbjq.cn/Article/details/gxvrgfddz.sHtML

Ruby: SecureRandom.uuid
来源：http://www.m.share.zdbjq.cn/Article/details/ggnqvyjcx.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://read.share.fehbvm.com/Article/details/gvttgtrou.sHtML

[P02] MD5 / SHA256 摘要
来源：http://m.share.hesvh.cn/Article/details/gedqrsbtr.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://baike.hesvh.cn/Article/details/gbvjzhvnl.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://mobile.hesvh.cn/Article/details/gzohclbfm.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://baike.fehbvm.com/Article/details/gwdsdqfzy.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://wap.zdbjq.cn/Article/details/gpaahjuvg.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://3g.hesvh.cn/Article/details/grqrwrvme.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.share.fehbvm.com/Article/details/gjjqxkmpr.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://mobile.zdbjq.cn/Article/details/gxlgjnnjn.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://blog.zdbjq.cn/Article/details/gafzylbvp.sHtML

[P03] 生成短随机字符串
来源：http://3g.fehbvm.com/Article/details/gksaxrzpi.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://3g.hesvh.cn/Article/details/gyvebsskj.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.share.fehbvm.com/Article/details/gfbjacucg.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.hesvh.cn/Article/details/guhvwomut.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://3g.hesvh.cn/Article/details/gqikkcewg.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://read.share.fehbvm.com/Article/details/gqgmpqotp.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://3g.zdbjq.cn/Article/details/gcojdhrwx.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://m.share.fehbvm.com/Article/details/gusavdstj.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://3g.hesvh.cn/Article/details/gyvikfzuv.sHtML

[P04] 求长度
来源：http://mobile.zdbjq.cn/Article/details/gofykvpgf.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.m.share.zdbjq.cn/Article/details/gawvpoozp.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.zdbjq.cn/Article/details/gquzoxzzb.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.zdbjq.cn/Article/details/gsmdcrlka.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.hesvh.cn/Article/details/gthqukthk.sHtML

Java: list.size();  map.size();  s.length()
来源：http://wap.zdbjq.cn/Article/details/giasnhffh.sHtML

Go:   len(arr);  len(m)
来源：http://mobile.zdbjq.cn/Article/details/grrcirilp.sHtML

Ruby: x.length;  x.size
来源：http://blog.zdbjq.cn/Article/details/gmzvyaxnm.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://m.share.fehbvm.com/Article/details/gepuviehk.sHtML

[P05] 判断两个对象内容是否相等
来源：http://baike.hesvh.cn/Article/details/gxjbyubob.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.share.zdbjq.cn/Article/details/gfhcsunze.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://read.share.fehbvm.com/Article/details/gewkgucef.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://blog.hesvh.cn/Article/details/gqiffswlb.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://m.share.zdbjq.cn/Article/details/gddgbnyzy.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://m.share.hesvh.cn/Article/details/gaqjybezk.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.share.fehbvm.com/Article/details/gfeijerkh.sHtML

Ruby: a == b
来源：http://mobile.hesvh.cn/Article/details/gdjhnblyz.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://mobile.hesvh.cn/Article/details/gcqgqdhch.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.share.zdbjq.cn/Article/details/ghulwuomr.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://wap.zdbjq.cn/Article/details/gndfmburc.sHtML

PHP:  if (empty($x)) {}
来源：http://mobile.hesvh.cn/Article/details/gvivhnkow.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.blog.zdbjq.cn/Article/details/gftwspnas.sHtML

TS:   if (x == null) {}
来源：http://wap.zdbjq.cn/Article/details/gkjfcolhw.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.share.fehbvm.com/Article/details/gxlvxweax.sHtML

Go:   if x == nil {}
来源：http://www.blog.hesvh.cn/Article/details/gpegdewcy.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://blog.hesvh.cn/Article/details/gbitvegcl.sHtML

C#:   if (x is null) {}
来源：http://3g.hesvh.cn/Article/details/ghsvxxbsu.sHtML

[P07] 防抖与节流
来源：http://www.blog.fehbvm.com/Article/details/gfaacxmpw.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://wap.hesvh.cn/Article/details/gsqeygcgr.sHtML

PHP:  // 手写时间戳比较
来源：http://m.share.zdbjq.cn/Article/details/grrfuudkm.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.zdbjq.cn/Article/details/gcqvtfxko.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.zdbjq.cn/Article/details/grjyadgfy.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.share.hesvh.cn/Article/details/gwwcudtkx.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.m.share.hesvh.cn/Article/details/gvattqptb.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://wap.fehbvm.com/Article/details/gtspqdarc.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://3g.zdbjq.cn/Article/details/gzmpjesnu.sHtML

[P08] 处理浮点精度问题
来源：http://baike.hesvh.cn/Article/details/gqwiswrjl.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://3g.fehbvm.com/Article/details/gheidzwji.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://read.share.zdbjq.cn/Article/details/gfvkmbzkg.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.blog.zdbjq.cn/Article/details/gkxorfffs.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.share.hesvh.cn/Article/details/gwlzeigyn.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://blog.zdbjq.cn/Article/details/gsbszbvyn.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://blog.zdbjq.cn/Article/details/gtllhumgs.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://mobile.fehbvm.com/Article/details/gigjpvrig.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://mobile.fehbvm.com/Article/details/gxvgbdsaj.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/garqyiarp.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://mobile.hesvh.cn/Article/details/gdvaamrgl.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gjrzdoswl.sHtML

[Q01] 创建表
来源：http://www.blog.zdbjq.cn/Article/details/gyjdcnmrg.sHtML

CREATE TABLE users (
来源：http://wap.zdbjq.cn/Article/details/gfuvlfnaz.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.hesvh.cn/Article/details/gejpnxmvs.sHtML

name VARCHAR(50) NOT NULL,
来源：http://m.share.fehbvm.com/Article/details/gazjeuxtc.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.m.share.zdbjq.cn/Article/details/gwqnkgqkn.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://read.share.zdbjq.cn/Article/details/gczqtzyap.sHtML

);
来源：http://mobile.zdbjq.cn/Article/details/ggqrtdcgf.sHtML

[Q02] 创建带外键的表
来源：http://m.share.fehbvm.com/Article/details/ghfbaijib.sHtML

CREATE TABLE orders (
来源：http://mobile.fehbvm.com/Article/details/gdquoyfem.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.zdbjq.cn/Article/details/gwmbzuwfa.sHtML

user_id INT NOT NULL,
来源：http://www.share.fehbvm.com/Article/details/gbvcmxusr.sHtML

amount DECIMAL(10, 2),
来源：http://blog.fehbvm.com/Article/details/gfyeebltj.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://read.share.hesvh.cn/Article/details/gtrrmaxkd.sHtML

);
来源：http://blog.fehbvm.com/Article/details/gykgjsfmt.sHtML

[Q03] 增加列
来源：http://www.share.zdbjq.cn/Article/details/ghguajupt.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.m.share.hesvh.cn/Article/details/gejcgecax.sHtML

[Q04] 修改列类型
来源：http://www.m.share.hesvh.cn/Article/details/gjdrproxm.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://3g.zdbjq.cn/Article/details/gyvusozmo.sHtML

[Q05] 重命名列
来源：http://wap.fehbvm.com/Article/details/gezwouodn.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://baike.hesvh.cn/Article/details/ggvitjwig.sHtML

[Q06] 删除列
来源：http://baike.hesvh.cn/Article/details/ghekryvpa.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://3g.zdbjq.cn/Article/details/gmolnlacx.sHtML

[Q07] 删除表
来源：http://www.share.hesvh.cn/Article/details/gcqblgrmo.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.blog.fehbvm.com/Article/details/groilpmop.sHtML

[Q08] 创建普通索引
来源：http://wap.hesvh.cn/Article/details/gsdlmjhlz.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.share.hesvh.cn/Article/details/garzgffvb.sHtML

[Q09] 创建唯一索引
来源：http://blog.hesvh.cn/Article/details/gwnwuoicf.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.blog.fehbvm.com/Article/details/gyuigtkze.sHtML

[Q10] 插入单行
来源：http://www.share.hesvh.cn/Article/details/gaguyvaeq.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.blog.fehbvm.com/Article/details/gsiqlricc.sHtML

[Q11] 一次插入多行
来源：http://www.blog.zdbjq.cn/Article/details/gklutnfqk.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.share.zdbjq.cn/Article/details/gnjavdaqb.sHtML

[Q12] 插入后取自增 ID
来源：http://m.share.zdbjq.cn/Article/details/gfkgwpncs.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://read.share.zdbjq.cn/Article/details/gpqlmdpxo.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://m.share.zdbjq.cn/Article/details/ghhwgmllz.sHtML

[Q13] 忽略重复插入
来源：http://baike.fehbvm.com/Article/details/gtlkboqut.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://wap.hesvh.cn/Article/details/geraplfeb.sHtML

[Q14] 存在则更新（upsert）
来源：http://read.share.hesvh.cn/Article/details/gcgasefgr.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://3g.fehbvm.com/Article/details/gxtwfxjgh.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.share.zdbjq.cn/Article/details/gjtjhbgud.sHtML

[Q15] 查询全部
来源：http://www.share.hesvh.cn/Article/details/gspvjqcxc.sHtML

SELECT * FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gcgvghdpn.sHtML

[Q16] 查询指定列
来源：http://www.m.share.hesvh.cn/Article/details/gggxrmlnz.sHtML

SELECT id, name FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gxguieesn.sHtML

[Q17] 条件查询
来源：http://m.share.hesvh.cn/Article/details/gvitygada.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.m.share.hesvh.cn/Article/details/gflrnmjqp.sHtML

[Q18] 模糊匹配
来源：http://www.blog.zdbjq.cn/Article/details/guhruqhgq.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://baike.fehbvm.com/Article/details/gywlbemmu.sHtML

[Q19] 范围查询
来源：http://www.share.fehbvm.com/Article/details/gbowjpven.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://blog.fehbvm.com/Article/details/grmsafwkv.sHtML

[Q20] IN 列表
来源：http://www.share.fehbvm.com/Article/details/glvjjlmxq.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://mobile.zdbjq.cn/Article/details/ghxgvchgd.sHtML

[Q21] 空值判断
来源：http://www.m.share.hesvh.cn/Article/details/gxdlmcwky.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.share.zdbjq.cn/Article/details/gkxyasaig.sHtML

[Q22] 排序
来源：http://mobile.zdbjq.cn/Article/details/gthibdzwc.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://3g.zdbjq.cn/Article/details/gfeepspgz.sHtML

[Q23] 分页
来源：http://mobile.hesvh.cn/Article/details/gbmanlgwp.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.m.share.hesvh.cn/Article/details/ggnddhyzr.sHtML

[Q24] 去重
来源：http://www.share.zdbjq.cn/Article/details/gbgzsnzkt.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gafsnqapi.sHtML

[Q25] 只取前 N 条
来源：http://www.share.hesvh.cn/Article/details/giarvxkfw.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://mobile.zdbjq.cn/Article/details/grlnnwxap.sHtML

[Q26] 计数
来源：http://www.share.zdbjq.cn/Article/details/gtplersmx.sHtML

SELECT COUNT(*) FROM users;
来源：http://blog.zdbjq.cn/Article/details/geclbjptz.sHtML

[Q27] 条件计数
来源：http://wap.zdbjq.cn/Article/details/gdhzoxhzr.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://baike.fehbvm.com/Article/details/gkbdfalgb.sHtML

[Q28] 求和与平均
来源：http://www.share.zdbjq.cn/Article/details/gtbjgcnnh.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://baike.hesvh.cn/Article/details/gunftmqme.sHtML

[Q29] 最大最小值
来源：http://www.m.share.fehbvm.com/Article/details/gpsxpfvug.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gyaaonvnk.sHtML

[Q30] 分组统计
来源：http://blog.hesvh.cn/Article/details/gmqqgrjem.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://wap.hesvh.cn/Article/details/ghtitbteh.sHtML

[Q31] 分组后过滤
来源：http://wap.fehbvm.com/Article/details/gmjxszaeg.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.m.share.hesvh.cn/Article/details/gpzhtcidt.sHtML

[Q32] 分组拼接字符串
来源：http://baike.fehbvm.com/Article/details/gdyckmuum.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://m.share.zdbjq.cn/Article/details/grzucnbgx.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://3g.fehbvm.com/Article/details/gdcwzajsf.sHtML

[Q33] 多列分组
来源：http://baike.fehbvm.com/Article/details/gujgiptol.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://baike.zdbjq.cn/Article/details/gekjeuisr.sHtML

[Q34] 每组取第一条
来源：http://blog.zdbjq.cn/Article/details/gemxtklpz.sHtML

SELECT * FROM (
来源：http://www.blog.fehbvm.com/Article/details/gjirlkgoa.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.m.share.zdbjq.cn/Article/details/gdcwmnifg.sHtML

) t WHERE rn = 1;
来源：http://mobile.hesvh.cn/Article/details/glhdrolqb.sHtML

[Q35] 内连接
来源：http://3g.zdbjq.cn/Article/details/gyflabxgs.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.fehbvm.com/Article/details/gsydkmzbw.sHtML

[Q36] 左连接
来源：http://3g.hesvh.cn/Article/details/gkcxltqkr.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://wap.hesvh.cn/Article/details/gkirzotgv.sHtML

[Q37] 右连接
来源：http://www.m.share.fehbvm.com/Article/details/gejqrrxmo.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://wap.hesvh.cn/Article/details/ggwhqdkva.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://mobile.zdbjq.cn/Article/details/geytkplin.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://wap.fehbvm.com/Article/details/ghlswvtjs.sHtML

[Q39] 自连接（查上下级）
来源：http://m.share.zdbjq.cn/Article/details/gtijtvstm.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://3g.fehbvm.com/Article/details/gugpjsxbd.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.share.zdbjq.cn/Article/details/ggfyzognj.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.m.share.fehbvm.com/Article/details/gqjamnvrx.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://3g.zdbjq.cn/Article/details/goehwboso.sHtML

[Q41] 多表连接
来源：http://www.m.share.fehbvm.com/Article/details/geqcawebr.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://mobile.zdbjq.cn/Article/details/gyyxodoiz.sHtML

JOIN users u ON u.id = o.user_id
来源：http://mobile.zdbjq.cn/Article/details/gouajrion.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://baike.fehbvm.com/Article/details/gguxsibgi.sHtML

[Q42] 连接条件附加过滤
来源：http://m.share.fehbvm.com/Article/details/gszxmntdh.sHtML

SELECT u.name, o.amount FROM users u
来源：http://mobile.hesvh.cn/Article/details/gbaazckju.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://blog.fehbvm.com/Article/details/gvvrehhcc.sHtML

[Q43] 标量子查询
来源：http://wap.fehbvm.com/Article/details/gbtcgooib.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://wap.zdbjq.cn/Article/details/gxfyyebdu.sHtML

[Q44] IN 子查询
来源：http://m.share.hesvh.cn/Article/details/gzqsdfxsk.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.blog.zdbjq.cn/Article/details/geaktomqh.sHtML

[Q45] EXISTS 判断存在
来源：http://wap.hesvh.cn/Article/details/gxnonjuym.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.zdbjq.cn/Article/details/gpwlkeggq.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://blog.zdbjq.cn/Article/details/gmploapbw.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.hesvh.cn/Article/details/ghegkgckf.sHtML

[Q47] 与平均值比较
来源：http://blog.zdbjq.cn/Article/details/gfntzxpsh.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.m.share.zdbjq.cn/Article/details/guutduwkz.sHtML

[Q48] CTE 公用表表达式
来源：http://baike.hesvh.cn/Article/details/grqjpoaey.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.m.share.zdbjq.cn/Article/details/ghviwnjin.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://m.share.zdbjq.cn/Article/details/grbamdzph.sHtML

[Q49] 更新单行
来源：http://www.share.zdbjq.cn/Article/details/gyyuzsazt.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://wap.hesvh.cn/Article/details/ghnjjzcvu.sHtML

[Q50] 批量更新
来源：http://3g.zdbjq.cn/Article/details/gvyojuwfy.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://baike.hesvh.cn/Article/details/gpklbspjm.sHtML

[Q51] 用子查询更新
来源：http://baike.zdbjq.cn/Article/details/gymfmsqlx.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://read.share.hesvh.cn/Article/details/gmojxqxlv.sHtML

[Q52] 删除指定行
来源：http://m.share.zdbjq.cn/Article/details/gwsvnkwcg.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.share.zdbjq.cn/Article/details/gbfxkikmw.sHtML

[Q53] 按条件删除
来源：http://wap.fehbvm.com/Article/details/gzvhxnodm.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://blog.zdbjq.cn/Article/details/garhkahdx.sHtML

[Q54] 清空表
来源：http://baike.hesvh.cn/Article/details/gyqfjvaua.sHtML

TRUNCATE TABLE logs;
来源：http://m.share.fehbvm.com/Article/details/gaywaevui.sHtML

[Q55] 排名（并列占位）
来源：http://mobile.zdbjq.cn/Article/details/gvtuswnau.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.blog.hesvh.cn/Article/details/gjhcjsnnd.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.share.fehbvm.com/Article/details/giwukbgbc.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://read.share.hesvh.cn/Article/details/gvbvwkmli.sHtML

[Q57] 行号
来源：http://read.share.zdbjq.cn/Article/details/godzljpmh.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.share.hesvh.cn/Article/details/grxaujsip.sHtML

[Q58] 累计求和
来源：http://www.m.share.fehbvm.com/Article/details/gctkivclk.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://m.share.fehbvm.com/Article/details/gljvhlynf.sHtML

[Q59] 分组内累计
来源：http://wap.fehbvm.com/Article/details/gwyrjeeld.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.m.share.hesvh.cn/Article/details/glufwzbbo.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.share.hesvh.cn/Article/details/gyusclqbk.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://m.share.hesvh.cn/Article/details/goliiuglz.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://blog.hesvh.cn/Article/details/gliljzfzd.sHtML

[Q61] 移动平均
来源：http://www.blog.hesvh.cn/Article/details/gyjhevvbc.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.m.share.fehbvm.com/Article/details/gbgcfripx.sHtML

[Q62] 分组占比
来源：http://baike.hesvh.cn/Article/details/grpoxgttt.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://mobile.hesvh.cn/Article/details/gursxgffk.sHtML

[Q63] 开启事务
来源：http://www.share.hesvh.cn/Article/details/ghlfvywmw.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://baike.hesvh.cn/Article/details/gukuamwma.sHtML

[Q64] 提交事务
来源：http://baike.hesvh.cn/Article/details/gjcwglmaj.sHtML

COMMIT;
来源：http://www.share.zdbjq.cn/Article/details/gtvpuioqn.sHtML

[Q65] 回滚事务
来源：http://blog.hesvh.cn/Article/details/gpjdcuhjs.sHtML

ROLLBACK;
来源：http://www.blog.fehbvm.com/Article/details/gnvvtqjpt.sHtML

[Q66] 行锁查询
来源：http://blog.fehbvm.com/Article/details/gorkrgjai.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://mobile.fehbvm.com/Article/details/ggkbrbipj.sHtML

[Q67] 设置隔离级别
来源：http://baike.hesvh.cn/Article/details/ggnrkorzn.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://3g.fehbvm.com/Article/details/gxcsxztjq.sHtML

[Q68] 保存点
来源：http://read.share.fehbvm.com/Article/details/gvnhiysek.sHtML

SAVEPOINT sp1;
来源：http://www.share.zdbjq.cn/Article/details/gjhsuubmj.sHtML

ROLLBACK TO sp1;
来源：http://baike.fehbvm.com/Article/details/gunelvlwo.sHtML

[Q69] 查看执行计划
来源：http://baike.fehbvm.com/Article/details/gvqampchh.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://m.share.fehbvm.com/Article/details/gooywkqpn.sHtML

[Q70] 更新统计信息
来源：http://www.m.share.fehbvm.com/Article/details/gjrfybaut.sHtML

ANALYZE TABLE users;
来源：http://www.blog.hesvh.cn/Article/details/gjmyxjmpz.sHtML

[Q71] 查看建表语句
来源：http://www.m.share.hesvh.cn/Article/details/gphieatks.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://m.share.hesvh.cn/Article/details/gwfxmtugb.sHtML

[Q72] 查看索引
来源：http://blog.hesvh.cn/Article/details/guqohasru.sHtML

SHOW INDEX FROM users;
来源：http://m.share.hesvh.cn/Article/details/gxrsdjecm.sHtML

[Q73] 查看表状态
来源：http://www.m.share.hesvh.cn/Article/details/gphkmgudc.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://blog.hesvh.cn/Article/details/ghnrhmijd.sHtML

[Q74] 强制使用索引
来源：http://baike.hesvh.cn/Article/details/gjofvcddw.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://baike.hesvh.cn/Article/details/glrllhevm.sHtML

[Q75] 日期格式化
来源：http://3g.hesvh.cn/Article/details/gtmvzfihr.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://3g.zdbjq.cn/Article/details/gqvuxdqcj.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.share.zdbjq.cn/Article/details/gnhvpyekq.sHtML

[Q76] 按天统计
来源：http://wap.hesvh.cn/Article/details/gxdiahzbe.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://mobile.hesvh.cn/Article/details/gnnjobdvp.sHtML

[Q77] 时间加减
来源：http://www.m.share.hesvh.cn/Article/details/gjvqwpvhu.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://m.share.hesvh.cn/Article/details/gloriammh.sHtML

[Q78] 当前时间
来源：http://www.blog.fehbvm.com/Article/details/gwktgivrq.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://read.share.hesvh.cn/Article/details/gcmglhots.sHtML

[Q79] 字符串拼接
来源：http://www.blog.hesvh.cn/Article/details/gnlcfjnpw.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://m.share.zdbjq.cn/Article/details/gvxcceqqv.sHtML

[Q80] 字符串截取
来源：http://mobile.hesvh.cn/Article/details/ghigfnudc.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.share.fehbvm.com/Article/details/gshqfihcz.sHtML

[Q81] 字符串替换
来源：http://mobile.hesvh.cn/Article/details/gnmcpuhdc.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://blog.hesvh.cn/Article/details/gojcmyuex.sHtML

[Q82] 字符长度与字节长度
来源：http://baike.fehbvm.com/Article/details/gensnubhw.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://read.share.hesvh.cn/Article/details/gpvaqwxiw.sHtML

[Q83] 大小写转换
来源：http://baike.hesvh.cn/Article/details/giddujkhu.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://mobile.hesvh.cn/Article/details/ghivmxncj.sHtML

[Q84] 去除首尾空格
来源：http://blog.fehbvm.com/Article/details/gbjwsonve.sHtML

SELECT TRIM(name) FROM users;
来源：http://blog.zdbjq.cn/Article/details/gzfalvuoi.sHtML

[Q85] 数值取整
来源：http://3g.hesvh.cn/Article/details/gxglhrmyo.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://read.share.hesvh.cn/Article/details/gijjmwhvy.sHtML

[Q86] 读取 JSON 字段
来源：http://3g.fehbvm.com/Article/details/gwhgawuot.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://m.share.fehbvm.com/Article/details/gcdatimsq.sHtML

[Q87] JSON 字段做条件
来源：http://baike.fehbvm.com/Article/details/geckaluby.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://3g.fehbvm.com/Article/details/gojyywaok.sHtML

[Q88] 行转列（条件聚合）
来源：http://blog.hesvh.cn/Article/details/gpnazzcfx.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://m.share.hesvh.cn/Article/details/gcygskpmx.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gwizgvsrn.sHtML

[Q89] 判断表是否存在
来源：http://3g.fehbvm.com/Article/details/gcjiefdtd.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://3g.zdbjq.cn/Article/details/gghbqjgvh.sHtML

[Q90] 生成序号列
来源：http://blog.zdbjq.cn/Article/details/gcefuthsp.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://blog.fehbvm.com/Article/details/gfpmsjimi.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gjculspev.sHtML

R. Bash 专题
来源：http://mobile.hesvh.cn/Article/details/gatzpkkqb.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gcbvivghw.sHtML

[R01] shebang 与严格模式
来源：http://www.share.fehbvm.com/Article/details/gjfsgyaut.sHtML

#!/usr/bin/env bash
来源：http://blog.hesvh.cn/Article/details/gpzzakrom.sHtML

set -euo pipefail
来源：http://read.share.zdbjq.cn/Article/details/gxhubogey.sHtML

[R02] 变量赋值与使用
来源：http://3g.zdbjq.cn/Article/details/gllppvuuw.sHtML

name="Tom"; echo "$name"
来源：http://m.share.zdbjq.cn/Article/details/girxpzgtx.sHtML

[R03] 只读变量
来源：http://wap.zdbjq.cn/Article/details/goeryqlge.sHtML

readonly PI=3.14
来源：http://m.share.hesvh.cn/Article/details/gslmcsskn.sHtML

[R04] 位置参数
来源：http://baike.zdbjq.cn/Article/details/gpcwcpbfv.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.blog.hesvh.cn/Article/details/glpseihpe.sHtML

[R05] 参数默认值
来源：http://mobile.fehbvm.com/Article/details/gbruvrpvr.sHtML

name="${1:-default}"
来源：http://read.share.fehbvm.com/Article/details/gvfmayetf.sHtML

[R06] 判断命令是否存在
来源：http://wap.fehbvm.com/Article/details/gcaqefgtp.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://3g.hesvh.cn/Article/details/ghuijrmcp.sHtML

[R07] if 判断文件
来源：http://www.share.hesvh.cn/Article/details/ghtafegzq.sHtML


<!-- 参考信息 -->