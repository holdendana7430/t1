代发 wailian999

Ruby: Digest::SHA256.hexdigest(s)
来源：http://blog.hesvh.cn/Article/details/gipgkddvo.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://wap.fehbvm.com/Article/details/gwslwlizs.sHtML

[P03] 生成短随机字符串
来源：http://read.share.fehbvm.com/Article/details/gmpbwsnjm.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://m.share.fehbvm.com/Article/details/gjdmtstev.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://read.share.hesvh.cn/Article/details/gjbkigepo.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.zdbjq.cn/Article/details/gdpnwakom.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.hesvh.cn/Article/details/gmlbctjqw.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://read.share.fehbvm.com/Article/details/gxomqpccu.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.m.share.fehbvm.com/Article/details/gmfbxznwf.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://3g.fehbvm.com/Article/details/gvlknpqnx.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://3g.zdbjq.cn/Article/details/gqirhxnfa.sHtML

[P04] 求长度
来源：http://www.blog.zdbjq.cn/Article/details/gcfxsacon.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://wap.hesvh.cn/Article/details/gvsptkfxf.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.fehbvm.com/Article/details/gsoidmsxm.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.fehbvm.com/Article/details/gfbumkpwf.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.fehbvm.com/Article/details/gndxncpzv.sHtML

Java: list.size();  map.size();  s.length()
来源：http://3g.fehbvm.com/Article/details/guqedvsal.sHtML

Go:   len(arr);  len(m)
来源：http://mobile.fehbvm.com/Article/details/gfoffxleq.sHtML

Ruby: x.length;  x.size
来源：http://blog.fehbvm.com/Article/details/glhghsdef.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.m.share.hesvh.cn/Article/details/gmefihqoo.sHtML

[P05] 判断两个对象内容是否相等
来源：http://mobile.fehbvm.com/Article/details/gmtsvjbma.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://mobile.fehbvm.com/Article/details/gmkaucjwy.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://baike.fehbvm.com/Article/details/gmwokloky.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://3g.zdbjq.cn/Article/details/gbrwistra.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.share.zdbjq.cn/Article/details/gddfhxrai.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://m.share.fehbvm.com/Article/details/gipjyvpfy.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://mobile.fehbvm.com/Article/details/gwulqlixl.sHtML

Ruby: a == b
来源：http://3g.zdbjq.cn/Article/details/gxirflssc.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://baike.fehbvm.com/Article/details/gmcvjbodk.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.m.share.hesvh.cn/Article/details/gfwszyccn.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.share.hesvh.cn/Article/details/ggmfnkvrv.sHtML

PHP:  if (empty($x)) {}
来源：http://baike.fehbvm.com/Article/details/gedkegulr.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://baike.hesvh.cn/Article/details/gkfmvbtsg.sHtML

TS:   if (x == null) {}
来源：http://www.blog.hesvh.cn/Article/details/gelyyirwn.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.m.share.fehbvm.com/Article/details/gtahhccyx.sHtML

Go:   if x == nil {}
来源：http://wap.zdbjq.cn/Article/details/gxtckqtpk.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://wap.zdbjq.cn/Article/details/gzbaixnwk.sHtML

C#:   if (x is null) {}
来源：http://www.share.hesvh.cn/Article/details/gytvelwbe.sHtML

[P07] 防抖与节流
来源：http://www.share.zdbjq.cn/Article/details/gaqkjqkpc.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.share.hesvh.cn/Article/details/gmqaqpuvq.sHtML

PHP:  // 手写时间戳比较
来源：http://baike.zdbjq.cn/Article/details/gjiwlxior.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.zdbjq.cn/Article/details/gkhhnbtut.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.zdbjq.cn/Article/details/gfuhkwdtw.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://blog.hesvh.cn/Article/details/gorhnqnee.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.m.share.hesvh.cn/Article/details/gvadjrxna.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://baike.zdbjq.cn/Article/details/ghphfirlf.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://baike.fehbvm.com/Article/details/gyhuitltu.sHtML

[P08] 处理浮点精度问题
来源：http://www.share.zdbjq.cn/Article/details/gtxhuzkcb.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.share.fehbvm.com/Article/details/ginddmnjz.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://mobile.fehbvm.com/Article/details/gzteweukm.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.share.zdbjq.cn/Article/details/gyogtlaad.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://baike.fehbvm.com/Article/details/gmguidnnn.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://read.share.zdbjq.cn/Article/details/guxbfmpma.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.blog.hesvh.cn/Article/details/gphgflnro.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.share.hesvh.cn/Article/details/gjpkzgnej.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://wap.hesvh.cn/Article/details/ggisdpctq.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gzvoeegnw.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.blog.hesvh.cn/Article/details/gkqzkpgdk.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gtomfoivs.sHtML

[Q01] 创建表
来源：http://read.share.zdbjq.cn/Article/details/gjqhmhnbz.sHtML

CREATE TABLE users (
来源：http://baike.hesvh.cn/Article/details/gnboesvbn.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.zdbjq.cn/Article/details/gflygudgy.sHtML

name VARCHAR(50) NOT NULL,
来源：http://baike.zdbjq.cn/Article/details/gpmxqafig.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.blog.zdbjq.cn/Article/details/gjasfdibn.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://mobile.fehbvm.com/Article/details/gghnjbhvo.sHtML

);
来源：http://blog.fehbvm.com/Article/details/gevyfkiws.sHtML

[Q02] 创建带外键的表
来源：http://wap.zdbjq.cn/Article/details/gulwzpcnt.sHtML

CREATE TABLE orders (
来源：http://m.share.hesvh.cn/Article/details/gdcdltoao.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.hesvh.cn/Article/details/gcxearcuv.sHtML

user_id INT NOT NULL,
来源：http://wap.fehbvm.com/Article/details/gukggucgj.sHtML

amount DECIMAL(10, 2),
来源：http://blog.hesvh.cn/Article/details/gyxazljtx.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://blog.hesvh.cn/Article/details/geczxwiru.sHtML

);
来源：http://www.blog.hesvh.cn/Article/details/gsnhfbhzx.sHtML

[Q03] 增加列
来源：http://3g.fehbvm.com/Article/details/gbrlmltkv.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://blog.zdbjq.cn/Article/details/gcxtcdpcx.sHtML

[Q04] 修改列类型
来源：http://m.share.fehbvm.com/Article/details/gkjnnwfhn.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://3g.hesvh.cn/Article/details/gfgfgtach.sHtML

[Q05] 重命名列
来源：http://3g.fehbvm.com/Article/details/gtyfthyyv.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://baike.hesvh.cn/Article/details/gnkatyzmr.sHtML

[Q06] 删除列
来源：http://blog.zdbjq.cn/Article/details/gorksjyyv.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.m.share.fehbvm.com/Article/details/gshtwizid.sHtML

[Q07] 删除表
来源：http://blog.zdbjq.cn/Article/details/ghkqzhmgy.sHtML

DROP TABLE IF EXISTS orders;
来源：http://read.share.fehbvm.com/Article/details/gdlfmzsbg.sHtML

[Q08] 创建普通索引
来源：http://www.blog.hesvh.cn/Article/details/gshqsxzqq.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.m.share.hesvh.cn/Article/details/gqiizvzvn.sHtML

[Q09] 创建唯一索引
来源：http://3g.fehbvm.com/Article/details/gbgnsnsbu.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.m.share.hesvh.cn/Article/details/ggrplvlns.sHtML

[Q10] 插入单行
来源：http://mobile.zdbjq.cn/Article/details/gczcqfwfk.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://read.share.hesvh.cn/Article/details/gnljbopzy.sHtML

[Q11] 一次插入多行
来源：http://wap.hesvh.cn/Article/details/gzclmwcjq.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://baike.hesvh.cn/Article/details/gzsrefyvz.sHtML

[Q12] 插入后取自增 ID
来源：http://read.share.hesvh.cn/Article/details/gnawaawrx.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://m.share.hesvh.cn/Article/details/gelszpeev.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://m.share.hesvh.cn/Article/details/gwughwgex.sHtML

[Q13] 忽略重复插入
来源：http://m.share.fehbvm.com/Article/details/gnsszbaov.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://m.share.zdbjq.cn/Article/details/gxqgvsihg.sHtML

[Q14] 存在则更新（upsert）
来源：http://m.share.zdbjq.cn/Article/details/gzkqrobrl.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://3g.hesvh.cn/Article/details/gimaawevx.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.share.hesvh.cn/Article/details/gnayvfsou.sHtML

[Q15] 查询全部
来源：http://www.blog.fehbvm.com/Article/details/gxhplmcbf.sHtML

SELECT * FROM users;
来源：http://m.share.fehbvm.com/Article/details/gdrvsmsto.sHtML

[Q16] 查询指定列
来源：http://3g.zdbjq.cn/Article/details/gyxlkvrvy.sHtML

SELECT id, name FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/ggkdkhfus.sHtML

[Q17] 条件查询
来源：http://wap.fehbvm.com/Article/details/ggimkbcsq.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://wap.fehbvm.com/Article/details/gvprnkdaw.sHtML

[Q18] 模糊匹配
来源：http://baike.zdbjq.cn/Article/details/guryxoopw.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.blog.fehbvm.com/Article/details/gxlanvtzv.sHtML

[Q19] 范围查询
来源：http://www.share.hesvh.cn/Article/details/glqywstwl.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://mobile.fehbvm.com/Article/details/gznkqnrjy.sHtML

[Q20] IN 列表
来源：http://m.share.hesvh.cn/Article/details/gafrupcuy.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://baike.zdbjq.cn/Article/details/greznwcxp.sHtML

[Q21] 空值判断
来源：http://baike.fehbvm.com/Article/details/gvorghiuy.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://m.share.hesvh.cn/Article/details/gmbldfqmi.sHtML

[Q22] 排序
来源：http://www.blog.hesvh.cn/Article/details/gdxxwitpq.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://3g.hesvh.cn/Article/details/gvangghkc.sHtML

[Q23] 分页
来源：http://read.share.fehbvm.com/Article/details/gvsalxsvh.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.m.share.hesvh.cn/Article/details/ggrrmyutc.sHtML

[Q24] 去重
来源：http://mobile.fehbvm.com/Article/details/gdibziqes.sHtML

SELECT DISTINCT city FROM users;
来源：http://read.share.fehbvm.com/Article/details/gyfhcwofu.sHtML

[Q25] 只取前 N 条
来源：http://baike.fehbvm.com/Article/details/gzpcdkebq.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.share.hesvh.cn/Article/details/gzdpjdbkh.sHtML

[Q26] 计数
来源：http://3g.hesvh.cn/Article/details/gaktpldev.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.share.fehbvm.com/Article/details/gnfbcxuwx.sHtML

[Q27] 条件计数
来源：http://m.share.hesvh.cn/Article/details/gakepztkz.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://baike.fehbvm.com/Article/details/gtpzgfhef.sHtML

[Q28] 求和与平均
来源：http://www.blog.fehbvm.com/Article/details/gljgmuuog.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.m.share.zdbjq.cn/Article/details/gcjkpdlyf.sHtML

[Q29] 最大最小值
来源：http://m.share.fehbvm.com/Article/details/ghatpodxh.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://blog.fehbvm.com/Article/details/gtzikydku.sHtML

[Q30] 分组统计
来源：http://read.share.fehbvm.com/Article/details/grkvovqqj.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://baike.fehbvm.com/Article/details/gmjdyyqnd.sHtML

[Q31] 分组后过滤
来源：http://read.share.hesvh.cn/Article/details/guozwmodo.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://mobile.hesvh.cn/Article/details/gyadbrydc.sHtML

[Q32] 分组拼接字符串
来源：http://m.share.fehbvm.com/Article/details/gnfubilbm.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://3g.zdbjq.cn/Article/details/giviurnjq.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://mobile.zdbjq.cn/Article/details/gqkdfvhja.sHtML

[Q33] 多列分组
来源：http://www.share.zdbjq.cn/Article/details/gvfypeipv.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://baike.fehbvm.com/Article/details/grwbjsfdp.sHtML

[Q34] 每组取第一条
来源：http://3g.fehbvm.com/Article/details/gzvouskzu.sHtML

SELECT * FROM (
来源：http://read.share.fehbvm.com/Article/details/gsuwldhiu.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://wap.fehbvm.com/Article/details/gcxjlidnv.sHtML

) t WHERE rn = 1;
来源：http://m.share.zdbjq.cn/Article/details/gcqfgvzcn.sHtML

[Q35] 内连接
来源：http://baike.hesvh.cn/Article/details/gxauvvcir.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://3g.fehbvm.com/Article/details/gkazdljri.sHtML

[Q36] 左连接
来源：http://www.blog.zdbjq.cn/Article/details/gphiljiwr.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://read.share.fehbvm.com/Article/details/gkhbmmbab.sHtML

[Q37] 右连接
来源：http://wap.fehbvm.com/Article/details/gaxjvaykz.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://wap.zdbjq.cn/Article/details/gkqduidod.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.m.share.fehbvm.com/Article/details/gfkpuukoi.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://baike.zdbjq.cn/Article/details/gzjmsriro.sHtML

[Q39] 自连接（查上下级）
来源：http://blog.zdbjq.cn/Article/details/gbuwdwbtp.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://baike.fehbvm.com/Article/details/glwlgbgdy.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.share.fehbvm.com/Article/details/gdrehorye.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://baike.zdbjq.cn/Article/details/gjccfwlti.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://read.share.hesvh.cn/Article/details/gyehmceyy.sHtML

[Q41] 多表连接
来源：http://www.m.share.hesvh.cn/Article/details/gtdzshytp.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://3g.hesvh.cn/Article/details/gxrrdkgvz.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.m.share.fehbvm.com/Article/details/gjazrglui.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://mobile.fehbvm.com/Article/details/gpsfbdard.sHtML

[Q42] 连接条件附加过滤
来源：http://www.blog.hesvh.cn/Article/details/gknkrswmf.sHtML

SELECT u.name, o.amount FROM users u
来源：http://wap.fehbvm.com/Article/details/gwbfcjdsa.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://blog.hesvh.cn/Article/details/gvkzbqphx.sHtML

[Q43] 标量子查询
来源：http://read.share.hesvh.cn/Article/details/goricrarj.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://baike.zdbjq.cn/Article/details/gmmeuqzuk.sHtML

[Q44] IN 子查询
来源：http://www.m.share.hesvh.cn/Article/details/gymuqnydd.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://m.share.zdbjq.cn/Article/details/gvsioqykl.sHtML

[Q45] EXISTS 判断存在
来源：http://m.share.zdbjq.cn/Article/details/gwgbqgfda.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.fehbvm.com/Article/details/gstiziafz.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://3g.zdbjq.cn/Article/details/gieeldham.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.hesvh.cn/Article/details/gnhbklmej.sHtML

[Q47] 与平均值比较
来源：http://m.share.hesvh.cn/Article/details/gzlzrdmzw.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://read.share.fehbvm.com/Article/details/gnsvlnoco.sHtML

[Q48] CTE 公用表表达式
来源：http://blog.hesvh.cn/Article/details/gonumdrni.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://3g.fehbvm.com/Article/details/gegicqjjo.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://wap.zdbjq.cn/Article/details/gklurnbks.sHtML

[Q49] 更新单行
来源：http://m.share.fehbvm.com/Article/details/gtzzxoffw.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://mobile.hesvh.cn/Article/details/gjpzehrmx.sHtML

[Q50] 批量更新
来源：http://www.m.share.fehbvm.com/Article/details/gbbefuhhr.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.blog.zdbjq.cn/Article/details/ggtjtcyfd.sHtML

[Q51] 用子查询更新
来源：http://www.m.share.hesvh.cn/Article/details/gwudjlpid.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://wap.hesvh.cn/Article/details/gjffdstfj.sHtML

[Q52] 删除指定行
来源：http://baike.zdbjq.cn/Article/details/ghcgyyihm.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.m.share.hesvh.cn/Article/details/ghvflqchi.sHtML

[Q53] 按条件删除
来源：http://www.m.share.zdbjq.cn/Article/details/gdikvrdrp.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://read.share.zdbjq.cn/Article/details/gydlqmkec.sHtML

[Q54] 清空表
来源：http://mobile.zdbjq.cn/Article/details/gkooahkuk.sHtML

TRUNCATE TABLE logs;
来源：http://blog.zdbjq.cn/Article/details/guevoenfp.sHtML

[Q55] 排名（并列占位）
来源：http://www.share.zdbjq.cn/Article/details/gcxesrsla.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.m.share.hesvh.cn/Article/details/gjomogdpb.sHtML

[Q56] 密集排名（并列不占位）
来源：http://blog.zdbjq.cn/Article/details/gzjnhpxxp.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.blog.fehbvm.com/Article/details/gdeueqpvh.sHtML

[Q57] 行号
来源：http://m.share.hesvh.cn/Article/details/gpktsdppo.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://3g.hesvh.cn/Article/details/gxcizihiw.sHtML

[Q58] 累计求和
来源：http://www.blog.fehbvm.com/Article/details/gpopjztxv.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://3g.fehbvm.com/Article/details/gehxhcunf.sHtML

[Q59] 分组内累计
来源：http://blog.fehbvm.com/Article/details/gzpdueong.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://3g.hesvh.cn/Article/details/gndwkruln.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.share.zdbjq.cn/Article/details/gfkkvpchb.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://3g.zdbjq.cn/Article/details/gopdhxjhg.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://mobile.hesvh.cn/Article/details/gvvbrfkoe.sHtML

[Q61] 移动平均
来源：http://www.blog.hesvh.cn/Article/details/grijejwwp.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.share.fehbvm.com/Article/details/gpzlyuxye.sHtML

[Q62] 分组占比
来源：http://3g.zdbjq.cn/Article/details/ghipceptw.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.share.hesvh.cn/Article/details/gtwabkzyb.sHtML

[Q63] 开启事务
来源：http://mobile.hesvh.cn/Article/details/gtauunlum.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://blog.zdbjq.cn/Article/details/grcymjqpy.sHtML

[Q64] 提交事务
来源：http://blog.fehbvm.com/Article/details/ggtbcaznn.sHtML

COMMIT;
来源：http://3g.hesvh.cn/Article/details/gaeqehouj.sHtML

[Q65] 回滚事务
来源：http://3g.fehbvm.com/Article/details/gdfuktpxf.sHtML

ROLLBACK;
来源：http://www.blog.fehbvm.com/Article/details/guypnkiwy.sHtML

[Q66] 行锁查询
来源：http://blog.hesvh.cn/Article/details/gnmbqiitv.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.blog.fehbvm.com/Article/details/gvlrijywc.sHtML

[Q67] 设置隔离级别
来源：http://www.m.share.fehbvm.com/Article/details/gawvwqykt.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.share.hesvh.cn/Article/details/gksekiuap.sHtML

[Q68] 保存点
来源：http://wap.fehbvm.com/Article/details/gogmtlvph.sHtML

SAVEPOINT sp1;
来源：http://m.share.zdbjq.cn/Article/details/gxvmezvlm.sHtML

ROLLBACK TO sp1;
来源：http://www.share.zdbjq.cn/Article/details/gojraqzah.sHtML

[Q69] 查看执行计划
来源：http://read.share.hesvh.cn/Article/details/gazdyvocw.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.blog.hesvh.cn/Article/details/gcaonqimd.sHtML

[Q70] 更新统计信息
来源：http://mobile.zdbjq.cn/Article/details/gicruvqht.sHtML

ANALYZE TABLE users;
来源：http://3g.fehbvm.com/Article/details/gkwsfgdzi.sHtML

[Q71] 查看建表语句
来源：http://baike.fehbvm.com/Article/details/gyjszfnzt.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://baike.hesvh.cn/Article/details/gugpquqti.sHtML

[Q72] 查看索引
来源：http://www.share.hesvh.cn/Article/details/gzbqqphzg.sHtML

SHOW INDEX FROM users;
来源：http://wap.zdbjq.cn/Article/details/grvcxtrrd.sHtML

[Q73] 查看表状态
来源：http://www.blog.hesvh.cn/Article/details/gjnvltwrp.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.share.hesvh.cn/Article/details/gliijccsc.sHtML

[Q74] 强制使用索引
来源：http://www.blog.hesvh.cn/Article/details/gpuambcfn.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://mobile.zdbjq.cn/Article/details/gitoyheon.sHtML

[Q75] 日期格式化
来源：http://www.blog.fehbvm.com/Article/details/gfoirexxg.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://read.share.zdbjq.cn/Article/details/gkfwxfviu.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://read.share.hesvh.cn/Article/details/girjpclcu.sHtML

[Q76] 按天统计
来源：http://m.share.zdbjq.cn/Article/details/grtdfwrsa.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://read.share.fehbvm.com/Article/details/gzzmvrhrx.sHtML

[Q77] 时间加减
来源：http://blog.zdbjq.cn/Article/details/gxyaslbha.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.m.share.zdbjq.cn/Article/details/gteseoqgv.sHtML

[Q78] 当前时间
来源：http://baike.zdbjq.cn/Article/details/gkpuiqsgd.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://baike.zdbjq.cn/Article/details/gxsrrtbuf.sHtML

[Q79] 字符串拼接
来源：http://m.share.fehbvm.com/Article/details/gfrctycnj.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://read.share.hesvh.cn/Article/details/gfvjgetbq.sHtML

[Q80] 字符串截取
来源：http://wap.hesvh.cn/Article/details/gpajvdfqd.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://3g.zdbjq.cn/Article/details/ghlgrrukm.sHtML

[Q81] 字符串替换
来源：http://3g.hesvh.cn/Article/details/gvcqowqlt.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://baike.hesvh.cn/Article/details/gfnjmxbai.sHtML

[Q82] 字符长度与字节长度
来源：http://m.share.fehbvm.com/Article/details/gkbgmacum.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://wap.zdbjq.cn/Article/details/gmnqznyey.sHtML

[Q83] 大小写转换
来源：http://mobile.hesvh.cn/Article/details/gqxcwxowk.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://mobile.fehbvm.com/Article/details/gkwltwqgf.sHtML

[Q84] 去除首尾空格
来源：http://www.m.share.zdbjq.cn/Article/details/gceermviq.sHtML

SELECT TRIM(name) FROM users;
来源：http://blog.zdbjq.cn/Article/details/gxqxuwlaf.sHtML

[Q85] 数值取整
来源：http://baike.fehbvm.com/Article/details/giyoydwkl.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.m.share.zdbjq.cn/Article/details/glkrylkzk.sHtML

[Q86] 读取 JSON 字段
来源：http://mobile.fehbvm.com/Article/details/gfylytxax.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://baike.hesvh.cn/Article/details/gosmbcwck.sHtML

[Q87] JSON 字段做条件
来源：http://m.share.fehbvm.com/Article/details/gctrxbpfc.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://m.share.zdbjq.cn/Article/details/ggzvpwnqs.sHtML

[Q88] 行转列（条件聚合）
来源：http://wap.zdbjq.cn/Article/details/guvuvyose.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://mobile.hesvh.cn/Article/details/ggbetfduq.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://wap.fehbvm.com/Article/details/ghiubsnje.sHtML

[Q89] 判断表是否存在
来源：http://www.m.share.hesvh.cn/Article/details/gkujoboja.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.share.fehbvm.com/Article/details/gpxiinpzq.sHtML

[Q90] 生成序号列
来源：http://www.m.share.fehbvm.com/Article/details/gmuifcsbo.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://mobile.fehbvm.com/Article/details/gapdmqpix.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gzvszotbk.sHtML

R. Bash 专题
来源：http://www.blog.fehbvm.com/Article/details/gfzwgguto.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gykodfbxf.sHtML

[R01] shebang 与严格模式
来源：http://www.m.share.zdbjq.cn/Article/details/gvouidige.sHtML

#!/usr/bin/env bash
来源：http://baike.hesvh.cn/Article/details/gomnoaviw.sHtML

set -euo pipefail
来源：http://baike.fehbvm.com/Article/details/glgcnrqze.sHtML

[R02] 变量赋值与使用
来源：http://www.m.share.zdbjq.cn/Article/details/gcivafuvf.sHtML

name="Tom"; echo "$name"
来源：http://3g.hesvh.cn/Article/details/gfoavmgtk.sHtML

[R03] 只读变量
来源：http://baike.fehbvm.com/Article/details/gtqaoolsk.sHtML

readonly PI=3.14
来源：http://read.share.hesvh.cn/Article/details/ggfolklll.sHtML

[R04] 位置参数
来源：http://www.blog.fehbvm.com/Article/details/gclrtyqfi.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.m.share.fehbvm.com/Article/details/goxegwlqa.sHtML

[R05] 参数默认值
来源：http://mobile.fehbvm.com/Article/details/ginvbzmkm.sHtML

name="${1:-default}"
来源：http://blog.zdbjq.cn/Article/details/gjrqensrn.sHtML

[R06] 判断命令是否存在
来源：http://blog.zdbjq.cn/Article/details/gkxyurwnx.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.share.zdbjq.cn/Article/details/gryuhqrmb.sHtML

[R07] if 判断文件
来源：http://baike.fehbvm.com/Article/details/gomohvffu.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://blog.zdbjq.cn/Article/details/gzdzshpdz.sHtML

[R08] 数值比较
来源：http://www.m.share.hesvh.cn/Article/details/gsatklumi.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.blog.fehbvm.com/Article/details/gvvyhbbzo.sHtML

[R09] 字符串比较
来源：http://www.share.fehbvm.com/Article/details/gdrnlfyhd.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://blog.hesvh.cn/Article/details/gozobilje.sHtML

[R10] 正则匹配
来源：http://www.share.hesvh.cn/Article/details/grebzaywl.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://read.share.zdbjq.cn/Article/details/glvsrhyok.sHtML

[R11] case 多分支
来源：http://baike.hesvh.cn/Article/details/gitouxbyz.sHtML

case "$1" in
来源：http://www.m.share.zdbjq.cn/Article/details/gtauelyid.sHtML

start) echo "启动" ;;
来源：http://baike.zdbjq.cn/Article/details/gipdpyjni.sHtML

stop)  echo "停止" ;;
来源：http://wap.fehbvm.com/Article/details/grxswjuah.sHtML

*)     echo "未知命令" ;;
来源：http://baike.zdbjq.cn/Article/details/gtjmhiioi.sHtML

esac
来源：http://mobile.zdbjq.cn/Article/details/gwqomlawf.sHtML

[R12] for 遍历文件
来源：http://www.blog.hesvh.cn/Article/details/gjnyoejjz.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.m.share.hesvh.cn/Article/details/gkrihijze.sHtML

[R13] for 计数循环
来源：http://wap.zdbjq.cn/Article/details/gibeorpnx.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://read.share.zdbjq.cn/Article/details/gwfmjlnhi.sHtML

[R14] C 风格 for
来源：http://blog.zdbjq.cn/Article/details/gbjdfcvyq.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://m.share.fehbvm.com/Article/details/gdgclwiba.sHtML

[R15] while 逐行读文件
来源：http://m.share.fehbvm.com/Article/details/ghtfdyspt.sHtML


<!-- 参考信息 -->