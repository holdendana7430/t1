代发 wailian999

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3mamteeqt.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3jnpjvujp.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt3kvmdwygs.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt3pjathycu.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt3hisgmahb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xtmmmktk.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt3lqlpuigy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ucjiutuv.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3hdxighnr.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt3ypsklxte.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3reuzzrze.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3lbnzajes.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3rtcxcxkx.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3bvthfnfo.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt3ppaknpft.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt3fzevpmrb.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3qfianmkb.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt3kxxtxhfd.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt3hxjeuxqf.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt3irzqnibr.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt3kvmalxur.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt3ctofitng.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt3zcxctino.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt3jdkkbroj.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt3zftykagc.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt3hynqywrn.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt3axywchlh.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt3bgpdypia.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt3mnasvayv.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3yiddnnzs.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3vdvzdvls.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt3uysxxypa.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt3pldwcvup.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt3zokgphga.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt3vxtpcpbl.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt3bpwtqbjt.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt3yfzewqgj.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3myepuitt.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3yiplqcxv.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3ffbdvtzd.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt3apdnbolf.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt3qkkqmvpc.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt3fsezryce.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3spzjurpg.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt3wcglnnkb.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt3jyfjagdf.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt3yiafjihr.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt3zcbbpycd.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3upcmhjwm.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt3uizgsnrc.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt3vomckggi.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt3xkczinmr.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt3glraggfj.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt3lbdngmwt.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt3mbeopftq.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3iazwchms.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt3oqsxgufw.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt3yicvqnwr.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3hsshctol.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt3bvljlrvp.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt3avrfsrjw.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3qzzrlsec.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt3ckabtelm.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt3wpzicpck.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt3wnnvizic.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3zkmqotze.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3oxyqbdtk.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt3vjcepxsa.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt3jfyvgcul.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt3vcunxqoy.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt3oodadscm.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt3qndzyafp.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt3nudrhjfi.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt3vkximmjc.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt3uziutegs.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3qcrqnvcf.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt3mcvtswwr.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt3erccvrte.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt3tjzzqdlo.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt3ozutyign.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3cdewqweb.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt3vrasmbtx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fashoatu.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt3mmukwuax.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt3thnnpmvs.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3sejtvdue.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3lbaabxpr.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt3kkqybuog.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt3wbsnzzfd.html

);
来源：http://www.52xcode.cn/Article/details/gt3oqospdic.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt3ogmqvnwt.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt3cupsjvhy.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3uuapuqbx.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3uyuuroxr.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt3jubjfepf.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt3tmijxzyl.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3sppyznym.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt3fzohekjl.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt3ykcrigkn.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt3jrqbrbmy.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt3blxuzihk.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt3ebfecgot.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt3zbbykiye.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt3pbysvqrv.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt3ohsrdklb.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt3jyxydvxj.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt3qromxpuo.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt3kcxmtysu.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3ynyseuid.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt3ikbkfeuz.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3ilqpqomq.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt3etxdfbbo.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3ngmflmpt.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt3vvtiltkw.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3whtzmrsg.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt3prfdtvsa.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt3ngboxezb.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt3fpyjgvba.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt3qrvitnvj.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3zurqflvn.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt3jnjjefmy.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt3lrhvfhde.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt3jzwgdyla.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt3mrurrmtu.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3phymgttq.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt3fdvzhvaj.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3lafyducu.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt3cqadafmd.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3lowqcqhy.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt3qacsmrja.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt3vliszrni.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt3ntjpyzxd.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt3utjomvnu.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt3ywczqgov.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt3ymhemodw.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt3dqfqwpdl.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt3kvvksvvw.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt3ipptxizc.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt3rzxohwbh.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt3qiarqkhe.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt3izzjnhph.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt3zveqzbic.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3gnafdazi.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt3fcmnbnld.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt3dxfozgqs.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt3ljkpmgzk.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3grespbft.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt3czmlifcv.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3veirxylu.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt3krxpkoyw.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3yldqhicq.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt3gkofullu.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3jvllfgab.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt3xryxkcae.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3bftaevvk.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt3micolgze.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt3vcmnzksp.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3dixlrwgw.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3apckhyfo.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt3qqyilpgj.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt3prxaunuv.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt3gmsmankz.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt3seskzyqo.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt3guzzrcmv.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt3bskimgyq.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt3lhusycfp.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt3ghtlpiez.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3esmooigk.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt3lpmgyyzg.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3arzpybjl.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt3jsqrsdjk.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt3rwzqfhpm.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt3stcpzpvf.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt3ajucrymc.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt3nhtkrsef.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt3epvrvljh.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt3jacjmbwd.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt3adntktqb.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt3vxpdpbat.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt3qresjcdc.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt3kqjmgtrs.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt3qxniatwb.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt3ldkhphwg.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt3dlsacnbd.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt3rdxoztet.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt3rjrpdppb.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt3ywyupwnx.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt3vfddxcgl.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt3copjgkst.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt3inepvqxa.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt3lssraqea.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3zijrabbn.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt3boimlqvf.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3mzmpizsu.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt3iygwfzuz.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt3erppvsst.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt3hufionil.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt3eyniociq.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt3ihhlokin.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt3ljxvbkqk.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3drlqhljp.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt3zsgwafdl.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3ldxsyyyf.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt3vmkntkov.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3katgquul.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt3vvcxwjuv.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3gccdkxac.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt3zsyvcydh.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3tvubhobx.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt3lcfpgkcm.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt3dcsrxvkf.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt3tydckhyz.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3syxxhocd.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt3btnzyrlz.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3xjggxzav.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt3mtjfnabc.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt3dvmorfmg.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt3tzfwvqbc.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3djxcbawo.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt3gdrgogsc.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3znxjjldt.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt3udxrzvjt.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt3lbjvcsbh.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3tafxhfgm.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt3rngszske.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3timhcyph.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt3ylislswd.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3mqjdqxrp.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt3cjrxodsm.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt3dsweynco.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt3ebbzxytu.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt3njskxmuj.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt3qxlkxqef.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt3wjhxdimj.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt3lkcfjqnx.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt3bnfkfrad.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt3nxjqavpw.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt3qprylhkd.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt3mqqrnlsw.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3ltzfqzhy.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt3ntfeembu.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt3sdljjymm.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt3xnuefefc.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt3tbqwhpow.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt3ofhmdmhz.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt3mhhgsiot.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt3lnofawcc.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt3ahdxexro.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt3uijoswrf.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt3yuiuvoqb.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3wvvwooat.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt3ydjjftas.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt3qeptpmox.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3mqsvdfzy.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3pvaqfbnz.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt3xwfmfojb.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt3ddhjzlbs.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt3pncxpuep.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt3vfarnngv.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt3kmeyvdjx.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3fizipceq.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt3mknbzkxv.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3qyctphiq.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt3zyvaafdj.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt3npwgirrt.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3mudhcjnb.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3yixhvxfv.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt3urwyvnjc.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt3zwybwysz.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3rtjvrwus.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3cdfdbugj.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3wufokalf.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt3jeoqtzup.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3mbascxai.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt3zaytnbel.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt3ntetsmou.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt3qkyevuhf.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt3gyayhwtj.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt3fssdjpoy.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt3hbzfrmdw.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt3jdimyghb.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt3nomnqukd.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt3pqxfkcuu.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3zbqjvtsm.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt3fjxuvuxa.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt3csyhmcgn.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt3fklaswkc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3drtomzcc.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt3bbvuaisq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3imesxjfx.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt3cylgxmeu.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt3oyrygylo.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt3spnoresu.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt3mwkudejq.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt3vrelzcmj.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt3jrlutskg.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt3plqjwcjz.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt3dvsbdypf.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt3mcclbgai.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt3pzdvpayb.html


<!-- 参考信息 -->