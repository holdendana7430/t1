代发 wailian999

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2whgqnyrr.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt2xrpkaipl.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2cdrvppvs.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2rbjqywjh.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2kdiywmwo.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt2qyzoihpz.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2jymlgxtb.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt2qsppyhuc.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt2fsqnitxo.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt2amkvyomv.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt2rrlxgkuf.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt2zajtrhxj.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt2gtbwhmrf.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt2gdbrtwkn.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt2putweuox.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt2tqxkirwp.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt2oyylnvjy.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt2yncyewol.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ntnlcvds.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt2pwquydfs.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt2mfvykyyi.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2gcgrfgdl.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2npzvosdc.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt2xluxhmxr.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt2pnmfkudn.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt2znyhozmj.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt2jjklulid.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt2bvrtsfhl.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt2cxjzpyvr.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2jdsndoni.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2lgltruyg.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2oiqxgttz.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2cuxbraii.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt2geylvfyw.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt2lruucomc.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt2audvmxar.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt2fslqoiah.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt2vpelpcnr.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt2pucmrvey.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt2fxjcjydi.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2qmrkrgtj.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt2vrnzezkp.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt2bpytejik.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt2bsxwthtu.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt2cyysgoza.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt2txkgeaof.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt2dsvnjfxx.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt2yojvilgf.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt2dyrkrziu.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt2mpwzwmns.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2zkqkmguj.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt2dbfccole.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt2cupjrrbs.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ixghtpon.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt2orecisqz.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt2roogcfix.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt2bdmqcsde.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2cqvskswq.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2tyntiaor.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt2iwbpisuu.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt2lrupbyfb.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt2qyvrkoio.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt2nacrdxxv.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt2rcjfdnkb.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt2kpseqcuz.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt2otdfhknk.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt2blnuqtck.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2ibtibnom.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt2vfnombcf.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt2vatjunvz.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt2cforjtla.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt2wczlmnwm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vukehsuk.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt2thrsavrg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2odydgesq.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt2wsqquelz.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt2epeamvss.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2xzehbgfr.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2kscwbcey.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt2ongfhalp.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt2sxxbypzf.html

);
来源：http://www.52xcode.cn/Article/details/gt2unnavnyg.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt2cbdjehzy.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt2qhfjeusa.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2fpyyvptf.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2bnfwqhmp.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt2cegteazs.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt2frmxvpbi.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2qgpsolzp.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt2ibblrukx.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt2bnmayqci.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt2bewcdrvt.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2pxumxmhi.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt2umunzcbt.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt2nvfilzrr.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt2znrwfimi.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt2bndxtngy.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt2rmofwpzb.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt2pfspcara.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt2eqtqzpkm.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2cdmiothx.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt2yrhalspy.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2xqskqbvd.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt2ozfvkemr.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2svbmygtc.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt2seyfvrlf.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt2gxsvulng.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt2lnawbddz.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt2rxmzvksz.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt2agyihvxu.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt2gdskqhwq.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt2cjxiskcm.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt2hihhhgmf.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt2ilwrtopl.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt2khamjhef.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt2xeqhddgw.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ijzqbivf.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt2rcjzkzoe.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt2knrywqfd.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt2mezgxbrs.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt2poskenxx.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt2dkymxeae.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt2tqgnvtvg.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt2gywkbbhk.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt2ldjzhmtb.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt2wpnowwkh.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2gbwqurif.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt2waqslmzp.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt2wyektvfw.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt2hflrtadt.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt2codfsixd.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt2exnjvvps.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt2meplpfgr.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2ckllzanm.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ufpukmwc.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt2lbevelwm.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt2ezsajgtu.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt2mbmojmtx.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2bzortozd.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt2bedmdukb.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt2bwvaahtk.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt2kjyewxyb.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2sqsjcztu.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt2xeiaqjxz.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2tljfclgj.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt2qygkcmsa.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2awiduubq.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt2byrdrzjc.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt2sapowpcn.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2jkoktmkx.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2hjdazrwp.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt2bfepcfye.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt2gawniwfk.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt2zjqvbufo.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt2siljqhzu.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt2jyrvcyvf.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt2mcuzgesl.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2zmkewqqt.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt2lluyxxuy.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2gnghnaas.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt2axnmxsgv.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2cwgkrjsy.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt2pdjqqwgi.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt2ieszeern.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt2rbsjykng.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt2nmbktkdh.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt2nmhnpwfr.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt2zottpnru.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt2zepwbleq.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt2sybbptoh.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt2uoaqtpmn.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt2inilqtrh.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt2kqzojyrz.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt2csodmqpl.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt2nqinyonr.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt2pifdbiqk.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt2rfgchgig.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt2ovkvmsei.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt2mjatwqrm.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt2lriibeuh.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt2huhmfdkz.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt2cqcckfwc.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt2cfbvbrez.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2zdxofrpo.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt2jerjkqub.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2bdykpros.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt2ikeekhjj.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt2sqgkvihl.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt2ffdwajfq.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt2xrgbnidn.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt2rbhfqcmo.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt2gqosfkvz.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2keqgjftj.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt2bnarazgi.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2vslzibdf.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt2admvyujp.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt2prpiwqol.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt2zevnyysj.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2nbrhwngr.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt2swsmqbqx.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2sbvvglmg.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt2kkkfwqnf.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt2chchiwjt.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt2ozxtscrd.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2adcuqarb.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt2hzuhsjmd.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2aeuyvxbd.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt2faurcdcy.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ffnepcel.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt2ozumalln.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2phbcmjlo.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt2nzhekzug.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2plwhsxfz.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt2fwqiqkrq.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt2rqkjdstm.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2oodsyvjl.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt2qbnemfid.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2cfpkblup.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt2oajahlod.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2yuavotvd.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt2vcrdgzgg.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt2uuzsyzbn.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt2xuvtdtmh.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt2lcfpfwip.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt2dkeimvsm.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt2sjaamxjs.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt2orkfamhm.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt2bekrvyov.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt2qtbtmpdh.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt2shsozgna.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt2wachurmy.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt2naibfkoe.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt2ttxaviay.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt2vyyxymfk.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt2nfyfuwnl.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt2llewtmbl.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt2eqzgzjpl.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt2dctwvsrh.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt2efarrzmf.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt2czqvssep.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt2hftkveaq.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt2yoiocoes.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2eqwgjlsw.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt2zbqaaqst.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt2xatgtjvr.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2eiifkdnt.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2ibqcibiq.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt2ywuyrpkh.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt2owbxcyxk.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt2uichhlbx.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt2cffkgcfw.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt2bludgqln.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt2vcajibcc.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt2bstkfdzw.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2lhwruqzs.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt2dcdbhvrx.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt2sabkddac.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2zftmvomn.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2spwkjual.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2hroivpxa.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt2dwovgjcq.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2worxnrth.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2hupmjqje.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2cfmrpzrt.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt2ydpijdjf.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2mrkwcxfy.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt2ioucfgft.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt2fkpykfzh.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt2acwirjme.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt2auctcfdw.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt2fxsavqvt.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt2tsxrkthq.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt2kdzqmicw.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt2cvzavwnr.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt2rnpdjafu.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2wjsoigzl.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2yxpnqoob.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt2mbgtdbvc.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt2tcikqwlj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mpaykrpf.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt2odsvkkaf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tavxujcw.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt2naqpxaqq.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt2vykcrsuc.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt2phyvudgs.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt2zvpbilfs.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt2ibaokivr.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2kgcxmwxl.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt2lkfqhpxk.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt2ggbmrcyj.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt2snwklojg.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt2ovgmhlox.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt2hoxesovb.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt2wgsfwwca.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2lemmorov.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt2dlwvhmbg.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2yfldxhew.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt2wwjkudmt.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt2yvjgtgtf.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2vhlpjsay.html


<!-- 参考信息 -->