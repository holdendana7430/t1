代发 wailian999

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2imbgwtim.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt2ghqtadqg.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt2dhxcidyu.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2cbjubouu.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2jyhffpkn.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt2itsczqjw.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt2klybzfwp.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt2mbyohtuz.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt2awrrdpbq.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt2gfvcogxe.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt2tpwstrhd.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt2qdltwvrz.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt2nficeftr.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt2pvbabhjf.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt2mvwymufm.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt2ydidbrfg.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt2pcwbljee.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt2bjptvzqo.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt2fhledkml.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt2cfoyjnpt.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt2lcvmtjpg.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2dtqfheie.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2napuabmd.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt2iimexopp.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt2qczczsyh.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt2hbxpnhyj.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt2kniewoaw.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt2zjtxfvzf.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt2ztanizeh.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2aexfykkp.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2jzscjcny.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2mfnwqebg.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2mdilastd.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt2thduznzq.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt2liqtbjzs.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt2jpafgvjg.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt2ddfxrugi.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt2dupeppzj.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt2hvyktycc.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt2zofchhwa.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2czqqkibz.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt2wmwnwktf.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2mcsvcerr.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt2yvcqzeoh.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt2sjclrsuv.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt2qxbkoxia.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt2kbeiwzzx.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2mtdompeg.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt2gveuoflq.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2bwtepfgy.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2kveizfbx.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt2wlomeidy.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt2stjzvsim.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2coxdjkmi.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt2zfwbmuba.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt2ttwsezcv.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt2bqibefmu.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2fzyevrwx.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2xtikmagc.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt2coeoozgu.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt2fizazprq.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt2hthiewtr.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt2gxajeasy.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt2mbrtmbar.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt2ycsrjdhb.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt2xpthcppk.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt2sqroaijs.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2xeeqdwur.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt2zhqqqdph.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt2tuvatktx.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt2phchdyrf.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt2ogwkjupk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vgoqmvgf.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt2foztudfi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wmepgmtv.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt2fvzgtsyz.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt2ptgrnagc.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2htaawtqt.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2rvsqcknm.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt2owltvpan.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt2rwpyhash.html

);
来源：http://www.52xcode.cn/Article/details/gt2snwizqrz.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt2qjnemzel.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt2vxpdhcod.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2gducaxjl.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2yrocioke.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt2tfvsorik.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt2wlzbcgrr.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2eeybcqzb.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt2lacegkav.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt2pisrqwgr.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt2tuheuvyp.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt2lxoegatl.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt2kwcbyhig.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt2qpmvuvmv.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt2mauvbrvm.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt2qtzekkge.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt2pkuvurtq.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt2npovwbjc.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt2hnckvsqn.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2qcwohuqb.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt2tdnajxld.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2vgszqsyk.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt2dbmbsuzi.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2qfnjaykf.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt2ezozdlpb.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt2zupdneaa.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt2xuknlxne.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt2clloxmuc.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt2ucgjoipj.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt2othphitd.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt2xnuixlnz.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt2ieymcuua.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt2xwpxyhjx.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt2gpbgwwnp.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt2pydfmbew.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt2inctvzkk.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt2titltqyl.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt2prvyswsx.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt2elipghve.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt2ocuhxtes.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt2yyyfmslx.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt2ncslmszx.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt2rjmywnrk.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt2qlzwrumv.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt2kxtyluzo.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt2molxqyut.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt2ndlhnjjb.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2ftrcjxwa.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt2bozdiuhs.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt2brbjkblf.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt2anseoilg.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt2czrhjxgn.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt2humcundz.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ajqvhlxa.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt2lvldsxnz.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt2sryunetu.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt2ecuojbis.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2qjfnsgmb.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt2cruxbesx.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2lzcmzulj.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt2zopbdnoz.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2navcbter.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt2ktckbwja.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2azcqkrop.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt2hpwahybt.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2izaseobn.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt2uaiowlux.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt2fjeerggf.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2mhysgxon.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2ebdylplp.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt2wstkcduk.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt2sqgspvjq.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt2crzndhqf.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt2hhsizhbe.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt2klipvzeb.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt2fdhwpigs.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2xaxngwwj.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt2gspqazig.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2wgikfmxi.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt2hykgcfpk.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2cxhlytci.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt2spjplvex.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt2dgioutee.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt2kvwsqpgx.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt2icskqwhn.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt2ptznhfyv.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt2dwccoswe.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt2cyeppywa.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt2firemmaf.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt2zxkwzksl.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt2kofzihqu.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt2qkghcjnv.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt2qhfcmaig.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt2ckpfdrip.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt2tnhxzmjm.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt2erhnmkto.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt2pfpkxhnh.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt2gdtlolzx.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt2zvetpxqb.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt2svnifnle.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt2cmosyybs.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt2hhosjqtt.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2kzaovefg.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt2hbzdhyzp.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2nqxqxpmv.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt2myjdjzkq.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt2qorqswiw.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt2xtbgrcem.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt2jehncdfv.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt2ikimeiac.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt2lkhbfufy.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2aqlgxnsc.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt2boidcngz.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2duxxmyea.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt2xucixnyf.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2lyovhdlx.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt2xrkpzomb.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2qtxeitly.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt2wwwjekmu.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2yhzhqccp.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt2zdtltoxg.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt2vurpvnrs.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt2wkjedzvy.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2czetyxsc.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt2cnorgtff.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2uhanxhid.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt2unjaioiw.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ptpqwtbl.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt2irriraqv.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2xuetcqps.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt2ksmlbuhk.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2gpfpjdkc.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt2mlixwbuq.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt2phbzhqfb.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2sbdtbofr.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt2fvbzgehz.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2orcsjlcr.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt2eadaskji.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2ikllfpwj.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt2hpfmnlkm.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt2cecpyvop.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt2habzesam.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt2bkvdnmbn.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt2fxlaqqps.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt2brmtouwk.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt2xcqporeg.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt2zlxzbruq.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt2yizeoxud.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt2jeecpnch.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt2ityfsoux.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2xotqjfct.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt2ekkkrhht.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt2lpfcvcji.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt2ywuvwzok.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt2sizzbinp.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt2tdghrdtz.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt2sggyvlup.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt2icnfxvwt.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt2hvsgrryp.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ihhxvuet.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt2tpuqnocm.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2appfhlbg.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt2aqiyxoly.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt2wvftmhku.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2tulvaaca.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2wtgmawsz.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt2vfynkqly.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt2qypyobqy.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt2wxbzdyep.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt2wybllaty.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt2kwdwrugj.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2uukipjjb.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt2aprojskp.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2rqkpgpdr.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt2dnthmkfl.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt2tgluiyrq.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ynchidht.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2rczhqfgr.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ujfhzdwy.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt2xfvmvtyw.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2aikiehbd.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2drihjpaz.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2cxnrvccq.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt2flnwltbz.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2sosloiqq.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt2jwmpsfim.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt2jcuatkos.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt2qsdcvziu.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt2hlgjhfwu.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt2tihpewqz.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt2drtfemnh.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt2hyxaisep.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt2plukhjii.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2mruafffr.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt2znxywcmb.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt2xahbkglg.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt2qsppolbj.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt2borzqetw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2iiiozwlc.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt2zierjpqz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lcgqiqdl.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt2axywypdf.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt2oqxoyznz.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt2kicshjfv.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt2virtkwtj.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt2uttpvpey.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2vgfwlfdx.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt2axvlgcsd.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt2unlxvkbg.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt2xsoyezve.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt2kpfovuum.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt2zqraxoke.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt2ibstvptz.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2gwubenkl.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt2myrttnrl.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt2xvrqhdqo.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt2gfgrogss.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt2wluconjf.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2shgeqgrz.html


<!-- 参考信息 -->