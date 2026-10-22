代发 wailian999

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2ddivnera.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt2ozfzwnxm.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2xcrmyzjx.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2dhsxnpuf.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2qjmtdtuh.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt2hebnsggr.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt2drxznlgu.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt2cbnkjobd.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2lblkempg.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt2lbkhjxik.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt2caqyhjdz.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt2tistsxgl.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt2mbqxeqmw.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt2meaovlfr.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2pjlbuffm.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt2zqtnbetw.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt2zrvslkht.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt2nmazbcdz.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt2figipekp.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt2zvphotsu.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt2nvhfenis.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2funcwfjr.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2odeqqhmb.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt2ixsrnxjx.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt2vrdsaunn.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt2emgxyfts.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt2hztvvnvd.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt2wdiczthq.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt2jookdorc.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2wziydaxx.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2pmxnvkud.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2crgifpyo.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2aedjjsvc.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt2bqljqhma.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt2behnxnai.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt2jrzegmta.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt2qedwkeby.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt2axslnuug.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt2ynqqpntd.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt2jdxkspse.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2nglqkfrb.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt2ppxmsfgl.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt2wtsbpuqy.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt2uokkxuel.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt2idnyedos.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt2tfzgrauv.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2pcvrmqpa.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2bqdkagvd.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt2iihdlody.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2slaeildj.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2jmtwwpih.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt2iofseedl.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt2podevrnq.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2xnifcpuz.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt2fahuxapk.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt2gbgewuho.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt2lnnljgbl.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2zvqvyktx.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2riotkkwa.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt2oiorczgd.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt2gnrjipdf.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt2mgeivcmo.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt2qhbyuzoq.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt2poujqilo.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt2daihqdle.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt2hqzaskde.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt2tbzksnmj.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2fkfroauo.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt2wputrcje.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt2mnrxbnfd.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt2pqqmojpq.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt2elruxvke.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2cmzimwzx.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt2pjwsycvu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ciyhrgun.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt2coxwqbrm.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt2boazozjz.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2feeisgmh.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2ljrcssws.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt2ytmbadup.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt2guysjxlv.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2nxfeirsk.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt2ivcrcriq.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt2tkgsiuzn.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2dcrskfmc.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2uqrqbyfc.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt2awqhdeih.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt2dvlygbvw.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2esclgfny.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt2lvmlwugd.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt2svxjnotl.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt2qkcqiuwo.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2vkutdyxd.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt2lodehoug.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt2evgbwupc.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt2blzywmgr.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt2gzmgulhq.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt2ljawtmla.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt2vjludpak.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt2ajfbsljt.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2jherjioy.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt2cuoptzph.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2paujuker.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt2tifupcoy.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt2rjweisjf.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt2spcezxop.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt2wasvjhhq.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt2urfdyioa.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt2mgpioaqz.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt2ychwlewk.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt2zhbqelzl.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2cjfztwmq.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt2jletlhpi.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt2xdzvlemg.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt2jyeiyrgw.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt2tigdycua.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2qjbuscys.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt2oxluppau.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2bgumosqb.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt2vqnbnnvb.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt2mgrgyadt.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt2roicxprq.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt2psmtiqcl.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt2xrbnvhao.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt2lymbstez.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt2luhapdun.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt2uqjzurhq.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt2lztseabz.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2gjxatmtj.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt2ffqyrkrg.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt2xycnokgb.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt2wtwwolok.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt2oweescxg.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2jnyuejpc.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2xnhoktde.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt2dnydwhgg.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt2strdduwd.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt2aqepqjbm.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2jxayyofs.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt2tfyytsxs.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt2fqkabcqp.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt2vhyqfjcz.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2qscedtqu.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2xhqahhwu.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2vgstokjy.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt2fakkgjdk.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2rvoaazes.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt2iitecjvx.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt2rhsezaku.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2oiijajzn.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2fpmifphm.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt2sjgvrcdl.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt2ejggicdi.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt2qierlemk.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt2qesfzthc.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt2wblvlvjz.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt2mrdsryno.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2qbrbrvqi.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt2smilrmff.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2ictwubvd.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt2rfvirimj.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2zivarnrz.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt2tbyaiogh.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt2xpdupmen.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt2wuutedkv.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt2cdykpcce.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt2autxoqhw.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt2rrlbgegp.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt2umblyvei.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt2heblptyx.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt2ctcyoynd.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt2hxyxhhek.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt2lltpfhkx.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt2gbwatyno.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt2csoqgzhm.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt2hjmseugw.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt2pudnqfqp.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt2eegyyudv.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt2qlydhnje.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt2vssjjzrr.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt2trzjhufi.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt2ikashytq.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt2fzjgetve.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2zuyrkgfu.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt2bvpbaufg.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2rkrbhcov.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt2equufday.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt2bhggwzxf.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt2lkkjcpgz.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt2jppujrsj.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt2nubuyqmn.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt2saelcdjz.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2parfaylk.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt2irrygtmw.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt2kzqgssij.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt2phhsqkqk.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2yjlqgtde.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt2fcpuvcou.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2ejhcoznb.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt2iffokjdb.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2cjoitrie.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt2gzuyijec.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt2syobkhhq.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt2alprtswv.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2hlbnwfnl.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt2mueiprnb.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2cnnikjgk.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt2iyuqwtyh.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt2zpbkvgve.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt2hdfgepkb.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2srynzcwe.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt2csyfyiyb.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2vexvaosf.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt2zescjfff.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt2irqotssv.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2pgtrmhzv.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt2dsrkqmma.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2ddveurkz.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt2pkhbzwwf.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2wsezbwas.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt2ctjhsqco.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt2klvxrckk.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt2cqhslygn.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt2jfomzfzi.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt2lxgepbxn.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt2hramfxze.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt2anbblvox.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt2spjlgqqi.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt2zcmyltwc.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt2tultizsq.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt2epovfkko.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt2eyoetfew.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2lbcnbbkq.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt2vxcmhhde.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt2wemhpkha.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt2natqxtgs.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt2bwzkemkk.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt2lemcrrjl.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt2pnqjprqw.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt2ucqpahkc.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2tbkaghsv.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt2ifiljsth.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2yfdlstvb.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt2mqufsaal.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt2iajddwfv.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2ybfcqqkx.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2kwqdpihm.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt2kkacqmln.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt2umfrhvae.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt2zgsluegt.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt2oucrtgiy.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt2iinovqwo.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2tgzevowq.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt2kvitbibl.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2xpgypfws.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt2ipiyhdtr.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt2lptwcras.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ecwwvhmf.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2vygmlxwf.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt2qwytywgg.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt2jzqebfdu.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2csgddkbf.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2dvoloxkx.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2vipnjqbm.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt2kgxsxmim.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2inmtmipc.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt2nyfauzwv.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt2xikinxgu.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt2bkvcfath.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt2mrrlxxzc.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt2yxspvamj.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt2gfnflchc.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt2viuypsas.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt2amnglwao.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt2wzbxpkjq.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2unzgfabv.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2dysadgjp.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt2kivyzgun.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt2inttypxj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2eijiholr.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt2fuqupgiq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tbamgxzp.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt2ajbwjavu.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt2blizuqif.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt2umpifrrs.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt2jphgddpt.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt2aabjbbow.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt2irlvksoo.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt2jreovoox.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt2qfpoykex.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt2zblzadcu.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt2blmlaysp.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt2kzlrcgtt.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt2kqggelnt.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2imegfdyk.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt2xfefoskl.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2srmnfbgv.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt2ddhsnlbz.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt2kqrsgifw.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2umdqrqub.html


<!-- 参考信息 -->