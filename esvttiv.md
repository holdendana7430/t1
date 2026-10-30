代发 wailian999

C#:   Guid.NewGuid().ToString()
来源：http://m.share.zdbjq.cn/Article/details/gsdjqlkpx.sHtML

[P02] MD5 / SHA256 摘要
来源：http://blog.hesvh.cn/Article/details/gdfqwlpzm.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://wap.fehbvm.com/Article/details/ghvffgzjk.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.m.share.fehbvm.com/Article/details/gzmszrceq.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://read.share.hesvh.cn/Article/details/guvstihoi.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://baike.zdbjq.cn/Article/details/giasbtupl.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://read.share.zdbjq.cn/Article/details/gnkowqbhf.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://blog.zdbjq.cn/Article/details/gwfrujhmi.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://baike.hesvh.cn/Article/details/ghqefrlcu.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://wap.fehbvm.com/Article/details/gunbklxbs.sHtML

[P03] 生成短随机字符串
来源：http://blog.zdbjq.cn/Article/details/gflykjzbt.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://wap.hesvh.cn/Article/details/gykfyhkct.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://mobile.hesvh.cn/Article/details/gxkmmhskt.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.fehbvm.com/Article/details/gkayfekqc.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.hesvh.cn/Article/details/gbnjkxqif.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://3g.hesvh.cn/Article/details/glyfscmds.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://3g.hesvh.cn/Article/details/gmrekysca.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://read.share.zdbjq.cn/Article/details/gumiugkye.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://blog.fehbvm.com/Article/details/gsjdayfed.sHtML

[P04] 求长度
来源：http://blog.hesvh.cn/Article/details/gmpozhynz.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://m.share.zdbjq.cn/Article/details/gqwpibexf.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://read.share.hesvh.cn/Article/details/gdbmltcrj.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.fehbvm.com/Article/details/gfeusmpjq.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.hesvh.cn/Article/details/gozbfipow.sHtML

Java: list.size();  map.size();  s.length()
来源：http://mobile.hesvh.cn/Article/details/gxfakmvgj.sHtML

Go:   len(arr);  len(m)
来源：http://www.m.share.fehbvm.com/Article/details/gkoisygve.sHtML

Ruby: x.length;  x.size
来源：http://3g.hesvh.cn/Article/details/golhqjvph.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://read.share.fehbvm.com/Article/details/goibstblr.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.blog.hesvh.cn/Article/details/geovpuhep.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.share.hesvh.cn/Article/details/gqzuowjki.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.share.hesvh.cn/Article/details/gzrqishcr.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://read.share.hesvh.cn/Article/details/gtrwrjkmp.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.share.fehbvm.com/Article/details/gheziilkz.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://m.share.fehbvm.com/Article/details/gjscectae.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://baike.fehbvm.com/Article/details/guvuazqnf.sHtML

Ruby: a == b
来源：http://read.share.fehbvm.com/Article/details/gccypceaf.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://baike.hesvh.cn/Article/details/gjimcqmxs.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://wap.hesvh.cn/Article/details/gcgavzvan.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://baike.hesvh.cn/Article/details/gydotodwq.sHtML

PHP:  if (empty($x)) {}
来源：http://wap.fehbvm.com/Article/details/gvxamnenj.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://blog.zdbjq.cn/Article/details/giowokvca.sHtML

TS:   if (x == null) {}
来源：http://www.blog.fehbvm.com/Article/details/gqgezyahz.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://m.share.hesvh.cn/Article/details/glbykuwel.sHtML

Go:   if x == nil {}
来源：http://www.share.zdbjq.cn/Article/details/gwojveqyo.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://blog.hesvh.cn/Article/details/gnuvyyyml.sHtML

C#:   if (x is null) {}
来源：http://read.share.zdbjq.cn/Article/details/gmyuijdnb.sHtML

[P07] 防抖与节流
来源：http://wap.hesvh.cn/Article/details/gnsqxtwtp.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://mobile.zdbjq.cn/Article/details/ggxmjbsmo.sHtML

PHP:  // 手写时间戳比较
来源：http://www.m.share.hesvh.cn/Article/details/gkiyopqsi.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.hesvh.cn/Article/details/gfdboxmap.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.hesvh.cn/Article/details/geiptsoyr.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://blog.hesvh.cn/Article/details/grfggrncp.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://read.share.zdbjq.cn/Article/details/groaojznh.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://wap.fehbvm.com/Article/details/gvijpoewq.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.m.share.fehbvm.com/Article/details/gcypgmgmh.sHtML

[P08] 处理浮点精度问题
来源：http://www.m.share.fehbvm.com/Article/details/gvjgcuiuw.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://mobile.fehbvm.com/Article/details/galxlekej.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.blog.zdbjq.cn/Article/details/glqwakuqq.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.share.fehbvm.com/Article/details/gympxykpg.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.share.fehbvm.com/Article/details/gytjyiqnc.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://3g.hesvh.cn/Article/details/gctlmsszs.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://3g.fehbvm.com/Article/details/gsmkyoluz.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://mobile.zdbjq.cn/Article/details/gupjyrnpi.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.m.share.zdbjq.cn/Article/details/gtihyiypg.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gwanxidue.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://read.share.zdbjq.cn/Article/details/gaxvuyuok.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gavriaijb.sHtML

[Q01] 创建表
来源：http://3g.zdbjq.cn/Article/details/gvdladolc.sHtML

CREATE TABLE users (
来源：http://m.share.fehbvm.com/Article/details/gwgpipagl.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.fehbvm.com/Article/details/gosxzhfka.sHtML

name VARCHAR(50) NOT NULL,
来源：http://mobile.zdbjq.cn/Article/details/ggzxrdzph.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.blog.hesvh.cn/Article/details/grevnjjbg.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.blog.hesvh.cn/Article/details/gyyaxanft.sHtML

);
来源：http://m.share.hesvh.cn/Article/details/gqexcuxdv.sHtML

[Q02] 创建带外键的表
来源：http://m.share.zdbjq.cn/Article/details/gbvssrdqd.sHtML

CREATE TABLE orders (
来源：http://wap.fehbvm.com/Article/details/gxumtsssw.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.zdbjq.cn/Article/details/gqouyirml.sHtML

user_id INT NOT NULL,
来源：http://read.share.zdbjq.cn/Article/details/gqjbpuict.sHtML

amount DECIMAL(10, 2),
来源：http://mobile.fehbvm.com/Article/details/ggkamzynj.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.share.zdbjq.cn/Article/details/gvosufrik.sHtML

);
来源：http://read.share.hesvh.cn/Article/details/gkahbjljb.sHtML

[Q03] 增加列
来源：http://read.share.fehbvm.com/Article/details/garklnecz.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.share.zdbjq.cn/Article/details/glzjgmztn.sHtML

[Q04] 修改列类型
来源：http://3g.hesvh.cn/Article/details/glluljjpj.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.share.hesvh.cn/Article/details/gqyeruqfq.sHtML

[Q05] 重命名列
来源：http://blog.hesvh.cn/Article/details/gahsxctig.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://baike.fehbvm.com/Article/details/gczgxtgzs.sHtML

[Q06] 删除列
来源：http://mobile.fehbvm.com/Article/details/gzwjtaojx.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.blog.fehbvm.com/Article/details/giqeiyidx.sHtML

[Q07] 删除表
来源：http://read.share.fehbvm.com/Article/details/gwjuasdzr.sHtML

DROP TABLE IF EXISTS orders;
来源：http://m.share.fehbvm.com/Article/details/gefwpkgpo.sHtML

[Q08] 创建普通索引
来源：http://www.blog.hesvh.cn/Article/details/gcsgquavn.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://blog.hesvh.cn/Article/details/gknimzrwx.sHtML

[Q09] 创建唯一索引
来源：http://www.m.share.zdbjq.cn/Article/details/gaohldtvz.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.blog.zdbjq.cn/Article/details/gjcbzleza.sHtML

[Q10] 插入单行
来源：http://m.share.fehbvm.com/Article/details/gwrosysqp.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://mobile.fehbvm.com/Article/details/gmsndiahc.sHtML

[Q11] 一次插入多行
来源：http://www.m.share.fehbvm.com/Article/details/goqgzotzw.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://baike.zdbjq.cn/Article/details/geblcbgxs.sHtML

[Q12] 插入后取自增 ID
来源：http://www.blog.fehbvm.com/Article/details/gnxibtbck.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.m.share.hesvh.cn/Article/details/gjjhgyggs.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.share.zdbjq.cn/Article/details/ganokrofv.sHtML

[Q13] 忽略重复插入
来源：http://www.blog.hesvh.cn/Article/details/gpsolvbcr.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://blog.hesvh.cn/Article/details/gndxygaau.sHtML

[Q14] 存在则更新（upsert）
来源：http://wap.fehbvm.com/Article/details/ggtzxkoev.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://m.share.fehbvm.com/Article/details/ggwnzdjjp.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://m.share.zdbjq.cn/Article/details/gkwwepbge.sHtML

[Q15] 查询全部
来源：http://blog.zdbjq.cn/Article/details/gvrlpctxb.sHtML

SELECT * FROM users;
来源：http://m.share.hesvh.cn/Article/details/grofwywei.sHtML

[Q16] 查询指定列
来源：http://3g.zdbjq.cn/Article/details/ghyhkwmmx.sHtML

SELECT id, name FROM users;
来源：http://mobile.hesvh.cn/Article/details/grjrrrooy.sHtML

[Q17] 条件查询
来源：http://3g.fehbvm.com/Article/details/gtbxykegq.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://m.share.zdbjq.cn/Article/details/gitmvqxdr.sHtML

[Q18] 模糊匹配
来源：http://blog.hesvh.cn/Article/details/gaokkcdrp.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://mobile.zdbjq.cn/Article/details/gbugniouk.sHtML

[Q19] 范围查询
来源：http://wap.fehbvm.com/Article/details/gokkdeqjm.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://3g.zdbjq.cn/Article/details/gygqumsyw.sHtML

[Q20] IN 列表
来源：http://www.share.fehbvm.com/Article/details/geswlcfso.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://wap.fehbvm.com/Article/details/gnrhlnbnx.sHtML

[Q21] 空值判断
来源：http://www.m.share.zdbjq.cn/Article/details/gyadickjq.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.blog.zdbjq.cn/Article/details/gyeddhrxj.sHtML

[Q22] 排序
来源：http://mobile.hesvh.cn/Article/details/gudzxcqkm.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://mobile.zdbjq.cn/Article/details/gslclcbzx.sHtML

[Q23] 分页
来源：http://baike.fehbvm.com/Article/details/guuwqdkki.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://baike.hesvh.cn/Article/details/gguwboute.sHtML

[Q24] 去重
来源：http://www.blog.zdbjq.cn/Article/details/goitduzrb.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/ggaxopvca.sHtML

[Q25] 只取前 N 条
来源：http://read.share.fehbvm.com/Article/details/gajpcitsi.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://3g.zdbjq.cn/Article/details/gddquowlt.sHtML

[Q26] 计数
来源：http://www.blog.zdbjq.cn/Article/details/gnxjyzphs.sHtML

SELECT COUNT(*) FROM users;
来源：http://blog.fehbvm.com/Article/details/gpiimyhwy.sHtML

[Q27] 条件计数
来源：http://wap.fehbvm.com/Article/details/gldaihnvg.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://read.share.fehbvm.com/Article/details/gzurvpckp.sHtML

[Q28] 求和与平均
来源：http://wap.fehbvm.com/Article/details/gkrhqxyqz.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.share.hesvh.cn/Article/details/gnelhdwqp.sHtML

[Q29] 最大最小值
来源：http://3g.zdbjq.cn/Article/details/gjypbzmhk.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://mobile.hesvh.cn/Article/details/gyaljbfik.sHtML

[Q30] 分组统计
来源：http://baike.fehbvm.com/Article/details/gprhlsnrl.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://wap.hesvh.cn/Article/details/ggghcdzef.sHtML

[Q31] 分组后过滤
来源：http://m.share.fehbvm.com/Article/details/ghxjferbr.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.m.share.zdbjq.cn/Article/details/gdywovrwy.sHtML

[Q32] 分组拼接字符串
来源：http://m.share.hesvh.cn/Article/details/gxfbizypu.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://blog.fehbvm.com/Article/details/gqnoxsahm.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.m.share.zdbjq.cn/Article/details/gemcjudqh.sHtML

[Q33] 多列分组
来源：http://wap.fehbvm.com/Article/details/gdviivwve.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://wap.fehbvm.com/Article/details/gntcjquyx.sHtML

[Q34] 每组取第一条
来源：http://baike.zdbjq.cn/Article/details/gwasmtyrv.sHtML

SELECT * FROM (
来源：http://wap.zdbjq.cn/Article/details/geuvkwqqw.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.share.zdbjq.cn/Article/details/gfrgjilfn.sHtML

) t WHERE rn = 1;
来源：http://wap.fehbvm.com/Article/details/guubwvjfw.sHtML

[Q35] 内连接
来源：http://blog.zdbjq.cn/Article/details/gfgxklygx.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://mobile.zdbjq.cn/Article/details/groierlwb.sHtML

[Q36] 左连接
来源：http://wap.fehbvm.com/Article/details/golqsyfca.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.fehbvm.com/Article/details/gxeufbxgi.sHtML

[Q37] 右连接
来源：http://3g.fehbvm.com/Article/details/gyxfcgyzv.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://blog.hesvh.cn/Article/details/gbxostqtq.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.m.share.zdbjq.cn/Article/details/ghoaefazh.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.share.hesvh.cn/Article/details/gmzarduye.sHtML

[Q39] 自连接（查上下级）
来源：http://baike.fehbvm.com/Article/details/gusgetflr.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.blog.zdbjq.cn/Article/details/gqhqhlycr.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.blog.zdbjq.cn/Article/details/gskfxtunc.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://blog.fehbvm.com/Article/details/gfgykfibm.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://mobile.zdbjq.cn/Article/details/gkwtanrnb.sHtML

[Q41] 多表连接
来源：http://m.share.fehbvm.com/Article/details/gkzusvkrr.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://mobile.hesvh.cn/Article/details/ghakpbfsv.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.blog.hesvh.cn/Article/details/gecoezaei.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://wap.zdbjq.cn/Article/details/gkasixanv.sHtML

[Q42] 连接条件附加过滤
来源：http://blog.zdbjq.cn/Article/details/gjtkgtwft.sHtML

SELECT u.name, o.amount FROM users u
来源：http://m.share.hesvh.cn/Article/details/gppugsgxx.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://read.share.hesvh.cn/Article/details/grlkustje.sHtML

[Q43] 标量子查询
来源：http://wap.fehbvm.com/Article/details/gpydakply.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.share.zdbjq.cn/Article/details/ghxugvvru.sHtML

[Q44] IN 子查询
来源：http://read.share.hesvh.cn/Article/details/gopoysbzm.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://3g.hesvh.cn/Article/details/golwimxut.sHtML

[Q45] EXISTS 判断存在
来源：http://blog.zdbjq.cn/Article/details/gqjsogjuu.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.hesvh.cn/Article/details/gvicgojpf.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.share.hesvh.cn/Article/details/gcusxypez.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.zdbjq.cn/Article/details/grvsltldw.sHtML

[Q47] 与平均值比较
来源：http://wap.zdbjq.cn/Article/details/gszilmqqm.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.blog.fehbvm.com/Article/details/gmmvysbfq.sHtML

[Q48] CTE 公用表表达式
来源：http://read.share.hesvh.cn/Article/details/ghyhultyh.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://wap.fehbvm.com/Article/details/gwcwyfzyc.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://m.share.hesvh.cn/Article/details/ghobadubi.sHtML

[Q49] 更新单行
来源：http://blog.hesvh.cn/Article/details/gzzubrdyf.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://mobile.fehbvm.com/Article/details/gdbqzbrue.sHtML

[Q50] 批量更新
来源：http://baike.fehbvm.com/Article/details/gmdkvigbt.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://mobile.zdbjq.cn/Article/details/gzerkwzhy.sHtML

[Q51] 用子查询更新
来源：http://www.m.share.zdbjq.cn/Article/details/gxoaxdwuu.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.share.zdbjq.cn/Article/details/glvbzcmml.sHtML

[Q52] 删除指定行
来源：http://read.share.fehbvm.com/Article/details/gthcxgtil.sHtML

DELETE FROM users WHERE id = 10;
来源：http://blog.fehbvm.com/Article/details/guiswiooo.sHtML

[Q53] 按条件删除
来源：http://wap.zdbjq.cn/Article/details/gefhfshdz.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://wap.fehbvm.com/Article/details/gzticubyi.sHtML

[Q54] 清空表
来源：http://blog.zdbjq.cn/Article/details/gpjpfgqtj.sHtML

TRUNCATE TABLE logs;
来源：http://m.share.fehbvm.com/Article/details/gxuvnvddf.sHtML

[Q55] 排名（并列占位）
来源：http://m.share.hesvh.cn/Article/details/gplbixuts.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://baike.fehbvm.com/Article/details/gfodesmpy.sHtML

[Q56] 密集排名（并列不占位）
来源：http://mobile.fehbvm.com/Article/details/gpwuymjay.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://baike.zdbjq.cn/Article/details/gbmzucjha.sHtML

[Q57] 行号
来源：http://www.share.zdbjq.cn/Article/details/grvpeakcd.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://wap.fehbvm.com/Article/details/gzknaghfx.sHtML

[Q58] 累计求和
来源：http://mobile.zdbjq.cn/Article/details/gdmctnalc.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://wap.hesvh.cn/Article/details/gvjudahyp.sHtML

[Q59] 分组内累计
来源：http://baike.zdbjq.cn/Article/details/gwovgahrv.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.share.fehbvm.com/Article/details/gbwqofzzz.sHtML

[Q60] 取上一行 / 下一行
来源：http://blog.hesvh.cn/Article/details/gdvpvpkma.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://3g.zdbjq.cn/Article/details/gszyfpzvu.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://3g.hesvh.cn/Article/details/ghtpizjwx.sHtML

[Q61] 移动平均
来源：http://www.share.hesvh.cn/Article/details/gyhfmuelt.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.m.share.zdbjq.cn/Article/details/gjvkzjzsb.sHtML

[Q62] 分组占比
来源：http://m.share.hesvh.cn/Article/details/gkuerkmib.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://mobile.zdbjq.cn/Article/details/gbjnzfjuz.sHtML

[Q63] 开启事务
来源：http://baike.hesvh.cn/Article/details/gbmgbewdp.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://read.share.zdbjq.cn/Article/details/gmvczsxci.sHtML

[Q64] 提交事务
来源：http://blog.hesvh.cn/Article/details/ghvsscopm.sHtML

COMMIT;
来源：http://wap.fehbvm.com/Article/details/gegolqxab.sHtML

[Q65] 回滚事务
来源：http://m.share.zdbjq.cn/Article/details/gfjpxdoem.sHtML

ROLLBACK;
来源：http://read.share.zdbjq.cn/Article/details/gcpynvwkb.sHtML

[Q66] 行锁查询
来源：http://read.share.fehbvm.com/Article/details/gjexyuiib.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.blog.hesvh.cn/Article/details/gztjrhibq.sHtML

[Q67] 设置隔离级别
来源：http://mobile.zdbjq.cn/Article/details/gyujjfhxb.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://m.share.fehbvm.com/Article/details/guivislsq.sHtML

[Q68] 保存点
来源：http://3g.hesvh.cn/Article/details/glbfbvdhm.sHtML

SAVEPOINT sp1;
来源：http://blog.hesvh.cn/Article/details/ghwxwgtud.sHtML

ROLLBACK TO sp1;
来源：http://www.m.share.zdbjq.cn/Article/details/gwfkciwmt.sHtML

[Q69] 查看执行计划
来源：http://www.m.share.fehbvm.com/Article/details/gatctduhv.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://m.share.hesvh.cn/Article/details/gwtgfiewr.sHtML

[Q70] 更新统计信息
来源：http://3g.hesvh.cn/Article/details/gtknydqeo.sHtML

ANALYZE TABLE users;
来源：http://www.share.hesvh.cn/Article/details/gozsiadjr.sHtML

[Q71] 查看建表语句
来源：http://baike.zdbjq.cn/Article/details/gokcegzuj.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://m.share.hesvh.cn/Article/details/gacdpwqtw.sHtML

[Q72] 查看索引
来源：http://www.m.share.hesvh.cn/Article/details/gxfvpauzd.sHtML

SHOW INDEX FROM users;
来源：http://www.share.fehbvm.com/Article/details/grgwvcgra.sHtML

[Q73] 查看表状态
来源：http://blog.fehbvm.com/Article/details/gbnvcbgon.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://read.share.fehbvm.com/Article/details/gyndfluea.sHtML

[Q74] 强制使用索引
来源：http://wap.hesvh.cn/Article/details/gzcoaemiw.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://wap.fehbvm.com/Article/details/gecynlcjz.sHtML

[Q75] 日期格式化
来源：http://blog.hesvh.cn/Article/details/gzrfhnoep.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://mobile.hesvh.cn/Article/details/gyhpskjig.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.m.share.hesvh.cn/Article/details/giuujthtk.sHtML

[Q76] 按天统计
来源：http://www.blog.fehbvm.com/Article/details/gltqroxog.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://blog.fehbvm.com/Article/details/gcfuijhyo.sHtML

[Q77] 时间加减
来源：http://www.share.fehbvm.com/Article/details/gvrilhvua.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://mobile.fehbvm.com/Article/details/gsgzcawun.sHtML

[Q78] 当前时间
来源：http://3g.fehbvm.com/Article/details/gxtzudixm.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://blog.hesvh.cn/Article/details/gdcuyfqkx.sHtML

[Q79] 字符串拼接
来源：http://www.blog.fehbvm.com/Article/details/gkemyvxxp.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.m.share.zdbjq.cn/Article/details/gxiwyrdns.sHtML

[Q80] 字符串截取
来源：http://blog.hesvh.cn/Article/details/gmbvkuldo.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://mobile.hesvh.cn/Article/details/gigzcxjox.sHtML

[Q81] 字符串替换
来源：http://www.blog.zdbjq.cn/Article/details/grwzjlovb.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://mobile.hesvh.cn/Article/details/gqinqnnuq.sHtML

[Q82] 字符长度与字节长度
来源：http://baike.fehbvm.com/Article/details/gsoalgtkv.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gbjmarjou.sHtML

[Q83] 大小写转换
来源：http://www.share.hesvh.cn/Article/details/guvbxeqdv.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gtfhgxbzh.sHtML

[Q84] 去除首尾空格
来源：http://www.blog.fehbvm.com/Article/details/gbvbdewig.sHtML

SELECT TRIM(name) FROM users;
来源：http://baike.zdbjq.cn/Article/details/gisbdpmyt.sHtML

[Q85] 数值取整
来源：http://wap.zdbjq.cn/Article/details/gwzujcjyk.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://wap.hesvh.cn/Article/details/gfmtcekeq.sHtML

[Q86] 读取 JSON 字段
来源：http://wap.hesvh.cn/Article/details/gazzyxxdr.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.m.share.hesvh.cn/Article/details/gsycpnlfd.sHtML

[Q87] JSON 字段做条件
来源：http://read.share.zdbjq.cn/Article/details/gneaqaqff.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://m.share.fehbvm.com/Article/details/gsbjcabmx.sHtML

[Q88] 行转列（条件聚合）
来源：http://blog.hesvh.cn/Article/details/ghrcywefq.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.share.hesvh.cn/Article/details/gocbtwwsd.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.share.zdbjq.cn/Article/details/goozwxfdk.sHtML

[Q89] 判断表是否存在
来源：http://baike.hesvh.cn/Article/details/gyosqufwu.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://read.share.fehbvm.com/Article/details/gwbnncgiy.sHtML

[Q90] 生成序号列
来源：http://3g.fehbvm.com/Article/details/gkqvojtrq.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.m.share.hesvh.cn/Article/details/gtfpwirme.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gsqakydih.sHtML

R. Bash 专题
来源：http://m.share.hesvh.cn/Article/details/genuagysi.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gpyidkvjv.sHtML

[R01] shebang 与严格模式
来源：http://www.m.share.fehbvm.com/Article/details/gfvjwvkfg.sHtML

#!/usr/bin/env bash
来源：http://baike.zdbjq.cn/Article/details/gfsurqnys.sHtML

set -euo pipefail
来源：http://wap.zdbjq.cn/Article/details/gsrfwnijl.sHtML

[R02] 变量赋值与使用
来源：http://m.share.fehbvm.com/Article/details/gzdythdgn.sHtML

name="Tom"; echo "$name"
来源：http://mobile.zdbjq.cn/Article/details/gnhhdcidi.sHtML

[R03] 只读变量
来源：http://blog.hesvh.cn/Article/details/guaducgwu.sHtML

readonly PI=3.14
来源：http://www.m.share.hesvh.cn/Article/details/gyqtkbsga.sHtML

[R04] 位置参数
来源：http://m.share.fehbvm.com/Article/details/gbvsfmeoz.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://read.share.zdbjq.cn/Article/details/gzceoavue.sHtML

[R05] 参数默认值
来源：http://www.blog.hesvh.cn/Article/details/gnhwxkgot.sHtML

name="${1:-default}"
来源：http://mobile.hesvh.cn/Article/details/glnewzwfv.sHtML

[R06] 判断命令是否存在
来源：http://wap.zdbjq.cn/Article/details/glbkjupcl.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://read.share.zdbjq.cn/Article/details/gotidzmcj.sHtML

[R07] if 判断文件
来源：http://baike.hesvh.cn/Article/details/gfuwtukld.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://baike.zdbjq.cn/Article/details/gxqnrjgnk.sHtML

[R08] 数值比较
来源：http://3g.fehbvm.com/Article/details/gexhkcedz.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://baike.zdbjq.cn/Article/details/gvuowffbz.sHtML

[R09] 字符串比较
来源：http://baike.hesvh.cn/Article/details/gulkglwhl.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.blog.fehbvm.com/Article/details/gdfbpdluy.sHtML

[R10] 正则匹配
来源：http://mobile.fehbvm.com/Article/details/gutrxyrix.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://m.share.fehbvm.com/Article/details/gharmywgr.sHtML

[R11] case 多分支
来源：http://blog.fehbvm.com/Article/details/gapqcowjx.sHtML

case "$1" in
来源：http://wap.fehbvm.com/Article/details/gmwkoycal.sHtML

start) echo "启动" ;;
来源：http://www.share.hesvh.cn/Article/details/ghufbzoku.sHtML

stop)  echo "停止" ;;
来源：http://m.share.zdbjq.cn/Article/details/gspxirmcw.sHtML

*)     echo "未知命令" ;;
来源：http://www.m.share.hesvh.cn/Article/details/gjgkbddof.sHtML


<!-- 参考信息 -->