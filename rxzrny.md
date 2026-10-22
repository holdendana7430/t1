代发 wailian999

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2lcgzdgfi.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2igvgehio.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt2favyybxw.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt2hmrgrbrq.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt2xvgrbwsa.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jriqtoio.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt2hextoxkz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mhjniiqr.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2qdetqlan.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt2wpdndejc.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt2chttvtrq.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2xfegoivx.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2jhrujwkh.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2iixwtgel.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2npymkvji.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt2xkujpujv.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt2ssxkridw.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt2nleuotdv.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt2ggopmkqh.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt2tskylcoc.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt2zzfnlegs.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt2vwgnaxyg.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2jadqjudy.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt2swbubehg.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt2nmfrbmvl.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt2vlyjrxac.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt2npytawla.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt2vfqpczon.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt2xuprlaww.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2rwvjzcdm.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2vyggkgyo.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt2jymijoxk.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt2utobcfmj.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt2apocmxae.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt2rbkbtnjh.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt2tyundvzz.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt2mrvetabf.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2ezmlguus.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2ckrsjnvb.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2vkqtyixj.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt2ynwagelg.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt2xvsbohmz.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt2lvwbrorj.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2cmpbpvom.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt2rtgpazsw.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt2malcwmja.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt2medvwxql.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt2pidzglde.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2fylcpmrk.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt2eqpdvknc.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2mcniliej.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt2tvssjnzq.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt2hheanrte.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt2hsytvdch.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt2zxakurxq.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2dzsrgakh.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt2htnwucal.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt2okojikey.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2mknlfoev.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt2whizcpcb.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt2mjjqaeom.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt2irvuvqqe.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt2gjptmoyb.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt2fbzlfmkg.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt2cdugebrx.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2hcjtbkwj.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2yfhazyim.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt2ctmoyvhq.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt2yuvlubcn.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt2tzinwrmu.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt2oxtrnavh.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt2rpsvsoxf.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt2slcdomae.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt2ahpdgfff.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt2spppqsde.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2wsitymfk.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt2wqboadlk.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt2slouvkkk.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt2nvugxual.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt2vwrjjhqa.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ibmjjeqe.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt2vdcvzztx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2elmwvyak.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt2cjabtvve.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt2oshoacuj.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2qbwzipnz.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2onauvpxa.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt2lwuywmmx.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt2ocqzamls.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2necafyik.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt2zczuyyic.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt2rmqzdqnh.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2tdaykmpe.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2ryyiueur.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt2lnatkucj.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt2hteufbaa.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2wpntutqi.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt2qtzczqkz.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt2vbwxmdxy.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt2toqzfvzy.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2iumvvjbd.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt2owpymcgq.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt2fbqysrbl.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt2quykdhuh.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt2sxuzxqlc.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt2zaxaksnz.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt2xhxfbqhl.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt2szvuakhp.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2vjitslsu.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt2rykgrszv.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2myihfmpq.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt2ywuqazsc.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt2tnnawlxm.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt2kiysvisd.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2ticesnnp.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt2zmchrcmv.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt2eihobifc.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt2dsmlcdlw.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt2unuhxjrw.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2pigklblp.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt2iyicuywh.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt2uwtehtgi.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt2owonqxfw.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt2ornbsatf.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2qfekulft.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt2qmixnopr.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2onjyugio.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt2untcwaar.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2hqayysqq.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt2evurgawk.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt2kjagayjz.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt2smtsrgmc.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt2ivtvwfpz.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt2xwkvaecq.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2stoifibp.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt2qpbiopxg.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2twjepfws.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt2ilgmsccf.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt2gpgwcucd.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt2isglwlss.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt2isovzpkv.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2uiytiryz.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt2wpwtdvgz.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt2qtpnwqnh.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt2yyhdlztk.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt2onxzsdit.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2qojkrsbb.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt2rcinbsty.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt2qvdvypsi.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt2iyiwvgor.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2xavftlgf.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2jjmlqoxw.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2zxubrevj.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt2hibkxopt.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2xehyikzc.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt2qjmmazce.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt2gwbukmni.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2xqwiygww.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2nmmcibdv.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt2limftequ.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt2gzianywa.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt2wmprtike.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt2anhvmrsd.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt2xrbgqwto.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt2bmmvgeot.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt2crkabaoq.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt2mzizrnmt.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2arcycptg.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt2gcmwfgmw.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2viedbyhe.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt2rgucbqsm.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt2zgvrmwej.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt2ntmcsclk.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt2llpgggmj.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt2ayvctnfb.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt2subpmubc.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt2aplqzqqy.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt2mfhwmbip.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt2xftuffje.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt2kglzqdca.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt2unhtjdce.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt2mevhmwox.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt2dxxhubdr.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt2phirsiiw.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt2newqsdhp.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt2lcyaiano.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt2lyxgsikb.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt2ylwhvwxv.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt2otwojtvf.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt2ayundoli.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt2licsnmuk.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2ogtseiod.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt2wzbserpw.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2rzlauqoo.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt2ihmwvgjh.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt2qlwynjwg.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt2ajgaxdet.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt2gnnvykqc.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt2tlyhulag.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt2gbtbiqsn.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2wlchisoc.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt2rhsiyhnj.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt2ksbbnxdc.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt2yiiytsra.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt2ghmyuhdp.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt2ihbnyoef.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2lgwurudb.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt2fhciapwo.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt2nhoeefml.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt2svgbrezf.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt2zpnunxow.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt2cgfakhzw.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2tvjnwsgk.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt2iowojyfm.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2zonpihde.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt2xfluxnni.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2roufwcnw.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt2bropbcnp.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2jchggbri.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt2xqnmntbg.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2hintoxwe.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt2rhcobxvj.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt2mumngraa.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2ksumqncz.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt2zfrnqwsa.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2unmoxgfp.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt2plpoazuj.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2ggxbrxik.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt2jhuapqcg.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt2wpumzver.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt2ywxteaft.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt2jfkjnsdk.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt2vdpaliyr.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt2zlewvhht.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt2cjpwevou.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt2gugplcei.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt2mkscsxec.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt2rftshhnt.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt2duvjanej.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt2ihedrqom.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2joklykym.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt2ldmzjqbj.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt2tqfjzqkx.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt2itzgnqav.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt2aaluslpc.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt2lmbiwfxm.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt2zoqspyrm.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt2rxjtockl.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt2gfmntuhx.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt2pgqbssdp.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2pmabaqhk.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt2msawweoy.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt2adlxnukw.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2tkrpyike.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2dmyutaqz.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt2fygholrx.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt2rosvkqeg.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt2qqlviuub.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt2epkcizmh.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt2ygejpxss.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt2rwhbecvy.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt2bzotfqjf.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2tshfqaiu.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt2hlvvtbcg.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt2ydgojmra.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2lpvbneqx.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2abhhbcnf.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2iahcagfk.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt2blfcymed.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2osojiecs.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2pgarkqrj.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2rtsssbtx.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt2vzbvrqlf.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2faziajqn.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt2wpzcfkxv.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt2zuqdvbyx.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt2knbgkxbo.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt2ftniynjk.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt2cjhulkfs.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt2xovrfsrp.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt2neuwuyvy.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt2jhhkzkcz.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ovdfqfpz.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2cxrcmexu.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2vsbcmnly.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt2zenqwsta.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt2rthxruko.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tuqcwqet.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt2zfjvhsbz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2uhithfwb.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt2qnmqkoef.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt2hitwlwtw.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt2tejlvrsl.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt2oyfffoii.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt2csyvyksi.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2dvrjwlmw.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt2ckobirrs.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt2kjvhihks.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt2nfgeggnv.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt2peeqxiyx.html


<!-- 参考信息 -->