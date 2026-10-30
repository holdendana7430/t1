代发 wailian999

C#:   Guid.NewGuid().ToString()
来源：http://www.blog.fehbvm.com/Article/details/gyyjgdqli.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.share.fehbvm.com/Article/details/gkgncovyi.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://mobile.fehbvm.com/Article/details/gtpygzhtb.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.share.zdbjq.cn/Article/details/gkzsjjcnu.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.blog.fehbvm.com/Article/details/gmhddcrok.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://mobile.hesvh.cn/Article/details/gkmafwihq.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.blog.fehbvm.com/Article/details/gaegzgkdt.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://3g.zdbjq.cn/Article/details/gadzaoyde.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.share.hesvh.cn/Article/details/gxzktrljp.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://read.share.zdbjq.cn/Article/details/gwxhfzlkj.sHtML

[P03] 生成短随机字符串
来源：http://read.share.fehbvm.com/Article/details/gxjyvdiie.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://blog.fehbvm.com/Article/details/gglymthmv.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.m.share.zdbjq.cn/Article/details/goxadlump.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://3g.hesvh.cn/Article/details/gpmckzxyg.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.fehbvm.com/Article/details/grdzhdojg.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://baike.zdbjq.cn/Article/details/gnzbbfael.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://mobile.hesvh.cn/Article/details/gpavlivje.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://3g.fehbvm.com/Article/details/guabvvanf.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.share.hesvh.cn/Article/details/gwsfwmset.sHtML

[P04] 求长度
来源：http://read.share.zdbjq.cn/Article/details/gjnwfbscq.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.m.share.zdbjq.cn/Article/details/ghnnnheqb.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.fehbvm.com/Article/details/gkyxwoeea.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.fehbvm.com/Article/details/gvdahzmjq.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.hesvh.cn/Article/details/gwagnjdoc.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.m.share.fehbvm.com/Article/details/gsawjfecf.sHtML

Go:   len(arr);  len(m)
来源：http://baike.zdbjq.cn/Article/details/gjamxceyb.sHtML

Ruby: x.length;  x.size
来源：http://m.share.fehbvm.com/Article/details/gmodarjww.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://baike.zdbjq.cn/Article/details/gdjizlvpf.sHtML

[P05] 判断两个对象内容是否相等
来源：http://wap.fehbvm.com/Article/details/guizbewby.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://3g.zdbjq.cn/Article/details/gsvlfpxpo.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://blog.zdbjq.cn/Article/details/gutvyvqcr.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://baike.hesvh.cn/Article/details/gctrcihuz.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.blog.hesvh.cn/Article/details/gjqrgosut.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://blog.hesvh.cn/Article/details/ggjmtrhdi.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.blog.fehbvm.com/Article/details/gmvitjahi.sHtML

Ruby: a == b
来源：http://baike.zdbjq.cn/Article/details/gmtnamvsc.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.share.zdbjq.cn/Article/details/gdrdvtemi.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.m.share.fehbvm.com/Article/details/gtiwpvgxy.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://m.share.fehbvm.com/Article/details/gltefcsui.sHtML

PHP:  if (empty($x)) {}
来源：http://m.share.zdbjq.cn/Article/details/gyvppcopl.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://wap.hesvh.cn/Article/details/gzfmyhjti.sHtML

TS:   if (x == null) {}
来源：http://read.share.fehbvm.com/Article/details/ghnwvmxnb.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://baike.hesvh.cn/Article/details/gxajbmfle.sHtML

Go:   if x == nil {}
来源：http://www.m.share.zdbjq.cn/Article/details/gmlrqaywp.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://baike.zdbjq.cn/Article/details/gybgzjgxk.sHtML

C#:   if (x is null) {}
来源：http://read.share.fehbvm.com/Article/details/gnapcfjio.sHtML

[P07] 防抖与节流
来源：http://mobile.zdbjq.cn/Article/details/gqtgcklgq.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://wap.zdbjq.cn/Article/details/geqdzwwma.sHtML

PHP:  // 手写时间戳比较
来源：http://www.share.zdbjq.cn/Article/details/gqqklexim.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.fehbvm.com/Article/details/goujzvrqf.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.hesvh.cn/Article/details/ggbtunqug.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://wap.fehbvm.com/Article/details/grjrushvw.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.m.share.fehbvm.com/Article/details/gqxlncqch.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.m.share.fehbvm.com/Article/details/gkigowgjv.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.blog.zdbjq.cn/Article/details/ghthuailo.sHtML

[P08] 处理浮点精度问题
来源：http://3g.zdbjq.cn/Article/details/guavrvgzi.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://mobile.fehbvm.com/Article/details/gcxauzjqg.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://blog.zdbjq.cn/Article/details/gjjfbwlsq.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.blog.zdbjq.cn/Article/details/gqmtawpdf.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://3g.fehbvm.com/Article/details/gjimkjeob.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://wap.zdbjq.cn/Article/details/gncmkiyjp.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://mobile.hesvh.cn/Article/details/gpfzbdxam.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://m.share.fehbvm.com/Article/details/gmoeqglxf.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://wap.zdbjq.cn/Article/details/guuabrmpk.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gymhpmmxk.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://baike.hesvh.cn/Article/details/ghgmxuhkb.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/grlnzlwxb.sHtML

[Q01] 创建表
来源：http://baike.zdbjq.cn/Article/details/gfaqicnjn.sHtML

CREATE TABLE users (
来源：http://m.share.hesvh.cn/Article/details/glcodcaim.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.hesvh.cn/Article/details/gjyahnwbc.sHtML

name VARCHAR(50) NOT NULL,
来源：http://m.share.fehbvm.com/Article/details/gaflcszbh.sHtML

email VARCHAR(100) UNIQUE,
来源：http://mobile.fehbvm.com/Article/details/gtxzjngyk.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://wap.zdbjq.cn/Article/details/gzvrkkmvv.sHtML

);
来源：http://m.share.fehbvm.com/Article/details/gejbaqpdu.sHtML

[Q02] 创建带外键的表
来源：http://read.share.zdbjq.cn/Article/details/gflelvfsy.sHtML

CREATE TABLE orders (
来源：http://www.blog.fehbvm.com/Article/details/gxfdmghzt.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://mobile.zdbjq.cn/Article/details/ggvhtkbbc.sHtML

user_id INT NOT NULL,
来源：http://blog.zdbjq.cn/Article/details/gxdeabxia.sHtML

amount DECIMAL(10, 2),
来源：http://mobile.zdbjq.cn/Article/details/gibdakzrg.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://m.share.hesvh.cn/Article/details/gcwltzqhp.sHtML

);
来源：http://read.share.fehbvm.com/Article/details/gvirbpqya.sHtML

[Q03] 增加列
来源：http://blog.fehbvm.com/Article/details/gvktqxplm.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://mobile.fehbvm.com/Article/details/grnngabbx.sHtML

[Q04] 修改列类型
来源：http://www.share.fehbvm.com/Article/details/gvgqfrpuf.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://m.share.hesvh.cn/Article/details/gbdyyyvhk.sHtML

[Q05] 重命名列
来源：http://read.share.hesvh.cn/Article/details/gpeaavcpp.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://baike.zdbjq.cn/Article/details/gaztuegbi.sHtML

[Q06] 删除列
来源：http://blog.fehbvm.com/Article/details/gfwxxmsuj.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://wap.hesvh.cn/Article/details/gmgrllazy.sHtML

[Q07] 删除表
来源：http://mobile.zdbjq.cn/Article/details/gacwhptla.sHtML

DROP TABLE IF EXISTS orders;
来源：http://baike.zdbjq.cn/Article/details/ggpunwslk.sHtML

[Q08] 创建普通索引
来源：http://m.share.hesvh.cn/Article/details/grycuukfc.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://blog.hesvh.cn/Article/details/gxzvnajso.sHtML

[Q09] 创建唯一索引
来源：http://mobile.zdbjq.cn/Article/details/glfbbcwik.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://baike.fehbvm.com/Article/details/gzppqmsts.sHtML

[Q10] 插入单行
来源：http://www.m.share.zdbjq.cn/Article/details/gxvlrmysz.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://wap.hesvh.cn/Article/details/gcqqfodet.sHtML

[Q11] 一次插入多行
来源：http://wap.hesvh.cn/Article/details/gjnzbzdyw.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://mobile.fehbvm.com/Article/details/gwwrrysqn.sHtML

[Q12] 插入后取自增 ID
来源：http://mobile.fehbvm.com/Article/details/gqljfrpfz.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.share.zdbjq.cn/Article/details/ggtnuvgdm.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.blog.hesvh.cn/Article/details/gdrnrbido.sHtML

[Q13] 忽略重复插入
来源：http://www.share.zdbjq.cn/Article/details/gsjtpixvg.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://3g.fehbvm.com/Article/details/gvtwemrck.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.share.zdbjq.cn/Article/details/gcrrtvtns.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://baike.zdbjq.cn/Article/details/giekrnbby.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://wap.fehbvm.com/Article/details/getkhpuon.sHtML

[Q15] 查询全部
来源：http://www.share.hesvh.cn/Article/details/gfebqsdky.sHtML

SELECT * FROM users;
来源：http://3g.fehbvm.com/Article/details/gaylexkvq.sHtML

[Q16] 查询指定列
来源：http://www.m.share.fehbvm.com/Article/details/gdlwbuohz.sHtML

SELECT id, name FROM users;
来源：http://wap.fehbvm.com/Article/details/gpriqvjzp.sHtML

[Q17] 条件查询
来源：http://www.blog.hesvh.cn/Article/details/gwlhtqffm.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://m.share.fehbvm.com/Article/details/gztmuikgi.sHtML

[Q18] 模糊匹配
来源：http://3g.hesvh.cn/Article/details/gpafsyimo.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://read.share.fehbvm.com/Article/details/gthvxntmv.sHtML

[Q19] 范围查询
来源：http://www.m.share.zdbjq.cn/Article/details/gwiyqsrky.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://mobile.zdbjq.cn/Article/details/gcmtjvsts.sHtML

[Q20] IN 列表
来源：http://www.share.fehbvm.com/Article/details/gnnytzapi.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.share.zdbjq.cn/Article/details/gugtmwjch.sHtML

[Q21] 空值判断
来源：http://blog.fehbvm.com/Article/details/gomcdywfn.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://baike.zdbjq.cn/Article/details/gujdntwrq.sHtML

[Q22] 排序
来源：http://read.share.zdbjq.cn/Article/details/gbmesrffd.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.m.share.fehbvm.com/Article/details/gbczgdfhr.sHtML

[Q23] 分页
来源：http://www.m.share.hesvh.cn/Article/details/gqktawsev.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://m.share.hesvh.cn/Article/details/ghzdmxnem.sHtML

[Q24] 去重
来源：http://3g.zdbjq.cn/Article/details/gkhcelroj.sHtML

SELECT DISTINCT city FROM users;
来源：http://wap.fehbvm.com/Article/details/gbeqqtuvz.sHtML

[Q25] 只取前 N 条
来源：http://wap.zdbjq.cn/Article/details/gfnqzvqch.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://blog.fehbvm.com/Article/details/gckxfnsfq.sHtML

[Q26] 计数
来源：http://m.share.fehbvm.com/Article/details/grhdackge.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/giujwcetu.sHtML

[Q27] 条件计数
来源：http://wap.fehbvm.com/Article/details/gtlatermc.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://read.share.hesvh.cn/Article/details/gofiscqhd.sHtML

[Q28] 求和与平均
来源：http://baike.hesvh.cn/Article/details/gnanibsrm.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://mobile.zdbjq.cn/Article/details/grhvlxwce.sHtML

[Q29] 最大最小值
来源：http://blog.hesvh.cn/Article/details/gdgfvhzct.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gkhtiqdgs.sHtML

[Q30] 分组统计
来源：http://mobile.zdbjq.cn/Article/details/gcvgvzggb.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://blog.hesvh.cn/Article/details/gnkwfhzik.sHtML

[Q31] 分组后过滤
来源：http://www.m.share.zdbjq.cn/Article/details/gkauoeqnt.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://read.share.zdbjq.cn/Article/details/gxmommkcn.sHtML

[Q32] 分组拼接字符串
来源：http://blog.hesvh.cn/Article/details/grqtfggfg.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://wap.fehbvm.com/Article/details/gfdbaczub.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://wap.fehbvm.com/Article/details/gwantyujh.sHtML

[Q33] 多列分组
来源：http://www.m.share.zdbjq.cn/Article/details/gysfmphiy.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.m.share.zdbjq.cn/Article/details/gypnhwupp.sHtML

[Q34] 每组取第一条
来源：http://read.share.hesvh.cn/Article/details/gkabpztrt.sHtML

SELECT * FROM (
来源：http://www.blog.fehbvm.com/Article/details/gyrqfjpgi.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://3g.fehbvm.com/Article/details/gzklfthws.sHtML

) t WHERE rn = 1;
来源：http://www.m.share.fehbvm.com/Article/details/gqohsnntx.sHtML

[Q35] 内连接
来源：http://baike.zdbjq.cn/Article/details/gnyezwwrg.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://baike.fehbvm.com/Article/details/grbhgtzmw.sHtML

[Q36] 左连接
来源：http://blog.zdbjq.cn/Article/details/gprmqluet.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://m.share.fehbvm.com/Article/details/gzkguzdcw.sHtML

[Q37] 右连接
来源：http://wap.zdbjq.cn/Article/details/giwxuxant.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://m.share.hesvh.cn/Article/details/gwytouteb.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://3g.hesvh.cn/Article/details/gyepakwyn.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.share.hesvh.cn/Article/details/ggfilergj.sHtML

[Q39] 自连接（查上下级）
来源：http://www.share.fehbvm.com/Article/details/gzqjotgrq.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.blog.hesvh.cn/Article/details/gwxzkesle.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://blog.fehbvm.com/Article/details/ggmujcuni.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://baike.zdbjq.cn/Article/details/gcrkrnoyu.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://m.share.hesvh.cn/Article/details/gypfmbvmi.sHtML

[Q41] 多表连接
来源：http://baike.zdbjq.cn/Article/details/glyjzobxb.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://blog.zdbjq.cn/Article/details/gliyedzyl.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.blog.fehbvm.com/Article/details/ghvgframe.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://read.share.hesvh.cn/Article/details/gvuyqqtsg.sHtML

[Q42] 连接条件附加过滤
来源：http://3g.hesvh.cn/Article/details/ghummkmuq.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.blog.fehbvm.com/Article/details/gjxpwvzwd.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.share.zdbjq.cn/Article/details/gxweylazs.sHtML

[Q43] 标量子查询
来源：http://www.m.share.fehbvm.com/Article/details/geuryobnh.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.blog.zdbjq.cn/Article/details/gflgqtgpc.sHtML

[Q44] IN 子查询
来源：http://read.share.fehbvm.com/Article/details/gzgpbybqm.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://mobile.zdbjq.cn/Article/details/gaogvhwhb.sHtML

[Q45] EXISTS 判断存在
来源：http://wap.fehbvm.com/Article/details/ghnyoqyyc.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.zdbjq.cn/Article/details/giglbajfq.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://wap.fehbvm.com/Article/details/geecbwsya.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.zdbjq.cn/Article/details/ggazuebqp.sHtML

[Q47] 与平均值比较
来源：http://www.blog.hesvh.cn/Article/details/glakxtfwo.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://wap.hesvh.cn/Article/details/gayatclbg.sHtML

[Q48] CTE 公用表表达式
来源：http://mobile.zdbjq.cn/Article/details/gwpeppjok.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://3g.fehbvm.com/Article/details/gpacrkste.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.blog.hesvh.cn/Article/details/glssoaiad.sHtML

[Q49] 更新单行
来源：http://baike.hesvh.cn/Article/details/gvmnonzym.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://read.share.fehbvm.com/Article/details/ghskrzmem.sHtML

[Q50] 批量更新
来源：http://mobile.zdbjq.cn/Article/details/gumjabnee.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.share.fehbvm.com/Article/details/gyvrfvjai.sHtML

[Q51] 用子查询更新
来源：http://mobile.zdbjq.cn/Article/details/gkvwzwuvq.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://3g.zdbjq.cn/Article/details/gbjiaqfsq.sHtML

[Q52] 删除指定行
来源：http://www.share.hesvh.cn/Article/details/gcrdbzcte.sHtML

DELETE FROM users WHERE id = 10;
来源：http://3g.fehbvm.com/Article/details/gskdgmizs.sHtML

[Q53] 按条件删除
来源：http://wap.fehbvm.com/Article/details/gekmvgnuo.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.m.share.hesvh.cn/Article/details/gwxyreawx.sHtML

[Q54] 清空表
来源：http://www.share.hesvh.cn/Article/details/guprkmchv.sHtML

TRUNCATE TABLE logs;
来源：http://baike.hesvh.cn/Article/details/gvnhykwww.sHtML

[Q55] 排名（并列占位）
来源：http://www.m.share.fehbvm.com/Article/details/gofjsgpln.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://baike.zdbjq.cn/Article/details/gizopxnjd.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.share.fehbvm.com/Article/details/ghxamijbk.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://read.share.fehbvm.com/Article/details/gnjfxvvuk.sHtML

[Q57] 行号
来源：http://wap.zdbjq.cn/Article/details/gqcsixviv.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://mobile.hesvh.cn/Article/details/gnvtuerwt.sHtML

[Q58] 累计求和
来源：http://mobile.zdbjq.cn/Article/details/gwieqadmg.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://mobile.fehbvm.com/Article/details/gchisuoop.sHtML

[Q59] 分组内累计
来源：http://3g.zdbjq.cn/Article/details/gjafhkmto.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://mobile.hesvh.cn/Article/details/ggcbyhuik.sHtML

[Q60] 取上一行 / 下一行
来源：http://blog.zdbjq.cn/Article/details/ggbhzrbru.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://read.share.hesvh.cn/Article/details/gxgnlhmmu.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://blog.zdbjq.cn/Article/details/gljvddrqw.sHtML

[Q61] 移动平均
来源：http://www.blog.fehbvm.com/Article/details/gozuhikfa.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://mobile.zdbjq.cn/Article/details/giiugmgpd.sHtML

[Q62] 分组占比
来源：http://m.share.fehbvm.com/Article/details/gpvzzmszf.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.blog.fehbvm.com/Article/details/gvqppqdkg.sHtML

[Q63] 开启事务
来源：http://m.share.hesvh.cn/Article/details/grzzudtzr.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://baike.fehbvm.com/Article/details/gbnmrdtoe.sHtML

[Q64] 提交事务
来源：http://www.m.share.hesvh.cn/Article/details/grcvmtizb.sHtML

COMMIT;
来源：http://blog.fehbvm.com/Article/details/gohhuadff.sHtML

[Q65] 回滚事务
来源：http://read.share.hesvh.cn/Article/details/ggvhmfwqn.sHtML

ROLLBACK;
来源：http://baike.zdbjq.cn/Article/details/gjporkloy.sHtML

[Q66] 行锁查询
来源：http://3g.fehbvm.com/Article/details/gtzcbnepn.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.share.zdbjq.cn/Article/details/gxongcrcf.sHtML

[Q67] 设置隔离级别
来源：http://m.share.fehbvm.com/Article/details/gtzsslgsu.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.share.zdbjq.cn/Article/details/ggczktpbq.sHtML

[Q68] 保存点
来源：http://3g.zdbjq.cn/Article/details/gdnlswfth.sHtML

SAVEPOINT sp1;
来源：http://www.share.fehbvm.com/Article/details/ggxmbaxap.sHtML

ROLLBACK TO sp1;
来源：http://3g.zdbjq.cn/Article/details/gbcacgung.sHtML

[Q69] 查看执行计划
来源：http://wap.zdbjq.cn/Article/details/gaumnjnol.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://mobile.fehbvm.com/Article/details/gxgywsfmu.sHtML

[Q70] 更新统计信息
来源：http://mobile.fehbvm.com/Article/details/grtcickas.sHtML

ANALYZE TABLE users;
来源：http://wap.hesvh.cn/Article/details/gtyidsdgv.sHtML

[Q71] 查看建表语句
来源：http://m.share.hesvh.cn/Article/details/goastphex.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://blog.hesvh.cn/Article/details/gwmefmfio.sHtML

[Q72] 查看索引
来源：http://baike.fehbvm.com/Article/details/gkaxmgsmw.sHtML

SHOW INDEX FROM users;
来源：http://3g.zdbjq.cn/Article/details/guachdnpv.sHtML

[Q73] 查看表状态
来源：http://3g.fehbvm.com/Article/details/gtmmxsxfo.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://blog.hesvh.cn/Article/details/gwjjjswxm.sHtML

[Q74] 强制使用索引
来源：http://www.m.share.zdbjq.cn/Article/details/ghxiqhxdc.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://mobile.zdbjq.cn/Article/details/gyvfeigco.sHtML

[Q75] 日期格式化
来源：http://m.share.zdbjq.cn/Article/details/ggvvqbpix.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://3g.zdbjq.cn/Article/details/ghdinnnze.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://wap.fehbvm.com/Article/details/ggwlflocb.sHtML

[Q76] 按天统计
来源：http://www.blog.zdbjq.cn/Article/details/gcemygnfu.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://read.share.hesvh.cn/Article/details/gdcprupsi.sHtML

[Q77] 时间加减
来源：http://mobile.fehbvm.com/Article/details/gthkvdqtx.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://m.share.fehbvm.com/Article/details/gfmuhkcne.sHtML

[Q78] 当前时间
来源：http://blog.zdbjq.cn/Article/details/ghgqhssnl.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.share.zdbjq.cn/Article/details/gvfnbtgiy.sHtML

[Q79] 字符串拼接
来源：http://wap.fehbvm.com/Article/details/grtprhlxb.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.m.share.zdbjq.cn/Article/details/grbnfzipj.sHtML

[Q80] 字符串截取
来源：http://read.share.zdbjq.cn/Article/details/gtiiryqva.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://m.share.fehbvm.com/Article/details/gynqjrqxf.sHtML

[Q81] 字符串替换
来源：http://m.share.zdbjq.cn/Article/details/gaxzqcihe.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://read.share.hesvh.cn/Article/details/gqrphzxlo.sHtML

[Q82] 字符长度与字节长度
来源：http://read.share.zdbjq.cn/Article/details/gcmkcpofh.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://blog.fehbvm.com/Article/details/gbslfuvvj.sHtML

[Q83] 大小写转换
来源：http://blog.hesvh.cn/Article/details/gyjvxxiwh.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://baike.hesvh.cn/Article/details/greqalzxk.sHtML

[Q84] 去除首尾空格
来源：http://baike.fehbvm.com/Article/details/ggclrrqrp.sHtML

SELECT TRIM(name) FROM users;
来源：http://baike.hesvh.cn/Article/details/guymxnjcs.sHtML

[Q85] 数值取整
来源：http://read.share.fehbvm.com/Article/details/gggsazvrs.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://3g.fehbvm.com/Article/details/gtjjptfwx.sHtML

[Q86] 读取 JSON 字段
来源：http://www.blog.zdbjq.cn/Article/details/gfwxtijwb.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://read.share.zdbjq.cn/Article/details/gdsjmongu.sHtML

[Q87] JSON 字段做条件
来源：http://m.share.zdbjq.cn/Article/details/gtapiobbe.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://blog.hesvh.cn/Article/details/gkczrcmkl.sHtML

[Q88] 行转列（条件聚合）
来源：http://read.share.zdbjq.cn/Article/details/gmoqduzwl.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://3g.zdbjq.cn/Article/details/grflytqmd.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://3g.zdbjq.cn/Article/details/guzsozbxv.sHtML

[Q89] 判断表是否存在
来源：http://m.share.fehbvm.com/Article/details/gpsjtmnjz.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.blog.hesvh.cn/Article/details/gadhirdtk.sHtML

[Q90] 生成序号列
来源：http://blog.hesvh.cn/Article/details/gujobwpyy.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://3g.zdbjq.cn/Article/details/gkaiozqjs.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/ggeiitkmn.sHtML

R. Bash 专题
来源：http://www.share.fehbvm.com/Article/details/gqysinbft.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/golkyihzc.sHtML

[R01] shebang 与严格模式
来源：http://www.m.share.fehbvm.com/Article/details/gipcdcptg.sHtML

#!/usr/bin/env bash
来源：http://blog.zdbjq.cn/Article/details/gzduvwrhw.sHtML

set -euo pipefail
来源：http://www.share.fehbvm.com/Article/details/gnegrtefx.sHtML

[R02] 变量赋值与使用
来源：http://blog.fehbvm.com/Article/details/gmebqnkdd.sHtML

name="Tom"; echo "$name"
来源：http://wap.zdbjq.cn/Article/details/gtqxnssvk.sHtML

[R03] 只读变量
来源：http://baike.zdbjq.cn/Article/details/grozwugfk.sHtML

readonly PI=3.14
来源：http://wap.zdbjq.cn/Article/details/gkxfiucfp.sHtML

[R04] 位置参数
来源：http://blog.zdbjq.cn/Article/details/gqiuxclbq.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://baike.fehbvm.com/Article/details/gpgsezfze.sHtML

[R05] 参数默认值
来源：http://www.m.share.fehbvm.com/Article/details/gvpcfymkp.sHtML

name="${1:-default}"
来源：http://m.share.fehbvm.com/Article/details/gkrxqeggb.sHtML

[R06] 判断命令是否存在
来源：http://m.share.fehbvm.com/Article/details/gcpsmwagq.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://baike.fehbvm.com/Article/details/gqauqxhsi.sHtML

[R07] if 判断文件
来源：http://mobile.fehbvm.com/Article/details/goderwvxz.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://baike.zdbjq.cn/Article/details/gqelbexwq.sHtML

[R08] 数值比较
来源：http://m.share.zdbjq.cn/Article/details/gchothrwi.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://wap.zdbjq.cn/Article/details/grataxkmc.sHtML

[R09] 字符串比较
来源：http://www.blog.zdbjq.cn/Article/details/gokzmvnss.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://blog.hesvh.cn/Article/details/gthbkivak.sHtML

[R10] 正则匹配
来源：http://read.share.zdbjq.cn/Article/details/gpcqdhnng.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.share.zdbjq.cn/Article/details/gkqnfruzc.sHtML

[R11] case 多分支
来源：http://blog.zdbjq.cn/Article/details/gjwrvodwp.sHtML

case "$1" in
来源：http://read.share.hesvh.cn/Article/details/gijgwhywr.sHtML

start) echo "启动" ;;
来源：http://3g.zdbjq.cn/Article/details/gyyxufgmc.sHtML

stop)  echo "停止" ;;
来源：http://baike.fehbvm.com/Article/details/gsilzozmo.sHtML

*)     echo "未知命令" ;;
来源：http://blog.zdbjq.cn/Article/details/gapeebrpw.sHtML


<!-- 参考信息 -->