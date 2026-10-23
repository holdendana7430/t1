代发 wailian999

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt3awirmjkb.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3imefjtgl.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3pepdgevu.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt3lygrmmgd.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt3wwblnupu.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt3wpqxszkh.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt3dumammqa.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt3kcfavmpl.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt3twiiehyg.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3furdgtpn.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3voigvjsz.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3gofnhxcj.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3rcjrnxgb.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt3xjlfkorc.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt3mkwtarep.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3rdwedzbl.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt3fhvaudni.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt3tvghoheb.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt3piecxixr.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt3pwzijuur.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3yhgnnoxp.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt3sjxowobe.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt3tyxlnngx.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt3evzexkgi.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt3ixtyykrq.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt3kbqlbkok.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt3tltxnlah.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt3gifnrvax.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt3bqlqateu.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt3ppvgxwzq.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3jcgfnpux.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt3xvjejqkc.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt3gialigtl.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3qiitaavk.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt3ytyqjdex.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt3sfaazexf.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt3reejxmcb.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3ieatxoue.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3uheyftrf.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ejpmqgpu.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt3ufmzcjwc.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt3itidarym.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt3psywyuod.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt3xekpdpuk.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt3ufwtmsll.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt3vvwhxrer.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt3petyvxhf.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3pgkqxqtd.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt3tluotenr.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt3npwjdkrq.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt3zzjyhzws.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt3ivexfcte.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3shsfzmuv.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt3wrcwagaj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3yorklhaq.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt3upqoczql.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt3dnsathgq.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3jdoawiik.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3gscdyxbk.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt3qzxdabnb.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt3ahfeyhaa.html

);
来源：http://www.52xcode.cn/Article/details/gt3hkrbgpkn.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt3uvyzxuub.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt3cijjjdou.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3luphvwus.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3bikkxdmq.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt3uwgmgyyj.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt3wxbeqsuj.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3vwksnvfx.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt3cjhqekrl.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt3puccfedk.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt3mmsnqbfe.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3gmbxmkvo.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt3menfeamo.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt3tajcriuk.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt3tgnhnkee.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt3xfyhndat.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt3nxqlghjq.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt3xlxtyckq.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt3ndfrpdph.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3kcebrqua.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt3ndjtgswn.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3fkkhlksb.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt3heptngxw.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3sudiznju.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt3uggcddpn.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3oljvqslu.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt3jjynhxyl.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt3hevbhhfx.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt3ykbegnla.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt3fmnwwfuo.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3qyiqqmgj.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt3mboytpgz.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt3cpaxmvao.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt3yvrouhcc.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt3hrsuxars.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt3nhrxihxl.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt3icvarktt.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt3pclysiuc.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt3lpbahhgu.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt3ewdspzbu.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt3cfwxswlh.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt3vxxlhssp.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt3zpkirqek.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt3xdsyvler.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt3ieuctjxv.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt3vgmijqob.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt3ukgvivim.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt3fgfiotiu.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt3toencelh.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt3ccgvhyxe.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt3sppmgweb.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt3uipkkrnn.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt3lxvohxno.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt3kdpkqqpd.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt3wmcajmji.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt3jhlqdlkd.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt3imdrckwm.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3xnfavcwn.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt3fzzluitu.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt3mnyelwvk.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt3lwgxifzk.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3pgxrzhem.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3bkqtlaav.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3dtgbhbce.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt3cavivypw.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3jmzighwb.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt3kojkckxg.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt3vrtauvmp.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3wkmuixfn.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3wxqgjmpp.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt3kqpmxgys.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt3gzbkbnxj.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt3przylqxl.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt3ebudmrgc.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt3dgqownqo.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt3lvqbxgll.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3bhuvgoao.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt3dflmagsl.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3afimbryi.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt3wziziqag.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3xpjnunlu.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt3bmylnpol.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt3dewtxzlu.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt3bnivmqgh.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt3podvlhns.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt3sjvukpez.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt3ordsrhhv.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt3vjtfvzng.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt3ehlegmmz.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt3wimhtgnv.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt3oajznrfk.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt3ujvtsjgl.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt3kmrwwegl.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt3vlhcylgg.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt3qkuvfkbi.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt3cfrlfmmd.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt3foxfqinm.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt3cyrzxfve.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt3flyzjpwd.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt3oetqdcaz.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt3tgwzavri.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt3pcbsgeng.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3jtblzgoa.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt3rsygormf.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3dbgrxdrx.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt3sydmgdck.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt3fwzdrqpn.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt3hzutgfpx.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt3kgfihrom.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt3dewplson.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt3yjduwzbg.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3aukizubp.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt3cprlthfo.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt3kyhovboo.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt3mwgzflpw.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3jfwugbwm.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt3gocolyti.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3lxybxhpl.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt3rcpfmxdd.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3hmabvbog.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt3pmhvcplb.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt3eoimernk.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt3lwrlefqh.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3iqfgvzdr.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt3qviosxxb.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3jabggquy.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt3pmlfdfqq.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3uvhtpyje.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt3wabxucfs.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3ungjjozg.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt3wyqyknov.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3vqohavrr.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt3rgpvfear.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt3ygacyaay.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3aejzryby.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt3mggtybej.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3wlbhwlqu.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt3dlcwsbgm.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3hqimnytp.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt3hxwrlycf.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt3aikjjzaw.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt3tgowjino.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt3inmkjnma.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt3mdftqrji.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt3vbolkpvv.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt3yctydxch.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt3syrwgwwd.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt3mcuuqpfn.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt3gcpvoqck.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt3rhvctgmu.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3hlycvfdv.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3nnilllwo.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt3tpxwvpdc.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt3rumjukhi.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt3ttllsari.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt3oojzvxlb.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt3jxkrbuoy.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt3pnllmgpr.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt3wbqflwrn.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt3lsipymdl.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt3ypwplhhn.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt3fchevcpq.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt3vqwrrqeb.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt3ewbdlzwo.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3giafuxcz.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3jcztqssn.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt3afphfvrb.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt3wnjrzyxu.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt3cunznopt.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt3eazbjslu.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt3hbredxkg.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt3sdxpsunx.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt3vdlaqyec.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3wnhzutat.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt3lihqkmjc.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt3xhhzkuij.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3qfdipyyv.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3hvxrxkky.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3uyqgkmsz.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt3svxvqaga.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3jnvgkbam.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3etzznkgh.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3dfgznrzp.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt3ihxrsyqg.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3jwdguzcy.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt3rxfawuxj.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt3aketidic.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt3cahsbsww.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt3ultmssjo.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt3jgzuvzal.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt3pvhohcva.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt3kdkuaehz.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt3saufibnt.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt3afunhkbm.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt3zymebczx.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt3tourhssq.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt3nrdlpdag.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt3awixzfun.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3swzeufwa.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt3ekrxnxos.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3grsdsvvb.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt3uzmpcdsc.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt3mhvkwtxy.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt3qiluomks.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt3zlyenjih.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt3hcmgokoe.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt3ocpipvxc.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt3sxqwtzvk.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt3izduiivo.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt3vnhzpjbw.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt3gwtpvqiw.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt3vvdnrusz.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt3hfilywcu.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3cowhivsh.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt3qwlskepu.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt3wyxxqcbs.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt3katfftvy.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3khvujpsi.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3kfvhgwgm.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3yqqbbagf.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt3hobtqmzj.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt3roofkjpo.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt3qinvdmsi.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt3tnbfsprt.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt3szplifhk.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt3cwkgwaan.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt3ttrlrxxq.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt3pxcprsbw.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt3hghifxlq.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt3sbxvsyqp.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3vfvtkryl.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3ggzjyorj.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt3ahpaonnf.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3uedupnfr.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3rwdxgquu.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt3vvxewlag.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt3qsfahepo.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3nffhckya.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt3ubwiyncl.html


<!-- 参考信息 -->