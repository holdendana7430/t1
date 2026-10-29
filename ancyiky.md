代发 wailian999

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://mobile.fehbvm.com/Article/details/gzvztqudk.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.zdbjq.cn/Article/details/gantwgmsn.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.hesvh.cn/Article/details/gprjqgmjp.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://m.share.hesvh.cn/Article/details/gvtzlgcho.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://3g.fehbvm.com/Article/details/goapmtxtn.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://blog.fehbvm.com/Article/details/ggtjifoyk.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://read.share.hesvh.cn/Article/details/gttyddmao.sHtML

[P04] 求长度
来源：http://www.blog.fehbvm.com/Article/details/gvwiicygy.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://read.share.fehbvm.com/Article/details/gvwhzbwcb.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.hesvh.cn/Article/details/guesetnws.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.hesvh.cn/Article/details/gcqvycliu.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.fehbvm.com/Article/details/gcqtsapmj.sHtML

Java: list.size();  map.size();  s.length()
来源：http://wap.zdbjq.cn/Article/details/goejbsqhj.sHtML

Go:   len(arr);  len(m)
来源：http://3g.fehbvm.com/Article/details/gxaxoczuh.sHtML

Ruby: x.length;  x.size
来源：http://3g.hesvh.cn/Article/details/gftolapag.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://blog.hesvh.cn/Article/details/gvwoidgks.sHtML

[P05] 判断两个对象内容是否相等
来源：http://3g.hesvh.cn/Article/details/gqarkcljj.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.blog.hesvh.cn/Article/details/gzsmvoqdw.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://wap.zdbjq.cn/Article/details/gzxbliigj.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://m.share.fehbvm.com/Article/details/gnzpocqqk.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://read.share.hesvh.cn/Article/details/gvkxpukra.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://blog.fehbvm.com/Article/details/gqznwxvld.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.m.share.hesvh.cn/Article/details/gjzgbidhw.sHtML

Ruby: a == b
来源：http://wap.hesvh.cn/Article/details/ggjrofkgz.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://blog.zdbjq.cn/Article/details/gkbprjyty.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://m.share.fehbvm.com/Article/details/grjjaqjfs.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://read.share.hesvh.cn/Article/details/guqasgnny.sHtML

PHP:  if (empty($x)) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gxmgvprlt.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.blog.zdbjq.cn/Article/details/ghmbpnbfo.sHtML

TS:   if (x == null) {}
来源：http://read.share.zdbjq.cn/Article/details/gsstzhldl.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://mobile.fehbvm.com/Article/details/gqvwjwfva.sHtML

Go:   if x == nil {}
来源：http://www.m.share.zdbjq.cn/Article/details/gvsnmfbeg.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://mobile.hesvh.cn/Article/details/gepvdpcsg.sHtML

C#:   if (x is null) {}
来源：http://www.m.share.fehbvm.com/Article/details/gtfehctvn.sHtML

[P07] 防抖与节流
来源：http://www.blog.zdbjq.cn/Article/details/gzlrswmot.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://blog.hesvh.cn/Article/details/gmkrpblls.sHtML

PHP:  // 手写时间戳比较
来源：http://www.share.zdbjq.cn/Article/details/glshuuiau.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.hesvh.cn/Article/details/gukkxeirx.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.hesvh.cn/Article/details/gkylnlife.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://3g.zdbjq.cn/Article/details/gdhhaylns.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.m.share.fehbvm.com/Article/details/ghawgycyb.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://read.share.zdbjq.cn/Article/details/gojieiarl.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://wap.hesvh.cn/Article/details/gyahrmnty.sHtML

[P08] 处理浮点精度问题
来源：http://www.m.share.fehbvm.com/Article/details/gbilomfzt.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://baike.zdbjq.cn/Article/details/glyjtgzfd.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://m.share.fehbvm.com/Article/details/gvhbaqnin.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.m.share.fehbvm.com/Article/details/ghhzulsis.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.blog.zdbjq.cn/Article/details/gnlyyzcnk.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://m.share.zdbjq.cn/Article/details/gxrkwobxi.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.blog.zdbjq.cn/Article/details/gmwupymtx.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://3g.fehbvm.com/Article/details/gwypzzfwv.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://blog.fehbvm.com/Article/details/giiegkjkn.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gxjvdqkah.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.share.zdbjq.cn/Article/details/gwoqhblfn.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/ggxgtepmp.sHtML

[Q01] 创建表
来源：http://3g.fehbvm.com/Article/details/gugxdncqm.sHtML

CREATE TABLE users (
来源：http://3g.fehbvm.com/Article/details/gdanapgjl.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.hesvh.cn/Article/details/gyrvyzzzj.sHtML

name VARCHAR(50) NOT NULL,
来源：http://wap.fehbvm.com/Article/details/gypvgvsam.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.m.share.zdbjq.cn/Article/details/gypkxoano.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://3g.zdbjq.cn/Article/details/gcbxzjjto.sHtML

);
来源：http://wap.zdbjq.cn/Article/details/gdkiuxbyl.sHtML

[Q02] 创建带外键的表
来源：http://m.share.zdbjq.cn/Article/details/gxhlofnwa.sHtML

CREATE TABLE orders (
来源：http://read.share.hesvh.cn/Article/details/gkhkiqmhs.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.fehbvm.com/Article/details/giuuaektm.sHtML

user_id INT NOT NULL,
来源：http://www.blog.zdbjq.cn/Article/details/gkpsglowg.sHtML

amount DECIMAL(10, 2),
来源：http://www.share.hesvh.cn/Article/details/gelblsvhu.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://baike.zdbjq.cn/Article/details/ghvabstas.sHtML

);
来源：http://blog.hesvh.cn/Article/details/ghfngjztt.sHtML

[Q03] 增加列
来源：http://www.m.share.zdbjq.cn/Article/details/giopmwicn.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.share.hesvh.cn/Article/details/gfpxyejxk.sHtML

[Q04] 修改列类型
来源：http://read.share.zdbjq.cn/Article/details/gnsrbkhqf.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://baike.fehbvm.com/Article/details/gthinkzxt.sHtML

[Q05] 重命名列
来源：http://3g.hesvh.cn/Article/details/gimrgvqku.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://3g.fehbvm.com/Article/details/gqaecdfpz.sHtML

[Q06] 删除列
来源：http://blog.fehbvm.com/Article/details/gwomuahfw.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://wap.hesvh.cn/Article/details/gmrnyiabr.sHtML

[Q07] 删除表
来源：http://wap.zdbjq.cn/Article/details/gxkhcgigu.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.m.share.zdbjq.cn/Article/details/grblroqcz.sHtML

[Q08] 创建普通索引
来源：http://mobile.hesvh.cn/Article/details/gqjkihtij.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://blog.zdbjq.cn/Article/details/gmgsxwfoq.sHtML

[Q09] 创建唯一索引
来源：http://3g.fehbvm.com/Article/details/gnzwclwan.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://read.share.fehbvm.com/Article/details/geamumorl.sHtML

[Q10] 插入单行
来源：http://www.blog.hesvh.cn/Article/details/guxraymri.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://3g.fehbvm.com/Article/details/gdpzxbfxn.sHtML

[Q11] 一次插入多行
来源：http://www.share.hesvh.cn/Article/details/gmfenywft.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://m.share.hesvh.cn/Article/details/grlirmuzy.sHtML

[Q12] 插入后取自增 ID
来源：http://www.share.zdbjq.cn/Article/details/gzkipomec.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://m.share.fehbvm.com/Article/details/ggkyedawb.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://read.share.hesvh.cn/Article/details/gtwlgfjkz.sHtML

[Q13] 忽略重复插入
来源：http://baike.zdbjq.cn/Article/details/gqpcrvkqw.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://baike.fehbvm.com/Article/details/gmnrgjtck.sHtML

[Q14] 存在则更新（upsert）
来源：http://wap.zdbjq.cn/Article/details/gwqcfstvx.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://read.share.hesvh.cn/Article/details/giowlskuy.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.m.share.fehbvm.com/Article/details/gdnqphbza.sHtML

[Q15] 查询全部
来源：http://www.m.share.zdbjq.cn/Article/details/gijgazqil.sHtML

SELECT * FROM users;
来源：http://m.share.fehbvm.com/Article/details/gugwmuobk.sHtML

[Q16] 查询指定列
来源：http://3g.zdbjq.cn/Article/details/gtaxurxbn.sHtML

SELECT id, name FROM users;
来源：http://m.share.fehbvm.com/Article/details/gjsnapmps.sHtML

[Q17] 条件查询
来源：http://3g.hesvh.cn/Article/details/giglthlsj.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://mobile.zdbjq.cn/Article/details/gjjmpibbx.sHtML

[Q18] 模糊匹配
来源：http://www.blog.fehbvm.com/Article/details/gjwhlwefd.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://3g.hesvh.cn/Article/details/gadelkhfy.sHtML

[Q19] 范围查询
来源：http://read.share.zdbjq.cn/Article/details/goxfwzdre.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://read.share.zdbjq.cn/Article/details/ghelytqup.sHtML

[Q20] IN 列表
来源：http://m.share.hesvh.cn/Article/details/gdkxgxgqi.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://read.share.hesvh.cn/Article/details/gniyvtfvw.sHtML

[Q21] 空值判断
来源：http://baike.zdbjq.cn/Article/details/gagrkinsc.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.m.share.zdbjq.cn/Article/details/gqaeunvfc.sHtML

[Q22] 排序
来源：http://3g.hesvh.cn/Article/details/guphleyfb.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.blog.zdbjq.cn/Article/details/gpajoayow.sHtML

[Q23] 分页
来源：http://www.m.share.hesvh.cn/Article/details/gkjffdngi.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.share.fehbvm.com/Article/details/gizgexqfh.sHtML

[Q24] 去重
来源：http://mobile.zdbjq.cn/Article/details/gvmqlohfc.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gfufxqeoj.sHtML

[Q25] 只取前 N 条
来源：http://baike.fehbvm.com/Article/details/gvwrgmrkz.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.share.zdbjq.cn/Article/details/gxugtaxxp.sHtML

[Q26] 计数
来源：http://wap.zdbjq.cn/Article/details/gejokgrwv.sHtML

SELECT COUNT(*) FROM users;
来源：http://blog.zdbjq.cn/Article/details/gggteqfhh.sHtML

[Q27] 条件计数
来源：http://baike.hesvh.cn/Article/details/gonhurqcp.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.blog.hesvh.cn/Article/details/ggwqivagn.sHtML

[Q28] 求和与平均
来源：http://www.blog.zdbjq.cn/Article/details/gggjkylng.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://3g.zdbjq.cn/Article/details/garwytuvl.sHtML

[Q29] 最大最小值
来源：http://www.blog.fehbvm.com/Article/details/glwbzrodc.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/giislvtaq.sHtML

[Q30] 分组统计
来源：http://www.share.fehbvm.com/Article/details/gayuhlbpp.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://wap.hesvh.cn/Article/details/gsvwuhxfo.sHtML

[Q31] 分组后过滤
来源：http://3g.zdbjq.cn/Article/details/gktjvvtgj.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://mobile.fehbvm.com/Article/details/gnpyizufp.sHtML

[Q32] 分组拼接字符串
来源：http://read.share.fehbvm.com/Article/details/gdhohsajv.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://3g.zdbjq.cn/Article/details/gutkpqboy.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://blog.zdbjq.cn/Article/details/gygdhnojv.sHtML

[Q33] 多列分组
来源：http://blog.fehbvm.com/Article/details/gvcxvuhnh.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.blog.hesvh.cn/Article/details/gdqqlxzuc.sHtML

[Q34] 每组取第一条
来源：http://www.blog.zdbjq.cn/Article/details/gvoxxwnjz.sHtML

SELECT * FROM (
来源：http://m.share.hesvh.cn/Article/details/gqvcrxavz.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.share.zdbjq.cn/Article/details/gvragrgfq.sHtML

) t WHERE rn = 1;
来源：http://www.share.hesvh.cn/Article/details/gsasvbeik.sHtML

[Q35] 内连接
来源：http://wap.fehbvm.com/Article/details/grejmcusg.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://m.share.zdbjq.cn/Article/details/gqdqhwiit.sHtML

[Q36] 左连接
来源：http://mobile.hesvh.cn/Article/details/ghzxvbpau.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://blog.hesvh.cn/Article/details/gwykrgdbj.sHtML

[Q37] 右连接
来源：http://blog.zdbjq.cn/Article/details/gzwhucwqz.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.blog.fehbvm.com/Article/details/gljyikjig.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.blog.zdbjq.cn/Article/details/gmytzxyxs.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://mobile.zdbjq.cn/Article/details/gwlhxhomg.sHtML

[Q39] 自连接（查上下级）
来源：http://baike.hesvh.cn/Article/details/ghpsgiqnb.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://wap.zdbjq.cn/Article/details/goacusnle.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.m.share.zdbjq.cn/Article/details/geodiugne.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.blog.zdbjq.cn/Article/details/gypbwrmyk.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://3g.zdbjq.cn/Article/details/gwqgszyoo.sHtML

[Q41] 多表连接
来源：http://m.share.zdbjq.cn/Article/details/gvkkxrmia.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.share.fehbvm.com/Article/details/gilqvigtl.sHtML

JOIN users u ON u.id = o.user_id
来源：http://baike.zdbjq.cn/Article/details/gvohowemb.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://baike.hesvh.cn/Article/details/gjbhkmfsf.sHtML

[Q42] 连接条件附加过滤
来源：http://wap.fehbvm.com/Article/details/gsrojgmdd.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.m.share.fehbvm.com/Article/details/gffyjmnth.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://wap.fehbvm.com/Article/details/gwutmzusz.sHtML

[Q43] 标量子查询
来源：http://www.m.share.hesvh.cn/Article/details/gvbucbfsr.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://read.share.fehbvm.com/Article/details/gyknibivg.sHtML

[Q44] IN 子查询
来源：http://blog.fehbvm.com/Article/details/gpfxgulzx.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.blog.fehbvm.com/Article/details/gmjzcsrbt.sHtML

[Q45] EXISTS 判断存在
来源：http://mobile.hesvh.cn/Article/details/gywpzjopn.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.fehbvm.com/Article/details/gwtsozxre.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.share.fehbvm.com/Article/details/godbrskto.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.zdbjq.cn/Article/details/ggzqhksln.sHtML

[Q47] 与平均值比较
来源：http://baike.zdbjq.cn/Article/details/gtutfysfq.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.m.share.fehbvm.com/Article/details/gxdrlnccz.sHtML

[Q48] CTE 公用表表达式
来源：http://read.share.fehbvm.com/Article/details/guegiojhd.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.blog.zdbjq.cn/Article/details/gmzthbjlx.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://3g.hesvh.cn/Article/details/gkwzbjfjj.sHtML

[Q49] 更新单行
来源：http://baike.fehbvm.com/Article/details/gayhszkeo.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.blog.zdbjq.cn/Article/details/gkqrnmpaz.sHtML

[Q50] 批量更新
来源：http://www.m.share.fehbvm.com/Article/details/gqcpbihwn.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://baike.zdbjq.cn/Article/details/gojemdwye.sHtML

[Q51] 用子查询更新
来源：http://m.share.zdbjq.cn/Article/details/gejeytvuj.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://mobile.fehbvm.com/Article/details/gjqunwate.sHtML

[Q52] 删除指定行
来源：http://m.share.zdbjq.cn/Article/details/gqkgesnrg.sHtML

DELETE FROM users WHERE id = 10;
来源：http://baike.zdbjq.cn/Article/details/gydmmjhbv.sHtML

[Q53] 按条件删除
来源：http://mobile.hesvh.cn/Article/details/gjqsiohxe.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://blog.hesvh.cn/Article/details/gyuwfptnz.sHtML

[Q54] 清空表
来源：http://baike.fehbvm.com/Article/details/gwsmabqdh.sHtML

TRUNCATE TABLE logs;
来源：http://baike.zdbjq.cn/Article/details/gxkwbzvym.sHtML

[Q55] 排名（并列占位）
来源：http://www.m.share.hesvh.cn/Article/details/gcbabahcz.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://blog.hesvh.cn/Article/details/guhtzcguq.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.m.share.hesvh.cn/Article/details/gwdjrsxgo.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://m.share.zdbjq.cn/Article/details/gwuzlhlcp.sHtML

[Q57] 行号
来源：http://www.m.share.fehbvm.com/Article/details/gnrxmddad.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gwjqrahzu.sHtML

[Q58] 累计求和
来源：http://www.share.fehbvm.com/Article/details/glllntczs.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://3g.zdbjq.cn/Article/details/gpjnocjeh.sHtML

[Q59] 分组内累计
来源：http://m.share.zdbjq.cn/Article/details/gbdnqptam.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://m.share.zdbjq.cn/Article/details/gqbgwcxjx.sHtML

[Q60] 取上一行 / 下一行
来源：http://baike.hesvh.cn/Article/details/gpueezhzz.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://mobile.zdbjq.cn/Article/details/geenadynq.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://m.share.zdbjq.cn/Article/details/gzkbrpnla.sHtML

[Q61] 移动平均
来源：http://www.m.share.zdbjq.cn/Article/details/gbqmbtdxl.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.share.zdbjq.cn/Article/details/gadcimbdm.sHtML

[Q62] 分组占比
来源：http://www.m.share.fehbvm.com/Article/details/glhpdqztl.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://blog.fehbvm.com/Article/details/gsmiasddj.sHtML

[Q63] 开启事务
来源：http://blog.zdbjq.cn/Article/details/giqxdsnbp.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://mobile.fehbvm.com/Article/details/gtqbopqjz.sHtML

[Q64] 提交事务
来源：http://www.share.hesvh.cn/Article/details/gjokyddbb.sHtML

COMMIT;
来源：http://3g.hesvh.cn/Article/details/gtrimqznn.sHtML

[Q65] 回滚事务
来源：http://www.blog.fehbvm.com/Article/details/gyauxdvko.sHtML

ROLLBACK;
来源：http://m.share.zdbjq.cn/Article/details/glnriqeta.sHtML

[Q66] 行锁查询
来源：http://www.blog.fehbvm.com/Article/details/gnbuiicvc.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.m.share.zdbjq.cn/Article/details/gykvhqnjm.sHtML

[Q67] 设置隔离级别
来源：http://baike.hesvh.cn/Article/details/gqidvbzcr.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://wap.hesvh.cn/Article/details/gxwcumscw.sHtML

[Q68] 保存点
来源：http://wap.zdbjq.cn/Article/details/gzdijmvmk.sHtML

SAVEPOINT sp1;
来源：http://mobile.hesvh.cn/Article/details/ggyeiqrdq.sHtML

ROLLBACK TO sp1;
来源：http://www.share.fehbvm.com/Article/details/gzdtvmxku.sHtML

[Q69] 查看执行计划
来源：http://m.share.hesvh.cn/Article/details/gollnoujs.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.m.share.fehbvm.com/Article/details/glnwrfkyf.sHtML

[Q70] 更新统计信息
来源：http://blog.fehbvm.com/Article/details/gahjtwggb.sHtML

ANALYZE TABLE users;
来源：http://read.share.fehbvm.com/Article/details/gpcbqcicl.sHtML

[Q71] 查看建表语句
来源：http://baike.fehbvm.com/Article/details/gupizlmrx.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://baike.zdbjq.cn/Article/details/grmwlsaql.sHtML

[Q72] 查看索引
来源：http://m.share.hesvh.cn/Article/details/gvwtczvwo.sHtML

SHOW INDEX FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gdsrnnqnz.sHtML

[Q73] 查看表状态
来源：http://m.share.fehbvm.com/Article/details/gbtpoyqmx.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://blog.zdbjq.cn/Article/details/ggonniiia.sHtML

[Q74] 强制使用索引
来源：http://www.share.hesvh.cn/Article/details/gjdreflup.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://3g.zdbjq.cn/Article/details/ggtrmmdxi.sHtML

[Q75] 日期格式化
来源：http://read.share.zdbjq.cn/Article/details/gpxkcyony.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://read.share.hesvh.cn/Article/details/gtkpwxlyn.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.m.share.hesvh.cn/Article/details/gtbwkkuxa.sHtML

[Q76] 按天统计
来源：http://m.share.fehbvm.com/Article/details/grnkwolys.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.share.fehbvm.com/Article/details/gqzkgghim.sHtML

[Q77] 时间加减
来源：http://www.share.fehbvm.com/Article/details/gvrclysby.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://wap.zdbjq.cn/Article/details/gfvdrqage.sHtML

[Q78] 当前时间
来源：http://www.share.fehbvm.com/Article/details/goyzsfyhk.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://3g.zdbjq.cn/Article/details/gkrrocijq.sHtML

[Q79] 字符串拼接
来源：http://m.share.hesvh.cn/Article/details/gsaqwpwff.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.m.share.hesvh.cn/Article/details/gryprgwyb.sHtML

[Q80] 字符串截取
来源：http://wap.hesvh.cn/Article/details/ggbdnrfap.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://m.share.fehbvm.com/Article/details/gwozcdjnq.sHtML

[Q81] 字符串替换
来源：http://www.blog.fehbvm.com/Article/details/gvxmzcaha.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://mobile.zdbjq.cn/Article/details/ggzjjttkp.sHtML

[Q82] 字符长度与字节长度
来源：http://wap.fehbvm.com/Article/details/gjjzijhnl.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://3g.fehbvm.com/Article/details/gqytfmfki.sHtML

[Q83] 大小写转换
来源：http://baike.fehbvm.com/Article/details/gjlwecwpa.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://baike.zdbjq.cn/Article/details/gyslqahwt.sHtML

[Q84] 去除首尾空格
来源：http://read.share.zdbjq.cn/Article/details/gngxostot.sHtML

SELECT TRIM(name) FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gamjepfoa.sHtML

[Q85] 数值取整
来源：http://wap.hesvh.cn/Article/details/gmqnfwwot.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.blog.fehbvm.com/Article/details/gnfhovzak.sHtML

[Q86] 读取 JSON 字段
来源：http://www.m.share.fehbvm.com/Article/details/gnjcayioi.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.blog.fehbvm.com/Article/details/gqrrwzhfl.sHtML

[Q87] JSON 字段做条件
来源：http://m.share.hesvh.cn/Article/details/gqlncbbel.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://3g.hesvh.cn/Article/details/gpznpvems.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.m.share.zdbjq.cn/Article/details/glyadlwwd.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://mobile.hesvh.cn/Article/details/gbozusrfn.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://mobile.fehbvm.com/Article/details/gbhpalthc.sHtML

[Q89] 判断表是否存在
来源：http://www.m.share.fehbvm.com/Article/details/gwtyfjiuo.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://m.share.fehbvm.com/Article/details/gnteocozs.sHtML

[Q90] 生成序号列
来源：http://baike.fehbvm.com/Article/details/gdxmvkimx.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://mobile.zdbjq.cn/Article/details/gjgmogvxu.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gfzinfnay.sHtML

R. Bash 专题
来源：http://www.blog.fehbvm.com/Article/details/gadlbvxof.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gevnfmgkd.sHtML

[R01] shebang 与严格模式
来源：http://read.share.hesvh.cn/Article/details/gkpfnyepy.sHtML

#!/usr/bin/env bash
来源：http://mobile.zdbjq.cn/Article/details/gvifsyrhd.sHtML

set -euo pipefail
来源：http://3g.fehbvm.com/Article/details/gebbzfzyg.sHtML

[R02] 变量赋值与使用
来源：http://www.share.zdbjq.cn/Article/details/guauovtmu.sHtML

name="Tom"; echo "$name"
来源：http://3g.hesvh.cn/Article/details/gdwkiscsv.sHtML

[R03] 只读变量
来源：http://www.share.hesvh.cn/Article/details/gvbvwzetl.sHtML

readonly PI=3.14
来源：http://m.share.zdbjq.cn/Article/details/gbxzhgrqq.sHtML

[R04] 位置参数
来源：http://www.blog.zdbjq.cn/Article/details/gytnxnaer.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://m.share.fehbvm.com/Article/details/goudzazmm.sHtML

[R05] 参数默认值
来源：http://www.share.zdbjq.cn/Article/details/gboqjkrlv.sHtML

name="${1:-default}"
来源：http://m.share.fehbvm.com/Article/details/gtcfuxukk.sHtML

[R06] 判断命令是否存在
来源：http://m.share.zdbjq.cn/Article/details/gkfziqvqb.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://read.share.zdbjq.cn/Article/details/gkgcibzvo.sHtML

[R07] if 判断文件
来源：http://read.share.zdbjq.cn/Article/details/gutkgxnbo.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.blog.fehbvm.com/Article/details/gdxskwhrh.sHtML

[R08] 数值比较
来源：http://www.share.hesvh.cn/Article/details/goxjfqfir.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://mobile.fehbvm.com/Article/details/glccvkfwe.sHtML

[R09] 字符串比较
来源：http://mobile.fehbvm.com/Article/details/gcrvxikka.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.blog.fehbvm.com/Article/details/guzyeysvp.sHtML

[R10] 正则匹配
来源：http://m.share.fehbvm.com/Article/details/glgubcate.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.m.share.zdbjq.cn/Article/details/gvhlaswrh.sHtML

[R11] case 多分支
来源：http://www.share.fehbvm.com/Article/details/gqikdusyc.sHtML

case "$1" in
来源：http://3g.fehbvm.com/Article/details/gynhfbulp.sHtML

start) echo "启动" ;;
来源：http://blog.zdbjq.cn/Article/details/gnsbcpalz.sHtML

stop)  echo "停止" ;;
来源：http://read.share.fehbvm.com/Article/details/gnnyddhzj.sHtML

*)     echo "未知命令" ;;
来源：http://www.blog.hesvh.cn/Article/details/ghctpxovr.sHtML

esac
来源：http://read.share.zdbjq.cn/Article/details/gymakeoya.sHtML

[R12] for 遍历文件
来源：http://baike.fehbvm.com/Article/details/gwxikblzh.sHtML

for f in *.txt; do echo "$f"; done
来源：http://m.share.fehbvm.com/Article/details/gjbmamxxb.sHtML

[R13] for 计数循环
来源：http://baike.fehbvm.com/Article/details/grzoakyca.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://blog.fehbvm.com/Article/details/gxazqpqad.sHtML

[R14] C 风格 for
来源：http://www.m.share.zdbjq.cn/Article/details/gognlkqys.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://baike.zdbjq.cn/Article/details/grvckwlkj.sHtML

[R15] while 逐行读文件
来源：http://read.share.hesvh.cn/Article/details/gvgawvrbl.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.share.fehbvm.com/Article/details/gvkszfhuo.sHtML

[R16] until 等待条件
来源：http://baike.hesvh.cn/Article/details/gdpjiuebx.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.share.hesvh.cn/Article/details/gwilgtpzf.sHtML

[R17] 数组定义与取值
来源：http://www.m.share.hesvh.cn/Article/details/gocacvenj.sHtML


<!-- 参考信息 -->