代发 wailian999

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.share.fehbvm.com/Article/details/guhbfnfxn.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://wap.hesvh.cn/Article/details/govtfdyzm.sHtML

[P03] 生成短随机字符串
来源：http://www.blog.fehbvm.com/Article/details/gobojuqqa.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.m.share.hesvh.cn/Article/details/gmucujnpq.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://3g.fehbvm.com/Article/details/gvyjrodcz.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.fehbvm.com/Article/details/gidsaiizg.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.fehbvm.com/Article/details/grmxadcwp.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://read.share.hesvh.cn/Article/details/gcyjbtofl.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://read.share.hesvh.cn/Article/details/gvqpnbzbo.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://baike.zdbjq.cn/Article/details/ggujeglvm.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://baike.hesvh.cn/Article/details/gztmwilhp.sHtML

[P04] 求长度
来源：http://read.share.zdbjq.cn/Article/details/gnntmwzsn.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://m.share.hesvh.cn/Article/details/gpxmkmyjw.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.zdbjq.cn/Article/details/glfmazglz.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mobile.zdbjq.cn/Article/details/gbkgaqyfo.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.hesvh.cn/Article/details/genpffwad.sHtML

Java: list.size();  map.size();  s.length()
来源：http://3g.fehbvm.com/Article/details/gjckpdxsy.sHtML

Go:   len(arr);  len(m)
来源：http://wap.fehbvm.com/Article/details/gzsfaoeuv.sHtML

Ruby: x.length;  x.size
来源：http://wap.fehbvm.com/Article/details/gwtrasffr.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.m.share.fehbvm.com/Article/details/gddlpmptr.sHtML

[P05] 判断两个对象内容是否相等
来源：http://read.share.zdbjq.cn/Article/details/gkhzzdmtj.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.m.share.hesvh.cn/Article/details/gixbjfsst.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://read.share.fehbvm.com/Article/details/gjwkdfjkb.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://baike.hesvh.cn/Article/details/gnszqyrea.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.zdbjq.cn/Article/details/gextnsazp.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://blog.zdbjq.cn/Article/details/gejgpyxwe.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.blog.zdbjq.cn/Article/details/gllvwrnjl.sHtML

Ruby: a == b
来源：http://www.blog.hesvh.cn/Article/details/gakhvkfla.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://mobile.hesvh.cn/Article/details/gelakomvq.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://baike.zdbjq.cn/Article/details/grutvrlyo.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://mobile.zdbjq.cn/Article/details/gersgporz.sHtML

PHP:  if (empty($x)) {}
来源：http://3g.zdbjq.cn/Article/details/gsxbytxfd.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.share.fehbvm.com/Article/details/giboovhhm.sHtML

TS:   if (x == null) {}
来源：http://mobile.fehbvm.com/Article/details/gkgqjjitk.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://3g.hesvh.cn/Article/details/gnnrdcjms.sHtML

Go:   if x == nil {}
来源：http://wap.fehbvm.com/Article/details/ginllyvwx.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://3g.hesvh.cn/Article/details/gqbhiornh.sHtML

C#:   if (x is null) {}
来源：http://www.share.zdbjq.cn/Article/details/guuhyokzz.sHtML

[P07] 防抖与节流
来源：http://wap.zdbjq.cn/Article/details/gkyjcebsl.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://mobile.hesvh.cn/Article/details/gsccyxzjv.sHtML

PHP:  // 手写时间戳比较
来源：http://www.share.hesvh.cn/Article/details/gjdxnsrcq.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.hesvh.cn/Article/details/gkztnrhtc.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.fehbvm.com/Article/details/giinaafgb.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.share.fehbvm.com/Article/details/glzimdkzr.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.share.hesvh.cn/Article/details/gsddcufhm.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://m.share.hesvh.cn/Article/details/gzzwhjwmg.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://baike.fehbvm.com/Article/details/gyvvbgfxn.sHtML

[P08] 处理浮点精度问题
来源：http://3g.fehbvm.com/Article/details/gnjsqujxc.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://wap.zdbjq.cn/Article/details/glgzijxhn.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://blog.fehbvm.com/Article/details/ggfggtfav.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://3g.zdbjq.cn/Article/details/gdqbqcqji.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://3g.zdbjq.cn/Article/details/geqksiaqk.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.share.hesvh.cn/Article/details/gublpcfga.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.share.hesvh.cn/Article/details/gjohwlhqs.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.share.fehbvm.com/Article/details/gmvgaobtk.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://baike.fehbvm.com/Article/details/gdlxhoepe.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/ghgzszbvn.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.blog.hesvh.cn/Article/details/gfvscjyjh.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/glwehkufh.sHtML

[Q01] 创建表
来源：http://3g.zdbjq.cn/Article/details/goaltjibz.sHtML

CREATE TABLE users (
来源：http://blog.fehbvm.com/Article/details/gbizslkkn.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.fehbvm.com/Article/details/ggazbexfk.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.share.hesvh.cn/Article/details/gnhwbibso.sHtML

email VARCHAR(100) UNIQUE,
来源：http://wap.fehbvm.com/Article/details/gklmwjzrm.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.share.zdbjq.cn/Article/details/gtvxslhek.sHtML

);
来源：http://mobile.fehbvm.com/Article/details/gvieknsuo.sHtML

[Q02] 创建带外键的表
来源：http://www.share.fehbvm.com/Article/details/gkoulycxy.sHtML

CREATE TABLE orders (
来源：http://m.share.fehbvm.com/Article/details/ggjqdrult.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.share.fehbvm.com/Article/details/gayhfltel.sHtML

user_id INT NOT NULL,
来源：http://m.share.hesvh.cn/Article/details/gpqmzmpkc.sHtML

amount DECIMAL(10, 2),
来源：http://www.blog.zdbjq.cn/Article/details/gtyrbebbh.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.m.share.zdbjq.cn/Article/details/gdverchyd.sHtML

);
来源：http://3g.zdbjq.cn/Article/details/gngtktqmx.sHtML

[Q03] 增加列
来源：http://baike.hesvh.cn/Article/details/ghqkjfaxm.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.blog.fehbvm.com/Article/details/ggjdvyrvr.sHtML

[Q04] 修改列类型
来源：http://www.share.zdbjq.cn/Article/details/gjerujfrq.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.m.share.fehbvm.com/Article/details/grnsvpyqj.sHtML

[Q05] 重命名列
来源：http://www.blog.fehbvm.com/Article/details/gifylnthc.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://baike.zdbjq.cn/Article/details/gsutfbzri.sHtML

[Q06] 删除列
来源：http://www.share.fehbvm.com/Article/details/gkjgopxxk.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://read.share.hesvh.cn/Article/details/gdlpxfxro.sHtML

[Q07] 删除表
来源：http://mobile.zdbjq.cn/Article/details/gdceyskhb.sHtML

DROP TABLE IF EXISTS orders;
来源：http://baike.fehbvm.com/Article/details/gfgdbnxru.sHtML

[Q08] 创建普通索引
来源：http://www.blog.fehbvm.com/Article/details/ghzbsbcwi.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.share.fehbvm.com/Article/details/gfpelrleh.sHtML

[Q09] 创建唯一索引
来源：http://blog.zdbjq.cn/Article/details/gojkbxzxw.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.m.share.zdbjq.cn/Article/details/gucbukyak.sHtML

[Q10] 插入单行
来源：http://baike.zdbjq.cn/Article/details/glbdmbaok.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://blog.hesvh.cn/Article/details/geiwbkjhx.sHtML

[Q11] 一次插入多行
来源：http://mobile.zdbjq.cn/Article/details/gddvjzvvb.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://3g.fehbvm.com/Article/details/gwtejqtec.sHtML

[Q12] 插入后取自增 ID
来源：http://www.share.fehbvm.com/Article/details/gzvzvdbqk.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.blog.hesvh.cn/Article/details/gzqbajwwg.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.blog.fehbvm.com/Article/details/gydautftf.sHtML

[Q13] 忽略重复插入
来源：http://read.share.zdbjq.cn/Article/details/gvmfiaxkj.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://mobile.fehbvm.com/Article/details/grexeaklq.sHtML

[Q14] 存在则更新（upsert）
来源：http://blog.zdbjq.cn/Article/details/ghqzuthfi.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.blog.zdbjq.cn/Article/details/gblufcdfy.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://blog.zdbjq.cn/Article/details/gptpmdxmc.sHtML

[Q15] 查询全部
来源：http://www.share.hesvh.cn/Article/details/gspihghzs.sHtML

SELECT * FROM users;
来源：http://m.share.hesvh.cn/Article/details/gnpywjlvj.sHtML

[Q16] 查询指定列
来源：http://wap.fehbvm.com/Article/details/gjhwnjlyb.sHtML

SELECT id, name FROM users;
来源：http://www.blog.hesvh.cn/Article/details/ghvxmrjpy.sHtML

[Q17] 条件查询
来源：http://mobile.hesvh.cn/Article/details/gvrfzwncl.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://mobile.fehbvm.com/Article/details/grnbvmpmi.sHtML

[Q18] 模糊匹配
来源：http://mobile.zdbjq.cn/Article/details/gdamumhub.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://baike.zdbjq.cn/Article/details/ggsjpbhrq.sHtML

[Q19] 范围查询
来源：http://m.share.hesvh.cn/Article/details/ghqqeaxgc.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.blog.fehbvm.com/Article/details/gpklwfmem.sHtML

[Q20] IN 列表
来源：http://www.share.fehbvm.com/Article/details/gxgfgumgg.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://mobile.zdbjq.cn/Article/details/gfmkbvebj.sHtML

[Q21] 空值判断
来源：http://blog.zdbjq.cn/Article/details/gesvwlekm.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.m.share.zdbjq.cn/Article/details/gifrdhcuu.sHtML

[Q22] 排序
来源：http://www.share.zdbjq.cn/Article/details/gtfukvamh.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.share.zdbjq.cn/Article/details/givaopryz.sHtML

[Q23] 分页
来源：http://3g.hesvh.cn/Article/details/gwjkvelbw.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://baike.hesvh.cn/Article/details/gbniimylm.sHtML

[Q24] 去重
来源：http://read.share.zdbjq.cn/Article/details/gzngqexja.sHtML

SELECT DISTINCT city FROM users;
来源：http://m.share.hesvh.cn/Article/details/gttkkbihx.sHtML

[Q25] 只取前 N 条
来源：http://3g.zdbjq.cn/Article/details/gwjgcniok.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://m.share.hesvh.cn/Article/details/gkuureoyi.sHtML

[Q26] 计数
来源：http://m.share.fehbvm.com/Article/details/gbujxkyyj.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gnhbbgdhp.sHtML

[Q27] 条件计数
来源：http://www.share.hesvh.cn/Article/details/gnpjklqfo.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gjsyteycr.sHtML

[Q28] 求和与平均
来源：http://mobile.fehbvm.com/Article/details/grzwwhkiz.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.share.hesvh.cn/Article/details/gugorkvuy.sHtML

[Q29] 最大最小值
来源：http://3g.hesvh.cn/Article/details/gkarhggrb.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://3g.zdbjq.cn/Article/details/gbcldctpz.sHtML

[Q30] 分组统计
来源：http://read.share.zdbjq.cn/Article/details/gevwsuggi.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://3g.hesvh.cn/Article/details/goehulzlx.sHtML

[Q31] 分组后过滤
来源：http://www.blog.zdbjq.cn/Article/details/gjyoilvln.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://read.share.hesvh.cn/Article/details/gcnbepfxc.sHtML

[Q32] 分组拼接字符串
来源：http://mobile.hesvh.cn/Article/details/glxjvlfca.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.blog.hesvh.cn/Article/details/gmcvtvltc.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://mobile.hesvh.cn/Article/details/gjkmnykfy.sHtML

[Q33] 多列分组
来源：http://blog.hesvh.cn/Article/details/gaiobsike.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://m.share.fehbvm.com/Article/details/gkjsbjqbo.sHtML

[Q34] 每组取第一条
来源：http://mobile.hesvh.cn/Article/details/gydbihadn.sHtML

SELECT * FROM (
来源：http://baike.zdbjq.cn/Article/details/gyatogtgz.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://3g.fehbvm.com/Article/details/ggnwjwuwj.sHtML

) t WHERE rn = 1;
来源：http://blog.zdbjq.cn/Article/details/gvanlbbxi.sHtML

[Q35] 内连接
来源：http://blog.zdbjq.cn/Article/details/gklvpnmuq.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://blog.hesvh.cn/Article/details/glogmeosa.sHtML

[Q36] 左连接
来源：http://3g.hesvh.cn/Article/details/gthvtwuax.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.hesvh.cn/Article/details/gvginnpof.sHtML

[Q37] 右连接
来源：http://m.share.zdbjq.cn/Article/details/gaopqbmyh.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.share.fehbvm.com/Article/details/gxhkcggae.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.m.share.hesvh.cn/Article/details/gvusedizp.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.blog.fehbvm.com/Article/details/gbvggxjiv.sHtML

[Q39] 自连接（查上下级）
来源：http://wap.zdbjq.cn/Article/details/gcootsssn.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://blog.fehbvm.com/Article/details/gbjfvkkci.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://blog.hesvh.cn/Article/details/gyvdrdgyk.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://blog.zdbjq.cn/Article/details/gfeytvkrt.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://blog.fehbvm.com/Article/details/grhtbkmfp.sHtML

[Q41] 多表连接
来源：http://read.share.fehbvm.com/Article/details/gmbdkvhxe.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://wap.fehbvm.com/Article/details/giizilbjd.sHtML

JOIN users u ON u.id = o.user_id
来源：http://read.share.fehbvm.com/Article/details/gewhbvyvq.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.m.share.fehbvm.com/Article/details/gssbkwtlp.sHtML

[Q42] 连接条件附加过滤
来源：http://www.m.share.fehbvm.com/Article/details/gfspylfqj.sHtML

SELECT u.name, o.amount FROM users u
来源：http://baike.hesvh.cn/Article/details/gwrxqsekn.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.blog.zdbjq.cn/Article/details/glmlnssqf.sHtML

[Q43] 标量子查询
来源：http://www.m.share.hesvh.cn/Article/details/gztqvhsfc.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.m.share.fehbvm.com/Article/details/gymrvpwgc.sHtML

[Q44] IN 子查询
来源：http://www.share.zdbjq.cn/Article/details/gpftapjiy.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://read.share.zdbjq.cn/Article/details/gxxyzejjy.sHtML

[Q45] EXISTS 判断存在
来源：http://wap.hesvh.cn/Article/details/ghuxgvido.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.fehbvm.com/Article/details/gcmwiqwvg.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://read.share.zdbjq.cn/Article/details/golraruuk.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.zdbjq.cn/Article/details/gtmxmrrfx.sHtML

[Q47] 与平均值比较
来源：http://mobile.fehbvm.com/Article/details/gkljgckdq.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.m.share.zdbjq.cn/Article/details/gochixzul.sHtML

[Q48] CTE 公用表表达式
来源：http://www.m.share.zdbjq.cn/Article/details/gqelykfzp.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://baike.hesvh.cn/Article/details/gnnczevbc.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.m.share.hesvh.cn/Article/details/gfrrzynac.sHtML

[Q49] 更新单行
来源：http://www.m.share.fehbvm.com/Article/details/grsfhaimt.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.m.share.hesvh.cn/Article/details/gipselqjg.sHtML

[Q50] 批量更新
来源：http://blog.hesvh.cn/Article/details/gxnzlapvp.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.m.share.hesvh.cn/Article/details/gsjnamxug.sHtML

[Q51] 用子查询更新
来源：http://mobile.fehbvm.com/Article/details/gdvczzcyx.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.m.share.zdbjq.cn/Article/details/gmuokhmve.sHtML

[Q52] 删除指定行
来源：http://m.share.fehbvm.com/Article/details/ghmymifxv.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.m.share.hesvh.cn/Article/details/gjyttjiwp.sHtML

[Q53] 按条件删除
来源：http://www.share.fehbvm.com/Article/details/gxqkhknss.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://baike.hesvh.cn/Article/details/gasghcwpa.sHtML

[Q54] 清空表
来源：http://baike.fehbvm.com/Article/details/gfqmbrlrg.sHtML

TRUNCATE TABLE logs;
来源：http://blog.hesvh.cn/Article/details/gkyqdvkno.sHtML

[Q55] 排名（并列占位）
来源：http://3g.fehbvm.com/Article/details/gigbfeahb.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://blog.hesvh.cn/Article/details/gnzcqzwbd.sHtML

[Q56] 密集排名（并列不占位）
来源：http://m.share.hesvh.cn/Article/details/gqpdbmdpw.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://blog.fehbvm.com/Article/details/gosiyyszt.sHtML

[Q57] 行号
来源：http://wap.zdbjq.cn/Article/details/gfqipchmt.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gwbbosolt.sHtML

[Q58] 累计求和
来源：http://mobile.zdbjq.cn/Article/details/gmolzlwkp.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://3g.zdbjq.cn/Article/details/gzjhlvfyl.sHtML

[Q59] 分组内累计
来源：http://www.share.zdbjq.cn/Article/details/gahlmjajc.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://m.share.fehbvm.com/Article/details/gygrklbdq.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.blog.zdbjq.cn/Article/details/gjuvlwtng.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://3g.fehbvm.com/Article/details/giupytjek.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://3g.hesvh.cn/Article/details/gthnxsbgj.sHtML

[Q61] 移动平均
来源：http://m.share.zdbjq.cn/Article/details/gorcsgndj.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://blog.hesvh.cn/Article/details/geizjwtvm.sHtML

[Q62] 分组占比
来源：http://3g.fehbvm.com/Article/details/gdvnhrxiv.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.m.share.hesvh.cn/Article/details/gppgcdkzd.sHtML

[Q63] 开启事务
来源：http://baike.zdbjq.cn/Article/details/gwomrfxrw.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://mobile.fehbvm.com/Article/details/gydkxubrv.sHtML

[Q64] 提交事务
来源：http://blog.fehbvm.com/Article/details/gnllfbeiu.sHtML

COMMIT;
来源：http://blog.zdbjq.cn/Article/details/grmhwsegp.sHtML

[Q65] 回滚事务
来源：http://mobile.hesvh.cn/Article/details/gdsdedqpr.sHtML

ROLLBACK;
来源：http://3g.hesvh.cn/Article/details/graboorwx.sHtML

[Q66] 行锁查询
来源：http://mobile.zdbjq.cn/Article/details/golrdkhda.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://3g.zdbjq.cn/Article/details/gxwnogivm.sHtML

[Q67] 设置隔离级别
来源：http://www.m.share.zdbjq.cn/Article/details/gggdfeugl.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://m.share.hesvh.cn/Article/details/gnbqjfleb.sHtML

[Q68] 保存点
来源：http://www.share.fehbvm.com/Article/details/gkjczmtnp.sHtML

SAVEPOINT sp1;
来源：http://read.share.hesvh.cn/Article/details/gpsvsiqhr.sHtML

ROLLBACK TO sp1;
来源：http://wap.fehbvm.com/Article/details/gwpenzpel.sHtML

[Q69] 查看执行计划
来源：http://wap.zdbjq.cn/Article/details/gpmcorcos.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.m.share.zdbjq.cn/Article/details/gnsdzsbmz.sHtML

[Q70] 更新统计信息
来源：http://wap.hesvh.cn/Article/details/goffnqskm.sHtML

ANALYZE TABLE users;
来源：http://3g.fehbvm.com/Article/details/geqzpthve.sHtML

[Q71] 查看建表语句
来源：http://3g.fehbvm.com/Article/details/gpyednvuz.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://blog.zdbjq.cn/Article/details/gvgxlpmuu.sHtML

[Q72] 查看索引
来源：http://blog.fehbvm.com/Article/details/gebqmykcq.sHtML

SHOW INDEX FROM users;
来源：http://blog.hesvh.cn/Article/details/gonlllbsd.sHtML

[Q73] 查看表状态
来源：http://baike.hesvh.cn/Article/details/gndwnmpwr.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.blog.hesvh.cn/Article/details/gujqrdlfq.sHtML

[Q74] 强制使用索引
来源：http://baike.hesvh.cn/Article/details/gwkdyiyes.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://blog.hesvh.cn/Article/details/gzhrxqoft.sHtML

[Q75] 日期格式化
来源：http://3g.hesvh.cn/Article/details/gcspmvwdd.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.blog.fehbvm.com/Article/details/ggsdttzgh.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.m.share.zdbjq.cn/Article/details/gczgpjthn.sHtML

[Q76] 按天统计
来源：http://www.m.share.hesvh.cn/Article/details/gsizwsyld.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.blog.hesvh.cn/Article/details/gnarjojwo.sHtML

[Q77] 时间加减
来源：http://blog.fehbvm.com/Article/details/ghzphtekc.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://wap.zdbjq.cn/Article/details/githofnps.sHtML

[Q78] 当前时间
来源：http://www.blog.hesvh.cn/Article/details/gboyvwphy.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.m.share.hesvh.cn/Article/details/gmsjizvsc.sHtML

[Q79] 字符串拼接
来源：http://3g.fehbvm.com/Article/details/ghsppedgc.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://baike.zdbjq.cn/Article/details/gmegqpyuz.sHtML

[Q80] 字符串截取
来源：http://m.share.fehbvm.com/Article/details/gcudpepfg.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://mobile.hesvh.cn/Article/details/gfqymcdzq.sHtML

[Q81] 字符串替换
来源：http://www.blog.hesvh.cn/Article/details/gmoxoouzg.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://m.share.hesvh.cn/Article/details/gkdgqasge.sHtML

[Q82] 字符长度与字节长度
来源：http://read.share.zdbjq.cn/Article/details/ghgthtgjb.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gnmqrcicr.sHtML

[Q83] 大小写转换
来源：http://m.share.fehbvm.com/Article/details/gwupjdasu.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://read.share.zdbjq.cn/Article/details/glhnpscef.sHtML

[Q84] 去除首尾空格
来源：http://www.m.share.hesvh.cn/Article/details/gcuhjibwm.sHtML

SELECT TRIM(name) FROM users;
来源：http://read.share.hesvh.cn/Article/details/gopvuytck.sHtML

[Q85] 数值取整
来源：http://read.share.hesvh.cn/Article/details/gzrqhfjyk.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://m.share.zdbjq.cn/Article/details/gpummoqnf.sHtML

[Q86] 读取 JSON 字段
来源：http://www.blog.hesvh.cn/Article/details/glpfrbqjm.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://mobile.fehbvm.com/Article/details/gkreqkrac.sHtML

[Q87] JSON 字段做条件
来源：http://3g.fehbvm.com/Article/details/gzdbjkdds.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://wap.fehbvm.com/Article/details/geccfteka.sHtML

[Q88] 行转列（条件聚合）
来源：http://blog.fehbvm.com/Article/details/gzneuemux.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://3g.zdbjq.cn/Article/details/gkosvcreo.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gjfykpdkt.sHtML

[Q89] 判断表是否存在
来源：http://wap.fehbvm.com/Article/details/gkjgewnbt.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.share.fehbvm.com/Article/details/gofzrvgzt.sHtML

[Q90] 生成序号列
来源：http://3g.zdbjq.cn/Article/details/gysotsrnc.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.m.share.hesvh.cn/Article/details/gmcksgbyd.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gsimefqbu.sHtML

R. Bash 专题
来源：http://blog.hesvh.cn/Article/details/gwovfzcvr.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gemwavbvc.sHtML

[R01] shebang 与严格模式
来源：http://www.blog.fehbvm.com/Article/details/gevbdraro.sHtML

#!/usr/bin/env bash
来源：http://wap.hesvh.cn/Article/details/gjyaofbyz.sHtML

set -euo pipefail
来源：http://3g.zdbjq.cn/Article/details/gocbiwpzc.sHtML

[R02] 变量赋值与使用
来源：http://m.share.zdbjq.cn/Article/details/goiwcfojo.sHtML

name="Tom"; echo "$name"
来源：http://baike.zdbjq.cn/Article/details/gyvoefxho.sHtML

[R03] 只读变量
来源：http://blog.zdbjq.cn/Article/details/gthbpkofs.sHtML

readonly PI=3.14
来源：http://wap.zdbjq.cn/Article/details/glponmwcg.sHtML

[R04] 位置参数
来源：http://blog.hesvh.cn/Article/details/gnnknpfvc.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://wap.hesvh.cn/Article/details/gtjtgaerz.sHtML

[R05] 参数默认值
来源：http://wap.fehbvm.com/Article/details/glzztscqp.sHtML

name="${1:-default}"
来源：http://www.share.hesvh.cn/Article/details/ghjadzuhe.sHtML

[R06] 判断命令是否存在
来源：http://baike.fehbvm.com/Article/details/gbzfanimc.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.blog.fehbvm.com/Article/details/gbisenbec.sHtML

[R07] if 判断文件
来源：http://baike.fehbvm.com/Article/details/gstmmmcmy.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://mobile.fehbvm.com/Article/details/glokfrvoo.sHtML

[R08] 数值比较
来源：http://wap.hesvh.cn/Article/details/gwhayqgei.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://mobile.hesvh.cn/Article/details/ggvyubibm.sHtML

[R09] 字符串比较
来源：http://wap.fehbvm.com/Article/details/gyqmrjbdo.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://3g.hesvh.cn/Article/details/guvenatpn.sHtML

[R10] 正则匹配
来源：http://mobile.zdbjq.cn/Article/details/gonewitau.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://read.share.fehbvm.com/Article/details/gehpmunlt.sHtML

[R11] case 多分支
来源：http://read.share.hesvh.cn/Article/details/goicqjcvq.sHtML

case "$1" in
来源：http://www.m.share.hesvh.cn/Article/details/gelievhai.sHtML

start) echo "启动" ;;
来源：http://blog.fehbvm.com/Article/details/gbixwztaz.sHtML

stop)  echo "停止" ;;
来源：http://wap.zdbjq.cn/Article/details/gahrvpsvv.sHtML

*)     echo "未知命令" ;;
来源：http://mobile.zdbjq.cn/Article/details/gaozpqozv.sHtML

esac
来源：http://www.share.hesvh.cn/Article/details/gaiqynqpt.sHtML

[R12] for 遍历文件
来源：http://www.share.hesvh.cn/Article/details/ggxjxdqxj.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.share.zdbjq.cn/Article/details/gudomyfju.sHtML

[R13] for 计数循环
来源：http://www.blog.fehbvm.com/Article/details/gfshnpzsi.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://read.share.hesvh.cn/Article/details/gkrjyeoom.sHtML

[R14] C 风格 for
来源：http://3g.zdbjq.cn/Article/details/guxaluaaq.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://m.share.fehbvm.com/Article/details/gauxfnvqt.sHtML

[R15] while 逐行读文件
来源：http://m.share.hesvh.cn/Article/details/grdzlokgr.sHtML


<!-- 参考信息 -->