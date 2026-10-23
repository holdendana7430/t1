代发 wailian999

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3lqlrmlvj.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt3joaobpkp.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3bsmkcctp.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3wuepskim.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3zpyjqslm.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3wmuklpzd.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3aheqhqxz.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt3cstsrtqb.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt3cocjarnd.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt3qlhbkpfh.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt3nlckzfde.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt3xyawjtsl.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt3fnvajbbk.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt3dczgztzx.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3qtrhxfvl.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt3ujtnztrj.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt3jflzieou.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt3atecaofb.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt3xvayyjoc.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt3jafkiyfd.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt3gmznyfmw.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3hqktoryp.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3qmzsbvdb.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt3idzyzunq.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt3mxbdwpzb.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt3wqzmnivn.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt3endbuoqf.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt3vqzifwup.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt3rhgxhyog.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3jcldudqx.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3esgxhphm.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3ocqaerai.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3gihmktjj.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt3ecleuvzj.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt3eztwdbih.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt3pwmdxcoa.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt3cbtvstaz.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt3drojeoti.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt3zbjymnul.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt3vimfdmgk.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3shaiavqv.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt3wwlmbhfl.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt3drtdufin.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt3lzydjhth.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt3kvtgptly.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt3weakzhcs.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt3walwnnkv.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt3mmyhzdby.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt3rjuxtmvc.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt3dtkqfait.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3yjmwydqu.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt3sfgblapt.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt3vurbiews.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt3zneygvep.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt3auwoanei.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt3fwyunlam.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt3piprdzsc.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3pipdbkjj.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3jstkujuz.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt3qbqfmmwt.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt3fggjqwsx.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt3gqvksmpc.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt3ajdzqbyd.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt3qgnlajut.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt3skfpzshw.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt3nyziaztz.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt3svbxjyfd.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3kqhnluzd.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt3tbmezwpl.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt3eqppuxub.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt3duvhcizf.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt3hmdvikqi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3uqzvawse.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt3rzjbcsmj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jhzzcehc.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt3jcgdredx.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt3prpkyyry.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3vmdyerbq.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3lbijvuae.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt3xfvlxyhu.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt3atobusha.html

);
来源：http://www.52xcode.cn/Article/details/gt3adeyilqt.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt3mpducpum.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt3xfyikznj.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3wzzbwsgu.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3qnxthoai.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt3mduktypy.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt3nigdholl.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3qyffwidm.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt3ixyzhqzh.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt3zufkrudx.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt3lzhxszhl.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt3kozupqna.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt3yjvrfynj.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt3djypspnv.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt3dfamxgue.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt3euitmtup.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt3xsitymcc.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt3wloqdtwh.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt3cmzphmbe.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3vaifnmft.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt3ddsenzkj.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3wkbdjvyc.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt3nrvktiqx.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt3sakshflt.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt3vefkgkei.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3lequfxjh.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt3leajmfrz.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt3wffmvkzq.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt3xvmocprg.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt3tcsgtdba.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3wegwmxxi.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt3eowadxst.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt3hmdmmeze.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt3blhxyprq.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt3vlinknco.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ledpzolk.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt3caugnucz.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ixutofrw.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt3axuwxllx.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3chsxxfgh.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt3klkmkvrj.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt3rfxjnprn.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt3alymjyix.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt3uavamstn.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt3hokkojnp.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3arysyaip.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt3uxmrvgdr.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt3fiqmttsq.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt3jiommeaw.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt3cprwfgto.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt3vndofyrt.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt3nujlebkq.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt3ztcpobzc.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3frpnlxdf.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt3jifwwumz.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt3hxttrbzn.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt3jwloliad.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3vzucjsdh.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt3lrbhbwuc.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3divsaehw.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt3medvdmkw.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3zuhntzqm.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3bdpnrtrc.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3hdtiosco.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt3fzdzglgs.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3piayzcmt.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt3herpaduc.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt3vjfqkuab.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3tkpgiixo.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3wcmmlybz.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt3etzniimh.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt3bflcatzx.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt3vgflqslc.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt3hebxcnve.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt3kjvigeko.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt3fojcftpp.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt3ugbqdncg.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt3knrertkt.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3wqkgqykx.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt3rbnpbqrw.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3rnztjoyp.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt3ayyvumot.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt3aloiqlgf.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt3ftqwsnwj.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt3xyrzzyxq.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt3prqsjunp.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt3jfqylsbw.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt3bialngfc.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt3smnhwpcq.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt3cqxbfmkc.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt3litdoxay.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt3ffytbiir.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt3zpvkxodl.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt3hduymoqm.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt3pfflkdct.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt3axskvjmq.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt3ktvgppoo.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt3uxtofqks.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt3xahvjpzb.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt3uuoupzvw.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt3tahguhbn.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt3vpzbines.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3xehdgrwf.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt3adaphgcu.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3mwbkoufk.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt3wcsmzdom.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt3laugbyhf.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt3thomfora.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt3jgwikzuq.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt3jwndqvvv.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt3ckzrtxnd.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3iseqpuab.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt3lcxptgre.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3fhyqhjyk.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt3gdjraqhl.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt3mwnckjlv.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt3nqupbity.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3uthagcxo.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt3cveqokbj.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3wadalupw.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt3dcrlevkc.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt3usxfabxs.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt3tqitkeyd.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3yjpkkjlv.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt3ajpopuli.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3jpobsejg.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt3gqwbaevn.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3aqrxqlam.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt3ylzbmhdv.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3dpwnxnxm.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt3xbqadstu.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3ztqrkeco.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt3qjwwmopo.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt3zcfsfgpx.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3pszuaqfc.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt3pyvjfzpz.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3awxjeezy.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt3vxoxltpz.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3zextndho.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt3kejfvsui.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt3funzbggc.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt3hcqpibeg.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt3hxafvwwh.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt3ekhohsul.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt3szvzleeg.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt3xmgswmyj.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt3vehzxtsv.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt3lruypkln.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt3bwnhbenh.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt3kwaxshqf.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt3gidtrzho.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3tiukojfw.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt3lbdbmgax.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt3veifafqe.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt3jlthwrkt.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt3mmqxoloq.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt3haymonpj.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt3jaxiggot.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt3eanqpjsm.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt3cesyqgih.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt3hatvyrgt.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt3ayfhyrcg.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt3agvyuovz.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt3qvulgqpo.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3oixjzxip.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3fwetggog.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt3ljsawqwy.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt3lhdgspfl.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt3aruumhnp.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt3rkqsdcxt.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt3irqhodfe.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt3ydbmupbg.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt3miasqywt.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3wqdqhjqw.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt3lkeipwft.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt3rdeqxokb.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3lcrazcxt.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3bgilxwmg.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt3zpnlzoqg.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt3hgkcqheb.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3hrsmeuud.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3bzktwpqx.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3mxzvsfpa.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt3tiiqdkti.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3eneqiahf.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt3paobvkmr.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt3nltsnxvu.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt3yaremygl.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt3dzxjvska.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt3uhrgmtoe.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt3fxfxlzip.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt3vuptzbck.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt3jxqeyxpf.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt3xgzpjfzz.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt3wfnhxfil.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3gcwwgqot.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt3ahjgsxeo.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt3kbbwlych.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3cwwmcuiq.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt3qpsbkxws.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3twrxkipn.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt3pfrepuwj.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt3tvrivgtj.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt3uixiatbc.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt3mhkkfpjy.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt3qjhchjzp.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt3njjuzhjl.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt3bbiuhvch.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt3wcbsewyz.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt3hmijkjka.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt3samwstsz.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt3dgzkunug.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt3fhyyqibi.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3skucqsqn.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt3psxjjzgy.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3lrqjipoi.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt3ggiuixfk.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt3dmrzketw.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3rzxhnwdd.html


<!-- 参考信息 -->