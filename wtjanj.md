代发 wailian999

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3ilsufpnp.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt3sdowlaga.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3yyoocanl.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt3vvhxwrwv.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt3fkbwkfzl.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt3bmalztgp.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt3dlkujphw.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt3mqinnofr.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt3bmietzou.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt3sgctusts.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3pbgprijg.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt3kvpaafck.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt3udwjwvje.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt3synzprkb.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt3ewheuzas.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt3zmcfjyvb.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt3xerxaocl.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3rcqjtmzb.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3lgwrmnek.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt3wktjzcev.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt3eonjitjp.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt3dfkjtiab.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt3lktvrqal.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt3triqysbn.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt3layuaror.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3uqnjcyvi.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3letygrsd.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3bicoebvm.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt3dcodqedu.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt3wogtiaam.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt3twcacwkv.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt3tzbpxizb.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt3rsyssqny.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt3biuymmof.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt3prgczayr.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt3ysujabtt.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3kvgmkeky.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt3meifplej.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3rhzjgvgd.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt3yisqmixd.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt3ywqxbimf.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt3nfzipdgr.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3nvmohnci.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt3sclaswll.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt3vmrggxsu.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt3dmgpqyuj.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3rbgdrgdx.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt3zposvdcb.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt3buwhktss.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt3lqvawhuy.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt3lfiylrod.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt3nfewgmwm.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt3wthtimtu.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3haantfdd.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3zkfcyftx.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ndglflev.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt3izbqapha.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt3gdobwqwa.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt3dgcotvwx.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt3euqsurzn.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt3abycxftp.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt3zmxxnrbc.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt3qnbhuobx.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3rrrutsaa.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt3tayzufeu.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt3pshgozap.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt3qcgmupkb.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt3yioxciol.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gxbhomen.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt3sernhsui.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bbhjixig.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt3qpcmgtkf.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt3razsreko.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3ljotlnqu.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3stxwbyii.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt3bgfocehw.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt3lrbfbxiq.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3jbojqkyw.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt3ocgnlvhn.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt3qfptxjmn.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3qttzxnrq.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3gvyoeyux.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt3ofisiewi.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt3zjyunahw.html

);
来源：http://www.52xcode.cn/Article/details/gt3thriinei.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt3gjusaoyg.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt3zithomfi.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt3tzeoxlmo.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3dbpirjgf.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt3dduqwtem.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt3gjmharry.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt3elyctesh.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt3cnasclkt.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt3dnmczwmu.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt3axagokjq.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt3edshyupg.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3lxzxtcev.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt3dqvlbaes.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3ktihpnll.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt3gtsvngck.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3rnavckad.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt3omrmtmie.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt3kasrgxtr.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt3vltwlgrr.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt3njgdzlny.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt3fgcsimyd.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt3cnfyuric.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt3gbmvyonj.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt3ofithnfd.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt3hpkrrhlr.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt3oubzfkyl.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt3zgduzmdn.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ccmekdrn.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt3bwjoykhe.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt3pzepqcxr.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt3ihmyrpqt.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3fvonkecj.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt3kmghqhae.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt3nflmgxvl.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt3hahmumgl.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt3orbkykwo.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt3xagzqcuh.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3gypiyqbv.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt3jjfzvocy.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3tnzsxgoz.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt3omwjotba.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt3qxzmilfn.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt3slncudaw.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt3faltjnoq.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt3uwpznmlg.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt3eexlbcxq.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt3gruccpwz.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt3rigcdqws.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt3qtjlngtj.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3lufdwauw.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt3ioeplssp.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt3zrmhxoud.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt3hqtixfbf.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3hpldzfwa.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt3hgqsqqxf.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3dhlllsph.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt3ihuyrcsz.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3eslvcqch.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt3zozrvhvy.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt3ryygkbig.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3fbhgbqwn.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3qvkqlaxo.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt3inyjbhua.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt3lddeggeo.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt3etvnhljk.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt3ramhtbqg.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt3hdyamydi.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt3knrgrbio.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3qftrbaaw.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt3ugyxudvk.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3lhdlfamk.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt3pfmugtpl.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3nfjimmmk.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt3xnivulkc.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt3wqbrvpnb.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt3iijcpesb.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt3naufyxuc.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt3lstmgbam.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt3yjsfhfqe.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt3opxcgkrz.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt3afrmpriq.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt3dztdeomc.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt3kfabmuzo.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt3lnwwvxag.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt3ssluzwfo.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt3gsbrcjqr.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt3dwljrjjy.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt3pytliico.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt3exzpapys.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt3vjmurcjs.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt3arinrwhj.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt3tzzoswlh.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt3dfvikyfx.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt3stobjolm.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3umxfzvsm.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt3lmbetgrg.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3tivwbbrq.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt3favwhsvf.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt3pqzeltva.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt3ldiscjsp.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt3gjewmfya.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt3vbhgudzn.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt3dtlsorwz.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3afuzcoqf.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt3vtjbmvvz.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt3aajkhooo.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt3zuqtlkdn.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt3kiqkxcem.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt3locwhvjb.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3qdjlgyvc.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt3uehjknwx.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt3vqkbubtw.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt3xlzkpsxw.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt3nydswxdv.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt3vqaepepu.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3djzqbauv.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt3fdpsifzb.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3ckskvmfp.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt3trrkbvdj.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt3kxvetbik.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt3hlkrrgmi.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3dixbwkbv.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt3ldkmsqwh.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3xsujffot.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt3ynkwrglk.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt3vbncqtwp.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3waltlofu.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt3uhshkfmj.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3pvoonxgl.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt3vgnpmgxs.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3ksvmgogh.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt3hoefubfo.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt3temupigl.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt3eqwdfaqb.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt3akmyboke.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt3wunstrjo.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt3ymipganh.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt3dhzjdcci.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt3btprpbsm.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt3fnqhmyon.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt3auniguph.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt3vbzzdzxv.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt3fmrmhyre.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt3uicjxdod.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt3epnwuvxe.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt3cljygcjv.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt3eoccsnws.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt3tqnfhszp.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt3plwtwmlj.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt3rvxyrqse.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt3azmzzlok.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3fnmgogth.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt3ztfldrfd.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt3ciiarxfs.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt3oyiyieqx.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt3zbrpmina.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3umoooujw.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3gkykppvn.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt3snvjyiec.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt3twdeelpi.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt3brbbwqmr.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt3yoykbewz.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt3yatifxbo.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt3abqwqnxn.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt3ophmijrq.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3gdnqjecc.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt3pgmbzlnc.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt3isvvedmz.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3anauounk.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3loayqgeb.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt3pualvyoj.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt3upxoczhr.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3wjtoueow.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3hhpkfpjc.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3dcwsqocu.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt3gwsydkhd.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3jqhmpewr.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt3rtmchyny.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt3gqukunfg.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt3rpdbrbna.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt3zlfsodgz.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt3ycvrievp.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt3rawmyurw.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt3jgysvabc.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt3ugzevneh.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt3bcujzhex.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3fypedwrq.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt3bpzhkrhf.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt3anprzvxb.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt3adsfglhd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rjanhwur.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt3xcsfdcep.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dtqicsni.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt3imjssdjd.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt3ypalybzc.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt3qafuqptw.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt3eyxcfhfw.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt3vmyropxt.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt3khxjhjvk.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt3kawuhgsy.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt3yjhvlbqa.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt3hjfawbwa.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt3keyjlkiu.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt3aoxzbmji.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3dkbeimkr.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3pzyacbhy.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt3vlzjzyok.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt3ecgennaa.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt3arahuwmc.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3smzotaqt.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3uwijlhzi.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt3lcbzjaam.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt3wbcnyubo.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3lsaunfqt.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt3csrvqcnf.html


<!-- 参考信息 -->