代发 wailian999

[P01] 生成 UUID
来源：http://blog.zdbjq.cn/Article/details/glpxmenqi.sHtML

Py:   str(uuid.uuid4())
来源：http://mobile.zdbjq.cn/Article/details/gmgwulwvt.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://wap.hesvh.cn/Article/details/gvdxxdzcc.sHtML

JS:   crypto.randomUUID()
来源：http://www.share.zdbjq.cn/Article/details/gapfnwvhl.sHtML

TS:   crypto.randomUUID()
来源：http://www.share.fehbvm.com/Article/details/gezjenpjj.sHtML

Java: UUID.randomUUID().toString()
来源：http://wap.zdbjq.cn/Article/details/gtkgbrfem.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.share.hesvh.cn/Article/details/glthfwmwt.sHtML

Ruby: SecureRandom.uuid
来源：http://3g.fehbvm.com/Article/details/gdozfzgpm.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://wap.zdbjq.cn/Article/details/ggrdkfufi.sHtML

[P02] MD5 / SHA256 摘要
来源：http://3g.zdbjq.cn/Article/details/gocvriscq.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://baike.zdbjq.cn/Article/details/gjstebpig.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.m.share.hesvh.cn/Article/details/gmlxetizj.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://m.share.fehbvm.com/Article/details/ggqshffph.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://mobile.hesvh.cn/Article/details/glhmjhtry.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.share.zdbjq.cn/Article/details/gyuyflstj.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://baike.hesvh.cn/Article/details/gtqwqinfc.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.m.share.hesvh.cn/Article/details/gkmtdnkti.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://m.share.hesvh.cn/Article/details/gdyqdsmfr.sHtML

[P03] 生成短随机字符串
来源：http://3g.hesvh.cn/Article/details/gpbtsdfgd.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.blog.fehbvm.com/Article/details/gnprdicqo.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://baike.zdbjq.cn/Article/details/gqtfvrckf.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.hesvh.cn/Article/details/gxqwguakg.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.fehbvm.com/Article/details/gxeskafqd.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.blog.hesvh.cn/Article/details/gwpgkzumd.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://read.share.hesvh.cn/Article/details/gusodyxee.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://read.share.zdbjq.cn/Article/details/gnwygbcpw.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://m.share.hesvh.cn/Article/details/giynvsemr.sHtML

[P04] 求长度
来源：http://mobile.hesvh.cn/Article/details/gxjuzwywa.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://mobile.fehbvm.com/Article/details/gewhnuteb.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.hesvh.cn/Article/details/goxtibdcz.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.hesvh.cn/Article/details/ggncmmvtx.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.zdbjq.cn/Article/details/gjrnmqxjf.sHtML

Java: list.size();  map.size();  s.length()
来源：http://read.share.zdbjq.cn/Article/details/goszdplru.sHtML

Go:   len(arr);  len(m)
来源：http://baike.fehbvm.com/Article/details/ghthksvoh.sHtML

Ruby: x.length;  x.size
来源：http://3g.hesvh.cn/Article/details/giasjexam.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://3g.fehbvm.com/Article/details/gwazqcomd.sHtML

[P05] 判断两个对象内容是否相等
来源：http://baike.hesvh.cn/Article/details/gjtlzqcpx.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.share.hesvh.cn/Article/details/gxtbxvuqt.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://m.share.zdbjq.cn/Article/details/gtdbarbek.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://blog.fehbvm.com/Article/details/gjoyfutbt.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.share.zdbjq.cn/Article/details/gsxplyuyz.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://mobile.hesvh.cn/Article/details/guqqnllgy.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://wap.zdbjq.cn/Article/details/gomyrdkuj.sHtML

Ruby: a == b
来源：http://mobile.hesvh.cn/Article/details/gumnhiafu.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://blog.hesvh.cn/Article/details/gmbqevdem.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://mobile.hesvh.cn/Article/details/gdmajweli.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://mobile.hesvh.cn/Article/details/gomgpfdqe.sHtML

PHP:  if (empty($x)) {}
来源：http://mobile.zdbjq.cn/Article/details/gzcnlkszo.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://m.share.zdbjq.cn/Article/details/gqpkmjasr.sHtML

TS:   if (x == null) {}
来源：http://www.blog.fehbvm.com/Article/details/gbppkoxiq.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.m.share.hesvh.cn/Article/details/gifmeicrb.sHtML

Go:   if x == nil {}
来源：http://wap.zdbjq.cn/Article/details/griaulsyz.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://baike.zdbjq.cn/Article/details/gbujxqsrb.sHtML

C#:   if (x is null) {}
来源：http://www.share.zdbjq.cn/Article/details/grrlsgmzi.sHtML

[P07] 防抖与节流
来源：http://3g.zdbjq.cn/Article/details/gifyfghyl.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://m.share.zdbjq.cn/Article/details/gvsrgglnd.sHtML

PHP:  // 手写时间戳比较
来源：http://blog.fehbvm.com/Article/details/gptaknuwc.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.hesvh.cn/Article/details/gxdobkhyc.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.hesvh.cn/Article/details/grcrdizex.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.blog.fehbvm.com/Article/details/glxodlgef.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://read.share.zdbjq.cn/Article/details/giaiebqcd.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://mobile.zdbjq.cn/Article/details/ggxsykipi.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://baike.zdbjq.cn/Article/details/ghkbffklf.sHtML

[P08] 处理浮点精度问题
来源：http://www.m.share.fehbvm.com/Article/details/giocampct.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.blog.hesvh.cn/Article/details/gigplalmd.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.m.share.hesvh.cn/Article/details/gotelpysf.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://m.share.fehbvm.com/Article/details/guslymhsb.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://3g.hesvh.cn/Article/details/gpaescfhd.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://blog.fehbvm.com/Article/details/gwlplosef.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://read.share.zdbjq.cn/Article/details/gsatmyfcc.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.blog.fehbvm.com/Article/details/grokobytw.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.blog.zdbjq.cn/Article/details/gfoxtihoq.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/ghrtrkqqt.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://blog.fehbvm.com/Article/details/gimchqcaj.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gctmanlje.sHtML

[Q01] 创建表
来源：http://baike.zdbjq.cn/Article/details/gnrfopdyt.sHtML

CREATE TABLE users (
来源：http://www.m.share.hesvh.cn/Article/details/gcgfhovjc.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.fehbvm.com/Article/details/gvoeatbjl.sHtML

name VARCHAR(50) NOT NULL,
来源：http://blog.fehbvm.com/Article/details/gjwwlapek.sHtML

email VARCHAR(100) UNIQUE,
来源：http://baike.hesvh.cn/Article/details/gffekxawm.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://wap.hesvh.cn/Article/details/gvgzodggr.sHtML

);
来源：http://blog.hesvh.cn/Article/details/gxezksmuj.sHtML

[Q02] 创建带外键的表
来源：http://3g.hesvh.cn/Article/details/gphaazyxy.sHtML

CREATE TABLE orders (
来源：http://www.m.share.fehbvm.com/Article/details/gzdfzjlvh.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.zdbjq.cn/Article/details/grcqmqzop.sHtML

user_id INT NOT NULL,
来源：http://3g.hesvh.cn/Article/details/gftvqbflt.sHtML

amount DECIMAL(10, 2),
来源：http://3g.fehbvm.com/Article/details/gcxdbbddi.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://blog.fehbvm.com/Article/details/gcwgvqcus.sHtML

);
来源：http://www.m.share.zdbjq.cn/Article/details/guxvxfmex.sHtML

[Q03] 增加列
来源：http://www.m.share.hesvh.cn/Article/details/gnksdmgfp.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://mobile.hesvh.cn/Article/details/guydhdtql.sHtML

[Q04] 修改列类型
来源：http://read.share.hesvh.cn/Article/details/gikynzcwu.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://blog.fehbvm.com/Article/details/gpuztvnlr.sHtML

[Q05] 重命名列
来源：http://www.m.share.zdbjq.cn/Article/details/gmmqkjzqw.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.share.fehbvm.com/Article/details/gxyjtapdr.sHtML

[Q06] 删除列
来源：http://mobile.hesvh.cn/Article/details/gbefdsmsi.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://blog.zdbjq.cn/Article/details/guuiiziot.sHtML

[Q07] 删除表
来源：http://www.share.fehbvm.com/Article/details/gpvafzclo.sHtML

DROP TABLE IF EXISTS orders;
来源：http://m.share.fehbvm.com/Article/details/glxrhtvxt.sHtML

[Q08] 创建普通索引
来源：http://www.m.share.zdbjq.cn/Article/details/gyhybzkxc.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://read.share.zdbjq.cn/Article/details/gmqxygtwd.sHtML

[Q09] 创建唯一索引
来源：http://3g.zdbjq.cn/Article/details/gsainqplw.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://m.share.fehbvm.com/Article/details/ggidosxtr.sHtML

[Q10] 插入单行
来源：http://baike.zdbjq.cn/Article/details/ghrfenydj.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://m.share.zdbjq.cn/Article/details/gzkacoomh.sHtML

[Q11] 一次插入多行
来源：http://www.share.fehbvm.com/Article/details/gfwemplbh.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://baike.hesvh.cn/Article/details/gniwnwqvr.sHtML

[Q12] 插入后取自增 ID
来源：http://www.m.share.hesvh.cn/Article/details/gjmewvtrw.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://read.share.zdbjq.cn/Article/details/gwvitdegn.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.share.fehbvm.com/Article/details/gsxwcybdf.sHtML

[Q13] 忽略重复插入
来源：http://baike.zdbjq.cn/Article/details/gpqutydym.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://3g.zdbjq.cn/Article/details/gzftselwn.sHtML

[Q14] 存在则更新（upsert）
来源：http://3g.zdbjq.cn/Article/details/glhqqugtn.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://m.share.zdbjq.cn/Article/details/gydzwvzpd.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.blog.fehbvm.com/Article/details/gkvunoqvv.sHtML

[Q15] 查询全部
来源：http://www.m.share.hesvh.cn/Article/details/gxjweamsu.sHtML

SELECT * FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gxpsattqc.sHtML

[Q16] 查询指定列
来源：http://blog.hesvh.cn/Article/details/ghxinvzam.sHtML

SELECT id, name FROM users;
来源：http://3g.zdbjq.cn/Article/details/gsmnvorfl.sHtML

[Q17] 条件查询
来源：http://3g.hesvh.cn/Article/details/gdtncjfqw.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://blog.hesvh.cn/Article/details/gtdpbrxkz.sHtML

[Q18] 模糊匹配
来源：http://mobile.hesvh.cn/Article/details/gptjtmhck.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://blog.zdbjq.cn/Article/details/grjchifjs.sHtML

[Q19] 范围查询
来源：http://baike.fehbvm.com/Article/details/guknnrarp.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://baike.hesvh.cn/Article/details/gvbizxohc.sHtML

[Q20] IN 列表
来源：http://read.share.hesvh.cn/Article/details/gungzchyx.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://3g.zdbjq.cn/Article/details/gsluebbiy.sHtML

[Q21] 空值判断
来源：http://baike.zdbjq.cn/Article/details/glkelzcfk.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.share.zdbjq.cn/Article/details/gqhdwrxxx.sHtML

[Q22] 排序
来源：http://wap.hesvh.cn/Article/details/gtsfdgdrq.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://m.share.hesvh.cn/Article/details/grzudgrzo.sHtML

[Q23] 分页
来源：http://baike.zdbjq.cn/Article/details/ggfshalcr.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.blog.fehbvm.com/Article/details/gdydwpzyj.sHtML

[Q24] 去重
来源：http://3g.hesvh.cn/Article/details/ggtbwphrb.sHtML

SELECT DISTINCT city FROM users;
来源：http://blog.fehbvm.com/Article/details/gzjkddgcc.sHtML

[Q25] 只取前 N 条
来源：http://blog.fehbvm.com/Article/details/gurslrkmj.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://3g.fehbvm.com/Article/details/gbzgjecdy.sHtML

[Q26] 计数
来源：http://blog.hesvh.cn/Article/details/gupoyecij.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/ggzvwhios.sHtML

[Q27] 条件计数
来源：http://3g.zdbjq.cn/Article/details/gpaoihara.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gabzqbgjj.sHtML

[Q28] 求和与平均
来源：http://mobile.zdbjq.cn/Article/details/gtfooazyf.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://3g.hesvh.cn/Article/details/gpzyrcrbz.sHtML

[Q29] 最大最小值
来源：http://baike.zdbjq.cn/Article/details/glewbsbrh.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://blog.fehbvm.com/Article/details/grtmpjggn.sHtML

[Q30] 分组统计
来源：http://m.share.hesvh.cn/Article/details/gubtyigev.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://baike.fehbvm.com/Article/details/gebtcsqfq.sHtML

[Q31] 分组后过滤
来源：http://3g.hesvh.cn/Article/details/gzpxzinwx.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.blog.fehbvm.com/Article/details/gfxdrpfve.sHtML

[Q32] 分组拼接字符串
来源：http://read.share.fehbvm.com/Article/details/gmsslildr.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://mobile.zdbjq.cn/Article/details/gigayieul.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.blog.zdbjq.cn/Article/details/gexxcjfmc.sHtML

[Q33] 多列分组
来源：http://www.share.fehbvm.com/Article/details/gqisbhxis.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://baike.hesvh.cn/Article/details/ggmwdadeh.sHtML

[Q34] 每组取第一条
来源：http://www.m.share.hesvh.cn/Article/details/gitnnjptf.sHtML

SELECT * FROM (
来源：http://wap.fehbvm.com/Article/details/gosjeiwwz.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.share.fehbvm.com/Article/details/gyhqgvuhg.sHtML

) t WHERE rn = 1;
来源：http://www.share.hesvh.cn/Article/details/gzujejblv.sHtML

[Q35] 内连接
来源：http://www.share.hesvh.cn/Article/details/gwnrnnncu.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://baike.hesvh.cn/Article/details/gfzisjajs.sHtML

[Q36] 左连接
来源：http://www.blog.hesvh.cn/Article/details/guyivdcvh.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://baike.fehbvm.com/Article/details/gapttofrl.sHtML

[Q37] 右连接
来源：http://3g.zdbjq.cn/Article/details/gvayndyfl.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://3g.fehbvm.com/Article/details/glnidguca.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://baike.fehbvm.com/Article/details/gfyoretob.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://wap.hesvh.cn/Article/details/garttnfwr.sHtML

[Q39] 自连接（查上下级）
来源：http://3g.fehbvm.com/Article/details/gzqspuemo.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.share.hesvh.cn/Article/details/gogpdjrqs.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.m.share.zdbjq.cn/Article/details/gxsabueaf.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://baike.zdbjq.cn/Article/details/gnkimzcxj.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.m.share.fehbvm.com/Article/details/gaapytewj.sHtML

[Q41] 多表连接
来源：http://www.blog.fehbvm.com/Article/details/gbxripejb.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.share.fehbvm.com/Article/details/gnpfkkluz.sHtML

JOIN users u ON u.id = o.user_id
来源：http://wap.fehbvm.com/Article/details/gvxklksuu.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://blog.hesvh.cn/Article/details/gcnxxukho.sHtML

[Q42] 连接条件附加过滤
来源：http://baike.fehbvm.com/Article/details/gvyvpjmpr.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.m.share.fehbvm.com/Article/details/gcpdekhva.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://m.share.zdbjq.cn/Article/details/gbryuignh.sHtML

[Q43] 标量子查询
来源：http://mobile.hesvh.cn/Article/details/ghptubuqp.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://read.share.hesvh.cn/Article/details/gzpvgyjxf.sHtML

[Q44] IN 子查询
来源：http://3g.fehbvm.com/Article/details/gzfjobqta.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://mobile.fehbvm.com/Article/details/gnbjnzuar.sHtML

[Q45] EXISTS 判断存在
来源：http://blog.fehbvm.com/Article/details/gvtsoapcu.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.hesvh.cn/Article/details/grgtjnqab.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://m.share.zdbjq.cn/Article/details/gnbqyeoef.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.hesvh.cn/Article/details/gbzrictad.sHtML

[Q47] 与平均值比较
来源：http://www.blog.hesvh.cn/Article/details/gaermkqej.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.share.hesvh.cn/Article/details/gsemyqkfc.sHtML

[Q48] CTE 公用表表达式
来源：http://baike.hesvh.cn/Article/details/gdxiawerd.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://mobile.hesvh.cn/Article/details/gvmzzxbvt.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://mobile.hesvh.cn/Article/details/girroukru.sHtML

[Q49] 更新单行
来源：http://3g.hesvh.cn/Article/details/gymbsercw.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://blog.zdbjq.cn/Article/details/gyzcvalhq.sHtML

[Q50] 批量更新
来源：http://wap.zdbjq.cn/Article/details/gyncmzsly.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.share.hesvh.cn/Article/details/gcwjerhyk.sHtML

[Q51] 用子查询更新
来源：http://www.blog.zdbjq.cn/Article/details/ggauktzem.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://baike.fehbvm.com/Article/details/gykixzinn.sHtML

[Q52] 删除指定行
来源：http://wap.zdbjq.cn/Article/details/gtqlvjojz.sHtML

DELETE FROM users WHERE id = 10;
来源：http://read.share.zdbjq.cn/Article/details/gtscdxfeg.sHtML

[Q53] 按条件删除
来源：http://read.share.fehbvm.com/Article/details/gqglxtamm.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://read.share.hesvh.cn/Article/details/gqvftwzhr.sHtML

[Q54] 清空表
来源：http://www.m.share.fehbvm.com/Article/details/gvqkvpeip.sHtML

TRUNCATE TABLE logs;
来源：http://3g.zdbjq.cn/Article/details/gbyilclpc.sHtML

[Q55] 排名（并列占位）
来源：http://blog.zdbjq.cn/Article/details/gnwmxjcko.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.share.fehbvm.com/Article/details/grzkjklfe.sHtML

[Q56] 密集排名（并列不占位）
来源：http://blog.hesvh.cn/Article/details/gszsblplj.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://wap.zdbjq.cn/Article/details/gxhhcwpsr.sHtML

[Q57] 行号
来源：http://read.share.zdbjq.cn/Article/details/gzxmmiezt.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://baike.hesvh.cn/Article/details/gdavqkyna.sHtML

[Q58] 累计求和
来源：http://read.share.zdbjq.cn/Article/details/glcxggcwy.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://3g.hesvh.cn/Article/details/glvltomxh.sHtML

[Q59] 分组内累计
来源：http://blog.zdbjq.cn/Article/details/gjxqgqnkr.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://blog.hesvh.cn/Article/details/gavmmpqop.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.share.zdbjq.cn/Article/details/gzyvyxpbk.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://read.share.hesvh.cn/Article/details/gfsvunnys.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.m.share.zdbjq.cn/Article/details/glgxbqcsr.sHtML

[Q61] 移动平均
来源：http://mobile.hesvh.cn/Article/details/gvbqhihol.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://mobile.fehbvm.com/Article/details/gstrosyzo.sHtML

[Q62] 分组占比
来源：http://mobile.hesvh.cn/Article/details/gxllxbigu.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://3g.zdbjq.cn/Article/details/gcbqfjweg.sHtML

[Q63] 开启事务
来源：http://wap.hesvh.cn/Article/details/grojjvdah.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://mobile.hesvh.cn/Article/details/ggnzdzqos.sHtML

[Q64] 提交事务
来源：http://blog.fehbvm.com/Article/details/gxqgyndac.sHtML

COMMIT;
来源：http://3g.fehbvm.com/Article/details/goxdlnkiw.sHtML

[Q65] 回滚事务
来源：http://3g.zdbjq.cn/Article/details/gmaamtrwn.sHtML

ROLLBACK;
来源：http://3g.zdbjq.cn/Article/details/gzlcwndtw.sHtML

[Q66] 行锁查询
来源：http://www.m.share.hesvh.cn/Article/details/gzltxobbl.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.m.share.fehbvm.com/Article/details/gnspologc.sHtML

[Q67] 设置隔离级别
来源：http://mobile.zdbjq.cn/Article/details/gkvjooxdc.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://read.share.hesvh.cn/Article/details/gsscwcmqc.sHtML

[Q68] 保存点
来源：http://blog.hesvh.cn/Article/details/gwmwjslev.sHtML

SAVEPOINT sp1;
来源：http://blog.hesvh.cn/Article/details/gcxxfrcjz.sHtML

ROLLBACK TO sp1;
来源：http://read.share.hesvh.cn/Article/details/glkmldgia.sHtML

[Q69] 查看执行计划
来源：http://www.m.share.hesvh.cn/Article/details/gxviktrpz.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://3g.hesvh.cn/Article/details/gtuyndpwu.sHtML

[Q70] 更新统计信息
来源：http://blog.fehbvm.com/Article/details/gshkphamz.sHtML

ANALYZE TABLE users;
来源：http://read.share.hesvh.cn/Article/details/gstrjldmn.sHtML

[Q71] 查看建表语句
来源：http://mobile.fehbvm.com/Article/details/gnollkbyi.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://baike.fehbvm.com/Article/details/ggqqbprxf.sHtML

[Q72] 查看索引
来源：http://www.blog.zdbjq.cn/Article/details/gxjeicdbw.sHtML

SHOW INDEX FROM users;
来源：http://mobile.fehbvm.com/Article/details/gohquvsnw.sHtML

[Q73] 查看表状态
来源：http://blog.fehbvm.com/Article/details/grluzguqi.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.blog.fehbvm.com/Article/details/gmzxkmpmn.sHtML

[Q74] 强制使用索引
来源：http://wap.hesvh.cn/Article/details/gkczlvvno.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://3g.zdbjq.cn/Article/details/grlsxtplc.sHtML

[Q75] 日期格式化
来源：http://read.share.zdbjq.cn/Article/details/gopgsyrdx.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://mobile.zdbjq.cn/Article/details/gnuikrqpw.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.share.hesvh.cn/Article/details/gwxgpaebl.sHtML

[Q76] 按天统计
来源：http://m.share.fehbvm.com/Article/details/gsexcnzig.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://baike.hesvh.cn/Article/details/gzloztuan.sHtML

[Q77] 时间加减
来源：http://m.share.zdbjq.cn/Article/details/gzlwbbeza.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.m.share.hesvh.cn/Article/details/gdbtldlnp.sHtML

[Q78] 当前时间
来源：http://blog.zdbjq.cn/Article/details/gvamlsiin.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://3g.zdbjq.cn/Article/details/gcwufajpm.sHtML

[Q79] 字符串拼接
来源：http://m.share.fehbvm.com/Article/details/giucugrhu.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://mobile.zdbjq.cn/Article/details/gtjcmhgnm.sHtML

[Q80] 字符串截取
来源：http://www.blog.fehbvm.com/Article/details/gqqnvjien.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gdvdqrmfh.sHtML

[Q81] 字符串替换
来源：http://read.share.hesvh.cn/Article/details/gelxjidre.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gnfralzti.sHtML

[Q82] 字符长度与字节长度
来源：http://www.blog.zdbjq.cn/Article/details/gcazxhugd.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://baike.fehbvm.com/Article/details/gcxybroeh.sHtML

[Q83] 大小写转换
来源：http://www.share.hesvh.cn/Article/details/grhrmpbwf.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://3g.zdbjq.cn/Article/details/gfgyievzu.sHtML

[Q84] 去除首尾空格
来源：http://baike.hesvh.cn/Article/details/gbjdbymdc.sHtML

SELECT TRIM(name) FROM users;
来源：http://baike.fehbvm.com/Article/details/gdtxpxsnv.sHtML

[Q85] 数值取整
来源：http://mobile.zdbjq.cn/Article/details/gocjpvime.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://3g.fehbvm.com/Article/details/gmfqtvjpy.sHtML

[Q86] 读取 JSON 字段
来源：http://www.share.zdbjq.cn/Article/details/gauddqjty.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://wap.fehbvm.com/Article/details/gypdsxbul.sHtML

[Q87] JSON 字段做条件
来源：http://www.share.zdbjq.cn/Article/details/gyshpkvpy.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.blog.hesvh.cn/Article/details/geuhhgrsg.sHtML

[Q88] 行转列（条件聚合）
来源：http://blog.hesvh.cn/Article/details/gujliftgp.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.blog.hesvh.cn/Article/details/gzvtlawdf.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://m.share.fehbvm.com/Article/details/glufpsfxw.sHtML

[Q89] 判断表是否存在
来源：http://m.share.fehbvm.com/Article/details/gagqqputh.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://3g.fehbvm.com/Article/details/goxznfapt.sHtML

[Q90] 生成序号列
来源：http://mobile.hesvh.cn/Article/details/gahjkcxay.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.share.fehbvm.com/Article/details/gnpxyvenf.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/galtfvhaz.sHtML

R. Bash 专题
来源：http://blog.fehbvm.com/Article/details/gmtltshqv.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/ggvvjpzfi.sHtML

[R01] shebang 与严格模式
来源：http://wap.zdbjq.cn/Article/details/gkcjbamja.sHtML

#!/usr/bin/env bash
来源：http://wap.hesvh.cn/Article/details/gdwjdlkwp.sHtML

set -euo pipefail
来源：http://read.share.fehbvm.com/Article/details/gemfbesbn.sHtML

[R02] 变量赋值与使用
来源：http://www.share.fehbvm.com/Article/details/gczcbajln.sHtML

name="Tom"; echo "$name"
来源：http://wap.hesvh.cn/Article/details/gsdjqlovx.sHtML

[R03] 只读变量
来源：http://mobile.zdbjq.cn/Article/details/gtjmxiisj.sHtML

readonly PI=3.14
来源：http://read.share.fehbvm.com/Article/details/gymjfxqiz.sHtML

[R04] 位置参数
来源：http://baike.fehbvm.com/Article/details/gtfpcrzdh.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.share.fehbvm.com/Article/details/gjhxpjgll.sHtML

[R05] 参数默认值
来源：http://baike.hesvh.cn/Article/details/givmmewoh.sHtML

name="${1:-default}"
来源：http://m.share.zdbjq.cn/Article/details/ghaehwyph.sHtML

[R06] 判断命令是否存在
来源：http://blog.fehbvm.com/Article/details/gxnyiaeqz.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://3g.zdbjq.cn/Article/details/glzgajkvj.sHtML

[R07] if 判断文件
来源：http://www.share.fehbvm.com/Article/details/gqqfukuhw.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.m.share.zdbjq.cn/Article/details/gdmfpufbk.sHtML

[R08] 数值比较
来源：http://m.share.fehbvm.com/Article/details/gbwfgenyy.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.blog.zdbjq.cn/Article/details/gacnxyuqp.sHtML

[R09] 字符串比较
来源：http://blog.zdbjq.cn/Article/details/gysxbojup.sHtML


<!-- 参考信息 -->