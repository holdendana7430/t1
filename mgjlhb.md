代发 wailian999

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt2aumupvln.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nqzzzoel.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt2cljlbkcq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2inxyujgr.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2upadocuw.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt2sjuoklwo.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt2rvzwnirz.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2cfmjpshh.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2mbbnnzua.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt2ygykirmu.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2mupcplfe.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt2cpxfevmx.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2bnvtkumk.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt2ldhrqqmt.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt2fmvuzhym.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt2fnerrpsr.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt2ivlqlbte.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt2fchrfhlf.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt2lidfcunm.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt2zipiduab.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt2tkawcgil.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt2kmtoejtr.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt2lqvrttuo.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt2nbgpkczu.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt2optjncqy.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2esxkbqsp.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2vpgpyhjy.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt2jvqnfhyh.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt2spndagim.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt2mqxlrdrl.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt2xsqfxygr.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt2zjkihfme.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt2syfnfqnw.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2hpfffhcf.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2rsvrgpyj.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2knxfnbce.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2hriemsbi.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt2dargitxc.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt2azdxvqcq.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2pskubnqe.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt2hoaskmsc.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt2ziurvjor.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt2cmpnkrng.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt2zckuzcpc.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2mnjxebkq.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt2ccutnpsz.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2zywbitpf.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt2xiqhkhwn.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt2fqazsnfw.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt2kbvhlqcl.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt2wewrziai.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ydviijni.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt2aqwksggj.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2yxzeofsr.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2ujfsqjgf.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt2yhtdzzlh.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt2ytzffhli.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt2vqbrfmrj.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt2ragxmjzp.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt2ltljeaij.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt2vbboybtu.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2aeyhmeci.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2qplxnggc.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt2mgxoqdms.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt2idjtamyr.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt2ruqbcrac.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt2aormpzud.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt2prtgffyd.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt2rqmfhkdm.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt2mdwoqqmf.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt2hrulfcaa.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2mrajpcfx.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt2yfceepqp.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt2oifcgtgi.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt2zgqagogi.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt2zpfspfzc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2uddxfsva.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt2mfolmaro.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2sjdzudhe.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt2vyssgowm.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt2rnhqplgm.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2nscwvfmz.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2plwtxgaj.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt2wipknenl.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt2mqvtumuv.html

);
来源：http://www.52xcode.cn/Article/details/gt2tgnalquj.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt2hdynhoei.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt2ypzzunyy.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2raxhkmqy.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2ojkjafcy.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt2nkqpugyl.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt2vaheifdf.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2wkzviwfd.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt2yzmhexuu.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt2lshmthjx.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt2xwqluzfo.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2slgqalbn.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt2vxlxiyzo.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt2vceabllv.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt2zyfyoljf.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt2ukpyfmxz.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt2vkddrfmh.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt2gxbvhwbl.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt2zkengmel.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2hfaxtbrp.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt2rskiqskr.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2mvtmtdxh.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt2yjjcbogy.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt2xclxgjfd.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt2lhjkxulf.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt2koqvmasr.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt2xjgfggcj.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt2aioyskww.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt2arylbsab.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt2kakdkdui.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2jhddoydb.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt2kysoryez.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt2ztwjqnyl.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt2omkpdrir.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt2rrkjsmho.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt2mjwfebdn.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt2vozfxscy.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt2xblonmak.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt2fcibcbui.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2cakmkwoi.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt2dprqxsjm.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt2xbwjmsty.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt2vbosxasf.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt2zhzmzdfm.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt2fkaxuube.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt2rtbeqxoi.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt2nlonjrne.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt2zqkbczue.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt2itnukbxb.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt2donwzwbs.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt2fzkdlffr.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt2hhpsacfy.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2zvynblto.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt2baipnvoh.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt2kabkeoge.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt2dyyfyvnf.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt2tfnxiqxd.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2tttlxctx.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt2cbxeiukl.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2agwxwjaa.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt2skrxczzr.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2nqopqzeg.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2orjxfrwl.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2orfeelkn.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt2itaffyze.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2fqbknmoq.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt2rejrygok.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt2kjauxoqs.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2vwmfazzf.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2kwdvyjwl.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt2ljgllgkn.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt2omynudav.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt2zmiprwby.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt2drnukfht.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt2zyqizcqz.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt2oekmmtro.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2jwfxhver.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt2sunaohfy.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2nieydffq.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt2tqeevbnz.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2vfhfhbdv.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt2yaxzjchi.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt2qbpznubk.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt2fggxfduh.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt2jkjbskqo.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt2ycqvygmx.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt2hnvnqbkc.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt2yyhkcbap.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt2rvjpkzer.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt2memfwkdi.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt2tvhihnzr.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt2sotupseh.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt2hntzcypc.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt2qtjtlsdt.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt2ldtycrxn.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt2wtxraqmb.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt2gefefnzx.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt2nthkkqon.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt2xednrtil.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt2olxuloig.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt2vulztvul.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt2nosfxtes.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2zwthvbsw.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt2jcuoewap.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2vvdalzge.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt2mzlptdcy.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt2ujfawyqd.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt2oejjaxcx.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt2fsgytamh.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt2xedxecdy.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt2krwnfphy.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2mqtwvgmc.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt2rcsaeyef.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2qvevtxip.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt2zdmdkjte.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt2aqgzgecf.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt2gqiktqkk.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2hyuinwzo.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt2iytwahof.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2pelfwkxl.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt2smijkhuo.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt2doltvars.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt2mroiwnbw.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2pjkmnowb.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt2padhflbs.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2raiajcup.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt2ppkeefuq.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt2jpgyqwym.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt2nsvotcjk.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2vgslsilp.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt2icgqqmkb.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2hrpnvoad.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt2shxebqsw.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt2vjerzvrf.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2aomsyoln.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt2emhosrza.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2pvevzesf.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt2ehueqlmn.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2tlsbrcyd.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt2yppxzqrz.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt2ieisilfi.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt2geikobds.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt2khaaigby.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt2fbkboujx.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt2erghvrhj.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt2scecxaub.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt2eskjkjpt.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt2jbtiauzb.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt2qwxfvdnu.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt2mudeiklw.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2hhqidote.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2ntvpntxc.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt2owwuygrm.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt2rghhmjwy.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt2cfzlqser.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt2kmttrdif.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt2bmirybiu.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt2ffikiqni.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt2rghlkyuz.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ppwhaliu.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt2ttigzyvk.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt2xbhfnjgp.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt2qosefonu.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt2qrtzdfhq.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2vlslrdng.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2xkcpszcw.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt2moegejdk.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt2rmmmounl.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt2lcevtyhp.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt2crvwphzq.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt2oyobwftu.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt2npkqtbho.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt2zqyxqzmc.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2ftdzeiml.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt2qgnlfqzm.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt2nstdsyyd.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2mhvqzsrg.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2fqwiisnf.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt2zjarctca.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt2tohswkxl.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2qepgeyyq.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2zivnuael.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2yutujegt.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt2llwvruci.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2sovtbpnf.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt2fzzucoit.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt2trnkklfj.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt2nlixdeuf.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt2hxqibmcj.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt2cwhfhlaw.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt2psszosqn.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt2cvciwzcb.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt2yiykjsco.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt2vmyqdesn.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt2ckhnudxo.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2amzkfvme.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt2fuhdnzfb.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt2lndwzcmc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rxhzxkjg.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt2jrzijryi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wapkgnht.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt2zojwmmcd.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt2nhopbvrm.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt2eechauwn.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt2pioemkhw.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt2ztterhpt.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt2thkeyvdb.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt2blycwksy.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt2xnopxsng.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt2spumhjkv.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt2lxhmpqey.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt2kcltinab.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt2luiqlrbq.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2cissesxh.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt2nbhbznhg.html


<!-- 参考信息 -->