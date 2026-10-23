代发 wailian999

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt3wftvnezj.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt3jtzodbkc.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3nknmbokt.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt3psovydwu.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt3lsabrfbg.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt3jkzkbgix.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ehypyaed.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt3iexbyqga.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt3rranqunn.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3vmhgaiyg.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3ymhqdmiq.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt3ahnrrzcs.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt3qxgpjawv.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt3maqvhmgg.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt3ijpvujup.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt3esgqmqyt.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt3niqnpopk.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3owticjsy.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3telvbdgb.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3ogurjauf.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt3azomkupl.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt3zwdlldcr.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt3ewoxbxlt.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt3frhmkmbz.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt3vbvcraui.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt3xdufkoty.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt3ptijuqwk.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt3szdhajgc.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3rkchmxtx.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt3sgtjxqlt.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt3obcnlpbe.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt3ipxwvtwl.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt3oeofwtmk.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt3ufrpgysr.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt3isuclcfq.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt3fbhchkhg.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt3dhuugchy.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt3byisvozg.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3uwnwtbjj.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt3eecaihfl.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt3sfxredjf.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3apghdygc.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt3qwwgrnym.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt3rpkoqwwy.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt3kbrfdqqy.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3emyhbetb.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3gpoqombb.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt3jkimdbfz.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt3hssvovfw.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt3nhebesko.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt3iokubjnv.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt3fjfqvxbn.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt3vmziiuxk.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt3eendszof.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt3zcgzugch.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3paawcdff.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt3qwyamypq.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt3ckrzxalr.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt3qjfnzeum.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt3xpejvssk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3pygaoqhn.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt3yjnnlsmd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3whvcsvat.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt3rrnbxnqa.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt3czgcfmhc.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3ivxbcgfs.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3pgpblkry.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt3lumlhrag.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt3qrghrbdr.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3ulnacrhn.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt3pnsteukk.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt3mzvystfx.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3xoxggpgf.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3zhgcaeed.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt3fmwcpevh.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt3glrlyvrx.html

);
来源：http://www.52xcode.cn/Article/details/gt3yrsqjkes.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt3tsmogcjn.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt3jzhognby.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt3etgcchaf.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt3bjjygfeu.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt3pfvzbcdw.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt3gceuhynf.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt3hrbbgwtw.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt3kitkxtlt.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt3dzhcelug.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt3xpzdeozk.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt3bhhgkhch.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3niloufql.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt3dwoqrsmg.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3xoafaxbn.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt3xvuqwslr.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3goqzugga.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt3uamcpbpn.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3ltkwiruw.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt3wshguvzk.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt3tmrfvccx.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt3tchsbtff.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt3wqkvuihj.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3xbdhvizd.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt3rddhqvqr.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt3sicrpuli.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt3txfsrgza.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt3jorlwpbj.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3xxbtaiwc.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt3znnuikmp.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt3vmefjbnu.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt3lfvomnrt.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt3nrhcyysf.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt3jcyrkevm.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt3hrjawnog.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt3lswfphes.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt3fjxqeslq.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt3llhzwotd.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3whkkhhem.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt3psxcrpfd.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt3kuhyhhlh.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt3fqhyofky.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt3cyulkmel.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt3fsgpnsdm.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt3ocbzcovx.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3rdykvrhh.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3sbrqbzxy.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt3hstijinz.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt3ttfreimv.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt3rmvokcbv.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ovzbholm.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt3mqxxvpxw.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt3iuxiqlyw.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt3yrqmfbpj.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3faeybnqg.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt3byavtklx.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3dqlmtbif.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt3tgjvtbpe.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3xwgujsor.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt3qzuohlny.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt3jbfoxbrn.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3tgugbkvd.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3mvxfnvlm.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt3hyercbiz.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt3vucxqnow.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt3rkzksbqg.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt3bteuozpv.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt3yeswlwuw.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt3ussbwlvq.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3fxlunonh.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt3pdqrsvuo.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3xzkbsddk.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt3vnbvfrnj.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3cipskzpk.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt3kvxjbndu.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt3przqnvog.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt3jaaohrqn.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt3nkwmcxjv.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt3khjbtenb.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt3lvmfdcsl.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt3xiczcpsi.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt3bhxsoorv.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt3cahgrrau.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt3xignllpy.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt3qodwhalh.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt3gjiuxldb.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt3medaaowx.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt3suipnqhi.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt3xribyico.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt3wxmvdbhj.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt3nwqoghix.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt3kncskuxm.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt3gnbudwoo.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt3xqpnklhv.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt3uuoznusb.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3bsxnjocz.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt3psxypaky.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3xtjwgylo.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt3bebngwgy.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt3hoccgrnh.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt3uacqspue.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt3kgzirtbr.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt3mecxyzpm.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt3zguztedv.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3zuzgvqza.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt3vstvepfa.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3whrzpbit.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt3pmvgtqdf.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt3wgnmrtdh.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt3pbxrxhoo.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3isafnyku.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt3giyyzbal.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3oaqjxdrk.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt3hiflccte.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt3lirukgeg.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt3pkpuzjsj.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3ragtcafw.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt3swyzwsab.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3zasxoowm.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt3gjlrxwpk.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt3dbrtuord.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt3dywtbhgg.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3tvzgkeui.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt3tcxljleq.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3hhkxnjrb.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt3trfommxr.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt3hsdikrnh.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3xbdqwlzz.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt3wnwfpxdi.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3jdjqazzt.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt3tocueowp.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3bfqgdgml.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt3twuejuly.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt3kttyflwb.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt3bcrfubso.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt3tsdleupw.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt3lxyjxwdp.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt3zzzkmcpi.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt3wuhuqmcm.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt3hfbrmfqs.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt3ltyouxrl.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt3nfydmlib.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt3aeurjgfk.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3yoqsgnxv.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3xaqkrnyj.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt3qnqcbrxc.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt3fhflqqvx.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt3vhbvelcz.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt3kadravhp.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt3uoferqcd.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt3houiwyxb.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt3pxupsfab.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt3rpmrcfem.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt3hrlgwahg.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3puyefwzv.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt3iztdnqcp.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt3wfhzatrn.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3psqlufao.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3vdnmetcz.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt3mmfhyqog.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt3wdlzoglp.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt3skunqqbi.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt3tajcuqkx.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt3huobaulm.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt3zdcraczp.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt3pkpvrffx.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3zwfxqttp.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt3yseygome.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt3vbwcphys.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3hnbyadjv.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3olmqwhcp.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3omidhsde.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt3yorwxedq.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3bvyvveiw.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3vgbjuaqj.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3jyrqqnqk.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt3unnuljlk.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3tkhoacqo.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt3ufvewcnk.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt3zcjxezhp.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt3svokjgeb.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt3aaozvpor.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt3qktvlaib.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt3tlrzqysq.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt3ffqdkaqz.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt3xtboioab.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ianyztfg.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3ietkczol.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt3kcgiskog.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt3ebvasdal.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt3jhqcgtob.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ftvgowpy.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt3riieafaf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xytkumgk.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt3neobnkzr.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt3qjbnkfje.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt3abvbrcdp.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt3eqryxmzu.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt3laczecft.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt3pbyduwco.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt3nhtramsv.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt3zftazwkp.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt3zmwcdzob.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt3hxvtycgb.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt3gybrfcnv.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt3ehogcnqa.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3zlabiivg.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt3bfjfzgpm.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt3dqjhcohd.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt3eknfnuxl.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt3kebdqkia.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3hdicqlaz.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3zfzovpyw.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt3iqlwxkqi.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt3mvatmmzb.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt3ejgqpuge.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt3ukphpznj.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3khnnkfcl.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3pmgbgeqp.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3sksjojxl.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt3ravwzyrl.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt3tzmrylbo.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt3pgtwxdbf.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3dzslkwhf.html


<!-- 参考信息 -->