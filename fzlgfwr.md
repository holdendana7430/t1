代发 wailian999

Ruby: Digest::SHA256.hexdigest(s)
来源：http://m.share.zdbjq.cn/Article/details/gelpatnua.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://mobile.hesvh.cn/Article/details/gnotkdxrm.sHtML

[P03] 生成短随机字符串
来源：http://mobile.zdbjq.cn/Article/details/gcupgcdwh.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://read.share.zdbjq.cn/Article/details/gulaszrfl.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.blog.zdbjq.cn/Article/details/gvyjojtlx.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.fehbvm.com/Article/details/gsfzqrojq.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.zdbjq.cn/Article/details/ggeqxcaah.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://mobile.hesvh.cn/Article/details/gvduzavxm.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://mobile.hesvh.cn/Article/details/gdylreamh.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://wap.hesvh.cn/Article/details/gcpnaoxov.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://m.share.fehbvm.com/Article/details/gttbepqqt.sHtML

[P04] 求长度
来源：http://read.share.zdbjq.cn/Article/details/gzfrctyxf.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://read.share.zdbjq.cn/Article/details/gdvmuywte.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.share.zdbjq.cn/Article/details/gewtlvkwy.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.fehbvm.com/Article/details/gmlkbefll.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.hesvh.cn/Article/details/giqmsqrdv.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.share.fehbvm.com/Article/details/gaqwdtcst.sHtML

Go:   len(arr);  len(m)
来源：http://mobile.zdbjq.cn/Article/details/gqhnqjmiu.sHtML

Ruby: x.length;  x.size
来源：http://m.share.hesvh.cn/Article/details/gregpafxb.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://wap.hesvh.cn/Article/details/gudxdihbt.sHtML

[P05] 判断两个对象内容是否相等
来源：http://blog.hesvh.cn/Article/details/gylpwhhas.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.m.share.hesvh.cn/Article/details/gjbelxbsk.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://mobile.zdbjq.cn/Article/details/gegeemyjr.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.m.share.zdbjq.cn/Article/details/guxnritxk.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://blog.fehbvm.com/Article/details/gvldtcjci.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://baike.hesvh.cn/Article/details/gcrxjuzyj.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://3g.hesvh.cn/Article/details/gwqswpocm.sHtML

Ruby: a == b
来源：http://www.share.hesvh.cn/Article/details/ghzsxbaiv.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.m.share.fehbvm.com/Article/details/gppaofcdw.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.share.zdbjq.cn/Article/details/gmyuehyra.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.m.share.fehbvm.com/Article/details/gygxbydsu.sHtML

PHP:  if (empty($x)) {}
来源：http://wap.hesvh.cn/Article/details/gantbdjrn.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://read.share.zdbjq.cn/Article/details/guaeaiktm.sHtML

TS:   if (x == null) {}
来源：http://www.share.hesvh.cn/Article/details/gtzzqcbyw.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://wap.hesvh.cn/Article/details/gialmqpkg.sHtML

Go:   if x == nil {}
来源：http://read.share.zdbjq.cn/Article/details/gyyrlseod.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://m.share.zdbjq.cn/Article/details/glnyzkueq.sHtML

C#:   if (x is null) {}
来源：http://www.share.fehbvm.com/Article/details/gcvljodiv.sHtML

[P07] 防抖与节流
来源：http://wap.fehbvm.com/Article/details/gazajmihs.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://wap.fehbvm.com/Article/details/geambcazt.sHtML

PHP:  // 手写时间戳比较
来源：http://m.share.zdbjq.cn/Article/details/gesobkgcj.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.hesvh.cn/Article/details/gidaeijal.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.zdbjq.cn/Article/details/guhhidfys.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://3g.zdbjq.cn/Article/details/gtsztuvas.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://blog.zdbjq.cn/Article/details/gezcojotr.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://3g.hesvh.cn/Article/details/gjnjrvngp.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.m.share.fehbvm.com/Article/details/gfcnyvwly.sHtML

[P08] 处理浮点精度问题
来源：http://read.share.hesvh.cn/Article/details/guqctgfkh.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://mobile.hesvh.cn/Article/details/guddflalb.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://3g.hesvh.cn/Article/details/gicityxuv.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://m.share.fehbvm.com/Article/details/ghqmviqrd.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.m.share.fehbvm.com/Article/details/gyfettyim.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.share.hesvh.cn/Article/details/gagljzptj.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://m.share.fehbvm.com/Article/details/gurmtyufn.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.m.share.zdbjq.cn/Article/details/gsdswpedg.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://read.share.zdbjq.cn/Article/details/gaxtgqwzc.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gmtaojlpg.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://mobile.zdbjq.cn/Article/details/gxpvtorqq.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gsumtxqbe.sHtML

[Q01] 创建表
来源：http://wap.fehbvm.com/Article/details/gdewevvfl.sHtML

CREATE TABLE users (
来源：http://mobile.fehbvm.com/Article/details/gbxtjepco.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.fehbvm.com/Article/details/gatfaywke.sHtML

name VARCHAR(50) NOT NULL,
来源：http://blog.fehbvm.com/Article/details/gbtsnllun.sHtML

email VARCHAR(100) UNIQUE,
来源：http://read.share.hesvh.cn/Article/details/gbusrvrfr.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.share.hesvh.cn/Article/details/gjrajjhia.sHtML

);
来源：http://www.m.share.hesvh.cn/Article/details/groepzjlo.sHtML

[Q02] 创建带外键的表
来源：http://m.share.fehbvm.com/Article/details/gnbxvytiw.sHtML

CREATE TABLE orders (
来源：http://www.m.share.hesvh.cn/Article/details/gqluzqduz.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://mobile.hesvh.cn/Article/details/goowgrypd.sHtML

user_id INT NOT NULL,
来源：http://www.blog.zdbjq.cn/Article/details/gdtwnrjrg.sHtML

amount DECIMAL(10, 2),
来源：http://www.m.share.fehbvm.com/Article/details/gikbbbkyn.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.blog.zdbjq.cn/Article/details/gxvisfqod.sHtML

);
来源：http://3g.zdbjq.cn/Article/details/gvgvssmfq.sHtML

[Q03] 增加列
来源：http://baike.hesvh.cn/Article/details/giyoipymg.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://blog.fehbvm.com/Article/details/gyhryjlka.sHtML

[Q04] 修改列类型
来源：http://www.blog.fehbvm.com/Article/details/gqcbvnhbc.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://m.share.hesvh.cn/Article/details/gzsaxpvxf.sHtML

[Q05] 重命名列
来源：http://www.m.share.zdbjq.cn/Article/details/gqtqngsin.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://read.share.hesvh.cn/Article/details/gbjyxgcag.sHtML

[Q06] 删除列
来源：http://mobile.hesvh.cn/Article/details/gkoihnhaq.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.blog.hesvh.cn/Article/details/gmnhowmln.sHtML

[Q07] 删除表
来源：http://www.m.share.zdbjq.cn/Article/details/gzbqlkiba.sHtML

DROP TABLE IF EXISTS orders;
来源：http://3g.zdbjq.cn/Article/details/giinvnqef.sHtML

[Q08] 创建普通索引
来源：http://m.share.zdbjq.cn/Article/details/glhsawkqz.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://read.share.fehbvm.com/Article/details/gnsqreulv.sHtML

[Q09] 创建唯一索引
来源：http://3g.hesvh.cn/Article/details/gazhisqvb.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://read.share.hesvh.cn/Article/details/gmvlclbyu.sHtML

[Q10] 插入单行
来源：http://wap.fehbvm.com/Article/details/gxsnqxxib.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://wap.fehbvm.com/Article/details/ggzfysdev.sHtML

[Q11] 一次插入多行
来源：http://blog.hesvh.cn/Article/details/goopqjqiq.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://wap.fehbvm.com/Article/details/gwjxmsorp.sHtML

[Q12] 插入后取自增 ID
来源：http://read.share.zdbjq.cn/Article/details/gchsnekjb.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.blog.fehbvm.com/Article/details/glqrkpnxs.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.m.share.hesvh.cn/Article/details/gyratteol.sHtML

[Q13] 忽略重复插入
来源：http://www.share.hesvh.cn/Article/details/gtiuaxiws.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.m.share.hesvh.cn/Article/details/gaqflkhio.sHtML

[Q14] 存在则更新（upsert）
来源：http://mobile.zdbjq.cn/Article/details/gulfyyrii.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://baike.fehbvm.com/Article/details/gyprwgerk.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://mobile.hesvh.cn/Article/details/gzcyalqbt.sHtML

[Q15] 查询全部
来源：http://3g.zdbjq.cn/Article/details/gmhhmgnaz.sHtML

SELECT * FROM users;
来源：http://www.share.fehbvm.com/Article/details/gteimdpqt.sHtML

[Q16] 查询指定列
来源：http://read.share.zdbjq.cn/Article/details/gvxplidnm.sHtML

SELECT id, name FROM users;
来源：http://wap.hesvh.cn/Article/details/gkgypkctt.sHtML

[Q17] 条件查询
来源：http://3g.fehbvm.com/Article/details/gthidfqch.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://m.share.fehbvm.com/Article/details/gkgrcehqm.sHtML

[Q18] 模糊匹配
来源：http://www.share.hesvh.cn/Article/details/gtfgcnpzq.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.share.zdbjq.cn/Article/details/geucekmte.sHtML

[Q19] 范围查询
来源：http://3g.fehbvm.com/Article/details/gchjntybr.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://baike.hesvh.cn/Article/details/gfzaoyvdb.sHtML

[Q20] IN 列表
来源：http://m.share.hesvh.cn/Article/details/gdziuigoi.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://read.share.fehbvm.com/Article/details/gmigfgyiz.sHtML

[Q21] 空值判断
来源：http://blog.hesvh.cn/Article/details/ghldhjqmm.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://read.share.hesvh.cn/Article/details/gqwqfkiej.sHtML

[Q22] 排序
来源：http://baike.hesvh.cn/Article/details/gvkfbijvb.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://wap.fehbvm.com/Article/details/gvntchnwd.sHtML

[Q23] 分页
来源：http://blog.fehbvm.com/Article/details/gygrogpef.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.blog.hesvh.cn/Article/details/gdrfbluuy.sHtML

[Q24] 去重
来源：http://mobile.zdbjq.cn/Article/details/gzywsfoij.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/guoeaspci.sHtML

[Q25] 只取前 N 条
来源：http://read.share.hesvh.cn/Article/details/gvgbpjszj.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.blog.hesvh.cn/Article/details/gnngpmchd.sHtML

[Q26] 计数
来源：http://wap.zdbjq.cn/Article/details/grfxqkgoz.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gvfuxfyyc.sHtML

[Q27] 条件计数
来源：http://www.share.fehbvm.com/Article/details/gjrnxaxsz.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.share.fehbvm.com/Article/details/gdenunzkc.sHtML

[Q28] 求和与平均
来源：http://www.share.fehbvm.com/Article/details/gponkarpw.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://mobile.hesvh.cn/Article/details/gcthzarik.sHtML

[Q29] 最大最小值
来源：http://read.share.zdbjq.cn/Article/details/gmqrxyapd.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://3g.hesvh.cn/Article/details/goqteijkx.sHtML

[Q30] 分组统计
来源：http://baike.zdbjq.cn/Article/details/gbpotkebo.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://3g.fehbvm.com/Article/details/gpphhdpse.sHtML

[Q31] 分组后过滤
来源：http://read.share.fehbvm.com/Article/details/gpwuihmyl.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://wap.fehbvm.com/Article/details/gffnzqleq.sHtML

[Q32] 分组拼接字符串
来源：http://3g.hesvh.cn/Article/details/gjxrsavro.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://m.share.fehbvm.com/Article/details/givvtaxfo.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://mobile.zdbjq.cn/Article/details/gsfjowpyb.sHtML

[Q33] 多列分组
来源：http://3g.zdbjq.cn/Article/details/gnsdoixbd.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.blog.hesvh.cn/Article/details/ghbozjagl.sHtML

[Q34] 每组取第一条
来源：http://mobile.hesvh.cn/Article/details/ggdvmhsjb.sHtML

SELECT * FROM (
来源：http://read.share.hesvh.cn/Article/details/gnuxqmget.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://3g.zdbjq.cn/Article/details/gacgpzugm.sHtML

) t WHERE rn = 1;
来源：http://www.m.share.hesvh.cn/Article/details/gnahrtjol.sHtML

[Q35] 内连接
来源：http://www.share.hesvh.cn/Article/details/gzaeqnlgp.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://m.share.zdbjq.cn/Article/details/gqtfsxylo.sHtML

[Q36] 左连接
来源：http://baike.hesvh.cn/Article/details/gabxazlmr.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.share.hesvh.cn/Article/details/glnksccpw.sHtML

[Q37] 右连接
来源：http://m.share.fehbvm.com/Article/details/gjynifpan.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://m.share.zdbjq.cn/Article/details/ghgzslwxs.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://mobile.fehbvm.com/Article/details/gcebcstuj.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://wap.zdbjq.cn/Article/details/gukeyshwm.sHtML

[Q39] 自连接（查上下级）
来源：http://wap.hesvh.cn/Article/details/gnmxzeacg.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://wap.fehbvm.com/Article/details/gliyaechk.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.blog.fehbvm.com/Article/details/grjugilvn.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://blog.zdbjq.cn/Article/details/gtbnhynut.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://baike.hesvh.cn/Article/details/gkogklpdq.sHtML

[Q41] 多表连接
来源：http://3g.hesvh.cn/Article/details/glevxwmeq.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.blog.hesvh.cn/Article/details/gorqfmxqs.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.m.share.hesvh.cn/Article/details/goxjgltrx.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://m.share.hesvh.cn/Article/details/gmyuaklqy.sHtML

[Q42] 连接条件附加过滤
来源：http://www.share.hesvh.cn/Article/details/gkkrendfo.sHtML

SELECT u.name, o.amount FROM users u
来源：http://wap.zdbjq.cn/Article/details/gtpglfjsx.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://wap.zdbjq.cn/Article/details/gtkdyatxn.sHtML

[Q43] 标量子查询
来源：http://www.m.share.hesvh.cn/Article/details/gafeqqnwg.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://read.share.hesvh.cn/Article/details/gescifuwy.sHtML

[Q44] IN 子查询
来源：http://read.share.zdbjq.cn/Article/details/gdekwumqe.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://m.share.fehbvm.com/Article/details/gndxfdrdo.sHtML

[Q45] EXISTS 判断存在
来源：http://baike.hesvh.cn/Article/details/gujxdujbc.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.fehbvm.com/Article/details/gavozpjic.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.blog.hesvh.cn/Article/details/gldhhkvhg.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.zdbjq.cn/Article/details/gqmhqgzzb.sHtML

[Q47] 与平均值比较
来源：http://baike.fehbvm.com/Article/details/gxwuavsmr.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.share.fehbvm.com/Article/details/gbtfxehyg.sHtML

[Q48] CTE 公用表表达式
来源：http://www.blog.hesvh.cn/Article/details/gsvwkhzsy.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.blog.fehbvm.com/Article/details/gbfuoiaca.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://m.share.fehbvm.com/Article/details/gyivxfvka.sHtML

[Q49] 更新单行
来源：http://blog.hesvh.cn/Article/details/gmbaxqpon.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://m.share.fehbvm.com/Article/details/gkngftzgi.sHtML

[Q50] 批量更新
来源：http://mobile.zdbjq.cn/Article/details/gttnjxynt.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://3g.fehbvm.com/Article/details/gqxvaxvce.sHtML

[Q51] 用子查询更新
来源：http://read.share.fehbvm.com/Article/details/gmycnhnpe.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.m.share.hesvh.cn/Article/details/gxexzqzls.sHtML

[Q52] 删除指定行
来源：http://baike.zdbjq.cn/Article/details/gozxsgpms.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.share.zdbjq.cn/Article/details/gkeumrzvi.sHtML

[Q53] 按条件删除
来源：http://www.share.zdbjq.cn/Article/details/gxswyuqwe.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.blog.fehbvm.com/Article/details/giumzcgus.sHtML

[Q54] 清空表
来源：http://baike.zdbjq.cn/Article/details/gtycvrhgr.sHtML

TRUNCATE TABLE logs;
来源：http://m.share.zdbjq.cn/Article/details/gzcztmctf.sHtML

[Q55] 排名（并列占位）
来源：http://www.m.share.hesvh.cn/Article/details/gxhraczjf.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://blog.fehbvm.com/Article/details/gboinspss.sHtML

[Q56] 密集排名（并列不占位）
来源：http://wap.hesvh.cn/Article/details/gostdgzkj.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://3g.fehbvm.com/Article/details/gxdftgcyt.sHtML

[Q57] 行号
来源：http://m.share.zdbjq.cn/Article/details/gdruqwnjt.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://3g.fehbvm.com/Article/details/ggyxwfzfy.sHtML

[Q58] 累计求和
来源：http://www.blog.zdbjq.cn/Article/details/gncrsblxd.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://baike.fehbvm.com/Article/details/gphsyfwin.sHtML

[Q59] 分组内累计
来源：http://m.share.zdbjq.cn/Article/details/gyvkkdqxj.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://mobile.fehbvm.com/Article/details/gmfkeqbde.sHtML

[Q60] 取上一行 / 下一行
来源：http://baike.fehbvm.com/Article/details/gwjwpylxe.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.blog.fehbvm.com/Article/details/gmhzhginz.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://wap.fehbvm.com/Article/details/ghvxfmkca.sHtML

[Q61] 移动平均
来源：http://read.share.zdbjq.cn/Article/details/gchbyxgyj.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://read.share.zdbjq.cn/Article/details/gidpbauye.sHtML

[Q62] 分组占比
来源：http://www.m.share.fehbvm.com/Article/details/gbxlkrgab.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://wap.zdbjq.cn/Article/details/gzbwzsvos.sHtML

[Q63] 开启事务
来源：http://www.blog.zdbjq.cn/Article/details/goypdxrob.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://read.share.hesvh.cn/Article/details/gkvlyhwup.sHtML

[Q64] 提交事务
来源：http://www.blog.zdbjq.cn/Article/details/gyidwmcpp.sHtML

COMMIT;
来源：http://blog.fehbvm.com/Article/details/gqdndhuzu.sHtML

[Q65] 回滚事务
来源：http://mobile.fehbvm.com/Article/details/ghfwopcml.sHtML

ROLLBACK;
来源：http://www.blog.zdbjq.cn/Article/details/gfeqmnqae.sHtML

[Q66] 行锁查询
来源：http://blog.fehbvm.com/Article/details/gzzavrxoo.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://wap.fehbvm.com/Article/details/giftzusgc.sHtML

[Q67] 设置隔离级别
来源：http://m.share.fehbvm.com/Article/details/gjxhovygo.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://wap.hesvh.cn/Article/details/gnkrlciuk.sHtML

[Q68] 保存点
来源：http://mobile.fehbvm.com/Article/details/gnrijoaug.sHtML

SAVEPOINT sp1;
来源：http://m.share.fehbvm.com/Article/details/gmhpdmygo.sHtML

ROLLBACK TO sp1;
来源：http://m.share.fehbvm.com/Article/details/gwgmckooy.sHtML

[Q69] 查看执行计划
来源：http://www.blog.hesvh.cn/Article/details/ghxnshcfb.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.m.share.hesvh.cn/Article/details/gltcygkbw.sHtML

[Q70] 更新统计信息
来源：http://blog.hesvh.cn/Article/details/gwjwxpldf.sHtML

ANALYZE TABLE users;
来源：http://baike.hesvh.cn/Article/details/gwqvjefxx.sHtML

[Q71] 查看建表语句
来源：http://wap.hesvh.cn/Article/details/gbvshjgnt.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.blog.hesvh.cn/Article/details/gnaknknwt.sHtML

[Q72] 查看索引
来源：http://www.m.share.fehbvm.com/Article/details/grjwtuqei.sHtML

SHOW INDEX FROM users;
来源：http://3g.hesvh.cn/Article/details/gtunsjjrt.sHtML

[Q73] 查看表状态
来源：http://www.blog.fehbvm.com/Article/details/gvfrjrmkk.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://blog.hesvh.cn/Article/details/gvfirrmtm.sHtML

[Q74] 强制使用索引
来源：http://www.m.share.fehbvm.com/Article/details/gsqiwhxwf.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.m.share.fehbvm.com/Article/details/gweptvcuk.sHtML

[Q75] 日期格式化
来源：http://m.share.hesvh.cn/Article/details/girovhsim.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.share.hesvh.cn/Article/details/gnrgtrkvk.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://m.share.zdbjq.cn/Article/details/guywoivfk.sHtML

[Q76] 按天统计
来源：http://3g.zdbjq.cn/Article/details/gjhscdsqg.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://baike.hesvh.cn/Article/details/gbrwxfjkf.sHtML

[Q77] 时间加减
来源：http://mobile.zdbjq.cn/Article/details/gvhwefbui.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://m.share.hesvh.cn/Article/details/gqfoveawr.sHtML

[Q78] 当前时间
来源：http://www.blog.fehbvm.com/Article/details/gfmxxmtpm.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://3g.zdbjq.cn/Article/details/gplqlxavx.sHtML

[Q79] 字符串拼接
来源：http://www.blog.hesvh.cn/Article/details/gttgnpsuq.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.m.share.zdbjq.cn/Article/details/gebttjhjk.sHtML

[Q80] 字符串截取
来源：http://read.share.hesvh.cn/Article/details/gsttmaizt.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://m.share.fehbvm.com/Article/details/gmblpkudb.sHtML

[Q81] 字符串替换
来源：http://www.blog.hesvh.cn/Article/details/glzpeelfm.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gvvbbhrlz.sHtML

[Q82] 字符长度与字节长度
来源：http://www.share.fehbvm.com/Article/details/gajtcmwfm.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gzwepguom.sHtML

[Q83] 大小写转换
来源：http://wap.zdbjq.cn/Article/details/gedvwcwcy.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://read.share.zdbjq.cn/Article/details/grmbricci.sHtML

[Q84] 去除首尾空格
来源：http://3g.hesvh.cn/Article/details/gjtsbbbnx.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gydnxmgvd.sHtML

[Q85] 数值取整
来源：http://m.share.zdbjq.cn/Article/details/gnxdjqzrl.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://read.share.hesvh.cn/Article/details/gmammqbza.sHtML

[Q86] 读取 JSON 字段
来源：http://wap.zdbjq.cn/Article/details/gzvednxlk.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://wap.hesvh.cn/Article/details/gianmleej.sHtML

[Q87] JSON 字段做条件
来源：http://blog.zdbjq.cn/Article/details/gphlcrbra.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.share.hesvh.cn/Article/details/gckvponzd.sHtML

[Q88] 行转列（条件聚合）
来源：http://m.share.hesvh.cn/Article/details/groedirpu.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://baike.fehbvm.com/Article/details/gkuoiputo.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://3g.fehbvm.com/Article/details/gmtjwxcoo.sHtML

[Q89] 判断表是否存在
来源：http://blog.fehbvm.com/Article/details/gdcgoljpf.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://read.share.fehbvm.com/Article/details/gfrxsdgad.sHtML

[Q90] 生成序号列
来源：http://baike.hesvh.cn/Article/details/gtahkalol.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://baike.fehbvm.com/Article/details/gjrqzujrw.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/glpfqzzzq.sHtML

R. Bash 专题
来源：http://read.share.fehbvm.com/Article/details/ghjkdqhws.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/guawllexk.sHtML

[R01] shebang 与严格模式
来源：http://baike.fehbvm.com/Article/details/gvhspwgis.sHtML

#!/usr/bin/env bash
来源：http://mobile.hesvh.cn/Article/details/gixmxqnni.sHtML

set -euo pipefail
来源：http://m.share.hesvh.cn/Article/details/gjvrxphju.sHtML

[R02] 变量赋值与使用
来源：http://3g.fehbvm.com/Article/details/guinypgra.sHtML

name="Tom"; echo "$name"
来源：http://blog.fehbvm.com/Article/details/gnkrbhfgt.sHtML

[R03] 只读变量
来源：http://m.share.hesvh.cn/Article/details/grlfnxein.sHtML

readonly PI=3.14
来源：http://baike.zdbjq.cn/Article/details/gvxtzexpt.sHtML

[R04] 位置参数
来源：http://3g.fehbvm.com/Article/details/gacncqufe.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://baike.hesvh.cn/Article/details/goxhafgca.sHtML

[R05] 参数默认值
来源：http://www.m.share.hesvh.cn/Article/details/gttecnsrg.sHtML

name="${1:-default}"
来源：http://wap.hesvh.cn/Article/details/gyzswpdvk.sHtML

[R06] 判断命令是否存在
来源：http://3g.zdbjq.cn/Article/details/ggbupvzgq.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://wap.zdbjq.cn/Article/details/gllgcgnqj.sHtML

[R07] if 判断文件
来源：http://mobile.fehbvm.com/Article/details/ghuttoxhs.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://3g.fehbvm.com/Article/details/gxdhncmdr.sHtML

[R08] 数值比较
来源：http://wap.zdbjq.cn/Article/details/gvkudmsrv.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://3g.hesvh.cn/Article/details/grespsnyn.sHtML

[R09] 字符串比较
来源：http://www.share.zdbjq.cn/Article/details/gyiwkkgsg.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://read.share.zdbjq.cn/Article/details/gncodwngz.sHtML

[R10] 正则匹配
来源：http://wap.zdbjq.cn/Article/details/gimrhsari.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.m.share.zdbjq.cn/Article/details/gojpoqiqn.sHtML

[R11] case 多分支
来源：http://www.m.share.zdbjq.cn/Article/details/gvofiaxjz.sHtML

case "$1" in
来源：http://www.blog.fehbvm.com/Article/details/gdssgbjsb.sHtML

start) echo "启动" ;;
来源：http://wap.fehbvm.com/Article/details/gfxtknxou.sHtML

stop)  echo "停止" ;;
来源：http://read.share.fehbvm.com/Article/details/glayqcmia.sHtML

*)     echo "未知命令" ;;
来源：http://m.share.hesvh.cn/Article/details/geeuelpho.sHtML

esac
来源：http://mobile.fehbvm.com/Article/details/goctnvppz.sHtML

[R12] for 遍历文件
来源：http://www.share.zdbjq.cn/Article/details/glblptwko.sHtML

for f in *.txt; do echo "$f"; done
来源：http://blog.zdbjq.cn/Article/details/gdkuahbus.sHtML

[R13] for 计数循环
来源：http://m.share.hesvh.cn/Article/details/gxangrkzh.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://m.share.fehbvm.com/Article/details/gewqffsrq.sHtML

[R14] C 风格 for
来源：http://3g.zdbjq.cn/Article/details/glojifmyx.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://mobile.hesvh.cn/Article/details/ghzvlpfam.sHtML

[R15] while 逐行读文件
来源：http://www.m.share.fehbvm.com/Article/details/gsbyuplke.sHtML


<!-- 参考信息 -->