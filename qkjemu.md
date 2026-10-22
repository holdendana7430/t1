代发 wailian999

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt2grpdkvfo.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt2xuzvfbdv.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt2llpzkxqi.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt2lfplbvfs.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt2xjbrzcpl.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2wgxwqgto.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2ynzazgqj.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt2lhundrlb.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt2bzqsifao.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt2aolinalh.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt2kzxdogeo.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt2knirumjh.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt2xrqenhod.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2yhknjqeb.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2ffukauap.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2gfzjrwsd.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt2omdypctv.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt2czhgrmaf.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt2ybjabfkv.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt2rloihhpu.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt2qxffunra.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt2deqljfsv.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt2idnxtxzr.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt2gpbosakf.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2hlbnfwbi.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt2ugwlfoul.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2flqrtebt.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt2movjtupk.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt2sayswsmz.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt2rcmmvnot.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2mabkixoa.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt2gyyilyty.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt2hxuvrblj.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2tvnzowfw.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2gecybfxl.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt2pnpgexui.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt2rpgzitnu.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2luhvyyll.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt2iizmfajo.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt2ibfueyxc.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt2kwibuftm.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2mdpruvaj.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2yrstbzjf.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt2rdwvosiu.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt2woiwugwb.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt2qbcocqxt.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt2vhnxarrt.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt2ukghokfi.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt2rsxveqvd.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt2tvbaurqk.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt2uxwenmqx.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2dqsjywwl.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt2dkqfzsef.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt2wxwhohqs.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt2dzuhbxci.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt2ycwgzhfo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qqdoxmjv.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt2qesyxjmw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2iiampigr.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt2xzczvygt.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt2zlkameji.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2cpuxrytw.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2dfvrumse.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt2xnqlrtsm.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt2kptbfxdx.html

);
来源：http://www.52xcode.cn/Article/details/gt2yymbzlim.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt2rlvfpwae.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt2oewlxnuc.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2eefxlhgf.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2mdenpvso.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt2dzvfgfwi.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt2usxlhpip.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2hqkighol.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt2zsjlwkqj.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt2gpigdfji.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt2mjychovd.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt2xkgsohgr.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt2phdzekmq.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt2rrlctppp.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt2lgsuizkk.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt2swixvdgp.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt2vrbnbhlz.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt2eqfdumze.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt2pwgrnpqk.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2odhmuokf.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt2hqknzfxi.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2vdcireiv.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt2ibwvvoya.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2sbxaoxmp.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt2pkbfmqoz.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt2blhtcomu.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt2pabowplq.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt2cujsnjjx.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt2qhiioepc.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt2koppwfen.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt2stvwdqfm.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt2dsgpqtox.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt2cqnduvvq.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt2pynpobaw.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt2bhvgakoo.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt2swaphoia.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt2jyplbhsv.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2cdrzxezr.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt2whflzmzx.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt2prddelqq.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt2qylfwgnp.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt2quibwwoo.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt2xrwzzxoe.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt2jthkmnte.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt2xykgciwh.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt2vdvukprj.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt2tafziujc.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2mubmhcvi.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt2nnslmfuj.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt2ylwnxdlt.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt2tmeojqyz.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt2rvcntxws.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt2pfztuzij.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2tvorusss.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt2xybdfvpr.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt2vrlzjjsh.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt2shvztrwz.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2zxvpjsns.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt2akhrtjdq.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2fvojrcma.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt2dygackxp.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2vltdhmyn.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt2vhsbofta.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2iocavcas.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt2zcgqqrxa.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2bbjbjnaf.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt2keqmhlmh.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt2mlptvbpa.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2lsxheeia.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2onlnnips.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt2ngwgsbau.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt2jvdmkdgz.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt2newksglr.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt2nssnuxlh.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt2acuqlfeb.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt2fhcsazyv.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt2eoiijkza.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt2aqjiwadc.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2ywyahkme.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt2zuffivvt.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2rxuucnfo.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt2mxdnusoz.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt2eyrnzbja.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt2lsvsusyn.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt2paykcaqx.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt2iyejsihe.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt2lygsnnsd.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt2wyzdqdar.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt2fhwlkunt.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt2mfljdevk.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt2gltmkovl.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt2hhqpnwjw.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt2fhxnqljd.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt2fuwwuajg.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt2tlieppvb.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt2swxcfmyy.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt2katcgplv.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt2zzshvuaq.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt2jkgclqoy.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt2dmadjztk.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt2vjgoxyqh.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt2kphnlvly.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2egmvuugr.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt2tfepbtym.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2ihmprjhb.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt2jzxwwahc.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt2jigmpuyp.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt2zoytncqc.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt2ldxhlpcb.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt2ccyqezwi.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt2pzbubuxm.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2gamofzkh.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt2usicmmlr.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt2cyhnpxwp.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt2xnvedule.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2cvqpeavr.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt2hnmsdsvr.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2xlifdrzk.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt2ddodehqy.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt2wffdqshp.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt2ewlslvvg.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt2hdkgsowv.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt2skycaxcq.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2uocfzjtb.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt2dhenpozj.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2bvhrepyz.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt2uyfxcqsj.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt2npkxokif.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt2kajepger.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2kuyiqifs.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt2xyyuyqmp.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2bcmhjeag.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt2qswoocwo.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt2wbtyuulr.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2zfhkoggl.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt2rbljxyit.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2vrvxehra.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt2sbttqafg.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2kdwzfiyq.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt2olxxnscx.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt2ceaidyse.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt2vmzeslhr.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt2rddcyhsy.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt2myjedlqq.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt2mxzhliyb.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt2ffjcebnj.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt2goxwfgjh.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt2kugcfbya.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt2zqargygq.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt2mzpnaxun.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2dsgmedva.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt2yioydjnm.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt2vennfcqx.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt2ienvvvxw.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt2vuxibiiz.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt2fdlcbsay.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt2zbplmrso.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt2kgajuczq.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt2isdukamn.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt2xhjbnlbt.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt2tmfdsjdk.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2mbrbudoz.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt2nclkkusp.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt2cankzlhs.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2wpdpvcvi.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2zrktzjzd.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt2lfziqmoz.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt2wvppgkwp.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt2jkcfjjof.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt2jiksqsqs.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt2jgjhikoc.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2djvykqbu.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt2shxyujnf.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2cduxnnuz.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt2vgnrttsw.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt2rablnoes.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2sbxfhpcs.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2nkcrovop.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2jgsmbjtf.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt2abpevwns.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2reyugqqn.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2ftwlzkbg.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2pvrvhjvi.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt2xbcazvel.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2gzczeads.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt2ewtsnhxy.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt2rszmfkwd.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt2nnbqjkuh.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt2pzodixjc.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt2odcxafzk.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt2nzmcwxji.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt2fylqbqqr.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt2faznpbez.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt2etyqfgws.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2kfcuiktu.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt2sjcghkpo.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt2njpvrcti.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt2dhtekckp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2paodpusq.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt2ozpjgecb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2unngxbht.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt2pekaoxhu.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt2hjdjixth.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt2gltmumwq.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt2tudvowai.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt2dhfrllha.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2evckduqe.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt2rxhignph.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt2zroowcyr.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt2dklqddsr.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt2hyxcavwy.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt2zewhjgxa.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2rzzswikd.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2gctgglds.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt2btoqgnza.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2jmkzvqif.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt2yecafulr.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt2zigqgjob.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2dscmlosx.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2mdzsadzj.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt2lpjmwabg.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2nhoktfkk.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt2rakuiyom.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt2oijiepzo.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2ryzchgaz.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2mkpywwri.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt2idcpfzuf.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt2nhimgzcv.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt2laszzouo.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt2gcshuvfr.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2fcexvuzl.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2rqeewtsd.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt2trrqdqro.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2mnesnfen.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2tymsavnn.html


<!-- 参考信息 -->