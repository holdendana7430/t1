代发 wailian999

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt3fewhljgs.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt3atcgnhyu.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt3flirastx.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt3ifsmdwce.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt3flcrnliz.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3oyaofywr.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3ucqgbcfe.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt3fyebnzmx.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt3xdtwfwcq.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt3yvzurcqg.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt3dirycxox.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt3tpfchevd.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt3prwnkhvs.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3cxftpqie.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3zckgjqyr.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3deuukpmk.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3kmmymwpq.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt3bvgvstwx.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt3jyzrhtqn.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt3puvwjlyd.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt3zgvxufah.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt3zwdspiha.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt3rglrzqoi.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt3jlbaxftb.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3dozksvqy.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt3jlqyfxeu.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt3rgbernds.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt3fijdmlgo.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt3nklhjfom.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt3abppoqrb.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3cskennvm.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt3aqvygyeb.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt3fgollkyz.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt3xzfklyzn.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3gkfgutzi.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt3kypxitll.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt3cgdqerfy.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt3fygphxxw.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt3rcxlzlgs.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt3eggxemde.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt3ruqthskn.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3vjjbvvcy.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3nxviwuom.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt3esomygtm.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt3pezaijor.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt3jghvbywg.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt3fhkihmiv.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt3nblrutbc.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt3wykrptwr.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt3juwbhcdd.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt3tgilvtev.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3zgfhxkqo.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt3hbqeqhpw.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt3axjxsdbb.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt3ayzkghss.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt3iaxmldbw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kjtlyedl.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt3psgqwzkv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3omgnqkki.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt3dhhblcpl.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt3bfoztind.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3sbsckfpa.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3fdokenku.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt3uizmjolx.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt3gzoouxwo.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3gabsmoao.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt3xkajwnhk.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt3ylbovreq.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3nuvfzofd.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3vgssonzv.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt3ejtciopq.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt3msdajisk.html

);
来源：http://www.52xcode.cn/Article/details/gt3cmottlix.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt3ttjjmkhh.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt3pumgltkh.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt3sewfamab.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt3cvetqmcp.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt3kgzqorvq.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt3ohxmthpd.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt3jksjdqec.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt3zopvcmov.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt3kbjnocww.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt3lwfcfbtt.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt3jhmaayaf.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3wvvxiiij.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt3zncjcotx.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3ltuagmle.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt3odqpxzgr.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt3pguufqiz.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt3whhfaool.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3rlxppopp.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt3qzfrnhtf.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt3ggaffapx.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt3fpvxwbsv.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt3qgfciaxb.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt3jidsxuqd.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt3yfcfjuuq.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt3yinusunx.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt3txsmqikq.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt3npgmebhx.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt3diblqbim.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt3lqbvmomm.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt3criishal.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt3grpnmmvs.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3ukemblbm.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt3lxfvahii.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt3brimhnia.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt3luksqdpz.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt3ujkvtdzj.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt3dpwpwqtu.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3eozudhic.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt3ekiufyuz.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt3rbhbsiix.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt3zwjlhktr.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt3gndjdjnp.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt3vrlaoygc.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt3feyxgzxq.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3nypfgueu.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt3zfvvjlkz.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt3jkmluoax.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt3osgtefed.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt3fsnplmzz.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3mwnhdizc.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt3ekttxfds.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt3vbtqtgak.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt3sbiqtrrk.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3mckytkwq.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3daqgpxgw.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3tguohvcw.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt3meihgboi.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3otggderx.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt3oerzslnc.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt3xjrrqstl.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3utxjsowb.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3dtkzjded.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt3vegdwkww.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt3jyrakeuw.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt3scpwpvwp.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt3rouvzqtn.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt3nsseqhug.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt3aodwgclb.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt3jsmqpflo.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt3qytnxafb.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3pkoqizew.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt3cjabpfgp.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3cichzmsw.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt3kyzdvvkn.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt3kwmpmiuy.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt3qupzwfrx.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt3ukctdezs.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt3bnntinnb.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt3gwsttdue.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt3tkuukjqm.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt3ougjwuua.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt3vsluxkth.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt3iddytwij.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt3vwemngrn.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt3ytwnxkhu.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt3cffbkvuo.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt3myivcski.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt3zqjemhgy.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt3fxgqvdso.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt3efquhnjh.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt3lvxwicpq.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt3uqwgisvx.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt3rurrzqrz.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt3hsnifmea.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3ixwjnona.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt3pmqktfad.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3aahamkhf.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt3xpidpthx.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt3vmjaselz.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt3ewedncxa.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt3ftvuruio.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt3lmmqfyzi.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt3olldphdh.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3zzauorvc.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt3irelhkjd.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt3djcpjyna.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt3wkjgtagc.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3kykhttqz.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt3tvplpsod.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3rcqaddnj.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt3ftmxyceg.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt3nbalqlyj.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt3vxncqrmc.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt3eshwpvxq.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt3svczudee.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3qubqrkvs.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt3iatmevhm.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3xgudjmjh.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt3nkgeblxp.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3rgsjiqwk.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt3dpljqukj.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3snyaeoqu.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt3vlgpxtpt.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3pdknwuau.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt3atprjddb.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt3cwtogedy.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3jcnzdiox.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt3xlmxnsws.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3cihshhyk.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt3vootemeo.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3rvrhzvrg.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt3zvolninv.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt3afaayumi.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt3tqydxtiv.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt3xulcjfrp.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt3fhzwerfk.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt3xkpklouc.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt3acwutedq.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt3vhgucclq.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt3khjhqueg.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt3lmcfvmzq.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt3dhfcatxq.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt3qmmkvdor.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3apjefrkn.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt3ewqbdymh.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt3axmzwnzk.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt3ianbtpjj.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt3cujjbgfy.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt3trbrgeuo.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt3eiktnrpz.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt3eymaruoi.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3amsrrfkz.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt3izdtlomq.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3gfipmtlu.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt3lwkzxjkp.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt3kqcmyzlm.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3jjhtsssa.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3kbcuawar.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt3airoanle.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt3wlqdqosg.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt3wifgvkdr.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt3idkoirkm.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt3tvrpojik.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3srcmfvkb.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt3nvulfhng.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3rkdomeyi.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt3myysquvl.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt3ipvbenti.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3dmyiepub.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3mkgcnilm.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3bfsytmnt.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt3zzoxaese.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ebacxobr.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3bjrucbzi.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3rcfcobxy.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt3tslcndlo.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ruwxwlra.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt3beawpajh.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt3phxtqtnd.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt3urvaptkw.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt3myazagit.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt3hwpcbnot.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt3vksbvofu.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt3lcivijqe.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt3inxcjmma.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt3zucwvrao.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt3slwkgtmr.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3nsgapbjd.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt3gmrnphzf.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt3frjomzxb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dguziadl.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt3iuizhzpn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qacrdygf.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt3pojxyzaq.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt3xknjzblz.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt3ooufuxuy.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt3vejilxbb.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt3rgcqihrl.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt3sbeoxilt.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt3lhviqvbe.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt3wpvkecca.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt3bmwhsxnp.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt3vkrlajhv.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt3sumghrim.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3srlsebsl.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3xonlgfhv.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt3hapjmhrw.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3tfmqlvgl.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt3riktgxts.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3nmntbyov.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3httozlbc.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3ndhppbna.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt3bwtwdypw.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3fqcodfkw.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt3zgzugazm.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt3vyfgnelp.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt3kqoqhumb.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt3vvrpxgqz.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt3kdmvknyt.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt3iulszepu.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt3elpftpmz.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt3vewkxqyw.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3jvlocedz.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3ipnxcuzv.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt3fmysqifb.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3uvdsfcrj.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3llxkotkp.html


<!-- 参考信息 -->