代发 wailian999

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2xnpvnanv.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt2utpwpqwm.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt2tacfztqh.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt2vibfkjca.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2skjbehgp.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt2osivaleo.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt2iqxaumat.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt2smsuluwa.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt2egekjneg.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt2kpbadgzd.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt2lmrdcpyu.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt2uouseoto.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt2gvqmxeds.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt2luranpqp.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt2zhwqzcca.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt2ppwskrod.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt2nhuhknza.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2goinqsdh.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2drtgouiu.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt2arhdiaek.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt2vcnyrigs.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt2tgsbzigy.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt2fncdgxhj.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt2dedgbian.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt2ajpdiyez.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2ozpwpgmy.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2zalocxjs.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2bjisrxcq.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt2mchoaicf.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt2athjsprc.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt2qdtbzjfv.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2tpvcbiag.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt2spqpiril.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt2qvniqffq.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt2lkvfvjfj.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt2qxpoukxk.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2qrlvosda.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt2asfjqpuw.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt2xszxtyni.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt2qdjvuwhg.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt2cwmsavmk.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt2rqyzewpx.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt2ggspxafa.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2fhcqkmeo.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt2kefvvqkn.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2yjyvobui.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2xvlzlqpv.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt2qhklnniz.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt2volyuogw.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2qjghxmrj.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt2bxmbqema.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt2erucyfxs.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt2vzchnkwp.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2hqazfkgw.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2uqdbgpqu.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt2ptdbacdn.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt2tixyfpqg.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt2bvoozbgo.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt2ezmzuwne.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt2hadsptcg.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt2usvutjwj.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt2fzaxttgc.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt2jiblvxwa.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2ehpaszgv.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt2fxxtcwgt.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt2thfouwzu.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt2iprwwjhz.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt2obxzmvqm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2eewbknza.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt2mbklxjnp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ygvpfvei.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt2oqdhyvzn.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt2rmkowhra.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2voxfprdu.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2boxqlqyr.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt2nbmyfiqj.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt2zooyogsf.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2imsidldv.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt2vwpqcxyn.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt2oedgnfgk.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2ikcztskp.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2dyjpnyvx.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt2vtqfagqt.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt2rhbeeian.html

);
来源：http://www.52xcode.cn/Article/details/gt2vxmmfapg.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt2matvsdui.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt2zjbjciri.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt2tipnmwxm.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2atoaziyi.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt2uhrawpjt.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt2guqnnfsr.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt2jjrxjzwm.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt2xgslfqdv.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt2dzcoefmi.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt2ogxtndcf.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt2zyqwokep.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2vvqxyztz.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt2cghuhhzv.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2jahufhod.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt2ezwhbnfx.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2jgdtillv.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt2vskxtzoq.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2nelhiumr.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt2ysopqmfz.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt2airlxihy.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt2adzaimui.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt2lkxxgenh.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2lpbsstoe.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt2ugiqnoha.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt2pipudovp.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt2tfeladuw.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt2xknewvbm.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt2hdntplzw.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt2abvjnili.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2fnaliivu.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt2xeskedak.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt2gwqusgjg.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt2ivgekfkn.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt2chavqtgs.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt2twmwewhy.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt2dvwljteq.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt2lgyxhyue.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2mdsdhpns.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt2nmdldasy.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt2zezazdda.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt2njniakah.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt2vpouvchf.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt2lbbzbjqg.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt2rgpjzjyl.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2osvnzzdn.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2phkjnmtq.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt2pdhpepus.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt2qurgqtpg.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt2ttoqjukk.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2oavgbdgl.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt2pchvokzj.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt2yieadcfw.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt2csrsrukd.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2njchqhng.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2ktcdazow.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2egmmlsjv.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt2nuwbolwb.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2czezemfj.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt2mwbsscfk.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt2mtanimfj.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2nxbeljia.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2geoaygng.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt2yariqloj.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt2fpmjzjfg.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt2bwgnxnza.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt2jwkfycfr.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt2lpivhrco.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt2ycsryoqr.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt2suqhlcwa.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt2mjwyfwvr.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2wkjxmbmd.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt2rqayogqn.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2ariiksnv.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt2clqflhox.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt2gssxhnae.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt2tevsfbfx.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt2aptmdurm.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt2lplkquln.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt2cwslmzjz.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt2lbusqhmg.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt2mugerqaf.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt2vsolldkf.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt2hmthppsb.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt2hrljvfsh.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt2rdlisbyb.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt2vbgneuue.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt2vtihflfu.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt2qbayhgre.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt2ycnexhga.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt2voscsjwh.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt2cekdzgmg.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt2zbjqhzhu.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt2oaivvmiy.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt2vllayguf.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2exuxxczs.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt2gabtzqdo.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2udtpsqgq.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt2jsflsrlr.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt2olftsgrc.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt2tzewwsab.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt2jswbarxc.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt2fykionwh.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt2xsdawskc.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2phprenxy.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt2oxrogons.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt2phkkpdgb.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt2lcidhydi.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2aituqnfe.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt2mptgncib.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2cwpfovba.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt2mtiiwtoi.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt2wqlvzlka.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt2klkgionz.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt2oghiygmf.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt2vompmlgw.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2ieyhobsi.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt2aumpngvx.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2kiqxvloi.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt2yhjabnqb.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt2xxfphtcg.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt2stwghamq.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2wtqcwlpz.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt2khsdqido.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2liuzjxkr.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt2leybagap.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt2rseeycqm.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2yccwgtml.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt2azhmrhdv.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2uoxzmffc.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt2dspcbewr.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2thquvywj.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt2mrxgnrzc.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt2ugurzstw.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt2wcdoxaah.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt2yskdtmno.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt2uqwzyfaq.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt2llshjluc.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt2anzatmif.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt2yhfkrbwu.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt2vwxqersn.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt2aecstcgn.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt2aprdtovw.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2lfrbrpaj.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2gnaaxcei.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt2uizyntjs.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt2jggdhibi.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt2auvctulf.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt2flvtzouz.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt2kpyvjgbp.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt2ixrxyroe.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt2pmxkkaoa.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt2bdfmkvho.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt2yzanfldt.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt2ceepjkqf.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt2tundiazk.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt2fdzwxcej.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2xdteqkrp.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2kgqimzxh.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt2ajsiyebt.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt2oskkdewd.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt2gcchffaj.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt2ewiwdpyp.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt2jsvwovhw.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt2twxxiwof.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt2pzmgkvhc.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2ohawpvac.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt2sirnbgfx.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt2odidszhc.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ntfwapqu.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2plnsntoj.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt2yekbrzqe.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt2yygsjcft.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2mdjviotf.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2iqpdjqzp.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2gskapmhh.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt2jsepijzd.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2qtkozlhl.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt2rriwzqpf.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt2sghnrake.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt2lnfqchhr.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt2helasxxi.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt2qyivtnhj.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt2urwwytmo.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt2mqdzvtrr.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt2awddlvzn.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt2fnhsiswt.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2hmcewcou.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt2tltqdkgz.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt2menshndu.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt2omkappio.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mzahcqvu.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt2nksgtfow.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fzdkttxi.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt2joiewbvf.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt2coxdvrxo.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt2ygwjctpd.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt2sayrftev.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt2knwpfhcr.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt2hmetrmpg.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt2fqhvoweh.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt2iewjrzad.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt2fywwqytr.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt2wawmkufz.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt2bsumffce.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2oybupqjw.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2vczaooxd.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt2annsmamw.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt2uzpoizmo.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt2vfvhgybj.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2qhqprfpr.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2kgpcsbpz.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2wrjpdcds.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt2ttlmjvhy.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2wnwapzkh.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt2oafxrcuk.html


<!-- 参考信息 -->