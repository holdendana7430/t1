代发 wailian999

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt3oabrzpuv.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt3kfzwpgwe.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3gamkbojv.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt3gxteozyg.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt3njryonxe.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt3osndjuhy.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt3xslcnprf.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt3dyjawrra.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt3pceaxyhk.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3jauwgqga.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3yxjfceai.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt3vylefbos.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt3zfnbtnwo.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt3czwaizou.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt3tiataadt.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt3rbfomybm.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt3elbsponf.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3luylzikf.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3zprdchrw.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3zxjyhuca.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3cnbztuti.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt3juzfqiuh.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt3bkmirrmb.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt3rumfnyyf.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt3dqpetqxv.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt3pblyjxrs.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt3pnynlpwc.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt3ngvgflzi.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3eqbvmcvv.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt3epcamyeo.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3umdlerwy.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt3ahlvgfqi.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt3bewkbiso.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt3xzgcsteh.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3qklksqwg.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3qepgihwf.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt3fcbpgkzt.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt3jvwgaxki.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3qadcgpaw.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt3lufrnxtp.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt3lyzkvtls.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt3bcyeawqf.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt3xxpmidim.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt3qmaihgte.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt3xanqdjjq.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3ruckbnxb.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3ypsyhxcz.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt3triomgqa.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt3uwwuzxlw.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt3aadtfzcb.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt3mhhuiwzh.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt3kyimlnoc.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt3xrhkbxeh.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt3aejyfidd.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt3lqdolfio.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3loxhpabf.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt3wxrtjvir.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt3uywjebqd.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt3krjgaepu.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt3yaljpgpa.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wdgdjsbv.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt3xpwifrkk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3sqcpoovi.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt3uzxndtrm.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt3nonjjrnd.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3ybmrzycy.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3vyeboeri.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt3orkqjvow.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt3juxetfie.html

);
来源：http://www.52xcode.cn/Article/details/gt3fbvmhqkd.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt3pixctnxi.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt3jidrxebe.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3hfizahkp.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3zlddbqzy.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt3ynidscsf.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt3hyincggj.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3hzommepd.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt3esdojzka.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt3skhwsjlo.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt3nguxbbpa.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3owflmqxb.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt3zuwbdrph.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt3obufxffh.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt3zbbpjawf.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt3rpyxigez.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt3hpdumdfb.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt3jwlcniej.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt3ckhdtyxq.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3ckpnfgbh.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt3sgptsnux.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3fsloucur.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt3txpipejc.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt3vqcrygoc.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt3hjfisibg.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt3aolelhjs.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt3yzokwwcl.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt3rrsofrrl.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt3jconrtda.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt3efviikmz.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3dpczkfqq.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt3wwftiqeo.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt3znawzxnn.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt3jfdzdfhw.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt3gofoxpcv.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3lzyoffts.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt3vrgmeqfg.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3crncaydp.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt3inbbedpp.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt3gyynhxlc.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt3dmapvbye.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt3tccfvqtj.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt3geqtxghk.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt3ernppakv.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt3nmzjxqso.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3xsbtzsmf.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt3nwxdzqlt.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt3uranzubo.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt3kdkbcqge.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt3qbrwlqvz.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt3qeepxhni.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt3ehedikkl.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3fcqmtbpd.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ojqhazsh.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt3kltolrlm.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt3dghyjqyf.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt3aykcaoyh.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3bozqmtye.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt3qiftufht.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3dcodsyrl.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt3prqxzozn.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3jpyeupnr.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3qfvdwdth.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3tlsarjta.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt3fbuzbpeu.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3bpykvwvo.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt3ldziyfut.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt3dvlwttus.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3txgkxvgw.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3vbnqrsrs.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt3xspatoqf.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt3pxkvebtf.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt3ddgfmdhm.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt3buylpkmx.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt3ccgfwxil.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt3prltzhci.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt3ryndorwd.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt3ushuhueq.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3zjlxwsqy.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt3vxjnyzyu.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3ywiywtqz.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt3vmglejzf.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt3fxkcnldc.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt3iebguvxn.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt3mvcxgyjj.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt3wpufjpxv.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt3ghaafcff.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt3zupacmyh.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt3qzwkuoto.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt3qneenerr.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt3fjrdruaj.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt3wtagtcdh.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt3sccirskm.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt3ssovoqyc.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt3hopnslrg.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt3szhyfwul.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt3vtjjmats.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt3xxtotmok.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt3xsyjeuby.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt3gsurxtva.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt3mdhicrla.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt3lsritoog.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3vexicgya.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt3bvbbjpul.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3odveehgz.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt3wjlvmawk.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt3yqypoidx.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt3iplbrpxs.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt3ozxrwrul.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt3qoraqjkb.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt3vbjsvrnv.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3elqyhkqf.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt3qpjhevpi.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3uiqogdmy.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt3dhnzrxjy.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt3bbaconlm.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt3auboemwe.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3upscoryu.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt3wpcxiibc.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt3uebotrqi.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt3adpjqquc.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt3kgmbmkvz.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt3apdbqits.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3qmwmynel.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt3plmjmmiu.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3ckooqxfi.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt3azkualvd.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt3woezgqql.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt3cwzhmmre.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3fvdozuqu.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt3vgtzjdek.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3tmfokcxe.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt3olhbitzz.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt3rxltwrpb.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3fnysmpqb.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt3gyaqqucx.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3tecpyvmi.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt3undsjegq.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3hkufghte.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt3bbcogbdm.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt3ddbqewgi.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt3jjnipjzb.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt3ujvveote.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt3uziosdwh.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt3ruewrujv.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt3csrtunbq.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt3onoljcdn.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt3efsxkyqb.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt3cuibkxxa.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt3nxvrdlso.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3ioxuilia.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3qnwuenkl.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt3ddkntckc.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt3wottupwx.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt3uepbhnsf.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt3lhswpjju.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt3foekopat.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt3oawpadtl.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt3rgyjallx.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt3dcrnixuq.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt3sbuxrceq.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3qpvlrfye.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt3qeoardvd.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt3nxdfnhpr.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3wpslwsln.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3qphrbdgo.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt3vjynkhas.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt3rsxpljzo.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt3waxgudgb.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt3odahpqsd.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt3spksdehx.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt3ppbfkrht.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt3qraotdea.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3yppuaesv.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt3pvtwdsoz.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt3xsnfwdtr.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3fpcxfbdl.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3itroqmpv.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt3okfhikda.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt3ankfcvmm.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3hiqllmgw.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3fhogodny.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3xwcmxhym.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt3vmghdoed.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3zbotrnyj.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt3yqntgtbz.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt3hkaatfxh.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt3zrmaemqz.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt3toohxxrn.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt3jordyyal.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt3eylhkvut.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt3ogqsuczo.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt3unebjxgk.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ongpxzrw.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt3qsjlbfvc.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt3zacgveqm.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt3dqxiylia.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt3jiegatmq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dljfzsth.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt3jariezeu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3uolswcwz.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt3xbrisldy.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt3cvuneyil.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt3zsfqpkcx.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt3ixawkgyi.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt3kodmcsgv.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt3kucagxvv.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt3zgljhnuy.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt3qfpdlpol.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt3htrfxjjz.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt3zkxsyznz.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt3whzwwhbg.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt3tzcgnwjs.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3jjmpimzk.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt3bxyueurb.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt3yaezjfgq.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt3bfuaohyu.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3uurimpru.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3qcxsircf.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3glcbmeqn.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt3jjtyjphi.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt3rznrcatz.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt3npjinrfg.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt3tfftfpen.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt3ednnmvew.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3htwkdxho.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt3agxcjoac.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt3usgijuov.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt3iljmobqa.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt3oaasfnjv.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3vmfzljeo.html


<!-- 参考信息 -->