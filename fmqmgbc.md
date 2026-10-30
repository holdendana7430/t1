代发 wailian999

C#:   Parallel.For
来源：http://www.m.share.zdbjq.cn/Article/details/gxktzmavt.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gqgbdwyuv.sHtML

P. 常用工具函数
来源：http://baike.fehbvm.com/Article/details/gqpwpoyvz.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gtupoicwu.sHtML

[P01] 生成 UUID
来源：http://m.share.zdbjq.cn/Article/details/gsqafwgjn.sHtML

Py:   str(uuid.uuid4())
来源：http://mobile.fehbvm.com/Article/details/ggvzlmabw.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://blog.hesvh.cn/Article/details/giorlgccc.sHtML

JS:   crypto.randomUUID()
来源：http://wap.zdbjq.cn/Article/details/gtlphuxdd.sHtML

TS:   crypto.randomUUID()
来源：http://mobile.fehbvm.com/Article/details/gncuodhjc.sHtML

Java: UUID.randomUUID().toString()
来源：http://baike.fehbvm.com/Article/details/glvsxrpaw.sHtML

Go:   // 用 github.com/google/uuid
来源：http://3g.hesvh.cn/Article/details/gdphsimdf.sHtML

Ruby: SecureRandom.uuid
来源：http://www.m.share.hesvh.cn/Article/details/grsevbpel.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://m.share.hesvh.cn/Article/details/grwzpiwei.sHtML

[P02] MD5 / SHA256 摘要
来源：http://read.share.zdbjq.cn/Article/details/gttbckxee.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://read.share.fehbvm.com/Article/details/gnfhkumes.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://3g.hesvh.cn/Article/details/geylnkgtn.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://read.share.fehbvm.com/Article/details/ghqnqqjyd.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://mobile.zdbjq.cn/Article/details/gjsadfxap.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.share.hesvh.cn/Article/details/glzylqzst.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.m.share.fehbvm.com/Article/details/gfdlkpmnb.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://3g.fehbvm.com/Article/details/gszqcafny.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://read.share.zdbjq.cn/Article/details/gofccjyql.sHtML

[P03] 生成短随机字符串
来源：http://read.share.fehbvm.com/Article/details/gzarmalkf.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.share.hesvh.cn/Article/details/gkzteswnd.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://blog.zdbjq.cn/Article/details/gvsrvmwnp.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.hesvh.cn/Article/details/gadtopqpv.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.fehbvm.com/Article/details/gcpmsbhae.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.share.fehbvm.com/Article/details/gykdarcxh.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://m.share.fehbvm.com/Article/details/gpartrfjt.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://read.share.zdbjq.cn/Article/details/gleomrjmw.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://blog.hesvh.cn/Article/details/gpjaezeur.sHtML

[P04] 求长度
来源：http://3g.hesvh.cn/Article/details/gocelkrgr.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://mobile.fehbvm.com/Article/details/gtjibsbvq.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.fehbvm.com/Article/details/ghpqpcitl.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.fehbvm.com/Article/details/gwoxqtgap.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.hesvh.cn/Article/details/gxqpjbbcu.sHtML

Java: list.size();  map.size();  s.length()
来源：http://mobile.fehbvm.com/Article/details/gfuabhrdu.sHtML

Go:   len(arr);  len(m)
来源：http://wap.zdbjq.cn/Article/details/gzgziwdmy.sHtML

Ruby: x.length;  x.size
来源：http://mobile.zdbjq.cn/Article/details/gsqlsohnz.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://blog.hesvh.cn/Article/details/geezflajp.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.share.zdbjq.cn/Article/details/gjchqisxn.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://m.share.fehbvm.com/Article/details/geuacwdvy.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://wap.hesvh.cn/Article/details/geyzwcsfz.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://mobile.zdbjq.cn/Article/details/gxbyphgfi.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://m.share.hesvh.cn/Article/details/gdxsrgcpg.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://baike.fehbvm.com/Article/details/grmdfbssd.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://3g.hesvh.cn/Article/details/gcpfinnky.sHtML

Ruby: a == b
来源：http://3g.hesvh.cn/Article/details/ggwrqdunm.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://3g.zdbjq.cn/Article/details/gsylzakmz.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.share.hesvh.cn/Article/details/gkcxywyqp.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://blog.zdbjq.cn/Article/details/gcwwfhlso.sHtML

PHP:  if (empty($x)) {}
来源：http://baike.hesvh.cn/Article/details/gwzpqyycw.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://mobile.fehbvm.com/Article/details/gimwpymkf.sHtML

TS:   if (x == null) {}
来源：http://www.blog.fehbvm.com/Article/details/gkechlaqk.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.blog.fehbvm.com/Article/details/gvftfwzpd.sHtML

Go:   if x == nil {}
来源：http://3g.hesvh.cn/Article/details/gyhpjvvzo.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://m.share.zdbjq.cn/Article/details/geycynlvj.sHtML

C#:   if (x is null) {}
来源：http://m.share.fehbvm.com/Article/details/guzremcqe.sHtML

[P07] 防抖与节流
来源：http://3g.fehbvm.com/Article/details/gpukcleif.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://baike.hesvh.cn/Article/details/gzafzqyml.sHtML

PHP:  // 手写时间戳比较
来源：http://www.m.share.hesvh.cn/Article/details/gdwvzsfky.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.fehbvm.com/Article/details/gckmoszqm.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.hesvh.cn/Article/details/gfblwlmjx.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://blog.hesvh.cn/Article/details/gnsvpqtpk.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://wap.zdbjq.cn/Article/details/gmgsxsbms.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.blog.fehbvm.com/Article/details/gdodyucie.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://wap.zdbjq.cn/Article/details/gzjujbiap.sHtML

[P08] 处理浮点精度问题
来源：http://3g.hesvh.cn/Article/details/gofnjgfwm.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.blog.hesvh.cn/Article/details/gaptpndxf.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://baike.hesvh.cn/Article/details/gxmmyhjmw.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.blog.hesvh.cn/Article/details/gntmymdcq.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://wap.zdbjq.cn/Article/details/goftizvxw.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://m.share.fehbvm.com/Article/details/gvkrrguzs.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://blog.fehbvm.com/Article/details/gysvczduy.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://blog.hesvh.cn/Article/details/gwguaxqlk.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://wap.fehbvm.com/Article/details/gfmsyjqbn.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gkdodyxrj.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://baike.zdbjq.cn/Article/details/gryohmsdo.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/getlwzshd.sHtML

[Q01] 创建表
来源：http://m.share.zdbjq.cn/Article/details/gnuvuhuwj.sHtML

CREATE TABLE users (
来源：http://www.m.share.hesvh.cn/Article/details/gmhaaiyov.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.hesvh.cn/Article/details/goskhnqlp.sHtML

name VARCHAR(50) NOT NULL,
来源：http://blog.hesvh.cn/Article/details/gtnjuumnw.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.share.hesvh.cn/Article/details/gebndrtfy.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.m.share.fehbvm.com/Article/details/gfsujhoxc.sHtML

);
来源：http://mobile.hesvh.cn/Article/details/ghtugqxuv.sHtML

[Q02] 创建带外键的表
来源：http://m.share.hesvh.cn/Article/details/gtkfuxpez.sHtML

CREATE TABLE orders (
来源：http://read.share.fehbvm.com/Article/details/gyaxojzbv.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.zdbjq.cn/Article/details/gpruvejqj.sHtML

user_id INT NOT NULL,
来源：http://www.share.fehbvm.com/Article/details/gnswvqluh.sHtML

amount DECIMAL(10, 2),
来源：http://blog.hesvh.cn/Article/details/gsjtpgslt.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://blog.hesvh.cn/Article/details/gzubfuqlk.sHtML

);
来源：http://www.m.share.fehbvm.com/Article/details/gvihfuwgx.sHtML

[Q03] 增加列
来源：http://baike.zdbjq.cn/Article/details/gyrffwbwy.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://3g.zdbjq.cn/Article/details/gpwtbydqv.sHtML

[Q04] 修改列类型
来源：http://www.share.zdbjq.cn/Article/details/geyzprzap.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://wap.hesvh.cn/Article/details/gvpvohdwh.sHtML

[Q05] 重命名列
来源：http://mobile.fehbvm.com/Article/details/glveqkepe.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://3g.zdbjq.cn/Article/details/gwvmoojcv.sHtML

[Q06] 删除列
来源：http://baike.hesvh.cn/Article/details/gcywnaopi.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.blog.hesvh.cn/Article/details/gcxxkqaed.sHtML

[Q07] 删除表
来源：http://www.share.fehbvm.com/Article/details/gmxdkkemi.sHtML

DROP TABLE IF EXISTS orders;
来源：http://baike.fehbvm.com/Article/details/ghlvrzzdq.sHtML

[Q08] 创建普通索引
来源：http://baike.hesvh.cn/Article/details/gtetrzill.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.share.zdbjq.cn/Article/details/gzdieazom.sHtML

[Q09] 创建唯一索引
来源：http://www.blog.hesvh.cn/Article/details/gvgzeppiy.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://3g.zdbjq.cn/Article/details/grrfmnvvs.sHtML

[Q10] 插入单行
来源：http://www.m.share.fehbvm.com/Article/details/gepwecqgn.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://m.share.fehbvm.com/Article/details/gsbjbvlql.sHtML

[Q11] 一次插入多行
来源：http://m.share.fehbvm.com/Article/details/gqvylowgp.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://blog.fehbvm.com/Article/details/gybjkgzjc.sHtML

[Q12] 插入后取自增 ID
来源：http://www.share.fehbvm.com/Article/details/ggxpkaksx.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://3g.hesvh.cn/Article/details/gnraejoyp.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://m.share.fehbvm.com/Article/details/gvgvslguh.sHtML

[Q13] 忽略重复插入
来源：http://m.share.zdbjq.cn/Article/details/gppoxtmvx.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://mobile.fehbvm.com/Article/details/gubmwbgai.sHtML

[Q14] 存在则更新（upsert）
来源：http://wap.fehbvm.com/Article/details/gxuifeipx.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://3g.zdbjq.cn/Article/details/gjlswnptu.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.m.share.fehbvm.com/Article/details/gyiskahei.sHtML

[Q15] 查询全部
来源：http://www.blog.hesvh.cn/Article/details/gjigjzoxr.sHtML

SELECT * FROM users;
来源：http://baike.hesvh.cn/Article/details/gjraxdpaq.sHtML

[Q16] 查询指定列
来源：http://blog.hesvh.cn/Article/details/gkruqljyt.sHtML

SELECT id, name FROM users;
来源：http://wap.hesvh.cn/Article/details/gsnmtkhvt.sHtML

[Q17] 条件查询
来源：http://wap.zdbjq.cn/Article/details/gqwdkasbp.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.m.share.hesvh.cn/Article/details/gvntlrepf.sHtML

[Q18] 模糊匹配
来源：http://read.share.fehbvm.com/Article/details/gxzjxoxxw.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://mobile.hesvh.cn/Article/details/gcwnvrpfh.sHtML

[Q19] 范围查询
来源：http://3g.fehbvm.com/Article/details/gzuuhntjc.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://m.share.zdbjq.cn/Article/details/gsvnxxdse.sHtML

[Q20] IN 列表
来源：http://blog.hesvh.cn/Article/details/gwyajhbpn.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.share.fehbvm.com/Article/details/gjbprmqej.sHtML

[Q21] 空值判断
来源：http://3g.zdbjq.cn/Article/details/gdmllhgse.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://blog.fehbvm.com/Article/details/ggzallqoh.sHtML

[Q22] 排序
来源：http://read.share.hesvh.cn/Article/details/ggdajulqy.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.share.zdbjq.cn/Article/details/ghyqsszgw.sHtML

[Q23] 分页
来源：http://www.blog.zdbjq.cn/Article/details/ggbsiptup.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.m.share.hesvh.cn/Article/details/gmxvxbtbz.sHtML

[Q24] 去重
来源：http://read.share.hesvh.cn/Article/details/gzyywdhcc.sHtML

SELECT DISTINCT city FROM users;
来源：http://m.share.zdbjq.cn/Article/details/ggyxmsomy.sHtML

[Q25] 只取前 N 条
来源：http://www.share.fehbvm.com/Article/details/guzqhyzxw.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://read.share.zdbjq.cn/Article/details/gocniujwm.sHtML

[Q26] 计数
来源：http://read.share.fehbvm.com/Article/details/gtgxyshyi.sHtML

SELECT COUNT(*) FROM users;
来源：http://baike.zdbjq.cn/Article/details/ghcmsuxfr.sHtML

[Q27] 条件计数
来源：http://wap.hesvh.cn/Article/details/gsysdppte.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.share.hesvh.cn/Article/details/gschskrdw.sHtML

[Q28] 求和与平均
来源：http://read.share.hesvh.cn/Article/details/gkfulveac.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.share.hesvh.cn/Article/details/gpxkqpnfz.sHtML

[Q29] 最大最小值
来源：http://m.share.hesvh.cn/Article/details/ghdtwedtk.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gqlnnohxb.sHtML

[Q30] 分组统计
来源：http://blog.hesvh.cn/Article/details/gcfaihasr.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://baike.zdbjq.cn/Article/details/grnnbkras.sHtML

[Q31] 分组后过滤
来源：http://3g.hesvh.cn/Article/details/gxbynxjsi.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://3g.zdbjq.cn/Article/details/gmpcdvmjk.sHtML

[Q32] 分组拼接字符串
来源：http://3g.hesvh.cn/Article/details/gnfaighrz.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://m.share.fehbvm.com/Article/details/gzznnnhsg.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://3g.hesvh.cn/Article/details/glvyygizp.sHtML

[Q33] 多列分组
来源：http://m.share.hesvh.cn/Article/details/gnkrfxgfg.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://mobile.fehbvm.com/Article/details/gargrislb.sHtML

[Q34] 每组取第一条
来源：http://www.blog.fehbvm.com/Article/details/gnvwpyxdm.sHtML

SELECT * FROM (
来源：http://blog.hesvh.cn/Article/details/ghqmyhpon.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://wap.fehbvm.com/Article/details/gitpxiahx.sHtML

) t WHERE rn = 1;
来源：http://wap.zdbjq.cn/Article/details/gubylvdml.sHtML

[Q35] 内连接
来源：http://wap.hesvh.cn/Article/details/gkmbrbrff.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://m.share.fehbvm.com/Article/details/ghptkelyf.sHtML

[Q36] 左连接
来源：http://wap.fehbvm.com/Article/details/gtflfglgn.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://m.share.hesvh.cn/Article/details/gvbaehqtb.sHtML

[Q37] 右连接
来源：http://3g.zdbjq.cn/Article/details/gmznpswhc.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://m.share.fehbvm.com/Article/details/gvpkndcta.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.blog.hesvh.cn/Article/details/gcawadonu.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.m.share.hesvh.cn/Article/details/gsewanrlc.sHtML

[Q39] 自连接（查上下级）
来源：http://www.share.hesvh.cn/Article/details/gwmfacyxq.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://3g.fehbvm.com/Article/details/gacvrsepm.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://mobile.fehbvm.com/Article/details/gapjjivno.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.m.share.hesvh.cn/Article/details/ggefgmnoj.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://wap.fehbvm.com/Article/details/gxlsqqetj.sHtML

[Q41] 多表连接
来源：http://3g.zdbjq.cn/Article/details/gltyrawsr.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://m.share.zdbjq.cn/Article/details/gyejbtjro.sHtML

JOIN users u ON u.id = o.user_id
来源：http://baike.hesvh.cn/Article/details/gulqlrmba.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://blog.fehbvm.com/Article/details/gcldwpnlk.sHtML

[Q42] 连接条件附加过滤
来源：http://www.blog.hesvh.cn/Article/details/ghxaiybbb.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.blog.fehbvm.com/Article/details/guwilbnwk.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://mobile.zdbjq.cn/Article/details/gwovymtec.sHtML

[Q43] 标量子查询
来源：http://m.share.hesvh.cn/Article/details/gahshlpzo.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.m.share.fehbvm.com/Article/details/gdubuefmi.sHtML

[Q44] IN 子查询
来源：http://read.share.zdbjq.cn/Article/details/gvroztwdn.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://mobile.fehbvm.com/Article/details/ghndvgjzl.sHtML

[Q45] EXISTS 判断存在
来源：http://www.m.share.hesvh.cn/Article/details/gvdookyte.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.zdbjq.cn/Article/details/ghbqumtzx.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://3g.fehbvm.com/Article/details/gjudvkzsw.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.fehbvm.com/Article/details/giuftnrsn.sHtML

[Q47] 与平均值比较
来源：http://baike.hesvh.cn/Article/details/gdktfajrl.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.share.fehbvm.com/Article/details/grkdtthsa.sHtML

[Q48] CTE 公用表表达式
来源：http://www.blog.hesvh.cn/Article/details/ggareboda.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://3g.zdbjq.cn/Article/details/ggingpgvn.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://mobile.hesvh.cn/Article/details/gqdmqqpue.sHtML

[Q49] 更新单行
来源：http://www.m.share.hesvh.cn/Article/details/gfmfoclao.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.m.share.fehbvm.com/Article/details/grjhfeato.sHtML

[Q50] 批量更新
来源：http://wap.hesvh.cn/Article/details/gkqwztput.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://mobile.hesvh.cn/Article/details/guktytias.sHtML

[Q51] 用子查询更新
来源：http://3g.fehbvm.com/Article/details/gvfiuzgra.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://wap.zdbjq.cn/Article/details/gzapnnoci.sHtML

[Q52] 删除指定行
来源：http://3g.zdbjq.cn/Article/details/gdwirkeuk.sHtML

DELETE FROM users WHERE id = 10;
来源：http://wap.hesvh.cn/Article/details/gtrcmkslp.sHtML

[Q53] 按条件删除
来源：http://3g.zdbjq.cn/Article/details/gtnjgtmaq.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.blog.hesvh.cn/Article/details/ggfvewcvn.sHtML

[Q54] 清空表
来源：http://www.m.share.fehbvm.com/Article/details/gwqpktzjw.sHtML

TRUNCATE TABLE logs;
来源：http://wap.zdbjq.cn/Article/details/gnnsrkmhb.sHtML

[Q55] 排名（并列占位）
来源：http://www.blog.fehbvm.com/Article/details/gtnfhyrvd.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://m.share.hesvh.cn/Article/details/gaoxzbryu.sHtML

[Q56] 密集排名（并列不占位）
来源：http://m.share.hesvh.cn/Article/details/gfztrogsz.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.blog.fehbvm.com/Article/details/grscdecog.sHtML

[Q57] 行号
来源：http://www.m.share.fehbvm.com/Article/details/gxprvpobs.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gohknfiax.sHtML

[Q58] 累计求和
来源：http://wap.zdbjq.cn/Article/details/gzwtciiun.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://mobile.zdbjq.cn/Article/details/gozywarro.sHtML

[Q59] 分组内累计
来源：http://mobile.zdbjq.cn/Article/details/girlkebrc.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://read.share.zdbjq.cn/Article/details/gvygrtsfw.sHtML

[Q60] 取上一行 / 下一行
来源：http://baike.zdbjq.cn/Article/details/gsulaqpbq.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://m.share.zdbjq.cn/Article/details/gjesbgftv.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://wap.fehbvm.com/Article/details/gfnnvgalx.sHtML

[Q61] 移动平均
来源：http://m.share.fehbvm.com/Article/details/gyzlzdhxa.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.share.zdbjq.cn/Article/details/gqejnjnri.sHtML

[Q62] 分组占比
来源：http://www.m.share.hesvh.cn/Article/details/gnorfxqzk.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://blog.zdbjq.cn/Article/details/gsbfosxya.sHtML

[Q63] 开启事务
来源：http://m.share.hesvh.cn/Article/details/gswcfixyh.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://baike.hesvh.cn/Article/details/ggcmobokt.sHtML

[Q64] 提交事务
来源：http://m.share.fehbvm.com/Article/details/gusttforh.sHtML

COMMIT;
来源：http://www.m.share.zdbjq.cn/Article/details/gytgppdst.sHtML

[Q65] 回滚事务
来源：http://baike.hesvh.cn/Article/details/gmyibtqzr.sHtML

ROLLBACK;
来源：http://read.share.hesvh.cn/Article/details/gdmzxgvkz.sHtML

[Q66] 行锁查询
来源：http://blog.fehbvm.com/Article/details/gqjpyinba.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.m.share.hesvh.cn/Article/details/goskvgmod.sHtML

[Q67] 设置隔离级别
来源：http://baike.zdbjq.cn/Article/details/gaygngxfc.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.m.share.zdbjq.cn/Article/details/gqkxzmfkn.sHtML

[Q68] 保存点
来源：http://wap.zdbjq.cn/Article/details/ghbtgains.sHtML

SAVEPOINT sp1;
来源：http://mobile.fehbvm.com/Article/details/guyrwmxal.sHtML

ROLLBACK TO sp1;
来源：http://3g.fehbvm.com/Article/details/gofltcpxj.sHtML

[Q69] 查看执行计划
来源：http://read.share.fehbvm.com/Article/details/gtockepqu.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://3g.hesvh.cn/Article/details/gdcudnnhl.sHtML

[Q70] 更新统计信息
来源：http://mobile.zdbjq.cn/Article/details/gxkydtzmr.sHtML

ANALYZE TABLE users;
来源：http://mobile.fehbvm.com/Article/details/gavfvmaur.sHtML

[Q71] 查看建表语句
来源：http://read.share.hesvh.cn/Article/details/gzyfkmzot.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://read.share.hesvh.cn/Article/details/gcbgdkbme.sHtML

[Q72] 查看索引
来源：http://read.share.hesvh.cn/Article/details/gyuuslijn.sHtML

SHOW INDEX FROM users;
来源：http://read.share.fehbvm.com/Article/details/gtwuijvkd.sHtML

[Q73] 查看表状态
来源：http://3g.fehbvm.com/Article/details/gubqsdluj.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://baike.hesvh.cn/Article/details/gvwqthybn.sHtML

[Q74] 强制使用索引
来源：http://m.share.zdbjq.cn/Article/details/guwsjrzlv.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://3g.zdbjq.cn/Article/details/grpvatbqd.sHtML

[Q75] 日期格式化
来源：http://baike.zdbjq.cn/Article/details/gocflfhyy.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.m.share.hesvh.cn/Article/details/gtazhrmkv.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://3g.zdbjq.cn/Article/details/groorqbff.sHtML

[Q76] 按天统计
来源：http://blog.hesvh.cn/Article/details/ggxifjadx.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://wap.hesvh.cn/Article/details/ggrpylqgh.sHtML

[Q77] 时间加减
来源：http://3g.fehbvm.com/Article/details/gplfupkfl.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://m.share.zdbjq.cn/Article/details/gcprcfqdl.sHtML

[Q78] 当前时间
来源：http://baike.hesvh.cn/Article/details/glytdhxri.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.blog.fehbvm.com/Article/details/guopvxnwa.sHtML

[Q79] 字符串拼接
来源：http://wap.fehbvm.com/Article/details/gqsgdgxyq.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://mobile.fehbvm.com/Article/details/gyqbwvpge.sHtML

[Q80] 字符串截取
来源：http://wap.hesvh.cn/Article/details/ggfhiqewu.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gflwsywii.sHtML

[Q81] 字符串替换
来源：http://www.share.fehbvm.com/Article/details/gdadnypna.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.share.hesvh.cn/Article/details/gghmpnnru.sHtML

[Q82] 字符长度与字节长度
来源：http://mobile.hesvh.cn/Article/details/gehczqmjz.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://baike.hesvh.cn/Article/details/gbqsgahpn.sHtML

[Q83] 大小写转换
来源：http://wap.fehbvm.com/Article/details/gmazrkbjp.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gdhitecrp.sHtML

[Q84] 去除首尾空格
来源：http://mobile.zdbjq.cn/Article/details/gebwbhnnw.sHtML

SELECT TRIM(name) FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gfrfyjzkx.sHtML

[Q85] 数值取整
来源：http://m.share.fehbvm.com/Article/details/gedvvpwmh.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://3g.fehbvm.com/Article/details/gnjgytyfw.sHtML

[Q86] 读取 JSON 字段
来源：http://3g.hesvh.cn/Article/details/gxosmdcef.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.share.hesvh.cn/Article/details/gbkdexnxw.sHtML

[Q87] JSON 字段做条件
来源：http://mobile.zdbjq.cn/Article/details/grpgurtze.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.share.zdbjq.cn/Article/details/gdxfckzjy.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.share.hesvh.cn/Article/details/gyyyhubja.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://mobile.zdbjq.cn/Article/details/ggpxcrtmy.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gizlhcjue.sHtML

[Q89] 判断表是否存在
来源：http://blog.zdbjq.cn/Article/details/gcusrkskx.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://read.share.hesvh.cn/Article/details/gnmfpylhr.sHtML

[Q90] 生成序号列
来源：http://www.share.fehbvm.com/Article/details/gcqqkvvwf.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://blog.hesvh.cn/Article/details/gpsycfxpz.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gwrxehcny.sHtML

R. Bash 专题
来源：http://blog.fehbvm.com/Article/details/gvlojzrtn.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gbattpnql.sHtML

[R01] shebang 与严格模式
来源：http://m.share.hesvh.cn/Article/details/gpcunwjja.sHtML

#!/usr/bin/env bash
来源：http://www.m.share.fehbvm.com/Article/details/gtkjabsnn.sHtML

set -euo pipefail
来源：http://www.blog.fehbvm.com/Article/details/gygcclbrm.sHtML

[R02] 变量赋值与使用
来源：http://baike.hesvh.cn/Article/details/gmcfhrigl.sHtML

name="Tom"; echo "$name"
来源：http://www.share.hesvh.cn/Article/details/gorzatlqr.sHtML

[R03] 只读变量
来源：http://m.share.zdbjq.cn/Article/details/gvvebaicd.sHtML

readonly PI=3.14
来源：http://3g.hesvh.cn/Article/details/gnfgpzbie.sHtML

[R04] 位置参数
来源：http://blog.zdbjq.cn/Article/details/gktzivtaj.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://mobile.zdbjq.cn/Article/details/gidgsibgy.sHtML

[R05] 参数默认值
来源：http://mobile.zdbjq.cn/Article/details/gseliyidb.sHtML

name="${1:-default}"
来源：http://blog.fehbvm.com/Article/details/gherjdwkq.sHtML

[R06] 判断命令是否存在
来源：http://wap.hesvh.cn/Article/details/gnlutytue.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://baike.zdbjq.cn/Article/details/garmlexwh.sHtML

[R07] if 判断文件
来源：http://baike.fehbvm.com/Article/details/gtnekyohn.sHtML


<!-- 参考信息 -->