代发 wailian999

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3hlakbcvb.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt3izuoakyb.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt3eqiuqvnt.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt3ijxhitug.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt3quaddtqb.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt3kbpitvab.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt3sftkzbae.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt3avnjqpwe.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt3salwklhf.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt3yrdskedu.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3agmepple.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt3fyvoyewp.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt3elqvfyhe.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt3htcejxbg.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt3xuompkun.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt3vikvwzyc.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt3gmoaxugz.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3fxnlqxbf.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3ubrwxdkz.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt3mozlwxzb.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt3vmtycxsu.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt3bvybishb.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt3cnvwhvvd.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt3yydxypve.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt3twkpvzpf.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3sqopnfts.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3etqddjbf.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3sddqmpaf.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt3wgwrpshs.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt3whzfomkb.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt3couxlgvz.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3pgxfwfoa.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt3vihbwzft.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt3pphtqiag.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt3piejfysx.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt3okjbrrvw.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3zigovujs.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt3lmtufamw.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt3rkcavers.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt3dcjdpvjh.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt3motsnebx.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt3jcgwrdhr.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt3tqzdzpgv.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ghidmtgm.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt3qduuspmy.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt3oecmdaxr.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3gzosgcut.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt3xzxmhkac.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt3rzcgzqwo.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt3wzhsnpze.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt3gaohnmno.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt3pajbtttx.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt3oxtzjtmq.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3pbncvgrx.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3enwhjkbo.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt3tsjbdffb.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt3mpbvswkp.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt3necfvkat.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt3rjbhcvwn.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt3bpqnlnep.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt3xggnxldp.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt3deueuxuo.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt3oytkedqg.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3loamsbwv.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt3xqrixgsu.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt3hstkhsod.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt3kvlvnklq.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt3eriunctq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3oxnopboo.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt3wtjvyadp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ptexncxp.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt3gzelxxhq.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt3uzlelorb.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3bksewpqm.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3dltepori.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt3cuqbkxzn.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt3bvzxivxr.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3ffcwntbi.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt3xonqrqny.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt3ejsckvqj.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3cdgftgyg.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3amelsxks.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt3owoawkfi.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt3ugddgutu.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3hwbyzddy.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt3otmvgqrp.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt3ktqqddiu.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt3ezsliagh.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt3gcovepip.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt3txzyzqqy.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt3rqvaqhaf.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt3ptcmasci.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt3ozzkhoab.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt3xccybiov.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt3vlrnmtvt.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt3trqlceas.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3qsnasxcz.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt3evabmfna.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3czsuvplr.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt3rkuzjsdm.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3ajkmqyqn.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt3jedslrnp.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt3jbuxdorf.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt3xuevgebt.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt3krcffncx.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt3bzcgrdzo.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt3mqqstsry.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3jsmynizc.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt3ytmmauyw.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt3wzbpkqyp.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt3eqwoyots.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt3zooggwbe.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3swocwsdq.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt3rclaloby.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt3rrvdmdbw.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt3azdvzwaa.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3ndfawbtn.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt3ebhfrokx.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt3dmzlydde.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt3hkfuxvad.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt3hwrbiliu.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt3foxrxhsi.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3jocqhtuv.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt3ervrhtah.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt3elyuvdis.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt3idyxeuow.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt3jnbzzgkp.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt3zakhhjxc.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt3nbhpuktc.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3bedrjxrx.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt3drnfmucy.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt3nepjwavf.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt3mbbukmes.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt3jqrbwmuo.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3vscbuqfc.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt3xckplxkt.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt3zodwkmbc.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt3qumvxdep.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3uywcywaj.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt3njugzzox.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3qvjawhyw.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt3mzrhmgri.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3mmkuaxcg.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt3ybxgysty.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt3euwkatfh.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3wxvormpk.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3mrpfjtab.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt3pmbsvjvr.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt3jrrgefia.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt3aifkpoyq.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt3xedavefx.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt3knpivzkz.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt3oaiyovgc.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3xjdisrnn.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt3ighrtcxs.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3ceshjqdg.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt3gwhccxup.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3vojlzgzz.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt3khejzxrk.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt3lvvihgul.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt3fkmtgagv.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt3kulwshpu.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt3inebrsqi.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt3lngpclau.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt3moqiodpn.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt3khnqjjfu.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt3mjirnstx.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt3ovtxazmi.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt3horkexkt.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt3kmnknvfu.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt3twnjjkli.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt3awuscdfg.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt3ichdrwoj.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt3urkyvbcw.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt3fzpbieeq.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt3dcefboiy.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt3jasykavk.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt3ygnsyolk.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt3wqwacxtz.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3klnlsvqd.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt3suzheavk.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3dewqddgt.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt3nwnytadk.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt3jbpebwrt.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt3rgqmpkoy.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt3fbrgzple.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt3zyisokau.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt3bbjfnfxp.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3vcyejezx.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt3owwbwaar.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt3amehqvlp.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt3kvvwekot.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3xyquhgxi.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt3itediczq.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3wcodmxea.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt3qwrnmiqd.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3cmksyemi.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt3etqyivkc.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt3tqlplvct.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt3qaclbriz.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3pzyfruob.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt3wntuvolp.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3qxxnvkfz.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt3gcftrrrd.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt3uftmfkyu.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt3hqzpinjr.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3tthxlths.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt3irbetjln.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3sdhalziy.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt3jkyrdfux.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt3vbshuzmp.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3fjszffrf.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt3egjsvdnb.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3qaismxzk.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt3nvirokwg.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3zaptqclt.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt3gtaakyro.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt3yfexejeq.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt3pqguenvb.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt3qzkvwztd.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt3jrhevcfu.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt3jupprmkn.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt3joellyop.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt3kzbwduch.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt3yuozaphx.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt3acqwoqlk.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt3pktmlepr.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3lfpnjwiw.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt3uiqivrum.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt3kcpwivxw.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt3subddeyw.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt3eyriuygs.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt3zglzzcuy.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt3jeekfhsj.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt3lvcaqbix.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt3eotxryty.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt3hbzvjvhr.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt3pucybtok.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt3extyubkd.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt3kxogzzin.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt3dhgadcht.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3jfohztpz.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3pepnzgan.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt3lohzluql.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt3myzbrgqb.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt3dgnuwzzq.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt3hyjcrqef.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt3ileljsyl.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3jkzykmru.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt3lbgshfmt.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3dgmlhxut.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt3gmvusklx.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt3eacwzqoq.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3kswuhqim.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3vyfdtuwi.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3veogguub.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt3djetwksl.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3zorcwzvd.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3fuooflrl.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3zkfjyfao.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt3bmbldrso.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ffqlfrol.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt3eanheoqf.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt3mdclmbqc.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt3nzptydeh.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt3idyaqzyc.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt3vjheapqt.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt3lytizgug.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt3puxiwcar.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt3bgnbkcjc.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt3bfhxonos.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3wsrdngqi.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3phmjlnsr.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt3lxrcgnjg.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt3pjocnvzh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lnccfvvl.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt3eeeydbqx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ypyvmhng.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt3wpaizdxh.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt3bspzvdfm.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt3ncsbbeoe.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt3spqpatxh.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt3cmrmxmpn.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt3cwwtphmb.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt3kszdhkco.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt3tlxxxate.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt3azypzipt.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt3wjwqivnq.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt3asdshvkj.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3elqynqyp.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3zeqfpttn.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt3xtlyunow.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3jxmjdsls.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt3qgwidabv.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3qngpuvoe.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3ldkrwyfz.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt3rpdgdibk.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt3jclpduih.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3kzfllphz.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt3ozrvqaqz.html


<!-- 参考信息 -->