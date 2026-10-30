代发 wailian999

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.blog.hesvh.cn/Article/details/gayecdpkv.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.m.share.fehbvm.com/Article/details/gemlutsrr.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://baike.hesvh.cn/Article/details/gbkcpbmlp.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://m.share.hesvh.cn/Article/details/gueibtiww.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://wap.fehbvm.com/Article/details/gifdluchu.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://wap.fehbvm.com/Article/details/gcquzyxwc.sHtML

[P03] 生成短随机字符串
来源：http://www.share.fehbvm.com/Article/details/gzimylhwl.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://wap.hesvh.cn/Article/details/gkyhvmcza.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://wap.zdbjq.cn/Article/details/ggxplonhs.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.zdbjq.cn/Article/details/gamlyvfll.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.fehbvm.com/Article/details/gphkbbrpz.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.blog.zdbjq.cn/Article/details/gytneejto.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://m.share.fehbvm.com/Article/details/gjijykcis.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://m.share.fehbvm.com/Article/details/gkmajcwzm.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://wap.fehbvm.com/Article/details/gtvemvamg.sHtML

[P04] 求长度
来源：http://3g.hesvh.cn/Article/details/gareycpnh.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://baike.zdbjq.cn/Article/details/guhkrqiit.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.fehbvm.com/Article/details/gvmuquhos.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.zdbjq.cn/Article/details/guwqvhivd.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.hesvh.cn/Article/details/giidjfdah.sHtML

Java: list.size();  map.size();  s.length()
来源：http://3g.fehbvm.com/Article/details/gdnbvrrit.sHtML

Go:   len(arr);  len(m)
来源：http://www.m.share.hesvh.cn/Article/details/gyoehzeoh.sHtML

Ruby: x.length;  x.size
来源：http://m.share.zdbjq.cn/Article/details/goyswcivy.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://m.share.zdbjq.cn/Article/details/gfzogxomm.sHtML

[P05] 判断两个对象内容是否相等
来源：http://mobile.fehbvm.com/Article/details/gjgqjbodf.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://blog.zdbjq.cn/Article/details/gdvhqikyp.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://3g.hesvh.cn/Article/details/gnwnvygnz.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.blog.zdbjq.cn/Article/details/gocskeust.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.zdbjq.cn/Article/details/gipowhymr.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.m.share.zdbjq.cn/Article/details/ggwzhggiz.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.m.share.zdbjq.cn/Article/details/gkvnhksjc.sHtML

Ruby: a == b
来源：http://www.blog.zdbjq.cn/Article/details/gesghtupj.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.share.fehbvm.com/Article/details/gopupecvh.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://wap.fehbvm.com/Article/details/gualmnrbp.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.m.share.hesvh.cn/Article/details/gjlloujuz.sHtML

PHP:  if (empty($x)) {}
来源：http://m.share.hesvh.cn/Article/details/gbqliutcn.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://blog.zdbjq.cn/Article/details/griskjhfg.sHtML

TS:   if (x == null) {}
来源：http://3g.fehbvm.com/Article/details/gwjtqnsrn.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://wap.zdbjq.cn/Article/details/gujmsksbz.sHtML

Go:   if x == nil {}
来源：http://www.blog.hesvh.cn/Article/details/gmjynfwlb.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://mobile.zdbjq.cn/Article/details/ghmtagsne.sHtML

C#:   if (x is null) {}
来源：http://blog.fehbvm.com/Article/details/gpdscknwl.sHtML

[P07] 防抖与节流
来源：http://wap.zdbjq.cn/Article/details/ggoevpyjc.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://blog.hesvh.cn/Article/details/gcuwsznhm.sHtML

PHP:  // 手写时间戳比较
来源：http://3g.fehbvm.com/Article/details/gbvobevlc.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.hesvh.cn/Article/details/gntqrqcpw.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.hesvh.cn/Article/details/gqkokxwhb.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.share.zdbjq.cn/Article/details/gdjcvitus.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.share.fehbvm.com/Article/details/gsicwhteu.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.m.share.hesvh.cn/Article/details/gepttenxm.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.m.share.fehbvm.com/Article/details/gkkofxvkm.sHtML

[P08] 处理浮点精度问题
来源：http://3g.zdbjq.cn/Article/details/gkazuqups.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.blog.hesvh.cn/Article/details/gxkinoryn.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://baike.zdbjq.cn/Article/details/grghehykh.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.share.hesvh.cn/Article/details/ghayfdcbk.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://wap.fehbvm.com/Article/details/gmqxlffce.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://3g.zdbjq.cn/Article/details/gbkcewmle.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.share.zdbjq.cn/Article/details/goextxpmd.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://mobile.fehbvm.com/Article/details/gigprsiby.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://wap.hesvh.cn/Article/details/gbxjiblih.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gllxfwwyz.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://m.share.zdbjq.cn/Article/details/gvgpnbjzz.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gdcxczynt.sHtML

[Q01] 创建表
来源：http://www.m.share.fehbvm.com/Article/details/glaojyjgr.sHtML

CREATE TABLE users (
来源：http://mobile.hesvh.cn/Article/details/gdendiyxg.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.fehbvm.com/Article/details/gdjnvspnc.sHtML

name VARCHAR(50) NOT NULL,
来源：http://blog.fehbvm.com/Article/details/gsffulzpz.sHtML

email VARCHAR(100) UNIQUE,
来源：http://baike.hesvh.cn/Article/details/gvgkpwyed.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.blog.fehbvm.com/Article/details/gswyxoprc.sHtML

);
来源：http://read.share.zdbjq.cn/Article/details/gjnaytkyg.sHtML

[Q02] 创建带外键的表
来源：http://wap.fehbvm.com/Article/details/geodkrqcj.sHtML

CREATE TABLE orders (
来源：http://www.m.share.hesvh.cn/Article/details/gjoybcljk.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.fehbvm.com/Article/details/guxslasnc.sHtML

user_id INT NOT NULL,
来源：http://mobile.fehbvm.com/Article/details/gldfdblgx.sHtML

amount DECIMAL(10, 2),
来源：http://mobile.zdbjq.cn/Article/details/gdbcohlao.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://m.share.zdbjq.cn/Article/details/grskdeiqw.sHtML

);
来源：http://baike.zdbjq.cn/Article/details/gsvcpdcds.sHtML

[Q03] 增加列
来源：http://www.share.fehbvm.com/Article/details/gcqucscsu.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://baike.fehbvm.com/Article/details/gozbxudzz.sHtML

[Q04] 修改列类型
来源：http://blog.fehbvm.com/Article/details/gknfswksl.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.blog.zdbjq.cn/Article/details/gfjwtvftx.sHtML

[Q05] 重命名列
来源：http://www.share.zdbjq.cn/Article/details/gamwaelpq.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.share.zdbjq.cn/Article/details/gvbfmxigv.sHtML

[Q06] 删除列
来源：http://read.share.zdbjq.cn/Article/details/gpthgaqyn.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://m.share.zdbjq.cn/Article/details/gjiwnbfyr.sHtML

[Q07] 删除表
来源：http://blog.zdbjq.cn/Article/details/gypghomfg.sHtML

DROP TABLE IF EXISTS orders;
来源：http://m.share.zdbjq.cn/Article/details/gelkpvyda.sHtML

[Q08] 创建普通索引
来源：http://3g.hesvh.cn/Article/details/gxwrrbbmn.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://m.share.zdbjq.cn/Article/details/gdbizexou.sHtML

[Q09] 创建唯一索引
来源：http://3g.fehbvm.com/Article/details/gvhjgjhgb.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://3g.zdbjq.cn/Article/details/ggjjempnu.sHtML

[Q10] 插入单行
来源：http://blog.hesvh.cn/Article/details/gpcopedxq.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://mobile.hesvh.cn/Article/details/godegczcy.sHtML

[Q11] 一次插入多行
来源：http://m.share.zdbjq.cn/Article/details/gmeuocmtk.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.blog.fehbvm.com/Article/details/gpdcvppkm.sHtML

[Q12] 插入后取自增 ID
来源：http://m.share.fehbvm.com/Article/details/gezoqjeou.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.share.zdbjq.cn/Article/details/gvybiweki.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://mobile.hesvh.cn/Article/details/gqdgniims.sHtML

[Q13] 忽略重复插入
来源：http://baike.zdbjq.cn/Article/details/genpwihjy.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://baike.zdbjq.cn/Article/details/gvvwbfbtn.sHtML

[Q14] 存在则更新（upsert）
来源：http://m.share.zdbjq.cn/Article/details/ggwypvtnu.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.share.fehbvm.com/Article/details/gpxmhlana.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://wap.fehbvm.com/Article/details/gsxqfwbfl.sHtML

[Q15] 查询全部
来源：http://mobile.hesvh.cn/Article/details/gbnuanqha.sHtML

SELECT * FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gcqilpmuh.sHtML

[Q16] 查询指定列
来源：http://www.share.zdbjq.cn/Article/details/gmvklpphp.sHtML

SELECT id, name FROM users;
来源：http://3g.fehbvm.com/Article/details/gropcwqsa.sHtML

[Q17] 条件查询
来源：http://m.share.fehbvm.com/Article/details/gcimwjxlo.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://read.share.hesvh.cn/Article/details/gcucmjisx.sHtML

[Q18] 模糊匹配
来源：http://baike.fehbvm.com/Article/details/gjtedpnlj.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://3g.fehbvm.com/Article/details/gdafmzvsm.sHtML

[Q19] 范围查询
来源：http://www.blog.zdbjq.cn/Article/details/gpbwexsfo.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://read.share.hesvh.cn/Article/details/gdhbneyvm.sHtML

[Q20] IN 列表
来源：http://3g.hesvh.cn/Article/details/gbftlspuz.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.share.hesvh.cn/Article/details/gytqoiaij.sHtML

[Q21] 空值判断
来源：http://3g.fehbvm.com/Article/details/glpgqnwsm.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://m.share.zdbjq.cn/Article/details/grgcngnmd.sHtML

[Q22] 排序
来源：http://mobile.fehbvm.com/Article/details/gfkjgyzgv.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.m.share.fehbvm.com/Article/details/gqlgsacgz.sHtML

[Q23] 分页
来源：http://www.m.share.fehbvm.com/Article/details/gcisywzon.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.blog.zdbjq.cn/Article/details/gspegbqzh.sHtML

[Q24] 去重
来源：http://www.m.share.fehbvm.com/Article/details/gxjlyejqm.sHtML

SELECT DISTINCT city FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gughplbpz.sHtML

[Q25] 只取前 N 条
来源：http://baike.hesvh.cn/Article/details/ginilzgtq.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://baike.zdbjq.cn/Article/details/gtxixvzia.sHtML

[Q26] 计数
来源：http://read.share.fehbvm.com/Article/details/gdjwgqury.sHtML

SELECT COUNT(*) FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gxltaakxp.sHtML

[Q27] 条件计数
来源：http://blog.fehbvm.com/Article/details/grektwgbh.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://3g.fehbvm.com/Article/details/gdhsnecsu.sHtML

[Q28] 求和与平均
来源：http://mobile.zdbjq.cn/Article/details/gzwnpncun.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.m.share.zdbjq.cn/Article/details/gginnliwk.sHtML

[Q29] 最大最小值
来源：http://www.blog.hesvh.cn/Article/details/gfmmghlnk.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.share.hesvh.cn/Article/details/gnlnyhbrj.sHtML

[Q30] 分组统计
来源：http://m.share.fehbvm.com/Article/details/gctnbdrch.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://wap.fehbvm.com/Article/details/glqcqwdlr.sHtML

[Q31] 分组后过滤
来源：http://www.blog.fehbvm.com/Article/details/gytzwrvcn.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://blog.zdbjq.cn/Article/details/gjuqriqhy.sHtML

[Q32] 分组拼接字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gfjqoijpy.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.blog.hesvh.cn/Article/details/gxhkjfeon.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://read.share.zdbjq.cn/Article/details/gatuxgmjh.sHtML

[Q33] 多列分组
来源：http://baike.hesvh.cn/Article/details/gizzzlean.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://m.share.fehbvm.com/Article/details/gzzooihji.sHtML

[Q34] 每组取第一条
来源：http://baike.zdbjq.cn/Article/details/galjvgibs.sHtML

SELECT * FROM (
来源：http://read.share.fehbvm.com/Article/details/gssgtetsy.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.share.hesvh.cn/Article/details/ggakpuekl.sHtML

) t WHERE rn = 1;
来源：http://3g.zdbjq.cn/Article/details/gueljwgvp.sHtML

[Q35] 内连接
来源：http://baike.fehbvm.com/Article/details/gerufazrc.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://baike.zdbjq.cn/Article/details/gygvwreus.sHtML

[Q36] 左连接
来源：http://3g.zdbjq.cn/Article/details/gwcnbhzwu.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.zdbjq.cn/Article/details/ggwksrqth.sHtML

[Q37] 右连接
来源：http://baike.fehbvm.com/Article/details/gjycikdva.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://blog.fehbvm.com/Article/details/gbalqxadm.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.m.share.zdbjq.cn/Article/details/gkrgoftqq.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://wap.fehbvm.com/Article/details/goslmflvb.sHtML

[Q39] 自连接（查上下级）
来源：http://www.share.hesvh.cn/Article/details/ggtuucwou.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://baike.fehbvm.com/Article/details/golyljqlt.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://baike.fehbvm.com/Article/details/gfohhbxgk.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://m.share.fehbvm.com/Article/details/gzugkmerd.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.blog.hesvh.cn/Article/details/gfsekaaax.sHtML

[Q41] 多表连接
来源：http://3g.zdbjq.cn/Article/details/gkczubpca.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://wap.hesvh.cn/Article/details/guqfooqch.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.blog.hesvh.cn/Article/details/gvlrjhfnq.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.share.zdbjq.cn/Article/details/gfsjmzkqw.sHtML

[Q42] 连接条件附加过滤
来源：http://blog.zdbjq.cn/Article/details/gawzyuiag.sHtML

SELECT u.name, o.amount FROM users u
来源：http://wap.fehbvm.com/Article/details/gpdmpfstl.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.m.share.hesvh.cn/Article/details/gipqflxxk.sHtML

[Q43] 标量子查询
来源：http://m.share.hesvh.cn/Article/details/gojfpmile.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://wap.hesvh.cn/Article/details/gdufiixhq.sHtML

[Q44] IN 子查询
来源：http://blog.fehbvm.com/Article/details/gtzbnmche.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://read.share.fehbvm.com/Article/details/gbuonaglm.sHtML

[Q45] EXISTS 判断存在
来源：http://wap.fehbvm.com/Article/details/gqlaybxjw.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.hesvh.cn/Article/details/grjwpbwna.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://3g.zdbjq.cn/Article/details/godwbjkkm.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.hesvh.cn/Article/details/gqtvacxkr.sHtML

[Q47] 与平均值比较
来源：http://mobile.zdbjq.cn/Article/details/geafnaseo.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://m.share.hesvh.cn/Article/details/gqfhpemsn.sHtML

[Q48] CTE 公用表表达式
来源：http://baike.zdbjq.cn/Article/details/gcujfuvfg.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://wap.hesvh.cn/Article/details/gckcthkdv.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.blog.fehbvm.com/Article/details/gommtzmzc.sHtML

[Q49] 更新单行
来源：http://blog.fehbvm.com/Article/details/ggkqztjaa.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://read.share.fehbvm.com/Article/details/gyawmksib.sHtML

[Q50] 批量更新
来源：http://www.blog.hesvh.cn/Article/details/gyzgidcss.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.blog.hesvh.cn/Article/details/gphngtbgm.sHtML

[Q51] 用子查询更新
来源：http://www.m.share.zdbjq.cn/Article/details/gismvrwxa.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://mobile.hesvh.cn/Article/details/gyjrnhxsy.sHtML

[Q52] 删除指定行
来源：http://www.share.zdbjq.cn/Article/details/gnvnlupic.sHtML

DELETE FROM users WHERE id = 10;
来源：http://mobile.fehbvm.com/Article/details/gqweaknbw.sHtML

[Q53] 按条件删除
来源：http://mobile.fehbvm.com/Article/details/grvyrewox.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.blog.zdbjq.cn/Article/details/gjeohtrto.sHtML

[Q54] 清空表
来源：http://blog.hesvh.cn/Article/details/gmwiupvhl.sHtML

TRUNCATE TABLE logs;
来源：http://read.share.hesvh.cn/Article/details/gvolagejv.sHtML

[Q55] 排名（并列占位）
来源：http://www.share.fehbvm.com/Article/details/gslyrxrfx.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://baike.hesvh.cn/Article/details/gqxwusqaf.sHtML

[Q56] 密集排名（并列不占位）
来源：http://baike.zdbjq.cn/Article/details/gmvhhyycs.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://mobile.zdbjq.cn/Article/details/gbkyptpzn.sHtML

[Q57] 行号
来源：http://baike.fehbvm.com/Article/details/gpveftppf.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://baike.zdbjq.cn/Article/details/gdmpsvyur.sHtML

[Q58] 累计求和
来源：http://baike.zdbjq.cn/Article/details/gkaxwrcze.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://3g.zdbjq.cn/Article/details/gqcucpvrl.sHtML

[Q59] 分组内累计
来源：http://www.m.share.hesvh.cn/Article/details/gnwbxlydn.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://wap.zdbjq.cn/Article/details/gucmppevt.sHtML

[Q60] 取上一行 / 下一行
来源：http://m.share.zdbjq.cn/Article/details/geoofmrkq.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.blog.zdbjq.cn/Article/details/gqmemsksg.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://wap.fehbvm.com/Article/details/ghbhynoyi.sHtML

[Q61] 移动平均
来源：http://baike.hesvh.cn/Article/details/ghvgiqcox.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://m.share.fehbvm.com/Article/details/gtqzhroxh.sHtML

[Q62] 分组占比
来源：http://baike.hesvh.cn/Article/details/gbauqsixo.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://baike.hesvh.cn/Article/details/gyncuizxw.sHtML

[Q63] 开启事务
来源：http://www.m.share.fehbvm.com/Article/details/gzkybgxbd.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://blog.zdbjq.cn/Article/details/gcaxrvile.sHtML

[Q64] 提交事务
来源：http://www.blog.zdbjq.cn/Article/details/gbmgbnaes.sHtML

COMMIT;
来源：http://3g.zdbjq.cn/Article/details/gechletud.sHtML

[Q65] 回滚事务
来源：http://mobile.hesvh.cn/Article/details/gipnqhzuz.sHtML

ROLLBACK;
来源：http://mobile.zdbjq.cn/Article/details/gcsiadfqs.sHtML

[Q66] 行锁查询
来源：http://mobile.hesvh.cn/Article/details/giqxdnsfq.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://read.share.fehbvm.com/Article/details/gdymjixyv.sHtML

[Q67] 设置隔离级别
来源：http://www.share.hesvh.cn/Article/details/gewfoqeqj.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.blog.zdbjq.cn/Article/details/gmchkskcj.sHtML

[Q68] 保存点
来源：http://www.m.share.zdbjq.cn/Article/details/gkexkfsbs.sHtML

SAVEPOINT sp1;
来源：http://www.m.share.hesvh.cn/Article/details/grpmcgyho.sHtML

ROLLBACK TO sp1;
来源：http://read.share.zdbjq.cn/Article/details/grsoergxy.sHtML

[Q69] 查看执行计划
来源：http://3g.fehbvm.com/Article/details/gzrnydrrr.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://mobile.hesvh.cn/Article/details/gdfobxabp.sHtML

[Q70] 更新统计信息
来源：http://read.share.zdbjq.cn/Article/details/gujyqxhir.sHtML

ANALYZE TABLE users;
来源：http://blog.hesvh.cn/Article/details/gvkvmiklg.sHtML

[Q71] 查看建表语句
来源：http://www.m.share.fehbvm.com/Article/details/guqackrkb.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.m.share.hesvh.cn/Article/details/gnsgdhgff.sHtML

[Q72] 查看索引
来源：http://read.share.fehbvm.com/Article/details/gfkcdvodl.sHtML

SHOW INDEX FROM users;
来源：http://baike.hesvh.cn/Article/details/ghxglmjcr.sHtML

[Q73] 查看表状态
来源：http://wap.hesvh.cn/Article/details/giyqafxhw.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.blog.hesvh.cn/Article/details/gwmgqfvzl.sHtML

[Q74] 强制使用索引
来源：http://baike.zdbjq.cn/Article/details/gwqcbonvs.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://wap.hesvh.cn/Article/details/gwjgwziqm.sHtML

[Q75] 日期格式化
来源：http://mobile.hesvh.cn/Article/details/gyuyclsqj.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.m.share.hesvh.cn/Article/details/golhzhwxb.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://wap.hesvh.cn/Article/details/gcnpihsgz.sHtML

[Q76] 按天统计
来源：http://www.blog.zdbjq.cn/Article/details/glxgafvgy.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://3g.hesvh.cn/Article/details/gfniaeeuk.sHtML

[Q77] 时间加减
来源：http://www.blog.hesvh.cn/Article/details/gxypyfmnx.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://m.share.fehbvm.com/Article/details/gcosmxmxv.sHtML

[Q78] 当前时间
来源：http://www.share.hesvh.cn/Article/details/grtlsewdo.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://mobile.hesvh.cn/Article/details/gnjvnyaez.sHtML

[Q79] 字符串拼接
来源：http://read.share.hesvh.cn/Article/details/gdvhlflmu.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://read.share.fehbvm.com/Article/details/gmhepxaar.sHtML

[Q80] 字符串截取
来源：http://www.m.share.hesvh.cn/Article/details/ghopoxeed.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.share.hesvh.cn/Article/details/govbfiany.sHtML

[Q81] 字符串替换
来源：http://www.blog.zdbjq.cn/Article/details/gdrmsjydi.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gfkwwkmvv.sHtML

[Q82] 字符长度与字节长度
来源：http://3g.hesvh.cn/Article/details/gdqybhkky.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gwddqwdiw.sHtML

[Q83] 大小写转换
来源：http://mobile.fehbvm.com/Article/details/gftwfyfsi.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://mobile.hesvh.cn/Article/details/gealoeusz.sHtML

[Q84] 去除首尾空格
来源：http://m.share.hesvh.cn/Article/details/gcuxvshmt.sHtML

SELECT TRIM(name) FROM users;
来源：http://wap.fehbvm.com/Article/details/gamamlvdk.sHtML

[Q85] 数值取整
来源：http://wap.fehbvm.com/Article/details/gxdjoujrk.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://3g.fehbvm.com/Article/details/gpoigilny.sHtML

[Q86] 读取 JSON 字段
来源：http://www.blog.fehbvm.com/Article/details/gsxwymavr.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.m.share.fehbvm.com/Article/details/gcqprjzxm.sHtML

[Q87] JSON 字段做条件
来源：http://baike.fehbvm.com/Article/details/gubehogjr.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.share.zdbjq.cn/Article/details/gcvsjbooo.sHtML

[Q88] 行转列（条件聚合）
来源：http://baike.zdbjq.cn/Article/details/godeidmyj.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://3g.hesvh.cn/Article/details/gkrocolqx.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://3g.hesvh.cn/Article/details/gjiaelwog.sHtML

[Q89] 判断表是否存在
来源：http://baike.fehbvm.com/Article/details/gnrrmtjdq.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://m.share.fehbvm.com/Article/details/gmogmhytm.sHtML

[Q90] 生成序号列
来源：http://read.share.hesvh.cn/Article/details/gqylswlqi.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.m.share.zdbjq.cn/Article/details/grjbzjayo.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gcnlngklg.sHtML

R. Bash 专题
来源：http://m.share.fehbvm.com/Article/details/grdouupgk.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/grvqtvvgd.sHtML

[R01] shebang 与严格模式
来源：http://blog.zdbjq.cn/Article/details/gocfozndv.sHtML

#!/usr/bin/env bash
来源：http://www.share.zdbjq.cn/Article/details/gdvkquxzy.sHtML

set -euo pipefail
来源：http://wap.zdbjq.cn/Article/details/gesqwrblh.sHtML

[R02] 变量赋值与使用
来源：http://mobile.zdbjq.cn/Article/details/gxwbmhnap.sHtML

name="Tom"; echo "$name"
来源：http://3g.zdbjq.cn/Article/details/ghgtgsqng.sHtML

[R03] 只读变量
来源：http://3g.hesvh.cn/Article/details/gdusczjbx.sHtML

readonly PI=3.14
来源：http://read.share.fehbvm.com/Article/details/gcokjrrzv.sHtML

[R04] 位置参数
来源：http://www.m.share.fehbvm.com/Article/details/gwvmjlpie.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://mobile.fehbvm.com/Article/details/gpfbrqctg.sHtML

[R05] 参数默认值
来源：http://read.share.hesvh.cn/Article/details/gtzzrarff.sHtML

name="${1:-default}"
来源：http://m.share.hesvh.cn/Article/details/gnvearddl.sHtML

[R06] 判断命令是否存在
来源：http://read.share.hesvh.cn/Article/details/gcsvsvjka.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://blog.zdbjq.cn/Article/details/glxdkkitu.sHtML

[R07] if 判断文件
来源：http://3g.fehbvm.com/Article/details/gyjrczymb.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.blog.hesvh.cn/Article/details/gxwavckqa.sHtML

[R08] 数值比较
来源：http://www.m.share.hesvh.cn/Article/details/gynqwilla.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://m.share.fehbvm.com/Article/details/gnbjjixqn.sHtML

[R09] 字符串比较
来源：http://m.share.zdbjq.cn/Article/details/grfwqfxka.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://baike.fehbvm.com/Article/details/guooqahcj.sHtML

[R10] 正则匹配
来源：http://3g.hesvh.cn/Article/details/gebdjhbdu.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://baike.hesvh.cn/Article/details/ghtacwule.sHtML

[R11] case 多分支
来源：http://www.share.hesvh.cn/Article/details/geubrupfd.sHtML

case "$1" in
来源：http://blog.fehbvm.com/Article/details/gsdvpiank.sHtML

start) echo "启动" ;;
来源：http://mobile.zdbjq.cn/Article/details/gomdjmvda.sHtML

stop)  echo "停止" ;;
来源：http://3g.fehbvm.com/Article/details/gizspbbfr.sHtML

*)     echo "未知命令" ;;
来源：http://www.m.share.fehbvm.com/Article/details/ghsssxqge.sHtML

esac
来源：http://baike.zdbjq.cn/Article/details/gzadfuvwi.sHtML

[R12] for 遍历文件
来源：http://read.share.hesvh.cn/Article/details/gvvoimbob.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.m.share.zdbjq.cn/Article/details/goecvkjti.sHtML

[R13] for 计数循环
来源：http://www.share.zdbjq.cn/Article/details/gcueduoho.sHtML


<!-- 参考信息 -->