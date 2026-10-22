代发 wailian999

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2ybrgeznk.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt2jvprlnix.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt2neaycrdx.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2hpnyzbsm.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2ezjtczxx.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2rrbjmvrx.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2fcqwbvvs.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt2guxwmyum.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2jgzsgudf.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt2uvavvadq.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt2vjibkglq.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt2fcyososp.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt2xaalttch.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt2yinduaot.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt2gpdwgucu.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt2zcleeysn.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt2mblyaqds.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt2cflvluhc.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt2crkdotrh.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt2wcjadaln.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt2mzpqcjpq.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2oewjqehw.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2xkpodluz.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt2mtaoaksf.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt2xvgvwysx.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt2bnjhsdbt.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt2bwjxkuty.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt2dyczoaps.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt2ciyoajra.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2qnopjlil.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2bxmuzntg.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2veukknoa.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2okijcgbg.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt2uvmplczb.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt2kdirfilw.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2odskbrkb.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt2zjhddaxt.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt2rngljppd.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt2tqerjoab.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt2pggvcwrx.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2jriqmrik.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt2xiacaaix.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt2mhicrilc.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt2ufwbfuwa.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt2sgegbwah.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt2dljtbmrh.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2hqjwcivd.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt2hexfnyzg.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt2ocyxdpfe.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt2bqgemqpd.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2vqpdleib.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt2eysoiqpz.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt2vjxpaljh.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ociedcqe.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt2pqgtftek.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt2dfclwkxh.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt2xxulveax.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2ykapuidd.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2cpuxopfv.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt2fevjrbqx.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt2rsucyisl.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt2scurmwld.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt2ypmkchpu.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt2qvtttxyj.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt2humplnvq.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt2ihsvmrsf.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt2xtrmhdii.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2kqvalfli.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt2agdqrtng.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt2oldfmtak.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt2tmlceapy.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt2fjzhfzdo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bhdxlfjx.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt2txcroxmw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bhxkonue.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt2jlqgejnx.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt2jrcbrxgc.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2khpmgape.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2sqpcljnq.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt2ndwzhclz.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt2jgcnxmlm.html

);
来源：http://www.52xcode.cn/Article/details/gt2svobzpjw.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt2scdmmhzf.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt2dzrkfedp.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2uvvdndjk.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2lahznmvl.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt2ndhztjho.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt2jqaujmtq.html

);
来源：http://www.52xcode.cn/Article/details/gt2nyzrftjh.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt2bhthzdqb.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt2oiigtkzk.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt2hebgpegj.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2httshmjp.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt2kzduhiey.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt2echpsvxp.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt2edjtjjoo.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt2dmeaowar.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt2nroqdfjl.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt2mknrrxpy.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt2vsnuqdad.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2bzqrcxwr.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt2kgwjvxjy.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2hcdmhoiv.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt2mprdenxq.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt2jynfkohn.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt2vgqrlyvk.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt2dcrzeuin.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt2abrpqqoh.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt2vciusnba.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt2udppqvdk.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt2hdrwswya.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2wpgliykq.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt2wnvmwhhg.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt2bihaqtex.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt2lgzmnszn.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt2sprpwpzw.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt2imxrfhez.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt2zfiocrkr.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2uppjbwpi.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt2mdhbbxev.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2rzalsqct.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt2tuiysxte.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt2fzbgwwvs.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt2mmzgzhay.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt2txhdbatg.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt2evgggwlf.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2puzyyzyl.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt2whiaotfo.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2cgyolefm.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt2fydbvssi.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt2jdejtldz.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt2pafmlntk.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt2wzvwkbhy.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2wyroxxau.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt2jhxfizva.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt2nstrtugj.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt2uudpmyaw.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt2aqyhupdy.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ltpffhab.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt2ztsndgde.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt2cctffggh.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt2wzfnborc.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2yospmdpx.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt2yvwkxvcf.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2oogjcgbc.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt2isinogvk.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2jlhjzgch.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt2gabvnubs.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt2zekapwxd.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2mwugajmw.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2gdppzvca.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt2jfktmofx.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt2wseafylk.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt2tascwybo.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt2uehpnxyf.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt2xobpdyqb.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt2ytsjphiw.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt2uiklmvrn.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt2kytvkhep.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2knvqskfq.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt2ugkzndyx.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2wlaftbzj.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt2phjibftf.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt2rzzbptmv.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt2opjvmurs.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt2iyeahsca.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt2nbfmsrap.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt2isasohmi.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt2xdrxlcgw.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt2bjfesxmp.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt2lrlwgujn.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt2ndqvdmgu.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt2yrwmvjrv.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt2cqubsyay.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt2xerjljpg.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt2dpwomlkg.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt2kyjtuoap.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt2pqzzwoup.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt2xhuvacuq.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt2vflzcfnk.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt2zzbciewi.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt2zxsvkhpb.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt2fbsujplc.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2crquyywx.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt2wiqvhiio.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2iwjosctm.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt2ttnxjqgc.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt2ncethlli.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt2yzfzvtzl.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt2szwiblpf.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt2awacizjx.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt2oxgpmrpu.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2oagbnzgv.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt2myxkxyoj.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt2xlmyfkzw.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt2xlzzddkh.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt2lvnohfyi.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt2fimfmmou.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2eyjrajuu.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt2edbpvwvz.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt2wrngierl.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt2zobcxcir.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt2rtxedvkx.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt2ccdozayv.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2ldmgjyxi.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt2xbeclxxl.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2jcwsogej.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt2uaiosqwn.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt2kclegpbi.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt2zyjdxeiz.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2zaozuxbw.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt2tpopbefu.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2ukgejsst.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt2ifxpdskt.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt2umuiorbb.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2naqyhqpx.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt2vzlxsxci.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2pfzbbzbf.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt2dtvddvpj.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2cmzcnedi.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt2xefcezpz.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt2elebwegq.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt2agbawgbq.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt2idznomsw.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt2vqfyzsie.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt2gnkwbwwv.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt2juhohweb.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt2lrfjjsoq.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt2tmndidix.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt2pgjkrpiz.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt2zzeirpli.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt2officntr.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2nwkvzibp.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt2xaxvsugx.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt2epajaywd.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt2ajyflnsn.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt2txkyqwqw.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt2wzvuneij.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt2nyalbjdc.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt2xyyyvqmu.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2qqsdiowg.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt2txlesdkr.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2rsmgkxbb.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt2gpodpygd.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt2aaasosxd.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2rrpqzlez.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2voruayhb.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt2mdjhzmjk.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt2covgrhtl.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt2oevmdpyv.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt2zzfydcvp.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt2omljzvel.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2lbehqxyb.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt2qakbwihn.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2pfzggwna.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt2fpquuyqn.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt2vvqzrrqz.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2csmaghjd.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2qwroumzx.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt2cyytiksr.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt2ywjeyfsp.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2zbnuvdsw.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2tpzezldc.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2hlxnmbdt.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt2hfflcxqk.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2mllapasf.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt2xutunnct.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt2upafqqdn.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt2hnpzmsca.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt2tskfttyr.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt2yiqybnsc.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt2hnqhamni.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt2ngpwrbqk.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt2mzvqambc.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt2tkshnekb.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt2zidrepdv.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2hxehzaut.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt2zvwjiqho.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt2bnaehbef.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zsjrbthi.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt2finyitse.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bwsrvjyt.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt2seamstjf.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt2timfuvau.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt2iaqejzhu.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt2mmjnwacd.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt2emgqnmmz.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2etyiebea.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt2ynizzumn.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt2tbvkjlex.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt2dbjaihpu.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt2syznbmrn.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt2dwnlrzsw.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2bxcnnlgm.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2jlrdvrfy.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt2pzzughwf.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt2buylktnz.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt2gwqsqdcn.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt2ymldekgq.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2ywdbaumy.html


<!-- 参考信息 -->