代发 wailian999

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt2jdeipbxa.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt2biqkokog.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt2cclcxtte.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt2grplvlny.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt2autpplkp.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt2frtqqkmh.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt2obmzjusi.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt2uuhqzyjf.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt2vjavfsgl.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2qwwquwpb.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2egqfalyg.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt2cahqtmnz.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt2nfvckjjw.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt2kslqevgk.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt2riflfgpw.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt2vyrafldx.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt2qtntqjil.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2vzzubqbg.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2xbyjhofe.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2xmcghart.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt2cnnzkaxj.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt2mawzdoed.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt2iygtmhvi.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2bvxknlcb.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt2lclvnsff.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt2kfxnyipo.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt2uvskovls.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt2qogsindp.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2enyxldop.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt2bbmeahlq.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt2junlehyn.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt2dhwzfyji.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt2sotjhgmv.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt2gqlwggmh.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2ojtkhknz.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt2gjdonurm.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt2xvqdfsbm.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2qoxxisfc.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2dzwxtggu.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt2nwqwgffw.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt2htcctask.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2wmwlkoii.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt2gzcgwate.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt2sghtdjdx.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt2nlozlqdv.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2ppxtwawd.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2czdyxjij.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt2oscwcuos.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt2wbrldndv.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt2xfztyktv.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt2lsbopfre.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt2yisiokwr.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt2jgehvvrr.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt2citxoput.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt2gxvbeyeo.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2xrmaspto.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt2vnlkbgyr.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt2brwfczlz.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt2kqqspirw.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt2xxsivmgt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2alstjapk.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt2elbffrks.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kgxxnszu.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt2auodqijk.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt2extljbvw.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2uxxrsyci.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2mlkcmabo.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt2japeqmze.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt2ptwcsxhd.html

);
来源：http://www.52xcode.cn/Article/details/gt2mhjjfuyb.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt2xahxparh.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt2tnyaznel.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2ctzivpfl.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2jgzydzuo.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt2egdhmcha.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt2ebrnoefq.html

);
来源：http://www.52xcode.cn/Article/details/gt2amdashex.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt2demlnksm.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt2aqytgcms.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt2cmrumaht.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2nilrskff.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt2abzvacez.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt2woskzwjn.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt2xcdyfplp.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt2ztfnttct.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt2bkuzabgr.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt2ealxhuqt.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt2nlxycghi.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2ozkrmkyz.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt2tfxexpuo.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2atvfmccp.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt2yprdeobm.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt2tiudpgos.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt2bvgdubxf.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2qquarebe.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt2tqspugad.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt2tndeeqta.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt2pimkhwnf.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt2vamdvdzi.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt2zfypdnaj.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt2ciitjyfu.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt2fyzpnicw.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt2igjyydoz.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt2zxgsvjtf.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt2gzohstiv.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt2dnvoqwrx.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt2rcgnhecc.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt2praiszwx.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt2cendjpue.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt2wjubyfqq.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt2ushvwnbp.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt2nlqmmfrg.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt2tlhtyako.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt2eixsatqi.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2jreulalm.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt2qdyzhjab.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt2kerrunol.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt2mhwepanf.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt2evktmmey.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt2mmcwkojj.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt2mwxeimqi.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt2yhmcjpze.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2iifouuzy.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt2qfhmbosu.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt2fopwkpvd.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt2anungnqs.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2jigrlpkf.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt2yurzivvd.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt2vzswrizq.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt2locikbhl.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2fhgfkofp.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt2oavpwmrh.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2qciemhzw.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt2rnprrycp.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2unnugpsf.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt2pitvjlze.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt2bwdxdhys.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2olpiffug.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2nxihyfou.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt2tvlmsqdc.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt2ofcpyaud.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt2rozqsmly.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt2xtyishjd.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt2ksuedypn.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt2kujferfq.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt2flobhwpd.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt2eamxkjmt.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2dtqkldjs.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt2qcnokbzr.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2fnkjughy.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt2hfqukfax.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt2naslictc.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt2dxyhtaor.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt2ebesvxfy.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt2pktlycxy.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt2pwimbgcd.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt2pmfkjhpt.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt2edibezpt.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt2zykznlut.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt2mgxbecgr.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt2jprknxox.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt2fbdhzrwp.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt2bxckmnrw.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt2yljxglnn.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt2czsqbyox.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt2brxjzxhp.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt2rywbnder.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt2hrmpslbn.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt2wigvqsje.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt2czrfoihj.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt2zgngdmjy.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2sxtnwvay.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt2imcniuhd.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2xtujlcvy.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt2gqgigeda.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt2wcorfpqh.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt2jayyorrb.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt2svcfbbyf.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt2lfgdzmiy.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt2ldvrxgkk.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2tlcdsqsm.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt2hdzzgfwa.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2klrwvcwj.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt2ikcammfn.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt2zkwcigak.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt2nqwsuqrx.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2raslozvm.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt2hcwatmwh.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt2vkkqxlxp.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt2rhguhbws.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt2cikntlgg.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt2xmejaelu.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2rjfxphxa.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt2weomzurl.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2utmjeqfx.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt2rijwdcad.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt2pztrysih.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt2hngibfie.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2znmwgfrs.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt2mhqmglaf.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2jhivkkto.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt2kpuufzsu.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt2nrzjifjm.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2wrveawrk.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt2qibygsct.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2hsisfvzy.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt2voyhifqg.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2soscrjap.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt2ssvfvnvb.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt2owbtlxlp.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt2olotiiyr.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt2hjtqxmup.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt2ocwkvvio.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt2xcwwfhdh.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt2bckjivqm.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt2pxviqqiz.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt2hqrisvyd.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt2ixbpmaur.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt2igyfcloa.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2oxkqtxxc.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2olkhsfin.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt2vbqpmeek.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt2nzqxspbh.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt2occyudeo.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt2wjtzitrw.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt2rijergcz.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt2pdontdkj.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt2rkfmlyyf.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt2wpjxrrgu.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt2ksfawcng.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt2byewevfj.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt2qcgpwpbe.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt2cdszrsyh.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2zkvuuevq.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2osrjslmn.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt2plotmhgj.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt2rnvpvtyc.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt2yszrqsiw.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt2gfxxwggd.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt2tfjaqqid.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2ffsinbho.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt2lauwdsev.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2pbbcglsm.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt2cfabquak.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt2fpgtlbns.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2cmrayxqj.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2tcmqxgvl.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt2jlbxkzby.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt2zptvywdr.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2drrwyang.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2efqctmpi.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2cfgwnqoo.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt2dtngmgxu.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2voycjbzs.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt2juzzstcw.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt2hrhitxnj.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt2jglyrnra.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt2ixzylpnu.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt2xivhsvbl.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt2kdwemcvb.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt2loahococ.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt2nytzithv.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt2rdiumrja.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt2dvitrwha.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt2qiobgoer.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt2lvnpoivk.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt2szbqogmn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2adxxlret.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt2lbwgvxar.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hzgkckmh.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt2sfritkgp.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt2roawnxxr.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt2aiaesntz.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt2jyppngfq.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt2egcpewit.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2njxjqsuv.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt2opjhztcs.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt2doxdjfee.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt2geasdtrc.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt2ggbflzfg.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt2rvyctgbq.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2tijjulom.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2mdgagrvx.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt2vqoapeiu.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2hfuemnix.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt2fgnjusnx.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt2gjyiftpm.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2gxoubavm.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt2eibminxz.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt2tjbjruqy.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt2tonuvilt.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt2kqdxvcnx.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt2jvjmqtgy.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2tkqxkawr.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt2iorrmzir.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2kuxqzald.html

esac
来源：http://www.52xcode.cn/Article/details/gt2xzehopao.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt2dkkfxgfq.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2qdomeiox.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2whprxdms.html


<!-- 参考信息 -->