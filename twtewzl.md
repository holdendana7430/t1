代发 wailian999

C#:   Parallel.For
来源：http://www.share.zdbjq.cn/Article/details/gcblsbmrz.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gwiqhrxeo.sHtML

P. 常用工具函数
来源：http://baike.hesvh.cn/Article/details/grcwryyba.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gvtdbkieu.sHtML

[P01] 生成 UUID
来源：http://www.m.share.fehbvm.com/Article/details/gbodvdbcu.sHtML

Py:   str(uuid.uuid4())
来源：http://m.share.zdbjq.cn/Article/details/ghisoktvj.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://read.share.zdbjq.cn/Article/details/gkxvvbrzq.sHtML

JS:   crypto.randomUUID()
来源：http://baike.hesvh.cn/Article/details/gnzchkpdf.sHtML

TS:   crypto.randomUUID()
来源：http://www.m.share.hesvh.cn/Article/details/giqydqtie.sHtML

Java: UUID.randomUUID().toString()
来源：http://m.share.zdbjq.cn/Article/details/gowvcrykb.sHtML

Go:   // 用 github.com/google/uuid
来源：http://baike.fehbvm.com/Article/details/gtjwwsllq.sHtML

Ruby: SecureRandom.uuid
来源：http://www.blog.hesvh.cn/Article/details/gdmfrjqqp.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://read.share.hesvh.cn/Article/details/gvdyaiwtk.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.share.fehbvm.com/Article/details/ghxhuesek.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://wap.zdbjq.cn/Article/details/ghjsyrmim.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.m.share.hesvh.cn/Article/details/gjobnzcuq.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://read.share.zdbjq.cn/Article/details/gmijaojpk.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.m.share.zdbjq.cn/Article/details/giripwicy.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.blog.hesvh.cn/Article/details/gldonnxlm.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://3g.fehbvm.com/Article/details/gijuvuorj.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://wap.hesvh.cn/Article/details/gzmmqdzkv.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://wap.hesvh.cn/Article/details/gzqljquvs.sHtML

[P03] 生成短随机字符串
来源：http://read.share.zdbjq.cn/Article/details/gouaxqtex.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://read.share.hesvh.cn/Article/details/getofqceu.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.blog.fehbvm.com/Article/details/gpuqpnqjn.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.fehbvm.com/Article/details/girqctyjz.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.zdbjq.cn/Article/details/gkboshllo.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://baike.fehbvm.com/Article/details/gbugpvzpy.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://baike.hesvh.cn/Article/details/ghvtulwlz.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.blog.zdbjq.cn/Article/details/glpjpvblp.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.m.share.zdbjq.cn/Article/details/gyndllelt.sHtML

[P04] 求长度
来源：http://baike.fehbvm.com/Article/details/gksgxgadk.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.share.hesvh.cn/Article/details/gwdzxbufa.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.zdbjq.cn/Article/details/gwtcddjws.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mobile.fehbvm.com/Article/details/gvtgmuiwm.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.fehbvm.com/Article/details/gmyknqldp.sHtML

Java: list.size();  map.size();  s.length()
来源：http://wap.zdbjq.cn/Article/details/grzhjowcj.sHtML

Go:   len(arr);  len(m)
来源：http://blog.fehbvm.com/Article/details/gsfkgqvly.sHtML

Ruby: x.length;  x.size
来源：http://m.share.fehbvm.com/Article/details/gcgarifzx.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.share.fehbvm.com/Article/details/ghxalojwl.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.blog.zdbjq.cn/Article/details/gxydvgcee.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://3g.fehbvm.com/Article/details/gjgfhocvl.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://read.share.fehbvm.com/Article/details/ggizbchho.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://baike.fehbvm.com/Article/details/gjrlglqat.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.zdbjq.cn/Article/details/glkszwvew.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.blog.zdbjq.cn/Article/details/gvkuxqczt.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.blog.hesvh.cn/Article/details/gfbmphkbr.sHtML

Ruby: a == b
来源：http://baike.zdbjq.cn/Article/details/glnysxpyr.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.m.share.fehbvm.com/Article/details/ggpwmhwuk.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.blog.fehbvm.com/Article/details/gisohpwvh.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://blog.zdbjq.cn/Article/details/gdfmbmmti.sHtML

PHP:  if (empty($x)) {}
来源：http://www.m.share.fehbvm.com/Article/details/gohfwulxv.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.m.share.fehbvm.com/Article/details/gcwuaibvd.sHtML

TS:   if (x == null) {}
来源：http://wap.fehbvm.com/Article/details/gyuifslzp.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://m.share.hesvh.cn/Article/details/glmfquftp.sHtML

Go:   if x == nil {}
来源：http://mobile.zdbjq.cn/Article/details/glcjlldkv.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.share.zdbjq.cn/Article/details/gxqfmdauu.sHtML

C#:   if (x is null) {}
来源：http://baike.fehbvm.com/Article/details/ggwmjtjjh.sHtML

[P07] 防抖与节流
来源：http://www.share.hesvh.cn/Article/details/grlhakxti.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.share.fehbvm.com/Article/details/glzqqhdoh.sHtML

PHP:  // 手写时间戳比较
来源：http://www.share.hesvh.cn/Article/details/gejljpxhu.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.fehbvm.com/Article/details/gfysprdmm.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.fehbvm.com/Article/details/girnyfsme.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://3g.fehbvm.com/Article/details/gonxxtyac.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://wap.zdbjq.cn/Article/details/gdzdkwryf.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://blog.fehbvm.com/Article/details/gbslysipb.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://baike.zdbjq.cn/Article/details/gnxvtjhnw.sHtML

[P08] 处理浮点精度问题
来源：http://www.share.hesvh.cn/Article/details/goynqjoij.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://m.share.fehbvm.com/Article/details/gsliburjc.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://m.share.zdbjq.cn/Article/details/glywvmpmc.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.share.hesvh.cn/Article/details/gbsupimnu.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.blog.fehbvm.com/Article/details/gvbytpkdj.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://m.share.hesvh.cn/Article/details/govudrgxw.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://wap.fehbvm.com/Article/details/gprudiebn.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.m.share.fehbvm.com/Article/details/gsqzxwvzw.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.blog.fehbvm.com/Article/details/goypbisnh.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/galeuktuy.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://mobile.fehbvm.com/Article/details/gtwrmxnyo.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gqcwexmsg.sHtML

[Q01] 创建表
来源：http://wap.fehbvm.com/Article/details/gmwhgkkku.sHtML

CREATE TABLE users (
来源：http://3g.hesvh.cn/Article/details/gsteygxbu.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.zdbjq.cn/Article/details/gyweguxuy.sHtML

name VARCHAR(50) NOT NULL,
来源：http://baike.fehbvm.com/Article/details/gfsqpudmw.sHtML

email VARCHAR(100) UNIQUE,
来源：http://read.share.fehbvm.com/Article/details/guarlwcic.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://3g.hesvh.cn/Article/details/gfuewzzcr.sHtML

);
来源：http://mobile.hesvh.cn/Article/details/gzpfsekev.sHtML

[Q02] 创建带外键的表
来源：http://blog.zdbjq.cn/Article/details/gzsswagvr.sHtML

CREATE TABLE orders (
来源：http://mobile.zdbjq.cn/Article/details/galqpqxev.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.hesvh.cn/Article/details/givdjrsot.sHtML

user_id INT NOT NULL,
来源：http://www.m.share.zdbjq.cn/Article/details/gruwssare.sHtML

amount DECIMAL(10, 2),
来源：http://read.share.fehbvm.com/Article/details/gvfbvnvev.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.blog.zdbjq.cn/Article/details/gtngfotqx.sHtML

);
来源：http://mobile.hesvh.cn/Article/details/gtviexxvj.sHtML

[Q03] 增加列
来源：http://baike.fehbvm.com/Article/details/gzdqryrcn.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.share.zdbjq.cn/Article/details/gpvusyvtb.sHtML

[Q04] 修改列类型
来源：http://www.m.share.zdbjq.cn/Article/details/gmufpvddc.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://mobile.fehbvm.com/Article/details/gurhhcesm.sHtML

[Q05] 重命名列
来源：http://m.share.hesvh.cn/Article/details/gnaaaqfwe.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://read.share.zdbjq.cn/Article/details/gwqmypndh.sHtML

[Q06] 删除列
来源：http://baike.zdbjq.cn/Article/details/gaqrsrlji.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://baike.zdbjq.cn/Article/details/gskzaizom.sHtML

[Q07] 删除表
来源：http://www.blog.hesvh.cn/Article/details/gpyowjpuc.sHtML

DROP TABLE IF EXISTS orders;
来源：http://read.share.fehbvm.com/Article/details/gjdncuxep.sHtML

[Q08] 创建普通索引
来源：http://3g.hesvh.cn/Article/details/gqlfdymze.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://read.share.zdbjq.cn/Article/details/gxpsxfskt.sHtML

[Q09] 创建唯一索引
来源：http://blog.fehbvm.com/Article/details/gkywsnbzo.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.m.share.fehbvm.com/Article/details/gurrufico.sHtML

[Q10] 插入单行
来源：http://wap.fehbvm.com/Article/details/ggfolnjly.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://read.share.fehbvm.com/Article/details/gmbdjrhhk.sHtML

[Q11] 一次插入多行
来源：http://wap.hesvh.cn/Article/details/gygrifixg.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://read.share.zdbjq.cn/Article/details/gnzzlrihf.sHtML

[Q12] 插入后取自增 ID
来源：http://www.m.share.hesvh.cn/Article/details/gwsbkvmda.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://baike.fehbvm.com/Article/details/gxjnldrtx.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://read.share.hesvh.cn/Article/details/gfpuyrbtk.sHtML

[Q13] 忽略重复插入
来源：http://blog.zdbjq.cn/Article/details/gdtlsujqd.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://3g.zdbjq.cn/Article/details/gggsywylz.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.blog.hesvh.cn/Article/details/gyprevmwy.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://baike.zdbjq.cn/Article/details/gmlinwpdl.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://wap.fehbvm.com/Article/details/gfbqasjei.sHtML

[Q15] 查询全部
来源：http://m.share.hesvh.cn/Article/details/gdicgdswe.sHtML

SELECT * FROM users;
来源：http://read.share.fehbvm.com/Article/details/gdhpwhqdn.sHtML

[Q16] 查询指定列
来源：http://wap.zdbjq.cn/Article/details/gkayagvhh.sHtML

SELECT id, name FROM users;
来源：http://www.share.hesvh.cn/Article/details/gxbsqppmm.sHtML

[Q17] 条件查询
来源：http://www.share.hesvh.cn/Article/details/glekaxhvl.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.share.fehbvm.com/Article/details/ghronzjbu.sHtML

[Q18] 模糊匹配
来源：http://m.share.fehbvm.com/Article/details/gjgnaltsl.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://3g.hesvh.cn/Article/details/grqwxdmbe.sHtML

[Q19] 范围查询
来源：http://www.blog.hesvh.cn/Article/details/ghpkktdzw.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.m.share.zdbjq.cn/Article/details/ggyganwrr.sHtML

[Q20] IN 列表
来源：http://www.m.share.hesvh.cn/Article/details/ggctjaczq.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.m.share.hesvh.cn/Article/details/golbycavf.sHtML

[Q21] 空值判断
来源：http://www.m.share.fehbvm.com/Article/details/gjjzmygid.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://m.share.hesvh.cn/Article/details/ggtxmxjmv.sHtML

[Q22] 排序
来源：http://wap.zdbjq.cn/Article/details/gbwhlmtca.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://m.share.hesvh.cn/Article/details/gnynbxtox.sHtML

[Q23] 分页
来源：http://www.m.share.fehbvm.com/Article/details/gquqlpwlg.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.m.share.fehbvm.com/Article/details/gjzpwuvgb.sHtML

[Q24] 去重
来源：http://blog.zdbjq.cn/Article/details/gqkxpumau.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gnxmtkscu.sHtML

[Q25] 只取前 N 条
来源：http://www.share.hesvh.cn/Article/details/gnrfcldag.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://m.share.zdbjq.cn/Article/details/gvztxromw.sHtML

[Q26] 计数
来源：http://www.m.share.fehbvm.com/Article/details/griaglqwf.sHtML

SELECT COUNT(*) FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gmholnaeg.sHtML

[Q27] 条件计数
来源：http://www.share.zdbjq.cn/Article/details/gnjcbhgai.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://wap.hesvh.cn/Article/details/gyqxwgehv.sHtML

[Q28] 求和与平均
来源：http://www.m.share.hesvh.cn/Article/details/gkoczictu.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://m.share.hesvh.cn/Article/details/gzlajpupk.sHtML

[Q29] 最大最小值
来源：http://www.blog.hesvh.cn/Article/details/gqodbgbjb.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://wap.fehbvm.com/Article/details/gjhcjlbrh.sHtML

[Q30] 分组统计
来源：http://3g.hesvh.cn/Article/details/grkbuiibx.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.share.hesvh.cn/Article/details/gecjyecoy.sHtML

[Q31] 分组后过滤
来源：http://m.share.zdbjq.cn/Article/details/gvwqntkbu.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://read.share.fehbvm.com/Article/details/grtroluza.sHtML

[Q32] 分组拼接字符串
来源：http://www.m.share.fehbvm.com/Article/details/gfkcchsrs.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://3g.hesvh.cn/Article/details/gfuqnkgxm.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.share.fehbvm.com/Article/details/gttpplobk.sHtML

[Q33] 多列分组
来源：http://www.share.fehbvm.com/Article/details/gmhwaatbe.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://mobile.fehbvm.com/Article/details/gopdftkni.sHtML

[Q34] 每组取第一条
来源：http://m.share.zdbjq.cn/Article/details/gqxdhotpq.sHtML

SELECT * FROM (
来源：http://read.share.zdbjq.cn/Article/details/gcpmmfmgb.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.m.share.hesvh.cn/Article/details/gjdbegxfz.sHtML

) t WHERE rn = 1;
来源：http://www.m.share.zdbjq.cn/Article/details/gstgxonlc.sHtML

[Q35] 内连接
来源：http://blog.hesvh.cn/Article/details/ggnembetw.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.hesvh.cn/Article/details/gwlyyksde.sHtML

[Q36] 左连接
来源：http://blog.fehbvm.com/Article/details/gmmkxresf.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://baike.fehbvm.com/Article/details/grnxnssdx.sHtML

[Q37] 右连接
来源：http://read.share.fehbvm.com/Article/details/gmjzwvvpt.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://3g.fehbvm.com/Article/details/gwxzbzjip.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://blog.zdbjq.cn/Article/details/gikumcsbd.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://blog.hesvh.cn/Article/details/ghhriyfxu.sHtML

[Q39] 自连接（查上下级）
来源：http://baike.fehbvm.com/Article/details/gsiyszyqv.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://m.share.zdbjq.cn/Article/details/gimbtguui.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://baike.zdbjq.cn/Article/details/gfexvbjjx.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://m.share.zdbjq.cn/Article/details/ggzvjaiwq.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://mobile.fehbvm.com/Article/details/gdeggweui.sHtML

[Q41] 多表连接
来源：http://wap.zdbjq.cn/Article/details/gzqpxiuwd.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://baike.fehbvm.com/Article/details/gusmqbvda.sHtML

JOIN users u ON u.id = o.user_id
来源：http://baike.hesvh.cn/Article/details/gjglolzrv.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://m.share.hesvh.cn/Article/details/goidorvam.sHtML

[Q42] 连接条件附加过滤
来源：http://www.blog.zdbjq.cn/Article/details/gpawlarij.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.blog.hesvh.cn/Article/details/ghnxkkyxk.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://blog.zdbjq.cn/Article/details/gloqghqow.sHtML

[Q43] 标量子查询
来源：http://blog.fehbvm.com/Article/details/gwzmpyxed.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://3g.hesvh.cn/Article/details/gwqpycxve.sHtML

[Q44] IN 子查询
来源：http://read.share.hesvh.cn/Article/details/gqjokqnnh.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.blog.hesvh.cn/Article/details/gysuyfcne.sHtML

[Q45] EXISTS 判断存在
来源：http://3g.zdbjq.cn/Article/details/gpestydmc.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.zdbjq.cn/Article/details/gsvaotycr.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://3g.hesvh.cn/Article/details/gkmmmfitp.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.hesvh.cn/Article/details/gpfsjcbok.sHtML

[Q47] 与平均值比较
来源：http://baike.zdbjq.cn/Article/details/gnpuowasw.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.m.share.zdbjq.cn/Article/details/gsvopirhm.sHtML

[Q48] CTE 公用表表达式
来源：http://wap.fehbvm.com/Article/details/gabrrwrqn.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://blog.hesvh.cn/Article/details/gcvudjiqj.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://blog.fehbvm.com/Article/details/gcsqvpnmt.sHtML

[Q49] 更新单行
来源：http://mobile.hesvh.cn/Article/details/gooabkwrd.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://baike.zdbjq.cn/Article/details/ghwapmift.sHtML

[Q50] 批量更新
来源：http://blog.hesvh.cn/Article/details/ggherbhfh.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://mobile.zdbjq.cn/Article/details/gxhctgtyj.sHtML

[Q51] 用子查询更新
来源：http://mobile.hesvh.cn/Article/details/gphbkltgi.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.m.share.fehbvm.com/Article/details/gpylqvmgg.sHtML

[Q52] 删除指定行
来源：http://m.share.zdbjq.cn/Article/details/gwuzfalrv.sHtML

DELETE FROM users WHERE id = 10;
来源：http://read.share.hesvh.cn/Article/details/guucxeekw.sHtML

[Q53] 按条件删除
来源：http://read.share.fehbvm.com/Article/details/gpvqarvvj.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://read.share.fehbvm.com/Article/details/gkqffucxv.sHtML

[Q54] 清空表
来源：http://baike.hesvh.cn/Article/details/glptofhub.sHtML

TRUNCATE TABLE logs;
来源：http://blog.zdbjq.cn/Article/details/gzgeusuiz.sHtML

[Q55] 排名（并列占位）
来源：http://blog.fehbvm.com/Article/details/gajevllde.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.m.share.hesvh.cn/Article/details/gxtjbraps.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.blog.zdbjq.cn/Article/details/gnfzbzigm.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://read.share.fehbvm.com/Article/details/gtyxnrvkp.sHtML

[Q57] 行号
来源：http://baike.fehbvm.com/Article/details/ghqhidydd.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gmvlizkro.sHtML

[Q58] 累计求和
来源：http://www.blog.zdbjq.cn/Article/details/gfmcjzczq.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.share.zdbjq.cn/Article/details/gapdzibkb.sHtML

[Q59] 分组内累计
来源：http://mobile.fehbvm.com/Article/details/gpytprurz.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://3g.fehbvm.com/Article/details/gpnpefrxk.sHtML

[Q60] 取上一行 / 下一行
来源：http://wap.zdbjq.cn/Article/details/gouiaxgca.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.blog.zdbjq.cn/Article/details/gsxhnzdwv.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://m.share.hesvh.cn/Article/details/gjricoxht.sHtML

[Q61] 移动平均
来源：http://3g.fehbvm.com/Article/details/giyntugex.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://read.share.fehbvm.com/Article/details/glxdkmvfr.sHtML

[Q62] 分组占比
来源：http://www.blog.fehbvm.com/Article/details/gsxlocctl.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://wap.zdbjq.cn/Article/details/glfwwjucz.sHtML

[Q63] 开启事务
来源：http://www.blog.zdbjq.cn/Article/details/gbivyhcnx.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.blog.fehbvm.com/Article/details/gsriceeqf.sHtML

[Q64] 提交事务
来源：http://mobile.hesvh.cn/Article/details/glbfkafub.sHtML

COMMIT;
来源：http://blog.fehbvm.com/Article/details/gfetrqqeq.sHtML

[Q65] 回滚事务
来源：http://blog.zdbjq.cn/Article/details/gfnzjgqbs.sHtML

ROLLBACK;
来源：http://read.share.hesvh.cn/Article/details/gftqnrzqx.sHtML

[Q66] 行锁查询
来源：http://m.share.zdbjq.cn/Article/details/gpxgzfcud.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.m.share.zdbjq.cn/Article/details/goziblonq.sHtML

[Q67] 设置隔离级别
来源：http://blog.hesvh.cn/Article/details/gqesipjrw.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://baike.hesvh.cn/Article/details/gvpoommku.sHtML

[Q68] 保存点
来源：http://baike.zdbjq.cn/Article/details/gklqegvkw.sHtML

SAVEPOINT sp1;
来源：http://www.share.hesvh.cn/Article/details/gwzsriijx.sHtML

ROLLBACK TO sp1;
来源：http://www.m.share.fehbvm.com/Article/details/gfmlwuteu.sHtML

[Q69] 查看执行计划
来源：http://mobile.fehbvm.com/Article/details/gslnzlrry.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://3g.fehbvm.com/Article/details/gvhjzgowm.sHtML

[Q70] 更新统计信息
来源：http://wap.zdbjq.cn/Article/details/gsfxiggha.sHtML

ANALYZE TABLE users;
来源：http://read.share.fehbvm.com/Article/details/gzeczryyw.sHtML

[Q71] 查看建表语句
来源：http://www.share.fehbvm.com/Article/details/grbjdtfux.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://blog.fehbvm.com/Article/details/gkgsyieqm.sHtML

[Q72] 查看索引
来源：http://read.share.fehbvm.com/Article/details/gsjkvusva.sHtML

SHOW INDEX FROM users;
来源：http://read.share.fehbvm.com/Article/details/gvlahcpbh.sHtML

[Q73] 查看表状态
来源：http://www.blog.hesvh.cn/Article/details/gjoubajet.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://wap.hesvh.cn/Article/details/ggvgusowc.sHtML

[Q74] 强制使用索引
来源：http://wap.hesvh.cn/Article/details/guvkefrhh.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://mobile.zdbjq.cn/Article/details/gxmkeihrk.sHtML

[Q75] 日期格式化
来源：http://www.blog.zdbjq.cn/Article/details/gvvojecup.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://read.share.hesvh.cn/Article/details/glojklddh.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://read.share.zdbjq.cn/Article/details/ghxgioqbj.sHtML

[Q76] 按天统计
来源：http://www.m.share.hesvh.cn/Article/details/gfxrsizjc.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://wap.hesvh.cn/Article/details/gjbzipovk.sHtML

[Q77] 时间加减
来源：http://mobile.fehbvm.com/Article/details/guatbgimp.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://wap.fehbvm.com/Article/details/gjbfnjqbm.sHtML

[Q78] 当前时间
来源：http://www.m.share.hesvh.cn/Article/details/gmcdnpjwb.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://blog.zdbjq.cn/Article/details/gsmmjfnsa.sHtML

[Q79] 字符串拼接
来源：http://www.m.share.fehbvm.com/Article/details/gdmscbsmw.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.share.zdbjq.cn/Article/details/guabmscol.sHtML

[Q80] 字符串截取
来源：http://wap.hesvh.cn/Article/details/gxzsyccrb.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://blog.fehbvm.com/Article/details/gdiiezdfi.sHtML

[Q81] 字符串替换
来源：http://www.blog.fehbvm.com/Article/details/glxzrzghm.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://wap.zdbjq.cn/Article/details/gkcdoacya.sHtML

[Q82] 字符长度与字节长度
来源：http://read.share.hesvh.cn/Article/details/gzkkgkkyb.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://mobile.hesvh.cn/Article/details/gndelenwh.sHtML

[Q83] 大小写转换
来源：http://m.share.zdbjq.cn/Article/details/guzwthyft.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gabldjayh.sHtML

[Q84] 去除首尾空格
来源：http://wap.fehbvm.com/Article/details/gebvfnylr.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gyaaqemyc.sHtML

[Q85] 数值取整
来源：http://wap.zdbjq.cn/Article/details/gaygulelc.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.blog.zdbjq.cn/Article/details/gijzixlyu.sHtML

[Q86] 读取 JSON 字段
来源：http://www.blog.hesvh.cn/Article/details/gcbwisnei.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://blog.fehbvm.com/Article/details/gikzoblee.sHtML

[Q87] JSON 字段做条件
来源：http://read.share.fehbvm.com/Article/details/ghyqadrhf.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://wap.fehbvm.com/Article/details/guyppjylp.sHtML

[Q88] 行转列（条件聚合）
来源：http://mobile.fehbvm.com/Article/details/gykclnrxb.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://baike.hesvh.cn/Article/details/gfpxuabgn.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gzxgpvzkm.sHtML

[Q89] 判断表是否存在
来源：http://baike.hesvh.cn/Article/details/gwcvfkedx.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.share.fehbvm.com/Article/details/ghxwvuztd.sHtML

[Q90] 生成序号列
来源：http://mobile.hesvh.cn/Article/details/gfrfvtwad.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://mobile.fehbvm.com/Article/details/grdhwcgxm.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gbcoegimd.sHtML

R. Bash 专题
来源：http://baike.fehbvm.com/Article/details/gxxdvzhyx.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gpbovklam.sHtML

[R01] shebang 与严格模式
来源：http://www.share.fehbvm.com/Article/details/gaeqkmagq.sHtML

#!/usr/bin/env bash
来源：http://mobile.hesvh.cn/Article/details/grsygpbre.sHtML

set -euo pipefail
来源：http://baike.hesvh.cn/Article/details/gcsmtihec.sHtML

[R02] 变量赋值与使用
来源：http://www.m.share.zdbjq.cn/Article/details/gftcuyvpg.sHtML

name="Tom"; echo "$name"
来源：http://3g.zdbjq.cn/Article/details/gkmoedmkh.sHtML

[R03] 只读变量
来源：http://wap.hesvh.cn/Article/details/gbspggzut.sHtML

readonly PI=3.14
来源：http://www.share.hesvh.cn/Article/details/gwmtwhqsm.sHtML

[R04] 位置参数
来源：http://blog.fehbvm.com/Article/details/gtvadlnhf.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://wap.hesvh.cn/Article/details/ghxqhuxsu.sHtML

[R05] 参数默认值
来源：http://www.share.hesvh.cn/Article/details/gqcpravvg.sHtML

name="${1:-default}"
来源：http://m.share.zdbjq.cn/Article/details/gdvxuoktq.sHtML

[R06] 判断命令是否存在
来源：http://mobile.hesvh.cn/Article/details/gpvhydbzc.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.m.share.zdbjq.cn/Article/details/gppxuwkmi.sHtML

[R07] if 判断文件
来源：http://mobile.hesvh.cn/Article/details/gojhkdnek.sHtML


<!-- 参考信息 -->