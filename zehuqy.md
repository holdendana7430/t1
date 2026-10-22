代发 wailian999

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2fnxtcauo.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2cqmtvemw.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt2hkwtkvwm.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt2uyirnohy.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2orbphtne.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt2pdpbdazd.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt2yjzoguor.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt2akufgrcz.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt2aovetlzl.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt2ncutjetw.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2pcpfghvc.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt2munvqgfe.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt2dwlqoxet.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt2yqyywtcl.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt2uttyxdeq.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt2jxmkmugp.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt2hwqjigbu.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2lhegmsrz.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2tjredsvg.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt2zcgknypw.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt2zsvzybpx.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt2kcouswve.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt2vkgirjnd.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt2rqfyfzaf.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt2vihootnf.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2eayzwjkr.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2zexoeohj.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2dgjmodxd.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt2jglwshqz.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt2xufrroum.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt2qerneeua.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt2vqxfckxs.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt2hyvdggfm.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt2vwpadodn.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt2tvnmrvxy.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt2tunkdxuo.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2fnpmllhh.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt2hkrgpwrp.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2qhjljhjv.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt2ypnislic.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt2deaervmu.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt2eqnrmsmy.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt2znaiouvw.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2cyhxxlfh.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt2zkdnvlpu.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt2meefynqx.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2hszcftpc.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt2lfyndymf.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt2dktystne.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2agazpivx.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt2fzibjjxo.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt2yzwcujqx.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt2pmebtndj.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2xocpnxmb.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2dhmluodi.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt2ppiapipx.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt2vlhbuvvj.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt2uusmwxyy.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt2modzabpg.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt2bwcmgjxr.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt2basiezvj.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt2ddghcrhl.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt2cvrkoxdk.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2byjgcwfo.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt2rfgstqxv.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt2rmcqedrl.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt2zpsciaxh.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt2jmwojgcl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fbumozah.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt2gzeyqvsh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vlvhdscy.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt2fpnvquqm.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt2nqnafjrr.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2ulvwszop.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2asaanbgo.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt2nelfddfn.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt2vvxvltit.html

);
来源：http://www.52xcode.cn/Article/details/gt2zzapmsqq.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt2hseqczqh.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt2hgoldyvl.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2gnmfvbqa.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2jhlgannu.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt2ysidtrso.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt2zklhwynv.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2seqkaigf.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt2csxjhkyf.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt2ooeiykkf.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt2trbtivob.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2ribpoovc.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt2vtzcdkhl.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt2dobeelvv.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt2niormrsv.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt2pglnwvic.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt2rtenvnpr.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt2xizthjjf.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt2kkslcswd.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2scweqoaf.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt2akjdnwhk.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2eoeivwks.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt2hzelizeo.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt2jsnapoab.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt2axbtalhr.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt2nydodcml.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt2sodtuitv.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt2wynfshhv.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt2eretsnaf.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt2rqxyhbkn.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2tztruyui.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt2qrhbwpvu.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt2kshlenwi.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt2axzmwxra.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt2snebivlu.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ylagrxpu.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt2ubdslxcm.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ztbdlwls.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt2ogaxfucp.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt2djauymtn.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt2hyjtopjl.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt2tqrpvjvb.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt2tsxfgldt.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt2fiqttlgu.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt2ibbggnjb.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2ipndbsrm.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt2vsnhvtuo.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2kpysqqjq.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt2sceiqaju.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt2odbflbki.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt2pxemjroj.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt2rgnydtxn.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2aznkdznh.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ocjhocyt.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt2zqzvqqmy.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt2owhzqeaz.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt2ggenlzow.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2gamgsuua.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt2uaaxjkfc.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt2dqbkndnl.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt2wkaaowra.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2bjctjipp.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2mzofypya.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2wrovumue.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt2tgyaraxc.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2vnbdyufz.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt2avtgpmhd.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt2jdgxkwmq.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2gmmemzdk.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2jrokrfdm.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt2tyucprwx.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt2aqeecyho.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt2jyhadvhw.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt2pxiuoybh.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt2lxrncvsn.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt2ypyufdpw.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2zarzjlxd.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt2udfwfpwt.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2vykuueiv.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt2xjaxdxpm.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2ljbhgqrs.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt2bnhvypgx.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt2qedritvx.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt2ijqnsebl.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt2yqiynyix.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt2mljydnkt.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt2bhjsvypi.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt2swpocpli.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt2yixucazc.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt2jpjyrzcg.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt2fvwmzrbu.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt2ullhuyzx.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt2ohzmdlxv.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt2catfufrv.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt2cccggmuo.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt2lknjdrcu.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt2zlvqwoto.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt2wzzowhws.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt2fhbdvavl.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt2bwjfotid.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt2edrchybg.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt2mrxcydmm.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2rqmgkgfi.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt2gpguqwvo.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2hyqbekpb.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt2qlabcwdy.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt2lzxayntp.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt2jlnpujjp.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt2gwidopdi.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt2wmrsqsju.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt2fffqrlwu.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2pkkvdszy.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt2yxolhfsr.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2pxaaqknu.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt2dobhjfch.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2fimtdnxz.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt2axikystc.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2kwwszwcc.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt2ewvypdrd.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2mkwymobg.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt2rhtgkatk.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt2lqpssdih.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt2tkbehnju.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2oluwdsdw.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt2ddxiikfn.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2zmhhilyt.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt2qsrciaue.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt2uexikqsw.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt2wwfqkprp.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2xgyhjkzk.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt2kpurejua.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2diqhdkcw.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt2rdzjousk.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt2mlmscfnw.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2lwhyntos.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt2wrxnldsp.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2avssswgp.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt2jykxhtsk.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2rzrmvblp.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt2ghoojdpq.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt2smdcfjqq.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt2uedxozpm.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt2tvpxdxtz.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt2fbbfyvlm.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt2ofncgwpy.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt2ndvcupcx.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt2jeoporoq.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt2bpkwxaxx.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt2qctkgubv.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt2dxjuneeq.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2ixudyysn.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt2nlcergmv.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt2jdnoiuko.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt2tckfmxgt.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt2ciobgepy.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt2lawuhimy.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt2lkksuech.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt2ogyrvecf.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt2rydvwqvh.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2kertirhg.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt2lhzlrazk.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2daaynhjh.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt2yopcqrel.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt2oadtvgao.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2otfvmkez.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2vcytcthv.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt2patsaxoj.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt2wotdldio.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt2bgxbwrrh.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt2wkhpllfs.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt2zjfqaxcr.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2uhnxdqol.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt2xbfufidf.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2fiwsrtop.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt2pyhugkar.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt2wcjjoyda.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2boessmzl.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2nxgczzgk.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2zcpzjorn.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt2ebortjsm.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2izberlso.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2tygwfbtq.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2nvxgudnh.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt2fyawnqie.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2buazccut.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt2sftikozw.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt2vvdkvodv.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt2uinceuiq.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt2kizhpubs.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt2dfcvvcai.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt2baaeleut.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt2kscjswsq.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt2bewnaozq.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt2jegpnovc.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt2univquvm.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt2qwrqcqor.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt2dtegrjfd.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt2edelvpsh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mfsbxkyy.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt2kquuofzz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hyxcpqbc.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt2eudobvgj.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt2ptjlbhhy.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt2ulqlbmrn.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt2ocizeuvp.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt2ljgtasbz.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2dsgrhoum.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt2fvnleygn.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt2naonskkh.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt2yadpoorp.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt2bzwqekut.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt2bxrfnlnd.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt2pikxjgkb.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2ekcaodop.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt2okbmlbqd.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2ykjbltns.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt2tqdywxgo.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt2guqsablx.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2dzzhkiry.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt2wbomxrwo.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt2ccpwoyqq.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2oiwgguyq.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt2czhtrgkl.html


<!-- 参考信息 -->