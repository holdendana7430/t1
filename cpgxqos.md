代发 wailian999

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://3g.hesvh.cn/Article/details/gqkjlatxq.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://read.share.zdbjq.cn/Article/details/gsotucubm.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://m.share.fehbvm.com/Article/details/gxokrhmov.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://wap.fehbvm.com/Article/details/gvntjlrha.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://read.share.fehbvm.com/Article/details/gkryepkod.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://read.share.zdbjq.cn/Article/details/gfdzgrdxs.sHtML

[P03] 生成短随机字符串
来源：http://3g.zdbjq.cn/Article/details/gffzyfzvq.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://blog.zdbjq.cn/Article/details/giwgsbjpa.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://wap.hesvh.cn/Article/details/gmrktqhjy.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.fehbvm.com/Article/details/gjjcueflc.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://3g.fehbvm.com/Article/details/gthkfqtiq.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://m.share.zdbjq.cn/Article/details/gbqjeqttd.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://baike.zdbjq.cn/Article/details/gvbfviwmx.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://m.share.fehbvm.com/Article/details/gnhruipvd.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.blog.fehbvm.com/Article/details/gvlhxyolv.sHtML

[P04] 求长度
来源：http://m.share.hesvh.cn/Article/details/glhjdttjp.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.share.zdbjq.cn/Article/details/girpwgsha.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.zdbjq.cn/Article/details/gqxemhmwe.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.zdbjq.cn/Article/details/goexpsuxb.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.zdbjq.cn/Article/details/gcoqfzvdm.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.share.fehbvm.com/Article/details/gvwgqhzgq.sHtML

Go:   len(arr);  len(m)
来源：http://3g.hesvh.cn/Article/details/gjmarzpkd.sHtML

Ruby: x.length;  x.size
来源：http://www.share.fehbvm.com/Article/details/gyqxgrmwf.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://baike.hesvh.cn/Article/details/gyhebvxvn.sHtML

[P05] 判断两个对象内容是否相等
来源：http://read.share.hesvh.cn/Article/details/gxpqwvkfh.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://m.share.fehbvm.com/Article/details/gwellxvoj.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://wap.fehbvm.com/Article/details/ginkhklgh.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.m.share.zdbjq.cn/Article/details/gsagrczgb.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.hesvh.cn/Article/details/gblscckkj.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.share.hesvh.cn/Article/details/gvwvkuqaj.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.share.hesvh.cn/Article/details/gxfldfpvr.sHtML

Ruby: a == b
来源：http://wap.fehbvm.com/Article/details/gmlnmttyi.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://read.share.fehbvm.com/Article/details/ghlxtyraw.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://blog.hesvh.cn/Article/details/gbmkvcbtt.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.m.share.zdbjq.cn/Article/details/gencptdpk.sHtML

PHP:  if (empty($x)) {}
来源：http://baike.zdbjq.cn/Article/details/gsadzlvlk.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.share.zdbjq.cn/Article/details/gzfccanjk.sHtML

TS:   if (x == null) {}
来源：http://baike.hesvh.cn/Article/details/ggtukfsgw.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://blog.hesvh.cn/Article/details/gwshblfzz.sHtML

Go:   if x == nil {}
来源：http://wap.zdbjq.cn/Article/details/gpqwdxtlq.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.m.share.hesvh.cn/Article/details/gbtkrmcyh.sHtML

C#:   if (x is null) {}
来源：http://m.share.zdbjq.cn/Article/details/gqsjbrgyl.sHtML

[P07] 防抖与节流
来源：http://m.share.fehbvm.com/Article/details/gbzybtioo.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.m.share.hesvh.cn/Article/details/gfwhgokuk.sHtML

PHP:  // 手写时间戳比较
来源：http://www.share.zdbjq.cn/Article/details/gfacfvdxs.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.fehbvm.com/Article/details/goglvqnso.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.zdbjq.cn/Article/details/gonsmgraa.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://mobile.hesvh.cn/Article/details/gsimftqua.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.m.share.zdbjq.cn/Article/details/gbpmvoope.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://mobile.fehbvm.com/Article/details/gyqigerpq.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://3g.hesvh.cn/Article/details/glxoiwwnp.sHtML

[P08] 处理浮点精度问题
来源：http://baike.zdbjq.cn/Article/details/ggcuuxunt.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://blog.fehbvm.com/Article/details/gzmmmefpl.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://3g.fehbvm.com/Article/details/gkgfjahxt.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://baike.hesvh.cn/Article/details/gijgludaz.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://wap.fehbvm.com/Article/details/gptitdaje.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://m.share.hesvh.cn/Article/details/gedglrqov.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://read.share.hesvh.cn/Article/details/ggpyextnq.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://3g.hesvh.cn/Article/details/gjvqcthvv.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://mobile.zdbjq.cn/Article/details/glylgupgk.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gsmbcythc.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.share.fehbvm.com/Article/details/gkxdjjgku.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gaizpxpua.sHtML

[Q01] 创建表
来源：http://www.blog.hesvh.cn/Article/details/gafxefomu.sHtML

CREATE TABLE users (
来源：http://www.m.share.zdbjq.cn/Article/details/gdlpmrrfy.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.zdbjq.cn/Article/details/gyiaktegl.sHtML

name VARCHAR(50) NOT NULL,
来源：http://read.share.hesvh.cn/Article/details/grlfwwjvx.sHtML

email VARCHAR(100) UNIQUE,
来源：http://baike.fehbvm.com/Article/details/giwewfgiz.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://3g.zdbjq.cn/Article/details/glmwslqkm.sHtML

);
来源：http://wap.hesvh.cn/Article/details/greriyjwt.sHtML

[Q02] 创建带外键的表
来源：http://m.share.fehbvm.com/Article/details/gpqxtcioe.sHtML

CREATE TABLE orders (
来源：http://www.share.hesvh.cn/Article/details/gxfeuqtre.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.hesvh.cn/Article/details/gbyyckxmz.sHtML

user_id INT NOT NULL,
来源：http://3g.hesvh.cn/Article/details/gncwystaf.sHtML

amount DECIMAL(10, 2),
来源：http://blog.fehbvm.com/Article/details/gineagtvx.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.m.share.hesvh.cn/Article/details/goqsqvxan.sHtML

);
来源：http://mobile.zdbjq.cn/Article/details/gxnybzyit.sHtML

[Q03] 增加列
来源：http://www.blog.fehbvm.com/Article/details/gbvpdezge.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://wap.zdbjq.cn/Article/details/guuqflxbr.sHtML

[Q04] 修改列类型
来源：http://baike.zdbjq.cn/Article/details/gvlpdgphj.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://mobile.fehbvm.com/Article/details/gmbmrkcnt.sHtML

[Q05] 重命名列
来源：http://www.m.share.fehbvm.com/Article/details/gzzcqmvky.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.m.share.zdbjq.cn/Article/details/gizozmsbj.sHtML

[Q06] 删除列
来源：http://www.blog.hesvh.cn/Article/details/grrblzqzw.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.share.fehbvm.com/Article/details/ghlyhnhga.sHtML

[Q07] 删除表
来源：http://m.share.zdbjq.cn/Article/details/grgcioqpn.sHtML

DROP TABLE IF EXISTS orders;
来源：http://blog.hesvh.cn/Article/details/gkytatobs.sHtML

[Q08] 创建普通索引
来源：http://www.blog.zdbjq.cn/Article/details/greosswid.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://wap.fehbvm.com/Article/details/gazvnymrp.sHtML

[Q09] 创建唯一索引
来源：http://www.m.share.hesvh.cn/Article/details/giogvlibp.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://baike.zdbjq.cn/Article/details/gapiiyqfy.sHtML

[Q10] 插入单行
来源：http://www.m.share.hesvh.cn/Article/details/gczkfjjai.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://mobile.zdbjq.cn/Article/details/gorbfenkr.sHtML

[Q11] 一次插入多行
来源：http://mobile.hesvh.cn/Article/details/gqdkiobrg.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://baike.zdbjq.cn/Article/details/gijaoyjeb.sHtML

[Q12] 插入后取自增 ID
来源：http://wap.fehbvm.com/Article/details/gqubwtkbp.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://blog.zdbjq.cn/Article/details/getpwggre.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.blog.zdbjq.cn/Article/details/grhxdmcro.sHtML

[Q13] 忽略重复插入
来源：http://wap.hesvh.cn/Article/details/gmrhoxesg.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://wap.zdbjq.cn/Article/details/gotwalcyq.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.blog.hesvh.cn/Article/details/gppundmwe.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://read.share.fehbvm.com/Article/details/geqdgytqz.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://3g.fehbvm.com/Article/details/gelvamvos.sHtML

[Q15] 查询全部
来源：http://www.blog.zdbjq.cn/Article/details/gazwarniz.sHtML

SELECT * FROM users;
来源：http://m.share.hesvh.cn/Article/details/gzzauxcgs.sHtML

[Q16] 查询指定列
来源：http://m.share.zdbjq.cn/Article/details/gcscbhxhc.sHtML

SELECT id, name FROM users;
来源：http://baike.zdbjq.cn/Article/details/gtixhvsav.sHtML

[Q17] 条件查询
来源：http://wap.fehbvm.com/Article/details/gvwkvkucu.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://m.share.hesvh.cn/Article/details/gasytpvdx.sHtML

[Q18] 模糊匹配
来源：http://wap.fehbvm.com/Article/details/gzneymfqs.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://baike.zdbjq.cn/Article/details/gjspyihix.sHtML

[Q19] 范围查询
来源：http://blog.zdbjq.cn/Article/details/ghvjjnhey.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.share.hesvh.cn/Article/details/gtidpsfic.sHtML

[Q20] IN 列表
来源：http://mobile.zdbjq.cn/Article/details/gjerpkfqf.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://3g.hesvh.cn/Article/details/gjitbfehl.sHtML

[Q21] 空值判断
来源：http://m.share.zdbjq.cn/Article/details/gkmdefagw.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://wap.zdbjq.cn/Article/details/gkxabsucg.sHtML

[Q22] 排序
来源：http://www.m.share.fehbvm.com/Article/details/gwkuvfjid.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.share.zdbjq.cn/Article/details/glfmtvgwe.sHtML

[Q23] 分页
来源：http://www.blog.fehbvm.com/Article/details/ghhppluds.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.share.hesvh.cn/Article/details/gmmzrygdm.sHtML

[Q24] 去重
来源：http://wap.zdbjq.cn/Article/details/gdmbdtaqi.sHtML

SELECT DISTINCT city FROM users;
来源：http://m.share.zdbjq.cn/Article/details/guozrvybq.sHtML

[Q25] 只取前 N 条
来源：http://www.blog.fehbvm.com/Article/details/gnpszckmd.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://m.share.zdbjq.cn/Article/details/gepwgdpok.sHtML

[Q26] 计数
来源：http://wap.fehbvm.com/Article/details/gojpbhaju.sHtML

SELECT COUNT(*) FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gpumyfvjh.sHtML

[Q27] 条件计数
来源：http://read.share.zdbjq.cn/Article/details/gwxhkhgra.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://3g.hesvh.cn/Article/details/gzulpcstg.sHtML

[Q28] 求和与平均
来源：http://baike.fehbvm.com/Article/details/gqgxwkbso.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://3g.hesvh.cn/Article/details/gapubwiqv.sHtML

[Q29] 最大最小值
来源：http://read.share.fehbvm.com/Article/details/ggexomudi.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gplszadta.sHtML

[Q30] 分组统计
来源：http://www.blog.zdbjq.cn/Article/details/glptuqxca.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://read.share.fehbvm.com/Article/details/gxwgnokwx.sHtML

[Q31] 分组后过滤
来源：http://3g.zdbjq.cn/Article/details/gpdavhzpz.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://mobile.fehbvm.com/Article/details/gsagjlbgc.sHtML

[Q32] 分组拼接字符串
来源：http://wap.hesvh.cn/Article/details/gqtvossmq.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://mobile.fehbvm.com/Article/details/gwbongjao.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://baike.zdbjq.cn/Article/details/gkftimkoh.sHtML

[Q33] 多列分组
来源：http://mobile.zdbjq.cn/Article/details/gtgqabrei.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://read.share.fehbvm.com/Article/details/gbunucnaj.sHtML

[Q34] 每组取第一条
来源：http://mobile.zdbjq.cn/Article/details/gwnwettwl.sHtML

SELECT * FROM (
来源：http://m.share.hesvh.cn/Article/details/gyzgfuowr.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://wap.fehbvm.com/Article/details/grrjjcimn.sHtML

) t WHERE rn = 1;
来源：http://read.share.hesvh.cn/Article/details/ghqvgfwmn.sHtML

[Q35] 内连接
来源：http://wap.hesvh.cn/Article/details/guuggokia.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.zdbjq.cn/Article/details/gwzfeuyuu.sHtML

[Q36] 左连接
来源：http://www.share.zdbjq.cn/Article/details/gglbhpnns.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://mobile.hesvh.cn/Article/details/gkhzylglb.sHtML

[Q37] 右连接
来源：http://blog.hesvh.cn/Article/details/gulxnmyxd.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.blog.zdbjq.cn/Article/details/gkqrsnpnh.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://3g.hesvh.cn/Article/details/gutbyvwco.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://mobile.zdbjq.cn/Article/details/gmetwrckr.sHtML

[Q39] 自连接（查上下级）
来源：http://m.share.hesvh.cn/Article/details/glifrslis.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://m.share.hesvh.cn/Article/details/gpiqkytml.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://3g.fehbvm.com/Article/details/gxeovhoqc.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://mobile.hesvh.cn/Article/details/ghmlkwsrn.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://baike.zdbjq.cn/Article/details/gyxzlbnko.sHtML

[Q41] 多表连接
来源：http://blog.zdbjq.cn/Article/details/gynbexkrg.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://mobile.hesvh.cn/Article/details/gmaksnupq.sHtML

JOIN users u ON u.id = o.user_id
来源：http://read.share.hesvh.cn/Article/details/gijjzybti.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.m.share.fehbvm.com/Article/details/gnbbdvdfj.sHtML

[Q42] 连接条件附加过滤
来源：http://m.share.fehbvm.com/Article/details/gcpbsygqd.sHtML

SELECT u.name, o.amount FROM users u
来源：http://read.share.hesvh.cn/Article/details/gxumjmfmj.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.share.hesvh.cn/Article/details/gzsdzgrnj.sHtML

[Q43] 标量子查询
来源：http://www.blog.zdbjq.cn/Article/details/gtqzpmeil.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://wap.zdbjq.cn/Article/details/gwgoclrze.sHtML

[Q44] IN 子查询
来源：http://www.blog.fehbvm.com/Article/details/gtuztgirp.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.share.hesvh.cn/Article/details/gwiualalr.sHtML

[Q45] EXISTS 判断存在
来源：http://baike.zdbjq.cn/Article/details/gakipvcdh.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.zdbjq.cn/Article/details/gjunxwidz.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://mobile.fehbvm.com/Article/details/gjsxqnsri.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.hesvh.cn/Article/details/ghzdzqhzz.sHtML

[Q47] 与平均值比较
来源：http://blog.hesvh.cn/Article/details/gamdzajyd.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://3g.fehbvm.com/Article/details/gudbvtmqm.sHtML

[Q48] CTE 公用表表达式
来源：http://wap.zdbjq.cn/Article/details/grmxkxizy.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://3g.fehbvm.com/Article/details/gyefpdtwk.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://blog.fehbvm.com/Article/details/ggbthwxop.sHtML

[Q49] 更新单行
来源：http://m.share.fehbvm.com/Article/details/gavhuzkpq.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://blog.hesvh.cn/Article/details/gwzxyzwdl.sHtML

[Q50] 批量更新
来源：http://www.blog.zdbjq.cn/Article/details/gguttpqzs.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.blog.fehbvm.com/Article/details/guujzxozt.sHtML

[Q51] 用子查询更新
来源：http://read.share.fehbvm.com/Article/details/gnwlxzmds.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://m.share.hesvh.cn/Article/details/gvaedvdbq.sHtML

[Q52] 删除指定行
来源：http://m.share.zdbjq.cn/Article/details/geqdyrupu.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.share.fehbvm.com/Article/details/gfyrpfejn.sHtML

[Q53] 按条件删除
来源：http://www.m.share.zdbjq.cn/Article/details/gkozekbax.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://mobile.hesvh.cn/Article/details/grkbkqwpc.sHtML

[Q54] 清空表
来源：http://read.share.zdbjq.cn/Article/details/gpbxlxxae.sHtML

TRUNCATE TABLE logs;
来源：http://www.share.zdbjq.cn/Article/details/gmaisdmjd.sHtML

[Q55] 排名（并列占位）
来源：http://m.share.fehbvm.com/Article/details/gnucujwzd.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.share.zdbjq.cn/Article/details/ghmvqswgy.sHtML

[Q56] 密集排名（并列不占位）
来源：http://3g.fehbvm.com/Article/details/gsztuoicg.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.m.share.fehbvm.com/Article/details/gjnknajzu.sHtML

[Q57] 行号
来源：http://baike.fehbvm.com/Article/details/gswgpqkhx.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://wap.zdbjq.cn/Article/details/gfpuqrekg.sHtML

[Q58] 累计求和
来源：http://read.share.fehbvm.com/Article/details/gxxftkccq.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://m.share.zdbjq.cn/Article/details/gwfanxlph.sHtML

[Q59] 分组内累计
来源：http://m.share.zdbjq.cn/Article/details/gztahvfyq.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://wap.hesvh.cn/Article/details/gjugplvyh.sHtML

[Q60] 取上一行 / 下一行
来源：http://blog.fehbvm.com/Article/details/giupcbmza.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://mobile.hesvh.cn/Article/details/ggoimbzez.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://m.share.hesvh.cn/Article/details/gvtwbztwu.sHtML

[Q61] 移动平均
来源：http://blog.zdbjq.cn/Article/details/gfxschjoi.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://wap.fehbvm.com/Article/details/gmhyimtlh.sHtML

[Q62] 分组占比
来源：http://mobile.fehbvm.com/Article/details/gqjuowbgk.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.m.share.fehbvm.com/Article/details/gbildqbiv.sHtML

[Q63] 开启事务
来源：http://3g.zdbjq.cn/Article/details/gziuhavpb.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.blog.hesvh.cn/Article/details/gfhluqasc.sHtML

[Q64] 提交事务
来源：http://read.share.zdbjq.cn/Article/details/gsnkgonqt.sHtML

COMMIT;
来源：http://read.share.hesvh.cn/Article/details/gfchhtkee.sHtML

[Q65] 回滚事务
来源：http://www.share.fehbvm.com/Article/details/grdoycdnc.sHtML

ROLLBACK;
来源：http://blog.fehbvm.com/Article/details/gzdhwucre.sHtML

[Q66] 行锁查询
来源：http://www.blog.fehbvm.com/Article/details/guysodddb.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://wap.fehbvm.com/Article/details/gjagzgxxd.sHtML

[Q67] 设置隔离级别
来源：http://read.share.fehbvm.com/Article/details/gfsytjxlx.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://baike.zdbjq.cn/Article/details/gxkzncuyb.sHtML

[Q68] 保存点
来源：http://read.share.fehbvm.com/Article/details/gmcicezrl.sHtML

SAVEPOINT sp1;
来源：http://3g.hesvh.cn/Article/details/gnfpjbkdm.sHtML

ROLLBACK TO sp1;
来源：http://baike.fehbvm.com/Article/details/gzqyncubo.sHtML

[Q69] 查看执行计划
来源：http://www.share.hesvh.cn/Article/details/gwvpimsqp.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://baike.fehbvm.com/Article/details/gdnsremyc.sHtML

[Q70] 更新统计信息
来源：http://www.m.share.fehbvm.com/Article/details/gpwpyrafj.sHtML

ANALYZE TABLE users;
来源：http://wap.zdbjq.cn/Article/details/gldyyvcij.sHtML

[Q71] 查看建表语句
来源：http://blog.hesvh.cn/Article/details/gcsbanfrd.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://wap.hesvh.cn/Article/details/gtecwoitc.sHtML

[Q72] 查看索引
来源：http://baike.hesvh.cn/Article/details/govqgeuzp.sHtML

SHOW INDEX FROM users;
来源：http://blog.hesvh.cn/Article/details/gkoffchmd.sHtML

[Q73] 查看表状态
来源：http://www.blog.zdbjq.cn/Article/details/gowslpyox.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://blog.hesvh.cn/Article/details/glyhtnjhl.sHtML

[Q74] 强制使用索引
来源：http://wap.hesvh.cn/Article/details/gcdffcjrw.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.m.share.zdbjq.cn/Article/details/gqdfcfozr.sHtML

[Q75] 日期格式化
来源：http://wap.zdbjq.cn/Article/details/goyarjoiv.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.blog.fehbvm.com/Article/details/ghhbvfnsl.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://m.share.fehbvm.com/Article/details/gxlbkhjqk.sHtML

[Q76] 按天统计
来源：http://m.share.hesvh.cn/Article/details/ghnzkapzy.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.blog.zdbjq.cn/Article/details/gmihjjxez.sHtML

[Q77] 时间加减
来源：http://mobile.fehbvm.com/Article/details/gfdpbhgmq.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://baike.hesvh.cn/Article/details/gsbentsln.sHtML

[Q78] 当前时间
来源：http://www.share.zdbjq.cn/Article/details/gojjgjgjt.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://read.share.fehbvm.com/Article/details/gnoksmsac.sHtML

[Q79] 字符串拼接
来源：http://www.blog.zdbjq.cn/Article/details/gcouamcqk.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://m.share.zdbjq.cn/Article/details/gallygjse.sHtML

[Q80] 字符串截取
来源：http://mobile.zdbjq.cn/Article/details/gjftdkrpy.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gyfvlklvo.sHtML

[Q81] 字符串替换
来源：http://blog.fehbvm.com/Article/details/gjtrsyclh.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://3g.zdbjq.cn/Article/details/gwvsdfyus.sHtML

[Q82] 字符长度与字节长度
来源：http://mobile.zdbjq.cn/Article/details/gujrysmrz.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.blog.hesvh.cn/Article/details/guvolmzps.sHtML

[Q83] 大小写转换
来源：http://baike.zdbjq.cn/Article/details/gpyoxnurp.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://3g.zdbjq.cn/Article/details/ggmadullx.sHtML

[Q84] 去除首尾空格
来源：http://www.share.fehbvm.com/Article/details/glpbihgob.sHtML

SELECT TRIM(name) FROM users;
来源：http://read.share.fehbvm.com/Article/details/grjywbeos.sHtML

[Q85] 数值取整
来源：http://wap.zdbjq.cn/Article/details/gxujoaekh.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://blog.hesvh.cn/Article/details/gawaqsdgu.sHtML

[Q86] 读取 JSON 字段
来源：http://www.share.hesvh.cn/Article/details/gwptepjbs.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://m.share.hesvh.cn/Article/details/gdixxkugi.sHtML

[Q87] JSON 字段做条件
来源：http://www.m.share.fehbvm.com/Article/details/gaabpkaga.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://blog.fehbvm.com/Article/details/grbbsyqjh.sHtML

[Q88] 行转列（条件聚合）
来源：http://3g.zdbjq.cn/Article/details/gbgvosywo.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://baike.zdbjq.cn/Article/details/golkbnfcm.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://mobile.hesvh.cn/Article/details/gfjhgqrdg.sHtML

[Q89] 判断表是否存在
来源：http://www.share.zdbjq.cn/Article/details/guedjhnaf.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://mobile.zdbjq.cn/Article/details/gcwrszxlr.sHtML

[Q90] 生成序号列
来源：http://wap.hesvh.cn/Article/details/gcrsawgmi.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://baike.fehbvm.com/Article/details/gzgcrcdnq.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gyikmibgh.sHtML

R. Bash 专题
来源：http://m.share.fehbvm.com/Article/details/gavpfnoyp.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/ggndjejhm.sHtML

[R01] shebang 与严格模式
来源：http://www.m.share.zdbjq.cn/Article/details/gvgdkdseq.sHtML

#!/usr/bin/env bash
来源：http://baike.hesvh.cn/Article/details/ghjcyygxl.sHtML

set -euo pipefail
来源：http://www.blog.hesvh.cn/Article/details/gqtygtoqd.sHtML

[R02] 变量赋值与使用
来源：http://www.blog.hesvh.cn/Article/details/guonmjhqy.sHtML

name="Tom"; echo "$name"
来源：http://baike.hesvh.cn/Article/details/gkdwpbsjr.sHtML

[R03] 只读变量
来源：http://wap.hesvh.cn/Article/details/gvjtkbeuf.sHtML

readonly PI=3.14
来源：http://www.share.fehbvm.com/Article/details/ggevwwyzs.sHtML

[R04] 位置参数
来源：http://blog.zdbjq.cn/Article/details/gikeifkqk.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://read.share.zdbjq.cn/Article/details/gtblrtbhn.sHtML

[R05] 参数默认值
来源：http://www.m.share.hesvh.cn/Article/details/gufqlnlga.sHtML

name="${1:-default}"
来源：http://www.blog.hesvh.cn/Article/details/gwmihmnnh.sHtML

[R06] 判断命令是否存在
来源：http://www.share.hesvh.cn/Article/details/gewialjys.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://mobile.zdbjq.cn/Article/details/gcflaokgh.sHtML

[R07] if 判断文件
来源：http://mobile.hesvh.cn/Article/details/gejoaesjr.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.share.zdbjq.cn/Article/details/gjffgebfv.sHtML

[R08] 数值比较
来源：http://blog.fehbvm.com/Article/details/gtyeoyron.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://read.share.fehbvm.com/Article/details/grodabyhi.sHtML

[R09] 字符串比较
来源：http://m.share.fehbvm.com/Article/details/gwlwpzwwf.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.blog.fehbvm.com/Article/details/gjnpwvxeq.sHtML

[R10] 正则匹配
来源：http://wap.fehbvm.com/Article/details/gdtvvphnc.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://blog.fehbvm.com/Article/details/gaitfwije.sHtML

[R11] case 多分支
来源：http://baike.fehbvm.com/Article/details/gazmuhxue.sHtML

case "$1" in
来源：http://blog.hesvh.cn/Article/details/gvbllqhcy.sHtML

start) echo "启动" ;;
来源：http://read.share.zdbjq.cn/Article/details/gbgqqildb.sHtML

stop)  echo "停止" ;;
来源：http://wap.fehbvm.com/Article/details/gwvxfsyja.sHtML

*)     echo "未知命令" ;;
来源：http://wap.fehbvm.com/Article/details/gqxavawmm.sHtML

esac
来源：http://mobile.zdbjq.cn/Article/details/gnhejlvzz.sHtML

[R12] for 遍历文件
来源：http://blog.zdbjq.cn/Article/details/gfwrwnovo.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.share.zdbjq.cn/Article/details/gezodxtin.sHtML

[R13] for 计数循环
来源：http://www.blog.hesvh.cn/Article/details/gideywict.sHtML


<!-- 参考信息 -->