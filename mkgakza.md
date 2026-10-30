代发 wailian999

TS:   // child_process / cluster 模块
来源：http://www.m.share.hesvh.cn/Article/details/gvayfpptj.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://mobile.fehbvm.com/Article/details/gmltixbcc.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.share.hesvh.cn/Article/details/gbaoivfxi.sHtML

Ruby: // fork 块
来源：http://mobile.hesvh.cn/Article/details/gtgileqra.sHtML

C#:   Parallel.For
来源：http://www.blog.fehbvm.com/Article/details/gvtzyqotg.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gcpxpodpa.sHtML

P. 常用工具函数
来源：http://www.blog.zdbjq.cn/Article/details/gocdpvaff.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/grgyussat.sHtML

[P01] 生成 UUID
来源：http://m.share.hesvh.cn/Article/details/gvlaeaufi.sHtML

Py:   str(uuid.uuid4())
来源：http://www.blog.hesvh.cn/Article/details/gcnlcqexq.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.m.share.fehbvm.com/Article/details/gcrafolnp.sHtML

JS:   crypto.randomUUID()
来源：http://mobile.fehbvm.com/Article/details/gjnmquxlo.sHtML

TS:   crypto.randomUUID()
来源：http://www.blog.zdbjq.cn/Article/details/guskiiydb.sHtML

Java: UUID.randomUUID().toString()
来源：http://baike.hesvh.cn/Article/details/glyebmfeu.sHtML

Go:   // 用 github.com/google/uuid
来源：http://baike.hesvh.cn/Article/details/gsyowhsgw.sHtML

Ruby: SecureRandom.uuid
来源：http://mobile.hesvh.cn/Article/details/gsqczyjzy.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.m.share.hesvh.cn/Article/details/gknwfoxbv.sHtML

[P02] MD5 / SHA256 摘要
来源：http://read.share.zdbjq.cn/Article/details/gqynvbvct.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://wap.hesvh.cn/Article/details/giujhzalu.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://baike.fehbvm.com/Article/details/gjmhnhxuc.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://wap.fehbvm.com/Article/details/ggrmiitrb.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://read.share.hesvh.cn/Article/details/gcbvaggts.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://read.share.hesvh.cn/Article/details/gikevgxmm.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://baike.zdbjq.cn/Article/details/gpzhrzskz.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.share.zdbjq.cn/Article/details/gosecajju.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://baike.zdbjq.cn/Article/details/glzmfndyj.sHtML

[P03] 生成短随机字符串
来源：http://www.share.fehbvm.com/Article/details/gmmbskgjj.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://baike.fehbvm.com/Article/details/gzymmipjn.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://3g.zdbjq.cn/Article/details/gozqqzpuc.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.zdbjq.cn/Article/details/gcvumicip.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.zdbjq.cn/Article/details/gycbvjbpi.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.share.zdbjq.cn/Article/details/gqwzlwevp.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.blog.fehbvm.com/Article/details/gbzmcmgvm.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://baike.zdbjq.cn/Article/details/gemlmamaw.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://m.share.zdbjq.cn/Article/details/gitdilzxf.sHtML

[P04] 求长度
来源：http://www.blog.hesvh.cn/Article/details/govgvibqs.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://m.share.hesvh.cn/Article/details/gkjpfpoia.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.hesvh.cn/Article/details/gizuiapus.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.hesvh.cn/Article/details/gpogsylyk.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.zdbjq.cn/Article/details/gipfjappe.sHtML

Java: list.size();  map.size();  s.length()
来源：http://read.share.fehbvm.com/Article/details/grusxlmlq.sHtML

Go:   len(arr);  len(m)
来源：http://www.share.zdbjq.cn/Article/details/gmwtsizlg.sHtML

Ruby: x.length;  x.size
来源：http://www.share.fehbvm.com/Article/details/gvianoqqm.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://read.share.fehbvm.com/Article/details/gcelyxvzq.sHtML

[P05] 判断两个对象内容是否相等
来源：http://m.share.fehbvm.com/Article/details/ghjluedun.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.share.hesvh.cn/Article/details/galfzltsi.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.m.share.hesvh.cn/Article/details/ghtenhkgb.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.m.share.hesvh.cn/Article/details/gshzvfkpm.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.zdbjq.cn/Article/details/gmvnhwiwh.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://mobile.hesvh.cn/Article/details/gqnebbbqe.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://3g.hesvh.cn/Article/details/gsjqpozxv.sHtML

Ruby: a == b
来源：http://read.share.zdbjq.cn/Article/details/gtneoqjwg.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://m.share.hesvh.cn/Article/details/grqfssilf.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://mobile.hesvh.cn/Article/details/gyeytwatu.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.blog.hesvh.cn/Article/details/gjanzhaox.sHtML

PHP:  if (empty($x)) {}
来源：http://blog.hesvh.cn/Article/details/gdmxfhgnw.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.share.fehbvm.com/Article/details/gnfoyrkoe.sHtML

TS:   if (x == null) {}
来源：http://mobile.hesvh.cn/Article/details/gsbkurxqg.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://blog.fehbvm.com/Article/details/gbcpmpkgd.sHtML

Go:   if x == nil {}
来源：http://wap.zdbjq.cn/Article/details/gacptmdbz.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://blog.fehbvm.com/Article/details/ghcdcozkf.sHtML

C#:   if (x is null) {}
来源：http://read.share.zdbjq.cn/Article/details/gwhsvissu.sHtML

[P07] 防抖与节流
来源：http://www.blog.hesvh.cn/Article/details/gbdhdoaee.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://baike.fehbvm.com/Article/details/geebezelm.sHtML

PHP:  // 手写时间戳比较
来源：http://blog.zdbjq.cn/Article/details/gdyfqwgfd.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.zdbjq.cn/Article/details/grlkwzdjq.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.fehbvm.com/Article/details/grpkxdhkm.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://mobile.fehbvm.com/Article/details/gszzdfumf.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.blog.fehbvm.com/Article/details/gsgvwjbkv.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.m.share.fehbvm.com/Article/details/gwnuickzs.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://m.share.zdbjq.cn/Article/details/gpkhsrhdx.sHtML

[P08] 处理浮点精度问题
来源：http://mobile.zdbjq.cn/Article/details/gwdkclkma.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://3g.fehbvm.com/Article/details/gvqawtgom.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://3g.fehbvm.com/Article/details/gxwdetxzl.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://blog.fehbvm.com/Article/details/gasnmgtjv.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://blog.hesvh.cn/Article/details/grkggwyzu.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://m.share.zdbjq.cn/Article/details/grxbfmygp.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.m.share.hesvh.cn/Article/details/gcpcacobq.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://mobile.fehbvm.com/Article/details/gofmaotot.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://3g.hesvh.cn/Article/details/gcptujnkb.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gnuytswrz.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://wap.fehbvm.com/Article/details/garttiylm.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gemhxxnoa.sHtML

[Q01] 创建表
来源：http://3g.zdbjq.cn/Article/details/gunkztwir.sHtML

CREATE TABLE users (
来源：http://blog.zdbjq.cn/Article/details/gcdnrptil.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.fehbvm.com/Article/details/gldbgaxux.sHtML

name VARCHAR(50) NOT NULL,
来源：http://3g.fehbvm.com/Article/details/ggzwbqvnw.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.share.zdbjq.cn/Article/details/ghzoqilyo.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.m.share.zdbjq.cn/Article/details/golkqosgd.sHtML

);
来源：http://www.share.zdbjq.cn/Article/details/ghpeesiws.sHtML

[Q02] 创建带外键的表
来源：http://m.share.hesvh.cn/Article/details/guascdlvp.sHtML

CREATE TABLE orders (
来源：http://mobile.fehbvm.com/Article/details/gqipfubtx.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.zdbjq.cn/Article/details/glzgtpvis.sHtML

user_id INT NOT NULL,
来源：http://wap.zdbjq.cn/Article/details/gcsvmuvyq.sHtML

amount DECIMAL(10, 2),
来源：http://www.share.zdbjq.cn/Article/details/gcmibdlna.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://mobile.fehbvm.com/Article/details/gzzdphhig.sHtML

);
来源：http://blog.fehbvm.com/Article/details/ghjqgkvew.sHtML

[Q03] 增加列
来源：http://www.m.share.fehbvm.com/Article/details/gpuixoxim.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://mobile.fehbvm.com/Article/details/gjgapqina.sHtML

[Q04] 修改列类型
来源：http://www.share.zdbjq.cn/Article/details/gugsxfkyq.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://blog.zdbjq.cn/Article/details/gkkxhcgvm.sHtML

[Q05] 重命名列
来源：http://www.blog.zdbjq.cn/Article/details/gzygscmrb.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://3g.fehbvm.com/Article/details/grcsdmxgi.sHtML

[Q06] 删除列
来源：http://mobile.hesvh.cn/Article/details/gdtxvbfzf.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://mobile.hesvh.cn/Article/details/gjonpdtje.sHtML

[Q07] 删除表
来源：http://www.share.hesvh.cn/Article/details/gvadfaiai.sHtML

DROP TABLE IF EXISTS orders;
来源：http://blog.hesvh.cn/Article/details/gabnrdvqm.sHtML

[Q08] 创建普通索引
来源：http://wap.fehbvm.com/Article/details/gyoiupozf.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.m.share.fehbvm.com/Article/details/gyopfnieq.sHtML

[Q09] 创建唯一索引
来源：http://blog.fehbvm.com/Article/details/glgfkjrqs.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://blog.hesvh.cn/Article/details/gjxvzrtay.sHtML

[Q10] 插入单行
来源：http://www.blog.zdbjq.cn/Article/details/gllebmkfc.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://m.share.zdbjq.cn/Article/details/gcriubzts.sHtML

[Q11] 一次插入多行
来源：http://blog.fehbvm.com/Article/details/gbxydseuj.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.m.share.zdbjq.cn/Article/details/gkgqarhdf.sHtML

[Q12] 插入后取自增 ID
来源：http://3g.fehbvm.com/Article/details/gyhyhoxry.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.share.hesvh.cn/Article/details/gfyejncmn.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://wap.zdbjq.cn/Article/details/gqfplhfsm.sHtML

[Q13] 忽略重复插入
来源：http://www.share.hesvh.cn/Article/details/glsrajxkc.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://3g.fehbvm.com/Article/details/griwqbdpz.sHtML

[Q14] 存在则更新（upsert）
来源：http://m.share.zdbjq.cn/Article/details/ggniiijrx.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://3g.fehbvm.com/Article/details/gxtaaorrv.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://mobile.hesvh.cn/Article/details/gybiizbwm.sHtML

[Q15] 查询全部
来源：http://www.m.share.zdbjq.cn/Article/details/gwbidscfe.sHtML

SELECT * FROM users;
来源：http://baike.hesvh.cn/Article/details/giqmgvvxk.sHtML

[Q16] 查询指定列
来源：http://baike.fehbvm.com/Article/details/gpbcltdyh.sHtML

SELECT id, name FROM users;
来源：http://blog.zdbjq.cn/Article/details/gillnyism.sHtML

[Q17] 条件查询
来源：http://www.blog.zdbjq.cn/Article/details/gkcnjvtvy.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://blog.hesvh.cn/Article/details/gqkjasiaz.sHtML

[Q18] 模糊匹配
来源：http://www.share.zdbjq.cn/Article/details/gtjyhfmsy.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://3g.zdbjq.cn/Article/details/gilcbnbwp.sHtML

[Q19] 范围查询
来源：http://baike.fehbvm.com/Article/details/grrkltfyr.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://3g.fehbvm.com/Article/details/gtyhmbkwv.sHtML

[Q20] IN 列表
来源：http://wap.hesvh.cn/Article/details/ghgjzhkqk.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://blog.fehbvm.com/Article/details/gitrzjyjd.sHtML

[Q21] 空值判断
来源：http://www.m.share.zdbjq.cn/Article/details/ghhuijsma.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://blog.hesvh.cn/Article/details/ghhttpqvf.sHtML

[Q22] 排序
来源：http://m.share.fehbvm.com/Article/details/grljpmaii.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://3g.hesvh.cn/Article/details/gmszixpxo.sHtML

[Q23] 分页
来源：http://www.blog.zdbjq.cn/Article/details/gtocghuck.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://3g.zdbjq.cn/Article/details/gcdoeewxl.sHtML

[Q24] 去重
来源：http://m.share.fehbvm.com/Article/details/glqbievut.sHtML

SELECT DISTINCT city FROM users;
来源：http://m.share.fehbvm.com/Article/details/gtmrjzegh.sHtML

[Q25] 只取前 N 条
来源：http://www.m.share.hesvh.cn/Article/details/gddgdfeug.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.m.share.zdbjq.cn/Article/details/gvpfcmuwj.sHtML

[Q26] 计数
来源：http://read.share.fehbvm.com/Article/details/gqmalclrj.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.share.fehbvm.com/Article/details/gydfmqsrj.sHtML

[Q27] 条件计数
来源：http://wap.zdbjq.cn/Article/details/gljrlzcuj.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://wap.zdbjq.cn/Article/details/gefcrlksk.sHtML

[Q28] 求和与平均
来源：http://www.blog.hesvh.cn/Article/details/gegjccvno.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://3g.fehbvm.com/Article/details/gtyzobljz.sHtML

[Q29] 最大最小值
来源：http://www.blog.fehbvm.com/Article/details/gsxurziyk.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://blog.zdbjq.cn/Article/details/gaoqdjtph.sHtML

[Q30] 分组统计
来源：http://www.m.share.zdbjq.cn/Article/details/gxkjdrsaj.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.blog.hesvh.cn/Article/details/gdqmzvooz.sHtML

[Q31] 分组后过滤
来源：http://www.m.share.hesvh.cn/Article/details/gjimibakz.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.blog.hesvh.cn/Article/details/gjnmsnslh.sHtML

[Q32] 分组拼接字符串
来源：http://m.share.fehbvm.com/Article/details/gxtnfvwoc.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://mobile.fehbvm.com/Article/details/geahvqjjk.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.blog.fehbvm.com/Article/details/ggirylmzc.sHtML

[Q33] 多列分组
来源：http://baike.hesvh.cn/Article/details/gltwuzphw.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.blog.fehbvm.com/Article/details/gawgzfrnt.sHtML

[Q34] 每组取第一条
来源：http://read.share.hesvh.cn/Article/details/gofeuqruc.sHtML

SELECT * FROM (
来源：http://www.share.fehbvm.com/Article/details/gkqvegpah.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://mobile.hesvh.cn/Article/details/gaubmrtqk.sHtML

) t WHERE rn = 1;
来源：http://mobile.zdbjq.cn/Article/details/gckonyjzi.sHtML

[Q35] 内连接
来源：http://baike.zdbjq.cn/Article/details/gafjkwokq.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://wap.zdbjq.cn/Article/details/gjrzvmcbq.sHtML

[Q36] 左连接
来源：http://baike.zdbjq.cn/Article/details/ggvvrlqvp.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.hesvh.cn/Article/details/gtiacuear.sHtML

[Q37] 右连接
来源：http://www.share.fehbvm.com/Article/details/gkftkrqyn.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://baike.hesvh.cn/Article/details/gkkctztwd.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.blog.hesvh.cn/Article/details/gkextagqy.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://baike.zdbjq.cn/Article/details/gahdxxkzi.sHtML

[Q39] 自连接（查上下级）
来源：http://3g.hesvh.cn/Article/details/gvdwgsipq.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.share.fehbvm.com/Article/details/gqopbszth.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.blog.hesvh.cn/Article/details/gaswignxp.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.share.zdbjq.cn/Article/details/glinmvctn.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.share.hesvh.cn/Article/details/gsytdruxp.sHtML

[Q41] 多表连接
来源：http://blog.hesvh.cn/Article/details/gypjqhgkq.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.m.share.zdbjq.cn/Article/details/gwzwmkkec.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.m.share.fehbvm.com/Article/details/gffbznjkv.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.m.share.zdbjq.cn/Article/details/gvayoapml.sHtML

[Q42] 连接条件附加过滤
来源：http://mobile.zdbjq.cn/Article/details/gbmphljwi.sHtML

SELECT u.name, o.amount FROM users u
来源：http://3g.fehbvm.com/Article/details/gisqapcpe.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://mobile.zdbjq.cn/Article/details/gosaxamdo.sHtML

[Q43] 标量子查询
来源：http://www.m.share.zdbjq.cn/Article/details/giajflhmo.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.m.share.fehbvm.com/Article/details/gndqprmjq.sHtML

[Q44] IN 子查询
来源：http://blog.fehbvm.com/Article/details/gormerqpp.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.blog.zdbjq.cn/Article/details/gvxlzdudy.sHtML

[Q45] EXISTS 判断存在
来源：http://www.share.hesvh.cn/Article/details/gzxiqyuul.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.hesvh.cn/Article/details/gnyavzwtw.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://baike.hesvh.cn/Article/details/gdtzupbnq.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.zdbjq.cn/Article/details/glhpsxefu.sHtML

[Q47] 与平均值比较
来源：http://read.share.zdbjq.cn/Article/details/guxtbpcqd.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://read.share.fehbvm.com/Article/details/gqnnlylbx.sHtML

[Q48] CTE 公用表表达式
来源：http://mobile.fehbvm.com/Article/details/gegdwhbrc.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://read.share.zdbjq.cn/Article/details/gciftxgvd.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://mobile.hesvh.cn/Article/details/gutrnzteu.sHtML

[Q49] 更新单行
来源：http://mobile.fehbvm.com/Article/details/gokfityno.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://blog.hesvh.cn/Article/details/galmyoago.sHtML

[Q50] 批量更新
来源：http://read.share.hesvh.cn/Article/details/gpzmjpmwk.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.blog.fehbvm.com/Article/details/gmdctlkrc.sHtML

[Q51] 用子查询更新
来源：http://3g.hesvh.cn/Article/details/geoagobxi.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://blog.hesvh.cn/Article/details/ganuyzbcq.sHtML

[Q52] 删除指定行
来源：http://baike.zdbjq.cn/Article/details/guzxfhjsd.sHtML

DELETE FROM users WHERE id = 10;
来源：http://m.share.zdbjq.cn/Article/details/gpyjxgljo.sHtML

[Q53] 按条件删除
来源：http://read.share.zdbjq.cn/Article/details/gyqsuzhdw.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://wap.fehbvm.com/Article/details/glwgajhjt.sHtML

[Q54] 清空表
来源：http://m.share.zdbjq.cn/Article/details/gjxxaxhlq.sHtML

TRUNCATE TABLE logs;
来源：http://baike.hesvh.cn/Article/details/gxogqssim.sHtML

[Q55] 排名（并列占位）
来源：http://www.blog.hesvh.cn/Article/details/gzggrjyri.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://3g.hesvh.cn/Article/details/grbtvkbow.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.m.share.fehbvm.com/Article/details/gbicswvnp.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.blog.zdbjq.cn/Article/details/geiaeuoee.sHtML

[Q57] 行号
来源：http://3g.fehbvm.com/Article/details/gnllerusb.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gkqlrddma.sHtML

[Q58] 累计求和
来源：http://mobile.fehbvm.com/Article/details/groeuqphn.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://baike.hesvh.cn/Article/details/gzggrvaon.sHtML

[Q59] 分组内累计
来源：http://www.share.fehbvm.com/Article/details/gijutjicp.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.m.share.fehbvm.com/Article/details/gedmhlkxp.sHtML

[Q60] 取上一行 / 下一行
来源：http://mobile.hesvh.cn/Article/details/gpepcaqnt.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://baike.fehbvm.com/Article/details/gffqkfcob.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://read.share.fehbvm.com/Article/details/ganpenien.sHtML

[Q61] 移动平均
来源：http://www.share.hesvh.cn/Article/details/gjgdvhyvk.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://m.share.zdbjq.cn/Article/details/gmriamzyj.sHtML

[Q62] 分组占比
来源：http://3g.zdbjq.cn/Article/details/gpjchfghs.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.m.share.hesvh.cn/Article/details/gocpvzelw.sHtML

[Q63] 开启事务
来源：http://www.blog.fehbvm.com/Article/details/gcacdavir.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.share.fehbvm.com/Article/details/gprithqwe.sHtML

[Q64] 提交事务
来源：http://www.blog.fehbvm.com/Article/details/gpcxirjcp.sHtML

COMMIT;
来源：http://www.share.zdbjq.cn/Article/details/gbdtwgmni.sHtML

[Q65] 回滚事务
来源：http://www.blog.hesvh.cn/Article/details/gmnyrdkft.sHtML

ROLLBACK;
来源：http://baike.hesvh.cn/Article/details/gpctnzbay.sHtML

[Q66] 行锁查询
来源：http://wap.zdbjq.cn/Article/details/gmakguwkt.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.share.zdbjq.cn/Article/details/gbkqjohkm.sHtML

[Q67] 设置隔离级别
来源：http://m.share.hesvh.cn/Article/details/gosotjjcy.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://read.share.fehbvm.com/Article/details/gctdwerib.sHtML

[Q68] 保存点
来源：http://www.blog.hesvh.cn/Article/details/gugchkqei.sHtML

SAVEPOINT sp1;
来源：http://blog.fehbvm.com/Article/details/gspnlpqrj.sHtML

ROLLBACK TO sp1;
来源：http://www.blog.fehbvm.com/Article/details/gwjtmkyod.sHtML

[Q69] 查看执行计划
来源：http://baike.fehbvm.com/Article/details/gqygsjfsi.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://wap.fehbvm.com/Article/details/gxqupcduz.sHtML

[Q70] 更新统计信息
来源：http://www.share.fehbvm.com/Article/details/gzpziroal.sHtML

ANALYZE TABLE users;
来源：http://www.blog.zdbjq.cn/Article/details/gxyjgqnfh.sHtML

[Q71] 查看建表语句
来源：http://3g.zdbjq.cn/Article/details/gggglyxao.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://3g.zdbjq.cn/Article/details/gcnzwiast.sHtML

[Q72] 查看索引
来源：http://www.m.share.hesvh.cn/Article/details/gxmxdrazd.sHtML

SHOW INDEX FROM users;
来源：http://m.share.zdbjq.cn/Article/details/ghrheyvqj.sHtML

[Q73] 查看表状态
来源：http://www.share.zdbjq.cn/Article/details/gxucxzvex.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://wap.zdbjq.cn/Article/details/gtdpzfmnf.sHtML

[Q74] 强制使用索引
来源：http://baike.zdbjq.cn/Article/details/gfwjejdyy.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.share.hesvh.cn/Article/details/gcpifftuc.sHtML

[Q75] 日期格式化
来源：http://www.blog.hesvh.cn/Article/details/gllmlkfsd.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://blog.fehbvm.com/Article/details/gcxiyimlg.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://3g.fehbvm.com/Article/details/gskprvssg.sHtML

[Q76] 按天统计
来源：http://baike.zdbjq.cn/Article/details/gnljsuecy.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://m.share.fehbvm.com/Article/details/gjiobakkg.sHtML

[Q77] 时间加减
来源：http://read.share.fehbvm.com/Article/details/gjlooogmz.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.blog.zdbjq.cn/Article/details/gxkpmaryv.sHtML

[Q78] 当前时间
来源：http://baike.zdbjq.cn/Article/details/gkiaxlgdd.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://read.share.zdbjq.cn/Article/details/gfubiynom.sHtML

[Q79] 字符串拼接
来源：http://blog.zdbjq.cn/Article/details/gxghuzhvj.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://baike.fehbvm.com/Article/details/gwypookiv.sHtML

[Q80] 字符串截取
来源：http://blog.fehbvm.com/Article/details/gveysxotd.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gwhidabbw.sHtML

[Q81] 字符串替换
来源：http://m.share.zdbjq.cn/Article/details/gvybmbjjn.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://m.share.fehbvm.com/Article/details/gjgfskaet.sHtML

[Q82] 字符长度与字节长度
来源：http://blog.zdbjq.cn/Article/details/glellsffr.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://mobile.fehbvm.com/Article/details/gaumbhxzq.sHtML

[Q83] 大小写转换
来源：http://www.share.hesvh.cn/Article/details/gtpnirxwa.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://read.share.fehbvm.com/Article/details/gneoetoun.sHtML

[Q84] 去除首尾空格
来源：http://3g.fehbvm.com/Article/details/ghiktggkh.sHtML

SELECT TRIM(name) FROM users;
来源：http://wap.zdbjq.cn/Article/details/gkqfsalhl.sHtML

[Q85] 数值取整
来源：http://blog.hesvh.cn/Article/details/gjuamzhjz.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://blog.zdbjq.cn/Article/details/gpficugwc.sHtML

[Q86] 读取 JSON 字段
来源：http://baike.fehbvm.com/Article/details/gwdbxnwnd.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://read.share.fehbvm.com/Article/details/gfrpnydkf.sHtML

[Q87] JSON 字段做条件
来源：http://m.share.hesvh.cn/Article/details/gmxbwbeyo.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.blog.hesvh.cn/Article/details/gqenuaawc.sHtML

[Q88] 行转列（条件聚合）
来源：http://read.share.hesvh.cn/Article/details/gotbqukem.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://read.share.zdbjq.cn/Article/details/gidgxoopp.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://blog.hesvh.cn/Article/details/gzgkwixyw.sHtML

[Q89] 判断表是否存在
来源：http://www.share.zdbjq.cn/Article/details/gykhsawij.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.blog.hesvh.cn/Article/details/gmslsjkcv.sHtML

[Q90] 生成序号列
来源：http://blog.zdbjq.cn/Article/details/gbfvbixwf.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.blog.fehbvm.com/Article/details/gtcfoxgjp.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gjmzybatg.sHtML

R. Bash 专题
来源：http://www.share.zdbjq.cn/Article/details/gjrxeecmp.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gpnzltbzk.sHtML

[R01] shebang 与严格模式
来源：http://baike.fehbvm.com/Article/details/gisgznfxh.sHtML

#!/usr/bin/env bash
来源：http://www.share.fehbvm.com/Article/details/gnpixogde.sHtML

set -euo pipefail
来源：http://3g.fehbvm.com/Article/details/gglrfiexn.sHtML

[R02] 变量赋值与使用
来源：http://read.share.zdbjq.cn/Article/details/gfswhnwut.sHtML

name="Tom"; echo "$name"
来源：http://baike.fehbvm.com/Article/details/gzdsfjefp.sHtML

[R03] 只读变量
来源：http://m.share.hesvh.cn/Article/details/grvozjpda.sHtML

readonly PI=3.14
来源：http://baike.zdbjq.cn/Article/details/gffpiifxj.sHtML

[R04] 位置参数
来源：http://mobile.hesvh.cn/Article/details/gywtjbwcx.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://mobile.hesvh.cn/Article/details/gcrocyiqm.sHtML

[R05] 参数默认值
来源：http://blog.zdbjq.cn/Article/details/gaoahlovu.sHtML


<!-- 参考信息 -->