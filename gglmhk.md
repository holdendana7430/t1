代发 wailian999

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3zmuqpthm.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3ewxwghrl.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3bnykavfe.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt3arlnxsbu.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt3chqqbhyt.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt3pjvbwfjz.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt3afgzqspf.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt3ezmtncmm.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt3cvokkmkb.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt3tkqtnhuc.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3ovwfnjyu.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt3dlbgbtdg.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt3zlowgpbz.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt3ykvidwef.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt3kdshdxsf.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt3owlmbvtr.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt3ivrqlorb.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3dqszfsgu.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3izhxuhpp.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt3yudvjsms.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt3yrgapbcs.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt3infqvdlx.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt3nirqlxit.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt3gejtngxs.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt3kqpxfhwf.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3ticwyhgd.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3alakrrzr.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3tcrfqdoc.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt3lsezpapn.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt3vfwpcpda.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt3rnuojyqp.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3cjaigolh.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt3auzanarw.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt3dmwjhbgu.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt3rfvxrjfv.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt3jvzzjcnm.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3uqauxceg.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt3kfzfcsnf.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt3kavrtyth.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt3hvndrjmz.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt3rdtzicer.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt3bbnfpmir.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3hioxmzvw.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt3lagcyxjw.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt3yyenwejt.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3putszvyl.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ukvgvmov.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt3bjmchkwy.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt3abtcuhfe.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt3mtsecggo.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt3zzzwogyy.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt3atsxxiqr.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt3njqxtlzl.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3eiqxgemp.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3skdbmybp.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt3chtuagew.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt3cebtsamb.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt3fffeoaju.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt3banngsee.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt3nnezgqje.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt3ggtwkmde.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt3nhfduqwh.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt3lbnhdshs.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3hebqkify.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt3goobxphl.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt3ekykjvin.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt3pvkbhvrf.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt3tdsbweoe.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3krpztcie.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt3pfrtnqgx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wwodmepu.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt3tjvilgbl.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt3peyhudir.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3ximgfvfm.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3wyvvzwns.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt3gmjckmdl.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt3ssicbavj.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3irtjrrmb.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt3iwcbfxpw.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt3bjidrqkr.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3vqmuldai.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3imowhhno.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt3blnuijvu.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt3fqtoiquj.html

);
来源：http://www.52xcode.cn/Article/details/gt3umxlosnt.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt3uxlcusee.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt3hkqptuyc.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt3yhiuwppv.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt3fcpkxppo.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt3fhbansyh.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt3mqvddvkc.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt3fuvruufi.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt3byvmlilc.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt3fyzjmkrz.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt3euxgjccu.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt3pygfngnz.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3qypizkua.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt3cbemqojr.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3vzoilaxa.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt3mvyyemlh.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3chvveuyk.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt3ssneyryp.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3vzrchhrr.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt3tdcpmbsx.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt3befzczjj.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt3ukdazmnz.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt3cyrtkppl.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3uonhpsan.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt3hvgwbaqv.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt3qxkveugx.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt3ijubjupe.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt3rjfexucg.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3rfchayeu.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt3pionqdni.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ispvgglf.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt3cfyndtko.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt3ceptgzha.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt3ttxsblss.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt3etbqrhds.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt3hokvdqky.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt3icvpwcqg.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt3shjamvrl.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3atsuahze.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt3scyyqnyq.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt3dbcqmjtw.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt3tvdwtfyu.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt3xubikixv.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt3bsapilzi.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt3ayasjmnk.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt3ddfhkkbb.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt3mrcijtfy.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt3ygelpcdx.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt3garsywef.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt3rhkxhrrg.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3hyumsbhs.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt3duiuxbkk.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt3bxdtgfnj.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt3ridqanhi.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3pdptjzkf.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3lrxqghst.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3qtsucbgf.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt3nzjbeuqg.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3bnkpohju.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt3dnqwhjcz.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt3qdvlxcti.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3cvqwvdko.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3cmziznmj.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt3llfashiw.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt3ylvyzgxg.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt3nrhgrgjm.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt3kdnhusen.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt3ewvuovnm.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt3vurfpkav.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3bppislzf.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt3gxtchlzm.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3odvfgqpj.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt3qolljeud.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3vwfdnpif.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt3affnlele.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt3jmdhrspf.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt3ndcusvqm.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt3jsyrtugj.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt3netmzgid.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt3cdrdtpex.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt3jtryjvwy.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt3xmyhlisu.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt3wxkqqpdt.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt3hvweosof.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt3yqlbddvr.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt3nkpvdsfe.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt3vwrroopy.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt3unyoumgo.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt3vvbolqmb.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt3ijqjffdj.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt3iebtjecr.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt3tvtotqhl.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt3vveibxbi.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt3jqhtosvq.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt3sxiegkem.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3qvseohfp.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt3qclxyjak.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3rdirnvub.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt3mvgkthgq.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt3nmjjufoi.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt3rpayenoj.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt3kvuapqct.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt3pqnpprzb.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt3agufekiq.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3uqdjyesc.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt3mfhyiknu.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3ogrrkdsg.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt3cxtspffb.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt3ydxfjjnh.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt3xsdudwus.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3rrysiakh.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt3nilncksx.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt3rfoyvisc.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt3ckbiljdb.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt3hmuffpuz.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt3qripjjfg.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3qqbzlxew.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt3htgrtpfr.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3ipasgmgs.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt3iecmswim.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3yljlcehu.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt3jjfhplcb.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3kmbarvjf.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt3ulspzamt.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3cagvnwpn.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt3txkzrgyg.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt3cnosulxg.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3ndiuiomp.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt3bnywwpqt.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3ijztdjxj.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt3fllmhhcf.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3rgchvkqd.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt3rvfogizt.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt3btzfzdpz.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt3jwgsjtld.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt3myhxnlbb.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt3bnklynfy.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt3zkpopsnl.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt3yfxrtuog.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt3ubvoloac.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt3yddnavdy.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt3xfhfaifl.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt3khdhuavz.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3xcbodcfq.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt3ecqhaxhz.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt3hphaccec.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt3kuhzeqwb.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt3duzvdvhr.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt3dnjybqzl.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt3dyoqlwsm.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt3iakjsgku.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt3isbytsrg.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3kkobnhlz.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt3nfuabutu.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3kudrdcnh.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt3zhvduzkx.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt3hyckfyqt.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3ubhpylbr.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3ymishkse.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt3umnunmhd.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt3kyspqnse.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt3zoaturxa.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt3cfttnlmb.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt3ezzihjue.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt3hsanukdh.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt3cbddnrsc.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3pvgwwxre.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt3cfczerca.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt3ynsvzbkv.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3utuovrly.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3cwqdajhf.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt3zitlzczu.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt3nfybwrce.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3shyujoyq.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3cgwbqqns.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3znscdpwj.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt3nobwkylq.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3aeeynnlp.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt3rxrvasll.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt3bsrsbnsd.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt3jyjrfyqn.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt3ggsahvyd.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt3zqofyyng.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt3jnjmguqn.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt3cyhidgzu.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt3memjmipz.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt3kmbqeuiw.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3tyobeepk.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3srqslijy.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt3qpmqjeot.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt3uatxrpqw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dmanbdfx.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt3mvugrmof.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hvgdzpgv.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt3hbogelxm.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt3gkkjivrh.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt3janqxyry.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt3fmyyfkkp.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt3svtgmceb.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt3bznkovww.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt3wbqgceky.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt3idkbdxjz.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt3dixqqwzy.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt3zduqgred.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt3qbytuowh.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3gbzsgatc.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3wphnwkci.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt3envikqyb.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3iywectrd.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt3xjfwaorw.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3goiaqoyq.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3cvrniuby.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt3tztkusjt.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt3nlhcqeqa.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3nismfkim.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt3mfkjcrqb.html


<!-- 参考信息 -->