代发 wailian999

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3lighhfua.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3ewdefeje.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt3uccdyrzv.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt3iuaqciqi.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3wpqoozfb.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt3nfeowllf.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt3ztxyxwfq.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt3vbwlmusz.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt3puysmwjj.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt3rpcmvofr.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt3mnmxfxrm.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt3tyanqxdh.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt3jowleecm.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt3jhucsbvz.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt3zofhxwtl.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt3kpaspuvz.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt3kceqqqfh.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3ehoyhgnv.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3tbxruitv.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt3ectyaadn.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt3wwrjqabm.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt3uulmesur.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt3sfdwphkn.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt3kjcjxcdr.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt3wymqxryw.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3drxiahwd.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3mjhkhkpo.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3aqeqrwev.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3oeosrvcy.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt3lwuxptam.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt3fzrizaox.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt3tqwlmcwf.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt3twzffbjb.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt3nyiwmgok.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt3fvjeamxt.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt3fnsnltgk.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3ysnrykmc.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt3aethekkg.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt3fcbequeh.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt3cwfqxuhd.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt3ttfwbsjq.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt3mpkznawo.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3nnzrczpk.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3fewotbun.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt3atohlvjr.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3bncqeplv.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3vfsslroz.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt3nyfhswvk.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt3qmwebcvr.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3odzxgazy.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt3ppjlycpc.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt3fhygcupu.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt3wiakzraf.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3fbrqswvc.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3ehnbrtzd.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt3csgxavon.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt3kcgjopak.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt3zmhbwxxg.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt3sqyejmea.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt3jhafjvwp.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt3genydcdm.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt3fazkxbnu.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt3huzoyhlt.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3wumjkxwf.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt3hxjtgzrz.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt3bbfxfqzn.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt3mxcocslz.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt3bwfclsse.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ssjjrtlk.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt3lswnvvrn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ycoqujpj.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt3autuifxv.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt3gdqjnnkr.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3tqjzoqty.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3gkelgysx.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt3ovzrjrss.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt3saagdbsb.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3wvqybckq.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt3zwfojqqt.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt3hqkhdeiw.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3jszyiyzo.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3lpgxykho.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt3ikhkbcqx.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt3kzvjmmii.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3jkjlfirb.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt3edlxbtmw.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt3qexiclcl.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt3tiosmdph.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt3edywsgrg.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt3kqzzsihk.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt3kxdarphy.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt3qutcglgr.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt3qrwrmclw.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt3kdrvvxok.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt3dkmhatnl.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt3jqrissae.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3qoljskkv.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt3jifamhfv.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3jyhltsdf.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt3nhyglnvv.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt3cttkwisd.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt3yaerrobr.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt3ccgqjoxv.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt3yybwzsax.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt3yblmlpai.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt3qspsgniq.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt3wlbszkdk.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt3lhamhmix.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt3vswnkcpk.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt3yiralrws.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt3lpwhbqpp.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt3bryvwmsq.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3yvpcafgv.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt3vfmllrfz.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3clwthsdv.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt3sruzimil.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3mrkuwmrd.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt3lqswjuym.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt3dovfyzkz.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt3tyirjwlc.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt3mnvmqcbx.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt3qxjlagnl.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3hjnswprv.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt3oofchotj.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3zzgihxah.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt3ktjebpmz.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt3yhwfkcha.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt3dalakhvr.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt3btinqqel.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt3jhdwlgfj.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt3yyjsukae.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt3kiqjzgoz.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt3tapznyit.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt3hcgesfks.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3pjxtgcnm.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt3yhkxoqwo.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3qjajtnnx.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt3zmyvoktc.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3jtqvvogk.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt3jdodbnrm.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3wmqtnmwy.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt3xbmgsxmm.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3gjdmpnnb.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt3etqsgxep.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt3mmiwnonu.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3yfbiqfag.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3yljusiji.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt3chheyqwx.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt3mclyvhlw.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt3qzpfldau.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt3wlmmwpmg.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt3xxolbdzs.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt3mmzcppfi.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3qryvvevb.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt3suvitbne.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3ktvgztmd.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt3fgectkbu.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3lbqubfub.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt3yxspkicx.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt3fqchebky.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt3vftuxxkh.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt3uxoypozb.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt3qsyrokmc.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt3mflcflvx.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt3vvrleicc.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt3vlnbnfwo.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt3bbmbshch.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt3sewzmveg.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt3ylwqtxqm.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt3vniiubyg.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt3evykwkhm.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt3rdxftrtr.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt3lyokofwt.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt3xghwoxjq.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt3umxllkem.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt3tsurbinl.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt3knijytkm.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt3xmrgwjrt.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt3uienuvzs.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3yflvfwlx.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt3omvpwprc.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3vfovwglt.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt3kjzytufw.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt3hxlskfmn.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt3ipqzunbq.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt3wujuqdqq.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt3ngtxqrxt.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt3camktylf.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3jjaxthpj.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt3ipqumhdh.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3fzaytpzx.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt3tvoytomk.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3kojlkobi.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt3xvblffgg.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3yhreixvc.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt3rccxziid.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3oxwrxkll.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt3bldenwhy.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt3iftoexnp.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt3jcbglsej.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3ukkmlfkd.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt3hkhxipre.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3zwdldotd.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt3brcllyvh.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt3isenwayv.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt3jkwcwqin.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3ugzlkofu.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt3wfyuncoe.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3nuofwzar.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt3zieikszf.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt3sodrpzfv.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3yhhigyhl.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt3zixzlrkh.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3pggldlri.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt3clptsguz.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3amfmbynx.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt3qlncaksr.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt3xdgsvpys.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt3xilfjbcd.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt3evcswiqi.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt3ywwhitxt.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt3fpqriptm.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt3qbknoodn.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt3puoueomb.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt3yughkywb.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt3gyazlgxo.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt3qsrjpqea.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3dhcodyuf.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3zijuavej.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt3miladoxa.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt3avisvgbi.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt3jrtivvgt.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt3uhiowcpf.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt3gkxomcad.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt3couonprq.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt3wxrgnuug.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt3xquzvenz.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt3oedbkstq.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt3jmwljqpw.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt3dohkegmn.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt3rzztxwck.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3znfyhsvd.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3sdrpwnnw.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt3uipdlbqu.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt3kckdvvtc.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt3zllqfqvg.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt3xgvgdftj.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt3dhvjeztr.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3ocwnxvaf.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt3ljjijnma.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3orouiyqr.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt3gxsapckz.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt3hxikynyu.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3fljqetzi.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3ddqlcbrd.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ulegyysu.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt3gwawcyng.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3pacisdfz.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3aupivgam.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3estvfkkl.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt3riyxsbid.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3pshnzaud.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt3herzkvkc.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt3jvxdowhc.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt3netdilfe.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt3rsnadwcj.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt3ursrjvwp.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt3jixocbvr.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt3dbafqjns.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt3qclpqsdk.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt3aaqitvcd.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt3qmnxelvy.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt3fyuwbwjf.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt3hlgbnwkp.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt3fcglczvq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lrgplyru.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt3fkqddsya.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nytflwpe.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt3twgukfag.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt3blzrlklt.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt3mwtesflj.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt3jfqfmtwa.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt3eydypyax.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt3bjxvedfz.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt3xyqtikei.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt3zbmiwntj.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt3ocnugjty.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt3cdvkffou.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt3fqhtknyr.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt3lcuqclbl.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3ezpvogub.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt3sgjhafer.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt3apcjdvie.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt3tfbsrovh.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3ulaaqjiu.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3bxatjxgg.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt3waxjlvkl.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt3jyrsxxkl.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt3eojkhmdu.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt3rludguri.html


<!-- 参考信息 -->