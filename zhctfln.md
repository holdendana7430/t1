代发 wailian999

Ruby: Digest::SHA256.hexdigest(s)
来源：http://blog.zdbjq.cn/Article/details/gvmmohrbl.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://3g.hesvh.cn/Article/details/gdrmzmoop.sHtML

[P03] 生成短随机字符串
来源：http://3g.fehbvm.com/Article/details/gipnzdbwg.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://mobile.fehbvm.com/Article/details/gqibkhrqa.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.m.share.hesvh.cn/Article/details/gzipegetk.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.zdbjq.cn/Article/details/getqgsgse.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.hesvh.cn/Article/details/gsjifwgxc.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.share.zdbjq.cn/Article/details/glzvqlyxr.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.blog.zdbjq.cn/Article/details/gjiovgxpa.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://m.share.fehbvm.com/Article/details/gosgjhgfw.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://3g.fehbvm.com/Article/details/ggwjwuwcq.sHtML

[P04] 求长度
来源：http://3g.fehbvm.com/Article/details/gzkzopbjb.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://baike.fehbvm.com/Article/details/gooilgfpz.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://read.share.hesvh.cn/Article/details/ggdnfppks.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.zdbjq.cn/Article/details/gexberoaz.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.fehbvm.com/Article/details/gkdkwwamk.sHtML

Java: list.size();  map.size();  s.length()
来源：http://read.share.fehbvm.com/Article/details/gsdyecsij.sHtML

Go:   len(arr);  len(m)
来源：http://www.blog.hesvh.cn/Article/details/gxpewliiw.sHtML

Ruby: x.length;  x.size
来源：http://wap.fehbvm.com/Article/details/glpspzijp.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.m.share.hesvh.cn/Article/details/gocfwtgvu.sHtML

[P05] 判断两个对象内容是否相等
来源：http://3g.hesvh.cn/Article/details/gyfubxcnn.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.share.zdbjq.cn/Article/details/gzqoqduya.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://mobile.zdbjq.cn/Article/details/gzeynkzjs.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.blog.fehbvm.com/Article/details/gyhdodvvf.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://blog.fehbvm.com/Article/details/gsknrzhio.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://3g.zdbjq.cn/Article/details/ghqkfdnvc.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://mobile.hesvh.cn/Article/details/gqkviwjcg.sHtML

Ruby: a == b
来源：http://wap.zdbjq.cn/Article/details/gloloqljc.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.share.fehbvm.com/Article/details/gfemvglyw.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://wap.fehbvm.com/Article/details/gqfgylktt.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://3g.hesvh.cn/Article/details/germdqamp.sHtML

PHP:  if (empty($x)) {}
来源：http://www.m.share.zdbjq.cn/Article/details/guzdpsldo.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://read.share.zdbjq.cn/Article/details/gqfuytcdo.sHtML

TS:   if (x == null) {}
来源：http://mobile.fehbvm.com/Article/details/gnthrcuct.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://baike.fehbvm.com/Article/details/gwigfemyf.sHtML

Go:   if x == nil {}
来源：http://read.share.hesvh.cn/Article/details/gsetkqnco.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://mobile.zdbjq.cn/Article/details/gjmrpunbo.sHtML

C#:   if (x is null) {}
来源：http://blog.fehbvm.com/Article/details/gixsidhxp.sHtML

[P07] 防抖与节流
来源：http://www.blog.zdbjq.cn/Article/details/gsityvceu.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.m.share.fehbvm.com/Article/details/gzyowzqex.sHtML

PHP:  // 手写时间戳比较
来源：http://www.blog.hesvh.cn/Article/details/ggyfaphla.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.fehbvm.com/Article/details/goqljwydw.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.zdbjq.cn/Article/details/gpbarcrxh.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.m.share.hesvh.cn/Article/details/gwwtumkin.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://3g.hesvh.cn/Article/details/gnjrrxupx.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://blog.hesvh.cn/Article/details/gibqeicyw.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://m.share.fehbvm.com/Article/details/ggqitaulv.sHtML

[P08] 处理浮点精度问题
来源：http://mobile.zdbjq.cn/Article/details/gwudnhiiw.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://baike.hesvh.cn/Article/details/gkdubqdwl.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.m.share.zdbjq.cn/Article/details/gqplndpah.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://mobile.zdbjq.cn/Article/details/gcjcwqskv.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://blog.hesvh.cn/Article/details/gcmdbylxt.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://m.share.zdbjq.cn/Article/details/gxacdncrb.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://blog.zdbjq.cn/Article/details/gcxatxmep.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://blog.hesvh.cn/Article/details/giwrzofwd.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://baike.fehbvm.com/Article/details/gseftheaw.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gvzhqofom.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://3g.fehbvm.com/Article/details/gmydxjntj.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gxiplvayr.sHtML

[Q01] 创建表
来源：http://m.share.hesvh.cn/Article/details/gnxvfsrhi.sHtML

CREATE TABLE users (
来源：http://www.blog.hesvh.cn/Article/details/gebdvjzea.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://mobile.hesvh.cn/Article/details/gerhjwtcc.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.blog.hesvh.cn/Article/details/gyimuvngg.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.blog.hesvh.cn/Article/details/gkqchqtxj.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.m.share.zdbjq.cn/Article/details/gprlwigya.sHtML

);
来源：http://www.m.share.fehbvm.com/Article/details/gkrzxxrpu.sHtML

[Q02] 创建带外键的表
来源：http://www.m.share.fehbvm.com/Article/details/gpkxjgoxs.sHtML

CREATE TABLE orders (
来源：http://mobile.hesvh.cn/Article/details/gftgexrno.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.fehbvm.com/Article/details/ghorbulgh.sHtML

user_id INT NOT NULL,
来源：http://m.share.fehbvm.com/Article/details/giezxcjvx.sHtML

amount DECIMAL(10, 2),
来源：http://mobile.hesvh.cn/Article/details/gztqkmbck.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://3g.hesvh.cn/Article/details/gphvplden.sHtML

);
来源：http://baike.fehbvm.com/Article/details/gaxqykzex.sHtML

[Q03] 增加列
来源：http://read.share.fehbvm.com/Article/details/gusdmzgcj.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://mobile.fehbvm.com/Article/details/ggcmsdcpo.sHtML

[Q04] 修改列类型
来源：http://www.blog.hesvh.cn/Article/details/gsvnoapso.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://mobile.hesvh.cn/Article/details/gvqcpdgto.sHtML

[Q05] 重命名列
来源：http://read.share.hesvh.cn/Article/details/gpqiqevlv.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://m.share.zdbjq.cn/Article/details/gwxjsghhy.sHtML

[Q06] 删除列
来源：http://mobile.hesvh.cn/Article/details/gbxbrskly.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.blog.zdbjq.cn/Article/details/gqpliamyk.sHtML

[Q07] 删除表
来源：http://blog.zdbjq.cn/Article/details/gsoztjbes.sHtML

DROP TABLE IF EXISTS orders;
来源：http://mobile.fehbvm.com/Article/details/gaojhktaa.sHtML

[Q08] 创建普通索引
来源：http://m.share.fehbvm.com/Article/details/grdjfjtbq.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://read.share.hesvh.cn/Article/details/gernvmnki.sHtML

[Q09] 创建唯一索引
来源：http://www.m.share.hesvh.cn/Article/details/gzaujhmnr.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://mobile.zdbjq.cn/Article/details/gmgjvllsh.sHtML

[Q10] 插入单行
来源：http://m.share.hesvh.cn/Article/details/gryjszghq.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.blog.hesvh.cn/Article/details/gjkggmhuh.sHtML

[Q11] 一次插入多行
来源：http://read.share.hesvh.cn/Article/details/gcxjqamfb.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://3g.hesvh.cn/Article/details/giizqskwh.sHtML

[Q12] 插入后取自增 ID
来源：http://blog.fehbvm.com/Article/details/gvzmguhhk.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://3g.zdbjq.cn/Article/details/gkkyvptzh.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://baike.zdbjq.cn/Article/details/gowxxyatq.sHtML

[Q13] 忽略重复插入
来源：http://m.share.hesvh.cn/Article/details/gtdxzmioa.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://baike.hesvh.cn/Article/details/ghqrsdacn.sHtML

[Q14] 存在则更新（upsert）
来源：http://baike.hesvh.cn/Article/details/gitdvwgza.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.share.hesvh.cn/Article/details/gwlosbpom.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://m.share.fehbvm.com/Article/details/gxtkofrst.sHtML

[Q15] 查询全部
来源：http://mobile.fehbvm.com/Article/details/gosrxispq.sHtML

SELECT * FROM users;
来源：http://wap.zdbjq.cn/Article/details/gbnrautfv.sHtML

[Q16] 查询指定列
来源：http://3g.zdbjq.cn/Article/details/ghchqvohh.sHtML

SELECT id, name FROM users;
来源：http://blog.hesvh.cn/Article/details/gpxdefahd.sHtML

[Q17] 条件查询
来源：http://www.m.share.hesvh.cn/Article/details/ggqymlcvb.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://mobile.hesvh.cn/Article/details/ghzzaunbe.sHtML

[Q18] 模糊匹配
来源：http://blog.fehbvm.com/Article/details/gjzpzuiij.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://read.share.fehbvm.com/Article/details/gqvmqvvon.sHtML

[Q19] 范围查询
来源：http://blog.hesvh.cn/Article/details/gsvjuhfwi.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://baike.hesvh.cn/Article/details/gesxwslho.sHtML

[Q20] IN 列表
来源：http://wap.hesvh.cn/Article/details/gnlatjcaq.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://read.share.fehbvm.com/Article/details/gukvjloaz.sHtML

[Q21] 空值判断
来源：http://www.share.zdbjq.cn/Article/details/gvtaywyph.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.m.share.hesvh.cn/Article/details/gmszsbkka.sHtML

[Q22] 排序
来源：http://3g.hesvh.cn/Article/details/gpcgskath.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.share.zdbjq.cn/Article/details/gyllofxer.sHtML

[Q23] 分页
来源：http://3g.hesvh.cn/Article/details/gbbtqrhpw.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://baike.fehbvm.com/Article/details/gbmrmhygq.sHtML

[Q24] 去重
来源：http://m.share.zdbjq.cn/Article/details/gkulpsuae.sHtML

SELECT DISTINCT city FROM users;
来源：http://3g.fehbvm.com/Article/details/gwladhtxj.sHtML

[Q25] 只取前 N 条
来源：http://baike.zdbjq.cn/Article/details/gppxymwjp.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://3g.fehbvm.com/Article/details/gcmhrqamx.sHtML

[Q26] 计数
来源：http://m.share.hesvh.cn/Article/details/gayedmixu.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gkixwixmq.sHtML

[Q27] 条件计数
来源：http://mobile.hesvh.cn/Article/details/ggmvzhaii.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gvkcvuntx.sHtML

[Q28] 求和与平均
来源：http://wap.hesvh.cn/Article/details/gzvfykxgo.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://read.share.hesvh.cn/Article/details/gseecmzkp.sHtML

[Q29] 最大最小值
来源：http://baike.zdbjq.cn/Article/details/gmxhjebun.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://read.share.fehbvm.com/Article/details/gbhlnczlv.sHtML

[Q30] 分组统计
来源：http://blog.hesvh.cn/Article/details/gwsoovucl.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://m.share.hesvh.cn/Article/details/gzfobqepn.sHtML

[Q31] 分组后过滤
来源：http://www.share.fehbvm.com/Article/details/gjoexjcoj.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://baike.zdbjq.cn/Article/details/glebppzso.sHtML

[Q32] 分组拼接字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gxuudqaxl.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.share.zdbjq.cn/Article/details/gbfaffzgc.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.m.share.zdbjq.cn/Article/details/gmsbujnjy.sHtML

[Q33] 多列分组
来源：http://3g.hesvh.cn/Article/details/gexudkltd.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://blog.fehbvm.com/Article/details/guycnqesh.sHtML

[Q34] 每组取第一条
来源：http://3g.fehbvm.com/Article/details/gspusltqw.sHtML

SELECT * FROM (
来源：http://blog.hesvh.cn/Article/details/gtprvxqcm.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.m.share.fehbvm.com/Article/details/gspiohvsk.sHtML

) t WHERE rn = 1;
来源：http://www.m.share.hesvh.cn/Article/details/guyrbhdyu.sHtML

[Q35] 内连接
来源：http://3g.hesvh.cn/Article/details/gvupscwxg.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://mobile.fehbvm.com/Article/details/gceeljpbn.sHtML

[Q36] 左连接
来源：http://blog.hesvh.cn/Article/details/grzcynzva.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://mobile.hesvh.cn/Article/details/gcbgjjpzk.sHtML

[Q37] 右连接
来源：http://www.share.fehbvm.com/Article/details/grkvebzde.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://blog.zdbjq.cn/Article/details/gfdcyvdqp.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://mobile.fehbvm.com/Article/details/gtghzfmgm.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://wap.hesvh.cn/Article/details/gzxuwkjwi.sHtML

[Q39] 自连接（查上下级）
来源：http://3g.fehbvm.com/Article/details/gssrgvfsw.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://3g.hesvh.cn/Article/details/goysharfc.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://baike.zdbjq.cn/Article/details/gwmvjjold.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://mobile.hesvh.cn/Article/details/gigdpxxnp.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://blog.hesvh.cn/Article/details/gogiaotsu.sHtML

[Q41] 多表连接
来源：http://wap.zdbjq.cn/Article/details/gsvjrsumn.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://wap.zdbjq.cn/Article/details/grcthhiul.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.m.share.fehbvm.com/Article/details/gkogastom.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://baike.hesvh.cn/Article/details/gqxdhlbir.sHtML

[Q42] 连接条件附加过滤
来源：http://www.share.fehbvm.com/Article/details/gkqnwcikf.sHtML

SELECT u.name, o.amount FROM users u
来源：http://wap.hesvh.cn/Article/details/gwgqaprqq.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://baike.zdbjq.cn/Article/details/goyzioasc.sHtML

[Q43] 标量子查询
来源：http://3g.zdbjq.cn/Article/details/gsarzvchv.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://m.share.fehbvm.com/Article/details/gqjlirjip.sHtML

[Q44] IN 子查询
来源：http://m.share.zdbjq.cn/Article/details/gshxjzfaf.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://wap.hesvh.cn/Article/details/gidpyoghj.sHtML

[Q45] EXISTS 判断存在
来源：http://mobile.fehbvm.com/Article/details/gjqfgecxs.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.fehbvm.com/Article/details/guacauvrs.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.m.share.fehbvm.com/Article/details/giqlayoif.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.zdbjq.cn/Article/details/gnhochbej.sHtML

[Q47] 与平均值比较
来源：http://mobile.zdbjq.cn/Article/details/gfoyuoxsm.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.share.zdbjq.cn/Article/details/gxbcqyowz.sHtML

[Q48] CTE 公用表表达式
来源：http://m.share.zdbjq.cn/Article/details/gislgvdhh.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://blog.zdbjq.cn/Article/details/glejymhxy.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.blog.fehbvm.com/Article/details/gbbelyorc.sHtML

[Q49] 更新单行
来源：http://read.share.fehbvm.com/Article/details/gnyyjrkaq.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://blog.fehbvm.com/Article/details/gsparjffd.sHtML

[Q50] 批量更新
来源：http://www.m.share.fehbvm.com/Article/details/gpfyssytv.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.m.share.hesvh.cn/Article/details/gubqcbvxx.sHtML

[Q51] 用子查询更新
来源：http://www.m.share.zdbjq.cn/Article/details/gvvukpghe.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://3g.fehbvm.com/Article/details/gjsfppjto.sHtML

[Q52] 删除指定行
来源：http://www.share.hesvh.cn/Article/details/gjjwwrbet.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.share.zdbjq.cn/Article/details/gjllnmmxs.sHtML

[Q53] 按条件删除
来源：http://www.share.zdbjq.cn/Article/details/gvjjqogrs.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://read.share.zdbjq.cn/Article/details/gosxvvtsl.sHtML

[Q54] 清空表
来源：http://m.share.fehbvm.com/Article/details/gbhkxzubj.sHtML

TRUNCATE TABLE logs;
来源：http://wap.zdbjq.cn/Article/details/glrtouprv.sHtML

[Q55] 排名（并列占位）
来源：http://blog.zdbjq.cn/Article/details/gbuowvxuv.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://m.share.fehbvm.com/Article/details/gcljaekfm.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.share.hesvh.cn/Article/details/ggqkpbdet.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.share.fehbvm.com/Article/details/gcagmbiyp.sHtML

[Q57] 行号
来源：http://blog.hesvh.cn/Article/details/gynwukcvz.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://read.share.hesvh.cn/Article/details/gvvmssdtf.sHtML

[Q58] 累计求和
来源：http://m.share.fehbvm.com/Article/details/ghccvvqlq.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://3g.fehbvm.com/Article/details/gyzwbxnde.sHtML

[Q59] 分组内累计
来源：http://baike.zdbjq.cn/Article/details/gdzzjimhf.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://mobile.fehbvm.com/Article/details/gxbupscvs.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.blog.hesvh.cn/Article/details/gttdedeej.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://read.share.zdbjq.cn/Article/details/gfoydzqzt.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://mobile.fehbvm.com/Article/details/gcufwxyuw.sHtML

[Q61] 移动平均
来源：http://www.blog.fehbvm.com/Article/details/gcivekdxz.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://3g.hesvh.cn/Article/details/gawbzosky.sHtML

[Q62] 分组占比
来源：http://read.share.hesvh.cn/Article/details/garottabv.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://blog.hesvh.cn/Article/details/grpnayweb.sHtML

[Q63] 开启事务
来源：http://3g.zdbjq.cn/Article/details/gbbsppwfd.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://blog.zdbjq.cn/Article/details/gzysqvaqe.sHtML

[Q64] 提交事务
来源：http://www.share.fehbvm.com/Article/details/gcyhpqylu.sHtML

COMMIT;
来源：http://wap.zdbjq.cn/Article/details/gmgrzudyu.sHtML

[Q65] 回滚事务
来源：http://www.share.zdbjq.cn/Article/details/gatpqhcia.sHtML

ROLLBACK;
来源：http://baike.hesvh.cn/Article/details/ghfzpxcuq.sHtML

[Q66] 行锁查询
来源：http://blog.fehbvm.com/Article/details/gdypvaggu.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://m.share.hesvh.cn/Article/details/gdmroytwf.sHtML

[Q67] 设置隔离级别
来源：http://read.share.hesvh.cn/Article/details/gmmxixmfj.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://mobile.fehbvm.com/Article/details/gfmkvgzsg.sHtML

[Q68] 保存点
来源：http://3g.zdbjq.cn/Article/details/gzcuwgmpx.sHtML

SAVEPOINT sp1;
来源：http://www.blog.zdbjq.cn/Article/details/gvdbaokeu.sHtML

ROLLBACK TO sp1;
来源：http://www.share.fehbvm.com/Article/details/gyhhgzkww.sHtML

[Q69] 查看执行计划
来源：http://read.share.fehbvm.com/Article/details/gnqtdljnx.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.share.fehbvm.com/Article/details/gywcfklmi.sHtML

[Q70] 更新统计信息
来源：http://m.share.hesvh.cn/Article/details/gtfdehpqi.sHtML

ANALYZE TABLE users;
来源：http://m.share.fehbvm.com/Article/details/gjhemblel.sHtML

[Q71] 查看建表语句
来源：http://blog.fehbvm.com/Article/details/gmivdnlqa.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.m.share.hesvh.cn/Article/details/gbgqgphnf.sHtML

[Q72] 查看索引
来源：http://wap.fehbvm.com/Article/details/gcklxqxxj.sHtML

SHOW INDEX FROM users;
来源：http://mobile.fehbvm.com/Article/details/giawgnrji.sHtML

[Q73] 查看表状态
来源：http://read.share.zdbjq.cn/Article/details/gaxsnqbkg.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.share.zdbjq.cn/Article/details/gwsbbhrws.sHtML

[Q74] 强制使用索引
来源：http://blog.fehbvm.com/Article/details/gsssfzvex.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.m.share.zdbjq.cn/Article/details/gipchapqg.sHtML

[Q75] 日期格式化
来源：http://wap.hesvh.cn/Article/details/gsaccfrtk.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://baike.zdbjq.cn/Article/details/gwdaarmtg.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://m.share.zdbjq.cn/Article/details/gmareoysl.sHtML

[Q76] 按天统计
来源：http://m.share.fehbvm.com/Article/details/gogbrgmvo.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://3g.hesvh.cn/Article/details/gmsllwjci.sHtML

[Q77] 时间加减
来源：http://wap.hesvh.cn/Article/details/gqybybixf.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://read.share.hesvh.cn/Article/details/gzyjcvbyw.sHtML

[Q78] 当前时间
来源：http://read.share.hesvh.cn/Article/details/gvtafgmic.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://baike.zdbjq.cn/Article/details/gglghchli.sHtML

[Q79] 字符串拼接
来源：http://baike.fehbvm.com/Article/details/gqwvbnrsq.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://read.share.fehbvm.com/Article/details/gfhqrnlax.sHtML

[Q80] 字符串截取
来源：http://m.share.zdbjq.cn/Article/details/gdkrgygsb.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://blog.fehbvm.com/Article/details/gtcflecge.sHtML

[Q81] 字符串替换
来源：http://m.share.zdbjq.cn/Article/details/gtcdkrhln.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gbklclclv.sHtML

[Q82] 字符长度与字节长度
来源：http://blog.fehbvm.com/Article/details/gftghaqoa.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://baike.zdbjq.cn/Article/details/gxxpcoapl.sHtML

[Q83] 大小写转换
来源：http://m.share.hesvh.cn/Article/details/gvyqoatyo.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://wap.hesvh.cn/Article/details/gamsoocxg.sHtML

[Q84] 去除首尾空格
来源：http://baike.hesvh.cn/Article/details/gqztdckes.sHtML

SELECT TRIM(name) FROM users;
来源：http://m.share.fehbvm.com/Article/details/gaanneidr.sHtML

[Q85] 数值取整
来源：http://www.blog.fehbvm.com/Article/details/ggdyeeacp.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://read.share.fehbvm.com/Article/details/gjyevfkng.sHtML

[Q86] 读取 JSON 字段
来源：http://www.share.zdbjq.cn/Article/details/gesusdbyn.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://read.share.hesvh.cn/Article/details/gbqymojmw.sHtML

[Q87] JSON 字段做条件
来源：http://3g.fehbvm.com/Article/details/gjdlgeolr.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.m.share.fehbvm.com/Article/details/godosjlgq.sHtML

[Q88] 行转列（条件聚合）
来源：http://wap.fehbvm.com/Article/details/gidyhwniy.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://3g.zdbjq.cn/Article/details/gzlcolyvw.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://wap.hesvh.cn/Article/details/grklldeiu.sHtML

[Q89] 判断表是否存在
来源：http://m.share.fehbvm.com/Article/details/gjrpjeftw.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://baike.hesvh.cn/Article/details/gfkhdldqn.sHtML

[Q90] 生成序号列
来源：http://baike.hesvh.cn/Article/details/grqecgteg.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://3g.zdbjq.cn/Article/details/gulrfnbyn.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gpucrhvfu.sHtML

R. Bash 专题
来源：http://www.share.fehbvm.com/Article/details/gqzlzxrgr.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gdkhtpebt.sHtML

[R01] shebang 与严格模式
来源：http://www.m.share.hesvh.cn/Article/details/gkeeawhpw.sHtML

#!/usr/bin/env bash
来源：http://www.blog.zdbjq.cn/Article/details/grpjmnprs.sHtML

set -euo pipefail
来源：http://3g.zdbjq.cn/Article/details/glgzknmib.sHtML

[R02] 变量赋值与使用
来源：http://read.share.zdbjq.cn/Article/details/gvdqxoftv.sHtML

name="Tom"; echo "$name"
来源：http://read.share.fehbvm.com/Article/details/gussquyyl.sHtML

[R03] 只读变量
来源：http://wap.zdbjq.cn/Article/details/guhmkfelw.sHtML

readonly PI=3.14
来源：http://read.share.hesvh.cn/Article/details/gcvuqszsx.sHtML

[R04] 位置参数
来源：http://blog.fehbvm.com/Article/details/gzidrupxr.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://mobile.fehbvm.com/Article/details/gjadgepye.sHtML

[R05] 参数默认值
来源：http://m.share.hesvh.cn/Article/details/ggmvbvmvr.sHtML

name="${1:-default}"
来源：http://baike.fehbvm.com/Article/details/gxnrefpup.sHtML

[R06] 判断命令是否存在
来源：http://mobile.fehbvm.com/Article/details/gupvkpwib.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://baike.zdbjq.cn/Article/details/gaogozbvp.sHtML

[R07] if 判断文件
来源：http://read.share.hesvh.cn/Article/details/gjaqlhcww.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.m.share.fehbvm.com/Article/details/grcumvcmr.sHtML

[R08] 数值比较
来源：http://wap.hesvh.cn/Article/details/gtvkcasde.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.share.fehbvm.com/Article/details/ggauxucrn.sHtML

[R09] 字符串比较
来源：http://3g.zdbjq.cn/Article/details/gjfbhusek.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://3g.fehbvm.com/Article/details/gnglqcaet.sHtML

[R10] 正则匹配
来源：http://read.share.hesvh.cn/Article/details/gwvkskctk.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.blog.zdbjq.cn/Article/details/ghhogbhnw.sHtML

[R11] case 多分支
来源：http://blog.fehbvm.com/Article/details/gasulayng.sHtML

case "$1" in
来源：http://www.m.share.fehbvm.com/Article/details/gplmpqgql.sHtML

start) echo "启动" ;;
来源：http://www.share.hesvh.cn/Article/details/gvxexpvit.sHtML

stop)  echo "停止" ;;
来源：http://3g.zdbjq.cn/Article/details/gjwkueghs.sHtML

*)     echo "未知命令" ;;
来源：http://wap.fehbvm.com/Article/details/gaczltrbh.sHtML

esac
来源：http://m.share.zdbjq.cn/Article/details/gwxhodonf.sHtML

[R12] for 遍历文件
来源：http://mobile.fehbvm.com/Article/details/gjpyqonlc.sHtML

for f in *.txt; do echo "$f"; done
来源：http://mobile.fehbvm.com/Article/details/guvjvkjsn.sHtML

[R13] for 计数循环
来源：http://baike.zdbjq.cn/Article/details/gmxnfvynb.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://wap.fehbvm.com/Article/details/gzwofbrod.sHtML

[R14] C 风格 for
来源：http://m.share.fehbvm.com/Article/details/gkmckcxhs.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://mobile.hesvh.cn/Article/details/gdudawech.sHtML

[R15] while 逐行读文件
来源：http://www.m.share.fehbvm.com/Article/details/gsydtnuex.sHtML


<!-- 参考信息 -->