代发 wailian999

C#:   Parallel.For
来源：http://www.share.hesvh.cn/Article/details/gbvjywixp.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gvstktdkm.sHtML

P. 常用工具函数
来源：http://read.share.fehbvm.com/Article/details/gtowwmodq.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gjlykitnf.sHtML

[P01] 生成 UUID
来源：http://wap.fehbvm.com/Article/details/gichefigx.sHtML

Py:   str(uuid.uuid4())
来源：http://blog.fehbvm.com/Article/details/gqkwebaro.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://baike.zdbjq.cn/Article/details/ghiwwbkmi.sHtML

JS:   crypto.randomUUID()
来源：http://read.share.fehbvm.com/Article/details/gusgfepwd.sHtML

TS:   crypto.randomUUID()
来源：http://wap.zdbjq.cn/Article/details/gxsuaazep.sHtML

Java: UUID.randomUUID().toString()
来源：http://3g.zdbjq.cn/Article/details/gmbcokjfi.sHtML

Go:   // 用 github.com/google/uuid
来源：http://read.share.fehbvm.com/Article/details/gbblthxfa.sHtML

Ruby: SecureRandom.uuid
来源：http://www.share.zdbjq.cn/Article/details/gybjorgbe.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.m.share.hesvh.cn/Article/details/glyvcefef.sHtML

[P02] MD5 / SHA256 摘要
来源：http://3g.hesvh.cn/Article/details/gkufrylvg.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.blog.zdbjq.cn/Article/details/glmcdvfww.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://wap.fehbvm.com/Article/details/gbtrirvzu.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://read.share.hesvh.cn/Article/details/gwgwsujwo.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://mobile.fehbvm.com/Article/details/gbyzfvkmo.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://m.share.zdbjq.cn/Article/details/gavulyqhu.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://3g.fehbvm.com/Article/details/gjzndjeft.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.share.zdbjq.cn/Article/details/ghpiygsdc.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.share.hesvh.cn/Article/details/gixcadywj.sHtML

[P03] 生成短随机字符串
来源：http://www.share.fehbvm.com/Article/details/gvxnmcjzv.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.share.zdbjq.cn/Article/details/gglokbjaf.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://mobile.zdbjq.cn/Article/details/gwteizuku.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.zdbjq.cn/Article/details/grzsairdp.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.zdbjq.cn/Article/details/gsmzoxtcm.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://3g.fehbvm.com/Article/details/ginymllyx.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.share.fehbvm.com/Article/details/gzhejqcgy.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://baike.zdbjq.cn/Article/details/gaphbrujv.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://read.share.hesvh.cn/Article/details/gpqzgmhzs.sHtML

[P04] 求长度
来源：http://www.blog.hesvh.cn/Article/details/geosflphf.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.share.fehbvm.com/Article/details/gdzyidbsa.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.fehbvm.com/Article/details/gtsjdefcy.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.zdbjq.cn/Article/details/gkdpllzfs.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.fehbvm.com/Article/details/gxwqhcesy.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.blog.zdbjq.cn/Article/details/gwkuopuqh.sHtML

Go:   len(arr);  len(m)
来源：http://baike.hesvh.cn/Article/details/gjegjbrae.sHtML

Ruby: x.length;  x.size
来源：http://blog.fehbvm.com/Article/details/gfdfwspzg.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://3g.zdbjq.cn/Article/details/gpwzxcwpm.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.share.zdbjq.cn/Article/details/ghyoquzut.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://blog.fehbvm.com/Article/details/ghxaddhlz.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://blog.fehbvm.com/Article/details/ghrpqkynq.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://3g.fehbvm.com/Article/details/giwlvficr.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://wap.zdbjq.cn/Article/details/gcihxxweq.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.m.share.fehbvm.com/Article/details/gthjrhjlf.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.share.zdbjq.cn/Article/details/geodxkssc.sHtML

Ruby: a == b
来源：http://read.share.zdbjq.cn/Article/details/gcvbzleth.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://mobile.zdbjq.cn/Article/details/guhzzyzjv.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.share.fehbvm.com/Article/details/gpynhjqjq.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://3g.zdbjq.cn/Article/details/gxykebxax.sHtML

PHP:  if (empty($x)) {}
来源：http://www.blog.fehbvm.com/Article/details/glwnkarau.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://wap.fehbvm.com/Article/details/glehuneuu.sHtML

TS:   if (x == null) {}
来源：http://www.share.hesvh.cn/Article/details/godztdssj.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.blog.zdbjq.cn/Article/details/gnlxlpark.sHtML

Go:   if x == nil {}
来源：http://wap.hesvh.cn/Article/details/gemcokqrn.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://wap.zdbjq.cn/Article/details/gxmnzcejw.sHtML

C#:   if (x is null) {}
来源：http://mobile.zdbjq.cn/Article/details/gdqnzjdbw.sHtML

[P07] 防抖与节流
来源：http://www.share.fehbvm.com/Article/details/gyauqorqp.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://read.share.zdbjq.cn/Article/details/gontfnssj.sHtML

PHP:  // 手写时间戳比较
来源：http://www.blog.fehbvm.com/Article/details/gzskmesgc.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.hesvh.cn/Article/details/grqvfulhb.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.zdbjq.cn/Article/details/gycgmmtkr.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://wap.fehbvm.com/Article/details/guptsunxi.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://3g.fehbvm.com/Article/details/gzgwkzujm.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://baike.zdbjq.cn/Article/details/gncqjjicg.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.blog.hesvh.cn/Article/details/gtmwcpvft.sHtML

[P08] 处理浮点精度问题
来源：http://baike.zdbjq.cn/Article/details/gtognolgk.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://read.share.hesvh.cn/Article/details/gwitiudvk.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://3g.hesvh.cn/Article/details/gqqkszrsa.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://read.share.hesvh.cn/Article/details/gdyycrzno.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://3g.hesvh.cn/Article/details/gbjtntxaz.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://wap.hesvh.cn/Article/details/gmgfmyyoe.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://read.share.hesvh.cn/Article/details/gycfkxoay.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://read.share.fehbvm.com/Article/details/gpbxhhyfw.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.share.fehbvm.com/Article/details/gzxhqmudo.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gjnpzsfke.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.m.share.hesvh.cn/Article/details/gunpvpsrr.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/grovvyiks.sHtML

[Q01] 创建表
来源：http://read.share.fehbvm.com/Article/details/gszjbpepc.sHtML

CREATE TABLE users (
来源：http://read.share.hesvh.cn/Article/details/gfrndqfjb.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.hesvh.cn/Article/details/gdavicxnu.sHtML

name VARCHAR(50) NOT NULL,
来源：http://3g.zdbjq.cn/Article/details/gglgjohcf.sHtML

email VARCHAR(100) UNIQUE,
来源：http://m.share.zdbjq.cn/Article/details/gnxwxatoy.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.share.hesvh.cn/Article/details/galmfkxfj.sHtML

);
来源：http://www.blog.zdbjq.cn/Article/details/geyxdcdan.sHtML

[Q02] 创建带外键的表
来源：http://baike.hesvh.cn/Article/details/ggsvmoyft.sHtML

CREATE TABLE orders (
来源：http://www.share.fehbvm.com/Article/details/gzwumgkct.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.fehbvm.com/Article/details/gtgwhbwxi.sHtML

user_id INT NOT NULL,
来源：http://www.m.share.hesvh.cn/Article/details/gljydyvtl.sHtML

amount DECIMAL(10, 2),
来源：http://www.m.share.zdbjq.cn/Article/details/gtyhpvjtd.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.m.share.fehbvm.com/Article/details/gbsryokou.sHtML

);
来源：http://3g.fehbvm.com/Article/details/gbxtfjabt.sHtML

[Q03] 增加列
来源：http://mobile.hesvh.cn/Article/details/gxcgkctet.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://baike.hesvh.cn/Article/details/gyycoprxr.sHtML

[Q04] 修改列类型
来源：http://3g.hesvh.cn/Article/details/gjblmbgik.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://blog.zdbjq.cn/Article/details/guawtptsn.sHtML

[Q05] 重命名列
来源：http://mobile.zdbjq.cn/Article/details/gzamgjnny.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.share.fehbvm.com/Article/details/gqwzjvmtl.sHtML

[Q06] 删除列
来源：http://www.m.share.fehbvm.com/Article/details/gnvasifhd.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://m.share.hesvh.cn/Article/details/gvswlxdbk.sHtML

[Q07] 删除表
来源：http://www.share.zdbjq.cn/Article/details/gzvbzfhix.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.share.zdbjq.cn/Article/details/geokvbach.sHtML

[Q08] 创建普通索引
来源：http://baike.zdbjq.cn/Article/details/gzzdmzwtn.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://baike.zdbjq.cn/Article/details/glybgaddk.sHtML

[Q09] 创建唯一索引
来源：http://m.share.hesvh.cn/Article/details/gvoibmrsl.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://read.share.zdbjq.cn/Article/details/gpiouzxbk.sHtML

[Q10] 插入单行
来源：http://www.blog.zdbjq.cn/Article/details/gjsvoflmf.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://baike.hesvh.cn/Article/details/geeswzhjl.sHtML

[Q11] 一次插入多行
来源：http://www.blog.hesvh.cn/Article/details/gikzgffiv.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://baike.fehbvm.com/Article/details/geasooszw.sHtML

[Q12] 插入后取自增 ID
来源：http://www.share.hesvh.cn/Article/details/gybjibgjk.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.blog.hesvh.cn/Article/details/glcgkqpxp.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://read.share.fehbvm.com/Article/details/gtiiwbhjp.sHtML

[Q13] 忽略重复插入
来源：http://www.blog.hesvh.cn/Article/details/gmljcorbz.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://mobile.hesvh.cn/Article/details/glxakdxqh.sHtML

[Q14] 存在则更新（upsert）
来源：http://m.share.fehbvm.com/Article/details/gdszvusjk.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://read.share.fehbvm.com/Article/details/gvnoojqzp.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://3g.zdbjq.cn/Article/details/gevorpbti.sHtML

[Q15] 查询全部
来源：http://3g.hesvh.cn/Article/details/gbsuqtlea.sHtML

SELECT * FROM users;
来源：http://wap.hesvh.cn/Article/details/gibfnqtuf.sHtML

[Q16] 查询指定列
来源：http://read.share.hesvh.cn/Article/details/gsfefgwth.sHtML

SELECT id, name FROM users;
来源：http://baike.fehbvm.com/Article/details/gxhsdgraz.sHtML

[Q17] 条件查询
来源：http://blog.zdbjq.cn/Article/details/gmrayejll.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://read.share.zdbjq.cn/Article/details/gpcpmeevr.sHtML

[Q18] 模糊匹配
来源：http://wap.fehbvm.com/Article/details/gdodoquaz.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://m.share.hesvh.cn/Article/details/gpukjnjnd.sHtML

[Q19] 范围查询
来源：http://3g.zdbjq.cn/Article/details/gmypbteao.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.m.share.zdbjq.cn/Article/details/gcyfwayrk.sHtML

[Q20] IN 列表
来源：http://www.share.fehbvm.com/Article/details/gwqdqksmm.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://read.share.hesvh.cn/Article/details/gqmqtegql.sHtML

[Q21] 空值判断
来源：http://baike.fehbvm.com/Article/details/grbaznwfd.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://read.share.fehbvm.com/Article/details/gklwwcrio.sHtML

[Q22] 排序
来源：http://m.share.hesvh.cn/Article/details/gcebeijkp.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://3g.zdbjq.cn/Article/details/greppzdtc.sHtML

[Q23] 分页
来源：http://baike.fehbvm.com/Article/details/goxiikmvt.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.blog.hesvh.cn/Article/details/gtverasmp.sHtML

[Q24] 去重
来源：http://www.blog.zdbjq.cn/Article/details/glkzcdpej.sHtML

SELECT DISTINCT city FROM users;
来源：http://m.share.hesvh.cn/Article/details/gpibxebjy.sHtML

[Q25] 只取前 N 条
来源：http://mobile.zdbjq.cn/Article/details/gleeyljrr.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://blog.hesvh.cn/Article/details/givlofzji.sHtML

[Q26] 计数
来源：http://mobile.zdbjq.cn/Article/details/gwypmzbpd.sHtML

SELECT COUNT(*) FROM users;
来源：http://read.share.hesvh.cn/Article/details/gzapkybfm.sHtML

[Q27] 条件计数
来源：http://www.blog.fehbvm.com/Article/details/gculsrqtn.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://mobile.hesvh.cn/Article/details/gppfheakj.sHtML

[Q28] 求和与平均
来源：http://m.share.fehbvm.com/Article/details/gpxpfaoan.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://3g.hesvh.cn/Article/details/gzfydozgb.sHtML

[Q29] 最大最小值
来源：http://wap.hesvh.cn/Article/details/gctjpkrhr.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://baike.zdbjq.cn/Article/details/gptvcdoxb.sHtML

[Q30] 分组统计
来源：http://www.share.hesvh.cn/Article/details/gyadjkvla.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://mobile.fehbvm.com/Article/details/gevyzmixx.sHtML

[Q31] 分组后过滤
来源：http://m.share.zdbjq.cn/Article/details/gvdktqvpj.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://m.share.zdbjq.cn/Article/details/gldcbgpsr.sHtML

[Q32] 分组拼接字符串
来源：http://3g.hesvh.cn/Article/details/gbllxwxwl.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.blog.hesvh.cn/Article/details/glhcmquhw.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.blog.fehbvm.com/Article/details/gtunqfhhi.sHtML

[Q33] 多列分组
来源：http://m.share.hesvh.cn/Article/details/gudwjwaqb.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://blog.fehbvm.com/Article/details/gmoleoblt.sHtML

[Q34] 每组取第一条
来源：http://www.m.share.hesvh.cn/Article/details/gfvjskxgq.sHtML

SELECT * FROM (
来源：http://read.share.zdbjq.cn/Article/details/gsbmajpif.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.m.share.fehbvm.com/Article/details/ggzmueofz.sHtML

) t WHERE rn = 1;
来源：http://mobile.fehbvm.com/Article/details/gdkpgwvst.sHtML

[Q35] 内连接
来源：http://baike.hesvh.cn/Article/details/gvlhphwxp.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://baike.fehbvm.com/Article/details/gpmbvcuqe.sHtML

[Q36] 左连接
来源：http://3g.hesvh.cn/Article/details/gcfqqalcm.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://wap.zdbjq.cn/Article/details/grgzprisy.sHtML

[Q37] 右连接
来源：http://www.m.share.fehbvm.com/Article/details/gzwqecodx.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.m.share.fehbvm.com/Article/details/ggyfeqkxw.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.blog.hesvh.cn/Article/details/gkoiirynb.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://read.share.zdbjq.cn/Article/details/ganzshmga.sHtML

[Q39] 自连接（查上下级）
来源：http://m.share.fehbvm.com/Article/details/gwhbfuumd.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.m.share.fehbvm.com/Article/details/gfxtscyof.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://3g.hesvh.cn/Article/details/gsjlvuoos.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://baike.zdbjq.cn/Article/details/gghcqiuof.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.blog.zdbjq.cn/Article/details/glvhrvqou.sHtML

[Q41] 多表连接
来源：http://www.blog.hesvh.cn/Article/details/grwbspuse.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://wap.zdbjq.cn/Article/details/gstnrtvaj.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.share.fehbvm.com/Article/details/gzkbusjji.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://3g.hesvh.cn/Article/details/giqctmrhf.sHtML

[Q42] 连接条件附加过滤
来源：http://m.share.hesvh.cn/Article/details/gscpdfbbr.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.share.zdbjq.cn/Article/details/gfjxxkbna.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://read.share.zdbjq.cn/Article/details/gfpqvcfev.sHtML

[Q43] 标量子查询
来源：http://m.share.fehbvm.com/Article/details/gmsvetnnx.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://m.share.zdbjq.cn/Article/details/gvtnpmusc.sHtML

[Q44] IN 子查询
来源：http://baike.fehbvm.com/Article/details/gfpjdzxri.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://wap.hesvh.cn/Article/details/gixienbvi.sHtML

[Q45] EXISTS 判断存在
来源：http://mobile.fehbvm.com/Article/details/gtjynasnk.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.hesvh.cn/Article/details/goaspqhpk.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.share.fehbvm.com/Article/details/guaubbyru.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.zdbjq.cn/Article/details/gilqkwxga.sHtML

[Q47] 与平均值比较
来源：http://baike.hesvh.cn/Article/details/ghgofrzcm.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.blog.fehbvm.com/Article/details/giccggcft.sHtML

[Q48] CTE 公用表表达式
来源：http://baike.fehbvm.com/Article/details/geqpcavxw.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://wap.fehbvm.com/Article/details/gqpsfczqj.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.share.hesvh.cn/Article/details/gysnuzppm.sHtML

[Q49] 更新单行
来源：http://baike.zdbjq.cn/Article/details/gyknporls.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://mobile.fehbvm.com/Article/details/gcgndfmxw.sHtML

[Q50] 批量更新
来源：http://blog.hesvh.cn/Article/details/gwgftojus.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://wap.zdbjq.cn/Article/details/gjpkfobek.sHtML

[Q51] 用子查询更新
来源：http://www.m.share.fehbvm.com/Article/details/gtewerfeg.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.m.share.hesvh.cn/Article/details/gvarjzoog.sHtML

[Q52] 删除指定行
来源：http://wap.hesvh.cn/Article/details/grvevwwav.sHtML

DELETE FROM users WHERE id = 10;
来源：http://3g.fehbvm.com/Article/details/gmlkrhhan.sHtML

[Q53] 按条件删除
来源：http://www.share.zdbjq.cn/Article/details/gpagbbukt.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://blog.fehbvm.com/Article/details/gqnkqjupv.sHtML

[Q54] 清空表
来源：http://wap.zdbjq.cn/Article/details/glsthaaix.sHtML

TRUNCATE TABLE logs;
来源：http://m.share.fehbvm.com/Article/details/gengzaspx.sHtML

[Q55] 排名（并列占位）
来源：http://m.share.fehbvm.com/Article/details/guxjqqxhl.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://blog.zdbjq.cn/Article/details/ghhugbrvq.sHtML

[Q56] 密集排名（并列不占位）
来源：http://3g.fehbvm.com/Article/details/gkomrsysx.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://wap.fehbvm.com/Article/details/ggnjgnhiw.sHtML

[Q57] 行号
来源：http://m.share.zdbjq.cn/Article/details/gzgabqolh.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://baike.fehbvm.com/Article/details/gnuqygnsf.sHtML

[Q58] 累计求和
来源：http://www.blog.hesvh.cn/Article/details/ghcqvqyqy.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://read.share.hesvh.cn/Article/details/gtfwvwdqb.sHtML

[Q59] 分组内累计
来源：http://blog.hesvh.cn/Article/details/gwaxmpvgd.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://3g.hesvh.cn/Article/details/gvegcpbob.sHtML

[Q60] 取上一行 / 下一行
来源：http://baike.hesvh.cn/Article/details/ggqznmxzk.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://3g.hesvh.cn/Article/details/gfliwrnjg.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://wap.fehbvm.com/Article/details/gycbenjtf.sHtML

[Q61] 移动平均
来源：http://m.share.fehbvm.com/Article/details/gifyuwtlx.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.m.share.hesvh.cn/Article/details/ghjuisjjq.sHtML

[Q62] 分组占比
来源：http://mobile.hesvh.cn/Article/details/gftvtczoc.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://mobile.hesvh.cn/Article/details/gqmiwvnwh.sHtML

[Q63] 开启事务
来源：http://wap.hesvh.cn/Article/details/gmawxwria.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://mobile.zdbjq.cn/Article/details/gtkqkozsl.sHtML

[Q64] 提交事务
来源：http://www.share.fehbvm.com/Article/details/gdcxdzhmw.sHtML

COMMIT;
来源：http://wap.hesvh.cn/Article/details/grfgtfrdp.sHtML

[Q65] 回滚事务
来源：http://3g.fehbvm.com/Article/details/gxdvpaouv.sHtML

ROLLBACK;
来源：http://www.blog.zdbjq.cn/Article/details/gczuywhnf.sHtML

[Q66] 行锁查询
来源：http://www.blog.fehbvm.com/Article/details/gqhgljugz.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://m.share.fehbvm.com/Article/details/gvvssjzpp.sHtML

[Q67] 设置隔离级别
来源：http://www.m.share.fehbvm.com/Article/details/gqiotkqvw.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://mobile.fehbvm.com/Article/details/gkrrurhcn.sHtML

[Q68] 保存点
来源：http://wap.hesvh.cn/Article/details/gymfmgecm.sHtML

SAVEPOINT sp1;
来源：http://blog.fehbvm.com/Article/details/gaqnmnhpx.sHtML

ROLLBACK TO sp1;
来源：http://3g.hesvh.cn/Article/details/gxffmgruu.sHtML

[Q69] 查看执行计划
来源：http://wap.hesvh.cn/Article/details/gqucamzue.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://3g.zdbjq.cn/Article/details/gvlxesubl.sHtML

[Q70] 更新统计信息
来源：http://www.share.zdbjq.cn/Article/details/gfodbpnaq.sHtML

ANALYZE TABLE users;
来源：http://www.share.hesvh.cn/Article/details/gzekhcbju.sHtML

[Q71] 查看建表语句
来源：http://www.share.zdbjq.cn/Article/details/grdysxawg.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://read.share.hesvh.cn/Article/details/gupjxequg.sHtML

[Q72] 查看索引
来源：http://www.m.share.fehbvm.com/Article/details/glbvpbyvz.sHtML

SHOW INDEX FROM users;
来源：http://blog.zdbjq.cn/Article/details/gbbqunedz.sHtML

[Q73] 查看表状态
来源：http://3g.fehbvm.com/Article/details/gksjevkuy.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://read.share.fehbvm.com/Article/details/giamisshq.sHtML

[Q74] 强制使用索引
来源：http://baike.hesvh.cn/Article/details/gkjvxidhn.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://wap.hesvh.cn/Article/details/gcrnbahbk.sHtML

[Q75] 日期格式化
来源：http://mobile.fehbvm.com/Article/details/gskqaynmc.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://mobile.hesvh.cn/Article/details/gdzthjboa.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.blog.fehbvm.com/Article/details/gnegfttic.sHtML

[Q76] 按天统计
来源：http://3g.zdbjq.cn/Article/details/gxlmbskvm.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.blog.zdbjq.cn/Article/details/gajkhhwgi.sHtML

[Q77] 时间加减
来源：http://www.share.fehbvm.com/Article/details/gclttariv.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.m.share.zdbjq.cn/Article/details/gfwtracnz.sHtML

[Q78] 当前时间
来源：http://mobile.hesvh.cn/Article/details/gufenhxpf.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://read.share.hesvh.cn/Article/details/gowzdlpam.sHtML

[Q79] 字符串拼接
来源：http://www.blog.zdbjq.cn/Article/details/gznwcpfjm.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://wap.zdbjq.cn/Article/details/gdyjjstew.sHtML

[Q80] 字符串截取
来源：http://wap.zdbjq.cn/Article/details/guxxdnplg.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://m.share.fehbvm.com/Article/details/gqkleubza.sHtML

[Q81] 字符串替换
来源：http://wap.hesvh.cn/Article/details/glohnskev.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.share.zdbjq.cn/Article/details/guhzbvqun.sHtML

[Q82] 字符长度与字节长度
来源：http://www.share.hesvh.cn/Article/details/gvcwdomud.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gtatrwpbu.sHtML

[Q83] 大小写转换
来源：http://baike.hesvh.cn/Article/details/gpkdsenha.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://wap.zdbjq.cn/Article/details/gehicfllo.sHtML

[Q84] 去除首尾空格
来源：http://blog.hesvh.cn/Article/details/grgjennvk.sHtML

SELECT TRIM(name) FROM users;
来源：http://blog.hesvh.cn/Article/details/gftqbbzrn.sHtML

[Q85] 数值取整
来源：http://3g.zdbjq.cn/Article/details/gksagogrk.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://mobile.hesvh.cn/Article/details/gmbdcsbed.sHtML

[Q86] 读取 JSON 字段
来源：http://read.share.hesvh.cn/Article/details/gggqbkfho.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://m.share.hesvh.cn/Article/details/gbiujnwzg.sHtML

[Q87] JSON 字段做条件
来源：http://www.share.hesvh.cn/Article/details/gmamexkmf.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://3g.fehbvm.com/Article/details/gjqgiizzw.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.blog.fehbvm.com/Article/details/gcevfzsed.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://m.share.hesvh.cn/Article/details/godedqpjk.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://baike.zdbjq.cn/Article/details/gzkdinskw.sHtML

[Q89] 判断表是否存在
来源：http://baike.hesvh.cn/Article/details/gpatsbgif.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.share.fehbvm.com/Article/details/gvlvuvpss.sHtML

[Q90] 生成序号列
来源：http://baike.fehbvm.com/Article/details/gyihczuok.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.blog.fehbvm.com/Article/details/gnombfubi.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gmzsvlkxo.sHtML

R. Bash 专题
来源：http://www.m.share.fehbvm.com/Article/details/gfyddauvt.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/grijpxmtz.sHtML

[R01] shebang 与严格模式
来源：http://blog.fehbvm.com/Article/details/gsmwzyxep.sHtML

#!/usr/bin/env bash
来源：http://wap.hesvh.cn/Article/details/gomvkgers.sHtML

set -euo pipefail
来源：http://mobile.hesvh.cn/Article/details/gcnvghoie.sHtML

[R02] 变量赋值与使用
来源：http://read.share.hesvh.cn/Article/details/gzfasfzxt.sHtML

name="Tom"; echo "$name"
来源：http://www.blog.hesvh.cn/Article/details/ghgqqvlli.sHtML

[R03] 只读变量
来源：http://www.blog.zdbjq.cn/Article/details/gvxiiqnlr.sHtML

readonly PI=3.14
来源：http://www.share.fehbvm.com/Article/details/gpksqtnfo.sHtML

[R04] 位置参数
来源：http://blog.zdbjq.cn/Article/details/gpqzcfyyv.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://mobile.fehbvm.com/Article/details/gwdqznutr.sHtML

[R05] 参数默认值
来源：http://blog.zdbjq.cn/Article/details/gtqpnpbka.sHtML

name="${1:-default}"
来源：http://www.share.hesvh.cn/Article/details/ghqrwyzkm.sHtML

[R06] 判断命令是否存在
来源：http://www.share.fehbvm.com/Article/details/gzrxvkvgg.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.blog.fehbvm.com/Article/details/gothxqjuj.sHtML

[R07] if 判断文件
来源：http://read.share.zdbjq.cn/Article/details/ggvzijces.sHtML


<!-- 参考信息 -->