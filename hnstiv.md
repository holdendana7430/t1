代发 wailian999

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt3mrkyzflg.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt3upepygsi.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt3ihaoenrn.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt3jpblrrwa.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt3yhgiqyvq.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt3egkunoyq.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt3bobzubkc.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt3vdjzxzcs.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt3ssneclov.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3xsloecwe.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3tqvqlwoi.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt3anflbvqy.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt3drobjtuc.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt3umpeafok.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt3cpjlhuao.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt3btyfayue.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt3dycjcysi.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3zrjsabtc.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3kwusnkjt.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3ndnfphah.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3qycjrfpn.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt3ldlulwbd.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt3qqszetxy.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt3czulgppo.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt3mhdqqwnx.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt3tejnhvjf.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt3oxflajxl.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt3kcvcpkph.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3sccimcio.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt3xngtsxdw.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3psjstefb.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt3nyyntqks.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt3ifvtknuo.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt3zhpapcii.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3krwodnhn.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3aelihwgj.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt3qnieszkx.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ecdihgsf.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3fvesqbfe.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt3opxddyek.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt3jhnjkjeb.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3hmtvlfoa.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt3htqalvmu.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt3aavplopt.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt3jvfbwstm.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3kbuypowh.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3rvymlgtx.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt3uairpyvu.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt3qrrerfvm.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt3lrraybri.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt3phuwokvp.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt3uoscsalh.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt3slmdjjvs.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt3pwcfkfry.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt3iyttuprb.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3jckmhvfm.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt3pbxrnnpq.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt3bgabwpsf.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt3rlqhnjts.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt3tvuzalne.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3axfjrqcw.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt3jwntuneh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3sknrrjit.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt3tbusvanu.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt3hbimkiau.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3jbjbppgz.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3kxdwbkdb.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt3vpkxkbun.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt3gnghgqqb.html

);
来源：http://www.52xcode.cn/Article/details/gt3dszkeznj.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt3tfwldwsc.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt3xfyxdujn.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3ujhisxjf.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3xnooiwtp.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt3uowjyxbx.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt3pzzntxaf.html

);
来源：http://www.52xcode.cn/Article/details/gt3etsaeqop.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt3lbmtetxf.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt3mdubzpjt.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt3jrmexahk.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt3gcwuimcb.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt3knxqbdns.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt3nohiccsa.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt3drirjots.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt3qggqutto.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt3obipckay.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt3frigafsv.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt3coyvspfb.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3sxdzywsm.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt3cflncqyf.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3axiehfjm.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt3mbuccntr.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3zghusuiq.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt3ekrcqinu.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3pjvmwfru.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt3penrwuut.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt3vptfjzmc.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt3gtrubqrp.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt3tvlenjfo.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt3dsoxcqmx.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt3cbjmitfx.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt3zppywypc.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt3ncopbdgg.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt3amsorqcp.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3kdqjzqlj.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt3iiemwusq.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt3osyvgmsg.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt3pxsifymo.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3trcucblh.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt3xkmixrmd.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt3hcxlfcdx.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt3whtwpqlp.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt3xlnuygej.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt3fdfgghjo.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt3egprpndd.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt3htcfodcd.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt3gexprveg.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt3andmcthe.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt3yyqxqoll.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt3yetbvowx.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt3uxoxpgcg.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt3idqljaie.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ilyzhlar.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt3buzuzzie.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt3lemvzilz.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt3chpdpqri.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3hxyekqdh.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt3fphldegr.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt3mwzkgkxl.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt3rewjvvuq.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3xljqjpwm.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3aosxisru.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3bceyjqas.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt3ezhfjhsq.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3rprvwnxm.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt3jrvgjdhf.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt3uyoctgzb.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3tsyjgdqv.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3iykfbalf.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt3saprvpij.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt3nljhxzmv.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt3ekugnzyt.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt3efxnbqoe.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt3rzpijcsq.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt3uqgoxcor.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt3avspkkwg.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt3toavjbfa.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3eefdueue.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt3ocpwfxtl.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3eqddclnk.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt3fthlezfj.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt3mlbemlzd.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt3mkmmbhgt.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt3irrfmuio.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt3sdyooqas.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt3wgwmsqut.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt3rrumxadu.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt3xmohaklt.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt3vrgglfpz.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt3cllzqjdc.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt3dsecbujk.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt3hacmkwat.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt3inpbuiqf.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt3uttgutgl.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt3gvnhjqpl.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt3xccdvspw.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt3shetfhwy.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt3mzqcmlzh.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt3ibcifkvx.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt3csaxjcfv.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt3ujcvztqd.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3eqhmttei.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt3grjxuikb.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3ywbemsbt.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt3trystoyq.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt3kgcotncl.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt3gznhqypo.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt3hwefkoyq.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt3wxsjccxh.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt3wqddyndc.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3fgasrvdp.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt3jqwxkzlv.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3mzmkmoir.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt3hksvlpdz.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3wcsfhjfs.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt3okhcfupb.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3ejvqorvq.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt3hgicjiet.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt3zipmacsq.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt3hfqcouai.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt3wyeatosq.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt3pairyikv.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3pbdvlmcg.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt3xrlkxrsm.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3hbtbfftk.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt3ofsypdkf.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt3bzvfjvfp.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt3gxiarqxe.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3pwivfodn.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt3idcqlrha.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3zaqsqjrq.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt3kbgobwui.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt3hadiuplx.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3ypnmhyxw.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt3smhryqag.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3tlvdhqtn.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt3babdmyxv.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3nwbkuryg.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt3mmnmnkib.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt3qyxmwowy.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt3kvnimbxq.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt3kmdxbbot.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt3obanfqrm.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt3ujiujema.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt3stguffuj.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt3vxgpzaeq.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt3veztvqtp.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt3htvkabzp.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt3zvyfbmbi.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt3tbicebxn.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3vsefgufe.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt3wwsmalmw.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt3qzdyrhzx.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt3rutfipxb.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt3zoebdych.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt3pchjoxif.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt3etubyudr.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt3cjrguvym.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt3xqsvwjif.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt3kdwjvmmq.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt3nkxfolyo.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt3gdilcwbb.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt3obkrmbmr.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3qpazrplf.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3crddxkye.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt3lcfrccex.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt3xybjraha.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt3hsrsmzmw.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt3dxcmfqnd.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt3qznhfzsy.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3wdmbrjyc.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt3xamcqozp.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3zbzqqlab.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt3jnbwzlnk.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt3gefskqfv.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ylmmmqlo.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3usvgtvxp.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3mgmigmxc.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt3sarewykg.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3zixzauml.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3uvcuavzh.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3xjxuzyoc.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt3hskmughv.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3mfcgwahw.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt3hgxwpffj.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt3clodsjxa.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt3cxqugbao.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt3vqawstbx.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt3ccastmue.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt3kxxvxwfc.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt3jhtsbfrx.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt3fptlmlsu.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ruzbetxw.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3oborsgen.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3osjwnfpf.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt3puxkuhbr.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt3tozroedf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3yjouqxlt.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt3jymtkvob.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ytgskqfw.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt3swmdwozq.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt3elezwdub.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt3yvhcrjhr.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt3dflwxxci.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt3egooshkl.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt3jmuqqqle.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt3ootcyorv.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt3pajvysqg.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt3przpsjco.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt3cbsnwzjo.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt3nxbpmpaq.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3zkwkwfuc.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3mbciusme.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt3xpbmobkw.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt3eysknnrx.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt3ngacliky.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3qszbhsxp.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3mghtxlsl.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3xilxbmth.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt3ifvdbsbx.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3halgtyvd.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt3vmnztjfk.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt3ufompshw.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt3hvjczgdp.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt3nisgiaef.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt3gzmghntk.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt3alojhedo.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt3jaglhasc.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt3ypcyqisv.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3dbayqmqa.html


<!-- 参考信息 -->