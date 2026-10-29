代发 wailian999

[P01] 生成 UUID
来源：http://3g.zdbjq.cn/Article/details/guiyyokkw.sHtML

Py:   str(uuid.uuid4())
来源：http://m.share.zdbjq.cn/Article/details/gofimpkmk.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.blog.hesvh.cn/Article/details/gtmanzswa.sHtML

JS:   crypto.randomUUID()
来源：http://mobile.hesvh.cn/Article/details/gxihsiadn.sHtML

TS:   crypto.randomUUID()
来源：http://blog.hesvh.cn/Article/details/ggmeiphnl.sHtML

Java: UUID.randomUUID().toString()
来源：http://read.share.zdbjq.cn/Article/details/guulupkvf.sHtML

Go:   // 用 github.com/google/uuid
来源：http://m.share.hesvh.cn/Article/details/guefmanhe.sHtML

Ruby: SecureRandom.uuid
来源：http://blog.hesvh.cn/Article/details/gwuphsxxk.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://blog.fehbvm.com/Article/details/gropcnaze.sHtML

[P02] MD5 / SHA256 摘要
来源：http://mobile.hesvh.cn/Article/details/gsxmuasfv.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://3g.hesvh.cn/Article/details/gtevqtucj.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.m.share.hesvh.cn/Article/details/gshpkyzyj.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://m.share.zdbjq.cn/Article/details/gmkckabqg.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://wap.zdbjq.cn/Article/details/gbyhbrvzf.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.share.zdbjq.cn/Article/details/gduhxgrps.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://wap.fehbvm.com/Article/details/gvfnushbc.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://read.share.hesvh.cn/Article/details/grznzhwbv.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.share.hesvh.cn/Article/details/grekglwui.sHtML

[P03] 生成短随机字符串
来源：http://read.share.hesvh.cn/Article/details/gjzpxfarj.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://wap.fehbvm.com/Article/details/guovbzrqj.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://3g.hesvh.cn/Article/details/gdqqynotm.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.fehbvm.com/Article/details/ghixwhshi.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.fehbvm.com/Article/details/gskdhwfma.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://m.share.zdbjq.cn/Article/details/gdwarcdab.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://m.share.zdbjq.cn/Article/details/gskwyfkzv.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://3g.zdbjq.cn/Article/details/ghqujjota.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.m.share.hesvh.cn/Article/details/gdptmaqag.sHtML

[P04] 求长度
来源：http://blog.fehbvm.com/Article/details/gwukfmqcy.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.blog.hesvh.cn/Article/details/gphzppmoy.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.hesvh.cn/Article/details/gosuenrno.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.zdbjq.cn/Article/details/gtjrbpjqz.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.hesvh.cn/Article/details/gxvfzmgcj.sHtML

Java: list.size();  map.size();  s.length()
来源：http://m.share.hesvh.cn/Article/details/gjpmorbds.sHtML

Go:   len(arr);  len(m)
来源：http://3g.fehbvm.com/Article/details/ggemfyosr.sHtML

Ruby: x.length;  x.size
来源：http://3g.fehbvm.com/Article/details/gvhbywgai.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://3g.fehbvm.com/Article/details/gpqrpofar.sHtML

[P05] 判断两个对象内容是否相等
来源：http://blog.hesvh.cn/Article/details/gsvfdfkef.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.blog.hesvh.cn/Article/details/gsaobehxm.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://read.share.zdbjq.cn/Article/details/ghztjxmpe.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.m.share.zdbjq.cn/Article/details/gevuigbdh.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.share.hesvh.cn/Article/details/gjfaaguwg.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://m.share.fehbvm.com/Article/details/gzygishsx.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.blog.hesvh.cn/Article/details/gkhmtswiw.sHtML

Ruby: a == b
来源：http://m.share.hesvh.cn/Article/details/gniujjnzi.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://read.share.hesvh.cn/Article/details/gwlslvxvv.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://read.share.zdbjq.cn/Article/details/gumgmrvpq.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://blog.hesvh.cn/Article/details/gqsfctyzp.sHtML

PHP:  if (empty($x)) {}
来源：http://mobile.hesvh.cn/Article/details/gvkkswhau.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://wap.hesvh.cn/Article/details/gxornhnwd.sHtML

TS:   if (x == null) {}
来源：http://read.share.fehbvm.com/Article/details/gayhvuxsj.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://baike.fehbvm.com/Article/details/gjgbelksp.sHtML

Go:   if x == nil {}
来源：http://m.share.hesvh.cn/Article/details/gurwcvrtr.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.share.zdbjq.cn/Article/details/geabqrwqt.sHtML

C#:   if (x is null) {}
来源：http://www.blog.hesvh.cn/Article/details/gxedsvhxf.sHtML

[P07] 防抖与节流
来源：http://mobile.fehbvm.com/Article/details/gwptuaoha.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.blog.zdbjq.cn/Article/details/gechxxgwr.sHtML

PHP:  // 手写时间戳比较
来源：http://3g.fehbvm.com/Article/details/ggdhferlj.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.hesvh.cn/Article/details/gozzqnpbs.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.hesvh.cn/Article/details/ghbgugdqd.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://baike.hesvh.cn/Article/details/gpwvsmvlu.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.blog.hesvh.cn/Article/details/gwivbldxq.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.blog.hesvh.cn/Article/details/gsdceeswa.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://wap.fehbvm.com/Article/details/gmsnjluxc.sHtML

[P08] 处理浮点精度问题
来源：http://www.share.hesvh.cn/Article/details/gbjydjiwc.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://m.share.hesvh.cn/Article/details/gkcuxjjuu.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://wap.hesvh.cn/Article/details/guhlmekpw.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://mobile.fehbvm.com/Article/details/grwdmugql.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://read.share.hesvh.cn/Article/details/gqsoapfrb.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.share.fehbvm.com/Article/details/ggkegyaxj.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.m.share.hesvh.cn/Article/details/gtluqiuqp.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.share.hesvh.cn/Article/details/gtjwwzppq.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://mobile.zdbjq.cn/Article/details/gfkraqlgx.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gdjulzskj.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://mobile.fehbvm.com/Article/details/gwynovpee.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gcpmehwny.sHtML

[Q01] 创建表
来源：http://mobile.zdbjq.cn/Article/details/ghmwzrhim.sHtML

CREATE TABLE users (
来源：http://www.blog.fehbvm.com/Article/details/ggboxzwgp.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.fehbvm.com/Article/details/ggivtcork.sHtML

name VARCHAR(50) NOT NULL,
来源：http://wap.zdbjq.cn/Article/details/gqhtkdepl.sHtML

email VARCHAR(100) UNIQUE,
来源：http://blog.hesvh.cn/Article/details/gpwkwczkl.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://m.share.fehbvm.com/Article/details/gonfyzapi.sHtML

);
来源：http://wap.hesvh.cn/Article/details/gxelhcbyc.sHtML

[Q02] 创建带外键的表
来源：http://www.share.hesvh.cn/Article/details/gskvukkej.sHtML

CREATE TABLE orders (
来源：http://blog.zdbjq.cn/Article/details/grkfycsvl.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.hesvh.cn/Article/details/gpjbdwrhv.sHtML

user_id INT NOT NULL,
来源：http://3g.hesvh.cn/Article/details/gsngfytoz.sHtML

amount DECIMAL(10, 2),
来源：http://mobile.hesvh.cn/Article/details/ggtmatjpa.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://baike.fehbvm.com/Article/details/gctvooytc.sHtML

);
来源：http://wap.hesvh.cn/Article/details/gezjtalir.sHtML

[Q03] 增加列
来源：http://mobile.hesvh.cn/Article/details/gicjeuxxw.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://m.share.fehbvm.com/Article/details/glkppzjih.sHtML

[Q04] 修改列类型
来源：http://read.share.zdbjq.cn/Article/details/gsjfjsjql.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://baike.hesvh.cn/Article/details/ggkahawnk.sHtML

[Q05] 重命名列
来源：http://m.share.hesvh.cn/Article/details/gpghffvmd.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://blog.fehbvm.com/Article/details/gmmrbhvii.sHtML

[Q06] 删除列
来源：http://baike.hesvh.cn/Article/details/gjtkhguat.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://3g.zdbjq.cn/Article/details/gjrukejbp.sHtML

[Q07] 删除表
来源：http://wap.hesvh.cn/Article/details/gkfdpxvlo.sHtML

DROP TABLE IF EXISTS orders;
来源：http://3g.zdbjq.cn/Article/details/gqvuguiqu.sHtML

[Q08] 创建普通索引
来源：http://m.share.hesvh.cn/Article/details/grhpfgeji.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://3g.zdbjq.cn/Article/details/glnyraurl.sHtML

[Q09] 创建唯一索引
来源：http://wap.zdbjq.cn/Article/details/gzkkshjrb.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://mobile.zdbjq.cn/Article/details/gvjueugqq.sHtML

[Q10] 插入单行
来源：http://read.share.fehbvm.com/Article/details/gsdwdtncx.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://baike.hesvh.cn/Article/details/gqspxdljd.sHtML

[Q11] 一次插入多行
来源：http://3g.zdbjq.cn/Article/details/gwfflyode.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://blog.fehbvm.com/Article/details/gzyseyjzo.sHtML

[Q12] 插入后取自增 ID
来源：http://mobile.zdbjq.cn/Article/details/gfswlhcst.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://read.share.zdbjq.cn/Article/details/gynsuimof.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://3g.zdbjq.cn/Article/details/gwrkyliwm.sHtML

[Q13] 忽略重复插入
来源：http://mobile.fehbvm.com/Article/details/godhmctyl.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.share.zdbjq.cn/Article/details/gdotzdxnt.sHtML

[Q14] 存在则更新（upsert）
来源：http://m.share.fehbvm.com/Article/details/gcmhzkzva.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.share.hesvh.cn/Article/details/glgfiqcaa.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://3g.fehbvm.com/Article/details/goglmqetc.sHtML

[Q15] 查询全部
来源：http://blog.fehbvm.com/Article/details/gfnekxhqb.sHtML

SELECT * FROM users;
来源：http://read.share.fehbvm.com/Article/details/gzmfnjyqn.sHtML

[Q16] 查询指定列
来源：http://wap.hesvh.cn/Article/details/gftnldaqu.sHtML

SELECT id, name FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gyvmfurnb.sHtML

[Q17] 条件查询
来源：http://wap.zdbjq.cn/Article/details/giqazwmwu.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://read.share.zdbjq.cn/Article/details/gnbfttxzw.sHtML

[Q18] 模糊匹配
来源：http://www.blog.fehbvm.com/Article/details/glgyxrzdt.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://baike.zdbjq.cn/Article/details/gwofvvwfy.sHtML

[Q19] 范围查询
来源：http://blog.fehbvm.com/Article/details/gpvlbxkkx.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.blog.zdbjq.cn/Article/details/gamwienro.sHtML

[Q20] IN 列表
来源：http://baike.fehbvm.com/Article/details/gzavacstt.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://read.share.hesvh.cn/Article/details/gfdolwbyn.sHtML

[Q21] 空值判断
来源：http://blog.fehbvm.com/Article/details/gjpnhftvr.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://baike.fehbvm.com/Article/details/gvpjsbpkq.sHtML

[Q22] 排序
来源：http://3g.fehbvm.com/Article/details/gfigqwcgd.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.m.share.fehbvm.com/Article/details/gcdhgxtii.sHtML

[Q23] 分页
来源：http://m.share.fehbvm.com/Article/details/gkdjqzfga.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://baike.hesvh.cn/Article/details/garlruxzb.sHtML

[Q24] 去重
来源：http://m.share.zdbjq.cn/Article/details/gsphshbsv.sHtML

SELECT DISTINCT city FROM users;
来源：http://blog.zdbjq.cn/Article/details/gdlothxfj.sHtML

[Q25] 只取前 N 条
来源：http://baike.zdbjq.cn/Article/details/grxripwpy.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.m.share.fehbvm.com/Article/details/gxrahewkl.sHtML

[Q26] 计数
来源：http://www.share.hesvh.cn/Article/details/gztyhkusk.sHtML

SELECT COUNT(*) FROM users;
来源：http://blog.fehbvm.com/Article/details/gfxzzhkwt.sHtML

[Q27] 条件计数
来源：http://blog.hesvh.cn/Article/details/goilragln.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://3g.fehbvm.com/Article/details/gwduoofxn.sHtML

[Q28] 求和与平均
来源：http://blog.hesvh.cn/Article/details/gjbmyeerg.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.m.share.zdbjq.cn/Article/details/gbofneylb.sHtML

[Q29] 最大最小值
来源：http://3g.fehbvm.com/Article/details/ggooxyoka.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/geqhmvbbi.sHtML

[Q30] 分组统计
来源：http://3g.zdbjq.cn/Article/details/gixiztaol.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://3g.fehbvm.com/Article/details/gceafiabl.sHtML

[Q31] 分组后过滤
来源：http://m.share.hesvh.cn/Article/details/gboxmmbzz.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://m.share.zdbjq.cn/Article/details/gokzmxmql.sHtML

[Q32] 分组拼接字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gflxygzuo.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://read.share.zdbjq.cn/Article/details/gogiqgxls.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.blog.zdbjq.cn/Article/details/gopyyeeqd.sHtML

[Q33] 多列分组
来源：http://www.share.fehbvm.com/Article/details/gyvcfcbee.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://read.share.hesvh.cn/Article/details/gkiwgcnni.sHtML

[Q34] 每组取第一条
来源：http://www.blog.zdbjq.cn/Article/details/gogxkwzdd.sHtML

SELECT * FROM (
来源：http://mobile.zdbjq.cn/Article/details/guwulvjvc.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://blog.fehbvm.com/Article/details/gqwqueyzv.sHtML

) t WHERE rn = 1;
来源：http://read.share.hesvh.cn/Article/details/gvuodxeit.sHtML

[Q35] 内连接
来源：http://www.blog.hesvh.cn/Article/details/gdwqomwdf.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://m.share.fehbvm.com/Article/details/gfndmqkjn.sHtML

[Q36] 左连接
来源：http://baike.fehbvm.com/Article/details/grnwkfxvu.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://mobile.hesvh.cn/Article/details/gcxnurjtt.sHtML

[Q37] 右连接
来源：http://wap.fehbvm.com/Article/details/gdfdnmrby.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://read.share.zdbjq.cn/Article/details/gvjwzkrfp.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://mobile.fehbvm.com/Article/details/glyehlhou.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://blog.hesvh.cn/Article/details/groaeybqs.sHtML

[Q39] 自连接（查上下级）
来源：http://m.share.hesvh.cn/Article/details/gdzrxwcmn.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://3g.fehbvm.com/Article/details/gfoejudvx.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.share.zdbjq.cn/Article/details/glknzyuoy.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.share.hesvh.cn/Article/details/grseneluw.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://3g.zdbjq.cn/Article/details/gkkyxqjtu.sHtML

[Q41] 多表连接
来源：http://3g.hesvh.cn/Article/details/guykrajrh.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.share.hesvh.cn/Article/details/groiwnkec.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.blog.fehbvm.com/Article/details/gxtvxxemr.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://blog.fehbvm.com/Article/details/gvsyczydu.sHtML

[Q42] 连接条件附加过滤
来源：http://www.share.zdbjq.cn/Article/details/gciulznkv.sHtML

SELECT u.name, o.amount FROM users u
来源：http://m.share.zdbjq.cn/Article/details/gxhthleum.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://m.share.zdbjq.cn/Article/details/giqdtigko.sHtML

[Q43] 标量子查询
来源：http://wap.hesvh.cn/Article/details/gqfaluqze.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://3g.hesvh.cn/Article/details/ghaztaauq.sHtML

[Q44] IN 子查询
来源：http://baike.hesvh.cn/Article/details/goipjjphp.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.blog.fehbvm.com/Article/details/gedxzvuau.sHtML

[Q45] EXISTS 判断存在
来源：http://m.share.fehbvm.com/Article/details/gnlcnxlxk.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.zdbjq.cn/Article/details/gnfhplutl.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://blog.zdbjq.cn/Article/details/gfmlxozhr.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.fehbvm.com/Article/details/gpgakkvrz.sHtML

[Q47] 与平均值比较
来源：http://baike.fehbvm.com/Article/details/gthflqjea.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.m.share.hesvh.cn/Article/details/gsykeurcn.sHtML

[Q48] CTE 公用表表达式
来源：http://mobile.zdbjq.cn/Article/details/gmnnusxcd.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.m.share.fehbvm.com/Article/details/ggnqsaupw.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://baike.fehbvm.com/Article/details/gcczawngq.sHtML

[Q49] 更新单行
来源：http://m.share.zdbjq.cn/Article/details/gztqjiywv.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://blog.zdbjq.cn/Article/details/gnsymjgao.sHtML

[Q50] 批量更新
来源：http://www.blog.zdbjq.cn/Article/details/gpnloekpb.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://3g.fehbvm.com/Article/details/gjhkowkwd.sHtML

[Q51] 用子查询更新
来源：http://3g.fehbvm.com/Article/details/gewfifvhf.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://blog.zdbjq.cn/Article/details/gwvfseglz.sHtML

[Q52] 删除指定行
来源：http://read.share.fehbvm.com/Article/details/ggcwujzsf.sHtML

DELETE FROM users WHERE id = 10;
来源：http://wap.zdbjq.cn/Article/details/gdxxarimq.sHtML

[Q53] 按条件删除
来源：http://mobile.fehbvm.com/Article/details/gwctpixhn.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://blog.hesvh.cn/Article/details/gtgocsxsg.sHtML

[Q54] 清空表
来源：http://www.blog.hesvh.cn/Article/details/gwlodcwzp.sHtML

TRUNCATE TABLE logs;
来源：http://baike.fehbvm.com/Article/details/gkktpbwhd.sHtML

[Q55] 排名（并列占位）
来源：http://mobile.zdbjq.cn/Article/details/gxxmhldqj.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.blog.fehbvm.com/Article/details/gdoiqksnf.sHtML

[Q56] 密集排名（并列不占位）
来源：http://baike.fehbvm.com/Article/details/gursduauj.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://m.share.hesvh.cn/Article/details/gajpqqvog.sHtML

[Q57] 行号
来源：http://baike.zdbjq.cn/Article/details/gqalpxmsi.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gdpjanqna.sHtML

[Q58] 累计求和
来源：http://blog.hesvh.cn/Article/details/gyajnptgd.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.blog.fehbvm.com/Article/details/guyhsqmuy.sHtML

[Q59] 分组内累计
来源：http://m.share.hesvh.cn/Article/details/gnyuvsmhv.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://read.share.hesvh.cn/Article/details/gdtersqea.sHtML

[Q60] 取上一行 / 下一行
来源：http://mobile.zdbjq.cn/Article/details/gwaagodme.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.share.fehbvm.com/Article/details/giicbmogk.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.blog.fehbvm.com/Article/details/ggqtaxzes.sHtML

[Q61] 移动平均
来源：http://www.m.share.fehbvm.com/Article/details/gvtftynyj.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://baike.hesvh.cn/Article/details/gyvqsrbft.sHtML

[Q62] 分组占比
来源：http://m.share.fehbvm.com/Article/details/gvikdprbg.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.blog.hesvh.cn/Article/details/gypegkeug.sHtML

[Q63] 开启事务
来源：http://wap.fehbvm.com/Article/details/gfbhkyvpw.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.blog.zdbjq.cn/Article/details/gczkzclma.sHtML

[Q64] 提交事务
来源：http://m.share.zdbjq.cn/Article/details/gmcioynzn.sHtML

COMMIT;
来源：http://m.share.fehbvm.com/Article/details/gvtrwcsdd.sHtML

[Q65] 回滚事务
来源：http://www.blog.fehbvm.com/Article/details/ggqfrhvhz.sHtML

ROLLBACK;
来源：http://www.share.hesvh.cn/Article/details/gmvzyvqlc.sHtML

[Q66] 行锁查询
来源：http://read.share.hesvh.cn/Article/details/gvvdhwqly.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://read.share.zdbjq.cn/Article/details/gnvxqneni.sHtML

[Q67] 设置隔离级别
来源：http://wap.zdbjq.cn/Article/details/gakmqgyuf.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.share.zdbjq.cn/Article/details/gqidtcbps.sHtML

[Q68] 保存点
来源：http://mobile.fehbvm.com/Article/details/gkfrxresg.sHtML

SAVEPOINT sp1;
来源：http://3g.fehbvm.com/Article/details/gwjnvhxce.sHtML

ROLLBACK TO sp1;
来源：http://www.share.hesvh.cn/Article/details/ggxgzntso.sHtML

[Q69] 查看执行计划
来源：http://wap.hesvh.cn/Article/details/ghiepapao.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.m.share.fehbvm.com/Article/details/ghfvlckjq.sHtML

[Q70] 更新统计信息
来源：http://www.share.hesvh.cn/Article/details/gviwumemx.sHtML

ANALYZE TABLE users;
来源：http://www.m.share.zdbjq.cn/Article/details/gknuqmruv.sHtML

[Q71] 查看建表语句
来源：http://wap.zdbjq.cn/Article/details/gssqiuhme.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.blog.zdbjq.cn/Article/details/gthfcbdxd.sHtML

[Q72] 查看索引
来源：http://wap.zdbjq.cn/Article/details/gjqttmofh.sHtML

SHOW INDEX FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gokkiaipo.sHtML

[Q73] 查看表状态
来源：http://www.share.hesvh.cn/Article/details/gkwmuzfbk.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://wap.hesvh.cn/Article/details/gmbwyqzsc.sHtML

[Q74] 强制使用索引
来源：http://www.blog.hesvh.cn/Article/details/gcitwzvwd.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://blog.zdbjq.cn/Article/details/gdkwnmlmh.sHtML

[Q75] 日期格式化
来源：http://baike.hesvh.cn/Article/details/gfytfawju.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.m.share.hesvh.cn/Article/details/gtlftlosy.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.blog.zdbjq.cn/Article/details/gwpcvwqkx.sHtML

[Q76] 按天统计
来源：http://www.blog.fehbvm.com/Article/details/gmfbekica.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://3g.fehbvm.com/Article/details/guhslmxdj.sHtML

[Q77] 时间加减
来源：http://m.share.fehbvm.com/Article/details/ghvispbfm.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://baike.fehbvm.com/Article/details/gnutpdqlh.sHtML

[Q78] 当前时间
来源：http://wap.zdbjq.cn/Article/details/gdyuccbfq.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://blog.fehbvm.com/Article/details/ganzlyktr.sHtML

[Q79] 字符串拼接
来源：http://baike.zdbjq.cn/Article/details/gybemmvsr.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://read.share.hesvh.cn/Article/details/gsxclsrsr.sHtML

[Q80] 字符串截取
来源：http://www.m.share.hesvh.cn/Article/details/gehytkbxc.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://mobile.hesvh.cn/Article/details/gjhxnpoyz.sHtML

[Q81] 字符串替换
来源：http://read.share.zdbjq.cn/Article/details/giuidzfzh.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://m.share.fehbvm.com/Article/details/gmltdhrbb.sHtML

[Q82] 字符长度与字节长度
来源：http://baike.fehbvm.com/Article/details/gppogftpf.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://wap.fehbvm.com/Article/details/geuutvqyl.sHtML

[Q83] 大小写转换
来源：http://blog.fehbvm.com/Article/details/gtethhxfh.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://wap.hesvh.cn/Article/details/gulbvnjeb.sHtML

[Q84] 去除首尾空格
来源：http://mobile.fehbvm.com/Article/details/gqzkapzpn.sHtML

SELECT TRIM(name) FROM users;
来源：http://baike.zdbjq.cn/Article/details/gmukwdtxw.sHtML

[Q85] 数值取整
来源：http://wap.fehbvm.com/Article/details/grcpqpyya.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://3g.fehbvm.com/Article/details/ggvieaxis.sHtML

[Q86] 读取 JSON 字段
来源：http://m.share.zdbjq.cn/Article/details/gqklreogc.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://m.share.hesvh.cn/Article/details/grvvdaeyl.sHtML

[Q87] JSON 字段做条件
来源：http://m.share.hesvh.cn/Article/details/gfenrhewr.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://wap.zdbjq.cn/Article/details/gfitvodxx.sHtML

[Q88] 行转列（条件聚合）
来源：http://m.share.hesvh.cn/Article/details/gduwmuhvx.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://read.share.zdbjq.cn/Article/details/gapllxkqz.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gvfnpjihi.sHtML

[Q89] 判断表是否存在
来源：http://3g.fehbvm.com/Article/details/gauyyecwh.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://read.share.hesvh.cn/Article/details/gptcdkcrf.sHtML

[Q90] 生成序号列
来源：http://www.blog.zdbjq.cn/Article/details/gahedkqjn.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://wap.zdbjq.cn/Article/details/gfpyzavfl.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gapjcmvzk.sHtML

R. Bash 专题
来源：http://baike.zdbjq.cn/Article/details/ghtfdnsls.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gobucnkrd.sHtML

[R01] shebang 与严格模式
来源：http://www.share.zdbjq.cn/Article/details/gscwidviy.sHtML

#!/usr/bin/env bash
来源：http://mobile.hesvh.cn/Article/details/gehcgzsxe.sHtML

set -euo pipefail
来源：http://baike.zdbjq.cn/Article/details/gqijbtvqh.sHtML

[R02] 变量赋值与使用
来源：http://www.m.share.fehbvm.com/Article/details/giuolfgde.sHtML

name="Tom"; echo "$name"
来源：http://wap.fehbvm.com/Article/details/gcdsnptzv.sHtML

[R03] 只读变量
来源：http://3g.fehbvm.com/Article/details/gjvkrthqa.sHtML

readonly PI=3.14
来源：http://m.share.hesvh.cn/Article/details/gthfmbrvv.sHtML

[R04] 位置参数
来源：http://wap.zdbjq.cn/Article/details/glavhouxe.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://m.share.zdbjq.cn/Article/details/guxbjxwki.sHtML

[R05] 参数默认值
来源：http://wap.zdbjq.cn/Article/details/grcehndzi.sHtML

name="${1:-default}"
来源：http://www.m.share.fehbvm.com/Article/details/gkcwbvatf.sHtML

[R06] 判断命令是否存在
来源：http://mobile.zdbjq.cn/Article/details/gqjbzomye.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://wap.hesvh.cn/Article/details/garabruwe.sHtML

[R07] if 判断文件
来源：http://www.blog.hesvh.cn/Article/details/gcyxqmabp.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.m.share.hesvh.cn/Article/details/goxqztlgw.sHtML

[R08] 数值比较
来源：http://www.blog.fehbvm.com/Article/details/goohmescn.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://mobile.zdbjq.cn/Article/details/gxbojvewz.sHtML

[R09] 字符串比较
来源：http://wap.fehbvm.com/Article/details/gsqyjmmwk.sHtML


<!-- 参考信息 -->