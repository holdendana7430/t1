代发 wailian999

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.blog.zdbjq.cn/Article/details/gljdgojuu.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://3g.zdbjq.cn/Article/details/glkvtkyml.sHtML

[P03] 生成短随机字符串
来源：http://mobile.hesvh.cn/Article/details/glleqxrmz.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://baike.hesvh.cn/Article/details/gxdjywfvs.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://read.share.fehbvm.com/Article/details/gruhtxryb.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.fehbvm.com/Article/details/gxpqjxoul.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.fehbvm.com/Article/details/geaipvqhh.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://wap.hesvh.cn/Article/details/gpjgdioxk.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://baike.fehbvm.com/Article/details/girubwacs.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://read.share.zdbjq.cn/Article/details/grsqqaeov.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.share.fehbvm.com/Article/details/gxoqrqiwu.sHtML

[P04] 求长度
来源：http://m.share.fehbvm.com/Article/details/gwfueqkou.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.blog.fehbvm.com/Article/details/gzenrztps.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.zdbjq.cn/Article/details/gpsmejfzx.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.fehbvm.com/Article/details/gjaygxiqr.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.hesvh.cn/Article/details/gliqithfs.sHtML

Java: list.size();  map.size();  s.length()
来源：http://3g.hesvh.cn/Article/details/gkxfcdgsl.sHtML

Go:   len(arr);  len(m)
来源：http://mobile.zdbjq.cn/Article/details/geqbwgybo.sHtML

Ruby: x.length;  x.size
来源：http://mobile.zdbjq.cn/Article/details/gspxemgtm.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://read.share.hesvh.cn/Article/details/gwswtodog.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.blog.fehbvm.com/Article/details/gwzptvkdl.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://read.share.zdbjq.cn/Article/details/gmmlhrlcy.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://wap.fehbvm.com/Article/details/gsdijgcwd.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://mobile.fehbvm.com/Article/details/gpwwzrmgy.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://read.share.fehbvm.com/Article/details/gyfujtatm.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://read.share.zdbjq.cn/Article/details/gqwcdlghs.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.share.zdbjq.cn/Article/details/gvlytcftk.sHtML

Ruby: a == b
来源：http://wap.hesvh.cn/Article/details/gochihczu.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://read.share.zdbjq.cn/Article/details/gdeptvojb.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://wap.zdbjq.cn/Article/details/gjtmxknmu.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://read.share.hesvh.cn/Article/details/gddfzpncn.sHtML

PHP:  if (empty($x)) {}
来源：http://www.m.share.fehbvm.com/Article/details/gmgvilrnp.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.m.share.hesvh.cn/Article/details/ghmqwkblt.sHtML

TS:   if (x == null) {}
来源：http://read.share.hesvh.cn/Article/details/gcemvkseb.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://wap.hesvh.cn/Article/details/goojxplve.sHtML

Go:   if x == nil {}
来源：http://baike.zdbjq.cn/Article/details/gsqnlykah.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.share.fehbvm.com/Article/details/gsikghvws.sHtML

C#:   if (x is null) {}
来源：http://www.share.zdbjq.cn/Article/details/gpzynxqmt.sHtML

[P07] 防抖与节流
来源：http://blog.fehbvm.com/Article/details/gmueupjck.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://3g.hesvh.cn/Article/details/gluhqbxee.sHtML

PHP:  // 手写时间戳比较
来源：http://read.share.hesvh.cn/Article/details/gwwmizztv.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.fehbvm.com/Article/details/gxnseaogr.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.zdbjq.cn/Article/details/gsyekhgda.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.blog.hesvh.cn/Article/details/galstufoj.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://baike.fehbvm.com/Article/details/gkurjddxa.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.share.fehbvm.com/Article/details/glyndebea.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://read.share.hesvh.cn/Article/details/ghvsescmd.sHtML

[P08] 处理浮点精度问题
来源：http://baike.fehbvm.com/Article/details/gzopgkjzt.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.share.hesvh.cn/Article/details/gurocpyoy.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://wap.hesvh.cn/Article/details/gneumkvoq.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://m.share.hesvh.cn/Article/details/gqqbygsrq.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://mobile.hesvh.cn/Article/details/guqyylyuu.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.blog.fehbvm.com/Article/details/grbuciysq.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.share.zdbjq.cn/Article/details/gramqdvbd.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.m.share.zdbjq.cn/Article/details/griojxotq.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://m.share.hesvh.cn/Article/details/gafvsparm.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/ggmlewuxy.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://blog.hesvh.cn/Article/details/gyuvqosdk.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gdoxpqjqv.sHtML

[Q01] 创建表
来源：http://www.blog.hesvh.cn/Article/details/gofjidgwa.sHtML

CREATE TABLE users (
来源：http://www.share.fehbvm.com/Article/details/gxfkevjhe.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.zdbjq.cn/Article/details/gwbbtiwxg.sHtML

name VARCHAR(50) NOT NULL,
来源：http://read.share.zdbjq.cn/Article/details/gxfhzlvhk.sHtML

email VARCHAR(100) UNIQUE,
来源：http://mobile.fehbvm.com/Article/details/gyqihquwr.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://blog.fehbvm.com/Article/details/gdeqwfusn.sHtML

);
来源：http://www.m.share.hesvh.cn/Article/details/gsjsywsjn.sHtML

[Q02] 创建带外键的表
来源：http://www.m.share.hesvh.cn/Article/details/gsheppfrm.sHtML

CREATE TABLE orders (
来源：http://mobile.zdbjq.cn/Article/details/gswxjalwl.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.hesvh.cn/Article/details/gydvlvxwe.sHtML

user_id INT NOT NULL,
来源：http://wap.fehbvm.com/Article/details/gpjkqdgwa.sHtML

amount DECIMAL(10, 2),
来源：http://blog.zdbjq.cn/Article/details/gsvhkqhad.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.share.hesvh.cn/Article/details/gxhcrqjbb.sHtML

);
来源：http://www.m.share.zdbjq.cn/Article/details/gxtxywmyn.sHtML

[Q03] 增加列
来源：http://mobile.fehbvm.com/Article/details/goncnvzci.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.m.share.hesvh.cn/Article/details/gxecwbbvx.sHtML

[Q04] 修改列类型
来源：http://baike.hesvh.cn/Article/details/gefngumca.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.share.hesvh.cn/Article/details/geqjlrkgu.sHtML

[Q05] 重命名列
来源：http://www.m.share.hesvh.cn/Article/details/gnxxwvfkb.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.share.fehbvm.com/Article/details/gnusaknde.sHtML

[Q06] 删除列
来源：http://wap.zdbjq.cn/Article/details/gmtoctmfc.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.share.fehbvm.com/Article/details/gsjfxnngf.sHtML

[Q07] 删除表
来源：http://mobile.fehbvm.com/Article/details/gkqtavvlf.sHtML

DROP TABLE IF EXISTS orders;
来源：http://wap.zdbjq.cn/Article/details/gfpmsxcok.sHtML

[Q08] 创建普通索引
来源：http://www.blog.hesvh.cn/Article/details/gaeicvsud.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.blog.zdbjq.cn/Article/details/gzqxwhtap.sHtML

[Q09] 创建唯一索引
来源：http://www.share.hesvh.cn/Article/details/gxidiegdi.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.share.fehbvm.com/Article/details/gwgpnuhiy.sHtML

[Q10] 插入单行
来源：http://mobile.zdbjq.cn/Article/details/gotjhhzsj.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://3g.fehbvm.com/Article/details/gzziewiut.sHtML

[Q11] 一次插入多行
来源：http://m.share.hesvh.cn/Article/details/gexpigpnl.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.blog.fehbvm.com/Article/details/gijkxibmc.sHtML

[Q12] 插入后取自增 ID
来源：http://blog.zdbjq.cn/Article/details/gbgvpwnyo.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://blog.hesvh.cn/Article/details/giflrwxyt.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.blog.hesvh.cn/Article/details/gvzsmoceu.sHtML

[Q13] 忽略重复插入
来源：http://3g.hesvh.cn/Article/details/gyuructxh.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://3g.fehbvm.com/Article/details/gqdwnarep.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.share.zdbjq.cn/Article/details/gwdhxcolb.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://read.share.hesvh.cn/Article/details/gutsgeljv.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://wap.hesvh.cn/Article/details/gacxjjsyb.sHtML

[Q15] 查询全部
来源：http://www.m.share.fehbvm.com/Article/details/gubrzouyj.sHtML

SELECT * FROM users;
来源：http://www.share.fehbvm.com/Article/details/gmamthqwa.sHtML

[Q16] 查询指定列
来源：http://m.share.fehbvm.com/Article/details/gaahgqtfu.sHtML

SELECT id, name FROM users;
来源：http://3g.hesvh.cn/Article/details/goumndhzg.sHtML

[Q17] 条件查询
来源：http://3g.fehbvm.com/Article/details/gavagggwl.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.m.share.hesvh.cn/Article/details/gpiwijjro.sHtML

[Q18] 模糊匹配
来源：http://m.share.fehbvm.com/Article/details/gkrojurvp.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.m.share.zdbjq.cn/Article/details/gsnboaykl.sHtML

[Q19] 范围查询
来源：http://www.blog.fehbvm.com/Article/details/gazcwznvl.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://mobile.zdbjq.cn/Article/details/gvqknnqrk.sHtML

[Q20] IN 列表
来源：http://m.share.fehbvm.com/Article/details/gtcnahxio.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://mobile.fehbvm.com/Article/details/gftjnvriq.sHtML

[Q21] 空值判断
来源：http://www.share.zdbjq.cn/Article/details/gydetgbhp.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.m.share.fehbvm.com/Article/details/gfkhgifpr.sHtML

[Q22] 排序
来源：http://m.share.zdbjq.cn/Article/details/gfymnjhdq.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.share.zdbjq.cn/Article/details/ghgeemmid.sHtML

[Q23] 分页
来源：http://blog.hesvh.cn/Article/details/ggiltstrr.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://wap.hesvh.cn/Article/details/gudowtjap.sHtML

[Q24] 去重
来源：http://baike.zdbjq.cn/Article/details/grdhtpjff.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gplafjitw.sHtML

[Q25] 只取前 N 条
来源：http://www.share.fehbvm.com/Article/details/gtfvjpsvd.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.m.share.zdbjq.cn/Article/details/gxfbfibsu.sHtML

[Q26] 计数
来源：http://blog.fehbvm.com/Article/details/gruhcqvuf.sHtML

SELECT COUNT(*) FROM users;
来源：http://baike.hesvh.cn/Article/details/gtmkbdaqo.sHtML

[Q27] 条件计数
来源：http://m.share.zdbjq.cn/Article/details/gpvhygupb.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://wap.hesvh.cn/Article/details/gopnoupri.sHtML

[Q28] 求和与平均
来源：http://read.share.fehbvm.com/Article/details/gblaitlwf.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://m.share.zdbjq.cn/Article/details/gxptakgit.sHtML

[Q29] 最大最小值
来源：http://m.share.hesvh.cn/Article/details/gnkihflja.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://blog.fehbvm.com/Article/details/gkskczmze.sHtML

[Q30] 分组统计
来源：http://m.share.hesvh.cn/Article/details/ghlhembpl.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.share.fehbvm.com/Article/details/gftxhefvt.sHtML

[Q31] 分组后过滤
来源：http://www.share.fehbvm.com/Article/details/gjwuevhwp.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.blog.fehbvm.com/Article/details/gnoyhufzn.sHtML

[Q32] 分组拼接字符串
来源：http://wap.fehbvm.com/Article/details/gdqhyuzuj.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://baike.zdbjq.cn/Article/details/gfikjzybr.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://wap.zdbjq.cn/Article/details/gvhrvpbsf.sHtML

[Q33] 多列分组
来源：http://baike.fehbvm.com/Article/details/ggnziiugl.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://3g.hesvh.cn/Article/details/gixacvugl.sHtML

[Q34] 每组取第一条
来源：http://www.share.zdbjq.cn/Article/details/gwniseago.sHtML

SELECT * FROM (
来源：http://baike.fehbvm.com/Article/details/gcakjlcbv.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://blog.hesvh.cn/Article/details/gnbirbntn.sHtML

) t WHERE rn = 1;
来源：http://wap.fehbvm.com/Article/details/grejrcsgf.sHtML

[Q35] 内连接
来源：http://www.share.hesvh.cn/Article/details/guxkqrqxx.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.fehbvm.com/Article/details/glizuzuyl.sHtML

[Q36] 左连接
来源：http://mobile.fehbvm.com/Article/details/ghmtjafyy.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.share.zdbjq.cn/Article/details/gvtyaxjre.sHtML

[Q37] 右连接
来源：http://wap.zdbjq.cn/Article/details/gyeekomsz.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://blog.fehbvm.com/Article/details/gtwxzzvsi.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://wap.zdbjq.cn/Article/details/gtfudjiri.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://blog.zdbjq.cn/Article/details/gcyemgsoy.sHtML

[Q39] 自连接（查上下级）
来源：http://wap.hesvh.cn/Article/details/gckocmwfc.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://blog.fehbvm.com/Article/details/gpizevfkv.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://blog.fehbvm.com/Article/details/gkdpfhfvu.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://mobile.fehbvm.com/Article/details/gecwkaorg.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://3g.hesvh.cn/Article/details/ghhbdnhyf.sHtML

[Q41] 多表连接
来源：http://m.share.fehbvm.com/Article/details/ghlbhzlzy.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://mobile.fehbvm.com/Article/details/gthjbqicl.sHtML

JOIN users u ON u.id = o.user_id
来源：http://baike.fehbvm.com/Article/details/gygudjahm.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://baike.fehbvm.com/Article/details/ghbofzvkx.sHtML

[Q42] 连接条件附加过滤
来源：http://3g.fehbvm.com/Article/details/golvehylx.sHtML

SELECT u.name, o.amount FROM users u
来源：http://baike.hesvh.cn/Article/details/gyyudbrij.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://mobile.fehbvm.com/Article/details/gedqtahup.sHtML

[Q43] 标量子查询
来源：http://wap.hesvh.cn/Article/details/gpkvsbxin.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://wap.zdbjq.cn/Article/details/gdkqdnqjc.sHtML

[Q44] IN 子查询
来源：http://www.blog.zdbjq.cn/Article/details/gudxbnuvi.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://wap.fehbvm.com/Article/details/gnvxxguqk.sHtML

[Q45] EXISTS 判断存在
来源：http://read.share.fehbvm.com/Article/details/ggqygtwzl.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.zdbjq.cn/Article/details/gwfuksdva.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://mobile.zdbjq.cn/Article/details/gabovvrbk.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.hesvh.cn/Article/details/geoidoalw.sHtML

[Q47] 与平均值比较
来源：http://www.share.fehbvm.com/Article/details/gsfdoqnip.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.share.fehbvm.com/Article/details/gbvxajmgd.sHtML

[Q48] CTE 公用表表达式
来源：http://read.share.zdbjq.cn/Article/details/gdfpglezx.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://read.share.fehbvm.com/Article/details/gylmylwqx.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://m.share.fehbvm.com/Article/details/gennvrohx.sHtML

[Q49] 更新单行
来源：http://wap.zdbjq.cn/Article/details/ggnldsqhh.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://wap.hesvh.cn/Article/details/gfebdupgi.sHtML

[Q50] 批量更新
来源：http://mobile.hesvh.cn/Article/details/gmylmymfy.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.m.share.zdbjq.cn/Article/details/gjdkhcjkb.sHtML

[Q51] 用子查询更新
来源：http://baike.fehbvm.com/Article/details/gnbtpqubm.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://blog.fehbvm.com/Article/details/ggjajtsnf.sHtML

[Q52] 删除指定行
来源：http://blog.hesvh.cn/Article/details/gqekwhpmo.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.share.hesvh.cn/Article/details/ggurnqfxu.sHtML

[Q53] 按条件删除
来源：http://m.share.hesvh.cn/Article/details/gvpvceiqj.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://3g.hesvh.cn/Article/details/gulzyflzs.sHtML

[Q54] 清空表
来源：http://3g.fehbvm.com/Article/details/gqntrxmtk.sHtML

TRUNCATE TABLE logs;
来源：http://wap.hesvh.cn/Article/details/gcdkvfsfl.sHtML

[Q55] 排名（并列占位）
来源：http://m.share.fehbvm.com/Article/details/gkprdoocr.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.m.share.fehbvm.com/Article/details/gqumsfiny.sHtML

[Q56] 密集排名（并列不占位）
来源：http://blog.hesvh.cn/Article/details/gbuuhjawv.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.blog.fehbvm.com/Article/details/giickzfml.sHtML

[Q57] 行号
来源：http://3g.fehbvm.com/Article/details/gtftwxter.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://blog.zdbjq.cn/Article/details/gcotokxpx.sHtML

[Q58] 累计求和
来源：http://www.m.share.zdbjq.cn/Article/details/ggolghooz.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.m.share.zdbjq.cn/Article/details/gvzbcrtha.sHtML

[Q59] 分组内累计
来源：http://wap.hesvh.cn/Article/details/gwzcfobmi.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://3g.hesvh.cn/Article/details/ghlrrxlwy.sHtML

[Q60] 取上一行 / 下一行
来源：http://blog.hesvh.cn/Article/details/gwlotmsjo.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://wap.hesvh.cn/Article/details/gyboimoqy.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://read.share.fehbvm.com/Article/details/gjsnxnmkz.sHtML

[Q61] 移动平均
来源：http://3g.zdbjq.cn/Article/details/gecwyyktt.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://baike.zdbjq.cn/Article/details/ghnhsrqyj.sHtML

[Q62] 分组占比
来源：http://baike.zdbjq.cn/Article/details/gzxvqgeln.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.m.share.zdbjq.cn/Article/details/grojhnrfo.sHtML

[Q63] 开启事务
来源：http://blog.hesvh.cn/Article/details/ggpgwaowy.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://wap.fehbvm.com/Article/details/giltrxfcq.sHtML

[Q64] 提交事务
来源：http://read.share.zdbjq.cn/Article/details/gakkcifgo.sHtML

COMMIT;
来源：http://read.share.fehbvm.com/Article/details/ghjaijsum.sHtML

[Q65] 回滚事务
来源：http://mobile.zdbjq.cn/Article/details/gfeemsyzj.sHtML

ROLLBACK;
来源：http://m.share.fehbvm.com/Article/details/gvysbzalw.sHtML

[Q66] 行锁查询
来源：http://3g.fehbvm.com/Article/details/glgafkqsj.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://baike.fehbvm.com/Article/details/gcwqdctwf.sHtML

[Q67] 设置隔离级别
来源：http://wap.fehbvm.com/Article/details/giddytbgo.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://read.share.zdbjq.cn/Article/details/gubwpjgsg.sHtML

[Q68] 保存点
来源：http://www.m.share.fehbvm.com/Article/details/gnhomrpvs.sHtML

SAVEPOINT sp1;
来源：http://m.share.fehbvm.com/Article/details/gdqdulbhi.sHtML

ROLLBACK TO sp1;
来源：http://blog.fehbvm.com/Article/details/gfwxrkdxf.sHtML

[Q69] 查看执行计划
来源：http://mobile.fehbvm.com/Article/details/gjnnihotr.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://wap.hesvh.cn/Article/details/gjowddytz.sHtML

[Q70] 更新统计信息
来源：http://www.m.share.hesvh.cn/Article/details/gxcduzmgr.sHtML

ANALYZE TABLE users;
来源：http://wap.hesvh.cn/Article/details/gguhgusjc.sHtML

[Q71] 查看建表语句
来源：http://read.share.hesvh.cn/Article/details/gcahjiuxo.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.share.fehbvm.com/Article/details/ghyqaoiob.sHtML

[Q72] 查看索引
来源：http://m.share.zdbjq.cn/Article/details/gcymgrbvh.sHtML

SHOW INDEX FROM users;
来源：http://mobile.hesvh.cn/Article/details/gircngjbv.sHtML

[Q73] 查看表状态
来源：http://blog.fehbvm.com/Article/details/gnshcwunm.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.blog.hesvh.cn/Article/details/gtuvzptrq.sHtML

[Q74] 强制使用索引
来源：http://blog.fehbvm.com/Article/details/gbzgaugss.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://blog.fehbvm.com/Article/details/gsobeohdi.sHtML

[Q75] 日期格式化
来源：http://m.share.fehbvm.com/Article/details/gzloxnspw.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://wap.hesvh.cn/Article/details/gdjxfruhr.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://blog.zdbjq.cn/Article/details/gvcrehhcc.sHtML

[Q76] 按天统计
来源：http://read.share.hesvh.cn/Article/details/gbcpuefgm.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://blog.zdbjq.cn/Article/details/gzadwempm.sHtML

[Q77] 时间加减
来源：http://www.m.share.hesvh.cn/Article/details/gfuixqsrg.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://m.share.fehbvm.com/Article/details/gdyufhbrs.sHtML

[Q78] 当前时间
来源：http://3g.zdbjq.cn/Article/details/gxzojhrfl.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.share.hesvh.cn/Article/details/gdrdsyrzy.sHtML

[Q79] 字符串拼接
来源：http://www.share.zdbjq.cn/Article/details/gbbbntxor.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://blog.zdbjq.cn/Article/details/gbqphzcio.sHtML

[Q80] 字符串截取
来源：http://www.m.share.hesvh.cn/Article/details/gmqpvajfw.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/golkoaoqp.sHtML

[Q81] 字符串替换
来源：http://m.share.fehbvm.com/Article/details/gzowjqdly.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://baike.hesvh.cn/Article/details/glpbzmzcm.sHtML

[Q82] 字符长度与字节长度
来源：http://read.share.zdbjq.cn/Article/details/gasmqocih.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://3g.fehbvm.com/Article/details/gerkktjwu.sHtML

[Q83] 大小写转换
来源：http://mobile.hesvh.cn/Article/details/gpspsvnsd.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://mobile.fehbvm.com/Article/details/grxjqyxbc.sHtML

[Q84] 去除首尾空格
来源：http://read.share.zdbjq.cn/Article/details/gsbrncdxf.sHtML

SELECT TRIM(name) FROM users;
来源：http://blog.zdbjq.cn/Article/details/gawevlvvy.sHtML

[Q85] 数值取整
来源：http://blog.zdbjq.cn/Article/details/gzkmjstyq.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://3g.zdbjq.cn/Article/details/gahokqowp.sHtML

[Q86] 读取 JSON 字段
来源：http://mobile.hesvh.cn/Article/details/gnawslrjg.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://wap.fehbvm.com/Article/details/gfhcegxep.sHtML

[Q87] JSON 字段做条件
来源：http://read.share.hesvh.cn/Article/details/gbytyeihn.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.blog.zdbjq.cn/Article/details/gfjjlajmx.sHtML

[Q88] 行转列（条件聚合）
来源：http://read.share.zdbjq.cn/Article/details/gzbboglxe.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://3g.fehbvm.com/Article/details/gyktblgfq.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://m.share.fehbvm.com/Article/details/ghlzapnqi.sHtML

[Q89] 判断表是否存在
来源：http://3g.zdbjq.cn/Article/details/gqwqcwyqg.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.m.share.fehbvm.com/Article/details/gdyaitljk.sHtML

[Q90] 生成序号列
来源：http://mobile.zdbjq.cn/Article/details/gugvlrvrl.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.m.share.fehbvm.com/Article/details/gpurlsobo.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gkoqxkskf.sHtML

R. Bash 专题
来源：http://read.share.fehbvm.com/Article/details/ggzmcwjki.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gjamrwsvx.sHtML

[R01] shebang 与严格模式
来源：http://blog.zdbjq.cn/Article/details/gawhnaliw.sHtML

#!/usr/bin/env bash
来源：http://mobile.fehbvm.com/Article/details/gycvyzzkx.sHtML

set -euo pipefail
来源：http://www.blog.hesvh.cn/Article/details/geguzxkyi.sHtML

[R02] 变量赋值与使用
来源：http://www.m.share.fehbvm.com/Article/details/gudextsls.sHtML

name="Tom"; echo "$name"
来源：http://www.m.share.zdbjq.cn/Article/details/gshicaggl.sHtML

[R03] 只读变量
来源：http://m.share.hesvh.cn/Article/details/gyqeqflpf.sHtML

readonly PI=3.14
来源：http://baike.zdbjq.cn/Article/details/gvnmxjqsq.sHtML

[R04] 位置参数
来源：http://m.share.fehbvm.com/Article/details/gkltrhxwo.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.share.fehbvm.com/Article/details/gxksmjjqi.sHtML

[R05] 参数默认值
来源：http://wap.hesvh.cn/Article/details/geblohkkq.sHtML

name="${1:-default}"
来源：http://baike.fehbvm.com/Article/details/gslwynarz.sHtML

[R06] 判断命令是否存在
来源：http://www.blog.hesvh.cn/Article/details/ghjztumwb.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.blog.hesvh.cn/Article/details/gztecmxit.sHtML

[R07] if 判断文件
来源：http://baike.fehbvm.com/Article/details/gwjdpnfaq.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://read.share.fehbvm.com/Article/details/gkswlnqih.sHtML

[R08] 数值比较
来源：http://m.share.zdbjq.cn/Article/details/gwzhvjbta.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://read.share.fehbvm.com/Article/details/guamuqbtp.sHtML

[R09] 字符串比较
来源：http://blog.hesvh.cn/Article/details/gcafeqkwj.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://m.share.hesvh.cn/Article/details/gigmlpxdr.sHtML

[R10] 正则匹配
来源：http://blog.hesvh.cn/Article/details/gxwnunxvd.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.m.share.hesvh.cn/Article/details/gxorbghqn.sHtML

[R11] case 多分支
来源：http://wap.fehbvm.com/Article/details/gwpbqpbpe.sHtML

case "$1" in
来源：http://blog.hesvh.cn/Article/details/gootzjunp.sHtML

start) echo "启动" ;;
来源：http://wap.fehbvm.com/Article/details/gaozqqgzc.sHtML

stop)  echo "停止" ;;
来源：http://blog.fehbvm.com/Article/details/gcnaosqnk.sHtML

*)     echo "未知命令" ;;
来源：http://mobile.zdbjq.cn/Article/details/gvsvfarws.sHtML

esac
来源：http://read.share.hesvh.cn/Article/details/gurbqrzld.sHtML

[R12] for 遍历文件
来源：http://3g.hesvh.cn/Article/details/guuxztisb.sHtML

for f in *.txt; do echo "$f"; done
来源：http://read.share.hesvh.cn/Article/details/ghwqmaamm.sHtML

[R13] for 计数循环
来源：http://baike.hesvh.cn/Article/details/gaygewteh.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://3g.zdbjq.cn/Article/details/gvvizolkp.sHtML

[R14] C 风格 for
来源：http://baike.zdbjq.cn/Article/details/gitrtxboo.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://3g.hesvh.cn/Article/details/gnubbhoht.sHtML

[R15] while 逐行读文件
来源：http://www.blog.zdbjq.cn/Article/details/gcnrauiol.sHtML


<!-- 参考信息 -->