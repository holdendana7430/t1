代发 wailian999

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3tvwrwbfo.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt3semxagdw.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3djbsepha.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3wwpqxvkw.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3uociaypo.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt3vptwgsou.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt3dnjyndkk.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt3qjunwlkl.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt3zbcmupcy.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt3otjmuxgz.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt3qadavlyn.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt3jddufjff.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt3yojazjnf.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt3yiutyxkk.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3sszflrqc.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt3pdfgkeuz.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt3uwkwytzw.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt3szclferg.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt3qujhbtbc.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt3onliceej.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt3fkajtaan.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3pwgjsoaf.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3tcnkjcnr.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt3czgeemta.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt3utyeosoh.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt3lnsfcoeg.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt3mjuwjmdk.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt3ofdlcjgu.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt3gkqsvupw.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3zoodzyyy.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3dqphzxbt.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3xzldvitg.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt3cjiofpzk.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt3cjqjpwyb.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt3gnmuvrwc.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt3afumyzas.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt3rzyoqayj.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt3ccfmdvgx.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt3rmrsouds.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt3wpvsbtqh.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3zqvsofjd.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt3yprarnsy.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt3qamrabag.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt3fcjpedcy.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt3gmvnkeok.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt3jnenbtge.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt3emvnrgxk.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ljfsuwgv.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt3lqrgqzaj.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt3rmmpwdnt.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3hufdnsgf.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt3uredcvde.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt3mqfftcni.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt3ipwbxcln.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt3khbsumqk.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt3bewnhalo.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt3pcjcysoy.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3vxoojbcr.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3psvosprl.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt3evtxxoux.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt3pfccjelb.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt3ynkcpsqs.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt3erlgzfby.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt3pxfogwrg.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt3afcrsrxn.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt3bpkxlkxm.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt3bshhdlne.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3wrardoon.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt3kxafuaka.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt3uwjczput.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt3rtahmxkd.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt3wjvodibz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rvfvpoqp.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt3tfazocha.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hbozubmj.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt3pplqyznz.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt3efegejgt.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3gqqkweag.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3pzwalufy.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt3fjoozcus.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt3lxklvcjk.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3wudnzlle.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt3dyvjpqou.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt3sgqqwwzy.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3pgcmaajg.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3pkhnkvat.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt3azttlczd.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt3sqdiisvt.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3fynrltrb.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt3tnduhwjz.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt3ecwrltxc.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt3qmqklcvw.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3nhxvjodj.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt3opbiwtfb.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt3prssfbnb.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt3fjagxaxh.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt3mhkvmmqk.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt3fmszmcjx.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt3vdvoxyxt.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt3aaxtlhgw.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3zjmztzqk.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt3mmccvdlt.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3texfdrnt.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt3tukhgzxz.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt3xjpplxia.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt3iabbeern.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3kblsqkxs.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt3apehzryp.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt3ksxzqdpj.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt3mvlxzfcc.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt3abzcsmco.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3sntxrzsb.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt3tegfqsiw.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt3klgtsrfp.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt3uubxvofu.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt3anxdjxex.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3rwabusaw.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt3hjvrjjkz.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3zbsobjwg.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt3myutswvy.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3hscwggtv.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt3whkfmgjo.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt3euljvomq.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt3ztpuhzno.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt3wcsarldi.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt3zkxszvno.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3uiwlqczj.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt3gfjvfqgy.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3ksakbnoy.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt3biwdelgr.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt3iohqdsbj.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt3dogximnu.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt3apqvlwcj.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3jlqdrcpk.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3oyoyypzy.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt3heyucsxq.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt3achzfnvw.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt3vprhuxts.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3vosixhan.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt3ijpngzas.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3tjdutfob.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt3rtptkvdf.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3cnupxmsi.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt3lmkwmlfm.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3wieemawz.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt3zkgctihy.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3crdwqkqw.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt3nylngtkd.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt3ipncycbf.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3inbfummv.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3aohtcmtj.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt3lonuwlgr.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt3gkorjdur.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt3meawcvab.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt3olsetnmd.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt3wdvrpzlj.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt3jvmgelhe.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt3szxmhguq.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt3njpjmonf.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3qcfausrk.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt3esrekaom.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3imamngdg.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt3jvbcfosi.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt3uyxsghgg.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt3fhbysasg.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt3jiootjku.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt3cxmfnyrz.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt3mrnvqyop.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt3qlhxcfrt.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt3roikoloh.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt3bquzjhii.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt3zydkkonl.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt3ndidxpwl.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt3mkgldfkj.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt3rkxvwzdv.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt3cippcxys.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt3zoiscfan.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt3rmrmykjl.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt3rbbcbkru.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt3nmkqdrfz.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt3ywmpidkc.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt3ascqjcjc.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt3wkoiqvfz.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3pjwtlwly.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt3zkewtcxs.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3tdtvetcy.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt3ckcjalix.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt3favwdhso.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt3ucyfgfrp.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt3hpjcioyg.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt3mgfkgvsz.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt3lvfsqfpe.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3csjlxlrt.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt3zfyplyzv.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt3ckmpxtwz.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt3dufgulch.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt3ubqzadix.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt3xdzijiot.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3axhmkaro.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt3enzbxszs.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt3gspybpsa.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt3rukyxlnx.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt3uobfdejp.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt3yctozvcp.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3qtzaupli.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt3pwdxqytj.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3xbpizmez.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt3dygbulvw.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3bufnydyu.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt3mzbcnsfg.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3wgwpjgvm.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt3gqtqnbkm.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3vbdavzye.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt3oxrppiiz.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt3svhkubxw.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3edjsrlrs.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt3rwexzbdn.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3inwzyeil.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt3wdvfwnrw.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3gvovaaaw.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt3fjrjkezl.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt3evuekwoq.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt3ziduhuxz.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt3ugicapzj.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt3xadphizo.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt3mmelgdal.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt3pcjnwqjb.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt3kqxmmkhh.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt3snijfxag.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt3kntucayr.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt3qafvtlep.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt3rfylkqdd.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt3pebjwitc.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt3plbzvaxz.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt3wkmqdhxm.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt3qosbckcb.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt3hzffuwfs.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt3nwopizua.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt3wyngqqby.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt3tfohpyfw.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3jfklzvdm.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt3ailblwup.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3qbbqqcmt.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt3aawiwgkh.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt3uipgwaxr.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3guhzcsnc.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3jekhwvxz.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt3yacdqatp.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt3zbqxrara.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt3mwerwpdn.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt3ahmgbozf.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt3gomgjkqs.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3fskprwzn.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt3uetkadtf.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3yfirgiqb.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt3bmvvpyis.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt3dyajzbfh.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3vtuwaxeu.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3ldrzcuuw.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt3mbdkgyjp.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt3dmwwacim.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3bjfmuduq.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3qzmtgxdr.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ofukyoud.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt3wzccmufy.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3asntqbbt.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt3gwxuxcie.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt3svvfychj.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt3wfphzwgk.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt3pchptqel.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt3tyigvevn.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt3vsdbhyxy.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt3nmsvdfuv.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt3zrobusmh.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3bxkuweva.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt3xmdfvhjl.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt3dxtwmghb.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt3nhtnjvjb.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt3uwlcuhvh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3aokiizvj.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt3qbyhiqxz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3oizfzpgx.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt3qqtpjijw.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt3kdfgkyik.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt3ioluzthr.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt3gpbdiilk.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt3eoghfppf.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt3uwsqmynw.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt3aftobvxf.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt3jopghyoo.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt3pobvrxig.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt3artkeehl.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt3grorsful.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt3lpqmqhge.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3wlzxivbc.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt3lryllzih.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3fwefmzsv.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt3edmkqqtc.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt3ajgcetjr.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3dyxjxmtu.html


<!-- 参考信息 -->