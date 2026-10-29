代发 wailian999

C#:   Guid.NewGuid().ToString()
来源：http://www.share.fehbvm.com/Article/details/gsabjkjdw.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.share.zdbjq.cn/Article/details/gdkdyxvhi.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://baike.hesvh.cn/Article/details/gsarbrasi.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://blog.zdbjq.cn/Article/details/gpovcnxjt.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://3g.fehbvm.com/Article/details/gtfvfxztr.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://m.share.zdbjq.cn/Article/details/ggxyjbkft.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://blog.hesvh.cn/Article/details/glgyxorby.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.share.fehbvm.com/Article/details/gaxwzoizw.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://m.share.zdbjq.cn/Article/details/ghbkwjjjy.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://wap.zdbjq.cn/Article/details/glatxfaht.sHtML

[P03] 生成短随机字符串
来源：http://mobile.fehbvm.com/Article/details/gwadhdlrk.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.m.share.zdbjq.cn/Article/details/getlrbttb.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://3g.hesvh.cn/Article/details/gvmbadpfa.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.zdbjq.cn/Article/details/gnrlxhebu.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.zdbjq.cn/Article/details/gsqdvygey.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://3g.fehbvm.com/Article/details/gmowugghk.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://m.share.fehbvm.com/Article/details/getaxrlgx.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://3g.hesvh.cn/Article/details/gjhimbtny.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://m.share.fehbvm.com/Article/details/gxxdrpofy.sHtML

[P04] 求长度
来源：http://wap.fehbvm.com/Article/details/gqynbksuj.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.m.share.fehbvm.com/Article/details/gmyzuzqdt.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.fehbvm.com/Article/details/gqoxfjnav.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.zdbjq.cn/Article/details/gyyemeucf.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.hesvh.cn/Article/details/gzgkjhuoa.sHtML

Java: list.size();  map.size();  s.length()
来源：http://baike.fehbvm.com/Article/details/gqmoleqzy.sHtML

Go:   len(arr);  len(m)
来源：http://baike.hesvh.cn/Article/details/gcrwofjuv.sHtML

Ruby: x.length;  x.size
来源：http://m.share.hesvh.cn/Article/details/ghzyrkwab.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://blog.hesvh.cn/Article/details/gewtdpesi.sHtML

[P05] 判断两个对象内容是否相等
来源：http://mobile.hesvh.cn/Article/details/gulmvtykb.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://wap.zdbjq.cn/Article/details/gctdsjtlf.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://m.share.fehbvm.com/Article/details/gdvypgqlc.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.m.share.zdbjq.cn/Article/details/ggkczmeat.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://read.share.hesvh.cn/Article/details/gdqhzjijm.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.share.hesvh.cn/Article/details/grftcbdtu.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://baike.zdbjq.cn/Article/details/gtqbbomou.sHtML

Ruby: a == b
来源：http://read.share.fehbvm.com/Article/details/gguspoulz.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.blog.fehbvm.com/Article/details/gefzlrvts.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.blog.hesvh.cn/Article/details/grxvmntrt.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://blog.hesvh.cn/Article/details/gicicftaa.sHtML

PHP:  if (empty($x)) {}
来源：http://mobile.zdbjq.cn/Article/details/gcmbrdyll.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.share.fehbvm.com/Article/details/gvoiilspq.sHtML

TS:   if (x == null) {}
来源：http://mobile.hesvh.cn/Article/details/gmmsmmidq.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://baike.zdbjq.cn/Article/details/gauiirmop.sHtML

Go:   if x == nil {}
来源：http://www.blog.fehbvm.com/Article/details/gfoxujbwl.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://blog.fehbvm.com/Article/details/gyjyfkytk.sHtML

C#:   if (x is null) {}
来源：http://m.share.fehbvm.com/Article/details/gkeduoyge.sHtML

[P07] 防抖与节流
来源：http://blog.zdbjq.cn/Article/details/gqhjgokib.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.m.share.hesvh.cn/Article/details/gooigpplq.sHtML

PHP:  // 手写时间戳比较
来源：http://read.share.zdbjq.cn/Article/details/gcicdyjad.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.fehbvm.com/Article/details/gvvdetunz.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.hesvh.cn/Article/details/gdxnwjwyi.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://3g.hesvh.cn/Article/details/gvpnyqiid.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.m.share.zdbjq.cn/Article/details/grxouqdim.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.m.share.fehbvm.com/Article/details/ghdyruqla.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.m.share.zdbjq.cn/Article/details/gdqplzfru.sHtML

[P08] 处理浮点精度问题
来源：http://wap.zdbjq.cn/Article/details/gltmfypds.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.blog.zdbjq.cn/Article/details/gfbhrlhns.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://3g.zdbjq.cn/Article/details/gvsgyfcrh.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.share.hesvh.cn/Article/details/gjjrrxmqr.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://3g.hesvh.cn/Article/details/gfgcbeeeb.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.blog.fehbvm.com/Article/details/gxaqpfckc.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://blog.zdbjq.cn/Article/details/grwahwvtp.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://wap.fehbvm.com/Article/details/gvpoeovcr.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://mobile.zdbjq.cn/Article/details/gegedbxlw.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gsskrqffy.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://blog.hesvh.cn/Article/details/gejyffpxk.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gvvhnykip.sHtML

[Q01] 创建表
来源：http://mobile.fehbvm.com/Article/details/grfpilgqr.sHtML

CREATE TABLE users (
来源：http://baike.zdbjq.cn/Article/details/gaklypenj.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.fehbvm.com/Article/details/ggwwlqbcs.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.share.hesvh.cn/Article/details/goonaszrj.sHtML

email VARCHAR(100) UNIQUE,
来源：http://mobile.zdbjq.cn/Article/details/gmwhunoao.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://blog.hesvh.cn/Article/details/gnkwhjhcs.sHtML

);
来源：http://3g.fehbvm.com/Article/details/gilzkzdfw.sHtML

[Q02] 创建带外键的表
来源：http://wap.fehbvm.com/Article/details/gxlzjdwcz.sHtML

CREATE TABLE orders (
来源：http://mobile.fehbvm.com/Article/details/gvwywcgvk.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.fehbvm.com/Article/details/gexgkhawg.sHtML

user_id INT NOT NULL,
来源：http://3g.zdbjq.cn/Article/details/gijyrxzld.sHtML

amount DECIMAL(10, 2),
来源：http://www.blog.fehbvm.com/Article/details/gmpnrslwy.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://m.share.hesvh.cn/Article/details/gwadekxqu.sHtML

);
来源：http://blog.fehbvm.com/Article/details/ggjscatbd.sHtML

[Q03] 增加列
来源：http://mobile.zdbjq.cn/Article/details/gpqamunbq.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://wap.zdbjq.cn/Article/details/gejwmapbc.sHtML

[Q04] 修改列类型
来源：http://mobile.fehbvm.com/Article/details/gbsntomre.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://wap.fehbvm.com/Article/details/gzozmbbij.sHtML

[Q05] 重命名列
来源：http://www.share.hesvh.cn/Article/details/gkcfpliii.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://m.share.fehbvm.com/Article/details/gcqidavsl.sHtML

[Q06] 删除列
来源：http://www.share.hesvh.cn/Article/details/gmtnpwtpp.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://wap.hesvh.cn/Article/details/gfxeflfwq.sHtML

[Q07] 删除表
来源：http://mobile.hesvh.cn/Article/details/gxtiprmgl.sHtML

DROP TABLE IF EXISTS orders;
来源：http://wap.fehbvm.com/Article/details/gvednqqem.sHtML

[Q08] 创建普通索引
来源：http://read.share.zdbjq.cn/Article/details/gkwsrgoch.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://mobile.hesvh.cn/Article/details/ggdbzxbsf.sHtML

[Q09] 创建唯一索引
来源：http://www.blog.hesvh.cn/Article/details/gefhomqgj.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.blog.zdbjq.cn/Article/details/gesytqsxq.sHtML

[Q10] 插入单行
来源：http://wap.hesvh.cn/Article/details/gmbjaznfz.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.m.share.hesvh.cn/Article/details/gyxebpyms.sHtML

[Q11] 一次插入多行
来源：http://blog.hesvh.cn/Article/details/gweeqvqvo.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.blog.hesvh.cn/Article/details/gcpyohnca.sHtML

[Q12] 插入后取自增 ID
来源：http://m.share.hesvh.cn/Article/details/gotegnpfm.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.m.share.hesvh.cn/Article/details/gwohtqubn.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.m.share.fehbvm.com/Article/details/gclcdgepb.sHtML

[Q13] 忽略重复插入
来源：http://www.blog.fehbvm.com/Article/details/gduekjskf.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://m.share.hesvh.cn/Article/details/gmsqziwpc.sHtML

[Q14] 存在则更新（upsert）
来源：http://read.share.zdbjq.cn/Article/details/gytvislcq.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://mobile.hesvh.cn/Article/details/gvfxdgbrd.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://3g.fehbvm.com/Article/details/gyaamzgeq.sHtML

[Q15] 查询全部
来源：http://www.m.share.zdbjq.cn/Article/details/gwzbkozob.sHtML

SELECT * FROM users;
来源：http://mobile.hesvh.cn/Article/details/glurskhrz.sHtML

[Q16] 查询指定列
来源：http://www.share.fehbvm.com/Article/details/gfaxrtlxg.sHtML

SELECT id, name FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gbizyqxyf.sHtML

[Q17] 条件查询
来源：http://read.share.hesvh.cn/Article/details/gdzbxmvap.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://3g.hesvh.cn/Article/details/geteexphk.sHtML

[Q18] 模糊匹配
来源：http://www.m.share.zdbjq.cn/Article/details/gonrsvrqx.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.m.share.hesvh.cn/Article/details/gvmrgdpla.sHtML

[Q19] 范围查询
来源：http://www.m.share.hesvh.cn/Article/details/gwfgasmna.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.share.zdbjq.cn/Article/details/glmpoiwke.sHtML

[Q20] IN 列表
来源：http://read.share.hesvh.cn/Article/details/gbixelkuv.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.share.fehbvm.com/Article/details/gfbdsweed.sHtML

[Q21] 空值判断
来源：http://read.share.fehbvm.com/Article/details/ghqvmbygo.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.m.share.fehbvm.com/Article/details/gkdlslgmz.sHtML

[Q22] 排序
来源：http://read.share.hesvh.cn/Article/details/ggfqygyrs.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.share.zdbjq.cn/Article/details/guahovsbm.sHtML

[Q23] 分页
来源：http://www.m.share.hesvh.cn/Article/details/gobwysucv.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://mobile.fehbvm.com/Article/details/gzpzerwly.sHtML

[Q24] 去重
来源：http://www.m.share.hesvh.cn/Article/details/gftbiyzpr.sHtML

SELECT DISTINCT city FROM users;
来源：http://3g.hesvh.cn/Article/details/gprryeeli.sHtML

[Q25] 只取前 N 条
来源：http://blog.fehbvm.com/Article/details/gnufgwbmg.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://m.share.fehbvm.com/Article/details/gzktzkzue.sHtML

[Q26] 计数
来源：http://m.share.hesvh.cn/Article/details/gofxzhwvy.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gscaijgtm.sHtML

[Q27] 条件计数
来源：http://read.share.fehbvm.com/Article/details/gginqqqzb.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://m.share.hesvh.cn/Article/details/gegrktpzi.sHtML

[Q28] 求和与平均
来源：http://blog.fehbvm.com/Article/details/gecrrxpex.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.blog.fehbvm.com/Article/details/gyvloplck.sHtML

[Q29] 最大最小值
来源：http://www.blog.hesvh.cn/Article/details/gzueypzbj.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://mobile.fehbvm.com/Article/details/gsnvshlmb.sHtML

[Q30] 分组统计
来源：http://blog.fehbvm.com/Article/details/gmubuvjmi.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://blog.zdbjq.cn/Article/details/gqqzucnez.sHtML

[Q31] 分组后过滤
来源：http://3g.hesvh.cn/Article/details/glzgwnfbi.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://wap.hesvh.cn/Article/details/gxtysvzim.sHtML

[Q32] 分组拼接字符串
来源：http://m.share.hesvh.cn/Article/details/gnzpvehai.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.blog.fehbvm.com/Article/details/grzewxafr.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://mobile.fehbvm.com/Article/details/gjwgvhdrq.sHtML

[Q33] 多列分组
来源：http://read.share.hesvh.cn/Article/details/gbequgcti.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://baike.hesvh.cn/Article/details/geixqkuah.sHtML

[Q34] 每组取第一条
来源：http://m.share.fehbvm.com/Article/details/grysvdpeb.sHtML

SELECT * FROM (
来源：http://www.m.share.zdbjq.cn/Article/details/gvdctnhgv.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.m.share.fehbvm.com/Article/details/gcxtaszzq.sHtML

) t WHERE rn = 1;
来源：http://read.share.hesvh.cn/Article/details/gzkaobati.sHtML

[Q35] 内连接
来源：http://wap.zdbjq.cn/Article/details/gmtiqrkss.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://baike.hesvh.cn/Article/details/gnknlnvac.sHtML

[Q36] 左连接
来源：http://m.share.zdbjq.cn/Article/details/grbxczzit.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://baike.fehbvm.com/Article/details/gkahsxnlb.sHtML

[Q37] 右连接
来源：http://mobile.hesvh.cn/Article/details/goyhfrayi.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://baike.hesvh.cn/Article/details/gcwvhmgec.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://mobile.fehbvm.com/Article/details/gyaexvbtj.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.m.share.fehbvm.com/Article/details/gyuoznmlj.sHtML

[Q39] 自连接（查上下级）
来源：http://read.share.fehbvm.com/Article/details/gckjtnmax.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://m.share.hesvh.cn/Article/details/gbgabegfh.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://read.share.fehbvm.com/Article/details/gicppvjoj.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.share.hesvh.cn/Article/details/gcwbezsij.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://baike.zdbjq.cn/Article/details/gwjzldnsm.sHtML

[Q41] 多表连接
来源：http://www.blog.zdbjq.cn/Article/details/ghdycvoor.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.m.share.fehbvm.com/Article/details/gbxyqhofl.sHtML

JOIN users u ON u.id = o.user_id
来源：http://baike.fehbvm.com/Article/details/gncwlxcnn.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.m.share.fehbvm.com/Article/details/gqsbtvhwj.sHtML

[Q42] 连接条件附加过滤
来源：http://baike.hesvh.cn/Article/details/gtpabdcbm.sHtML

SELECT u.name, o.amount FROM users u
来源：http://baike.zdbjq.cn/Article/details/grsttzzel.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://3g.hesvh.cn/Article/details/gbzrvcztt.sHtML

[Q43] 标量子查询
来源：http://www.m.share.fehbvm.com/Article/details/gmkcnygtj.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://m.share.zdbjq.cn/Article/details/gxgpsshqf.sHtML

[Q44] IN 子查询
来源：http://www.blog.hesvh.cn/Article/details/glbtqegjx.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://wap.fehbvm.com/Article/details/gupdsdfzc.sHtML

[Q45] EXISTS 判断存在
来源：http://wap.fehbvm.com/Article/details/gerbxcywy.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.fehbvm.com/Article/details/giagaoiqo.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://3g.fehbvm.com/Article/details/gtfcmnszy.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.zdbjq.cn/Article/details/gsoisahml.sHtML

[Q47] 与平均值比较
来源：http://www.share.hesvh.cn/Article/details/gfdsiyyqt.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://mobile.fehbvm.com/Article/details/gucehnuxk.sHtML

[Q48] CTE 公用表表达式
来源：http://3g.hesvh.cn/Article/details/gvjhyeasy.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://m.share.hesvh.cn/Article/details/gmoiprole.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.share.hesvh.cn/Article/details/grhhfuhoz.sHtML

[Q49] 更新单行
来源：http://m.share.zdbjq.cn/Article/details/geundogdt.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://read.share.fehbvm.com/Article/details/ghzwsnkfy.sHtML

[Q50] 批量更新
来源：http://blog.zdbjq.cn/Article/details/gfbehiwyq.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://3g.fehbvm.com/Article/details/gbnggyyri.sHtML

[Q51] 用子查询更新
来源：http://blog.hesvh.cn/Article/details/ggfunpxet.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://read.share.zdbjq.cn/Article/details/gnzvgellb.sHtML

[Q52] 删除指定行
来源：http://www.blog.fehbvm.com/Article/details/ggqpcddoc.sHtML

DELETE FROM users WHERE id = 10;
来源：http://mobile.fehbvm.com/Article/details/gsqxlvqxu.sHtML

[Q53] 按条件删除
来源：http://read.share.hesvh.cn/Article/details/gnqooihih.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://wap.fehbvm.com/Article/details/grhgsefnu.sHtML

[Q54] 清空表
来源：http://www.blog.hesvh.cn/Article/details/gjmhdtnsk.sHtML

TRUNCATE TABLE logs;
来源：http://m.share.zdbjq.cn/Article/details/gjhkzrera.sHtML

[Q55] 排名（并列占位）
来源：http://mobile.hesvh.cn/Article/details/gxsjkwlkq.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.blog.fehbvm.com/Article/details/gdnvossxf.sHtML

[Q56] 密集排名（并列不占位）
来源：http://blog.fehbvm.com/Article/details/grwytylzn.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://wap.hesvh.cn/Article/details/gquqmcrnn.sHtML

[Q57] 行号
来源：http://blog.hesvh.cn/Article/details/gftcrwtyq.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://3g.hesvh.cn/Article/details/gsyvvxzee.sHtML

[Q58] 累计求和
来源：http://www.share.zdbjq.cn/Article/details/gtvhrskwr.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.share.hesvh.cn/Article/details/gowjgfolt.sHtML

[Q59] 分组内累计
来源：http://read.share.hesvh.cn/Article/details/gxsxunxhq.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://m.share.hesvh.cn/Article/details/gwewznouz.sHtML

[Q60] 取上一行 / 下一行
来源：http://3g.zdbjq.cn/Article/details/gsehrddug.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.share.hesvh.cn/Article/details/gugdiclho.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://m.share.hesvh.cn/Article/details/gphwinxkv.sHtML

[Q61] 移动平均
来源：http://www.m.share.zdbjq.cn/Article/details/ghduqtchy.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://3g.zdbjq.cn/Article/details/gbtqbzafk.sHtML

[Q62] 分组占比
来源：http://3g.hesvh.cn/Article/details/gbjdxeuzz.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.m.share.hesvh.cn/Article/details/gbunwjlms.sHtML

[Q63] 开启事务
来源：http://www.blog.hesvh.cn/Article/details/gdgxsjokn.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.blog.hesvh.cn/Article/details/gnknihhre.sHtML

[Q64] 提交事务
来源：http://baike.zdbjq.cn/Article/details/gnuwenucn.sHtML

COMMIT;
来源：http://blog.zdbjq.cn/Article/details/gooraxqqt.sHtML

[Q65] 回滚事务
来源：http://wap.zdbjq.cn/Article/details/gifcoptnx.sHtML

ROLLBACK;
来源：http://mobile.fehbvm.com/Article/details/gfrlvottt.sHtML

[Q66] 行锁查询
来源：http://www.m.share.hesvh.cn/Article/details/ganphxfim.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://blog.fehbvm.com/Article/details/gpaehuglk.sHtML

[Q67] 设置隔离级别
来源：http://read.share.fehbvm.com/Article/details/gloyovtbs.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.share.zdbjq.cn/Article/details/gvgyjivws.sHtML

[Q68] 保存点
来源：http://mobile.hesvh.cn/Article/details/gkshjesgt.sHtML

SAVEPOINT sp1;
来源：http://wap.hesvh.cn/Article/details/gogdoxewm.sHtML

ROLLBACK TO sp1;
来源：http://baike.zdbjq.cn/Article/details/gzqtseafr.sHtML

[Q69] 查看执行计划
来源：http://www.m.share.zdbjq.cn/Article/details/guimpdxkn.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://m.share.fehbvm.com/Article/details/gcrzsfvlh.sHtML

[Q70] 更新统计信息
来源：http://m.share.hesvh.cn/Article/details/gghkspybf.sHtML

ANALYZE TABLE users;
来源：http://www.blog.zdbjq.cn/Article/details/gvgrfqjne.sHtML

[Q71] 查看建表语句
来源：http://m.share.hesvh.cn/Article/details/guuxuqxsl.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://mobile.zdbjq.cn/Article/details/gixddjppi.sHtML

[Q72] 查看索引
来源：http://www.m.share.fehbvm.com/Article/details/gwgdcdsrb.sHtML

SHOW INDEX FROM users;
来源：http://baike.zdbjq.cn/Article/details/gehjmgavb.sHtML

[Q73] 查看表状态
来源：http://m.share.fehbvm.com/Article/details/gvkuurpzf.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://wap.fehbvm.com/Article/details/gaubbbhru.sHtML

[Q74] 强制使用索引
来源：http://baike.zdbjq.cn/Article/details/gdyawlune.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://3g.fehbvm.com/Article/details/gbrrsjaqx.sHtML

[Q75] 日期格式化
来源：http://www.share.zdbjq.cn/Article/details/gkrvfmpgc.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.m.share.zdbjq.cn/Article/details/gzhjkyszu.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://blog.zdbjq.cn/Article/details/ghbxdcxsp.sHtML

[Q76] 按天统计
来源：http://3g.fehbvm.com/Article/details/ggoihrspt.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://read.share.zdbjq.cn/Article/details/gbkixtmqm.sHtML

[Q77] 时间加减
来源：http://www.m.share.hesvh.cn/Article/details/gcmscqypp.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.share.fehbvm.com/Article/details/gzvubauyh.sHtML

[Q78] 当前时间
来源：http://www.share.zdbjq.cn/Article/details/gpwtvroty.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.m.share.fehbvm.com/Article/details/gbbhaopih.sHtML

[Q79] 字符串拼接
来源：http://www.share.hesvh.cn/Article/details/gukzadnjn.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://wap.hesvh.cn/Article/details/gfowrtnbh.sHtML

[Q80] 字符串截取
来源：http://m.share.hesvh.cn/Article/details/gbghvdyqz.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://read.share.fehbvm.com/Article/details/gqnabevih.sHtML

[Q81] 字符串替换
来源：http://3g.fehbvm.com/Article/details/gjvpfygje.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://read.share.hesvh.cn/Article/details/gxdluityy.sHtML

[Q82] 字符长度与字节长度
来源：http://3g.fehbvm.com/Article/details/gykpefpan.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.blog.fehbvm.com/Article/details/ggannfbrw.sHtML

[Q83] 大小写转换
来源：http://www.share.hesvh.cn/Article/details/geavmodmv.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://3g.zdbjq.cn/Article/details/givohfumg.sHtML

[Q84] 去除首尾空格
来源：http://blog.zdbjq.cn/Article/details/giwptrrrb.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/guefafggm.sHtML

[Q85] 数值取整
来源：http://www.blog.zdbjq.cn/Article/details/gowoaddzr.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://m.share.fehbvm.com/Article/details/gfzwjivuo.sHtML

[Q86] 读取 JSON 字段
来源：http://mobile.fehbvm.com/Article/details/gqmbilhzf.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://wap.zdbjq.cn/Article/details/gmokvygxa.sHtML

[Q87] JSON 字段做条件
来源：http://m.share.hesvh.cn/Article/details/gdtsrbnmq.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://read.share.zdbjq.cn/Article/details/ghozwngzp.sHtML

[Q88] 行转列（条件聚合）
来源：http://blog.zdbjq.cn/Article/details/gzruiczia.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://mobile.fehbvm.com/Article/details/gzhfjzydr.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://wap.hesvh.cn/Article/details/gcpulwhsw.sHtML

[Q89] 判断表是否存在
来源：http://blog.hesvh.cn/Article/details/gpxntyfpi.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.blog.zdbjq.cn/Article/details/gkeemdjxg.sHtML

[Q90] 生成序号列
来源：http://wap.fehbvm.com/Article/details/ggrftrzxt.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://m.share.hesvh.cn/Article/details/golbrievh.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gqjataynn.sHtML

R. Bash 专题
来源：http://wap.zdbjq.cn/Article/details/gyaikosde.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/ghouxenww.sHtML

[R01] shebang 与严格模式
来源：http://www.blog.zdbjq.cn/Article/details/gcgyktkpu.sHtML

#!/usr/bin/env bash
来源：http://mobile.hesvh.cn/Article/details/gvrzsstiw.sHtML

set -euo pipefail
来源：http://www.blog.fehbvm.com/Article/details/gwdjohbij.sHtML

[R02] 变量赋值与使用
来源：http://www.blog.fehbvm.com/Article/details/gynuysurd.sHtML

name="Tom"; echo "$name"
来源：http://wap.hesvh.cn/Article/details/goerysmyl.sHtML

[R03] 只读变量
来源：http://www.share.zdbjq.cn/Article/details/gvcpnzdzo.sHtML

readonly PI=3.14
来源：http://www.m.share.zdbjq.cn/Article/details/gsbfymtjp.sHtML

[R04] 位置参数
来源：http://www.blog.fehbvm.com/Article/details/gelscubzw.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.m.share.zdbjq.cn/Article/details/guoakgsau.sHtML

[R05] 参数默认值
来源：http://m.share.zdbjq.cn/Article/details/gerzxllap.sHtML

name="${1:-default}"
来源：http://m.share.zdbjq.cn/Article/details/gspqnoljk.sHtML

[R06] 判断命令是否存在
来源：http://m.share.fehbvm.com/Article/details/gmffkezjl.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://blog.fehbvm.com/Article/details/gzhxzmpoo.sHtML

[R07] if 判断文件
来源：http://blog.fehbvm.com/Article/details/gsudeksxy.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.m.share.hesvh.cn/Article/details/gxcwmtuvm.sHtML

[R08] 数值比较
来源：http://www.blog.fehbvm.com/Article/details/genkjeapb.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.blog.hesvh.cn/Article/details/gtvqyurch.sHtML

[R09] 字符串比较
来源：http://www.blog.hesvh.cn/Article/details/gdpbgxmvy.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://wap.zdbjq.cn/Article/details/gftxseboc.sHtML

[R10] 正则匹配
来源：http://read.share.zdbjq.cn/Article/details/gfcnwoehd.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://read.share.fehbvm.com/Article/details/giotfsrll.sHtML

[R11] case 多分支
来源：http://wap.hesvh.cn/Article/details/gsukupydq.sHtML

case "$1" in
来源：http://wap.zdbjq.cn/Article/details/gsxjsfbzn.sHtML

start) echo "启动" ;;
来源：http://www.m.share.hesvh.cn/Article/details/gwyzgxfpu.sHtML

stop)  echo "停止" ;;
来源：http://3g.fehbvm.com/Article/details/gujpwcthi.sHtML

*)     echo "未知命令" ;;
来源：http://3g.fehbvm.com/Article/details/gcjyrrthu.sHtML


<!-- 参考信息 -->