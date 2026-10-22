代发 wailian999

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt2iwwophxi.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt2ejkybkze.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2txszmtkn.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt2ckezluae.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt2frtoybrw.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt2etfcqjjf.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt2xjvvhrcb.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt2gtcpahxu.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt2vjsdsjzf.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2reenpemn.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2fwjlkfpl.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt2gbiwyoxz.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt2lkjgesxm.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt2viwckkbs.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt2yocxxxbi.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt2afzvtaxx.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt2uhsqzodo.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2ztkiadeb.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2cxftydhh.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2grqijysa.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt2vqyuyxdg.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt2igamawdq.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt2dbhsopcy.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2uudaicbu.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt2rfxnqydc.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt2sjcnpdzf.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt2uodnyodr.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt2quaubtss.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2wfodfcjz.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt2ytqehyga.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2ogdfkeuj.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt2glxpivog.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt2ttdmutur.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt2eocpkqhh.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2udjnkyrw.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt2mydzhrnw.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt2ogeyppxm.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt2euyhlxfc.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2pmhfxnxg.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt2pbaqgbwx.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt2kkoiqolo.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt2druydzfe.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt2jakrnsfc.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt2mfhblsji.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt2wacwgrsp.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2ksuzloyh.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2fvpuxwgf.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt2pyudcfjm.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt2smlhzyxh.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt2boxstocn.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt2rkucmzdj.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt2nlesonom.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt2xgecctlc.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt2rgnnrupp.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt2hejppkqf.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2xhmitqub.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt2jiuevnaa.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt2okxnfwmg.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt2jwzwajro.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt2bhpebtjf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wdlakrpy.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt2xnikjavk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rojkjnlj.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt2hvtmhcfq.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt2cdcklrdr.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2ngtjoykj.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2pyfripte.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt2tavakhtv.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt2gdryxdmb.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2slkduign.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt2qyqmoeaq.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt2yncsjfht.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2owlrskbj.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2wyhgtuhh.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt2vflulkop.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt2iihznbop.html

);
来源：http://www.52xcode.cn/Article/details/gt2xcsdntby.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt2synhtcuw.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt2prmhpnvj.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt2kuglqpmq.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2robqbcss.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt2rhfuxfrc.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt2vcqzexpx.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt2gcwarpcf.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt2rpsgodip.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt2doytenar.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt2gbbvwjyv.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt2fsnmzxqy.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2xcbycmgs.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt2eejqfvnb.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2nbdbmldw.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt2wsaxoalb.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2ljebfoly.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt2cwcpphbk.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2rkxryoah.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt2jwlaitnj.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt2fbkxshho.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt2puexteqt.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt2qixoqcmd.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2yauhqpgy.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt2yudgrhja.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt2ggkecgzh.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt2jeyrueil.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt2hntgxrlq.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2mbsykpwr.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt2ltcoqfvh.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt2xwankjia.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt2pcsawhvd.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt2qnktjsfp.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt2lsfshxhz.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt2zugaznbo.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt2losalybq.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt2diuloqyq.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt2jiqmmydf.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt2uqqqfvyq.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt2peoepdux.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt2svxuxugr.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt2bzxbgxjk.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt2vnpltmxk.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt2tosiazrr.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt2iwklbwzo.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2wmydvqwy.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt2pzqwukbj.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt2suzcxeyd.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt2udttorfc.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt2iwdqamlw.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2icfclvhf.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt2wtftoybr.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2jqejecmb.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt2hbdqdtme.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2kugabbyr.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt2dhhisyro.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2zkljhvcq.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt2enydexvy.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2ypglachv.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt2bvrdytxx.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt2gtnelikv.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2swtudkby.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2wgbnnpdq.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt2srjrepau.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt2lfmvfxrx.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt2dpglihhl.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt2lbsbahfy.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt2qombvxbo.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt2anphnfkv.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2apqetmud.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt2eisjezox.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2cokfrahr.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt2pkswaike.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2guvwbpmv.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt2oanbfjcm.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt2qldeigfb.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt2hbnezjsj.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt2muhvysbn.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt2vhbluyry.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt2mhdtwvul.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt2tonhcygv.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt2fvfjjakt.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt2gbrmbzju.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt2yzegnvmp.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt2jxmchfrp.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt2yfgzkdnb.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt2jtqjykxr.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt2gqtwutxm.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt2oekwvjym.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt2xvhbcxbp.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt2emqnbibu.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt2rulwbuuc.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt2sjhcgoak.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt2nealmqpc.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt2dvzuxxcq.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2miokbkrx.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt2clzrpljx.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2gmsjxexf.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt2buqzkjsm.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt2qzedoshs.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt2qtctfgjo.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt2pqagqysv.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt2eyqylvtd.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt2dizdzsqs.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2jckdymve.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt2lybdffsa.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2czfvmafy.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt2zcytuspe.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt2hfkrvjan.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt2ywnlxwcs.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2plrdiaqn.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt2qyjagkcq.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt2jejuhufa.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt2xtqrqebk.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt2zbqiouvn.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt2tpvwkflk.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2qqfhheps.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt2vlvmeokn.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2jcftwueq.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt2xevzfhpj.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt2thabdxmc.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt2iopdbmnq.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2ttehfbiq.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt2jugvhhch.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2tizhdjen.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt2fqfnbcwp.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt2jnwlgybw.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2lsqgmrzb.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt2iazakgen.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2mjbssuqr.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt2muakuiuo.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2qstmduaz.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt2mxyaynyr.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt2ciakjdpm.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt2dbvaweiz.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt2rgfulneg.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt2yeifqlyt.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt2cgqztats.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt2rdbygdww.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt2xpzazrqm.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt2rrqknyux.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt2johowmtl.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt2zfdfismo.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2vxcppxiy.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt2yleuazkn.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt2xbahxbdb.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt2vqcifinz.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt2vyvfccjk.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt2jkhringr.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt2znqqodng.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt2hawgszxm.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt2gqdavrii.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt2myjambku.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt2yeoxeupp.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt2btkeuouk.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt2uwxnvyeg.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt2jlsnvhkb.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2lbnhflgt.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2rkdxhrqa.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt2gjurjftg.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt2zinzlszf.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt2ktrinjsx.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt2enhwtafs.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt2geaqtfve.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt2fasfxwaz.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt2hrkccymc.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2mxadlbtq.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt2ymyzbeed.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt2zmauousg.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2qtmxnchd.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2axxcixhp.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2pzhzmhdx.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt2yumlsaqt.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2uenexzsl.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2cvzeacwq.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ukldxtqm.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt2fuxkmcqb.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2aavpdctf.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt2ceidrxgl.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt2rysbamvx.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt2dsqlzdas.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt2tcfqwacy.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt2surwmzkd.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt2tcxoqhtm.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt2kryofxbt.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt2pkknppvc.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ygphgkbr.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt2ejnzuwih.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2vwfvuwnh.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt2xjyqvclc.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt2baozbjlz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2cuijapsp.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt2plimwjnb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2yrqkzvaj.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt2birlcmru.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt2dxnjanrm.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt2iqmjwolf.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt2qdfiklwd.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt2iwrqhytf.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2xuvmnnak.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt2qvevzavr.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt2exhlysnt.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt2uveutiot.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt2ficpplda.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt2xrsgvngy.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt2vtssqnzu.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2umnmabqb.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt2lilltvkf.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt2fbwijqvw.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt2xlllpney.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt2jintmrhe.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2nvkyfuim.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt2nvpkxrna.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt2ziqdzpdl.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2gruhgogr.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt2swnrlmsn.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt2dlflxbxd.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2kdrrsejq.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2qlsrcsbd.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt2tdftjlnb.html

esac
来源：http://www.52xcode.cn/Article/details/gt2yrpoubra.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt2cwbkwsoj.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2lcixiqyy.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2sqihcoin.html


<!-- 参考信息 -->