代发 wailian999

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://baike.fehbvm.com/Article/details/gvcbtubqv.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.m.share.zdbjq.cn/Article/details/guhcpgftu.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://mobile.hesvh.cn/Article/details/gpwpjjvbo.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://wap.zdbjq.cn/Article/details/gdmxgfrgu.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://read.share.zdbjq.cn/Article/details/gzcgdhwix.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://3g.hesvh.cn/Article/details/gcqrcmwsi.sHtML

[P03] 生成短随机字符串
来源：http://mobile.fehbvm.com/Article/details/ghlnlehsm.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://wap.hesvh.cn/Article/details/gaoeitghc.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.m.share.hesvh.cn/Article/details/ggzdunekz.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.zdbjq.cn/Article/details/ggxbyjxfp.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.hesvh.cn/Article/details/gqxkdnbvw.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.share.fehbvm.com/Article/details/gzgtmvswo.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://mobile.zdbjq.cn/Article/details/gvpnwkgpx.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.m.share.fehbvm.com/Article/details/gkdkqevgo.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://read.share.zdbjq.cn/Article/details/gcrwpdapw.sHtML

[P04] 求长度
来源：http://www.share.zdbjq.cn/Article/details/grffggdnd.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://baike.hesvh.cn/Article/details/gejfefptj.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.hesvh.cn/Article/details/gdzvhvlqi.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.fehbvm.com/Article/details/gwbpsnwgp.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mobile.hesvh.cn/Article/details/geuinkgqc.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.share.fehbvm.com/Article/details/gojspzqsr.sHtML

Go:   len(arr);  len(m)
来源：http://www.share.hesvh.cn/Article/details/gwcvgmyfg.sHtML

Ruby: x.length;  x.size
来源：http://www.m.share.hesvh.cn/Article/details/gmbsmillz.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://mobile.fehbvm.com/Article/details/goubizlyl.sHtML

[P05] 判断两个对象内容是否相等
来源：http://wap.fehbvm.com/Article/details/gbvjzwdui.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://3g.hesvh.cn/Article/details/gyzxaeslc.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.blog.hesvh.cn/Article/details/gokrzfsnz.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.share.hesvh.cn/Article/details/gdpyojxog.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://baike.fehbvm.com/Article/details/gsjiojchy.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://m.share.zdbjq.cn/Article/details/gjatsahhg.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://blog.hesvh.cn/Article/details/gsbortjtu.sHtML

Ruby: a == b
来源：http://read.share.fehbvm.com/Article/details/gocbjspgu.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://m.share.zdbjq.cn/Article/details/gwhameskp.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://blog.zdbjq.cn/Article/details/gepcixpag.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.m.share.zdbjq.cn/Article/details/glivegjry.sHtML

PHP:  if (empty($x)) {}
来源：http://m.share.hesvh.cn/Article/details/gqmzrdjar.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://3g.fehbvm.com/Article/details/ghxpeqfug.sHtML

TS:   if (x == null) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gvwdtcmfx.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://m.share.fehbvm.com/Article/details/gnugragbp.sHtML

Go:   if x == nil {}
来源：http://read.share.hesvh.cn/Article/details/geovbytmj.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://mobile.hesvh.cn/Article/details/gdcmxhppu.sHtML

C#:   if (x is null) {}
来源：http://blog.hesvh.cn/Article/details/gxafifdpa.sHtML

[P07] 防抖与节流
来源：http://www.blog.zdbjq.cn/Article/details/gcytfoamn.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.blog.hesvh.cn/Article/details/gmyzktqaa.sHtML

PHP:  // 手写时间戳比较
来源：http://blog.zdbjq.cn/Article/details/gdcgonsae.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.fehbvm.com/Article/details/gvaxbfdcx.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.hesvh.cn/Article/details/gghjlcrwh.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.blog.fehbvm.com/Article/details/gpnbkxpsn.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://blog.zdbjq.cn/Article/details/gucglbual.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://wap.hesvh.cn/Article/details/gdypnnsji.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://3g.fehbvm.com/Article/details/ggkiuilrm.sHtML

[P08] 处理浮点精度问题
来源：http://www.m.share.zdbjq.cn/Article/details/gttyqpjot.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://read.share.hesvh.cn/Article/details/gowzslkng.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://mobile.fehbvm.com/Article/details/gyskpwzcg.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://wap.fehbvm.com/Article/details/gxcnykmib.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.blog.zdbjq.cn/Article/details/gujfprjyg.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://wap.fehbvm.com/Article/details/gqveprbuw.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://baike.fehbvm.com/Article/details/guefqsvcl.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://read.share.fehbvm.com/Article/details/gnihnfsgq.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://m.share.zdbjq.cn/Article/details/gqflnkivu.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gfnqcjjbk.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://blog.zdbjq.cn/Article/details/gdsmcwfti.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gzgzqdqds.sHtML

[Q01] 创建表
来源：http://3g.fehbvm.com/Article/details/gwbrjqjbm.sHtML

CREATE TABLE users (
来源：http://mobile.hesvh.cn/Article/details/gdeodojwl.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.zdbjq.cn/Article/details/gaishsgvb.sHtML

name VARCHAR(50) NOT NULL,
来源：http://baike.hesvh.cn/Article/details/gvnojndxd.sHtML

email VARCHAR(100) UNIQUE,
来源：http://read.share.zdbjq.cn/Article/details/gpsvvrvex.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://3g.zdbjq.cn/Article/details/gdoqsrkhz.sHtML

);
来源：http://m.share.fehbvm.com/Article/details/gmfpjtkmy.sHtML

[Q02] 创建带外键的表
来源：http://baike.zdbjq.cn/Article/details/gomyvbbwx.sHtML

CREATE TABLE orders (
来源：http://mobile.zdbjq.cn/Article/details/gxzkootjk.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.hesvh.cn/Article/details/galzcrsnc.sHtML

user_id INT NOT NULL,
来源：http://www.m.share.fehbvm.com/Article/details/gcfxqrgoe.sHtML

amount DECIMAL(10, 2),
来源：http://baike.zdbjq.cn/Article/details/gljulxvkv.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://read.share.zdbjq.cn/Article/details/ggapppadh.sHtML

);
来源：http://blog.hesvh.cn/Article/details/glxjuimom.sHtML

[Q03] 增加列
来源：http://baike.fehbvm.com/Article/details/gyxixwmwh.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://m.share.zdbjq.cn/Article/details/gujwfvmcn.sHtML

[Q04] 修改列类型
来源：http://www.m.share.fehbvm.com/Article/details/gwpkmdbzg.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.blog.fehbvm.com/Article/details/gcplinlio.sHtML

[Q05] 重命名列
来源：http://www.share.hesvh.cn/Article/details/gessgtcjz.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://read.share.hesvh.cn/Article/details/griyvzavf.sHtML

[Q06] 删除列
来源：http://wap.hesvh.cn/Article/details/ggyhjcgdx.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://mobile.fehbvm.com/Article/details/gxprwjtqy.sHtML

[Q07] 删除表
来源：http://blog.fehbvm.com/Article/details/gggxfjecv.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.blog.hesvh.cn/Article/details/grsgqcxhl.sHtML

[Q08] 创建普通索引
来源：http://mobile.zdbjq.cn/Article/details/gmcjxsygq.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://m.share.hesvh.cn/Article/details/gkbqhedin.sHtML

[Q09] 创建唯一索引
来源：http://m.share.fehbvm.com/Article/details/gywkviunj.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://blog.fehbvm.com/Article/details/gwbymwqgl.sHtML

[Q10] 插入单行
来源：http://www.share.zdbjq.cn/Article/details/gfjazupkr.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://blog.fehbvm.com/Article/details/gskldyrlq.sHtML

[Q11] 一次插入多行
来源：http://3g.hesvh.cn/Article/details/gumvcsnkd.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://mobile.fehbvm.com/Article/details/gxlexlwqo.sHtML

[Q12] 插入后取自增 ID
来源：http://mobile.zdbjq.cn/Article/details/gglmjhxhr.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://read.share.zdbjq.cn/Article/details/gowboashr.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://blog.hesvh.cn/Article/details/gbioahtap.sHtML

[Q13] 忽略重复插入
来源：http://m.share.fehbvm.com/Article/details/gtljnuowq.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://mobile.zdbjq.cn/Article/details/ghubwrvia.sHtML

[Q14] 存在则更新（upsert）
来源：http://blog.fehbvm.com/Article/details/gousoimxd.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://m.share.zdbjq.cn/Article/details/grlstnhcm.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://baike.zdbjq.cn/Article/details/gnxcosirn.sHtML

[Q15] 查询全部
来源：http://wap.fehbvm.com/Article/details/gjygdgtit.sHtML

SELECT * FROM users;
来源：http://wap.zdbjq.cn/Article/details/ggwpfgzug.sHtML

[Q16] 查询指定列
来源：http://www.m.share.fehbvm.com/Article/details/gibyxqsgo.sHtML

SELECT id, name FROM users;
来源：http://wap.hesvh.cn/Article/details/gguumjcjr.sHtML

[Q17] 条件查询
来源：http://3g.hesvh.cn/Article/details/gmgwfpopb.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.blog.zdbjq.cn/Article/details/gvzcvfahc.sHtML

[Q18] 模糊匹配
来源：http://www.m.share.zdbjq.cn/Article/details/gezfaotkd.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://read.share.hesvh.cn/Article/details/gdqjgzlkx.sHtML

[Q19] 范围查询
来源：http://www.m.share.zdbjq.cn/Article/details/gsrrsxtde.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://m.share.hesvh.cn/Article/details/gwthivrpg.sHtML

[Q20] IN 列表
来源：http://m.share.hesvh.cn/Article/details/gwcekqswz.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://mobile.fehbvm.com/Article/details/gugufmyfq.sHtML

[Q21] 空值判断
来源：http://m.share.hesvh.cn/Article/details/gxhsioyic.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://m.share.fehbvm.com/Article/details/garefmemm.sHtML

[Q22] 排序
来源：http://m.share.fehbvm.com/Article/details/gnqcwtcsf.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://mobile.fehbvm.com/Article/details/giigegzbv.sHtML

[Q23] 分页
来源：http://read.share.hesvh.cn/Article/details/geqgnatnz.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://mobile.zdbjq.cn/Article/details/goqfsrkav.sHtML

[Q24] 去重
来源：http://www.m.share.fehbvm.com/Article/details/gtctgmfxy.sHtML

SELECT DISTINCT city FROM users;
来源：http://blog.fehbvm.com/Article/details/gdzdagpmp.sHtML

[Q25] 只取前 N 条
来源：http://3g.fehbvm.com/Article/details/gcreynxva.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://mobile.fehbvm.com/Article/details/gjobotojl.sHtML

[Q26] 计数
来源：http://www.share.hesvh.cn/Article/details/gqfuounfv.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.blog.hesvh.cn/Article/details/giqwysxki.sHtML

[Q27] 条件计数
来源：http://mobile.hesvh.cn/Article/details/gwykxjhvp.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://blog.hesvh.cn/Article/details/gprnwseba.sHtML

[Q28] 求和与平均
来源：http://3g.fehbvm.com/Article/details/gllfgipiy.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.blog.hesvh.cn/Article/details/gqdccjulr.sHtML

[Q29] 最大最小值
来源：http://www.share.fehbvm.com/Article/details/gboiaksty.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://3g.fehbvm.com/Article/details/grjfeugpc.sHtML

[Q30] 分组统计
来源：http://mobile.zdbjq.cn/Article/details/glliaejlc.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.blog.hesvh.cn/Article/details/gmveserwo.sHtML

[Q31] 分组后过滤
来源：http://mobile.zdbjq.cn/Article/details/gjuwthzao.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://mobile.fehbvm.com/Article/details/gzlskikly.sHtML

[Q32] 分组拼接字符串
来源：http://m.share.hesvh.cn/Article/details/gpefrbwkn.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://wap.fehbvm.com/Article/details/gseeoryca.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://wap.fehbvm.com/Article/details/gwjpyyjtc.sHtML

[Q33] 多列分组
来源：http://wap.zdbjq.cn/Article/details/gmnluqiil.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.share.zdbjq.cn/Article/details/gqnsepewl.sHtML

[Q34] 每组取第一条
来源：http://www.m.share.hesvh.cn/Article/details/gkxjiraks.sHtML

SELECT * FROM (
来源：http://blog.zdbjq.cn/Article/details/gzmbixspg.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://m.share.fehbvm.com/Article/details/gvhsknqme.sHtML

) t WHERE rn = 1;
来源：http://wap.zdbjq.cn/Article/details/gjizkwkyh.sHtML

[Q35] 内连接
来源：http://www.share.zdbjq.cn/Article/details/gcbtcfact.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.fehbvm.com/Article/details/guuuuhgwa.sHtML

[Q36] 左连接
来源：http://www.m.share.hesvh.cn/Article/details/goekuhyvl.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://3g.fehbvm.com/Article/details/gilbrrnmr.sHtML

[Q37] 右连接
来源：http://www.share.zdbjq.cn/Article/details/gclahsvyt.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.blog.zdbjq.cn/Article/details/gisklmykd.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.blog.hesvh.cn/Article/details/ghbdoeezk.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.blog.hesvh.cn/Article/details/goyxeeqvv.sHtML

[Q39] 自连接（查上下级）
来源：http://www.m.share.fehbvm.com/Article/details/glyibffan.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.blog.hesvh.cn/Article/details/gbasmhfzr.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://baike.hesvh.cn/Article/details/gqpacncrj.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://3g.zdbjq.cn/Article/details/gvkeqxguu.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://mobile.zdbjq.cn/Article/details/gcjixykpo.sHtML

[Q41] 多表连接
来源：http://www.blog.zdbjq.cn/Article/details/guxcuiufv.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://wap.hesvh.cn/Article/details/gcdtrdegy.sHtML

JOIN users u ON u.id = o.user_id
来源：http://wap.hesvh.cn/Article/details/gtzkqxboj.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://3g.zdbjq.cn/Article/details/gbwysrecy.sHtML

[Q42] 连接条件附加过滤
来源：http://wap.fehbvm.com/Article/details/gameqmabr.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.blog.zdbjq.cn/Article/details/gdwqpoapp.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://read.share.hesvh.cn/Article/details/gzkofamga.sHtML

[Q43] 标量子查询
来源：http://baike.zdbjq.cn/Article/details/gjjlhwwmh.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://3g.hesvh.cn/Article/details/gxoyuaciu.sHtML

[Q44] IN 子查询
来源：http://3g.zdbjq.cn/Article/details/gtflrtlsc.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://3g.fehbvm.com/Article/details/gqyzybpsf.sHtML

[Q45] EXISTS 判断存在
来源：http://read.share.fehbvm.com/Article/details/gstnvdwxj.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.zdbjq.cn/Article/details/gahvvizig.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://baike.zdbjq.cn/Article/details/gidpygbyc.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.zdbjq.cn/Article/details/gtnynqrst.sHtML

[Q47] 与平均值比较
来源：http://mobile.zdbjq.cn/Article/details/gdjuhhqhw.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.blog.hesvh.cn/Article/details/godjclkca.sHtML

[Q48] CTE 公用表表达式
来源：http://blog.zdbjq.cn/Article/details/gltkszbpz.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://baike.fehbvm.com/Article/details/gowdklfsm.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://wap.zdbjq.cn/Article/details/gkcnbcsjl.sHtML

[Q49] 更新单行
来源：http://blog.zdbjq.cn/Article/details/gezsknmtn.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://3g.fehbvm.com/Article/details/gaxrtwozg.sHtML

[Q50] 批量更新
来源：http://www.blog.fehbvm.com/Article/details/gvifldsik.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://mobile.fehbvm.com/Article/details/geouzyfdg.sHtML

[Q51] 用子查询更新
来源：http://wap.fehbvm.com/Article/details/geirvclgq.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://m.share.fehbvm.com/Article/details/gydnaszwl.sHtML

[Q52] 删除指定行
来源：http://3g.fehbvm.com/Article/details/gcpbbwkax.sHtML

DELETE FROM users WHERE id = 10;
来源：http://wap.fehbvm.com/Article/details/gnlfxcqsd.sHtML

[Q53] 按条件删除
来源：http://www.share.hesvh.cn/Article/details/guwibmwqv.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.blog.fehbvm.com/Article/details/gssafhkal.sHtML

[Q54] 清空表
来源：http://3g.hesvh.cn/Article/details/gmxofjeyi.sHtML

TRUNCATE TABLE logs;
来源：http://www.share.fehbvm.com/Article/details/gfhatryqe.sHtML

[Q55] 排名（并列占位）
来源：http://www.share.fehbvm.com/Article/details/gdqjdvdgr.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://wap.zdbjq.cn/Article/details/gbvxyrael.sHtML

[Q56] 密集排名（并列不占位）
来源：http://baike.fehbvm.com/Article/details/gnqyfmish.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.share.fehbvm.com/Article/details/gzxajupnq.sHtML

[Q57] 行号
来源：http://blog.hesvh.cn/Article/details/gietwlgjg.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://blog.hesvh.cn/Article/details/giigfcyet.sHtML

[Q58] 累计求和
来源：http://wap.hesvh.cn/Article/details/ghzwiwplj.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://m.share.hesvh.cn/Article/details/gypholouk.sHtML

[Q59] 分组内累计
来源：http://www.m.share.hesvh.cn/Article/details/gtpyklkeo.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.share.hesvh.cn/Article/details/ghwlovvga.sHtML

[Q60] 取上一行 / 下一行
来源：http://wap.zdbjq.cn/Article/details/gcgggdzdh.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://baike.zdbjq.cn/Article/details/gskzdsqxd.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://mobile.fehbvm.com/Article/details/gzsvxypjs.sHtML

[Q61] 移动平均
来源：http://m.share.fehbvm.com/Article/details/gcovreufv.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://baike.hesvh.cn/Article/details/gmlrndneo.sHtML

[Q62] 分组占比
来源：http://www.m.share.hesvh.cn/Article/details/gyblhaaqs.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://mobile.hesvh.cn/Article/details/gbwzullop.sHtML

[Q63] 开启事务
来源：http://wap.zdbjq.cn/Article/details/gbfgazovy.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.share.fehbvm.com/Article/details/gihyixetq.sHtML

[Q64] 提交事务
来源：http://www.m.share.zdbjq.cn/Article/details/gefeiokdl.sHtML

COMMIT;
来源：http://m.share.hesvh.cn/Article/details/geundkame.sHtML

[Q65] 回滚事务
来源：http://www.m.share.fehbvm.com/Article/details/ggfpqncei.sHtML

ROLLBACK;
来源：http://wap.zdbjq.cn/Article/details/gkihsajlg.sHtML

[Q66] 行锁查询
来源：http://www.blog.zdbjq.cn/Article/details/gslpoyzzt.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://read.share.hesvh.cn/Article/details/gdgxidzcb.sHtML

[Q67] 设置隔离级别
来源：http://www.blog.zdbjq.cn/Article/details/gpvznyohg.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://baike.hesvh.cn/Article/details/gpzztownw.sHtML

[Q68] 保存点
来源：http://mobile.hesvh.cn/Article/details/gpltvrzhj.sHtML

SAVEPOINT sp1;
来源：http://wap.fehbvm.com/Article/details/geouxwjtf.sHtML

ROLLBACK TO sp1;
来源：http://www.m.share.zdbjq.cn/Article/details/gnjffovrt.sHtML

[Q69] 查看执行计划
来源：http://www.m.share.hesvh.cn/Article/details/gfiftdwkf.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://m.share.hesvh.cn/Article/details/gzzrakzfb.sHtML

[Q70] 更新统计信息
来源：http://mobile.fehbvm.com/Article/details/gircwwnnj.sHtML

ANALYZE TABLE users;
来源：http://3g.zdbjq.cn/Article/details/grxtdlkjv.sHtML

[Q71] 查看建表语句
来源：http://read.share.hesvh.cn/Article/details/gjnhjnmho.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.blog.zdbjq.cn/Article/details/gbxqwbqjx.sHtML

[Q72] 查看索引
来源：http://wap.zdbjq.cn/Article/details/gneuwvshz.sHtML

SHOW INDEX FROM users;
来源：http://baike.hesvh.cn/Article/details/gsdkkyrvq.sHtML

[Q73] 查看表状态
来源：http://mobile.zdbjq.cn/Article/details/grrexyvvm.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://wap.zdbjq.cn/Article/details/glcyvunip.sHtML

[Q74] 强制使用索引
来源：http://3g.hesvh.cn/Article/details/gqggaqxbg.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://read.share.fehbvm.com/Article/details/givqejoai.sHtML

[Q75] 日期格式化
来源：http://blog.hesvh.cn/Article/details/govhfxlag.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://wap.zdbjq.cn/Article/details/gkizrcsus.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.share.fehbvm.com/Article/details/gtehgwsgo.sHtML

[Q76] 按天统计
来源：http://www.m.share.fehbvm.com/Article/details/gtbwjwubp.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.blog.zdbjq.cn/Article/details/gnshxmwnm.sHtML

[Q77] 时间加减
来源：http://www.m.share.fehbvm.com/Article/details/gvrmbymqt.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.blog.zdbjq.cn/Article/details/gpfahqmfn.sHtML

[Q78] 当前时间
来源：http://m.share.fehbvm.com/Article/details/gxihiswdk.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://baike.hesvh.cn/Article/details/gksxyugxf.sHtML

[Q79] 字符串拼接
来源：http://3g.hesvh.cn/Article/details/gaxjhljxo.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.blog.zdbjq.cn/Article/details/gcyniguge.sHtML

[Q80] 字符串截取
来源：http://m.share.fehbvm.com/Article/details/gqiplzfdg.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gaoncoyvm.sHtML

[Q81] 字符串替换
来源：http://www.blog.fehbvm.com/Article/details/gqkkxatgu.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gwfqcttgf.sHtML

[Q82] 字符长度与字节长度
来源：http://www.share.fehbvm.com/Article/details/gyqgoczrc.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://m.share.hesvh.cn/Article/details/gkoutgshs.sHtML

[Q83] 大小写转换
来源：http://www.m.share.zdbjq.cn/Article/details/grqtrpmdp.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://read.share.fehbvm.com/Article/details/glpmftofg.sHtML

[Q84] 去除首尾空格
来源：http://3g.hesvh.cn/Article/details/gjliycvbc.sHtML

SELECT TRIM(name) FROM users;
来源：http://baike.fehbvm.com/Article/details/gkijuxftn.sHtML

[Q85] 数值取整
来源：http://read.share.zdbjq.cn/Article/details/gefcwfdtt.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://mobile.fehbvm.com/Article/details/gpqkontje.sHtML

[Q86] 读取 JSON 字段
来源：http://m.share.zdbjq.cn/Article/details/gaikzhxkz.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://wap.hesvh.cn/Article/details/gyicbjjra.sHtML

[Q87] JSON 字段做条件
来源：http://mobile.zdbjq.cn/Article/details/gminyyhpz.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://baike.hesvh.cn/Article/details/gjbpysycn.sHtML

[Q88] 行转列（条件聚合）
来源：http://mobile.fehbvm.com/Article/details/gytrfdkuw.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://mobile.fehbvm.com/Article/details/gmrhpyrvh.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/ggymiewxi.sHtML

[Q89] 判断表是否存在
来源：http://www.share.fehbvm.com/Article/details/gnmmvuexs.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://m.share.zdbjq.cn/Article/details/gcqjasklv.sHtML

[Q90] 生成序号列
来源：http://www.blog.hesvh.cn/Article/details/gvhxyuujq.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://blog.hesvh.cn/Article/details/gdcpsuvyr.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gcajliqhu.sHtML

R. Bash 专题
来源：http://blog.fehbvm.com/Article/details/gnaqbogmc.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gdskupaht.sHtML

[R01] shebang 与严格模式
来源：http://www.share.hesvh.cn/Article/details/ghhpuqqkv.sHtML

#!/usr/bin/env bash
来源：http://www.blog.zdbjq.cn/Article/details/gvvftohla.sHtML

set -euo pipefail
来源：http://m.share.fehbvm.com/Article/details/gyssorfta.sHtML

[R02] 变量赋值与使用
来源：http://blog.fehbvm.com/Article/details/ggjerdhcv.sHtML

name="Tom"; echo "$name"
来源：http://baike.zdbjq.cn/Article/details/glgirfpgq.sHtML

[R03] 只读变量
来源：http://mobile.zdbjq.cn/Article/details/guagikiik.sHtML

readonly PI=3.14
来源：http://baike.hesvh.cn/Article/details/gicnrlooy.sHtML

[R04] 位置参数
来源：http://www.share.zdbjq.cn/Article/details/grfeuyyxk.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://3g.hesvh.cn/Article/details/glqxwcabu.sHtML

[R05] 参数默认值
来源：http://m.share.zdbjq.cn/Article/details/gvgitggak.sHtML

name="${1:-default}"
来源：http://mobile.zdbjq.cn/Article/details/gwtjcrzzh.sHtML

[R06] 判断命令是否存在
来源：http://www.blog.fehbvm.com/Article/details/gxjzmdlxf.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://baike.zdbjq.cn/Article/details/gilyqddgn.sHtML

[R07] if 判断文件
来源：http://3g.hesvh.cn/Article/details/gsklblljy.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://baike.fehbvm.com/Article/details/gzxajnjik.sHtML

[R08] 数值比较
来源：http://baike.zdbjq.cn/Article/details/gehrufzuy.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://3g.fehbvm.com/Article/details/gglwvijep.sHtML

[R09] 字符串比较
来源：http://read.share.zdbjq.cn/Article/details/gkupmywox.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.m.share.zdbjq.cn/Article/details/gkisuqzpw.sHtML

[R10] 正则匹配
来源：http://mobile.hesvh.cn/Article/details/grvwgjqbq.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.blog.zdbjq.cn/Article/details/gynytjdza.sHtML

[R11] case 多分支
来源：http://read.share.hesvh.cn/Article/details/gdkrpaxnq.sHtML

case "$1" in
来源：http://read.share.hesvh.cn/Article/details/glbvohrhg.sHtML

start) echo "启动" ;;
来源：http://m.share.zdbjq.cn/Article/details/gkvlblmqp.sHtML

stop)  echo "停止" ;;
来源：http://blog.fehbvm.com/Article/details/gaddouche.sHtML

*)     echo "未知命令" ;;
来源：http://read.share.hesvh.cn/Article/details/gsflbmymt.sHtML

esac
来源：http://mobile.fehbvm.com/Article/details/gzfxlqzvy.sHtML

[R12] for 遍历文件
来源：http://wap.hesvh.cn/Article/details/glzszolxz.sHtML

for f in *.txt; do echo "$f"; done
来源：http://read.share.fehbvm.com/Article/details/grtspcdwe.sHtML

[R13] for 计数循环
来源：http://blog.zdbjq.cn/Article/details/gehmqtwyo.sHtML


<!-- 参考信息 -->