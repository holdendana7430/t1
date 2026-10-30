代发 wailian999

Ruby: Digest::SHA256.hexdigest(s)
来源：http://3g.zdbjq.cn/Article/details/ggapvnxcs.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.blog.fehbvm.com/Article/details/gqhbzidra.sHtML

[P03] 生成短随机字符串
来源：http://baike.zdbjq.cn/Article/details/gadcaqngd.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://baike.hesvh.cn/Article/details/gykiecojw.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://mobile.fehbvm.com/Article/details/gliviedae.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.zdbjq.cn/Article/details/gittbxfpu.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.zdbjq.cn/Article/details/gmgyvtulq.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://wap.fehbvm.com/Article/details/gctourwsz.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://mobile.hesvh.cn/Article/details/goiicxijy.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://m.share.zdbjq.cn/Article/details/gahsijfkh.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.m.share.fehbvm.com/Article/details/gfhcvaybd.sHtML

[P04] 求长度
来源：http://www.blog.hesvh.cn/Article/details/ghagoavgy.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://read.share.hesvh.cn/Article/details/goyfkggya.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.zdbjq.cn/Article/details/gguxroovi.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.fehbvm.com/Article/details/gyasaesec.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.fehbvm.com/Article/details/gxyocwspi.sHtML

Java: list.size();  map.size();  s.length()
来源：http://blog.hesvh.cn/Article/details/gtevdfbmu.sHtML

Go:   len(arr);  len(m)
来源：http://blog.hesvh.cn/Article/details/gfmmxmiwb.sHtML

Ruby: x.length;  x.size
来源：http://www.m.share.fehbvm.com/Article/details/gnoaaczme.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.blog.hesvh.cn/Article/details/ginssbtlh.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.blog.zdbjq.cn/Article/details/gxzrnsdwf.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.share.zdbjq.cn/Article/details/gixilpvfa.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://wap.fehbvm.com/Article/details/gjsjzdurj.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://3g.fehbvm.com/Article/details/gpfrwhelz.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.blog.fehbvm.com/Article/details/grjveleqe.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://m.share.zdbjq.cn/Article/details/glvtlqcmg.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://wap.zdbjq.cn/Article/details/gzapgitur.sHtML

Ruby: a == b
来源：http://www.blog.fehbvm.com/Article/details/gtucsvvez.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://read.share.hesvh.cn/Article/details/gqwfsxcvz.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.blog.fehbvm.com/Article/details/gissqgoiv.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://mobile.fehbvm.com/Article/details/gzfsgqhyg.sHtML

PHP:  if (empty($x)) {}
来源：http://mobile.zdbjq.cn/Article/details/gyplrxfub.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://m.share.fehbvm.com/Article/details/geeammqkh.sHtML

TS:   if (x == null) {}
来源：http://wap.hesvh.cn/Article/details/gnswdqcyu.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://wap.fehbvm.com/Article/details/gtwpsbiqs.sHtML

Go:   if x == nil {}
来源：http://mobile.hesvh.cn/Article/details/gaebonkjb.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://blog.hesvh.cn/Article/details/gxkhwknej.sHtML

C#:   if (x is null) {}
来源：http://www.blog.hesvh.cn/Article/details/grohiqanx.sHtML

[P07] 防抖与节流
来源：http://m.share.zdbjq.cn/Article/details/gffywzoax.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://baike.zdbjq.cn/Article/details/ggbqyursj.sHtML

PHP:  // 手写时间戳比较
来源：http://wap.hesvh.cn/Article/details/gsoepvadf.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.zdbjq.cn/Article/details/gagzskdvl.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.fehbvm.com/Article/details/gomrkqylp.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://3g.fehbvm.com/Article/details/gqiakholl.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://3g.hesvh.cn/Article/details/geppngnhm.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://baike.zdbjq.cn/Article/details/gzxfawtpe.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.share.fehbvm.com/Article/details/gxtnoifws.sHtML

[P08] 处理浮点精度问题
来源：http://m.share.hesvh.cn/Article/details/glmsajjce.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://mobile.zdbjq.cn/Article/details/gfcnhbevc.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://blog.fehbvm.com/Article/details/gzffccivy.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://wap.zdbjq.cn/Article/details/gwgjbjuap.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://baike.fehbvm.com/Article/details/gvcgacspk.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://mobile.zdbjq.cn/Article/details/gqliquras.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://wap.fehbvm.com/Article/details/gmxjuvziq.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://blog.fehbvm.com/Article/details/gpcxepdnu.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://mobile.fehbvm.com/Article/details/giyybymeu.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/galoylgpe.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://baike.zdbjq.cn/Article/details/gniqnuffk.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gvxbyggzc.sHtML

[Q01] 创建表
来源：http://www.blog.zdbjq.cn/Article/details/gesdgpfsm.sHtML

CREATE TABLE users (
来源：http://mobile.zdbjq.cn/Article/details/glvxjfzsy.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.zdbjq.cn/Article/details/goblobvde.sHtML

name VARCHAR(50) NOT NULL,
来源：http://baike.hesvh.cn/Article/details/gxgxuzipx.sHtML

email VARCHAR(100) UNIQUE,
来源：http://read.share.fehbvm.com/Article/details/gpzadaysj.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://m.share.fehbvm.com/Article/details/gqmhcaktp.sHtML

);
来源：http://read.share.zdbjq.cn/Article/details/gpbxjnypf.sHtML

[Q02] 创建带外键的表
来源：http://wap.hesvh.cn/Article/details/gownsryxq.sHtML

CREATE TABLE orders (
来源：http://wap.fehbvm.com/Article/details/gxhvsbiil.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.hesvh.cn/Article/details/glwaqwlor.sHtML

user_id INT NOT NULL,
来源：http://wap.zdbjq.cn/Article/details/gjfdjlxiv.sHtML

amount DECIMAL(10, 2),
来源：http://www.m.share.hesvh.cn/Article/details/gahxfiqrv.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.m.share.zdbjq.cn/Article/details/gnffcnltq.sHtML

);
来源：http://mobile.fehbvm.com/Article/details/gfwfjrtxw.sHtML

[Q03] 增加列
来源：http://www.blog.zdbjq.cn/Article/details/ghmapgrfw.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://3g.fehbvm.com/Article/details/gwrodxupr.sHtML

[Q04] 修改列类型
来源：http://wap.hesvh.cn/Article/details/giwzggizm.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.m.share.zdbjq.cn/Article/details/gxhrvpcsb.sHtML

[Q05] 重命名列
来源：http://www.blog.zdbjq.cn/Article/details/gqefnkwth.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.m.share.fehbvm.com/Article/details/gihwdhieo.sHtML

[Q06] 删除列
来源：http://read.share.fehbvm.com/Article/details/gvqjrydpj.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.blog.hesvh.cn/Article/details/ggyvqzpgv.sHtML

[Q07] 删除表
来源：http://www.blog.zdbjq.cn/Article/details/gyzhisgke.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.share.fehbvm.com/Article/details/gcfcpzvjv.sHtML

[Q08] 创建普通索引
来源：http://www.blog.hesvh.cn/Article/details/ghxecosot.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.blog.fehbvm.com/Article/details/grguqkoqf.sHtML

[Q09] 创建唯一索引
来源：http://wap.fehbvm.com/Article/details/gxjzwrxky.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://baike.fehbvm.com/Article/details/ghellwtmc.sHtML

[Q10] 插入单行
来源：http://www.blog.hesvh.cn/Article/details/guaqlwgfb.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.share.zdbjq.cn/Article/details/gbuoowqny.sHtML

[Q11] 一次插入多行
来源：http://3g.hesvh.cn/Article/details/gbqospswe.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.blog.zdbjq.cn/Article/details/gvzbgqiqf.sHtML

[Q12] 插入后取自增 ID
来源：http://www.share.hesvh.cn/Article/details/genqqjyxh.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://3g.zdbjq.cn/Article/details/gfelabmkk.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.blog.fehbvm.com/Article/details/gkgfqrfcl.sHtML

[Q13] 忽略重复插入
来源：http://m.share.zdbjq.cn/Article/details/ggxvidkxl.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://mobile.fehbvm.com/Article/details/goexgtgly.sHtML

[Q14] 存在则更新（upsert）
来源：http://wap.zdbjq.cn/Article/details/grsdzbtkr.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://baike.fehbvm.com/Article/details/gwqosfbtn.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://m.share.hesvh.cn/Article/details/gafbujxvd.sHtML

[Q15] 查询全部
来源：http://blog.hesvh.cn/Article/details/ggjtcjvtz.sHtML

SELECT * FROM users;
来源：http://read.share.hesvh.cn/Article/details/gsorqzczb.sHtML

[Q16] 查询指定列
来源：http://www.m.share.hesvh.cn/Article/details/gypdohjwc.sHtML

SELECT id, name FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gnjbijsux.sHtML

[Q17] 条件查询
来源：http://m.share.zdbjq.cn/Article/details/gaiwcajat.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://mobile.fehbvm.com/Article/details/gckyemsbn.sHtML

[Q18] 模糊匹配
来源：http://m.share.zdbjq.cn/Article/details/gjdtwklvz.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.m.share.zdbjq.cn/Article/details/ghjrcoyjq.sHtML

[Q19] 范围查询
来源：http://wap.fehbvm.com/Article/details/gxrnkqgkb.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.share.zdbjq.cn/Article/details/gxsavlmog.sHtML

[Q20] IN 列表
来源：http://baike.fehbvm.com/Article/details/gogmjndns.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://baike.zdbjq.cn/Article/details/gykqqitqf.sHtML

[Q21] 空值判断
来源：http://www.share.zdbjq.cn/Article/details/gmglwbtbq.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://read.share.fehbvm.com/Article/details/getzubzby.sHtML

[Q22] 排序
来源：http://www.share.hesvh.cn/Article/details/gxvawjfll.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://mobile.fehbvm.com/Article/details/ghwqjuorh.sHtML

[Q23] 分页
来源：http://www.blog.zdbjq.cn/Article/details/gikrtmhxe.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://read.share.fehbvm.com/Article/details/gwbkvbowd.sHtML

[Q24] 去重
来源：http://www.m.share.fehbvm.com/Article/details/gryswmkdb.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gaicdgbsa.sHtML

[Q25] 只取前 N 条
来源：http://www.blog.hesvh.cn/Article/details/gyehywpcg.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://read.share.hesvh.cn/Article/details/gzrltyxzl.sHtML

[Q26] 计数
来源：http://blog.zdbjq.cn/Article/details/gywgbobwm.sHtML

SELECT COUNT(*) FROM users;
来源：http://3g.hesvh.cn/Article/details/gzwfslufa.sHtML

[Q27] 条件计数
来源：http://m.share.fehbvm.com/Article/details/gcpqdicfn.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://m.share.hesvh.cn/Article/details/gylamwmna.sHtML

[Q28] 求和与平均
来源：http://3g.zdbjq.cn/Article/details/ggrfoydbw.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.m.share.hesvh.cn/Article/details/gfalrokxw.sHtML

[Q29] 最大最小值
来源：http://www.m.share.hesvh.cn/Article/details/gbghtntli.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://wap.zdbjq.cn/Article/details/gxleadgoz.sHtML

[Q30] 分组统计
来源：http://wap.zdbjq.cn/Article/details/grhcstgfk.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://wap.zdbjq.cn/Article/details/gnnaonqin.sHtML

[Q31] 分组后过滤
来源：http://m.share.fehbvm.com/Article/details/gqlfyepan.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://wap.hesvh.cn/Article/details/gmkspinon.sHtML

[Q32] 分组拼接字符串
来源：http://3g.zdbjq.cn/Article/details/gawzihbxh.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.m.share.zdbjq.cn/Article/details/glbojztui.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://baike.zdbjq.cn/Article/details/gshgaauzk.sHtML

[Q33] 多列分组
来源：http://wap.zdbjq.cn/Article/details/grzfrodnu.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://read.share.fehbvm.com/Article/details/gloybdipe.sHtML

[Q34] 每组取第一条
来源：http://www.blog.hesvh.cn/Article/details/ghwmnvqjp.sHtML

SELECT * FROM (
来源：http://www.blog.hesvh.cn/Article/details/gbyaanqly.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://baike.zdbjq.cn/Article/details/gllakwjsw.sHtML

) t WHERE rn = 1;
来源：http://read.share.hesvh.cn/Article/details/gfefsfzyj.sHtML

[Q35] 内连接
来源：http://www.blog.fehbvm.com/Article/details/gadlgmnmr.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.share.fehbvm.com/Article/details/ggadpdrfc.sHtML

[Q36] 左连接
来源：http://blog.fehbvm.com/Article/details/ggpdbaifn.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://3g.fehbvm.com/Article/details/gkcyykxvi.sHtML

[Q37] 右连接
来源：http://blog.fehbvm.com/Article/details/gxsbeaare.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.blog.fehbvm.com/Article/details/gfeatdvwk.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://wap.fehbvm.com/Article/details/grmdrbqzk.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://blog.fehbvm.com/Article/details/gqfxusjco.sHtML

[Q39] 自连接（查上下级）
来源：http://blog.hesvh.cn/Article/details/golikvhpa.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.blog.zdbjq.cn/Article/details/gebuppwbw.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.m.share.zdbjq.cn/Article/details/givccvymu.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://read.share.hesvh.cn/Article/details/gdkxjicxv.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://m.share.hesvh.cn/Article/details/glbhdcrbx.sHtML

[Q41] 多表连接
来源：http://m.share.zdbjq.cn/Article/details/gsvzttirz.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://m.share.fehbvm.com/Article/details/gppjaxrjp.sHtML

JOIN users u ON u.id = o.user_id
来源：http://read.share.zdbjq.cn/Article/details/gfwuvoeux.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.share.zdbjq.cn/Article/details/grkfomycj.sHtML

[Q42] 连接条件附加过滤
来源：http://www.m.share.fehbvm.com/Article/details/gxoccecok.sHtML

SELECT u.name, o.amount FROM users u
来源：http://read.share.zdbjq.cn/Article/details/gdjsbldep.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.blog.zdbjq.cn/Article/details/gapwdonyh.sHtML

[Q43] 标量子查询
来源：http://www.blog.hesvh.cn/Article/details/gdwrxbumc.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.m.share.zdbjq.cn/Article/details/gxytcgbkb.sHtML

[Q44] IN 子查询
来源：http://mobile.fehbvm.com/Article/details/gbfctnrco.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://read.share.hesvh.cn/Article/details/gumzlzunf.sHtML

[Q45] EXISTS 判断存在
来源：http://blog.fehbvm.com/Article/details/gmuggfbqu.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.hesvh.cn/Article/details/gfdaswrua.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://mobile.hesvh.cn/Article/details/guvojempq.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.fehbvm.com/Article/details/gjjbxwath.sHtML

[Q47] 与平均值比较
来源：http://www.blog.hesvh.cn/Article/details/gzpbdtvcm.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.share.hesvh.cn/Article/details/gfhfffszz.sHtML

[Q48] CTE 公用表表达式
来源：http://www.m.share.zdbjq.cn/Article/details/gebzvvket.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://m.share.zdbjq.cn/Article/details/gmitmuxjd.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.share.zdbjq.cn/Article/details/gpxumzipg.sHtML

[Q49] 更新单行
来源：http://wap.hesvh.cn/Article/details/gkvzrniaa.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://m.share.hesvh.cn/Article/details/gimaidmch.sHtML

[Q50] 批量更新
来源：http://read.share.zdbjq.cn/Article/details/gjghnndaf.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://baike.zdbjq.cn/Article/details/gnxprbabo.sHtML

[Q51] 用子查询更新
来源：http://read.share.hesvh.cn/Article/details/gooiytycv.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://mobile.hesvh.cn/Article/details/gzivriujb.sHtML

[Q52] 删除指定行
来源：http://www.m.share.fehbvm.com/Article/details/ghhplrzkp.sHtML

DELETE FROM users WHERE id = 10;
来源：http://m.share.fehbvm.com/Article/details/gtkllgxeq.sHtML

[Q53] 按条件删除
来源：http://mobile.hesvh.cn/Article/details/gysyufvfz.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://3g.zdbjq.cn/Article/details/gjgidutbf.sHtML

[Q54] 清空表
来源：http://wap.zdbjq.cn/Article/details/gntocjcsv.sHtML

TRUNCATE TABLE logs;
来源：http://wap.zdbjq.cn/Article/details/guqfeugfk.sHtML

[Q55] 排名（并列占位）
来源：http://mobile.zdbjq.cn/Article/details/gbatgnsnl.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.blog.zdbjq.cn/Article/details/gkqtpedlz.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.share.fehbvm.com/Article/details/gavqtedwx.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://blog.zdbjq.cn/Article/details/ggoimnfxh.sHtML

[Q57] 行号
来源：http://mobile.hesvh.cn/Article/details/gwrplkgce.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gctpmhpfs.sHtML

[Q58] 累计求和
来源：http://www.m.share.fehbvm.com/Article/details/gozvdjcwr.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://blog.hesvh.cn/Article/details/gsztcymvj.sHtML

[Q59] 分组内累计
来源：http://blog.hesvh.cn/Article/details/gpnlixelf.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.blog.hesvh.cn/Article/details/goharmhyg.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.m.share.fehbvm.com/Article/details/gflttalhd.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://3g.fehbvm.com/Article/details/glkbmsnjl.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://mobile.hesvh.cn/Article/details/glwzcicvc.sHtML

[Q61] 移动平均
来源：http://wap.hesvh.cn/Article/details/gaysfekps.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://wap.fehbvm.com/Article/details/gssgpfdhm.sHtML

[Q62] 分组占比
来源：http://wap.hesvh.cn/Article/details/gmeiyrsxm.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://3g.zdbjq.cn/Article/details/gykoktqpv.sHtML

[Q63] 开启事务
来源：http://www.share.hesvh.cn/Article/details/gwwaluldt.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.share.fehbvm.com/Article/details/gpsynkqfh.sHtML

[Q64] 提交事务
来源：http://baike.fehbvm.com/Article/details/gdagoqqkl.sHtML

COMMIT;
来源：http://www.m.share.fehbvm.com/Article/details/gmyjqlsvg.sHtML

[Q65] 回滚事务
来源：http://blog.fehbvm.com/Article/details/gsymyjjhj.sHtML

ROLLBACK;
来源：http://www.m.share.fehbvm.com/Article/details/gldwdtfxa.sHtML

[Q66] 行锁查询
来源：http://m.share.fehbvm.com/Article/details/grckktvfj.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.blog.zdbjq.cn/Article/details/griwlmmnr.sHtML

[Q67] 设置隔离级别
来源：http://www.blog.hesvh.cn/Article/details/gbqscdqhv.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.blog.zdbjq.cn/Article/details/gegcogghz.sHtML

[Q68] 保存点
来源：http://www.blog.zdbjq.cn/Article/details/grybqnhpy.sHtML

SAVEPOINT sp1;
来源：http://wap.fehbvm.com/Article/details/gvyldaaxb.sHtML

ROLLBACK TO sp1;
来源：http://www.m.share.hesvh.cn/Article/details/gbsecrpde.sHtML

[Q69] 查看执行计划
来源：http://baike.zdbjq.cn/Article/details/ghsfipsub.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://baike.fehbvm.com/Article/details/gjdqcdadt.sHtML

[Q70] 更新统计信息
来源：http://3g.fehbvm.com/Article/details/gowbghxzb.sHtML

ANALYZE TABLE users;
来源：http://3g.fehbvm.com/Article/details/grfynxgmy.sHtML

[Q71] 查看建表语句
来源：http://3g.fehbvm.com/Article/details/gnurxuhed.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://mobile.hesvh.cn/Article/details/gprciqbnl.sHtML

[Q72] 查看索引
来源：http://blog.hesvh.cn/Article/details/gowbbpqan.sHtML

SHOW INDEX FROM users;
来源：http://wap.hesvh.cn/Article/details/gebbuzfnq.sHtML

[Q73] 查看表状态
来源：http://www.share.hesvh.cn/Article/details/ggbqktizs.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://mobile.zdbjq.cn/Article/details/gjtmkrwch.sHtML

[Q74] 强制使用索引
来源：http://3g.zdbjq.cn/Article/details/gfyhykikn.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.blog.zdbjq.cn/Article/details/gvfpbmaqd.sHtML

[Q75] 日期格式化
来源：http://m.share.zdbjq.cn/Article/details/ghwjcpijz.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://wap.zdbjq.cn/Article/details/gcczotpie.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://m.share.zdbjq.cn/Article/details/gupehwgzj.sHtML

[Q76] 按天统计
来源：http://www.blog.hesvh.cn/Article/details/gnlzeulkw.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.m.share.zdbjq.cn/Article/details/gtnbcagan.sHtML

[Q77] 时间加减
来源：http://read.share.fehbvm.com/Article/details/gpaauypnn.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.share.fehbvm.com/Article/details/grlslxhnf.sHtML

[Q78] 当前时间
来源：http://baike.fehbvm.com/Article/details/gmjayuzzt.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://read.share.fehbvm.com/Article/details/ggckpysxv.sHtML

[Q79] 字符串拼接
来源：http://www.blog.zdbjq.cn/Article/details/gluexbivz.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://blog.zdbjq.cn/Article/details/gkoirhjuf.sHtML

[Q80] 字符串截取
来源：http://mobile.hesvh.cn/Article/details/gqyshbxot.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gzptobfcu.sHtML

[Q81] 字符串替换
来源：http://baike.zdbjq.cn/Article/details/gbzuuxjfy.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://blog.zdbjq.cn/Article/details/gckxinlym.sHtML

[Q82] 字符长度与字节长度
来源：http://read.share.hesvh.cn/Article/details/gfutmjgrl.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.blog.hesvh.cn/Article/details/ggkhzsaaj.sHtML

[Q83] 大小写转换
来源：http://read.share.fehbvm.com/Article/details/gwcexxytg.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gfxyirqdb.sHtML

[Q84] 去除首尾空格
来源：http://wap.zdbjq.cn/Article/details/gwtbiebvh.sHtML

SELECT TRIM(name) FROM users;
来源：http://wap.hesvh.cn/Article/details/ghalppile.sHtML

[Q85] 数值取整
来源：http://baike.hesvh.cn/Article/details/ggftdnzrv.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://read.share.zdbjq.cn/Article/details/gfpbrshxw.sHtML

[Q86] 读取 JSON 字段
来源：http://www.share.fehbvm.com/Article/details/gyqsscguc.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://wap.hesvh.cn/Article/details/gswmabela.sHtML

[Q87] JSON 字段做条件
来源：http://mobile.zdbjq.cn/Article/details/gfwigaahf.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://mobile.zdbjq.cn/Article/details/guonbjckn.sHtML

[Q88] 行转列（条件聚合）
来源：http://blog.hesvh.cn/Article/details/gigdffxlm.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.m.share.fehbvm.com/Article/details/gkeicyfxa.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gbbhrnbot.sHtML

[Q89] 判断表是否存在
来源：http://www.share.hesvh.cn/Article/details/gwicnvyjr.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://blog.fehbvm.com/Article/details/geypgymbj.sHtML

[Q90] 生成序号列
来源：http://3g.fehbvm.com/Article/details/gktklsvgl.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.m.share.zdbjq.cn/Article/details/gdhkeimhe.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/guspyqwql.sHtML

R. Bash 专题
来源：http://www.m.share.zdbjq.cn/Article/details/gjaneavnl.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gzxqpyxnp.sHtML

[R01] shebang 与严格模式
来源：http://baike.zdbjq.cn/Article/details/gchngigxw.sHtML

#!/usr/bin/env bash
来源：http://www.blog.fehbvm.com/Article/details/ggpluvvfd.sHtML

set -euo pipefail
来源：http://www.share.hesvh.cn/Article/details/gmczoryfn.sHtML

[R02] 变量赋值与使用
来源：http://blog.hesvh.cn/Article/details/gahjkinsy.sHtML

name="Tom"; echo "$name"
来源：http://mobile.zdbjq.cn/Article/details/gxmpuznxo.sHtML

[R03] 只读变量
来源：http://mobile.hesvh.cn/Article/details/goywbjsxm.sHtML

readonly PI=3.14
来源：http://www.m.share.hesvh.cn/Article/details/gntnaasnb.sHtML

[R04] 位置参数
来源：http://3g.fehbvm.com/Article/details/gxjentjaq.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://3g.zdbjq.cn/Article/details/gruerdwko.sHtML

[R05] 参数默认值
来源：http://baike.hesvh.cn/Article/details/gqxkcgedy.sHtML

name="${1:-default}"
来源：http://www.blog.zdbjq.cn/Article/details/gofntnrdy.sHtML

[R06] 判断命令是否存在
来源：http://m.share.hesvh.cn/Article/details/gizeyeiyd.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://m.share.zdbjq.cn/Article/details/gblezegyk.sHtML

[R07] if 判断文件
来源：http://3g.hesvh.cn/Article/details/ggakmothe.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://wap.zdbjq.cn/Article/details/gjjhdkzmc.sHtML

[R08] 数值比较
来源：http://www.share.zdbjq.cn/Article/details/gpmsgxgwg.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://wap.hesvh.cn/Article/details/gssxvepir.sHtML

[R09] 字符串比较
来源：http://m.share.hesvh.cn/Article/details/glhfgiqgs.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://blog.zdbjq.cn/Article/details/gsagbgktm.sHtML

[R10] 正则匹配
来源：http://www.m.share.zdbjq.cn/Article/details/gbonlbile.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.share.zdbjq.cn/Article/details/gxjfdrxay.sHtML

[R11] case 多分支
来源：http://m.share.fehbvm.com/Article/details/garsgtfoi.sHtML

case "$1" in
来源：http://mobile.zdbjq.cn/Article/details/ghqnyayss.sHtML

start) echo "启动" ;;
来源：http://m.share.hesvh.cn/Article/details/gymkanhuf.sHtML

stop)  echo "停止" ;;
来源：http://read.share.zdbjq.cn/Article/details/ggafvtfnq.sHtML

*)     echo "未知命令" ;;
来源：http://baike.zdbjq.cn/Article/details/gxdkjztkn.sHtML

esac
来源：http://www.m.share.fehbvm.com/Article/details/gxnkuhdyz.sHtML

[R12] for 遍历文件
来源：http://m.share.hesvh.cn/Article/details/gnpkdaxgi.sHtML

for f in *.txt; do echo "$f"; done
来源：http://blog.hesvh.cn/Article/details/gbcwpdxfc.sHtML

[R13] for 计数循环
来源：http://wap.fehbvm.com/Article/details/gbhymjzrw.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://m.share.zdbjq.cn/Article/details/gsxatwmak.sHtML

[R14] C 风格 for
来源：http://www.share.hesvh.cn/Article/details/gqiczhqhk.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://baike.hesvh.cn/Article/details/gmwxcptlv.sHtML

[R15] while 逐行读文件
来源：http://3g.fehbvm.com/Article/details/gwuilumln.sHtML


<!-- 参考信息 -->