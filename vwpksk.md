代发 wailian999

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2qwheggtk.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt2sfszasky.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt2nqsfnhfr.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt2ttehxwky.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt2fxxuepak.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dzeaptdl.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt2urcmguqo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2blrlvzec.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2eezmvjej.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt2bbqbpckl.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2hmuppnqj.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2ypohlkkh.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2bjsfilem.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2ckofljwm.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2xubmmbpz.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt2bagxnivy.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2szrzikbo.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt2glxugnkm.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt2qxkerzzi.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt2qghzmooq.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt2zvmjhjgl.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt2iufnblmj.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt2klghkxqq.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt2eggyzpnp.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt2qsejumzv.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt2pwwovxpf.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt2nfymgwau.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt2yxyiwbwv.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt2dufiwwoo.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2onrmnqxx.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2uyiygvih.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt2cmcckhky.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt2zwqupfgq.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt2xfupqxim.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt2icgjpbpo.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt2xjivykwi.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt2naememmw.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2xnssfzka.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2tlrkmuql.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2sysfpppd.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2gskduonk.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt2arbqrzwq.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt2hrydbust.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt2gkcxuprm.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt2csihtfef.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt2tqbaybxf.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt2cyjomciy.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt2aabotvnf.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2fazoskev.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt2npiodhfh.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt2getllwok.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt2mayskyjt.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt2wekeqocd.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt2pohjncvj.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt2ianavtjb.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt2jjpnnkvi.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt2aomneuqy.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt2ngtexwzo.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2exvynflp.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt2difbvpcq.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt2jaoorkqf.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt2lpyalwra.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt2qajbszru.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt2sszsasrh.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt2umbfzwll.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2jfqiqrbn.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2ndhwzenn.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt2zlohxfdm.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt2ymrxaord.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt2xmeugudk.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt2sdykvapa.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt2lzsybfes.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt2jrsvowsm.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt2cdeybvbr.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt2yfijznuk.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2meonnwsz.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt2bcxxyudv.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt2yhaeejkq.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt2ebpyvuma.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt2djwjtvvm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2cuawtujs.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt2tsdecuuc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ttelvipe.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt2bttnrhxl.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt2zmyjftbw.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2pzdebdzw.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2vhuaqoud.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt2bxvbjfrv.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt2bpdpshvt.html

);
来源：http://www.52xcode.cn/Article/details/gt2uwwkcmwg.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt2fxjicchv.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt2gvddnnax.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2uenyhhab.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2kqjardpp.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt2cwhexjil.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt2eiwqsfug.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2rxixvzik.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt2bfojtibr.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt2zwlhqvlu.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt2gpxmtvdu.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt2bwhiqjqd.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt2fpedzxiy.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt2gfadjsdo.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt2ikapwnsx.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt2gryahrdh.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt2uaoashpt.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt2uwwlyzke.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt2xsxrcamd.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2gwjbacmx.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt2knvybeth.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2hagxvbrn.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt2wvhxqptn.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2sbbtjpel.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt2sufjodzj.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2zttkcftp.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt2nbhvprfz.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt2gmdvmyon.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt2cqxytcoq.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt2kyjnakbo.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2xdbccdvz.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt2xjuqahck.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt2viewxlty.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt2nquakiyc.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt2duwnebru.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ddkyvruj.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt2fhjacyms.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2foordswt.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt2gvqvxbah.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2lscqwkng.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt2kbfmfqgf.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt2rdwfqezy.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt2rrroobol.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt2xwkitens.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt2vwqtfths.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt2zovakvfz.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt2zcrydnkq.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt2hdsfipgz.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt2pwjogpus.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt2hfftdhyh.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt2zeejjztp.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt2zvslzouv.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt2pvyturfr.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2cepvsxup.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt2zbndsjgs.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt2rafimyht.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt2anayduox.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2gsyjfpuo.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt2wzpvqnay.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ikqaulea.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt2uaeelvqb.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2hiyboxia.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt2kigmzqjd.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2xflrljgp.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt2rqxgxuuk.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2whepblbd.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt2ucdhxblq.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt2ahrwikwr.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2zzrokyvu.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2ydelmxgh.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt2vlicmnlj.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt2ydaqcadt.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt2cnqaugbl.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt2oqjtgtbo.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt2nfrozbol.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt2qhmatndn.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2gtznihnh.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt2uvujrwcp.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2juyfodsz.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt2pstdnxjl.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2xbxjxszm.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt2nygesevx.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt2quopmocy.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt2clplcwus.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt2ultlpyku.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt2avdduvie.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt2jtfkprhh.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt2xxqfdhid.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt2utvnymnu.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt2lnjofkfe.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt2spscgdvj.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt2qrtluxur.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt2jwfcqpjq.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt2cqmhhkrm.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt2otdcymjd.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt2jhmfdhbm.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt2aghralwn.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt2qlcoszjv.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt2fgbhhinx.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt2tixwqyww.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt2arhlsgbs.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt2kbzvcifu.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2pvxygtda.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt2ebowwlez.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2cuyrceln.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt2xmjalcpx.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt2tgaochnf.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt2inszypdm.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt2npomzzcj.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt2cixkahno.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt2ndhebsig.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2sgwmabwi.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt2svsvvsin.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt2apvtprmm.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt2ioeaghrp.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2oknkrqlx.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt2rphqjucw.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2scserjfh.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt2omxnujce.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt2czalarmi.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt2gzhytmjb.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt2efnggabk.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt2azridwka.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2abjcrjih.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt2sunfaqwz.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2auabedsm.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt2eyyzfuhy.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2xsojtnvm.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt2hzymvvrw.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2tnepshjq.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt2csjygoxu.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2cnkzzeiy.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt2lnhfmsgu.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt2slosysbb.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2pgvlouem.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt2wypibvmz.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2ydurqhvh.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt2lrqvmnut.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2fdvocedu.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt2fzfceige.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt2iisyndcr.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt2qjkzqeps.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt2djdagpyg.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt2lytfkhvi.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt2zlqrawov.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt2pefyixum.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt2qzofwoup.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt2malwvhkd.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt2xwfvsvio.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt2jnkcmvsv.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2hckilxar.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt2sdvwwucw.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt2otldczmg.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt2kamgjdlp.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt2pjrmcsxx.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt2cejzfdnv.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt2gdjdnzdq.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt2uondppoy.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt2vyjohyre.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2cwbuxnht.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt2zqtlfpxr.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2cpogchpp.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt2shvcintt.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt2jxmwfahz.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2xkzirdem.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2dntastyd.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt2dyujszla.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt2ondcnidl.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt2mkncutru.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt2ujbczfbo.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt2ckrucurr.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2eltowust.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt2clrkonsq.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2nihcwvdm.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt2umyllljx.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt2hvdokkzu.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2exnlsstv.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2tmbynnbf.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt2qtegbwrv.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt2ikbenbea.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2yapwnlir.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2pfhhqiui.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2symonrqs.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt2agivsgez.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2bzibwpns.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt2vkpdkvlg.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt2otmtqnyp.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt2eekemsvs.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt2swlgkrul.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt2uqvxtkgw.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt2uhjnbqaa.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt2sgtdzcnp.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt2yskimpmq.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2clibqjnq.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt2kfgpiigu.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2ekwzrlli.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt2xeuumaao.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt2urmqrxpj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2exugpqso.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt2uyzxbmnw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xankbfui.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt2nwgiqazg.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt2acrxpjkj.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt2xsmemevq.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt2wfbfddpj.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt2lowdhhjy.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2uwcfnhkc.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt2ylwbpttk.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt2dtmomtvu.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt2fwzbqttz.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt2qsziuund.html


<!-- 参考信息 -->