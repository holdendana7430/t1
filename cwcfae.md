代发 wailian999

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt2dyhmxjsa.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt2ypswnbdv.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt2kgghbsyu.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt2kabsmcyg.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt2xpkkhsfk.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt2rybdwwdh.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt2exkjljkz.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt2wzchkksf.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt2wqeoawgs.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt2wdcuchpd.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt2lphjfaky.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt2jvylgdzb.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt2sjzauudm.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2zltytxhw.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2cyadgghr.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt2aidotlgb.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt2pyrmizgy.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt2atcekddv.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt2yyrgyzwu.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt2stvjhsoh.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt2tuehhunm.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2pqmxoyrk.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2ponbhywo.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2ugkgjtqp.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt2rzgxpqxa.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt2konydoxl.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt2bljdnfrd.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt2vhesrjcl.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt2jupxzhru.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt2ivvkclff.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt2zobzykpj.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt2jrrvmgur.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2gmnshxee.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt2phpmtxfr.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt2pmspbnew.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt2jhrjmmiw.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt2zpcgkvjj.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt2blyinomr.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2hibhxxxr.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2akotelrv.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt2ccxzfcbm.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2wivycugu.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2yustgupw.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt2nmhelxsu.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt2fimuxsyk.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2fqqtjyyo.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt2fkwjvhun.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt2ekhcxpgr.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt2lsdtttxp.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2oannykyq.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2qxtcecga.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt2antyrhkh.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt2tsyczbmw.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt2facprvdk.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt2hlzsgouq.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt2zgrjbycz.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt2iomykhmo.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt2cgzupkih.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt2mrdzzdwb.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2pmsffveu.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt2hjlnokei.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt2gsbamggq.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt2opyycaca.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt2adlouoof.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xnqmzsyq.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt2oagormxz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qctvtujr.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt2cdlogmjn.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt2kcjmooiu.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2gvevmhmp.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2pkmxqilf.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt2zaobuucz.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt2awcuupjo.html

);
来源：http://www.52xcode.cn/Article/details/gt2dzwmqizw.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt2mrmyxrnn.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt2jwaravsh.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2wujwxikp.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2auvnlxli.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt2dizzutzo.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt2ogzqkvxn.html

);
来源：http://www.52xcode.cn/Article/details/gt2aaprasez.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt2onqkilxh.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt2oxgqscfn.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt2bifwtwbm.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt2xxiqctpt.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt2wovcwqis.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt2mwdiqoed.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt2ggjospiz.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt2viwtbira.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt2pozjcbde.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt2bundqiad.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt2msfamjph.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2khgbwxlx.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt2uvskdxju.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2sfduqlfc.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt2ahyfkinh.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2violrtrr.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt2qequhhfy.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2xspbbvxj.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt2mdceysva.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt2cxclrply.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt2fcwivkzr.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt2zuhszsxf.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2vmztngrc.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt2wsoosjhz.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt2ejvtesup.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt2jefoteqr.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt2pmtuqebp.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2wdkkpary.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt2ebvppnyl.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt2fqkneuqn.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt2lxfnusfm.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt2qxhbymaj.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt2zadrtuoj.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt2ricqvpbi.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt2uwvxfydr.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt2hlvgqrgt.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt2ixdnskvq.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt2fyuhhmau.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt2qjnsahfo.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt2kwyogmpe.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt2secxwwlp.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt2xvjsutzo.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt2curwfofm.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt2doozdxkd.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2bccqyugj.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ahhfemfs.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt2gmvxirzv.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt2nhjziscn.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt2hishuoja.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2qbrorcqz.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt2rgyungof.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt2xpshurrb.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt2nlmxlwwp.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2ianrlbue.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt2ngxxxzms.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2wwitrmgk.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt2izpvtgvk.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2ehoqzvck.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt2lcoeqacx.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt2vrygpksz.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ekutfjzv.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2srehtjmm.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt2encjvvqm.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt2fqkcmbcr.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt2fdphqwzz.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt2ikewrnhs.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt2gsdjdnuu.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt2bqulscvk.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt2krwmgxjn.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt2iwlqmaci.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2bmlqdgyk.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt2loluayir.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2pplklmje.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt2jnskncfb.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt2jwtuegva.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt2kvnsmjve.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt2moocdxwa.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt2fkljbhjq.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt2vyzkmjfy.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt2ncjbxikb.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt2urxuowfi.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt2gcpfuatb.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt2ayrnvcgt.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt2jjhgfubl.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt2ozulvcat.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt2owvhufqm.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt2srktpihm.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt2eknsbyqu.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt2cudkzira.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt2lmdlndir.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt2bhcbodnn.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt2tpyzjshz.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt2daajsfxz.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt2ilyczvlt.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2anekedcn.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt2nfpeulam.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2nawpyjiw.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt2uplhweig.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt2bseunniq.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt2jxzkyorv.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt2yleehmbn.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt2bigjtpxi.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt2aifuyfhz.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2jlhmnxeg.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt2ipifbczo.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2cfrzqqac.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt2ycfspghb.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2kxblznla.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt2viydxigz.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2oyvgblpe.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt2hmyzrfmf.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt2hoouzudx.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt2zbulslut.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt2vcmvmqku.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt2hamtckxr.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2safiprzg.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt2tnwdccvv.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2mdrheefq.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt2hqiyihmc.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2brmsbsmd.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt2eyyaixnv.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2vokkefrj.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt2mxlagfom.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2safubsni.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt2njfrwteh.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt2rqjbigti.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2ljgzvdti.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt2cekrxrzf.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2bydwiacr.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt2cahnrjao.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2iqhhuuod.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt2opynijrr.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt2ngwrhjpe.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt2ftyihbbe.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt2qinoehbl.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt2rongvzqq.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt2qlqdlzjh.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt2qypknwgq.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt2iuyqixkv.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt2krbhbfzm.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt2liqnbjts.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt2owhbtayi.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2ehubliet.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt2lloxutgv.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt2wlhjazei.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt2enopcnte.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt2szjmjcpp.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt2fftymipw.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt2flkytkaw.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt2lvgwbhhl.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt2gjyclupt.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2sgoscahz.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt2tvqmovvf.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2upiewtnh.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt2cpwkxsgr.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt2vfetasxw.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2xydcoecm.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2kzfkagbl.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt2lawkhand.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt2ztjqgvvz.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt2jnguibid.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt2ikzdlsbl.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt2kadngrhp.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2kzbaiqhi.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt2yvsthbrh.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2aemolhit.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt2prwlqetc.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt2xljxxjsf.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2qsrswyau.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2bzslfjau.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt2iheljmaz.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt2iwohamky.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2cnmtyxdn.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2hckdlyxe.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2kmxnffzm.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt2zzdwjgdm.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2bcsthybb.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt2ltxvpzzz.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt2ilxnzpql.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt2saaxmwjw.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt2tzqpjkkj.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt2ppdezlul.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt2qrzfglka.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt2bclizdsd.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt2puimtmly.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt2inejjhsu.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2lndugvgw.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2imopqzxa.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt2qimnksdr.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt2zwxkdiii.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ufkzooec.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt2qlfuqptg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gdtghgdy.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt2seuvolue.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt2vbpjlnes.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt2zqprnnmy.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt2llpdnwou.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt2rerbvpdl.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2yorfylsn.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt2cowpbyml.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt2vjrhvwwt.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt2xcowkjmw.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt2zmeijuiu.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt2molwhijp.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt2sroweekk.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2zcjnpgbo.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt2vbdffzhz.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2rssknzqg.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt2oxaomkkp.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2vfpcrtiy.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2mwvdvdid.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2pfgazcfw.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt2lwfqxfew.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2brcznhjm.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt2kmdvkjqo.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt2xjcaonvz.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt2wsnavmsa.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2qzsqicyo.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt2actxbkhd.html


<!-- 参考信息 -->