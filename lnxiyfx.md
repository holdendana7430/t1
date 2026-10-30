代发 wailian999

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggpcpohen.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmhgpocov.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://m.share.fanxiaobao.xyz/Article/details/geezxfnno.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://wap.fanxiaobao.xyz/Article/details/gpekojpqw.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.share.fanxiaobao.xyz/Article/details/gwznwntbq.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://3g.fanxiaobao.xyz/Article/details/goilgojkj.sHtML

[P03] 生成短随机字符串
来源：http://baike.fanxiaobao.xyz/Article/details/gsajfnhrh.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://wap.fanxiaobao.xyz/Article/details/ghywtfdfl.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://m.share.fanxiaobao.xyz/Article/details/gysfomfaw.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gevwlvitv.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.fanxiaobao.xyz/Article/details/gbtlvtdlw.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://read.share.fanxiaobao.xyz/Article/details/guxrfgpdu.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://blog.fanxiaobao.xyz/Article/details/gzelmrter.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjiqvdguu.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://read.share.fanxiaobao.xyz/Article/details/gjhthtuqo.sHtML

[P04] 求长度
来源：http://read.share.fanxiaobao.xyz/Article/details/gjqybywzc.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://read.share.fanxiaobao.xyz/Article/details/golgcyshg.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxurpbhur.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.fanxiaobao.xyz/Article/details/golsazlfg.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.fanxiaobao.xyz/Article/details/getngkybs.sHtML

Java: list.size();  map.size();  s.length()
来源：http://mobile.fanxiaobao.xyz/Article/details/gorudxxsb.sHtML

Go:   len(arr);  len(m)
来源：http://blog.fanxiaobao.xyz/Article/details/gwacezlzm.sHtML

Ruby: x.length;  x.size
来源：http://blog.fanxiaobao.xyz/Article/details/gdjxwjyqm.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://baike.fanxiaobao.xyz/Article/details/gtuffshkx.sHtML

[P05] 判断两个对象内容是否相等
来源：http://m.share.fanxiaobao.xyz/Article/details/gybxhfhyx.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://read.share.fanxiaobao.xyz/Article/details/gghaiamjq.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gataqxiiw.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://mobile.fanxiaobao.xyz/Article/details/ghnvztjfa.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://m.share.fanxiaobao.xyz/Article/details/gpmmqqmqa.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.share.fanxiaobao.xyz/Article/details/gvclazacz.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyxqnarst.sHtML

Ruby: a == b
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfbjlxckh.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://3g.fanxiaobao.xyz/Article/details/gohxztlyh.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://read.share.fanxiaobao.xyz/Article/details/gngwffpus.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.blog.fanxiaobao.xyz/Article/details/gltllojcw.sHtML

PHP:  if (empty($x)) {}
来源：http://www.share.fanxiaobao.xyz/Article/details/ggcnigmoo.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.blog.fanxiaobao.xyz/Article/details/gricfrpqf.sHtML

TS:   if (x == null) {}
来源：http://www.share.fanxiaobao.xyz/Article/details/gylvbfegi.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.share.fanxiaobao.xyz/Article/details/gwdsdquvu.sHtML

Go:   if x == nil {}
来源：http://blog.fanxiaobao.xyz/Article/details/gdrhdnmxs.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://baike.fanxiaobao.xyz/Article/details/gsmqauqgf.sHtML

C#:   if (x is null) {}
来源：http://blog.fanxiaobao.xyz/Article/details/gztemgkzv.sHtML

[P07] 防抖与节流
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghlnfpwua.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.blog.fanxiaobao.xyz/Article/details/geqrpwkdn.sHtML

PHP:  // 手写时间戳比较
来源：http://blog.fanxiaobao.xyz/Article/details/guaqyqjkr.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.fanxiaobao.xyz/Article/details/gorzmegns.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.fanxiaobao.xyz/Article/details/gklugkeky.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://baike.fanxiaobao.xyz/Article/details/gahwazvat.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://mobile.fanxiaobao.xyz/Article/details/gnuiaypay.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://blog.fanxiaobao.xyz/Article/details/gtfxajyrv.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.blog.fanxiaobao.xyz/Article/details/gavkfjyph.sHtML

[P08] 处理浮点精度问题
来源：http://baike.fanxiaobao.xyz/Article/details/ggoyrdwyg.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://blog.fanxiaobao.xyz/Article/details/gwixuubzp.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://mobile.fanxiaobao.xyz/Article/details/gjgmdibao.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://wap.fanxiaobao.xyz/Article/details/gcwymztub.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://read.share.fanxiaobao.xyz/Article/details/gldyfaayf.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://read.share.fanxiaobao.xyz/Article/details/gdezctrfh.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://blog.fanxiaobao.xyz/Article/details/gqgnbpeob.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghblvsjus.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://baike.fanxiaobao.xyz/Article/details/grbbkoxyi.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gsasxdmhl.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://baike.fanxiaobao.xyz/Article/details/gahcaytls.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjnwfhben.sHtML

[Q01] 创建表
来源：http://www.share.fanxiaobao.xyz/Article/details/gopxziswa.sHtML

CREATE TABLE users (
来源：http://wap.fanxiaobao.xyz/Article/details/gkkbdbulg.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsdojvnyi.sHtML

name VARCHAR(50) NOT NULL,
来源：http://blog.fanxiaobao.xyz/Article/details/gnvsbiaul.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.share.fanxiaobao.xyz/Article/details/gradlwgyx.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://baike.fanxiaobao.xyz/Article/details/gooludino.sHtML

);
来源：http://mobile.fanxiaobao.xyz/Article/details/gfbvokopo.sHtML

[Q02] 创建带外键的表
来源：http://baike.fanxiaobao.xyz/Article/details/gojotjtte.sHtML

CREATE TABLE orders (
来源：http://www.blog.fanxiaobao.xyz/Article/details/gemkzrgih.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.fanxiaobao.xyz/Article/details/glixsjlsd.sHtML

user_id INT NOT NULL,
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwwoleelz.sHtML

amount DECIMAL(10, 2),
来源：http://wap.fanxiaobao.xyz/Article/details/gzfrqhsmr.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://baike.fanxiaobao.xyz/Article/details/gxavbztbg.sHtML

);
来源：http://wap.fanxiaobao.xyz/Article/details/goikyzwnp.sHtML

[Q03] 增加列
来源：http://www.blog.fanxiaobao.xyz/Article/details/gquhrsech.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gccoasaax.sHtML

[Q04] 修改列类型
来源：http://3g.fanxiaobao.xyz/Article/details/gdrmbfdkx.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.blog.fanxiaobao.xyz/Article/details/glscjpqhe.sHtML

[Q05] 重命名列
来源：http://m.share.fanxiaobao.xyz/Article/details/gsfwuvknq.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://m.share.fanxiaobao.xyz/Article/details/geongwrtx.sHtML

[Q06] 删除列
来源：http://blog.fanxiaobao.xyz/Article/details/guihosodw.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://wap.fanxiaobao.xyz/Article/details/gvexizuwe.sHtML

[Q07] 删除表
来源：http://m.share.fanxiaobao.xyz/Article/details/gevegzctp.sHtML

DROP TABLE IF EXISTS orders;
来源：http://read.share.fanxiaobao.xyz/Article/details/gsfubgjya.sHtML

[Q08] 创建普通索引
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gapuylupw.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://blog.fanxiaobao.xyz/Article/details/gdzyrhage.sHtML

[Q09] 创建唯一索引
来源：http://m.share.fanxiaobao.xyz/Article/details/gnxiljnre.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.share.fanxiaobao.xyz/Article/details/gqznwupws.sHtML

[Q10] 插入单行
来源：http://wap.fanxiaobao.xyz/Article/details/ggaeadfzd.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://3g.fanxiaobao.xyz/Article/details/getxfxbrj.sHtML

[Q11] 一次插入多行
来源：http://mobile.fanxiaobao.xyz/Article/details/gjbxuaaya.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.blog.fanxiaobao.xyz/Article/details/gontjillc.sHtML

[Q12] 插入后取自增 ID
来源：http://mobile.fanxiaobao.xyz/Article/details/ghobebzjd.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.blog.fanxiaobao.xyz/Article/details/grdewbgow.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://3g.fanxiaobao.xyz/Article/details/gnkntsqnw.sHtML

[Q13] 忽略重复插入
来源：http://blog.fanxiaobao.xyz/Article/details/gpftxtmce.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://baike.fanxiaobao.xyz/Article/details/gvjabbcrj.sHtML

[Q14] 存在则更新（upsert）
来源：http://mobile.fanxiaobao.xyz/Article/details/gqtjcwzix.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://3g.fanxiaobao.xyz/Article/details/gjnnjzhcl.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://m.share.fanxiaobao.xyz/Article/details/ggjesebdr.sHtML

[Q15] 查询全部
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbijdnsks.sHtML

SELECT * FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/getjsgcnb.sHtML

[Q16] 查询指定列
来源：http://baike.fanxiaobao.xyz/Article/details/gqwxwdnct.sHtML

SELECT id, name FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gikpndihb.sHtML

[Q17] 条件查询
来源：http://wap.fanxiaobao.xyz/Article/details/gqthlvyas.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.share.fanxiaobao.xyz/Article/details/gjpumqkwi.sHtML

[Q18] 模糊匹配
来源：http://wap.fanxiaobao.xyz/Article/details/glsscpces.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://3g.fanxiaobao.xyz/Article/details/gjzwrzvcu.sHtML

[Q19] 范围查询
来源：http://mobile.fanxiaobao.xyz/Article/details/gfswjbifh.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://read.share.fanxiaobao.xyz/Article/details/geowobepz.sHtML

[Q20] IN 列表
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtfevotyz.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://blog.fanxiaobao.xyz/Article/details/guatdcqcw.sHtML

[Q21] 空值判断
来源：http://www.blog.fanxiaobao.xyz/Article/details/gadkdeeqm.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://3g.fanxiaobao.xyz/Article/details/geigpmmqd.sHtML

[Q22] 排序
来源：http://blog.fanxiaobao.xyz/Article/details/gswgfijid.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://mobile.fanxiaobao.xyz/Article/details/gfllixacs.sHtML

[Q23] 分页
来源：http://www.share.fanxiaobao.xyz/Article/details/gqncmzdim.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://read.share.fanxiaobao.xyz/Article/details/ggldkifnd.sHtML

[Q24] 去重
来源：http://www.share.fanxiaobao.xyz/Article/details/gxpvbomaj.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggkdcwxva.sHtML

[Q25] 只取前 N 条
来源：http://m.share.fanxiaobao.xyz/Article/details/glpptqpdz.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://m.share.fanxiaobao.xyz/Article/details/gvsyyjwbn.sHtML

[Q26] 计数
来源：http://wap.fanxiaobao.xyz/Article/details/gugcphbae.sHtML

SELECT COUNT(*) FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gdiwrhrno.sHtML

[Q27] 条件计数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtasujcgm.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvyuzekau.sHtML

[Q28] 求和与平均
来源：http://www.share.fanxiaobao.xyz/Article/details/gkbytdxhl.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://m.share.fanxiaobao.xyz/Article/details/gmgwahakv.sHtML

[Q29] 最大最小值
来源：http://wap.fanxiaobao.xyz/Article/details/gbdswvomw.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gwvqyxahd.sHtML

[Q30] 分组统计
来源：http://mobile.fanxiaobao.xyz/Article/details/gmeoyxuuk.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.share.fanxiaobao.xyz/Article/details/gjpvdawfj.sHtML

[Q31] 分组后过滤
来源：http://3g.fanxiaobao.xyz/Article/details/gzcyxibvo.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://mobile.fanxiaobao.xyz/Article/details/glqtmmpks.sHtML

[Q32] 分组拼接字符串
来源：http://wap.fanxiaobao.xyz/Article/details/gzddhcjmt.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.share.fanxiaobao.xyz/Article/details/gnjhqslzq.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://read.share.fanxiaobao.xyz/Article/details/ggqzuarhv.sHtML

[Q33] 多列分组
来源：http://3g.fanxiaobao.xyz/Article/details/gulmvegmg.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://blog.fanxiaobao.xyz/Article/details/gopnelumb.sHtML

[Q34] 每组取第一条
来源：http://3g.fanxiaobao.xyz/Article/details/gneiioijf.sHtML

SELECT * FROM (
来源：http://blog.fanxiaobao.xyz/Article/details/gztycesbr.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvbctfbqh.sHtML

) t WHERE rn = 1;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwtwrvulx.sHtML

[Q35] 内连接
来源：http://www.share.fanxiaobao.xyz/Article/details/ggwlcjiao.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://blog.fanxiaobao.xyz/Article/details/gmafjrbop.sHtML

[Q36] 左连接
来源：http://wap.fanxiaobao.xyz/Article/details/gbgrcdfat.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://mobile.fanxiaobao.xyz/Article/details/gscdeumoo.sHtML

[Q37] 右连接
来源：http://www.share.fanxiaobao.xyz/Article/details/gngmnrhno.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://wap.fanxiaobao.xyz/Article/details/gnlahthje.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://baike.fanxiaobao.xyz/Article/details/gohubtehp.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://mobile.fanxiaobao.xyz/Article/details/gavlvgqhs.sHtML

[Q39] 自连接（查上下级）
来源：http://3g.fanxiaobao.xyz/Article/details/gqfssgzgq.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://read.share.fanxiaobao.xyz/Article/details/gttwilssg.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcjqzuaof.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://wap.fanxiaobao.xyz/Article/details/guevcwsdo.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://wap.fanxiaobao.xyz/Article/details/glyiqhxka.sHtML

[Q41] 多表连接
来源：http://mobile.fanxiaobao.xyz/Article/details/gztejlrfy.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://m.share.fanxiaobao.xyz/Article/details/geuualkhf.sHtML

JOIN users u ON u.id = o.user_id
来源：http://read.share.fanxiaobao.xyz/Article/details/gtbpvcqca.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://baike.fanxiaobao.xyz/Article/details/goefahfyv.sHtML

[Q42] 连接条件附加过滤
来源：http://mobile.fanxiaobao.xyz/Article/details/gowthpavq.sHtML

SELECT u.name, o.amount FROM users u
来源：http://wap.fanxiaobao.xyz/Article/details/gjglarcwd.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://read.share.fanxiaobao.xyz/Article/details/ghzbjhhxp.sHtML

[Q43] 标量子查询
来源：http://blog.fanxiaobao.xyz/Article/details/gjjtseuuo.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://baike.fanxiaobao.xyz/Article/details/gbivztwks.sHtML

[Q44] IN 子查询
来源：http://blog.fanxiaobao.xyz/Article/details/gasqqfyyv.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gehucqpcj.sHtML

[Q45] EXISTS 判断存在
来源：http://www.blog.fanxiaobao.xyz/Article/details/gueduwlwg.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.fanxiaobao.xyz/Article/details/gmsjdhtjm.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://blog.fanxiaobao.xyz/Article/details/gqeydvett.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.fanxiaobao.xyz/Article/details/gkgzogknk.sHtML

[Q47] 与平均值比较
来源：http://blog.fanxiaobao.xyz/Article/details/goljpiyyl.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://wap.fanxiaobao.xyz/Article/details/gygtvggdy.sHtML

[Q48] CTE 公用表表达式
来源：http://blog.fanxiaobao.xyz/Article/details/guawpnegp.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcbrzvhtr.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://mobile.fanxiaobao.xyz/Article/details/gpckiukpu.sHtML

[Q49] 更新单行
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwosfxysx.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://mobile.fanxiaobao.xyz/Article/details/gsstqqmrx.sHtML

[Q50] 批量更新
来源：http://baike.fanxiaobao.xyz/Article/details/gaslczuse.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://wap.fanxiaobao.xyz/Article/details/giejfzsho.sHtML

[Q51] 用子查询更新
来源：http://read.share.fanxiaobao.xyz/Article/details/gjiepntvs.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gosktagdh.sHtML

[Q52] 删除指定行
来源：http://www.share.fanxiaobao.xyz/Article/details/gmryvorqj.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.share.fanxiaobao.xyz/Article/details/gxojnpdxr.sHtML

[Q53] 按条件删除
来源：http://www.share.fanxiaobao.xyz/Article/details/gbbecvcqp.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.blog.fanxiaobao.xyz/Article/details/gruxaidaq.sHtML

[Q54] 清空表
来源：http://www.share.fanxiaobao.xyz/Article/details/gvwteytvg.sHtML

TRUNCATE TABLE logs;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvwoqbhnq.sHtML

[Q55] 排名（并列占位）
来源：http://read.share.fanxiaobao.xyz/Article/details/gznbpbhff.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghiazzdqi.sHtML

[Q56] 密集排名（并列不占位）
来源：http://3g.fanxiaobao.xyz/Article/details/gswkgtctu.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://read.share.fanxiaobao.xyz/Article/details/gaaouytco.sHtML

[Q57] 行号
来源：http://read.share.fanxiaobao.xyz/Article/details/gmhshxmfc.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfugntmlt.sHtML

[Q58] 累计求和
来源：http://mobile.fanxiaobao.xyz/Article/details/ghnzwunla.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://blog.fanxiaobao.xyz/Article/details/gdwjrjrtx.sHtML

[Q59] 分组内累计
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggemovvip.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvghrxktu.sHtML

[Q60] 取上一行 / 下一行
来源：http://baike.fanxiaobao.xyz/Article/details/gfrrmarie.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://3g.fanxiaobao.xyz/Article/details/gvkwdmpgu.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://blog.fanxiaobao.xyz/Article/details/gimrcusbh.sHtML

[Q61] 移动平均
来源：http://www.share.fanxiaobao.xyz/Article/details/gojkmjlhs.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://baike.fanxiaobao.xyz/Article/details/gqjnzlydr.sHtML

[Q62] 分组占比
来源：http://read.share.fanxiaobao.xyz/Article/details/gwtuovitp.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://3g.fanxiaobao.xyz/Article/details/gxellwfwv.sHtML

[Q63] 开启事务
来源：http://read.share.fanxiaobao.xyz/Article/details/gxdnwxhse.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://read.share.fanxiaobao.xyz/Article/details/gfuqknbfd.sHtML

[Q64] 提交事务
来源：http://baike.fanxiaobao.xyz/Article/details/gbgnxwfrh.sHtML

COMMIT;
来源：http://3g.fanxiaobao.xyz/Article/details/gichnpece.sHtML

[Q65] 回滚事务
来源：http://3g.fanxiaobao.xyz/Article/details/guxfnyyrh.sHtML

ROLLBACK;
来源：http://www.share.fanxiaobao.xyz/Article/details/glkiyanbg.sHtML

[Q66] 行锁查询
来源：http://mobile.fanxiaobao.xyz/Article/details/gkycttbig.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://read.share.fanxiaobao.xyz/Article/details/gjkfskovy.sHtML

[Q67] 设置隔离级别
来源：http://wap.fanxiaobao.xyz/Article/details/gbaesrfbu.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.share.fanxiaobao.xyz/Article/details/gtlrklsxf.sHtML

[Q68] 保存点
来源：http://www.share.fanxiaobao.xyz/Article/details/gnqjwgwyk.sHtML

SAVEPOINT sp1;
来源：http://m.share.fanxiaobao.xyz/Article/details/gddoajjth.sHtML

ROLLBACK TO sp1;
来源：http://wap.fanxiaobao.xyz/Article/details/gjvdbtzbl.sHtML

[Q69] 查看执行计划
来源：http://mobile.fanxiaobao.xyz/Article/details/gdwehgxvm.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwxgvgqit.sHtML

[Q70] 更新统计信息
来源：http://mobile.fanxiaobao.xyz/Article/details/gtyrdsbrp.sHtML

ANALYZE TABLE users;
来源：http://m.share.fanxiaobao.xyz/Article/details/grssvfbow.sHtML

[Q71] 查看建表语句
来源：http://mobile.fanxiaobao.xyz/Article/details/gpttzurvb.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://baike.fanxiaobao.xyz/Article/details/geglptagr.sHtML

[Q72] 查看索引
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geuoriekp.sHtML

SHOW INDEX FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gwownheio.sHtML

[Q73] 查看表状态
来源：http://baike.fanxiaobao.xyz/Article/details/golskisrv.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzpnnvkii.sHtML

[Q74] 强制使用索引
来源：http://wap.fanxiaobao.xyz/Article/details/gavonmruq.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://mobile.fanxiaobao.xyz/Article/details/gsanbgdxn.sHtML

[Q75] 日期格式化
来源：http://read.share.fanxiaobao.xyz/Article/details/gntlroutq.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.blog.fanxiaobao.xyz/Article/details/geolalnwo.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://3g.fanxiaobao.xyz/Article/details/gheguyiwq.sHtML

[Q76] 按天统计
来源：http://www.share.fanxiaobao.xyz/Article/details/gdezqpchc.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gafslmerl.sHtML

[Q77] 时间加减
来源：http://3g.fanxiaobao.xyz/Article/details/ghmxqjaid.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://read.share.fanxiaobao.xyz/Article/details/gygldpsgb.sHtML

[Q78] 当前时间
来源：http://wap.fanxiaobao.xyz/Article/details/gebpggtkx.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://wap.fanxiaobao.xyz/Article/details/gmvqdcubh.sHtML

[Q79] 字符串拼接
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glpathynw.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqqxsufyh.sHtML

[Q80] 字符串截取
来源：http://wap.fanxiaobao.xyz/Article/details/gswtzdcee.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbyhvgjcv.sHtML

[Q81] 字符串替换
来源：http://read.share.fanxiaobao.xyz/Article/details/gaxcemqmb.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/guakpzjdp.sHtML

[Q82] 字符长度与字节长度
来源：http://3g.fanxiaobao.xyz/Article/details/gcedjjhzz.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gfpzfyjbq.sHtML

[Q83] 大小写转换
来源：http://www.share.fanxiaobao.xyz/Article/details/gbcclohpe.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gizgbjbdn.sHtML

[Q84] 去除首尾空格
来源：http://blog.fanxiaobao.xyz/Article/details/gztamubvi.sHtML

SELECT TRIM(name) FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gxldnqiko.sHtML

[Q85] 数值取整
来源：http://read.share.fanxiaobao.xyz/Article/details/gjywjzhva.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://m.share.fanxiaobao.xyz/Article/details/gzdsjuthn.sHtML

[Q86] 读取 JSON 字段
来源：http://baike.fanxiaobao.xyz/Article/details/giwvcibte.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://blog.fanxiaobao.xyz/Article/details/gkvgliojd.sHtML

[Q87] JSON 字段做条件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjbpxpjwo.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqyetunlf.sHtML

[Q88] 行转列（条件聚合）
来源：http://m.share.fanxiaobao.xyz/Article/details/gjqjfzdwt.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.blog.fanxiaobao.xyz/Article/details/grbtbxzuj.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gnnrfqjau.sHtML

[Q89] 判断表是否存在
来源：http://mobile.fanxiaobao.xyz/Article/details/guahgsbpz.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.share.fanxiaobao.xyz/Article/details/gvlyuhnmu.sHtML

[Q90] 生成序号列
来源：http://wap.fanxiaobao.xyz/Article/details/glzluhcvr.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://read.share.fanxiaobao.xyz/Article/details/geaekfmpu.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaqdssrch.sHtML

R. Bash 专题
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwglnseui.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/ggnxocftb.sHtML

[R01] shebang 与严格模式
来源：http://mobile.fanxiaobao.xyz/Article/details/gagusswvt.sHtML

#!/usr/bin/env bash
来源：http://mobile.fanxiaobao.xyz/Article/details/ggzsliceq.sHtML

set -euo pipefail
来源：http://3g.fanxiaobao.xyz/Article/details/grdvxqkkj.sHtML

[R02] 变量赋值与使用
来源：http://read.share.fanxiaobao.xyz/Article/details/gbblbtdzm.sHtML

name="Tom"; echo "$name"
来源：http://www.share.fanxiaobao.xyz/Article/details/gcbbrwyjc.sHtML

[R03] 只读变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxhoihdmk.sHtML

readonly PI=3.14
来源：http://3g.fanxiaobao.xyz/Article/details/geakchkkw.sHtML

[R04] 位置参数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gruzykkfp.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://mobile.fanxiaobao.xyz/Article/details/goattmece.sHtML

[R05] 参数默认值
来源：http://www.share.fanxiaobao.xyz/Article/details/gvkbepkpg.sHtML

name="${1:-default}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gprwariwg.sHtML

[R06] 判断命令是否存在
来源：http://blog.fanxiaobao.xyz/Article/details/gqdsfaisu.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://baike.fanxiaobao.xyz/Article/details/goqgpgzfk.sHtML

[R07] if 判断文件
来源：http://blog.fanxiaobao.xyz/Article/details/gdjzurthb.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://mobile.fanxiaobao.xyz/Article/details/gaifkonsg.sHtML

[R08] 数值比较
来源：http://baike.fanxiaobao.xyz/Article/details/gzqzpocsb.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://baike.fanxiaobao.xyz/Article/details/gmurlfeqq.sHtML

[R09] 字符串比较
来源：http://mobile.fanxiaobao.xyz/Article/details/gvjmasltr.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://baike.fanxiaobao.xyz/Article/details/gbmgwucbd.sHtML

[R10] 正则匹配
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdupexyxj.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://read.share.fanxiaobao.xyz/Article/details/ggygemaal.sHtML

[R11] case 多分支
来源：http://mobile.fanxiaobao.xyz/Article/details/gqnlqdaxm.sHtML

case "$1" in
来源：http://m.share.fanxiaobao.xyz/Article/details/gmnqvapho.sHtML

start) echo "启动" ;;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnhhkkefs.sHtML

stop)  echo "停止" ;;
来源：http://3g.fanxiaobao.xyz/Article/details/gcbqtlhcn.sHtML

*)     echo "未知命令" ;;
来源：http://blog.fanxiaobao.xyz/Article/details/gbkldykfo.sHtML

esac
来源：http://www.blog.fanxiaobao.xyz/Article/details/giwgmofwl.sHtML

[R12] for 遍历文件
来源：http://wap.fanxiaobao.xyz/Article/details/gjqppymvi.sHtML

for f in *.txt; do echo "$f"; done
来源：http://wap.fanxiaobao.xyz/Article/details/gsktlseyx.sHtML

[R13] for 计数循环
来源：http://mobile.fanxiaobao.xyz/Article/details/grdcnajlf.sHtML


<!-- 参考信息 -->