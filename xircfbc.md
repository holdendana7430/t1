代发 wailian999

Ruby: Digest::SHA256.hexdigest(s)
来源：http://blog.fehbvm.com/Article/details/gxhpcmcza.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.blog.hesvh.cn/Article/details/gkyaagssb.sHtML

[P03] 生成短随机字符串
来源：http://baike.zdbjq.cn/Article/details/gczgfuclj.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://read.share.zdbjq.cn/Article/details/gqegeptvh.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.m.share.zdbjq.cn/Article/details/gwhjjfajd.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.zdbjq.cn/Article/details/gllbzfswm.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.fehbvm.com/Article/details/gobmotpgy.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.blog.hesvh.cn/Article/details/gexrgwaav.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.share.hesvh.cn/Article/details/guzqrpwjc.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.blog.hesvh.cn/Article/details/gagsopuda.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://blog.zdbjq.cn/Article/details/ggxtmrcvh.sHtML

[P04] 求长度
来源：http://www.share.fehbvm.com/Article/details/ganxoyyru.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://read.share.fehbvm.com/Article/details/gluedrzvd.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.zdbjq.cn/Article/details/gstsoyzlr.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.hesvh.cn/Article/details/gjpwvqwqs.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.zdbjq.cn/Article/details/gcmlqjgka.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.m.share.zdbjq.cn/Article/details/gwiqxqrmx.sHtML

Go:   len(arr);  len(m)
来源：http://baike.fehbvm.com/Article/details/gajyrbini.sHtML

Ruby: x.length;  x.size
来源：http://mobile.zdbjq.cn/Article/details/gohtbvrlb.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://3g.hesvh.cn/Article/details/ghecnoomc.sHtML

[P05] 判断两个对象内容是否相等
来源：http://baike.zdbjq.cn/Article/details/gzvirjvfo.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://blog.fehbvm.com/Article/details/gnhrqbrfg.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://m.share.zdbjq.cn/Article/details/glzkdcflp.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://mobile.fehbvm.com/Article/details/gfdaerbdr.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://wap.fehbvm.com/Article/details/giqjckico.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://3g.zdbjq.cn/Article/details/gzrjnqjoi.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://wap.fehbvm.com/Article/details/gtxveowtj.sHtML

Ruby: a == b
来源：http://mobile.hesvh.cn/Article/details/ghqxvocos.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://wap.zdbjq.cn/Article/details/grnoakogv.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://wap.zdbjq.cn/Article/details/gwrpjdmrk.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://mobile.zdbjq.cn/Article/details/gyswlgxjg.sHtML

PHP:  if (empty($x)) {}
来源：http://blog.zdbjq.cn/Article/details/gymkvjsgt.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://3g.zdbjq.cn/Article/details/gybrdctpq.sHtML

TS:   if (x == null) {}
来源：http://www.share.fehbvm.com/Article/details/ghnudexmd.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://m.share.hesvh.cn/Article/details/gpokivyky.sHtML

Go:   if x == nil {}
来源：http://m.share.zdbjq.cn/Article/details/gulkkienv.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://mobile.fehbvm.com/Article/details/gjkchahhk.sHtML

C#:   if (x is null) {}
来源：http://wap.fehbvm.com/Article/details/gfuqzijtp.sHtML

[P07] 防抖与节流
来源：http://m.share.zdbjq.cn/Article/details/gryxbtezg.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://baike.zdbjq.cn/Article/details/gadvrhxgw.sHtML

PHP:  // 手写时间戳比较
来源：http://read.share.hesvh.cn/Article/details/gooqntulv.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.fehbvm.com/Article/details/gpsqqktnj.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.zdbjq.cn/Article/details/glaafcawe.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://blog.fehbvm.com/Article/details/gelgaqjjy.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://wap.zdbjq.cn/Article/details/gracdmvrj.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://mobile.zdbjq.cn/Article/details/gmngouowd.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://3g.fehbvm.com/Article/details/gplydwcyw.sHtML

[P08] 处理浮点精度问题
来源：http://mobile.zdbjq.cn/Article/details/gmfqtudsa.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.m.share.fehbvm.com/Article/details/gtelybpcl.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://3g.zdbjq.cn/Article/details/gpptbbgfe.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://wap.hesvh.cn/Article/details/gyfsmqcan.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://m.share.hesvh.cn/Article/details/ggpffxadz.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://mobile.zdbjq.cn/Article/details/glgeweitm.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://m.share.zdbjq.cn/Article/details/gxgezstgt.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://m.share.hesvh.cn/Article/details/glwmrefbv.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://mobile.fehbvm.com/Article/details/guelcxbev.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gevvsszvj.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://read.share.hesvh.cn/Article/details/gxgmeaezd.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gukwzbnue.sHtML

[Q01] 创建表
来源：http://www.share.hesvh.cn/Article/details/gnrdixgfs.sHtML

CREATE TABLE users (
来源：http://m.share.zdbjq.cn/Article/details/gcntnkkbu.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://mobile.zdbjq.cn/Article/details/gqnsqbqvx.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.m.share.hesvh.cn/Article/details/gkprxxtwr.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.m.share.hesvh.cn/Article/details/gdlwdsjvm.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://read.share.fehbvm.com/Article/details/ghbzcjsgw.sHtML

);
来源：http://blog.zdbjq.cn/Article/details/gidbvtkdc.sHtML

[Q02] 创建带外键的表
来源：http://m.share.hesvh.cn/Article/details/gojxvbfkc.sHtML

CREATE TABLE orders (
来源：http://read.share.zdbjq.cn/Article/details/gumdkklcy.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.hesvh.cn/Article/details/gkselwjdh.sHtML

user_id INT NOT NULL,
来源：http://3g.fehbvm.com/Article/details/gaxvzqzwv.sHtML

amount DECIMAL(10, 2),
来源：http://wap.fehbvm.com/Article/details/ghpvepisp.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://mobile.hesvh.cn/Article/details/gkshqirru.sHtML

);
来源：http://baike.hesvh.cn/Article/details/gwmqybjyv.sHtML

[Q03] 增加列
来源：http://www.blog.zdbjq.cn/Article/details/ghpacoexi.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.blog.hesvh.cn/Article/details/ggzdjvsbs.sHtML

[Q04] 修改列类型
来源：http://blog.fehbvm.com/Article/details/gvyeeseta.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.m.share.fehbvm.com/Article/details/gpxsoadoz.sHtML

[Q05] 重命名列
来源：http://baike.zdbjq.cn/Article/details/gcgeiiozl.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://mobile.fehbvm.com/Article/details/gplydyydv.sHtML

[Q06] 删除列
来源：http://3g.fehbvm.com/Article/details/ghdjcfghp.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://baike.zdbjq.cn/Article/details/gjwojivon.sHtML

[Q07] 删除表
来源：http://baike.zdbjq.cn/Article/details/gkhvpfdeq.sHtML

DROP TABLE IF EXISTS orders;
来源：http://blog.zdbjq.cn/Article/details/gmnybyluw.sHtML

[Q08] 创建普通索引
来源：http://wap.hesvh.cn/Article/details/glducwazn.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.share.zdbjq.cn/Article/details/gygfaltkz.sHtML

[Q09] 创建唯一索引
来源：http://m.share.zdbjq.cn/Article/details/gcaiyhpfh.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://blog.hesvh.cn/Article/details/gqeormpos.sHtML

[Q10] 插入单行
来源：http://www.m.share.fehbvm.com/Article/details/gkpjqqzmo.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://mobile.fehbvm.com/Article/details/gjgzcdwhm.sHtML

[Q11] 一次插入多行
来源：http://m.share.zdbjq.cn/Article/details/gksgfrjry.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://blog.hesvh.cn/Article/details/ghdizknnk.sHtML

[Q12] 插入后取自增 ID
来源：http://www.blog.zdbjq.cn/Article/details/goovymlow.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://baike.fehbvm.com/Article/details/gnhaaovtx.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://wap.hesvh.cn/Article/details/gkknnqgcm.sHtML

[Q13] 忽略重复插入
来源：http://blog.zdbjq.cn/Article/details/gcowtvjlw.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.share.fehbvm.com/Article/details/gfvjfzckh.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.blog.hesvh.cn/Article/details/ghdgquoli.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.share.zdbjq.cn/Article/details/gtfzhysba.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://baike.zdbjq.cn/Article/details/gdaggqbek.sHtML

[Q15] 查询全部
来源：http://www.blog.zdbjq.cn/Article/details/gecsdscam.sHtML

SELECT * FROM users;
来源：http://www.share.hesvh.cn/Article/details/gceujjygg.sHtML

[Q16] 查询指定列
来源：http://read.share.zdbjq.cn/Article/details/gsaixpezj.sHtML

SELECT id, name FROM users;
来源：http://wap.hesvh.cn/Article/details/gcusassrw.sHtML

[Q17] 条件查询
来源：http://mobile.hesvh.cn/Article/details/gaanaezsz.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.m.share.fehbvm.com/Article/details/gxmvikxei.sHtML

[Q18] 模糊匹配
来源：http://www.share.fehbvm.com/Article/details/gvbarexcm.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://m.share.zdbjq.cn/Article/details/gpxwfunjf.sHtML

[Q19] 范围查询
来源：http://read.share.hesvh.cn/Article/details/gpdrripgo.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.share.fehbvm.com/Article/details/gnpjvxztz.sHtML

[Q20] IN 列表
来源：http://m.share.zdbjq.cn/Article/details/gcrcebtkh.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://baike.fehbvm.com/Article/details/gzlkfybze.sHtML

[Q21] 空值判断
来源：http://mobile.fehbvm.com/Article/details/ghdtgrdww.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://read.share.zdbjq.cn/Article/details/gzkhjfozl.sHtML

[Q22] 排序
来源：http://blog.hesvh.cn/Article/details/gkjbhlhuo.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://blog.zdbjq.cn/Article/details/gniaxfgen.sHtML

[Q23] 分页
来源：http://3g.hesvh.cn/Article/details/gsqkmyybw.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://wap.fehbvm.com/Article/details/gxibttppj.sHtML

[Q24] 去重
来源：http://www.share.zdbjq.cn/Article/details/gscfbixsp.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gfblvsnde.sHtML

[Q25] 只取前 N 条
来源：http://wap.hesvh.cn/Article/details/gwoxuwjoy.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://wap.zdbjq.cn/Article/details/gdvkppkwx.sHtML

[Q26] 计数
来源：http://www.blog.zdbjq.cn/Article/details/gxdrzdydl.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/glyuffibd.sHtML

[Q27] 条件计数
来源：http://blog.hesvh.cn/Article/details/gzqygkpwu.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gszywhvmz.sHtML

[Q28] 求和与平均
来源：http://www.blog.zdbjq.cn/Article/details/ghsubjjse.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://blog.hesvh.cn/Article/details/gkihktshy.sHtML

[Q29] 最大最小值
来源：http://mobile.hesvh.cn/Article/details/gdvzcvfdf.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://m.share.hesvh.cn/Article/details/gkminylwj.sHtML

[Q30] 分组统计
来源：http://wap.zdbjq.cn/Article/details/grsbprstp.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://m.share.zdbjq.cn/Article/details/geprlcvfx.sHtML

[Q31] 分组后过滤
来源：http://wap.zdbjq.cn/Article/details/gcmppsflf.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://wap.fehbvm.com/Article/details/gzqsstdgw.sHtML

[Q32] 分组拼接字符串
来源：http://mobile.fehbvm.com/Article/details/grtxtfegd.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://wap.hesvh.cn/Article/details/gnrrdjyem.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://blog.zdbjq.cn/Article/details/gfutgfxnt.sHtML

[Q33] 多列分组
来源：http://www.blog.hesvh.cn/Article/details/gimgdplyz.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.blog.fehbvm.com/Article/details/gjzyfxolq.sHtML

[Q34] 每组取第一条
来源：http://wap.fehbvm.com/Article/details/gxpqmxlmv.sHtML

SELECT * FROM (
来源：http://www.m.share.fehbvm.com/Article/details/gktyugszq.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://mobile.hesvh.cn/Article/details/grbmrcqrs.sHtML

) t WHERE rn = 1;
来源：http://m.share.zdbjq.cn/Article/details/glyijuzaa.sHtML

[Q35] 内连接
来源：http://www.blog.fehbvm.com/Article/details/gipcsbxyf.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.fehbvm.com/Article/details/gtnkrpcpe.sHtML

[Q36] 左连接
来源：http://read.share.zdbjq.cn/Article/details/gdbwewuen.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://3g.zdbjq.cn/Article/details/gaatpwuxh.sHtML

[Q37] 右连接
来源：http://www.m.share.hesvh.cn/Article/details/glgteakcp.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://3g.zdbjq.cn/Article/details/gxmuwcznr.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://blog.fehbvm.com/Article/details/gaqxkatbf.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://mobile.zdbjq.cn/Article/details/ghoxxuhiu.sHtML

[Q39] 自连接（查上下级）
来源：http://www.share.hesvh.cn/Article/details/gqyvbqbvq.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://m.share.zdbjq.cn/Article/details/gbsrcgoja.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://baike.zdbjq.cn/Article/details/giosuntqz.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://m.share.hesvh.cn/Article/details/gqyyhlkeq.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://m.share.hesvh.cn/Article/details/gtbilujhg.sHtML

[Q41] 多表连接
来源：http://blog.hesvh.cn/Article/details/ggmqdkrrh.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://read.share.fehbvm.com/Article/details/glnxzsdgr.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.blog.zdbjq.cn/Article/details/gzkfypsib.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://m.share.zdbjq.cn/Article/details/gkfntcawt.sHtML

[Q42] 连接条件附加过滤
来源：http://wap.fehbvm.com/Article/details/gcmmmefbf.sHtML

SELECT u.name, o.amount FROM users u
来源：http://baike.fehbvm.com/Article/details/ghzkmvfnl.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://read.share.zdbjq.cn/Article/details/gtdebshex.sHtML

[Q43] 标量子查询
来源：http://read.share.zdbjq.cn/Article/details/goxpbyrzd.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://baike.fehbvm.com/Article/details/gzglmkqme.sHtML

[Q44] IN 子查询
来源：http://read.share.hesvh.cn/Article/details/gmakkyllw.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://mobile.fehbvm.com/Article/details/gisvqfliq.sHtML

[Q45] EXISTS 判断存在
来源：http://blog.hesvh.cn/Article/details/gisnaonjh.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.zdbjq.cn/Article/details/gbqsahila.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://read.share.zdbjq.cn/Article/details/gokgqqgno.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.fehbvm.com/Article/details/ggxbdeesh.sHtML

[Q47] 与平均值比较
来源：http://3g.hesvh.cn/Article/details/genvdzsaj.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.blog.hesvh.cn/Article/details/ggbwqxnln.sHtML

[Q48] CTE 公用表表达式
来源：http://mobile.hesvh.cn/Article/details/goqnqtwga.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.blog.fehbvm.com/Article/details/guvcshktz.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.blog.fehbvm.com/Article/details/ggdxctivc.sHtML

[Q49] 更新单行
来源：http://blog.hesvh.cn/Article/details/gxoupjaco.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://wap.zdbjq.cn/Article/details/gsrzttwnt.sHtML

[Q50] 批量更新
来源：http://3g.hesvh.cn/Article/details/gfxvjurxk.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://baike.zdbjq.cn/Article/details/gueaftupp.sHtML

[Q51] 用子查询更新
来源：http://www.blog.hesvh.cn/Article/details/gfbftlttx.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://baike.zdbjq.cn/Article/details/guigctgtp.sHtML

[Q52] 删除指定行
来源：http://m.share.fehbvm.com/Article/details/gzgnibtxh.sHtML

DELETE FROM users WHERE id = 10;
来源：http://read.share.fehbvm.com/Article/details/gdxqdscjr.sHtML

[Q53] 按条件删除
来源：http://wap.hesvh.cn/Article/details/gjstxnhvc.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://blog.hesvh.cn/Article/details/gersicexp.sHtML

[Q54] 清空表
来源：http://baike.hesvh.cn/Article/details/gbibiizpj.sHtML

TRUNCATE TABLE logs;
来源：http://read.share.fehbvm.com/Article/details/ggcpfiajr.sHtML

[Q55] 排名（并列占位）
来源：http://read.share.hesvh.cn/Article/details/gbfhzpqub.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://m.share.hesvh.cn/Article/details/gxgczzgbu.sHtML

[Q56] 密集排名（并列不占位）
来源：http://read.share.fehbvm.com/Article/details/gilsnjpja.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://baike.fehbvm.com/Article/details/gkbrgbmqk.sHtML

[Q57] 行号
来源：http://mobile.fehbvm.com/Article/details/gxlaxieip.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://m.share.hesvh.cn/Article/details/gfamqjqaj.sHtML

[Q58] 累计求和
来源：http://3g.fehbvm.com/Article/details/gwpbmtqyd.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://blog.hesvh.cn/Article/details/gaptucfgj.sHtML

[Q59] 分组内累计
来源：http://baike.fehbvm.com/Article/details/ghvuoslzu.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.m.share.zdbjq.cn/Article/details/gnhnutart.sHtML

[Q60] 取上一行 / 下一行
来源：http://mobile.hesvh.cn/Article/details/gwuwkkglt.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://mobile.fehbvm.com/Article/details/gptvwngjj.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://mobile.zdbjq.cn/Article/details/gyplraawb.sHtML

[Q61] 移动平均
来源：http://www.blog.zdbjq.cn/Article/details/gmqwdlmly.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.share.fehbvm.com/Article/details/gucxfjhwe.sHtML

[Q62] 分组占比
来源：http://3g.fehbvm.com/Article/details/gvwsuqupa.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.share.zdbjq.cn/Article/details/gucfzawvl.sHtML

[Q63] 开启事务
来源：http://wap.zdbjq.cn/Article/details/grkwzxccg.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://read.share.hesvh.cn/Article/details/gqqtragxm.sHtML

[Q64] 提交事务
来源：http://wap.hesvh.cn/Article/details/glmnlrvuw.sHtML

COMMIT;
来源：http://www.blog.hesvh.cn/Article/details/gjjawyeve.sHtML

[Q65] 回滚事务
来源：http://www.m.share.zdbjq.cn/Article/details/gxdifhvws.sHtML

ROLLBACK;
来源：http://www.m.share.hesvh.cn/Article/details/gjkgrcbbt.sHtML

[Q66] 行锁查询
来源：http://wap.fehbvm.com/Article/details/ggveqmnym.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://blog.fehbvm.com/Article/details/gqvjuijzn.sHtML

[Q67] 设置隔离级别
来源：http://read.share.hesvh.cn/Article/details/gcevzewlk.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://mobile.fehbvm.com/Article/details/gaajmmwht.sHtML

[Q68] 保存点
来源：http://blog.fehbvm.com/Article/details/gykbvfmqi.sHtML

SAVEPOINT sp1;
来源：http://blog.zdbjq.cn/Article/details/gddagjktl.sHtML

ROLLBACK TO sp1;
来源：http://wap.hesvh.cn/Article/details/gbmqxibrl.sHtML

[Q69] 查看执行计划
来源：http://3g.fehbvm.com/Article/details/grchbwtup.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.m.share.hesvh.cn/Article/details/grxyfupjt.sHtML

[Q70] 更新统计信息
来源：http://m.share.hesvh.cn/Article/details/gorajaqrb.sHtML

ANALYZE TABLE users;
来源：http://baike.fehbvm.com/Article/details/gxbtjgqkk.sHtML

[Q71] 查看建表语句
来源：http://www.blog.fehbvm.com/Article/details/ghmqpcuub.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://blog.hesvh.cn/Article/details/guiwlvroy.sHtML

[Q72] 查看索引
来源：http://read.share.zdbjq.cn/Article/details/gywipyivz.sHtML

SHOW INDEX FROM users;
来源：http://3g.fehbvm.com/Article/details/gzvwhrbok.sHtML

[Q73] 查看表状态
来源：http://wap.fehbvm.com/Article/details/gjyjkaovb.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://baike.zdbjq.cn/Article/details/gwwmrulht.sHtML

[Q74] 强制使用索引
来源：http://wap.hesvh.cn/Article/details/gkylcdthe.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://mobile.fehbvm.com/Article/details/gxjtjykfg.sHtML

[Q75] 日期格式化
来源：http://mobile.fehbvm.com/Article/details/gblzfifxf.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.m.share.fehbvm.com/Article/details/gzwzbmipm.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.m.share.fehbvm.com/Article/details/gqdksglsh.sHtML

[Q76] 按天统计
来源：http://mobile.fehbvm.com/Article/details/gnzecmfyj.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://baike.zdbjq.cn/Article/details/gjqxiacea.sHtML

[Q77] 时间加减
来源：http://www.blog.fehbvm.com/Article/details/gyljrzpxg.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.blog.hesvh.cn/Article/details/gdqgxvpqb.sHtML

[Q78] 当前时间
来源：http://3g.zdbjq.cn/Article/details/gkjpmkbzt.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://blog.hesvh.cn/Article/details/gyczsfuqt.sHtML

[Q79] 字符串拼接
来源：http://wap.fehbvm.com/Article/details/gppcuefxo.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://read.share.zdbjq.cn/Article/details/gbdfkaxws.sHtML

[Q80] 字符串截取
来源：http://wap.zdbjq.cn/Article/details/guuvdxgao.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.share.fehbvm.com/Article/details/grtbrnbmx.sHtML

[Q81] 字符串替换
来源：http://3g.hesvh.cn/Article/details/gjyhwkigz.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://mobile.hesvh.cn/Article/details/gdmxtmkwl.sHtML

[Q82] 字符长度与字节长度
来源：http://m.share.hesvh.cn/Article/details/gozyqzoee.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://read.share.hesvh.cn/Article/details/gsmcvcows.sHtML

[Q83] 大小写转换
来源：http://www.blog.zdbjq.cn/Article/details/gjwxxxsmm.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gvgrfvwge.sHtML

[Q84] 去除首尾空格
来源：http://read.share.fehbvm.com/Article/details/gnnmgykzr.sHtML

SELECT TRIM(name) FROM users;
来源：http://m.share.zdbjq.cn/Article/details/ggciecmom.sHtML

[Q85] 数值取整
来源：http://baike.zdbjq.cn/Article/details/gxmhlzswf.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://blog.fehbvm.com/Article/details/gngqvsyni.sHtML

[Q86] 读取 JSON 字段
来源：http://wap.hesvh.cn/Article/details/gpalwppyr.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.m.share.fehbvm.com/Article/details/gwmpuzbxs.sHtML

[Q87] JSON 字段做条件
来源：http://m.share.hesvh.cn/Article/details/gzixdidxd.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://3g.zdbjq.cn/Article/details/gopjnezmb.sHtML

[Q88] 行转列（条件聚合）
来源：http://m.share.fehbvm.com/Article/details/gsftfegep.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://m.share.zdbjq.cn/Article/details/gfuuyqdfn.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://read.share.hesvh.cn/Article/details/ghgbrozxx.sHtML

[Q89] 判断表是否存在
来源：http://mobile.hesvh.cn/Article/details/gkieyznsk.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.blog.fehbvm.com/Article/details/gafdgiyid.sHtML

[Q90] 生成序号列
来源：http://www.blog.fehbvm.com/Article/details/gdkbcltzi.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://wap.zdbjq.cn/Article/details/gqqrfutdi.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/ghhurfzxv.sHtML

R. Bash 专题
来源：http://read.share.fehbvm.com/Article/details/gwtempxve.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/glappyzth.sHtML

[R01] shebang 与严格模式
来源：http://baike.zdbjq.cn/Article/details/gpqthqxxd.sHtML

#!/usr/bin/env bash
来源：http://mobile.zdbjq.cn/Article/details/gtqkigihi.sHtML

set -euo pipefail
来源：http://www.m.share.hesvh.cn/Article/details/gywgabmqw.sHtML

[R02] 变量赋值与使用
来源：http://read.share.hesvh.cn/Article/details/ghkpsmnix.sHtML

name="Tom"; echo "$name"
来源：http://www.share.fehbvm.com/Article/details/gudegfiat.sHtML

[R03] 只读变量
来源：http://www.m.share.hesvh.cn/Article/details/gljesvmyz.sHtML

readonly PI=3.14
来源：http://blog.fehbvm.com/Article/details/gionfvzoh.sHtML

[R04] 位置参数
来源：http://www.blog.fehbvm.com/Article/details/gmqssuzdl.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://wap.zdbjq.cn/Article/details/gabrbsosm.sHtML

[R05] 参数默认值
来源：http://www.m.share.hesvh.cn/Article/details/gmvxbtflv.sHtML

name="${1:-default}"
来源：http://m.share.fehbvm.com/Article/details/graojscpy.sHtML

[R06] 判断命令是否存在
来源：http://baike.fehbvm.com/Article/details/gkiqfullf.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://3g.zdbjq.cn/Article/details/gwmhfovan.sHtML

[R07] if 判断文件
来源：http://mobile.hesvh.cn/Article/details/ggseqrfhq.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://mobile.hesvh.cn/Article/details/gysahecyb.sHtML

[R08] 数值比较
来源：http://blog.hesvh.cn/Article/details/gbemwsnol.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://read.share.zdbjq.cn/Article/details/goxvwoogn.sHtML

[R09] 字符串比较
来源：http://read.share.fehbvm.com/Article/details/gwkfvloni.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.share.zdbjq.cn/Article/details/gppdxswpe.sHtML

[R10] 正则匹配
来源：http://wap.zdbjq.cn/Article/details/gcbtypxsv.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.m.share.hesvh.cn/Article/details/gyrinepto.sHtML

[R11] case 多分支
来源：http://blog.fehbvm.com/Article/details/gamvpnogx.sHtML

case "$1" in
来源：http://baike.hesvh.cn/Article/details/gzdpqnxzt.sHtML

start) echo "启动" ;;
来源：http://www.share.fehbvm.com/Article/details/gjmupfvdg.sHtML

stop)  echo "停止" ;;
来源：http://3g.zdbjq.cn/Article/details/gpvwfemtv.sHtML

*)     echo "未知命令" ;;
来源：http://m.share.hesvh.cn/Article/details/glhiqfuxk.sHtML

esac
来源：http://m.share.fehbvm.com/Article/details/ggtkolafv.sHtML

[R12] for 遍历文件
来源：http://www.share.fehbvm.com/Article/details/gbidkohng.sHtML

for f in *.txt; do echo "$f"; done
来源：http://mobile.hesvh.cn/Article/details/gowdqawhr.sHtML

[R13] for 计数循环
来源：http://wap.fehbvm.com/Article/details/gpbheenen.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://read.share.fehbvm.com/Article/details/gfczuuopg.sHtML

[R14] C 风格 for
来源：http://blog.fehbvm.com/Article/details/gubuzzfvu.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://3g.zdbjq.cn/Article/details/glcrxvxhb.sHtML

[R15] while 逐行读文件
来源：http://www.blog.zdbjq.cn/Article/details/gfegcgkgd.sHtML


<!-- 参考信息 -->