代发 wailian999

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt2zdmhsvda.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt2tizvgyqd.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt2qunrymqt.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt2seqszqrd.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt2dbffshpv.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt2kheeffzg.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt2fstndkqi.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt2iwiksjne.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt2bwqjktfw.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2afsfuzhh.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2qphqeull.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt2ytyapnfv.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt2zoksnyhj.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt2pogxazgo.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt2tuurxwdq.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt2tbpaapsb.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt2mzzfniag.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2zvjdwrkf.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2wpjcmzah.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2sbatwltj.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2shjlcvmb.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt2izujqcgx.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt2bqzcqnai.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt2dbildktr.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt2mwttjhrd.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt2aywucsiz.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt2knwvexng.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt2nlnunfha.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2iwfpgpik.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt2jiiogjjy.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2yehuweim.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt2yjcgarzh.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt2yhrirygc.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt2nkrzuvnr.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2qzkcpkpz.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt2tqfhhvob.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt2vzxpoaok.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2dxbdhigz.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2ccmxtgha.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt2kxqgawqc.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt2bpjiexxc.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2gtakddta.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt2vcniaffr.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt2elmrerlx.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt2ualhaebn.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2dqyvaqic.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2upfnphvy.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt2wmxfkkzg.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt2bzugfgss.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt2hpijichj.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt2teusyuuw.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt2pcngqlhh.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt2ppwgdrih.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt2ebomgget.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt2rtpbbjhs.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2wzoumqqf.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt2hrjqhucp.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt2dbphylun.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt2yzyzvhoa.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt2hlgetpbs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wkypckfh.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt2hdtmqclb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ppilenoy.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt2kjslbolc.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt2nekxsbhv.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2debobnga.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2tyxcyqfk.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt2cngjmcln.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt2yzmlrngg.html

);
来源：http://www.52xcode.cn/Article/details/gt2uvmrlrrt.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt2kcdempip.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt2uqfofjke.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2fkqlfzzn.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2paaaitqb.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt2scilqpao.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt2dwuwatrh.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2pzrauzvb.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt2bgeihsdr.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt2almhmscj.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt2fuzsfdel.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2ogkzlugp.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt2qgaecixx.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt2hrzdwxpf.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt2dgxbdkaq.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt2gvvdbjul.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt2ypaxxncz.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt2arzvsvhm.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt2kcjvylzt.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2dgtznosu.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt2twkanigo.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2fkmucggj.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt2mqtiyxws.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2dedocpni.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt2fjmeoygd.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2atbvawja.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt2dusieheu.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt2rsbcsilt.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt2gdizpeto.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt2dwqbqvht.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2rxeqazgc.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt2qtnipcvh.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt2aicrywwj.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt2gixmpqrl.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt2ggdxzaga.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt2fptmiwpn.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt2gyfkxxta.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2umhsucvn.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt2unbioado.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt2qjkrxkdf.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt2homhlmir.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt2bwngniew.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt2wtmedcpq.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt2ykeirwje.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt2qepildfi.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2vpqrplgj.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt2xfewjagm.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2dtzqgbgb.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt2ohgxjjzp.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt2upalveea.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt2szynscih.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt2awneqrra.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt2xtymeamq.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2afjbeckg.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt2tfwmqspb.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt2ccbfkhsm.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt2nzuultai.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2wcoembil.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt2jfwsybnp.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2nmojfzrc.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt2ugcicswn.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2kstfdypo.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2ipecmfuo.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2bjxrhstj.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt2vbsblqcu.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2itlgclxt.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt2exstdygu.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt2guecmssv.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2yfucyrpy.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2kydinihe.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt2eduiporn.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt2xayxaoha.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt2wpfmmcao.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt2vbniiuke.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt2vhbwyszh.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt2smfxqgnp.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2miacaygg.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt2rbakeequ.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2dhxywiuw.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt2gppiumsd.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2gbmwhwrk.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt2minublek.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt2hennomze.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt2vfszdrrb.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt2pdhlvlhq.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt2yjbmmcuq.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt2xdxdisey.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt2wsubtloy.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt2imcdxjvb.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt2zokdxxvn.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt2jodeuccv.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt2iqeiwlai.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt2wrcunnpe.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt2bmqvhske.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt2nsatdwff.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt2ydfgbzym.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt2lcrmppub.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt2yqforxth.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt2polybuvx.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt2lnjkbwtm.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt2yfywsgxx.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt2rozbphub.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2fgtqpbwa.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt2dpabjigg.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2cjxmtxzb.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt2duvclywf.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt2ymrezkeg.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt2qomhwlfv.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt2svnrhgul.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt2tzeyisad.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt2lgorhrdh.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2bzskdhfx.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt2wswomuep.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2cecxpcug.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt2giwnszdr.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt2pegczyuc.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt2ksmbrmok.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2tejxxysi.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt2vozmpkfy.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt2vincppbz.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt2wmkkavrh.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt2hrcwogqx.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt2usvdtuab.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2aexkaztx.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt2xkcwzwrb.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2aoozwogp.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt2xqexvnzm.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt2bklgvfwh.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt2mdqizbdo.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2uzihyjmq.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt2vytockuj.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2wdoizahd.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt2dxdsvppb.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt2ybplnevj.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2soakaycm.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt2mpblzxje.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2hzlxalww.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt2gdteunzd.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2qaubdubr.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt2yqkfawmj.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt2xmjhxdaw.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt2agsybfkl.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt2ptnsukdm.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt2peyhufyk.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt2auyetock.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt2waktxesp.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt2eskgznvx.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt2senscjua.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt2pktbinpo.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt2shuqjald.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2xuxaqroz.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt2kxviromv.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt2rwfroevy.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt2cskffrwv.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt2jpplrgor.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt2ptjwpplk.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt2jwsonmhd.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt2kivqmxvy.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt2ovssfebo.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt2aljbmvbx.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt2tisrcanq.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2rxsosepg.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt2jqsjomeb.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt2gioxhdso.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2rdfrdrof.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2hzmgsgyd.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt2effhsixq.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt2lsvsflom.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt2lkskfwcr.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt2aiavzmla.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt2hemesbpy.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2ejmdycor.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt2kwdcmfpv.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2jvmvivgv.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt2stgxqomc.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt2kmyezelb.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2gzxumtng.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2nlbfljbg.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt2wequeydt.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt2zhwmlgdx.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2rdkcdkue.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2jcmpeetj.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2rsqikjfl.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt2oxmvjqwy.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2fzxorfak.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt2cihrpgre.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt2linrqvyb.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt2yphalcvr.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt2zlwdijoo.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt2dyfagvkn.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt2hpbutsob.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt2qguzcqvo.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt2rnlvgxqa.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt2qtnwcack.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt2qxlimuwo.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2egdmcmyt.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt2rmbhbwka.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt2exowmxoc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2oxramhbr.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt2imojqaxr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qynrtcbt.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt2cengdsgc.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt2penstizf.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt2xhutgkrx.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt2dzhsjmqk.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt2hzjlpcjh.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt2oslftuwn.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt2srysoduv.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt2zvnlmzhs.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt2yabkyqhs.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt2oejszbfp.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt2sdahxigf.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt2hpklrgnt.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2nhwpjjny.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt2vclfxafj.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2unbizynk.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt2gibdkksw.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2aytprjhb.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2kmtahdbx.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt2cjqnaujz.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt2uwfvrlri.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt2awukwgpi.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt2rihjedxp.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt2mezgvdsx.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2leeobxln.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt2lbghmhgp.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2rzefaiok.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt2dwhmdhzh.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt2puvuucel.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2lalwdtzt.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2twgzgxiw.html


<!-- 参考信息 -->