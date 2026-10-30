代发 wailian999

Ruby: Digest::SHA256.hexdigest(s)
来源：http://mobile.zdbjq.cn/Article/details/gkitodykr.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://3g.zdbjq.cn/Article/details/ghyofpgid.sHtML

[P03] 生成短随机字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gsfmuekjj.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://mobile.fehbvm.com/Article/details/gcxochqjn.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.share.hesvh.cn/Article/details/gdbiatqly.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.hesvh.cn/Article/details/ghyerorom.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.fehbvm.com/Article/details/gadiebius.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://3g.zdbjq.cn/Article/details/gakvjghna.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.m.share.hesvh.cn/Article/details/gcgduwgbm.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://mobile.fehbvm.com/Article/details/gzfvfypgj.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.share.zdbjq.cn/Article/details/gzaivizhb.sHtML

[P04] 求长度
来源：http://www.blog.fehbvm.com/Article/details/gznlmtamm.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://3g.fehbvm.com/Article/details/ghotiynbv.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.zdbjq.cn/Article/details/gbayqrtkm.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.fehbvm.com/Article/details/gitvzpjwx.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.zdbjq.cn/Article/details/gcyziqpkp.sHtML

Java: list.size();  map.size();  s.length()
来源：http://blog.hesvh.cn/Article/details/gsznxroaq.sHtML

Go:   len(arr);  len(m)
来源：http://www.blog.zdbjq.cn/Article/details/gpkjawraa.sHtML

Ruby: x.length;  x.size
来源：http://www.share.zdbjq.cn/Article/details/gfgxwcfte.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.share.hesvh.cn/Article/details/grkfftyiy.sHtML

[P05] 判断两个对象内容是否相等
来源：http://blog.fehbvm.com/Article/details/gfqaekidp.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://baike.hesvh.cn/Article/details/gtsiynden.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://mobile.hesvh.cn/Article/details/ggmvhrhkv.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://m.share.zdbjq.cn/Article/details/gkcyjntja.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.share.hesvh.cn/Article/details/ghcwyspda.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://mobile.zdbjq.cn/Article/details/ghapxfevm.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://mobile.zdbjq.cn/Article/details/gajqfhzuq.sHtML

Ruby: a == b
来源：http://read.share.hesvh.cn/Article/details/ghnyitatn.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.blog.hesvh.cn/Article/details/gdktpvqfn.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://mobile.zdbjq.cn/Article/details/gvutevemz.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://wap.zdbjq.cn/Article/details/gtjflttue.sHtML

PHP:  if (empty($x)) {}
来源：http://read.share.fehbvm.com/Article/details/gkshzcbyq.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.m.share.hesvh.cn/Article/details/guxufjmza.sHtML

TS:   if (x == null) {}
来源：http://read.share.hesvh.cn/Article/details/gmjxdkcgk.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://mobile.fehbvm.com/Article/details/gcdxbubqa.sHtML

Go:   if x == nil {}
来源：http://blog.zdbjq.cn/Article/details/gzfbkqnvi.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.share.fehbvm.com/Article/details/gngrbxpgf.sHtML

C#:   if (x is null) {}
来源：http://www.m.share.hesvh.cn/Article/details/gmdywyjnp.sHtML

[P07] 防抖与节流
来源：http://baike.zdbjq.cn/Article/details/glsbsaupx.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://3g.hesvh.cn/Article/details/gxokkpukv.sHtML

PHP:  // 手写时间戳比较
来源：http://baike.zdbjq.cn/Article/details/gjflsqqtc.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.fehbvm.com/Article/details/gwsvpkpij.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.fehbvm.com/Article/details/gmposapvn.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://blog.hesvh.cn/Article/details/gigakuwfp.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.m.share.fehbvm.com/Article/details/gzyjprggg.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.blog.zdbjq.cn/Article/details/gszlxwbhq.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://m.share.fehbvm.com/Article/details/gzdavnfzw.sHtML

[P08] 处理浮点精度问题
来源：http://www.m.share.zdbjq.cn/Article/details/ghuochhev.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://baike.zdbjq.cn/Article/details/gxwczmboi.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://baike.fehbvm.com/Article/details/gmpntdmuq.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.m.share.zdbjq.cn/Article/details/ggcyzaqrf.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://m.share.zdbjq.cn/Article/details/gffllwesy.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.m.share.zdbjq.cn/Article/details/gnuvcwrlj.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.blog.hesvh.cn/Article/details/gpxcdiyox.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://baike.hesvh.cn/Article/details/gfwbgtudq.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.m.share.hesvh.cn/Article/details/guetqbdvq.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gqosclyfs.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.share.zdbjq.cn/Article/details/ggaiigosq.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gndkxzime.sHtML

[Q01] 创建表
来源：http://www.m.share.hesvh.cn/Article/details/gdrlppoju.sHtML

CREATE TABLE users (
来源：http://baike.hesvh.cn/Article/details/gpisxbcbg.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.fehbvm.com/Article/details/ggclrrpth.sHtML

name VARCHAR(50) NOT NULL,
来源：http://blog.zdbjq.cn/Article/details/gnlimgqrk.sHtML

email VARCHAR(100) UNIQUE,
来源：http://read.share.fehbvm.com/Article/details/gyxauhcon.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://baike.zdbjq.cn/Article/details/gpvbpfgpp.sHtML

);
来源：http://read.share.zdbjq.cn/Article/details/gxfgomsic.sHtML

[Q02] 创建带外键的表
来源：http://read.share.hesvh.cn/Article/details/guhmcihbn.sHtML

CREATE TABLE orders (
来源：http://m.share.zdbjq.cn/Article/details/gjnumsuvz.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.hesvh.cn/Article/details/gfgnyfjgz.sHtML

user_id INT NOT NULL,
来源：http://www.share.zdbjq.cn/Article/details/gopqjobfh.sHtML

amount DECIMAL(10, 2),
来源：http://blog.hesvh.cn/Article/details/gmxxxvwly.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://mobile.fehbvm.com/Article/details/gcmcrfwfw.sHtML

);
来源：http://mobile.hesvh.cn/Article/details/gtotqqkcy.sHtML

[Q03] 增加列
来源：http://3g.hesvh.cn/Article/details/gqxcxowjp.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://blog.hesvh.cn/Article/details/gynhlsdrt.sHtML

[Q04] 修改列类型
来源：http://read.share.hesvh.cn/Article/details/gwdvskyph.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://mobile.zdbjq.cn/Article/details/gzjqdaybp.sHtML

[Q05] 重命名列
来源：http://baike.hesvh.cn/Article/details/guchdvmnu.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://mobile.hesvh.cn/Article/details/gyvkacabf.sHtML

[Q06] 删除列
来源：http://m.share.fehbvm.com/Article/details/gugcijlzm.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://mobile.hesvh.cn/Article/details/ghstrlyfo.sHtML

[Q07] 删除表
来源：http://wap.fehbvm.com/Article/details/ggzcbcynl.sHtML

DROP TABLE IF EXISTS orders;
来源：http://baike.fehbvm.com/Article/details/gmutjojkz.sHtML

[Q08] 创建普通索引
来源：http://www.m.share.fehbvm.com/Article/details/gmowgubzb.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://m.share.hesvh.cn/Article/details/gdnovsjmc.sHtML

[Q09] 创建唯一索引
来源：http://www.share.zdbjq.cn/Article/details/gsdrcwive.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.share.zdbjq.cn/Article/details/gxaiaxzyi.sHtML

[Q10] 插入单行
来源：http://3g.fehbvm.com/Article/details/gseprugpc.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.blog.hesvh.cn/Article/details/gyrncmmnr.sHtML

[Q11] 一次插入多行
来源：http://www.share.hesvh.cn/Article/details/gfitpjbbw.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://mobile.zdbjq.cn/Article/details/gringkghk.sHtML

[Q12] 插入后取自增 ID
来源：http://blog.hesvh.cn/Article/details/gqidcxtre.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://wap.fehbvm.com/Article/details/gblotiksv.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://mobile.fehbvm.com/Article/details/grohagvht.sHtML

[Q13] 忽略重复插入
来源：http://www.m.share.zdbjq.cn/Article/details/gfrnijaug.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://read.share.zdbjq.cn/Article/details/gsdaslcky.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.m.share.fehbvm.com/Article/details/gxpdxcydw.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://m.share.fehbvm.com/Article/details/gvfvjssnf.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://m.share.zdbjq.cn/Article/details/gddkppvdn.sHtML

[Q15] 查询全部
来源：http://read.share.zdbjq.cn/Article/details/gqmszfhuk.sHtML

SELECT * FROM users;
来源：http://m.share.fehbvm.com/Article/details/gegqjtrxs.sHtML

[Q16] 查询指定列
来源：http://baike.hesvh.cn/Article/details/gbokgkxez.sHtML

SELECT id, name FROM users;
来源：http://baike.zdbjq.cn/Article/details/gqizhyige.sHtML

[Q17] 条件查询
来源：http://www.m.share.hesvh.cn/Article/details/gafzqaffh.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://wap.fehbvm.com/Article/details/gueauwwir.sHtML

[Q18] 模糊匹配
来源：http://www.m.share.fehbvm.com/Article/details/gigixhmqk.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://wap.fehbvm.com/Article/details/gkanldppq.sHtML

[Q19] 范围查询
来源：http://3g.zdbjq.cn/Article/details/gfqexdrnj.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.blog.hesvh.cn/Article/details/gkalybhiv.sHtML

[Q20] IN 列表
来源：http://3g.zdbjq.cn/Article/details/ghniocawl.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://wap.hesvh.cn/Article/details/gmdrxuthz.sHtML

[Q21] 空值判断
来源：http://3g.hesvh.cn/Article/details/gqpystnyk.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.blog.hesvh.cn/Article/details/gypupqhfg.sHtML

[Q22] 排序
来源：http://wap.hesvh.cn/Article/details/glizinjkh.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://mobile.zdbjq.cn/Article/details/gsnacpzhk.sHtML

[Q23] 分页
来源：http://www.blog.fehbvm.com/Article/details/gprimhusr.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://mobile.zdbjq.cn/Article/details/gvbjotfop.sHtML

[Q24] 去重
来源：http://wap.zdbjq.cn/Article/details/gfophnsoy.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gmexpyzef.sHtML

[Q25] 只取前 N 条
来源：http://blog.zdbjq.cn/Article/details/gqcekjcif.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://read.share.zdbjq.cn/Article/details/ghagemglt.sHtML

[Q26] 计数
来源：http://www.m.share.zdbjq.cn/Article/details/guubqipge.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.share.zdbjq.cn/Article/details/goxakslyu.sHtML

[Q27] 条件计数
来源：http://www.blog.hesvh.cn/Article/details/gpcrtraug.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://blog.hesvh.cn/Article/details/gugopphbt.sHtML

[Q28] 求和与平均
来源：http://www.m.share.hesvh.cn/Article/details/ggpmusecf.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://mobile.fehbvm.com/Article/details/gqiaifzzw.sHtML

[Q29] 最大最小值
来源：http://3g.zdbjq.cn/Article/details/gnhmxnuta.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://blog.hesvh.cn/Article/details/gbuqnlxyh.sHtML

[Q30] 分组统计
来源：http://blog.fehbvm.com/Article/details/ggermseaq.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://baike.fehbvm.com/Article/details/gtjewhcli.sHtML

[Q31] 分组后过滤
来源：http://baike.hesvh.cn/Article/details/ghnvktjje.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://mobile.hesvh.cn/Article/details/gmzsigigj.sHtML

[Q32] 分组拼接字符串
来源：http://mobile.hesvh.cn/Article/details/gabazigcd.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.m.share.zdbjq.cn/Article/details/ghadqhgpj.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://wap.zdbjq.cn/Article/details/gnprpsxtt.sHtML

[Q33] 多列分组
来源：http://wap.zdbjq.cn/Article/details/gvihuqrij.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://blog.zdbjq.cn/Article/details/gmdbksmvm.sHtML

[Q34] 每组取第一条
来源：http://baike.fehbvm.com/Article/details/guzpbujrk.sHtML

SELECT * FROM (
来源：http://www.blog.fehbvm.com/Article/details/gvdosqvpx.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://wap.hesvh.cn/Article/details/guiuhpccv.sHtML

) t WHERE rn = 1;
来源：http://wap.fehbvm.com/Article/details/gwjwetmtj.sHtML

[Q35] 内连接
来源：http://read.share.zdbjq.cn/Article/details/gbqyxpmva.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://blog.hesvh.cn/Article/details/gtxrpdvag.sHtML

[Q36] 左连接
来源：http://blog.hesvh.cn/Article/details/gxenvegkp.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://m.share.hesvh.cn/Article/details/gnzjxqhwr.sHtML

[Q37] 右连接
来源：http://read.share.fehbvm.com/Article/details/gzyxyampr.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://baike.hesvh.cn/Article/details/guitgmdgo.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://m.share.zdbjq.cn/Article/details/gfraurcuu.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://read.share.fehbvm.com/Article/details/gobrjzmhr.sHtML

[Q39] 自连接（查上下级）
来源：http://read.share.zdbjq.cn/Article/details/ggcotejvc.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://blog.hesvh.cn/Article/details/gbyhntvbo.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://blog.fehbvm.com/Article/details/ghzjnjnqg.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://read.share.fehbvm.com/Article/details/ggiiqilsy.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://mobile.zdbjq.cn/Article/details/gsbiieaow.sHtML

[Q41] 多表连接
来源：http://blog.fehbvm.com/Article/details/gkxolskkg.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://mobile.fehbvm.com/Article/details/gimtzromj.sHtML

JOIN users u ON u.id = o.user_id
来源：http://read.share.fehbvm.com/Article/details/gicwuknhx.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.m.share.fehbvm.com/Article/details/gpguxixio.sHtML

[Q42] 连接条件附加过滤
来源：http://3g.hesvh.cn/Article/details/gnfiasqif.sHtML

SELECT u.name, o.amount FROM users u
来源：http://baike.hesvh.cn/Article/details/gtrsmucxn.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.m.share.zdbjq.cn/Article/details/gybakohaw.sHtML

[Q43] 标量子查询
来源：http://wap.hesvh.cn/Article/details/gdjkfdgej.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.blog.fehbvm.com/Article/details/ggpbnxbah.sHtML

[Q44] IN 子查询
来源：http://read.share.fehbvm.com/Article/details/gbwriscuz.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.blog.fehbvm.com/Article/details/gytscukhn.sHtML

[Q45] EXISTS 判断存在
来源：http://m.share.zdbjq.cn/Article/details/galhdgbjx.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.hesvh.cn/Article/details/gqktesdhx.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://mobile.hesvh.cn/Article/details/gasmtoqbu.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.zdbjq.cn/Article/details/gdxqlqztj.sHtML

[Q47] 与平均值比较
来源：http://blog.hesvh.cn/Article/details/gvnqxiecm.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://m.share.zdbjq.cn/Article/details/gqtijgbip.sHtML

[Q48] CTE 公用表表达式
来源：http://blog.zdbjq.cn/Article/details/gptxverlp.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.blog.hesvh.cn/Article/details/gpvahpgvk.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://m.share.fehbvm.com/Article/details/ggdxpjbkp.sHtML

[Q49] 更新单行
来源：http://mobile.zdbjq.cn/Article/details/gvrjqsfxx.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://read.share.hesvh.cn/Article/details/gqyexyezc.sHtML

[Q50] 批量更新
来源：http://www.m.share.hesvh.cn/Article/details/geavhpaxu.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://wap.fehbvm.com/Article/details/ghccuakov.sHtML

[Q51] 用子查询更新
来源：http://www.m.share.zdbjq.cn/Article/details/gsikhegbu.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://mobile.fehbvm.com/Article/details/gkulizaye.sHtML

[Q52] 删除指定行
来源：http://www.blog.zdbjq.cn/Article/details/gxlwxivrl.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.m.share.fehbvm.com/Article/details/gjspzplbn.sHtML

[Q53] 按条件删除
来源：http://baike.fehbvm.com/Article/details/gecxcrlaz.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://wap.fehbvm.com/Article/details/gnasbfjfh.sHtML

[Q54] 清空表
来源：http://blog.zdbjq.cn/Article/details/gmeyyzrdj.sHtML

TRUNCATE TABLE logs;
来源：http://www.share.fehbvm.com/Article/details/gplsewnhl.sHtML

[Q55] 排名（并列占位）
来源：http://blog.hesvh.cn/Article/details/gjuhrrulp.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://baike.fehbvm.com/Article/details/geqsnndwc.sHtML

[Q56] 密集排名（并列不占位）
来源：http://3g.fehbvm.com/Article/details/gfqxsuppc.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://3g.hesvh.cn/Article/details/gomlqqzow.sHtML

[Q57] 行号
来源：http://read.share.hesvh.cn/Article/details/gomvfvakj.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://3g.zdbjq.cn/Article/details/gqqofmjao.sHtML

[Q58] 累计求和
来源：http://www.blog.zdbjq.cn/Article/details/gwyhwueog.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://mobile.fehbvm.com/Article/details/goclvhmqr.sHtML

[Q59] 分组内累计
来源：http://m.share.hesvh.cn/Article/details/gttrxjobt.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://baike.zdbjq.cn/Article/details/gcpsffwoy.sHtML

[Q60] 取上一行 / 下一行
来源：http://baike.hesvh.cn/Article/details/grxtybvlk.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://read.share.fehbvm.com/Article/details/gsdybznfw.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://read.share.hesvh.cn/Article/details/ghabiyjdg.sHtML

[Q61] 移动平均
来源：http://www.m.share.fehbvm.com/Article/details/gsriyqurm.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.share.fehbvm.com/Article/details/gilqxxhnq.sHtML

[Q62] 分组占比
来源：http://blog.fehbvm.com/Article/details/gxuvjoyun.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.blog.hesvh.cn/Article/details/gppdwrxvz.sHtML

[Q63] 开启事务
来源：http://mobile.fehbvm.com/Article/details/gcojuxxya.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://blog.zdbjq.cn/Article/details/gufpwtxcn.sHtML

[Q64] 提交事务
来源：http://m.share.zdbjq.cn/Article/details/gxieiquim.sHtML

COMMIT;
来源：http://3g.hesvh.cn/Article/details/grrdyvwee.sHtML

[Q65] 回滚事务
来源：http://read.share.zdbjq.cn/Article/details/gfnbsjgsp.sHtML

ROLLBACK;
来源：http://mobile.hesvh.cn/Article/details/gndjmcafe.sHtML

[Q66] 行锁查询
来源：http://m.share.hesvh.cn/Article/details/gloclkcpe.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.blog.fehbvm.com/Article/details/gdhqmvkxb.sHtML

[Q67] 设置隔离级别
来源：http://wap.hesvh.cn/Article/details/gojrhqses.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://blog.zdbjq.cn/Article/details/gkegubpjt.sHtML

[Q68] 保存点
来源：http://read.share.zdbjq.cn/Article/details/gqdqqjciy.sHtML

SAVEPOINT sp1;
来源：http://www.blog.hesvh.cn/Article/details/gttzamcgd.sHtML

ROLLBACK TO sp1;
来源：http://www.share.zdbjq.cn/Article/details/ggzqimogc.sHtML

[Q69] 查看执行计划
来源：http://www.share.zdbjq.cn/Article/details/gvvzztjyk.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://mobile.hesvh.cn/Article/details/gpmsfqxje.sHtML

[Q70] 更新统计信息
来源：http://blog.fehbvm.com/Article/details/gzwfkauwb.sHtML

ANALYZE TABLE users;
来源：http://wap.fehbvm.com/Article/details/goxvhwkpr.sHtML

[Q71] 查看建表语句
来源：http://www.share.zdbjq.cn/Article/details/ggxjchlul.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://blog.zdbjq.cn/Article/details/gujmlmjil.sHtML

[Q72] 查看索引
来源：http://baike.zdbjq.cn/Article/details/gqnoetexe.sHtML

SHOW INDEX FROM users;
来源：http://blog.zdbjq.cn/Article/details/gpmsswvri.sHtML

[Q73] 查看表状态
来源：http://read.share.hesvh.cn/Article/details/gbrddzacc.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://wap.zdbjq.cn/Article/details/gyjtrwhil.sHtML

[Q74] 强制使用索引
来源：http://mobile.zdbjq.cn/Article/details/gtntmfafw.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.blog.zdbjq.cn/Article/details/gpfcgljdy.sHtML

[Q75] 日期格式化
来源：http://www.share.fehbvm.com/Article/details/gywbkfrmt.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://mobile.zdbjq.cn/Article/details/gwpyozhiy.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://baike.fehbvm.com/Article/details/gurizgzjh.sHtML

[Q76] 按天统计
来源：http://mobile.fehbvm.com/Article/details/gzivsulop.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://mobile.hesvh.cn/Article/details/gneeggqhq.sHtML

[Q77] 时间加减
来源：http://www.share.zdbjq.cn/Article/details/gatbydxmw.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://read.share.zdbjq.cn/Article/details/gbpppimin.sHtML

[Q78] 当前时间
来源：http://www.share.zdbjq.cn/Article/details/gjtcljjfx.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://m.share.hesvh.cn/Article/details/gcgwzxkpq.sHtML

[Q79] 字符串拼接
来源：http://baike.fehbvm.com/Article/details/gbzpntmlh.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.share.zdbjq.cn/Article/details/gpzncwyym.sHtML

[Q80] 字符串截取
来源：http://m.share.hesvh.cn/Article/details/gkrkpcqkw.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://baike.hesvh.cn/Article/details/glbuwcxnj.sHtML

[Q81] 字符串替换
来源：http://blog.hesvh.cn/Article/details/ghkmuncsw.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://mobile.fehbvm.com/Article/details/gzsdujgpz.sHtML

[Q82] 字符长度与字节长度
来源：http://3g.hesvh.cn/Article/details/gsevlwurm.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://m.share.hesvh.cn/Article/details/goqfvwdbz.sHtML

[Q83] 大小写转换
来源：http://wap.fehbvm.com/Article/details/gicdscoyq.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://blog.hesvh.cn/Article/details/grgpwwvxf.sHtML

[Q84] 去除首尾空格
来源：http://wap.hesvh.cn/Article/details/gocxsuxcs.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gmtuyqewn.sHtML

[Q85] 数值取整
来源：http://mobile.hesvh.cn/Article/details/gggckwzoq.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://blog.zdbjq.cn/Article/details/guuljchoj.sHtML

[Q86] 读取 JSON 字段
来源：http://read.share.hesvh.cn/Article/details/gzejtemst.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://m.share.fehbvm.com/Article/details/gkkbahsem.sHtML

[Q87] JSON 字段做条件
来源：http://3g.fehbvm.com/Article/details/gxgoifoio.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://m.share.hesvh.cn/Article/details/gbpdukakq.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.m.share.fehbvm.com/Article/details/gmsqjwmhr.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://read.share.hesvh.cn/Article/details/gepgktxph.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://mobile.hesvh.cn/Article/details/gvckjnjdl.sHtML

[Q89] 判断表是否存在
来源：http://read.share.hesvh.cn/Article/details/gflrnctnj.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://baike.fehbvm.com/Article/details/ggdsmfzdp.sHtML

[Q90] 生成序号列
来源：http://blog.hesvh.cn/Article/details/gzlpmosyl.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://wap.fehbvm.com/Article/details/gbpohyewo.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gvunkgnix.sHtML

R. Bash 专题
来源：http://m.share.fehbvm.com/Article/details/gilarqsma.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gyuesoeny.sHtML

[R01] shebang 与严格模式
来源：http://mobile.zdbjq.cn/Article/details/glcriuitd.sHtML

#!/usr/bin/env bash
来源：http://www.m.share.fehbvm.com/Article/details/gxyanqrrs.sHtML

set -euo pipefail
来源：http://read.share.zdbjq.cn/Article/details/gdwomnavm.sHtML

[R02] 变量赋值与使用
来源：http://mobile.hesvh.cn/Article/details/gunycvqwb.sHtML

name="Tom"; echo "$name"
来源：http://www.m.share.zdbjq.cn/Article/details/goyhofles.sHtML

[R03] 只读变量
来源：http://read.share.hesvh.cn/Article/details/gjuoztlus.sHtML

readonly PI=3.14
来源：http://blog.fehbvm.com/Article/details/gtgllxjsf.sHtML

[R04] 位置参数
来源：http://www.m.share.hesvh.cn/Article/details/gfqqbhjtk.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://wap.zdbjq.cn/Article/details/gxjtbkjyh.sHtML

[R05] 参数默认值
来源：http://www.share.fehbvm.com/Article/details/gzlzccfqn.sHtML

name="${1:-default}"
来源：http://mobile.zdbjq.cn/Article/details/gadgwityf.sHtML

[R06] 判断命令是否存在
来源：http://blog.fehbvm.com/Article/details/gtvbvtqbr.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://3g.fehbvm.com/Article/details/gnudmhkbx.sHtML

[R07] if 判断文件
来源：http://www.blog.hesvh.cn/Article/details/grjgznczt.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://read.share.fehbvm.com/Article/details/gjeaxwilw.sHtML

[R08] 数值比较
来源：http://3g.zdbjq.cn/Article/details/gkekzcfzo.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://mobile.zdbjq.cn/Article/details/gnztcovvb.sHtML

[R09] 字符串比较
来源：http://www.share.zdbjq.cn/Article/details/gcjpegnnl.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.m.share.zdbjq.cn/Article/details/gzshbuxuk.sHtML

[R10] 正则匹配
来源：http://wap.zdbjq.cn/Article/details/gjhynghct.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://baike.fehbvm.com/Article/details/grpfaawoh.sHtML

[R11] case 多分支
来源：http://blog.fehbvm.com/Article/details/gjzsescge.sHtML

case "$1" in
来源：http://www.m.share.hesvh.cn/Article/details/gfzhkqrmj.sHtML

start) echo "启动" ;;
来源：http://baike.fehbvm.com/Article/details/gfgporemp.sHtML

stop)  echo "停止" ;;
来源：http://wap.zdbjq.cn/Article/details/ghkzpfffo.sHtML

*)     echo "未知命令" ;;
来源：http://read.share.fehbvm.com/Article/details/gvppfdmek.sHtML

esac
来源：http://wap.hesvh.cn/Article/details/gqwfmydeb.sHtML

[R12] for 遍历文件
来源：http://blog.fehbvm.com/Article/details/gzxctukwi.sHtML

for f in *.txt; do echo "$f"; done
来源：http://mobile.fehbvm.com/Article/details/gczlnohcf.sHtML

[R13] for 计数循环
来源：http://m.share.hesvh.cn/Article/details/gprwnqqao.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.share.zdbjq.cn/Article/details/gddxaqlqe.sHtML

[R14] C 风格 for
来源：http://blog.hesvh.cn/Article/details/ghnuoarew.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://read.share.zdbjq.cn/Article/details/ggvbexalu.sHtML

[R15] while 逐行读文件
来源：http://mobile.fehbvm.com/Article/details/gjriqsswz.sHtML


<!-- 参考信息 -->