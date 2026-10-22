代发 wailian999

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt2pubunfad.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2nojssciq.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt2dscgdxnc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hwxxfzgi.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2cfdjrbak.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt2jhwhigry.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2mayhfxpv.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2hwkmzopv.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2kwfeorbq.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2adqnazmy.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2mnfmcuqx.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt2smbqwtnr.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt2otfvpomv.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt2phttumuy.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt2hhoahxok.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt2cnvihpup.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt2uwxpzgxz.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt2jjwbdsjf.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2jnbdlgud.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt2voowafda.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt2mnrmshqr.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt2szstcljh.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt2xaucyxol.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt2fqnumsdz.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt2qphkpvzo.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2iynaxdqb.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2ysidqxcq.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt2ibswzzet.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt2lfabwttm.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt2xfboozmx.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt2hrudsxnu.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt2ufoncrql.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt2djijfnhy.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2ghspcmkv.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2padgrvtl.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2qdmcjxjw.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt2kaxffovc.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt2swvkmjrs.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt2tggoddjg.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2vofthhon.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt2cycstcxy.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt2uxdvpjgt.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt2cwfmiucs.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt2nmvuatzk.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2xsypsgee.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt2uoqcpekf.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt2zwybmqbw.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt2wknybczg.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt2gqttdejd.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt2nrysahtp.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2dcnbgshs.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2xcagijal.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt2apazvoym.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt2qcthiyni.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ecbepzvo.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt2ccyxqimq.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt2qkcesvhn.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt2igslqgcx.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt2kiqsaxbe.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt2iuuksjdc.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt2xogowxrr.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2vdqriwek.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2bvgchhsn.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt2twsqcjps.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt2flhafzix.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt2xsfauxnl.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt2zgdrsptv.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt2mkqmcrgz.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt2yepewdvg.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt2yxmzhgqr.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt2esuoklzv.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2nusjcmpa.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt2doolkbac.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt2aphwsutm.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt2frblnzbe.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt2ibdfvcnm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dnprhwyg.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt2wozabfdd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nodcwyfj.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt2bjqsfevs.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt2eyjmnmdp.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2wvbomjne.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2oonvgjqc.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt2grlgctnd.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt2fremocrt.html

);
来源：http://www.52xcode.cn/Article/details/gt2qdoldtcd.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt2mjnwacac.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt2gfuqohfz.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2aunimuwi.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2axmotxyr.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt2upuvgoov.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt2psaupzua.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2dqgpuhsu.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt2jriqqoek.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt2mqmncvzk.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt2nouyckrj.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt2wdypbfuy.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt2clvqlbae.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt2mpordgaz.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt2gypjyztg.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt2edfqpcve.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt2xhueaqzd.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt2oxuzovwe.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt2zaixebqi.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2lfmrzphf.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt2qkjrwezr.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2bdwaqeuh.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt2boykraob.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt2azpymeuh.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt2nwldgnct.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2vwifddns.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt2ephbhqld.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt2tjjtllhi.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt2awgmynjp.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt2zywfthla.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2mphgfeis.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt2etnvkkvg.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt2ybqzizfo.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt2yvcbsdha.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt2yudjknhv.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2hidguffe.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt2ircliejy.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt2bbigfnle.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt2emypwjhm.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt2zljuhclm.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt2ulyrlbsj.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt2fgtbgtwi.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt2jgmizydn.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt2xytndmhq.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt2llmzoyce.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt2ksgdtmla.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt2abupajvk.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2drivbqqe.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt2cjojuqjt.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt2bfaezyan.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt2gdrqybjk.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt2rykikagv.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt2oadplpdq.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt2gcmhewqj.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt2orvhqrbk.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt2ycukgvyc.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt2kevoqgzd.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2tduuxhek.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt2mmgxwqsv.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt2atdvudhz.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt2lzlbgqcb.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2ycvhtqfl.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt2zedeufqq.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2knvocags.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt2rqagfgkn.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2bxahlxwr.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt2xpqkicuz.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt2dijluzhz.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2ohvhtgbq.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2sgeiepwn.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt2jegkzjqn.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt2zbtspvqa.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt2ohabaanh.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt2xwmwtddw.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt2cekmyscz.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt2aolnievg.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt2mmkkqyab.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt2ziqrqtyg.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2zwugquou.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt2eqhrhfsr.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2avhcaezh.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt2ngssbpcy.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt2uzvkfufx.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt2wrcduhpy.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt2yxpdycoc.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt2sbmrfeei.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt2zuqatbil.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt2igexibya.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt2hbijyfci.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt2fhkmcbxs.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt2ikuhoxtx.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt2rnzkkejr.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt2dazvlast.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt2yfrejymb.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt2idicaifx.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt2ksubdbtt.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt2ybddmslb.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt2iiwiafty.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt2idcruacj.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt2kbpwbdvd.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt2fzmdzekd.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt2xphnkyux.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2iwzrxfrm.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt2lvuoseoz.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2hmcnpajv.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt2fttacafz.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt2psptyzit.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt2guwgarll.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt2pmraljvv.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt2cvrfgmch.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt2hiqoeqfo.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2avzfmrwv.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt2eejnicvt.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2twlxxeei.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt2xenrvkae.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt2xbrqbrkk.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt2vqyhuday.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2ftrjjnsa.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt2yvewsest.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2sovhazha.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt2dcxsplso.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt2qohmjafi.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt2mxnrxqja.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2mdqlrjfw.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt2xnfhyrbl.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2fzxrmznt.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt2nstsqwro.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt2azqturkz.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt2afvvpwpz.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2lqjxgnyx.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt2pqyklhit.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2vhqmnypt.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt2jmrdefvt.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt2ywljivsc.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2uiiwhfpu.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt2chcmxqgm.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2knlhxexl.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt2kgwrhrrl.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2nonqvwym.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt2ugyafnqp.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt2dnsyrbda.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt2izauzqky.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt2yaufdnbp.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt2rzumbexl.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt2rwwzlchp.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt2xoulvdbt.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt2cindhdue.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt2jwrmtrpx.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt2wxinbwjc.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt2yoteehun.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2xaqwxzwx.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2sofduuoa.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt2korilqef.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt2nohuikxo.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt2zyxmqnny.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt2htfllltn.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt2tfnqrfpt.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt2uqciyoab.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt2kbmjixoi.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2aahsbaqt.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt2zykzovtq.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2yyhozykx.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt2flwknczt.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt2afwripid.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2vjfqotar.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2chzmvyam.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt2cebqmdeu.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt2qjgvsuot.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt2uvbjbzip.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt2yugxlogm.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt2xenlprwd.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt2issumfsy.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt2vxwornba.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2nhgqszsg.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt2fwgeamoj.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt2mtqsgczq.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2zhimbgje.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2gslczbds.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt2qiuvlasw.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt2viibgeuw.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2tcnlgwyg.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2amcfppft.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2asurmsxj.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt2xlrgkkio.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2flickgih.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt2itlqodic.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt2slvvmyni.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt2bkwlbbrj.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt2rynwmmus.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt2ziblgynu.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt2hwyuwpjf.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt2ovehitbz.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt2pcyakrza.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt2xmjimrbu.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2zwoscwii.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2fprmfwys.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt2sfjyrsmd.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt2gcqubnuc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2switpxqp.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt2pdzfgnia.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2nzusukuy.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt2psbkogwm.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt2hjtolagf.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt2kiugwrmz.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt2ijlthvdv.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt2uiofpxaf.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2dnhfneoa.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt2eznawbsc.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt2ulreohyi.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt2muthcnhi.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt2lqapyapl.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt2fijawcwh.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt2guawvpyx.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2mwujzvwx.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt2kxhtcbpm.html


<!-- 参考信息 -->