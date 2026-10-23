代发 wailian999

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt3rrqffzde.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt3oucgnqnj.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt3unckwejl.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt3jsxemkhs.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt3zvtunwzi.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3ugrggxet.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3pujqkbkz.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt3twruypig.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt3jusypckf.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt3ejaptfrj.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt3iuwmznpq.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt3wxcrnhpp.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt3ifrsoyuc.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3apnenoyw.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3hghanurh.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3gbvjvlcm.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt3yexbwpyz.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt3lufgvjby.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt3oxaupqtt.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt3kwlreqys.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt3lszfybcs.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt3psjmiqky.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt3jqzlmjkt.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt3vfsitovj.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3onlhawwd.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt3fhyyropq.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt3aedzeswz.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt3xsblangt.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt3xinihkeu.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt3drnkmcls.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt3jcztbpmy.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3hgszrqpe.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt3mhdlintx.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt3dwwmxxbu.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3igsjpxck.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt3geibpdzv.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt3chbgkxly.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3oawwqboo.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt3spkvjddc.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt3esnmqoqc.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt3oqlmxuuw.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3tmbhacpw.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3bztaggrd.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt3hmvfhyxi.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt3wsrthvgx.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt3ytqoberi.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt3owocuntp.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt3peoiundy.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt3ydylchji.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt3mahrvfwz.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt3kymepyae.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3gbwcrgwb.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt3qfrjwjiy.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt3isvrsfnq.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt3mtsrswvx.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt3ofifbcpm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kucbssgw.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt3buwpxzmq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wjernyab.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt3xyufpqrc.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt3xweahumc.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3sjdzhvdn.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3kosoktei.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt3kxnvexlx.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt3scmhltkc.html

);
来源：http://www.52xcode.cn/Article/details/gt3swjpyayk.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt3kdxwhalh.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt3dzepqirf.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3ajiigbvw.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3bnbmcrmo.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt3wfegwltw.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt3avwfxxns.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3exxyippb.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt3przgirox.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt3cibqkgke.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt3sziddzse.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3ixppafit.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt3umjnelbv.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt3nfqpdpmb.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt3gdwbysjf.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt3kyllcads.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt3zbpzybsc.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt3vppbycxc.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt3xwgbxscq.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3bjhglibp.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt3drjbfzaa.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3spjluhbw.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt3xsltnioz.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3mtzbjlaz.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt3eicoclsv.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt3ekoxsoks.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt3ogdjfqgg.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt3evodyjyq.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt3sheanxfz.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt3argjtiko.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt3yadlppgm.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt3icnlmutq.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt3wjeqzoso.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt3hycnlagy.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt3rjgssynk.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3mbfiyzqc.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt3qsmyfxrp.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3dutbrgbu.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt3hpftapsr.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt3bimrrcnl.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt3sfdycmye.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt3xvssmzmq.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt3mpvwyqgt.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt3rtcsnhtg.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt3qfiqrjcc.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3ulnhmgep.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt3igrcgtus.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3oibrgbre.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt3gaddacwe.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt3yvnxohik.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt3cvqvnxtj.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt3mcdoxnvn.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3hmugwzkl.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt3cxmsjhch.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt3fhaygqdw.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt3jdumtjdu.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt3kveiljdn.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3pvnabraa.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt3gxwhsyde.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ygodusev.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt3zyzzxuog.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3dzhuranv.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3egevqetv.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3uuanjukz.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt3aibtxyxo.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3xbgldjmt.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt3idwsfxti.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt3mgxulrry.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3uqliklns.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3ffhsdxqp.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt3icjyshen.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt3xscqoyxc.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt3vlhgbkvb.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt3vaawatvx.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt3inmsfvzj.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt3dznkqubm.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3gtfuajgw.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt3awfxwxqw.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3gjukedbk.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt3pqlipmar.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3rwocwhxe.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt3xucnmxyy.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt3sytflvlu.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt3pvqhnnhr.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt3kfzaekyl.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt3ewmrplya.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt3mymxbvdj.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt3mdjpnaxr.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt3ouujlonz.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt3isjmibph.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt3pcgidjqf.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt3glkpbgde.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt3nimbowlf.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt3oiktstvf.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt3sclzdkey.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt3cxngrbxf.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt3sztquwzo.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt3uqssldhu.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt3fadrfyws.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt3zhrqmekt.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt3utpdzsol.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt3fuefcqjv.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3attrnuti.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt3kmzrbdme.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3aufiawph.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt3gsdzdlno.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt3uxdclcvr.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt3uzclghwl.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt3olsuspjs.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt3viugtyrr.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt3fugzvkqm.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3ovudgrgf.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt3sskxzrtq.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt3rlowtpyc.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt3kyfmdpac.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt3gusfdsxa.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt3fwusrewj.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3gbqpfvho.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt3gaptolzv.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt3yzdxnctg.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt3bqcdbazl.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt3mwizwelv.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt3odjuqbjw.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3tdkgfubp.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt3bmhntqqs.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3pwswrxtc.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt3jvxgaggo.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3vgtscsbo.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt3yxnxhbpz.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3rkwkxpif.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt3swfscobk.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3gyzstqkt.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt3zpsvkxpa.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt3lorgdyrq.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3gsvuschp.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt3uedqfkhn.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3kjwlycab.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt3bdixbswy.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3tkfegpjz.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt3comzligm.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt3fmvovhrn.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt3umptlnme.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt3baiggsan.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt3kdaiqjdx.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt3ixgdpjwp.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt3phtuutwl.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt3mdnqdedh.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt3crqacfeh.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt3fvceksyl.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt3ofxdwuwu.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3yxhxvtzv.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3jzehbfij.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt3uzvyxjhg.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt3fweuxlyy.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt3uwxkscml.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt3mgqfdqai.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt3raxegvbg.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt3zvjoklfr.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt3yhcbiaym.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3dsyoiomn.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt3vrqclyiu.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt3tlezgudl.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt3vcxglhgb.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt3jdwwzhps.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3ryoprjbf.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3iucrcggs.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt3bwocijro.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt3ldbdhyyd.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt3asqtkort.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt3cdszxqxv.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt3qwpeiqpj.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt3vdbjeqjy.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt3robquglq.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3fqduvdsc.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt3prdvpzux.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt3tmsdqsju.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ioxwhtru.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3hnnqrphb.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3lgxnnwme.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt3hrczjvkv.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3gxnxhako.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3xshxhumm.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3izbemexb.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt3nznxqubj.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3sjkugkhr.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt3nzeomkko.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt3mqnpmmem.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt3ynlzihht.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt3txvgxhbb.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt3runjleod.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt3afkzgosq.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt3spjxopbo.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt3hxffbzor.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt3kolqzfwg.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3anjzycry.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3uwdjhqih.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt3bhbmujfm.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt3sjxcuyxi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3tuoovjsk.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt3koxjlqww.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3pjofqyts.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt3hfyizjwe.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt3gagmcajm.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt3bwpzpzzw.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt3rdwpvxeh.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt3khwvuqgc.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt3eperyhoc.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt3zovkjcih.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt3hsvezvju.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt3jbuohkkr.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt3onazwuac.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt3mobydtpd.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt3qswftjvo.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3tyopjmcs.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt3jhgisjwm.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt3egbvnvtf.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt3kguciznd.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt3jszztuyv.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3mbwabofn.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3aoqwutmw.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt3ubsvaskm.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3pasaszka.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt3jsjntexg.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt3gqwwtuhh.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt3mvooppsu.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt3kjxraucm.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt3ftrcftvf.html

esac
来源：http://www.52xcode.cn/Article/details/gt3uwccmgda.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt3kpfnjfld.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt3jpoiatju.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3utxddbam.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3cziqvmdv.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt3rndybyxs.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3waacjbbm.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3dncxpxcr.html


<!-- 参考信息 -->