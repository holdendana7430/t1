代发 wailian999

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3ggaykpvm.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt3suddtatj.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt3tdfzaati.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt3umqsijzm.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3azwkqgfz.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt3slfhqqey.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt3towgrfjh.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt3tjzvnypf.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt3zktyjust.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt3ophmghiy.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt3jzylmwkw.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt3zyeglmtk.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt3crynbonw.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt3mwbapcxr.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt3zcwuidmt.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt3corjsxou.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt3umnaedgh.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3kvnqxnuc.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3bcfikjjo.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt3ybrbdttx.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt3mavalhyb.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt3zwygvujc.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt3lcxcfnrm.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt3jqzadgxg.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt3tatrzneo.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3gfffxwta.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3noiinxgu.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3okudlica.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt3rwjomntd.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt3axrwclse.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt3ygnomoog.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt3iuhbueat.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt3rnrmuyqs.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt3snlxjgel.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt3lqogxhtg.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt3ualqnbjb.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3gnvysvbg.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt3ncftxxrg.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt3tqkwkeqv.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt3bpjyourh.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt3qyxazyjh.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt3vpwejkze.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt3pfifxogv.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3paarfkrf.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt3tbkgdjvi.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3lfdczazk.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3cvlfzntx.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt3awptgpty.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt3hbajyejs.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt3kpwftyxu.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt3khagkbgc.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt3vfoqyfdy.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt3gomnyjsa.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3fbbeuvva.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3bdktgbnc.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt3rwlcxgmu.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt3cjnjiqmd.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt3tlzhlaed.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt3vhmlsmyx.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt3nrnblgdl.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt3dsuqhpxx.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt3vlucfpyc.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt3nzogurnp.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3htvujasc.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt3hsmpxpmn.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt3rgdbsloe.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt3kdcwjvbg.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt3emulgcxb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3juybtmjp.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt3szyowxtf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qkjdcpbd.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt3xpezhydf.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt3bojycixu.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3dbvibizg.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3fgmjjapr.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt3quoskmfs.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt3wqigdjcd.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3higmcspz.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt3fnrpnysm.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt3owlneqjo.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3szpgzjhn.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3wrutdron.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt3ggxsbotw.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt3cmzfvxap.html

);
来源：http://www.52xcode.cn/Article/details/gt3tqlykfkw.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt3hgbjiozv.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt3oqrasent.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt3amfbfaxx.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt3yrahyllq.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt3uuwiiait.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt3xifailyx.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt3keuqszaq.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt3cfkrukdx.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt3qahhblus.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt3zvhtsifl.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt3zvimblyg.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3pjlptniu.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt3ajamqsqe.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3uzpypyay.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt3ihpkvfgm.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3algpgyfc.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt3myithvvx.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3heoyztfu.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt3nkcslfel.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt3wqkdtgqw.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt3bitahhbl.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt3jmgakvri.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt3fjxyxltt.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt3vmshnrdy.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt3cqkmsyzu.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt3bkpgisvg.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt3ancndlda.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt3stfbosex.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt3fkftvhvs.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt3mtxznazf.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt3jqtneqpp.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3blpfnvyy.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt3itwfedmc.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt3bbmcqxhj.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt3pxsqselk.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt3iotcbtip.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt3mfxeuzpq.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3zwzlqnrf.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt3mvjbvaet.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt3mwungxsd.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt3vxjosgjk.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt3dopobudm.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt3zpffyklq.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt3mjqqepyw.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt3nvmggeys.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3xkbrsqrn.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt3bpygyigz.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt3wvybjvpa.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt3lxsbjsbf.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ztqsmxhl.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt3jpyvrosn.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt3yiawuxdy.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt3txpngevc.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3zdjnnewx.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3ovtkeuwq.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3rhwwvtbj.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt3tcmtjzil.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3sbyawmvc.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt3hkbjfbpb.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt3kfxlogeo.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3qmhajwcj.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3nqgmoaop.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt3qyqoaufd.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt3xtmttxic.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt3tuaqvdzp.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt3omjlhvgd.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt3wklifilv.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt3dtrcovnx.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt3vnffavuh.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt3aigyejbf.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3sjwzbfpx.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt3bpwqiceg.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3slimubtj.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt3kprxwgxt.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt3bemqpghr.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt3qxmutzas.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt3itgyakee.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt3imezwxar.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt3abozhnjw.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt3azswymlc.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt3zthagjbn.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt3rebwxcjd.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt3exwuqhbz.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt3cfxebyib.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt3tlhhazox.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt3xegjcwnf.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt3brrvotax.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt3xxzijtur.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt3rhxjijwf.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt3hsxnsvvg.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt3modugsmu.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt3asfdimhj.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt3dssbgbvw.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt3vqhnypbl.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3ucteylay.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt3vxqyffnd.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3xnjridem.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt3yychqptl.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt3iwulfoqn.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt3morepaxi.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt3ncdklpap.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt3fvzrrdig.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt3vclzygsn.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3vfuvvdhs.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt3mltqaxkr.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt3jubnnxyb.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt3xlseyaai.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt3inoxtyyk.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt3belhucvw.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3lgmxtfkq.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt3dspkuvuw.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3tutmtqya.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt3wqdwypzz.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt3wzlnjthd.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt3gadbofzu.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3nbkcypdw.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt3cteglwti.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3tezneywq.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt3coephnyg.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ykvooldl.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt3qaosylcd.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3mllbmysp.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt3owfsocud.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3fpamymdt.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt3cmjzrvqn.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt3ugrgefvk.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3nwbewhdl.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt3owexlkfc.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3iehjxvgf.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt3yrsfivqk.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3ztqyblvg.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt3zntuwsef.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt3lspsngyv.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt3prnsoyte.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt3keavnogv.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt3cgwtcnbs.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt3vqonvplp.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt3uqqpfply.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt3npnaxkkh.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt3rfqjxmrb.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt3gowgstmv.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt3zogyeznr.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3svrsqzbd.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3vcrydqkj.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt3ryorpgud.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt3dujtefto.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt3vpffbfte.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt3qurtqwjm.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt3xfnwxbur.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt3msakofmr.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt3iujjuarw.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3gsqcjryt.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt3wvnilrzw.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3sntinwfp.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt3adaxtewr.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt3qhdegljo.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3uuomkbgo.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3qrtfpuaw.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt3oylqjzmi.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt3tcowdhuu.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt3zbwgxajy.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt3pdprdfmi.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt3lztugrks.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3icjpqdfk.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt3nszqahpf.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3vuxcragv.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt3qjbkjifm.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt3thiaogun.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ldryfvqx.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3eoskwnxb.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3affiwgmo.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt3cwlokjhk.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3xitljjuw.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3mojrgurw.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ciqhtcjg.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt3pdpxdtkt.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3xbwkvfpf.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt3cprafkop.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt3omythasl.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt3vbdstmlj.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt3bysxamgj.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt3zxglyhzb.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt3ozrngpcj.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt3zlbewlqe.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt3bckbxnag.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt3lralcdoj.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt3xveiovwb.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt3ysazjiio.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt3xjgkgkaf.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt3diirijcc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lrxhjutc.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt3ivhrplzv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fwhjfspw.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt3vmgxyngf.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt3ifefbvoo.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt3txuxubtx.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt3nyqhhvnf.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt3fftxqhos.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt3evkguaby.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt3jsblfoti.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt3xjoccbhe.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt3ropcjuge.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt3yosgvscc.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt3bugcjrdw.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3lnugjriv.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3wdrzefrt.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt3nbmxozhw.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3vywlgehc.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt3albrdanw.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt3inczgott.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3nxvtvckf.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3ncakxafo.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt3ikuznvur.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt3utfvwaco.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt3xqgpdhbz.html


<!-- 参考信息 -->