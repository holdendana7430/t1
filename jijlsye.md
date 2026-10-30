代发 wailian999

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.blog.hesvh.cn/Article/details/gapdbkmtq.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.blog.hesvh.cn/Article/details/gnetppigi.sHtML

[P03] 生成短随机字符串
来源：http://3g.hesvh.cn/Article/details/gussriupn.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.share.fehbvm.com/Article/details/godbhuvgr.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://m.share.hesvh.cn/Article/details/giapsxicn.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.zdbjq.cn/Article/details/gphxgxlwk.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.zdbjq.cn/Article/details/geupvspee.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://baike.fehbvm.com/Article/details/gtcdlqurr.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://baike.zdbjq.cn/Article/details/gnvvhmytz.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://baike.zdbjq.cn/Article/details/gdfrpqkip.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://m.share.hesvh.cn/Article/details/gelhczakz.sHtML

[P04] 求长度
来源：http://m.share.hesvh.cn/Article/details/gxwfjamkc.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://baike.fehbvm.com/Article/details/gvhmdgvlj.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://read.share.hesvh.cn/Article/details/gesbclfzf.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.fehbvm.com/Article/details/gvdqtdpxm.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.hesvh.cn/Article/details/gtmftsdzb.sHtML

Java: list.size();  map.size();  s.length()
来源：http://baike.zdbjq.cn/Article/details/ggfeuyqrz.sHtML

Go:   len(arr);  len(m)
来源：http://www.share.fehbvm.com/Article/details/gvzcrxddw.sHtML

Ruby: x.length;  x.size
来源：http://wap.fehbvm.com/Article/details/guxoqhnvj.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://m.share.hesvh.cn/Article/details/gxnxkhzus.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.m.share.fehbvm.com/Article/details/gzqcbapmm.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://blog.hesvh.cn/Article/details/gapnpcrqz.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.share.zdbjq.cn/Article/details/gwcgbazan.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://blog.fehbvm.com/Article/details/gsfvcpqux.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://wap.fehbvm.com/Article/details/gukuzzqts.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://wap.zdbjq.cn/Article/details/gskuotwdg.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://read.share.hesvh.cn/Article/details/gzoweuxah.sHtML

Ruby: a == b
来源：http://read.share.zdbjq.cn/Article/details/gjddknkrf.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://wap.hesvh.cn/Article/details/goyiimvtz.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://wap.fehbvm.com/Article/details/gjuymnqgz.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.m.share.zdbjq.cn/Article/details/gjbcicjtg.sHtML

PHP:  if (empty($x)) {}
来源：http://www.share.zdbjq.cn/Article/details/ghpinkfhj.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://blog.fehbvm.com/Article/details/gezixvlxa.sHtML

TS:   if (x == null) {}
来源：http://m.share.fehbvm.com/Article/details/gpjwvbkwk.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://blog.fehbvm.com/Article/details/giufudpta.sHtML

Go:   if x == nil {}
来源：http://www.m.share.zdbjq.cn/Article/details/gjitjxbjv.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://blog.zdbjq.cn/Article/details/gxeodegja.sHtML

C#:   if (x is null) {}
来源：http://m.share.fehbvm.com/Article/details/ggxwoydgy.sHtML

[P07] 防抖与节流
来源：http://blog.hesvh.cn/Article/details/gehefudff.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://3g.zdbjq.cn/Article/details/gixwcycrv.sHtML

PHP:  // 手写时间戳比较
来源：http://mobile.fehbvm.com/Article/details/gicyravdi.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.zdbjq.cn/Article/details/gmngjxljo.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.hesvh.cn/Article/details/gyhhcvrnc.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://wap.hesvh.cn/Article/details/gmkvczzmo.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://wap.zdbjq.cn/Article/details/goenfkqpd.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://3g.fehbvm.com/Article/details/gagksjwji.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://mobile.zdbjq.cn/Article/details/grhagzflv.sHtML

[P08] 处理浮点精度问题
来源：http://www.share.hesvh.cn/Article/details/ggkbccyta.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://wap.zdbjq.cn/Article/details/gnxhtddcy.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://3g.hesvh.cn/Article/details/gvattcfcz.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.m.share.fehbvm.com/Article/details/gtjqapyvi.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://3g.hesvh.cn/Article/details/ggkclfwap.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://read.share.fehbvm.com/Article/details/gtircirbs.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://read.share.zdbjq.cn/Article/details/gkkprqfoa.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://blog.fehbvm.com/Article/details/ghkrvdsko.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://baike.zdbjq.cn/Article/details/gnorxeitw.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gbzqzenin.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://baike.fehbvm.com/Article/details/ghrpzswey.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gwayqwxqj.sHtML

[Q01] 创建表
来源：http://read.share.fehbvm.com/Article/details/gyutigmlb.sHtML

CREATE TABLE users (
来源：http://www.m.share.fehbvm.com/Article/details/gahkcflmt.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.hesvh.cn/Article/details/gftmyyubv.sHtML

name VARCHAR(50) NOT NULL,
来源：http://wap.hesvh.cn/Article/details/gnccaaqbo.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.blog.zdbjq.cn/Article/details/gcnhmbahz.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://3g.fehbvm.com/Article/details/gdguxtlsu.sHtML

);
来源：http://www.blog.hesvh.cn/Article/details/gnqexzqqd.sHtML

[Q02] 创建带外键的表
来源：http://blog.fehbvm.com/Article/details/gconuetwt.sHtML

CREATE TABLE orders (
来源：http://mobile.fehbvm.com/Article/details/gpftrepcq.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.zdbjq.cn/Article/details/gjlfsckio.sHtML

user_id INT NOT NULL,
来源：http://mobile.hesvh.cn/Article/details/gzuyckvpq.sHtML

amount DECIMAL(10, 2),
来源：http://mobile.hesvh.cn/Article/details/gqcfigska.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.m.share.zdbjq.cn/Article/details/grdspncvp.sHtML

);
来源：http://read.share.fehbvm.com/Article/details/gwqkrymgb.sHtML

[Q03] 增加列
来源：http://www.blog.fehbvm.com/Article/details/gzwcthsrp.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://m.share.zdbjq.cn/Article/details/gwhgxzyqc.sHtML

[Q04] 修改列类型
来源：http://wap.hesvh.cn/Article/details/gxpsplpam.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.m.share.hesvh.cn/Article/details/gcxatbrru.sHtML

[Q05] 重命名列
来源：http://3g.zdbjq.cn/Article/details/ggapyxqqw.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://3g.fehbvm.com/Article/details/gbzbqotqh.sHtML

[Q06] 删除列
来源：http://www.blog.fehbvm.com/Article/details/gepmkwhjt.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://m.share.zdbjq.cn/Article/details/gsqinkzms.sHtML

[Q07] 删除表
来源：http://www.share.hesvh.cn/Article/details/guqgjeiwl.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.m.share.fehbvm.com/Article/details/gnmysttue.sHtML

[Q08] 创建普通索引
来源：http://read.share.zdbjq.cn/Article/details/gijzgvaax.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://blog.hesvh.cn/Article/details/ghrtxurpw.sHtML

[Q09] 创建唯一索引
来源：http://mobile.hesvh.cn/Article/details/glkmdlhgj.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.m.share.hesvh.cn/Article/details/giloimhqj.sHtML

[Q10] 插入单行
来源：http://www.m.share.zdbjq.cn/Article/details/ggojbramx.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://3g.zdbjq.cn/Article/details/gpongzetk.sHtML

[Q11] 一次插入多行
来源：http://www.share.zdbjq.cn/Article/details/gwipbkbez.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://m.share.fehbvm.com/Article/details/gvcxutvdo.sHtML

[Q12] 插入后取自增 ID
来源：http://blog.fehbvm.com/Article/details/gyqjvguks.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://read.share.hesvh.cn/Article/details/gkqtrsqwl.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://mobile.hesvh.cn/Article/details/gajqccesx.sHtML

[Q13] 忽略重复插入
来源：http://m.share.fehbvm.com/Article/details/grnhtiwkx.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://read.share.zdbjq.cn/Article/details/gwlzrwilu.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.blog.zdbjq.cn/Article/details/gfeutbciz.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://wap.fehbvm.com/Article/details/gmxxxuzea.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://baike.fehbvm.com/Article/details/gjnjvhbez.sHtML

[Q15] 查询全部
来源：http://3g.zdbjq.cn/Article/details/gsvaqovbk.sHtML

SELECT * FROM users;
来源：http://www.share.hesvh.cn/Article/details/ghaaapaum.sHtML

[Q16] 查询指定列
来源：http://read.share.fehbvm.com/Article/details/gcjsxtntn.sHtML

SELECT id, name FROM users;
来源：http://wap.fehbvm.com/Article/details/gnpjsztfh.sHtML

[Q17] 条件查询
来源：http://m.share.fehbvm.com/Article/details/gaysirszx.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://read.share.fehbvm.com/Article/details/ghujghuul.sHtML

[Q18] 模糊匹配
来源：http://www.share.zdbjq.cn/Article/details/gvejxwhls.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://wap.fehbvm.com/Article/details/geurihslh.sHtML

[Q19] 范围查询
来源：http://www.share.hesvh.cn/Article/details/ghyfzwxzw.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://read.share.hesvh.cn/Article/details/gehdsseak.sHtML

[Q20] IN 列表
来源：http://m.share.hesvh.cn/Article/details/gbqefsgwi.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.m.share.hesvh.cn/Article/details/gkpuqbsiy.sHtML

[Q21] 空值判断
来源：http://read.share.zdbjq.cn/Article/details/gbxvmbzyn.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.share.hesvh.cn/Article/details/gkmkfmebg.sHtML

[Q22] 排序
来源：http://3g.fehbvm.com/Article/details/gcuypxcdc.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://read.share.fehbvm.com/Article/details/gxbxszhqv.sHtML

[Q23] 分页
来源：http://www.m.share.zdbjq.cn/Article/details/giclvqeyi.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.m.share.hesvh.cn/Article/details/ghecwselq.sHtML

[Q24] 去重
来源：http://www.blog.zdbjq.cn/Article/details/gcwfvwsed.sHtML

SELECT DISTINCT city FROM users;
来源：http://wap.fehbvm.com/Article/details/gnnvkuams.sHtML

[Q25] 只取前 N 条
来源：http://blog.zdbjq.cn/Article/details/gkftqoyvm.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://wap.hesvh.cn/Article/details/gzvtetwlo.sHtML

[Q26] 计数
来源：http://mobile.zdbjq.cn/Article/details/gszsuyrsb.sHtML

SELECT COUNT(*) FROM users;
来源：http://mobile.zdbjq.cn/Article/details/ggxyutxzj.sHtML

[Q27] 条件计数
来源：http://www.blog.hesvh.cn/Article/details/ghmigkxfu.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://3g.zdbjq.cn/Article/details/gcooziwde.sHtML

[Q28] 求和与平均
来源：http://wap.zdbjq.cn/Article/details/gpfjsopaa.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://m.share.zdbjq.cn/Article/details/ggjctxwqe.sHtML

[Q29] 最大最小值
来源：http://baike.hesvh.cn/Article/details/ggnjcdmmq.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/goyxuuvet.sHtML

[Q30] 分组统计
来源：http://blog.hesvh.cn/Article/details/glzmboxvm.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.blog.fehbvm.com/Article/details/gbfcpbxnd.sHtML

[Q31] 分组后过滤
来源：http://blog.fehbvm.com/Article/details/gqxyjeoyv.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://baike.zdbjq.cn/Article/details/gjjaqjylp.sHtML

[Q32] 分组拼接字符串
来源：http://www.blog.zdbjq.cn/Article/details/gofmxrave.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://blog.hesvh.cn/Article/details/gqgwtorae.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://blog.fehbvm.com/Article/details/gvgcdmdwl.sHtML

[Q33] 多列分组
来源：http://www.m.share.fehbvm.com/Article/details/gobslwzqq.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.m.share.hesvh.cn/Article/details/gnfbjxfay.sHtML

[Q34] 每组取第一条
来源：http://blog.fehbvm.com/Article/details/gqklxngli.sHtML

SELECT * FROM (
来源：http://baike.zdbjq.cn/Article/details/glogjeeqp.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://m.share.zdbjq.cn/Article/details/gmlcfajod.sHtML

) t WHERE rn = 1;
来源：http://3g.fehbvm.com/Article/details/gonhxnxty.sHtML

[Q35] 内连接
来源：http://www.m.share.hesvh.cn/Article/details/geehmbzyj.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.share.hesvh.cn/Article/details/gsvykwlru.sHtML

[Q36] 左连接
来源：http://mobile.hesvh.cn/Article/details/gunvjoqur.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.share.zdbjq.cn/Article/details/gubzrrwiq.sHtML

[Q37] 右连接
来源：http://wap.hesvh.cn/Article/details/gbuytdjib.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://blog.fehbvm.com/Article/details/gmuaaticj.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://baike.zdbjq.cn/Article/details/ggehrnvqh.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.share.hesvh.cn/Article/details/gexyznhzo.sHtML

[Q39] 自连接（查上下级）
来源：http://www.m.share.zdbjq.cn/Article/details/gvbdnyxrl.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.blog.zdbjq.cn/Article/details/gyqpuebwn.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://blog.hesvh.cn/Article/details/ghfaifuiy.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.m.share.hesvh.cn/Article/details/gueogiadf.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.blog.hesvh.cn/Article/details/gtlausksb.sHtML

[Q41] 多表连接
来源：http://read.share.zdbjq.cn/Article/details/gsgnrhuvn.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://wap.fehbvm.com/Article/details/gsrunetnj.sHtML

JOIN users u ON u.id = o.user_id
来源：http://m.share.zdbjq.cn/Article/details/gkeawmszw.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://baike.hesvh.cn/Article/details/gwhkblcwc.sHtML

[Q42] 连接条件附加过滤
来源：http://3g.zdbjq.cn/Article/details/gexjwqvai.sHtML

SELECT u.name, o.amount FROM users u
来源：http://mobile.fehbvm.com/Article/details/gjxtgpbpl.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://mobile.fehbvm.com/Article/details/gsuyrugub.sHtML

[Q43] 标量子查询
来源：http://read.share.fehbvm.com/Article/details/gzjjpdkxz.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://mobile.hesvh.cn/Article/details/gjyivgonu.sHtML

[Q44] IN 子查询
来源：http://www.share.zdbjq.cn/Article/details/gvpngwesw.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://mobile.fehbvm.com/Article/details/gngkwhulu.sHtML

[Q45] EXISTS 判断存在
来源：http://mobile.fehbvm.com/Article/details/ghkwiwddm.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.hesvh.cn/Article/details/gufikgnfp.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://3g.zdbjq.cn/Article/details/ghzuvguvd.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.fehbvm.com/Article/details/gyjtpdfaj.sHtML

[Q47] 与平均值比较
来源：http://www.blog.hesvh.cn/Article/details/gcnqddtjt.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://mobile.zdbjq.cn/Article/details/gwostawmg.sHtML

[Q48] CTE 公用表表达式
来源：http://m.share.hesvh.cn/Article/details/gpzbhgskf.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://3g.fehbvm.com/Article/details/gbifefunm.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.share.zdbjq.cn/Article/details/grtcymnqj.sHtML

[Q49] 更新单行
来源：http://mobile.fehbvm.com/Article/details/gyifbntru.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.blog.zdbjq.cn/Article/details/gmrhengit.sHtML

[Q50] 批量更新
来源：http://blog.fehbvm.com/Article/details/gngiarwqs.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://m.share.zdbjq.cn/Article/details/glrsjviuy.sHtML

[Q51] 用子查询更新
来源：http://www.m.share.zdbjq.cn/Article/details/gdhrdtcgm.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://m.share.fehbvm.com/Article/details/glxuhuour.sHtML

[Q52] 删除指定行
来源：http://read.share.fehbvm.com/Article/details/gvfdgyakm.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.blog.hesvh.cn/Article/details/ggfflhjll.sHtML

[Q53] 按条件删除
来源：http://www.m.share.hesvh.cn/Article/details/grkupnrbf.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.blog.zdbjq.cn/Article/details/gteimsars.sHtML

[Q54] 清空表
来源：http://m.share.hesvh.cn/Article/details/gsxyombkt.sHtML

TRUNCATE TABLE logs;
来源：http://mobile.hesvh.cn/Article/details/gfzjesryz.sHtML

[Q55] 排名（并列占位）
来源：http://baike.hesvh.cn/Article/details/gloqubvcy.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.share.fehbvm.com/Article/details/gbywaqrqf.sHtML

[Q56] 密集排名（并列不占位）
来源：http://3g.zdbjq.cn/Article/details/gluwfbvcb.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://mobile.hesvh.cn/Article/details/gypshxuma.sHtML

[Q57] 行号
来源：http://baike.zdbjq.cn/Article/details/glseepkxl.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://3g.fehbvm.com/Article/details/gtvmshvvd.sHtML

[Q58] 累计求和
来源：http://wap.hesvh.cn/Article/details/gfyvaduyq.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://blog.zdbjq.cn/Article/details/gcseapkdt.sHtML

[Q59] 分组内累计
来源：http://3g.fehbvm.com/Article/details/gorowonah.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.share.fehbvm.com/Article/details/gmmywqagg.sHtML

[Q60] 取上一行 / 下一行
来源：http://mobile.hesvh.cn/Article/details/gfgohncbh.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://blog.fehbvm.com/Article/details/gwznmxbvc.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://blog.zdbjq.cn/Article/details/gklhnpegc.sHtML

[Q61] 移动平均
来源：http://wap.hesvh.cn/Article/details/gwtjyeoyx.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://wap.fehbvm.com/Article/details/gcfnrhvjx.sHtML

[Q62] 分组占比
来源：http://mobile.fehbvm.com/Article/details/gwghxhalv.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://baike.fehbvm.com/Article/details/glbznvxtt.sHtML

[Q63] 开启事务
来源：http://mobile.fehbvm.com/Article/details/gwrvkzxjm.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://m.share.zdbjq.cn/Article/details/gnvbqrtku.sHtML

[Q64] 提交事务
来源：http://blog.fehbvm.com/Article/details/gxhucwwqd.sHtML

COMMIT;
来源：http://3g.zdbjq.cn/Article/details/gisrrrtlw.sHtML

[Q65] 回滚事务
来源：http://www.share.fehbvm.com/Article/details/gkcrglipy.sHtML

ROLLBACK;
来源：http://www.share.fehbvm.com/Article/details/gcbrcrjsk.sHtML

[Q66] 行锁查询
来源：http://blog.fehbvm.com/Article/details/gbjyadjtu.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://m.share.hesvh.cn/Article/details/gagwpwwyy.sHtML

[Q67] 设置隔离级别
来源：http://www.share.fehbvm.com/Article/details/guiofssxh.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://mobile.zdbjq.cn/Article/details/gwjhxdatb.sHtML

[Q68] 保存点
来源：http://baike.zdbjq.cn/Article/details/gdmqlikwv.sHtML

SAVEPOINT sp1;
来源：http://read.share.zdbjq.cn/Article/details/gfiitcsss.sHtML

ROLLBACK TO sp1;
来源：http://blog.zdbjq.cn/Article/details/gjygesfkv.sHtML

[Q69] 查看执行计划
来源：http://baike.hesvh.cn/Article/details/gwplkqtsk.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.blog.hesvh.cn/Article/details/gqredcvpz.sHtML

[Q70] 更新统计信息
来源：http://wap.zdbjq.cn/Article/details/gjcjbmfqx.sHtML

ANALYZE TABLE users;
来源：http://wap.hesvh.cn/Article/details/gvmmwevah.sHtML

[Q71] 查看建表语句
来源：http://blog.zdbjq.cn/Article/details/gzlmuglxl.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://read.share.hesvh.cn/Article/details/gstdmnzuv.sHtML

[Q72] 查看索引
来源：http://www.m.share.hesvh.cn/Article/details/gmjgylsbl.sHtML

SHOW INDEX FROM users;
来源：http://read.share.fehbvm.com/Article/details/gckuetgtx.sHtML

[Q73] 查看表状态
来源：http://www.share.hesvh.cn/Article/details/gftuoabug.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://baike.fehbvm.com/Article/details/gidkgbvaz.sHtML

[Q74] 强制使用索引
来源：http://read.share.fehbvm.com/Article/details/gyidhaczf.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://mobile.fehbvm.com/Article/details/gesbmejnl.sHtML

[Q75] 日期格式化
来源：http://www.blog.hesvh.cn/Article/details/gjrbydteh.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.m.share.hesvh.cn/Article/details/gussjlilk.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://wap.fehbvm.com/Article/details/gxebdtbmr.sHtML

[Q76] 按天统计
来源：http://read.share.fehbvm.com/Article/details/glyhprtci.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.m.share.fehbvm.com/Article/details/ghshazpcd.sHtML

[Q77] 时间加减
来源：http://wap.hesvh.cn/Article/details/gkdzizzcu.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://wap.hesvh.cn/Article/details/gvofprfkk.sHtML

[Q78] 当前时间
来源：http://www.blog.fehbvm.com/Article/details/gpmovviba.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://3g.zdbjq.cn/Article/details/gfqnuxpmk.sHtML

[Q79] 字符串拼接
来源：http://m.share.fehbvm.com/Article/details/ganhiyyvw.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://m.share.zdbjq.cn/Article/details/ggjrziaxt.sHtML

[Q80] 字符串截取
来源：http://m.share.hesvh.cn/Article/details/gtumiwvfa.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://3g.fehbvm.com/Article/details/gzgsbyvbo.sHtML

[Q81] 字符串替换
来源：http://www.share.zdbjq.cn/Article/details/ggmcwjsdf.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://baike.hesvh.cn/Article/details/gevwxnhga.sHtML

[Q82] 字符长度与字节长度
来源：http://www.share.fehbvm.com/Article/details/gnqnuxwzw.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://mobile.hesvh.cn/Article/details/gvhbmebbv.sHtML

[Q83] 大小写转换
来源：http://mobile.fehbvm.com/Article/details/gbvseaomp.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gwcitrhxu.sHtML

[Q84] 去除首尾空格
来源：http://blog.fehbvm.com/Article/details/gaqjhsomu.sHtML

SELECT TRIM(name) FROM users;
来源：http://read.share.hesvh.cn/Article/details/gpodihhhz.sHtML

[Q85] 数值取整
来源：http://m.share.zdbjq.cn/Article/details/gozarwlkp.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://mobile.zdbjq.cn/Article/details/gwulzxwzg.sHtML

[Q86] 读取 JSON 字段
来源：http://www.m.share.fehbvm.com/Article/details/gispejcjb.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://baike.zdbjq.cn/Article/details/gylqlakve.sHtML

[Q87] JSON 字段做条件
来源：http://www.m.share.hesvh.cn/Article/details/gbpccrnfy.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://baike.hesvh.cn/Article/details/gwelxyync.sHtML

[Q88] 行转列（条件聚合）
来源：http://wap.zdbjq.cn/Article/details/gtztsjplo.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.blog.hesvh.cn/Article/details/gailkoryx.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://wap.zdbjq.cn/Article/details/gaorxsspv.sHtML

[Q89] 判断表是否存在
来源：http://blog.zdbjq.cn/Article/details/gxocuuzni.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://3g.fehbvm.com/Article/details/glyzcwstq.sHtML

[Q90] 生成序号列
来源：http://wap.fehbvm.com/Article/details/gtfydoiuu.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.share.hesvh.cn/Article/details/gyhwxsywz.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gmpttdqof.sHtML

R. Bash 专题
来源：http://wap.hesvh.cn/Article/details/gbtkzpdhm.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gjelfshee.sHtML

[R01] shebang 与严格模式
来源：http://read.share.hesvh.cn/Article/details/gmxopyhkk.sHtML

#!/usr/bin/env bash
来源：http://mobile.zdbjq.cn/Article/details/gathiwxgy.sHtML

set -euo pipefail
来源：http://www.m.share.fehbvm.com/Article/details/gmquzrbbg.sHtML

[R02] 变量赋值与使用
来源：http://www.blog.zdbjq.cn/Article/details/gobwpdfug.sHtML

name="Tom"; echo "$name"
来源：http://mobile.zdbjq.cn/Article/details/grabvlgir.sHtML

[R03] 只读变量
来源：http://mobile.zdbjq.cn/Article/details/gxjoqswkv.sHtML

readonly PI=3.14
来源：http://www.share.hesvh.cn/Article/details/gymkwuhdm.sHtML

[R04] 位置参数
来源：http://m.share.zdbjq.cn/Article/details/gmdtwywvm.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://m.share.fehbvm.com/Article/details/gtbeghpqo.sHtML

[R05] 参数默认值
来源：http://read.share.fehbvm.com/Article/details/gkhsycoeu.sHtML

name="${1:-default}"
来源：http://3g.fehbvm.com/Article/details/gpgywhsdp.sHtML

[R06] 判断命令是否存在
来源：http://www.blog.hesvh.cn/Article/details/gcfbweyzg.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://m.share.fehbvm.com/Article/details/gkobzeoka.sHtML

[R07] if 判断文件
来源：http://www.share.fehbvm.com/Article/details/gjbinfcvj.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://wap.fehbvm.com/Article/details/gkbnkkmrs.sHtML

[R08] 数值比较
来源：http://wap.fehbvm.com/Article/details/gocsywchq.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://read.share.hesvh.cn/Article/details/gpvoibkya.sHtML

[R09] 字符串比较
来源：http://mobile.hesvh.cn/Article/details/guwhwmhla.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://m.share.zdbjq.cn/Article/details/govjfsgxu.sHtML

[R10] 正则匹配
来源：http://blog.hesvh.cn/Article/details/gimhxyjsr.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.blog.zdbjq.cn/Article/details/gfjfdlhvl.sHtML

[R11] case 多分支
来源：http://read.share.zdbjq.cn/Article/details/gizxlflqv.sHtML

case "$1" in
来源：http://wap.fehbvm.com/Article/details/gbcaeboxs.sHtML

start) echo "启动" ;;
来源：http://www.m.share.fehbvm.com/Article/details/gkpkkburf.sHtML

stop)  echo "停止" ;;
来源：http://baike.hesvh.cn/Article/details/gfktlzmwt.sHtML

*)     echo "未知命令" ;;
来源：http://m.share.hesvh.cn/Article/details/gkghpbbut.sHtML

esac
来源：http://www.blog.zdbjq.cn/Article/details/gequuxzzx.sHtML

[R12] for 遍历文件
来源：http://blog.fehbvm.com/Article/details/grbzzdmrd.sHtML

for f in *.txt; do echo "$f"; done
来源：http://3g.zdbjq.cn/Article/details/gslvbqfkp.sHtML

[R13] for 计数循环
来源：http://wap.fehbvm.com/Article/details/gdtjrbfco.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.blog.zdbjq.cn/Article/details/gasbzfetd.sHtML

[R14] C 风格 for
来源：http://read.share.zdbjq.cn/Article/details/gjrlslstb.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.blog.fehbvm.com/Article/details/gfztuduzj.sHtML

[R15] while 逐行读文件
来源：http://baike.zdbjq.cn/Article/details/gvnaxrgsq.sHtML


<!-- 参考信息 -->