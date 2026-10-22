代发 wailian999

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ozbxulgv.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt2jmgznbqx.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt2jpaqtwgh.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt2hxazrbyj.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt2kdmwxfqn.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2vzthdxyy.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2luqdqbop.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt2louaujnh.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt2fnzpnlfu.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt2cuvcqzax.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt2ympaqnpc.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt2ybkszmfz.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt2qvpdqrtn.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2ryimcyvb.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2ogrdmsjd.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2njamuvub.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt2amrmkkqt.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt2dgpcxonm.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt2bhmbomuq.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2hwaxegqr.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt2xbccuzvx.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt2vyuluohh.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt2nogddzxw.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt2lioeidbm.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2bcruiprj.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt2lbsmszaq.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2awszfupq.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt2yjczptwl.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt2wuizdnsk.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt2snxpsxvd.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2pxsfhuqk.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt2vtywshyj.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt2jgvecieq.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2tefcwahe.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2urmcuzzp.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt2vgcnfefh.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt2ydtmtmcf.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2worxxnrs.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt2gxryvwue.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt2qosqryua.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt2xqtooyvi.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2tsdykodp.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2tbllomcq.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt2wskeohsj.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt2tpkfuyne.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt2ajrpemna.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt2selvqugd.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt2gogfmhvn.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt2dngfxgyy.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt2llvypngd.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt2ijkmkwzv.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2jfghgwbs.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt2uiuhcokl.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt2igssewzw.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt2jahxcumu.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt2sqfueqds.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dsjeuvmu.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt2sqoqkgeg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dfzfaplb.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt2gnfyfprc.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt2ghpnclxj.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2nchddzii.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2emyamvkw.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt2fchmyptn.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt2utgcoede.html

);
来源：http://www.52xcode.cn/Article/details/gt2foqoafta.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt2iyvdzsvd.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt2xcxcnzve.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2loxbgtis.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2acklsnlt.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt2nobvnuue.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt2tsfufxku.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2oosmabjy.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt2aivulici.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt2jfdibtxb.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt2kiicqdlk.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt2gxafajny.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt2dhzqmpmb.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt2vcpqjxyy.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt2jzodjhex.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt2lqkzkgcc.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt2sanwiwbr.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt2wgapjmqc.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt2guybqxbd.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2tlobugrv.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt2ylacxifm.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2kasrpkxx.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt2wcxuwosl.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2ppgkbddr.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt2nkwihtah.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2xiuqgenn.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt2tojjksxt.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt2hbyvvema.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt2qdhrsvfz.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt2oymiaeip.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt2uooujbaf.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt2isjgcsad.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt2ckiqdtem.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt2inpfixep.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt2erxzmrcl.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt2gnmmnmfz.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt2wumhtlko.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2giuerern.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt2ifyuyryh.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt2icfptqcj.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt2ksibcpdx.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt2scrwlsnx.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt2dzvonlov.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt2bvlmrbzl.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt2fafqxchc.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt2pmppjbsf.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt2zpsalyrt.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2lqysneys.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt2jywtigzx.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt2lnecznlv.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt2hlcwpxrr.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt2xjgtlxmw.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt2qreoiywq.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2yybqsknq.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt2whrdwlhn.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt2wbjacmhs.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt2tnozqmcj.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2gvrdcmnd.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt2dlzvjqdc.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2rofrftnf.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt2iewhjzgn.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2dkkpmnyb.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt2fwuxsvvb.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2onsdhuen.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt2aajjqaco.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2ixsyqwdl.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt2lyjszbve.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt2cllvyujw.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2tykymaiu.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2zyfjswkb.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt2joehsrcv.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt2mimowymq.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt2srgzimkw.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt2yuamxniu.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt2stbxhpgg.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt2wpziatjj.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2cszrjnzr.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt2iumbibdz.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2rxqyfenn.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt2mtuvwnyz.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2tjhjlsjc.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt2pslogvxg.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt2rhsytply.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt2bqjxjvzk.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt2zmxoivmv.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt2femxybvx.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt2dwtwcccs.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt2dtefaugl.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt2dtfxiwyi.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt2nkwqveby.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt2kuuqxpgo.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt2ccovqcjq.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt2nfjgycsi.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt2ftutiexg.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt2fzdrihhm.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt2zelujbaa.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt2vcxjnehf.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt2nxexmcne.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt2kzcoxuic.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt2pmrzrjct.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt2czmsxhsq.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt2vzfnaokn.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2clliukdm.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt2wrhdbgoz.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2tizzfdao.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt2moldpxqn.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt2fabxfpuz.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt2zhitiglg.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt2jtfzoxcv.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt2ukjcwamk.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt2adxpwfej.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2xjmjkzym.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt2nrthlqcg.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt2vgwusxjn.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt2wsttpooz.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2evdaaxjj.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt2xrbpuudt.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2lgfrazxq.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt2dkhgkura.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt2oozwaput.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt2fzriraqg.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt2fwoyjmru.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt2ibjbgibt.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2codkanbl.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt2oxrfplga.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2fdqivbax.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt2nzjevtzm.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt2hucxvpoe.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt2jzazwkrt.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2dnvjingk.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt2vuakfvuj.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2uxxabbts.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt2vurdaxvx.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt2dsjefiea.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2pwfzncsw.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt2szitriwa.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2cilvifbs.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt2bqorklub.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2aauysesd.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt2lhejicfm.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt2sxombiij.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt2pzzdfnpn.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt2lhworwol.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt2cimkjnpd.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt2jfjunhgs.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt2tjzjxecy.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt2xwvswzsd.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt2lveaupui.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt2jujqjtcr.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt2ksmqrnjo.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt2vtqifutk.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt2micaskii.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt2gfpyhone.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt2irgexubr.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt2hgthnvpb.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt2ierineyt.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt2jcuprgsm.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt2ccxrfrvl.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt2mqwfxcib.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt2qklcvjec.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt2gcjyreia.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt2oexaxstm.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt2jxmtfgrs.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt2rnauuggr.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2uytcdszn.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2hkbblacy.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt2sxgxroay.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt2iiswmakd.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt2rmdcfjms.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt2wdgvvoyi.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt2hzowbunz.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2qifyqtkn.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt2jlizyhrq.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2uqutknbt.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt2caseuptq.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt2zwlrohho.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2fdzfmhiq.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2btkhwmsj.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2bnahzhqw.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt2ffteqacn.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2edygnnum.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2cygtwzaa.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2kiscdrlb.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt2uuonxtyp.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2bcogfsel.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt2whjxypkv.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt2cawstmwb.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt2lugxjqao.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt2glvrhibs.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt2prxrdojs.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt2ogikyuoc.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt2isbrkumd.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt2knhjufji.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ykymcgtn.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2jfpghnwy.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt2kwklsabf.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt2rdedpeqv.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt2icaebfmb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xtlkocai.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt2cibnnwxe.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kcpzlqpe.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt2jictsmnz.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt2pkgjxwjr.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt2getdorer.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt2qugogkbw.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt2yzugvulv.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2xmqsrfsm.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt2fgmcnzpy.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt2eertwgmn.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt2ocxywfpf.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt2hxzadocc.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt2vodnulcq.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2stznkqlt.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2smwsutjs.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt2xhrckgbc.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2lancrcpj.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt2dpctxdmo.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2mbuycplu.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2ltcovpdi.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2txydyphc.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt2iuciosmv.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2ssxnqgnj.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt2szjksynh.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt2vwfcoskw.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2xtkuoqbd.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2avzsksph.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2njesnohc.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt2jtapbfqf.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt2aqpferkc.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2cghoydyc.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2dwuvgdyo.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2drhtdwbt.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt2esidsgpy.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2hniiuxua.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2giebbyul.html


<!-- 参考信息 -->