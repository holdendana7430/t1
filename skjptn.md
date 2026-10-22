代发 wailian999

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt2xwndobtm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2slqdcopi.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt2jahjpkwe.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2unnidlol.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2waozdeuh.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt2iiqofytb.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt2loxffucp.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2jkdxuwsr.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2efmvaizs.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2uxextzvx.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2vjtdbwen.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt2lmrqfwxa.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2qcrojnex.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt2kkuknlje.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt2favbdjgl.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt2ixvodrrk.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt2abuwlfal.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt2oeqivmmo.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt2ckikulwf.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt2etokjeck.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt2wxlvctyr.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt2icmcuvsp.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt2wrzuuxto.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt2bgmvkuat.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt2zpjlunql.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2xlmqgrhg.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2mtstvprk.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt2htyovyhi.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt2vidggffa.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt2adhimsop.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt2jcvsphbq.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt2mbqgnccx.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt2rhrqeqch.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2nnzxqkdz.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2nzsbkdwp.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2oftaztwf.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt2nwbaiwuh.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt2jcqgtugn.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt2nmbetjsm.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt2zpoofeoc.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt2lnzhuxkv.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt2vjugekrt.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt2ilhhykvy.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt2mrtkyjlr.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2ggrcjicf.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt2xqqcokky.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt2johzduuc.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt2yesudwhe.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt2xgfvhrho.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt2gvapiweu.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt2kreeixbl.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2yaizvsip.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt2mrbiimao.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt2tgpxaryk.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2mkdoufjw.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt2usdmnhhe.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt2lpapokei.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt2dnhofjag.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt2mlmaikzg.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt2htvqhrke.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt2omgrgxpp.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2mlctsfrw.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2gcjabhdp.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt2vtnvbsmo.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt2ncstdmsd.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt2kglhpmgd.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt2ckhgsgho.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt2tuxdflla.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt2yinselro.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt2liykozsn.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt2xowppdma.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2tcoplpua.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt2topujwmt.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt2ylpwuuxh.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt2ydallexy.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt2qqzyezlo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2guoihuja.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt2jlxzghek.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tnjjakfb.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt2jjqgyxpr.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt2ljcvgdwc.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2rvlmehts.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2sqykketf.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt2ufvhqvxs.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt2bjueqfvc.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2cveyqhoa.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt2jfkaselv.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt2ftaucozs.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2hjmmwawv.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2kefrkneu.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt2ozjzzphv.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt2shnhkxtw.html

);
来源：http://www.52xcode.cn/Article/details/gt2wvvmdxdt.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt2fovokmwk.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt2jjsgsowa.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt2cdfpaacp.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt2ihhtxvdb.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt2uaohfxrq.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt2ckfvqvgj.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt2jrvqzmsm.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt2nwxzynvy.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt2usupwgmm.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt2rgbzxfgj.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt2rcdyavgt.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2siplenet.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt2hteuhlta.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2azwyworg.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt2mekzrlpw.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt2isjbzizb.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt2fqsythft.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2irvfaxlr.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt2ugfoomsq.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt2slhchdnv.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt2anktolvg.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt2lnbhwysg.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt2elsyhkuh.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt2kgubhjof.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt2wrqsanlv.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt2gfuuwlkk.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt2rxvjcezm.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2uzhpkucu.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt2rjdswgrj.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2qokyzqim.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt2yhwwbzcv.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt2pfphvoan.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt2lkyntakg.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt2mxxvpfuc.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt2ilndxvqq.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt2dyzifmeo.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt2cmpnbcnf.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2ayuyhrya.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt2vjmqmpqr.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt2aburmwcx.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt2blwedrwo.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt2trgsmnkj.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt2viumslxp.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt2siickshi.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2jjklyoqb.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt2yhjfheak.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt2isvzpehg.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt2axebpydx.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt2itftasrv.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2tpxiojqc.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt2rbotpuqg.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2qvhqjtsx.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt2egiacyrv.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2norxuhro.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt2tmhffblf.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2nvfdhvry.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt2bvxeupfj.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2krgonahj.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt2grhdawpb.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt2jonlfmeb.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2uuaiwybo.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2tjhqqduo.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt2ftlrfnrj.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt2bnhubsqn.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt2pqmaexzi.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt2sqjutiur.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt2fpjnkafp.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt2lfujtmpq.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt2gbhqaszo.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt2aozuxerl.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2gtxjuixb.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt2aetstpdy.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2bpezmuxt.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt2wuuabycq.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt2ngsmgiyd.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt2jvvtdhxm.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt2btvknfsw.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt2eeaknvhp.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt2bcwooamy.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt2fqfbxtot.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt2lxdhpqzz.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt2kwczwxsg.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt2rvhkbtno.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt2fitkhkst.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt2ahzwmfxi.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt2lamshble.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt2foxvbtuc.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt2dzcvnmnc.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt2uvisuqtw.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt2ccdeqbmo.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt2yorrxwxj.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt2fiwrubpw.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt2kpmgljhz.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt2zotsmjoz.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2apxuhyib.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt2gbxtvunk.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2jefbdsyh.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt2wzptdwva.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt2mppcsqtc.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt2yxyiunaj.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt2fzwwnxjw.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt2vlaccipw.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt2yqskwvss.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2ssqhpyqo.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt2vxokqtoy.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2szgeeowg.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt2umwwdgib.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt2jibdfrcr.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt2nbqsabvp.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2ybbprinn.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt2gtdinpdx.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt2zirzkcvo.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt2qwrasbyu.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt2ddsfkovu.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt2ibnrvuic.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2gdhdcxnp.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt2esvrmxbb.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2dtkzrcuc.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt2ceavlbmo.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2lqbwhtjg.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt2wsndhimt.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2avvdszak.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt2tztacwno.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2qjykgtsc.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt2josetbmq.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt2bpqqacpi.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2qhvycfmg.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt2depsaheo.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2uoqeanxt.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt2imquptdl.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2qmhvghrh.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt2ngjnygnr.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt2fhikhrwh.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt2wfwcipok.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt2yqbtbhsn.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt2pnbpykqw.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt2rqplaqwp.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt2jvznolfd.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt2eshtclzn.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt2auuxmivw.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt2wcnpwavc.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt2ximmhezx.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2djedavpi.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt2dlwoznrn.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt2fpnopotz.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt2jmbpbfhg.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt2sgxqrivr.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt2ndpmppxz.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt2syvmlytu.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt2xijcvaih.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt2kafhutmr.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt2qealajds.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt2xstzhjaa.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt2gpzdqjts.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt2pvacdajv.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt2gryconzb.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2ymvuhrrc.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2zqxkmaal.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt2loxaaxsi.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt2xsknpqwv.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt2ieremqac.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt2cxsbzymh.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt2yjhbhsmh.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2lacawmmk.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt2eerxmloz.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2ljejdpst.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt2pvgehzlx.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt2dxkafbxf.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2kxytvsxw.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2ptdtcxwn.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ancdrmda.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt2lgtqnwjb.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2saiivlvh.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2huyzpeup.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2gfraviix.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt2tirhsxqv.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2mndfqykg.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt2joxbopod.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt2yqwdkwvx.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt2hqrgbicz.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt2rdlrxriq.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt2slgfqzpf.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt2bifvgoup.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt2iegbkejx.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt2vkgjgfhx.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt2lcuepdgu.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2csocvjzc.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt2uubglyhm.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt2bvdnbdsl.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt2mjahrljj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2sldigsbf.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt2ykgizdha.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mtncfyiq.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt2mwujddmu.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt2nhmcpfhe.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt2ecojqnzy.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt2sutbjils.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt2oasbhcnk.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt2uaboyuoz.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt2wgxitjln.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt2uzmrkzce.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt2uqfayxsg.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt2qrgmntzx.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt2secfrqnz.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2ozacppzd.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2iythkfec.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt2sxfgjjbc.html


<!-- 参考信息 -->