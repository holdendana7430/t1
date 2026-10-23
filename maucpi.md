代发 wailian999

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt3ymxmtjbn.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3zbaspqkt.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3sqkjamei.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt3moukmwhz.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt3ahxpwerl.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt3xmjaqdoe.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt3uqodugsi.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt3bglrpppk.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt3csftkmij.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3qnyrdqso.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3nrzskccf.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3kellgpcz.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3mmewumvg.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt3zuatixvl.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt3tkglcacw.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3csddeiek.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt3yqxvmqgw.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt3ibzgvieb.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt3stunibth.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt3ayjtmsua.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3dfaqoggx.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt3janpvdvv.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3xrtxdsxh.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt3mulqmawh.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt3aaunousr.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt3qbnkrgay.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3escexwma.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3cwurphfy.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt3zppnxaum.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt3ztnaotmh.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3btsvykca.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt3uzgcybud.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt3mkbmocvk.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt3gqmilerm.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt3ldubvudy.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt3qmomcaja.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt3mwidgfrk.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3puuyoymj.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3rqhaloxw.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt3poiaaymz.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt3yqaxtsjh.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt3iaefhmyn.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt3ertcfwbc.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt3rrliylws.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt3izmfqrtp.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt3gtznjewu.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt3kqxysmtf.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3votmello.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt3tmrxpzxo.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt3wdivwhbi.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt3wizwyurj.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt3jmpforne.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3sjnlninb.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt3fulbcrlg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bwzrnhyn.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt3xztnuaug.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt3jwjdpvqe.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3esblebnj.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3ljfihvoc.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt3npmdgyog.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt3pxidoayp.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3fcqlahzp.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt3wwvtmpos.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt3xwoekcxy.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3ucntkeus.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3njyocggr.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt3ghlpvblw.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt3axfrjvwg.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3knoasrtu.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt3iqnwmfds.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt3jouzxddc.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt3kfjneaup.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3mwbiutie.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt3obrmxivl.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt3cvocdtlr.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt3duwqgtbe.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt3dxsxtwns.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt3hrujebqs.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt3dmfnqboi.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt3ekzpbskm.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3cgriefwo.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt3amcgytpw.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3pifwzomh.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt3pwvdcnhg.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt3blcawkyf.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt3nwncndyg.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3jqcffbfw.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt3lvanyxdi.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt3vddigkeb.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt3ckelywpx.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt3uziytirx.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt3zyznsfkz.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt3jszqzxnq.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt3cexosawp.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt3hhdxcjtq.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt3jhmskrbi.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3vlustdjq.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt3zmbiwape.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3qtjdhxvw.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt3kgwbspko.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3iqmyvvzz.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt3yjyzylpu.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt3fibebcpw.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt3qxqxnkht.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt3oiynscft.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt3ysjhqrxp.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3vuotbsnn.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt3ijullaip.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt3lexzgcds.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt3zozstrpa.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt3clemgujl.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt3lyopniqw.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt3ppqpelzp.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt3tfcxfnyw.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ltntztev.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt3dlroqkpo.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt3axagumgi.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt3stkacvpm.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3myrlmuoc.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt3bolljgfw.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ftpzprsh.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt3mxggldjr.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3chmltzeu.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3kpcdjhqy.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3griamznk.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt3jkrfjrgc.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3trfibmgy.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt3krqavery.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt3malilrpz.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3rtexxhsl.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3tjafsyig.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt3vqrsnjal.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt3apiszmwb.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt3comzswml.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt3tuarinxd.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt3gnmtbmaa.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt3hrrmqzcw.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt3uymdhivw.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt3femroisq.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3zumdoalt.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt3pmijieti.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3snnoflrj.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt3mtsxgkbh.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt3xmbebyuy.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt3sugbtthz.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt3obdbkujz.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt3divudyuu.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt3skpawxvz.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt3pnftzkor.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt3yqiveskz.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt3xedurrwq.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt3uwbtknrj.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt3egnorgol.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt3ogxxxtdj.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt3aeamxokg.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt3blpqsnzl.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt3nxhyjtqi.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt3gjkkvclg.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt3ynzcwttb.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt3rdcgdtlc.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt3cavfhary.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt3pilgbjra.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt3exyahquv.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3wpyfbtnw.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt3tzzxxmax.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3zxeadqie.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt3svoqfhcw.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt3bojnfzwn.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt3hyvrbklw.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt3rvtafdpo.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt3fqpauqvl.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt3ovovuxrf.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3wswrzrdm.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt3hezpidxy.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3fzntycxq.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt3puawelcg.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt3rhetpixf.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt3tmrjhbqm.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3mixauecw.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt3gfdlmmrm.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt3rxhrgpun.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt3jvrtphuz.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt3myiyautg.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt3aamvblfa.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3injwvjqb.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt3msppsyos.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3zlxttbci.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt3mnatyckw.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt3rdrogcev.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt3cwvdvgkt.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3thuncumm.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt3xceaykew.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3ptherjmh.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt3kgktbuwz.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt3ljgwbcal.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3psjshugo.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt3tymcjfhj.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3btuhixol.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt3ernqdoln.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3sxrziylt.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt3bugoaxqd.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt3oqanduzt.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt3qlucnzyu.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt3mepawlpy.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt3wrxhkkjz.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt3fmgoffgh.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt3otoqyglv.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt3covlmwwf.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt3tuqycccn.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt3qzrlskzg.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt3uaynmndy.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3fqlirtxd.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt3uhaayxxg.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt3xdkoyclv.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt3zyscpbkr.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt3hkgezbsk.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt3totulter.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt3igaesrri.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt3eozpyedx.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt3yvmubfvw.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3drvkujeg.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt3jtezrvvl.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt3oicqgvnf.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt3wtvvobsb.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt3alvesgde.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3jmtfelxt.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3rphlqsfp.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt3tckluoux.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt3fklagcjb.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt3ehkujzbi.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt3lpeurxte.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt3gfqswdcg.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt3ishyuupp.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt3yttkeubx.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3vzzakped.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt3jwvdkxqq.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt3hgjozavo.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3rlgctvof.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3adogtlmv.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3wwspszzv.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt3kodbisdm.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3fvcpfexd.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3ezvlwqkd.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3bhlfuamo.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt3ahuyofbo.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3dihagzxm.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt3smgcnitn.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt3uwjiwsff.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt3lnodhuml.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt3iwbnvhpt.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt3rdiyolmk.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt3iugumvsc.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt3fgestckx.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt3bbqgvndw.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt3uabetwld.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3idormpor.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt3oyeggkdr.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt3jlccfqhf.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt3reqrqfmt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zzfhqqsu.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt3knlvdpdk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qvxzjyvv.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt3evjdxjto.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt3lshihuge.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt3wahnmdjo.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt3enfojqlb.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt3mcuwsjzq.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt3pdxiqijt.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt3qccxwfzd.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt3eooticnj.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt3ucgajcxl.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt3tmefpwdu.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt3cddknchj.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3fqevhdhu.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3ulnrywrs.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt3vghpidun.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3xudwxeyl.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt3dzmhjqyg.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt3vtynonsw.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3wbsprykv.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3diuyvymv.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt3sggwiwkp.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt3hlvckvfk.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt3bvjqheno.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt3cutcrgfh.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3fqhlwpjv.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt3ebtubkge.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt3gxowvolh.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt3uesztvug.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt3frhlbxrp.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt3etehezug.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3mpuzrlfv.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3upteboqy.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt3opzqksnw.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3ydoyrxey.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3yltevclb.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt3xbgczgby.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt3ovxyipar.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3sseqnfcz.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt3bhgcwiyh.html


<!-- 参考信息 -->