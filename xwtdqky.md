代发 wailian999

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://m.share.hesvh.cn/Article/details/gdzulrsij.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.zdbjq.cn/Article/details/gacxmisip.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.fehbvm.com/Article/details/gmgqsnifl.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://baike.fehbvm.com/Article/details/ghdflytxr.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.m.share.hesvh.cn/Article/details/guqfosaiq.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://read.share.hesvh.cn/Article/details/ghibgrkzj.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://3g.hesvh.cn/Article/details/gmjzzqryc.sHtML

[P04] 求长度
来源：http://mobile.hesvh.cn/Article/details/gpkylymua.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://wap.hesvh.cn/Article/details/gkujoacjx.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.hesvh.cn/Article/details/gsgjvaeym.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.hesvh.cn/Article/details/gjwxjojlw.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.zdbjq.cn/Article/details/gnolehikh.sHtML

Java: list.size();  map.size();  s.length()
来源：http://read.share.fehbvm.com/Article/details/gixpfhvun.sHtML

Go:   len(arr);  len(m)
来源：http://read.share.fehbvm.com/Article/details/gwsqleova.sHtML

Ruby: x.length;  x.size
来源：http://3g.zdbjq.cn/Article/details/gycpjyelc.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://baike.zdbjq.cn/Article/details/gfnkkspic.sHtML

[P05] 判断两个对象内容是否相等
来源：http://3g.hesvh.cn/Article/details/garnozleo.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://3g.hesvh.cn/Article/details/goagzenbj.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.m.share.zdbjq.cn/Article/details/gikrasbfm.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://baike.hesvh.cn/Article/details/gjysrlqsd.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.blog.fehbvm.com/Article/details/guvpfdjgt.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.m.share.hesvh.cn/Article/details/gvjchmnmx.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://m.share.fehbvm.com/Article/details/gcnjejpus.sHtML

Ruby: a == b
来源：http://wap.zdbjq.cn/Article/details/gikmmszyo.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.blog.fehbvm.com/Article/details/gqdiqdjlf.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://m.share.fehbvm.com/Article/details/gbwqtbuyl.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://read.share.hesvh.cn/Article/details/gfktuzwcr.sHtML

PHP:  if (empty($x)) {}
来源：http://www.blog.fehbvm.com/Article/details/gxxctaciv.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.share.hesvh.cn/Article/details/geknocczn.sHtML

TS:   if (x == null) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gdegtknfa.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.m.share.hesvh.cn/Article/details/golwbjxnc.sHtML

Go:   if x == nil {}
来源：http://wap.hesvh.cn/Article/details/gndgxqczw.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://blog.zdbjq.cn/Article/details/gubfcobsk.sHtML

C#:   if (x is null) {}
来源：http://www.m.share.fehbvm.com/Article/details/gjcurobqw.sHtML

[P07] 防抖与节流
来源：http://blog.fehbvm.com/Article/details/gxzemvveq.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.share.zdbjq.cn/Article/details/gnccivqsp.sHtML

PHP:  // 手写时间戳比较
来源：http://read.share.hesvh.cn/Article/details/gfogcdgih.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.fehbvm.com/Article/details/gdtszgide.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.fehbvm.com/Article/details/gksociplz.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.blog.fehbvm.com/Article/details/gvwwtphzr.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.blog.hesvh.cn/Article/details/gfortzctw.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.m.share.fehbvm.com/Article/details/ggklyowtx.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://mobile.zdbjq.cn/Article/details/gnbzelrbj.sHtML

[P08] 处理浮点精度问题
来源：http://read.share.fehbvm.com/Article/details/gbrmdutjt.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://m.share.hesvh.cn/Article/details/gulepjtfp.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://read.share.hesvh.cn/Article/details/gskyxmbzv.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://3g.zdbjq.cn/Article/details/gnxqeshog.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://read.share.hesvh.cn/Article/details/gajrcemvc.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://m.share.fehbvm.com/Article/details/gwkkgkivg.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://m.share.zdbjq.cn/Article/details/gwrqhnadm.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.blog.fehbvm.com/Article/details/gfqpjxhet.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://baike.hesvh.cn/Article/details/gzmhuremm.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gqkrvispk.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://3g.zdbjq.cn/Article/details/geggqcudu.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gakacbwiq.sHtML

[Q01] 创建表
来源：http://blog.hesvh.cn/Article/details/gfyvpukdv.sHtML

CREATE TABLE users (
来源：http://m.share.fehbvm.com/Article/details/gvfopuetb.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.fehbvm.com/Article/details/gydnswnmp.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.blog.hesvh.cn/Article/details/ggyjmkzxu.sHtML

email VARCHAR(100) UNIQUE,
来源：http://baike.fehbvm.com/Article/details/gxhymdifu.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.blog.hesvh.cn/Article/details/gmbbycrwr.sHtML

);
来源：http://3g.fehbvm.com/Article/details/gxjqpfcze.sHtML

[Q02] 创建带外键的表
来源：http://read.share.hesvh.cn/Article/details/ghwvdrkaf.sHtML

CREATE TABLE orders (
来源：http://blog.hesvh.cn/Article/details/ggjzkuswc.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://mobile.hesvh.cn/Article/details/gqwtrcxsl.sHtML

user_id INT NOT NULL,
来源：http://www.blog.zdbjq.cn/Article/details/gepyvqmua.sHtML

amount DECIMAL(10, 2),
来源：http://baike.fehbvm.com/Article/details/gigczjbzb.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://mobile.hesvh.cn/Article/details/gazlhznea.sHtML

);
来源：http://www.m.share.hesvh.cn/Article/details/gitvdhegc.sHtML

[Q03] 增加列
来源：http://read.share.zdbjq.cn/Article/details/gyghiugnf.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://blog.fehbvm.com/Article/details/gcgzohlvp.sHtML

[Q04] 修改列类型
来源：http://blog.zdbjq.cn/Article/details/ghttlarda.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.blog.hesvh.cn/Article/details/gtrhzeobn.sHtML

[Q05] 重命名列
来源：http://www.blog.fehbvm.com/Article/details/gkyrowvtc.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.blog.zdbjq.cn/Article/details/gllqcjjzs.sHtML

[Q06] 删除列
来源：http://wap.zdbjq.cn/Article/details/gmyrxejvv.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://baike.zdbjq.cn/Article/details/gtopcfloh.sHtML

[Q07] 删除表
来源：http://3g.fehbvm.com/Article/details/gzjtotydi.sHtML

DROP TABLE IF EXISTS orders;
来源：http://mobile.hesvh.cn/Article/details/gszjebphd.sHtML

[Q08] 创建普通索引
来源：http://m.share.zdbjq.cn/Article/details/glxkmnxsu.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://m.share.hesvh.cn/Article/details/gngimeeyb.sHtML

[Q09] 创建唯一索引
来源：http://baike.hesvh.cn/Article/details/gxkgehutn.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.m.share.zdbjq.cn/Article/details/gnckmsrve.sHtML

[Q10] 插入单行
来源：http://www.blog.fehbvm.com/Article/details/gemzeczlk.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.blog.hesvh.cn/Article/details/gopknatsu.sHtML

[Q11] 一次插入多行
来源：http://blog.fehbvm.com/Article/details/gfwtnmfin.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://blog.zdbjq.cn/Article/details/ggxbotlfb.sHtML

[Q12] 插入后取自增 ID
来源：http://www.blog.hesvh.cn/Article/details/gxsctkhhg.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://wap.hesvh.cn/Article/details/gbsvgvatm.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://read.share.zdbjq.cn/Article/details/gubhurysw.sHtML

[Q13] 忽略重复插入
来源：http://3g.hesvh.cn/Article/details/gawqroaxc.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://m.share.fehbvm.com/Article/details/giaqhaosx.sHtML

[Q14] 存在则更新（upsert）
来源：http://blog.fehbvm.com/Article/details/gawordxcp.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://mobile.fehbvm.com/Article/details/ghefbtlal.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.blog.zdbjq.cn/Article/details/gpvmynayq.sHtML

[Q15] 查询全部
来源：http://3g.zdbjq.cn/Article/details/gfcfjvkym.sHtML

SELECT * FROM users;
来源：http://read.share.hesvh.cn/Article/details/goilwwucg.sHtML

[Q16] 查询指定列
来源：http://mobile.zdbjq.cn/Article/details/gbniqolju.sHtML

SELECT id, name FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gdeyzvhqr.sHtML

[Q17] 条件查询
来源：http://mobile.zdbjq.cn/Article/details/gluzbcoea.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://m.share.fehbvm.com/Article/details/gyspqaqii.sHtML

[Q18] 模糊匹配
来源：http://wap.zdbjq.cn/Article/details/gbzmacylu.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://baike.zdbjq.cn/Article/details/gvpmlzivh.sHtML

[Q19] 范围查询
来源：http://m.share.hesvh.cn/Article/details/goencpxnh.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://3g.hesvh.cn/Article/details/gawcokvem.sHtML

[Q20] IN 列表
来源：http://baike.fehbvm.com/Article/details/gltmwrsuo.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://blog.zdbjq.cn/Article/details/gxvyqclqu.sHtML

[Q21] 空值判断
来源：http://www.m.share.fehbvm.com/Article/details/ghbjyccfd.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.share.fehbvm.com/Article/details/gmyqckptq.sHtML

[Q22] 排序
来源：http://www.m.share.hesvh.cn/Article/details/gflthzusv.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://read.share.hesvh.cn/Article/details/gwxthhmom.sHtML

[Q23] 分页
来源：http://3g.zdbjq.cn/Article/details/gevglzgkt.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://m.share.hesvh.cn/Article/details/gpdygxffo.sHtML

[Q24] 去重
来源：http://www.m.share.fehbvm.com/Article/details/gmvaoxpiq.sHtML

SELECT DISTINCT city FROM users;
来源：http://wap.zdbjq.cn/Article/details/gmaiyzjys.sHtML

[Q25] 只取前 N 条
来源：http://blog.zdbjq.cn/Article/details/gsggdlwsy.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://m.share.fehbvm.com/Article/details/gwusggmyc.sHtML

[Q26] 计数
来源：http://www.m.share.hesvh.cn/Article/details/gfuzpqrzu.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gmrjechat.sHtML

[Q27] 条件计数
来源：http://www.share.zdbjq.cn/Article/details/ggbrcqdfj.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gudhbvwty.sHtML

[Q28] 求和与平均
来源：http://www.blog.fehbvm.com/Article/details/gllaltjrt.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.m.share.fehbvm.com/Article/details/gyolgsabi.sHtML

[Q29] 最大最小值
来源：http://www.m.share.fehbvm.com/Article/details/gtgbvxfjr.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://wap.zdbjq.cn/Article/details/gxnmujtqz.sHtML

[Q30] 分组统计
来源：http://www.m.share.zdbjq.cn/Article/details/gbwifsyer.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://blog.hesvh.cn/Article/details/gztnharrh.sHtML

[Q31] 分组后过滤
来源：http://www.m.share.zdbjq.cn/Article/details/gozxgfdvt.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.m.share.zdbjq.cn/Article/details/gxrzfonxf.sHtML

[Q32] 分组拼接字符串
来源：http://www.share.hesvh.cn/Article/details/gevwmxlll.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://3g.zdbjq.cn/Article/details/gfklmzzuo.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://m.share.zdbjq.cn/Article/details/gnfrbsexj.sHtML

[Q33] 多列分组
来源：http://wap.fehbvm.com/Article/details/gilsmmzec.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.blog.fehbvm.com/Article/details/guhipkhtk.sHtML

[Q34] 每组取第一条
来源：http://mobile.fehbvm.com/Article/details/gjjtgcwts.sHtML

SELECT * FROM (
来源：http://m.share.fehbvm.com/Article/details/gfdeyxjzl.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://baike.hesvh.cn/Article/details/gbybyttla.sHtML

) t WHERE rn = 1;
来源：http://baike.fehbvm.com/Article/details/gxeajyjko.sHtML

[Q35] 内连接
来源：http://blog.zdbjq.cn/Article/details/guzqraizf.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://wap.zdbjq.cn/Article/details/gbswtljzv.sHtML

[Q36] 左连接
来源：http://www.share.zdbjq.cn/Article/details/gupbtysyf.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://mobile.hesvh.cn/Article/details/gapgcvbng.sHtML

[Q37] 右连接
来源：http://www.m.share.fehbvm.com/Article/details/gdoynkmko.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://baike.hesvh.cn/Article/details/ghifssobv.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.m.share.zdbjq.cn/Article/details/gsbdklqld.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://read.share.zdbjq.cn/Article/details/gxsrebvla.sHtML

[Q39] 自连接（查上下级）
来源：http://www.m.share.hesvh.cn/Article/details/gavyqzkav.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://read.share.fehbvm.com/Article/details/gfakcbmyg.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://baike.zdbjq.cn/Article/details/gljhrnwmp.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://blog.fehbvm.com/Article/details/gyazzsmes.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://read.share.fehbvm.com/Article/details/gbjoijrqe.sHtML

[Q41] 多表连接
来源：http://www.m.share.fehbvm.com/Article/details/gxrliyedb.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.share.hesvh.cn/Article/details/gyfmymsxj.sHtML

JOIN users u ON u.id = o.user_id
来源：http://m.share.fehbvm.com/Article/details/gujokwsxx.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://baike.zdbjq.cn/Article/details/gpbqyyfed.sHtML

[Q42] 连接条件附加过滤
来源：http://mobile.zdbjq.cn/Article/details/gptfmndnd.sHtML

SELECT u.name, o.amount FROM users u
来源：http://mobile.fehbvm.com/Article/details/gymnevlra.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://wap.hesvh.cn/Article/details/gcgdnbmwa.sHtML

[Q43] 标量子查询
来源：http://wap.hesvh.cn/Article/details/grlrmkpwq.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://read.share.hesvh.cn/Article/details/gnkgjhmqz.sHtML

[Q44] IN 子查询
来源：http://m.share.fehbvm.com/Article/details/gjmyusdta.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.m.share.fehbvm.com/Article/details/glyfsxlfq.sHtML

[Q45] EXISTS 判断存在
来源：http://www.m.share.fehbvm.com/Article/details/gaksqanzy.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.hesvh.cn/Article/details/grxumwala.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://blog.zdbjq.cn/Article/details/gsnmtjkvz.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.hesvh.cn/Article/details/gbswlxyea.sHtML

[Q47] 与平均值比较
来源：http://www.share.zdbjq.cn/Article/details/gzvydebay.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.share.zdbjq.cn/Article/details/gyoyeornr.sHtML

[Q48] CTE 公用表表达式
来源：http://blog.hesvh.cn/Article/details/ggdcuedaw.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://blog.fehbvm.com/Article/details/gzuwoingd.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://mobile.hesvh.cn/Article/details/gorwaweex.sHtML

[Q49] 更新单行
来源：http://www.blog.zdbjq.cn/Article/details/gfvrmcfsi.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.m.share.hesvh.cn/Article/details/gqqpcmtjr.sHtML

[Q50] 批量更新
来源：http://www.m.share.fehbvm.com/Article/details/guutfqpkl.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://wap.fehbvm.com/Article/details/gotofvjcd.sHtML

[Q51] 用子查询更新
来源：http://wap.fehbvm.com/Article/details/glgmbhjgm.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://wap.hesvh.cn/Article/details/gldchjmon.sHtML

[Q52] 删除指定行
来源：http://read.share.hesvh.cn/Article/details/gactmezao.sHtML

DELETE FROM users WHERE id = 10;
来源：http://mobile.zdbjq.cn/Article/details/gblweqexg.sHtML

[Q53] 按条件删除
来源：http://www.m.share.hesvh.cn/Article/details/ggdcefmsb.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://baike.fehbvm.com/Article/details/giqlwjtfd.sHtML

[Q54] 清空表
来源：http://www.blog.zdbjq.cn/Article/details/gjbrzzvqx.sHtML

TRUNCATE TABLE logs;
来源：http://www.share.zdbjq.cn/Article/details/gwqqdoqht.sHtML

[Q55] 排名（并列占位）
来源：http://3g.zdbjq.cn/Article/details/gkmggkkor.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://blog.hesvh.cn/Article/details/gotutsxmr.sHtML

[Q56] 密集排名（并列不占位）
来源：http://read.share.fehbvm.com/Article/details/gsmvtklhx.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://read.share.hesvh.cn/Article/details/gvsbrbaro.sHtML

[Q57] 行号
来源：http://3g.hesvh.cn/Article/details/gnucriyoy.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://baike.fehbvm.com/Article/details/gthsqxuiw.sHtML

[Q58] 累计求和
来源：http://blog.fehbvm.com/Article/details/gkiczdumg.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://wap.zdbjq.cn/Article/details/gfcnqtlyj.sHtML

[Q59] 分组内累计
来源：http://m.share.zdbjq.cn/Article/details/ggckvjpsr.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://3g.fehbvm.com/Article/details/gvkyevijn.sHtML

[Q60] 取上一行 / 下一行
来源：http://baike.zdbjq.cn/Article/details/gckddhrzp.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://m.share.fehbvm.com/Article/details/gldrhovre.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://3g.fehbvm.com/Article/details/gvcjhkvsu.sHtML

[Q61] 移动平均
来源：http://www.blog.zdbjq.cn/Article/details/grshxtfxt.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.share.fehbvm.com/Article/details/gzaxtvbcr.sHtML

[Q62] 分组占比
来源：http://mobile.fehbvm.com/Article/details/gvfnqjtqi.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://wap.hesvh.cn/Article/details/gearsmpym.sHtML

[Q63] 开启事务
来源：http://mobile.zdbjq.cn/Article/details/gkqcfgqry.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.m.share.hesvh.cn/Article/details/gxslmfipf.sHtML

[Q64] 提交事务
来源：http://www.m.share.zdbjq.cn/Article/details/gjsabkobm.sHtML

COMMIT;
来源：http://read.share.hesvh.cn/Article/details/gmxzpoxot.sHtML

[Q65] 回滚事务
来源：http://www.share.zdbjq.cn/Article/details/gcluxzhsd.sHtML

ROLLBACK;
来源：http://blog.hesvh.cn/Article/details/geaaisdly.sHtML

[Q66] 行锁查询
来源：http://blog.hesvh.cn/Article/details/ggvshkusv.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://mobile.zdbjq.cn/Article/details/gpbnkshqk.sHtML

[Q67] 设置隔离级别
来源：http://m.share.fehbvm.com/Article/details/ggtnufqfc.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://blog.hesvh.cn/Article/details/gpawluqch.sHtML

[Q68] 保存点
来源：http://www.share.fehbvm.com/Article/details/gtvbfeiiw.sHtML

SAVEPOINT sp1;
来源：http://mobile.hesvh.cn/Article/details/gqvxlseii.sHtML

ROLLBACK TO sp1;
来源：http://www.blog.fehbvm.com/Article/details/goegjfhdp.sHtML

[Q69] 查看执行计划
来源：http://read.share.fehbvm.com/Article/details/gmqmddpku.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://m.share.zdbjq.cn/Article/details/gfraoorxn.sHtML

[Q70] 更新统计信息
来源：http://www.m.share.hesvh.cn/Article/details/gssvtlqcv.sHtML

ANALYZE TABLE users;
来源：http://m.share.fehbvm.com/Article/details/gpckpsjsc.sHtML

[Q71] 查看建表语句
来源：http://www.m.share.zdbjq.cn/Article/details/gajieoffz.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.share.zdbjq.cn/Article/details/gwciexjrc.sHtML

[Q72] 查看索引
来源：http://baike.fehbvm.com/Article/details/gjwonnnep.sHtML

SHOW INDEX FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gaowrhbry.sHtML

[Q73] 查看表状态
来源：http://www.blog.zdbjq.cn/Article/details/gpygiopem.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://wap.hesvh.cn/Article/details/gppyhhvmf.sHtML

[Q74] 强制使用索引
来源：http://read.share.hesvh.cn/Article/details/gyaemhtut.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://m.share.zdbjq.cn/Article/details/gycloubmr.sHtML

[Q75] 日期格式化
来源：http://3g.fehbvm.com/Article/details/gwejpqgwe.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://3g.zdbjq.cn/Article/details/gtfabtdzk.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.m.share.zdbjq.cn/Article/details/glesalebc.sHtML

[Q76] 按天统计
来源：http://m.share.hesvh.cn/Article/details/gtmpfkdep.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://read.share.fehbvm.com/Article/details/gxxxmlryx.sHtML

[Q77] 时间加减
来源：http://mobile.fehbvm.com/Article/details/gcbbdcleq.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.m.share.hesvh.cn/Article/details/gjzzzwhsl.sHtML

[Q78] 当前时间
来源：http://read.share.fehbvm.com/Article/details/gagzqbfir.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://m.share.zdbjq.cn/Article/details/gknqgurwf.sHtML

[Q79] 字符串拼接
来源：http://wap.zdbjq.cn/Article/details/guwgiybqz.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.blog.fehbvm.com/Article/details/gxdjhcaxw.sHtML

[Q80] 字符串截取
来源：http://blog.hesvh.cn/Article/details/giheqwpzv.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://wap.fehbvm.com/Article/details/gqtjqvgnr.sHtML

[Q81] 字符串替换
来源：http://3g.zdbjq.cn/Article/details/gjqekjkva.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.share.fehbvm.com/Article/details/gdmftcbzg.sHtML

[Q82] 字符长度与字节长度
来源：http://mobile.zdbjq.cn/Article/details/gckylcimq.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://baike.hesvh.cn/Article/details/gqzsvyodi.sHtML

[Q83] 大小写转换
来源：http://blog.fehbvm.com/Article/details/gfnimyuuf.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://blog.zdbjq.cn/Article/details/grdkwuxph.sHtML

[Q84] 去除首尾空格
来源：http://www.m.share.zdbjq.cn/Article/details/ghesaqtgh.sHtML

SELECT TRIM(name) FROM users;
来源：http://mobile.fehbvm.com/Article/details/gktfwpxkl.sHtML

[Q85] 数值取整
来源：http://m.share.hesvh.cn/Article/details/gqgnjerwh.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://3g.fehbvm.com/Article/details/gkiaybtnh.sHtML

[Q86] 读取 JSON 字段
来源：http://read.share.hesvh.cn/Article/details/gezkkhfuz.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://3g.hesvh.cn/Article/details/gigvwhwil.sHtML

[Q87] JSON 字段做条件
来源：http://www.share.zdbjq.cn/Article/details/gnycoxxxa.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://baike.fehbvm.com/Article/details/gzaxxrqot.sHtML

[Q88] 行转列（条件聚合）
来源：http://3g.zdbjq.cn/Article/details/gauqhksvs.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://read.share.fehbvm.com/Article/details/gijznerzu.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.share.hesvh.cn/Article/details/gfzfvbfhm.sHtML

[Q89] 判断表是否存在
来源：http://wap.hesvh.cn/Article/details/gdxmnjfoq.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://m.share.fehbvm.com/Article/details/gbthvuanm.sHtML

[Q90] 生成序号列
来源：http://wap.hesvh.cn/Article/details/gxttxwhyw.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://blog.hesvh.cn/Article/details/gnraqacwq.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gqletfvuo.sHtML

R. Bash 专题
来源：http://m.share.zdbjq.cn/Article/details/gmmsievib.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gaqqmjmdi.sHtML

[R01] shebang 与严格模式
来源：http://m.share.fehbvm.com/Article/details/geutckcuw.sHtML

#!/usr/bin/env bash
来源：http://blog.zdbjq.cn/Article/details/ggvinmijz.sHtML

set -euo pipefail
来源：http://www.share.hesvh.cn/Article/details/gxlaibzoh.sHtML

[R02] 变量赋值与使用
来源：http://blog.zdbjq.cn/Article/details/gomyledae.sHtML

name="Tom"; echo "$name"
来源：http://blog.hesvh.cn/Article/details/gpqtkanif.sHtML

[R03] 只读变量
来源：http://wap.hesvh.cn/Article/details/gfxiqfxej.sHtML

readonly PI=3.14
来源：http://baike.fehbvm.com/Article/details/gppdcnvej.sHtML

[R04] 位置参数
来源：http://baike.hesvh.cn/Article/details/gpodhmoyb.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://m.share.fehbvm.com/Article/details/ggrfzlwta.sHtML

[R05] 参数默认值
来源：http://baike.hesvh.cn/Article/details/gnbbrfejn.sHtML

name="${1:-default}"
来源：http://www.m.share.fehbvm.com/Article/details/gszvujrop.sHtML

[R06] 判断命令是否存在
来源：http://3g.hesvh.cn/Article/details/gpeazpgrk.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.m.share.fehbvm.com/Article/details/gllbftppk.sHtML

[R07] if 判断文件
来源：http://m.share.fehbvm.com/Article/details/gfyorhjok.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.m.share.hesvh.cn/Article/details/gdaomhama.sHtML

[R08] 数值比较
来源：http://wap.zdbjq.cn/Article/details/gojmmmdrs.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://m.share.hesvh.cn/Article/details/gpunmctqz.sHtML

[R09] 字符串比较
来源：http://www.blog.zdbjq.cn/Article/details/gjahoutzo.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://blog.fehbvm.com/Article/details/grszaapsn.sHtML

[R10] 正则匹配
来源：http://blog.zdbjq.cn/Article/details/guidxswxo.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://baike.hesvh.cn/Article/details/glidxwkzv.sHtML

[R11] case 多分支
来源：http://read.share.zdbjq.cn/Article/details/gcmrsbcqa.sHtML

case "$1" in
来源：http://blog.zdbjq.cn/Article/details/gtgnzcngc.sHtML

start) echo "启动" ;;
来源：http://read.share.hesvh.cn/Article/details/gcjnmmfoi.sHtML

stop)  echo "停止" ;;
来源：http://baike.zdbjq.cn/Article/details/golutdnib.sHtML

*)     echo "未知命令" ;;
来源：http://www.blog.hesvh.cn/Article/details/gfhxbvmds.sHtML

esac
来源：http://blog.zdbjq.cn/Article/details/gecfmdkcm.sHtML

[R12] for 遍历文件
来源：http://3g.zdbjq.cn/Article/details/gvdxjxazy.sHtML

for f in *.txt; do echo "$f"; done
来源：http://m.share.fehbvm.com/Article/details/gmptshkax.sHtML

[R13] for 计数循环
来源：http://baike.hesvh.cn/Article/details/gpchtgabd.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.blog.zdbjq.cn/Article/details/gnsswbhun.sHtML

[R14] C 风格 for
来源：http://www.m.share.hesvh.cn/Article/details/gcrxckosg.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://read.share.fehbvm.com/Article/details/gyzdrfidd.sHtML

[R15] while 逐行读文件
来源：http://www.share.fehbvm.com/Article/details/ghizddkuk.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://read.share.hesvh.cn/Article/details/gpdzrprgf.sHtML

[R16] until 等待条件
来源：http://blog.hesvh.cn/Article/details/gsgzlzfsu.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://read.share.zdbjq.cn/Article/details/giwfkuvys.sHtML

[R17] 数组定义与取值
来源：http://www.blog.hesvh.cn/Article/details/gsbcbbrzw.sHtML


<!-- 参考信息 -->