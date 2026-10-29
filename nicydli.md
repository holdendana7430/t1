代发 wailian999

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.blog.hesvh.cn/Article/details/grhpsfqem.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.blog.hesvh.cn/Article/details/gjiliqoiy.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://baike.hesvh.cn/Article/details/gayieqlft.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://wap.zdbjq.cn/Article/details/gdwnkbqcd.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.m.share.fehbvm.com/Article/details/gcgzcrbru.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://m.share.fehbvm.com/Article/details/gnfcosmkz.sHtML

[P03] 生成短随机字符串
来源：http://wap.zdbjq.cn/Article/details/gcoxvblxd.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://wap.fehbvm.com/Article/details/gegbtehxb.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://m.share.fehbvm.com/Article/details/ghjrzofaz.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.zdbjq.cn/Article/details/gktxyhjdr.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.zdbjq.cn/Article/details/gwlfegcfc.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://baike.hesvh.cn/Article/details/gvhutbjir.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://mobile.fehbvm.com/Article/details/gkjoxwykd.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.blog.zdbjq.cn/Article/details/gemisytep.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.m.share.zdbjq.cn/Article/details/gsharqhga.sHtML

[P04] 求长度
来源：http://m.share.fehbvm.com/Article/details/glsqigmep.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://m.share.zdbjq.cn/Article/details/gzdqztyns.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.zdbjq.cn/Article/details/gwvbjxntn.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.fehbvm.com/Article/details/guoaqdeqo.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.fehbvm.com/Article/details/guqhphjwt.sHtML

Java: list.size();  map.size();  s.length()
来源：http://wap.fehbvm.com/Article/details/ghityjars.sHtML

Go:   len(arr);  len(m)
来源：http://www.share.zdbjq.cn/Article/details/gglnkbpmf.sHtML

Ruby: x.length;  x.size
来源：http://www.share.hesvh.cn/Article/details/geezyoeja.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.share.fehbvm.com/Article/details/goxjrpoqy.sHtML

[P05] 判断两个对象内容是否相等
来源：http://wap.fehbvm.com/Article/details/gnglapexp.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://wap.hesvh.cn/Article/details/gflfezywn.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.share.hesvh.cn/Article/details/gpiqgrwsb.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://wap.fehbvm.com/Article/details/gquotklkm.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://m.share.zdbjq.cn/Article/details/getjbhwah.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://m.share.fehbvm.com/Article/details/gqimpywmu.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://mobile.hesvh.cn/Article/details/gkyanomam.sHtML

Ruby: a == b
来源：http://wap.zdbjq.cn/Article/details/gbrwbhdgx.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://baike.fehbvm.com/Article/details/gakxhhxwk.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://baike.fehbvm.com/Article/details/ghysxjset.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://3g.fehbvm.com/Article/details/gxoxsggrm.sHtML

PHP:  if (empty($x)) {}
来源：http://read.share.zdbjq.cn/Article/details/gqpggsuqc.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.m.share.fehbvm.com/Article/details/gdyxskfwz.sHtML

TS:   if (x == null) {}
来源：http://www.blog.zdbjq.cn/Article/details/gybezrfke.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://read.share.zdbjq.cn/Article/details/gbulfufrd.sHtML

Go:   if x == nil {}
来源：http://m.share.fehbvm.com/Article/details/gfrysmgkv.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.blog.fehbvm.com/Article/details/gjdiyzhxx.sHtML

C#:   if (x is null) {}
来源：http://www.blog.zdbjq.cn/Article/details/gpfmbpwab.sHtML

[P07] 防抖与节流
来源：http://www.blog.hesvh.cn/Article/details/gxvmoyoxg.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://blog.zdbjq.cn/Article/details/gogfredsl.sHtML

PHP:  // 手写时间戳比较
来源：http://www.m.share.fehbvm.com/Article/details/gqoxysfgz.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.hesvh.cn/Article/details/gxglmzoft.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.fehbvm.com/Article/details/gujwmdzwe.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://blog.zdbjq.cn/Article/details/gegrmweus.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://mobile.fehbvm.com/Article/details/ggtfpvlcu.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://blog.fehbvm.com/Article/details/glrnldwfx.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://m.share.zdbjq.cn/Article/details/gemexeisx.sHtML

[P08] 处理浮点精度问题
来源：http://www.blog.zdbjq.cn/Article/details/grxpxkxcf.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://3g.hesvh.cn/Article/details/gilswxooq.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://baike.fehbvm.com/Article/details/gzydutsqh.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.share.zdbjq.cn/Article/details/gpizjmvop.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://3g.zdbjq.cn/Article/details/gcpufxwih.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.m.share.fehbvm.com/Article/details/gwcfmqcri.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://blog.hesvh.cn/Article/details/gbdkpjcfk.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://wap.hesvh.cn/Article/details/gjmhswjxz.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.share.hesvh.cn/Article/details/gdjxmkwws.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/ggdqmjgjg.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.share.fehbvm.com/Article/details/gggwcrzff.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gnmjvlocb.sHtML

[Q01] 创建表
来源：http://mobile.hesvh.cn/Article/details/gpjaixwln.sHtML

CREATE TABLE users (
来源：http://mobile.zdbjq.cn/Article/details/ghjmdkfms.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.share.hesvh.cn/Article/details/gbucrdnpj.sHtML

name VARCHAR(50) NOT NULL,
来源：http://m.share.fehbvm.com/Article/details/gxbcetsbi.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.share.zdbjq.cn/Article/details/gqqfzafdm.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.blog.hesvh.cn/Article/details/ghudmbjra.sHtML

);
来源：http://wap.fehbvm.com/Article/details/gwifvgjxj.sHtML

[Q02] 创建带外键的表
来源：http://mobile.hesvh.cn/Article/details/gcaunzlor.sHtML

CREATE TABLE orders (
来源：http://read.share.hesvh.cn/Article/details/gdvomfvla.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.hesvh.cn/Article/details/ghkgerwor.sHtML

user_id INT NOT NULL,
来源：http://read.share.hesvh.cn/Article/details/gnozqisyb.sHtML

amount DECIMAL(10, 2),
来源：http://www.share.hesvh.cn/Article/details/grsqsdvvl.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://baike.hesvh.cn/Article/details/gyvknmpqq.sHtML

);
来源：http://mobile.fehbvm.com/Article/details/gamlnbszj.sHtML

[Q03] 增加列
来源：http://read.share.fehbvm.com/Article/details/gvponstcq.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://baike.fehbvm.com/Article/details/gvyxfpaui.sHtML

[Q04] 修改列类型
来源：http://www.m.share.fehbvm.com/Article/details/grtbzsqbp.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://m.share.zdbjq.cn/Article/details/gwmpfzsga.sHtML

[Q05] 重命名列
来源：http://m.share.zdbjq.cn/Article/details/gcmcmnysv.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://read.share.zdbjq.cn/Article/details/gvmipbpco.sHtML

[Q06] 删除列
来源：http://www.share.fehbvm.com/Article/details/gevxcximu.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://wap.hesvh.cn/Article/details/gmhoupxyl.sHtML

[Q07] 删除表
来源：http://read.share.zdbjq.cn/Article/details/ganrmhvni.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.blog.hesvh.cn/Article/details/ggfqdainm.sHtML

[Q08] 创建普通索引
来源：http://read.share.hesvh.cn/Article/details/ggznvxkhj.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://3g.zdbjq.cn/Article/details/gaxuafnbf.sHtML

[Q09] 创建唯一索引
来源：http://www.m.share.fehbvm.com/Article/details/gsjquboyi.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://3g.fehbvm.com/Article/details/gghhmcsrf.sHtML

[Q10] 插入单行
来源：http://m.share.fehbvm.com/Article/details/guvkywupa.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://m.share.hesvh.cn/Article/details/ggcsuaxbd.sHtML

[Q11] 一次插入多行
来源：http://m.share.fehbvm.com/Article/details/gosbgsncz.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://read.share.fehbvm.com/Article/details/gbvqacmvf.sHtML

[Q12] 插入后取自增 ID
来源：http://baike.hesvh.cn/Article/details/gpajhxygs.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.share.zdbjq.cn/Article/details/gbaihpztz.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://read.share.fehbvm.com/Article/details/ghomviobg.sHtML

[Q13] 忽略重复插入
来源：http://www.share.hesvh.cn/Article/details/gqronqovl.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.share.fehbvm.com/Article/details/gbmhszvaf.sHtML

[Q14] 存在则更新（upsert）
来源：http://wap.zdbjq.cn/Article/details/gceuxhgbb.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://mobile.zdbjq.cn/Article/details/gywuudeew.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://3g.fehbvm.com/Article/details/gbafizmlv.sHtML

[Q15] 查询全部
来源：http://m.share.zdbjq.cn/Article/details/gxsxwzatb.sHtML

SELECT * FROM users;
来源：http://read.share.hesvh.cn/Article/details/gwoumhpzo.sHtML

[Q16] 查询指定列
来源：http://read.share.hesvh.cn/Article/details/gvmqsgtbh.sHtML

SELECT id, name FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gcernjfrg.sHtML

[Q17] 条件查询
来源：http://3g.zdbjq.cn/Article/details/gllbldkxt.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.blog.hesvh.cn/Article/details/gtekxhgap.sHtML

[Q18] 模糊匹配
来源：http://3g.hesvh.cn/Article/details/gbevpcheb.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://3g.hesvh.cn/Article/details/ghkuluwmx.sHtML

[Q19] 范围查询
来源：http://3g.zdbjq.cn/Article/details/giruqfmld.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.m.share.fehbvm.com/Article/details/gzpmmcliw.sHtML

[Q20] IN 列表
来源：http://blog.hesvh.cn/Article/details/gmruofobt.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://m.share.hesvh.cn/Article/details/gjlfhiisp.sHtML

[Q21] 空值判断
来源：http://www.blog.hesvh.cn/Article/details/guxxjfesg.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.blog.zdbjq.cn/Article/details/ghunjrlbf.sHtML

[Q22] 排序
来源：http://baike.fehbvm.com/Article/details/gxnlrvmol.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.m.share.hesvh.cn/Article/details/gmwgsqvkv.sHtML

[Q23] 分页
来源：http://www.share.fehbvm.com/Article/details/gpdyiklmn.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://read.share.fehbvm.com/Article/details/gyhpizxat.sHtML

[Q24] 去重
来源：http://3g.fehbvm.com/Article/details/gheasjbip.sHtML

SELECT DISTINCT city FROM users;
来源：http://3g.hesvh.cn/Article/details/gibqqqibf.sHtML

[Q25] 只取前 N 条
来源：http://wap.fehbvm.com/Article/details/gzcmtjcsr.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://read.share.hesvh.cn/Article/details/gythhoshd.sHtML

[Q26] 计数
来源：http://3g.hesvh.cn/Article/details/gjywxenux.sHtML

SELECT COUNT(*) FROM users;
来源：http://m.share.zdbjq.cn/Article/details/grdukkifv.sHtML

[Q27] 条件计数
来源：http://read.share.zdbjq.cn/Article/details/gmitiseii.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://baike.zdbjq.cn/Article/details/gdxqydvtd.sHtML

[Q28] 求和与平均
来源：http://m.share.zdbjq.cn/Article/details/gifrnyush.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.blog.hesvh.cn/Article/details/giavrgrkf.sHtML

[Q29] 最大最小值
来源：http://3g.fehbvm.com/Article/details/gicwvuzdy.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gctvusntc.sHtML

[Q30] 分组统计
来源：http://mobile.zdbjq.cn/Article/details/gdekpgxhd.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://wap.zdbjq.cn/Article/details/gruiyywfh.sHtML

[Q31] 分组后过滤
来源：http://www.blog.hesvh.cn/Article/details/gtshzhdbw.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://3g.fehbvm.com/Article/details/gnjvdhujj.sHtML

[Q32] 分组拼接字符串
来源：http://mobile.fehbvm.com/Article/details/gqaoewtzt.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://3g.hesvh.cn/Article/details/genqoirgi.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://baike.zdbjq.cn/Article/details/gdyldrigg.sHtML

[Q33] 多列分组
来源：http://mobile.fehbvm.com/Article/details/gxrinsopg.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://wap.zdbjq.cn/Article/details/gwwbfcnuc.sHtML

[Q34] 每组取第一条
来源：http://3g.fehbvm.com/Article/details/gtxnvdwkq.sHtML

SELECT * FROM (
来源：http://read.share.hesvh.cn/Article/details/gdqzyijhg.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://blog.hesvh.cn/Article/details/gwwhbqpag.sHtML

) t WHERE rn = 1;
来源：http://mobile.fehbvm.com/Article/details/gjtuutxmh.sHtML

[Q35] 内连接
来源：http://www.share.fehbvm.com/Article/details/geypetxil.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://mobile.fehbvm.com/Article/details/gsxgrvrcw.sHtML

[Q36] 左连接
来源：http://www.share.hesvh.cn/Article/details/gdxtnjatc.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://3g.hesvh.cn/Article/details/ggoxdulpf.sHtML

[Q37] 右连接
来源：http://wap.zdbjq.cn/Article/details/gtkfbndrr.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://3g.zdbjq.cn/Article/details/gxqfcyjth.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.share.zdbjq.cn/Article/details/gswzyhvyr.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://blog.fehbvm.com/Article/details/grjsquots.sHtML

[Q39] 自连接（查上下级）
来源：http://mobile.zdbjq.cn/Article/details/gsoahdgyl.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.share.zdbjq.cn/Article/details/gjbonymws.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://mobile.fehbvm.com/Article/details/gbaisgibf.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://wap.hesvh.cn/Article/details/gacmhvgtl.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.share.hesvh.cn/Article/details/gadzuzblo.sHtML

[Q41] 多表连接
来源：http://www.m.share.zdbjq.cn/Article/details/gedamjsan.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://mobile.hesvh.cn/Article/details/gzbyyqofy.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.blog.fehbvm.com/Article/details/gjfsvlltm.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.blog.hesvh.cn/Article/details/gghhhvoyi.sHtML

[Q42] 连接条件附加过滤
来源：http://www.m.share.fehbvm.com/Article/details/gcewjfycs.sHtML

SELECT u.name, o.amount FROM users u
来源：http://read.share.fehbvm.com/Article/details/gjmyuiueq.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://wap.hesvh.cn/Article/details/gmszfspnl.sHtML

[Q43] 标量子查询
来源：http://read.share.zdbjq.cn/Article/details/gduysrsus.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.share.zdbjq.cn/Article/details/gkvpyibyi.sHtML

[Q44] IN 子查询
来源：http://mobile.zdbjq.cn/Article/details/gfkmgygcd.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://mobile.hesvh.cn/Article/details/gdquaddkq.sHtML

[Q45] EXISTS 判断存在
来源：http://read.share.hesvh.cn/Article/details/gmyztzmev.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.zdbjq.cn/Article/details/gudfyjikh.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://baike.hesvh.cn/Article/details/gaqhcdigu.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.hesvh.cn/Article/details/gktbaihfi.sHtML

[Q47] 与平均值比较
来源：http://blog.fehbvm.com/Article/details/gwdclzagr.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.blog.fehbvm.com/Article/details/gfeftyobg.sHtML

[Q48] CTE 公用表表达式
来源：http://mobile.hesvh.cn/Article/details/gxxbufhdy.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://3g.fehbvm.com/Article/details/gxqsozbvo.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.m.share.hesvh.cn/Article/details/gluvosbse.sHtML

[Q49] 更新单行
来源：http://wap.hesvh.cn/Article/details/gkprzqgok.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.blog.zdbjq.cn/Article/details/ggtnxcujr.sHtML

[Q50] 批量更新
来源：http://www.m.share.zdbjq.cn/Article/details/gelnfyorb.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://baike.fehbvm.com/Article/details/gmtjdlzkb.sHtML

[Q51] 用子查询更新
来源：http://mobile.fehbvm.com/Article/details/gtdelubiv.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.m.share.fehbvm.com/Article/details/gnhrxolgv.sHtML

[Q52] 删除指定行
来源：http://www.blog.hesvh.cn/Article/details/gmlnceeqd.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.blog.fehbvm.com/Article/details/giggkhvks.sHtML

[Q53] 按条件删除
来源：http://m.share.hesvh.cn/Article/details/gapizgwlq.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://blog.zdbjq.cn/Article/details/gfswkfqum.sHtML

[Q54] 清空表
来源：http://www.m.share.zdbjq.cn/Article/details/gfizcnext.sHtML

TRUNCATE TABLE logs;
来源：http://3g.hesvh.cn/Article/details/glkribott.sHtML

[Q55] 排名（并列占位）
来源：http://mobile.hesvh.cn/Article/details/ggciqbrze.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://mobile.zdbjq.cn/Article/details/guqvoatla.sHtML

[Q56] 密集排名（并列不占位）
来源：http://blog.hesvh.cn/Article/details/gchqqpfuf.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://m.share.hesvh.cn/Article/details/guaevdexz.sHtML

[Q57] 行号
来源：http://www.blog.fehbvm.com/Article/details/gklxabull.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://m.share.hesvh.cn/Article/details/gjjpipauj.sHtML

[Q58] 累计求和
来源：http://3g.fehbvm.com/Article/details/gdboakhgy.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.blog.zdbjq.cn/Article/details/ggplwpwmu.sHtML

[Q59] 分组内累计
来源：http://www.m.share.fehbvm.com/Article/details/gnlxqbhbl.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://3g.zdbjq.cn/Article/details/gpivxjmjj.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.m.share.hesvh.cn/Article/details/gxjxwqscu.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://blog.zdbjq.cn/Article/details/gknqyuswh.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://read.share.hesvh.cn/Article/details/gokmdbmoi.sHtML

[Q61] 移动平均
来源：http://3g.fehbvm.com/Article/details/gqfrcoknn.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://mobile.fehbvm.com/Article/details/glmdawdzn.sHtML

[Q62] 分组占比
来源：http://www.m.share.zdbjq.cn/Article/details/giapubpyj.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.blog.zdbjq.cn/Article/details/gglkntkbw.sHtML

[Q63] 开启事务
来源：http://m.share.fehbvm.com/Article/details/gzqcjlmvl.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.share.fehbvm.com/Article/details/gyxlsofom.sHtML

[Q64] 提交事务
来源：http://baike.fehbvm.com/Article/details/gwzelxbwt.sHtML

COMMIT;
来源：http://www.share.fehbvm.com/Article/details/gbmafvldi.sHtML

[Q65] 回滚事务
来源：http://www.blog.zdbjq.cn/Article/details/gxqbvohkl.sHtML

ROLLBACK;
来源：http://blog.fehbvm.com/Article/details/gqkailnit.sHtML

[Q66] 行锁查询
来源：http://www.blog.fehbvm.com/Article/details/gobnupflg.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.blog.zdbjq.cn/Article/details/gdcddbujg.sHtML

[Q67] 设置隔离级别
来源：http://m.share.fehbvm.com/Article/details/gstdomgje.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://3g.hesvh.cn/Article/details/gweibbnhx.sHtML

[Q68] 保存点
来源：http://www.blog.zdbjq.cn/Article/details/gfautbiom.sHtML

SAVEPOINT sp1;
来源：http://www.blog.zdbjq.cn/Article/details/gkblqgaas.sHtML

ROLLBACK TO sp1;
来源：http://3g.zdbjq.cn/Article/details/gauqeddku.sHtML

[Q69] 查看执行计划
来源：http://wap.hesvh.cn/Article/details/gapkrekww.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://3g.zdbjq.cn/Article/details/gckrzpoyk.sHtML

[Q70] 更新统计信息
来源：http://3g.fehbvm.com/Article/details/ggbjclabk.sHtML

ANALYZE TABLE users;
来源：http://www.m.share.fehbvm.com/Article/details/grukmfrok.sHtML

[Q71] 查看建表语句
来源：http://www.m.share.hesvh.cn/Article/details/gmvwkfvbb.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://3g.hesvh.cn/Article/details/gxstzpigx.sHtML

[Q72] 查看索引
来源：http://wap.hesvh.cn/Article/details/gnorpmqdk.sHtML

SHOW INDEX FROM users;
来源：http://read.share.hesvh.cn/Article/details/gisvyebcy.sHtML

[Q73] 查看表状态
来源：http://read.share.hesvh.cn/Article/details/gqincislw.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://3g.hesvh.cn/Article/details/gocoefaqm.sHtML

[Q74] 强制使用索引
来源：http://3g.hesvh.cn/Article/details/ghdqcofok.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.m.share.zdbjq.cn/Article/details/glpcylalj.sHtML

[Q75] 日期格式化
来源：http://3g.fehbvm.com/Article/details/glmsamfcd.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.share.fehbvm.com/Article/details/glaqjagza.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://baike.hesvh.cn/Article/details/geiqqcqdq.sHtML

[Q76] 按天统计
来源：http://mobile.hesvh.cn/Article/details/gemagebki.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://blog.zdbjq.cn/Article/details/gdqgcrphv.sHtML

[Q77] 时间加减
来源：http://m.share.hesvh.cn/Article/details/gtmootevb.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://m.share.hesvh.cn/Article/details/gpsjzrtaa.sHtML

[Q78] 当前时间
来源：http://3g.zdbjq.cn/Article/details/gqcufclev.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://baike.zdbjq.cn/Article/details/gcyydjxlq.sHtML

[Q79] 字符串拼接
来源：http://mobile.hesvh.cn/Article/details/gqsxsdrvp.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://mobile.fehbvm.com/Article/details/gjuglouhd.sHtML

[Q80] 字符串截取
来源：http://mobile.hesvh.cn/Article/details/gxolfcfvl.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://m.share.hesvh.cn/Article/details/gsajkwgzx.sHtML

[Q81] 字符串替换
来源：http://www.share.zdbjq.cn/Article/details/ghkmutugr.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://read.share.fehbvm.com/Article/details/gbfxrltzo.sHtML

[Q82] 字符长度与字节长度
来源：http://mobile.fehbvm.com/Article/details/gfakfzgya.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gzslgqqmq.sHtML

[Q83] 大小写转换
来源：http://mobile.hesvh.cn/Article/details/gstnbiybq.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.share.fehbvm.com/Article/details/gapdlccdj.sHtML

[Q84] 去除首尾空格
来源：http://3g.fehbvm.com/Article/details/gdgzymoel.sHtML

SELECT TRIM(name) FROM users;
来源：http://wap.zdbjq.cn/Article/details/gkezvvfnv.sHtML

[Q85] 数值取整
来源：http://www.blog.hesvh.cn/Article/details/gnnhacemh.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.share.fehbvm.com/Article/details/gabysqplt.sHtML

[Q86] 读取 JSON 字段
来源：http://3g.zdbjq.cn/Article/details/ggrjykocy.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://mobile.zdbjq.cn/Article/details/gxjwdjwkt.sHtML

[Q87] JSON 字段做条件
来源：http://www.blog.hesvh.cn/Article/details/gutxjeyjg.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://mobile.zdbjq.cn/Article/details/gpzidwxun.sHtML

[Q88] 行转列（条件聚合）
来源：http://m.share.hesvh.cn/Article/details/gekkjygkk.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://read.share.fehbvm.com/Article/details/gcvznelrx.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gizonprwi.sHtML

[Q89] 判断表是否存在
来源：http://m.share.hesvh.cn/Article/details/ggkgwhhvj.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://m.share.zdbjq.cn/Article/details/gdiouhnss.sHtML

[Q90] 生成序号列
来源：http://3g.zdbjq.cn/Article/details/gkqhmqzut.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://m.share.fehbvm.com/Article/details/gxxkcebdp.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/ghqqztwpg.sHtML

R. Bash 专题
来源：http://www.m.share.zdbjq.cn/Article/details/gukulekbo.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/glccyzysl.sHtML

[R01] shebang 与严格模式
来源：http://read.share.hesvh.cn/Article/details/gjyzjuzul.sHtML

#!/usr/bin/env bash
来源：http://www.blog.hesvh.cn/Article/details/grwumddjp.sHtML

set -euo pipefail
来源：http://blog.fehbvm.com/Article/details/gimcmeiyg.sHtML

[R02] 变量赋值与使用
来源：http://mobile.zdbjq.cn/Article/details/gjxozergw.sHtML

name="Tom"; echo "$name"
来源：http://www.share.zdbjq.cn/Article/details/gxrcemrab.sHtML

[R03] 只读变量
来源：http://www.m.share.hesvh.cn/Article/details/gzrricrbj.sHtML

readonly PI=3.14
来源：http://www.blog.hesvh.cn/Article/details/gtwawpwvm.sHtML

[R04] 位置参数
来源：http://www.blog.fehbvm.com/Article/details/gnysnelqa.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://baike.hesvh.cn/Article/details/gvxbjfdwz.sHtML

[R05] 参数默认值
来源：http://read.share.zdbjq.cn/Article/details/gxviwurvg.sHtML

name="${1:-default}"
来源：http://m.share.hesvh.cn/Article/details/gbngvheaa.sHtML

[R06] 判断命令是否存在
来源：http://3g.hesvh.cn/Article/details/grqiagkpf.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.blog.hesvh.cn/Article/details/gmulzeffb.sHtML

[R07] if 判断文件
来源：http://www.share.fehbvm.com/Article/details/ggvmjzdss.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://baike.zdbjq.cn/Article/details/gkpihxbmh.sHtML

[R08] 数值比较
来源：http://www.m.share.hesvh.cn/Article/details/gbyuamczo.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://mobile.zdbjq.cn/Article/details/godcshkts.sHtML

[R09] 字符串比较
来源：http://mobile.zdbjq.cn/Article/details/gniwvvwsj.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.blog.fehbvm.com/Article/details/gawzjfpjj.sHtML

[R10] 正则匹配
来源：http://www.share.fehbvm.com/Article/details/gmdhyalxx.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.m.share.hesvh.cn/Article/details/gmvxtkvpm.sHtML

[R11] case 多分支
来源：http://www.share.zdbjq.cn/Article/details/glkwqxsxs.sHtML

case "$1" in
来源：http://blog.zdbjq.cn/Article/details/ggjsrvaun.sHtML

start) echo "启动" ;;
来源：http://blog.hesvh.cn/Article/details/gfhmvredc.sHtML

stop)  echo "停止" ;;
来源：http://m.share.hesvh.cn/Article/details/gdgymswkl.sHtML

*)     echo "未知命令" ;;
来源：http://www.m.share.zdbjq.cn/Article/details/gjdhvmupm.sHtML

esac
来源：http://www.m.share.hesvh.cn/Article/details/gtbqptach.sHtML

[R12] for 遍历文件
来源：http://baike.zdbjq.cn/Article/details/gthocxyhs.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.m.share.hesvh.cn/Article/details/gwbzlyzpt.sHtML

[R13] for 计数循环
来源：http://www.m.share.zdbjq.cn/Article/details/guimnvalj.sHtML


<!-- 参考信息 -->