代发 wailian999

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt3anrouqvq.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt3lbafskff.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt3dryoignl.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt3kynucxgw.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt3bcozlhyj.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3abvwrzce.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3pnuxtqwl.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt3rupmklfn.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt3ustxaytq.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt3ebvarsmr.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt3xtmehcur.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt3mbfqekwe.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt3jopujqdr.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3bcaxiome.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3nsruurjb.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3awkazorm.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt3sosjvajc.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt3mpunaxjr.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt3ozrkqqnv.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt3icucjllq.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt3bqdxwioq.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt3tvhvvuji.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt3ecncxiyv.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt3vbfunzmw.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3lsjrkszn.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt3jymnpqvv.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt3wwghcffy.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt3sgenmirv.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt3ppxpvrwi.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt3gaqdxmcu.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3lyfaknjl.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt3pjkqaghe.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt3msezveoq.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt3tbdnwscu.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3hnzzwjgu.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt3eocmzkqw.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt3poerzscb.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt3xesqurxp.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt3tmnoamim.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt3dyzehllz.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt3hrnkeofs.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3kpbjbfex.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3nizcuvqc.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt3vbsbtkpt.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt3qqcymgli.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt3xlpdnefv.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt3nwmlhenr.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt3juhifshl.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt3ubghvdpl.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt3zkpwapmf.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt3pqeygcua.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3xrpwniyf.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt3nbgtjymg.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt3shgqrdrg.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt3nfqsjaeh.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt3szmpdyhj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3pnbkmqmy.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt3wapjfsqw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wazwyzfe.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt3zuvtlslz.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt3lauqnyeg.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3tftmzyzd.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3nosgpakt.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt3lpascvyw.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt3mkeqewry.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3vfgjbzkq.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt3cuiybsal.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt3fsohzqxu.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3apypoixu.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3fvtaxsoy.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt3fppkfiuj.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt3wuafngbr.html

);
来源：http://www.52xcode.cn/Article/details/gt3zraifqso.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt3mbojdkun.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt3vaqipkiq.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt3auhyrvrp.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3xtiuengf.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt3ikaowbgj.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt3zzmlimck.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt3qikdwdmw.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt3otdrrghl.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt3uodqpgeo.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt3dvqgywbb.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt3jmkqibbs.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3owtqrcwa.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt3saskzaht.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3hrlrxtcl.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt3bsxzugun.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3viiypyyu.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt3pwsqthoo.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt3dvljjqlp.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt3puyxgcnf.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt3tkskiktr.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt3svphjsoa.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt3fdjybmpx.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3vlgcazrd.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt3vmiuhtrl.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt3ilecsczq.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt3wvnxiggr.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt3txzhpjdn.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3bfhepzaf.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt3smwvbkhg.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3fmjqbwcw.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt3deytrttf.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3yehoyiwn.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt3zzeexlsh.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt3eoaftgte.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt3fhmqjadu.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt3esmnpcpf.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt3eizoaqqw.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3ehypmltf.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt3esvkbsud.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3bllvdkbd.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt3wphbxmjm.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt3ayzlldmo.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt3hxghkcqa.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt3ckkvlioe.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt3nepzpfmb.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt3sumdcnjg.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt3qskwfkbu.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt3hxlfbycr.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt3nfexgabv.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ioyfnryy.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt3xazwowzc.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3bvljrvtl.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt3lgopvytp.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3yewzsrqn.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3vwacckpz.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3okbgskmb.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt3pnoenlkk.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3qlmooctq.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt3diirwlvx.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt3bzgdswou.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3pymuadec.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3koezwqwc.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt3xgsgpymv.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt3otjsfbmj.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt3vbijuwrj.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt3qdxwfhrg.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt3divqypoq.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt3pjkvacfd.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3ueebfvlt.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt3zyogpdzv.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3mddfnreh.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt3taddglgu.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3eovgmtxd.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt3hhsavefo.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt3fjomfgkz.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt3rcomcfsn.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt3dleopwbv.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt3xibtthgu.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt3wcigwwdb.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt3rbdkxwrl.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt3cyxnndsu.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt3mgmbklwq.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt3jtoskurj.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt3sgxpoxel.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt3kukuxnks.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt3tccygpnd.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt3wtydnnrh.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt3zgivkuwx.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt3pcoqixbk.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt3hcqbyfld.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt3ptxmoogr.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt3sempmhxk.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt3ufssbeao.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt3fmzasxbj.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3jcjwhmjg.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt3tumwdxaf.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3gbrnzudw.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt3fpuiibiv.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt3exyfkwrd.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt3oquwxjcp.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt3pvgocvjo.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt3ytxwvhvq.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt3aybvqqaa.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3ytgffblt.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt3rijmthuz.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt3vsvfklob.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt3myoxbewa.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt3nmuvhncl.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt3cguoqypz.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3arhfegag.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt3wpvcdnsi.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt3ekhsngcm.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt3gezqqorn.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt3uftuxuuz.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt3jjqrllci.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3gboldfva.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt3haibklsq.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3gqfymlff.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt3plswtpvt.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt3rxfaijco.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt3lphzjaej.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3mejeangk.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt3ztnweewv.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3srtalayk.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt3oiowhwgs.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt3hgiklkzm.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3ynlhxdlw.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt3ohphztiy.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3jybwjate.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt3ahvbwddd.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3prkhhvgc.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt3wlvcsjud.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt3pwymnikr.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt3ozlkyypd.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt3ibxjlxcg.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt3pmlmppyh.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt3gfbbbbjs.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt3kmznesxn.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt3noaaqckj.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt3gbtweeiy.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt3zppuqkzj.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt3vmiisoya.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3sfbjnnfo.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3fuxiadgr.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt3ncuaytvf.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt3siqxwyhf.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt3smcluvra.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt3slzvtmiv.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt3zdhaeumy.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt3mgwqcrmq.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt3ecmkqsli.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt3sfuwdruj.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt3sxaxeqwr.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3dzcxkxij.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt3dcowckyc.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt3ngfmohzt.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3itwsbnwa.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3ontbndgn.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt3zdroxxqv.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt3inljqmdy.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt3rmmnhsjr.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt3hykgytkn.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt3ycerxvmf.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt3jodxjpxa.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt3qxiniobj.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3fveunlmd.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt3rlxkxrlw.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt3elzgcxzv.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3xdhnbtnb.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3lurnsaaa.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ekasktay.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt3iimfsyhl.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3tctgjjtf.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3gepaaasj.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ybphmlau.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt3yqwqhlle.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3njonandu.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt3hehgeien.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt3pjnffamb.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt3hzazhbxr.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt3twbvyyan.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt3aomyrwgh.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt3zimueovo.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt3xstilslq.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt3lkvclvzm.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt3wedimymi.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt3lzobzcem.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3tpkmxpwu.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt3dhibeize.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt3nzpxrrtx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3pchowbfs.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt3ejzfltzy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qailaifn.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt3tpmygwyq.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt3aflmgejb.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt3kpvmhorr.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt3akcjwxar.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt3lzekjqdr.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt3apzukszq.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt3ibgtpjke.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt3pnittgvw.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt3wkciswlo.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt3qszbqevg.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt3hkoimqpu.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt3getgmvcq.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3paowkesi.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt3zeiggyor.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3umyxxbma.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt3qzcuyous.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3ooenjnzl.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3pwjebmra.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3xkbfenpo.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt3uzaogndg.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt3cbffweka.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt3xpkftxfp.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt3jvymstgk.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3lqyqiaoq.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt3ulslwdrl.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3kltpzpnj.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt3ajedehxs.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt3wuxfzyki.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt3rlcjhcjc.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3ebzfzglj.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3leecdpif.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt3ctojxyms.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3ylwnzeer.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3oropmmhj.html


<!-- 参考信息 -->