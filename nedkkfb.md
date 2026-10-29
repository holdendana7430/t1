代发 wailian999

TS:   crypto.randomUUID()
来源：http://wap.hesvh.cn/Article/details/gzgxcdhzg.sHtML

Java: UUID.randomUUID().toString()
来源：http://baike.hesvh.cn/Article/details/gknjjosbv.sHtML

Go:   // 用 github.com/google/uuid
来源：http://blog.fehbvm.com/Article/details/gxxmnpjng.sHtML

Ruby: SecureRandom.uuid
来源：http://3g.hesvh.cn/Article/details/gexeqykfh.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://blog.zdbjq.cn/Article/details/gmlxrjgph.sHtML

[P02] MD5 / SHA256 摘要
来源：http://3g.fehbvm.com/Article/details/glsxltqtt.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.share.zdbjq.cn/Article/details/gjloonesb.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://wap.hesvh.cn/Article/details/gurdfpsef.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://mobile.fehbvm.com/Article/details/ghrejktsf.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://m.share.zdbjq.cn/Article/details/gayxqmmvx.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.m.share.hesvh.cn/Article/details/gcvjpuexg.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://m.share.zdbjq.cn/Article/details/gcbpxxmgc.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://3g.zdbjq.cn/Article/details/gsmopitjb.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://wap.fehbvm.com/Article/details/guzwhuldc.sHtML

[P03] 生成短随机字符串
来源：http://read.share.fehbvm.com/Article/details/gcknjyqyl.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://wap.zdbjq.cn/Article/details/glpjlwpfv.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://blog.hesvh.cn/Article/details/gwoxghrkd.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.fehbvm.com/Article/details/gpsqttsdh.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.zdbjq.cn/Article/details/gzpfgdxaf.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://blog.hesvh.cn/Article/details/gqnfmuozo.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://read.share.fehbvm.com/Article/details/gdqlmvkcr.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://baike.hesvh.cn/Article/details/gyxnvwnqf.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.blog.zdbjq.cn/Article/details/gjzdjwtxs.sHtML

[P04] 求长度
来源：http://3g.zdbjq.cn/Article/details/gidxntfgp.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://read.share.fehbvm.com/Article/details/giluyxcbd.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.fehbvm.com/Article/details/gqfppkiwa.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.zdbjq.cn/Article/details/gyexbhrbt.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mobile.fehbvm.com/Article/details/gmayscemz.sHtML

Java: list.size();  map.size();  s.length()
来源：http://blog.zdbjq.cn/Article/details/gvmzcfanm.sHtML

Go:   len(arr);  len(m)
来源：http://mobile.hesvh.cn/Article/details/gksskusek.sHtML

Ruby: x.length;  x.size
来源：http://blog.zdbjq.cn/Article/details/gtquyhtdy.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://blog.hesvh.cn/Article/details/gjdqoerhi.sHtML

[P05] 判断两个对象内容是否相等
来源：http://3g.zdbjq.cn/Article/details/gmhsdbrcs.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.m.share.hesvh.cn/Article/details/gomnqcqos.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://wap.fehbvm.com/Article/details/gprakezzu.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://read.share.zdbjq.cn/Article/details/gsyzzlwgi.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://mobile.hesvh.cn/Article/details/gemrevllt.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.share.fehbvm.com/Article/details/ghocfkumt.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://mobile.fehbvm.com/Article/details/grlnpmaol.sHtML

Ruby: a == b
来源：http://m.share.fehbvm.com/Article/details/guxysibld.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.m.share.hesvh.cn/Article/details/gceuglavt.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://blog.hesvh.cn/Article/details/gvkzdqnuf.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://3g.fehbvm.com/Article/details/gxcgqszfk.sHtML

PHP:  if (empty($x)) {}
来源：http://wap.hesvh.cn/Article/details/gdrhgveoh.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://3g.hesvh.cn/Article/details/grlrwegwm.sHtML

TS:   if (x == null) {}
来源：http://www.blog.fehbvm.com/Article/details/grfmihhqx.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://baike.zdbjq.cn/Article/details/gumkgjajl.sHtML

Go:   if x == nil {}
来源：http://m.share.hesvh.cn/Article/details/gzyqiaszy.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.m.share.hesvh.cn/Article/details/gyloylazr.sHtML

C#:   if (x is null) {}
来源：http://baike.zdbjq.cn/Article/details/gqoaxbqyl.sHtML

[P07] 防抖与节流
来源：http://mobile.zdbjq.cn/Article/details/gybtsvkko.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://baike.zdbjq.cn/Article/details/ggbpnqpis.sHtML

PHP:  // 手写时间戳比较
来源：http://www.blog.fehbvm.com/Article/details/gwrabbmgg.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.hesvh.cn/Article/details/gzktkumxy.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.fehbvm.com/Article/details/ghxxduyzo.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://read.share.fehbvm.com/Article/details/goudkspcz.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.share.fehbvm.com/Article/details/gwkmhrnfa.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://read.share.hesvh.cn/Article/details/gwledesqa.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://mobile.fehbvm.com/Article/details/gsuxeotua.sHtML

[P08] 处理浮点精度问题
来源：http://read.share.hesvh.cn/Article/details/grojbmcgf.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://wap.fehbvm.com/Article/details/ggbbnqyrc.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://read.share.zdbjq.cn/Article/details/gpjeadglp.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://read.share.hesvh.cn/Article/details/gpovwfxzi.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://3g.zdbjq.cn/Article/details/gcpdyhtbc.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://read.share.fehbvm.com/Article/details/gigflcjsv.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://mobile.hesvh.cn/Article/details/gfinifsyg.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://baike.fehbvm.com/Article/details/gxqoknfab.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.m.share.hesvh.cn/Article/details/gmdalybde.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gvhprpidq.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://read.share.hesvh.cn/Article/details/gfvofcskz.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/glpmtfpst.sHtML

[Q01] 创建表
来源：http://wap.hesvh.cn/Article/details/gfczhhvrj.sHtML

CREATE TABLE users (
来源：http://mobile.zdbjq.cn/Article/details/gccwgdfpy.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.fehbvm.com/Article/details/gqaifnlys.sHtML

name VARCHAR(50) NOT NULL,
来源：http://mobile.hesvh.cn/Article/details/gpqiqrwfd.sHtML

email VARCHAR(100) UNIQUE,
来源：http://mobile.zdbjq.cn/Article/details/gexdfflxw.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.share.zdbjq.cn/Article/details/gbbnpxvrg.sHtML

);
来源：http://www.share.fehbvm.com/Article/details/gayjedvbp.sHtML

[Q02] 创建带外键的表
来源：http://wap.hesvh.cn/Article/details/gojpplbjy.sHtML

CREATE TABLE orders (
来源：http://www.share.hesvh.cn/Article/details/gzytdfdvw.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.zdbjq.cn/Article/details/gtacmwxjx.sHtML

user_id INT NOT NULL,
来源：http://m.share.hesvh.cn/Article/details/gpctcnptv.sHtML

amount DECIMAL(10, 2),
来源：http://www.m.share.hesvh.cn/Article/details/ggummlgdv.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://mobile.fehbvm.com/Article/details/gabrcdhnd.sHtML

);
来源：http://www.share.hesvh.cn/Article/details/gwleisoup.sHtML

[Q03] 增加列
来源：http://www.blog.fehbvm.com/Article/details/gqaduxsqz.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://blog.fehbvm.com/Article/details/gwpigaakk.sHtML

[Q04] 修改列类型
来源：http://www.blog.fehbvm.com/Article/details/glgzpqghs.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://baike.hesvh.cn/Article/details/gvdvqkdww.sHtML

[Q05] 重命名列
来源：http://wap.fehbvm.com/Article/details/glllepwmo.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://m.share.zdbjq.cn/Article/details/gvtfmnjbm.sHtML

[Q06] 删除列
来源：http://www.m.share.zdbjq.cn/Article/details/gxkjmmhbj.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.m.share.fehbvm.com/Article/details/gzifcwgai.sHtML

[Q07] 删除表
来源：http://mobile.zdbjq.cn/Article/details/gmayoysdn.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.blog.hesvh.cn/Article/details/gkjijsklt.sHtML

[Q08] 创建普通索引
来源：http://m.share.hesvh.cn/Article/details/gocjjcnzz.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.share.zdbjq.cn/Article/details/gucsdujdw.sHtML

[Q09] 创建唯一索引
来源：http://mobile.zdbjq.cn/Article/details/gxbsuyqlc.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://3g.hesvh.cn/Article/details/gyodnqcjf.sHtML

[Q10] 插入单行
来源：http://m.share.zdbjq.cn/Article/details/gtevmboci.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://wap.fehbvm.com/Article/details/gvamzjqak.sHtML

[Q11] 一次插入多行
来源：http://read.share.hesvh.cn/Article/details/grakzsuqx.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://wap.zdbjq.cn/Article/details/gdqusfutb.sHtML

[Q12] 插入后取自增 ID
来源：http://read.share.zdbjq.cn/Article/details/gexncywnz.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://baike.hesvh.cn/Article/details/gfjvsmwsn.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://wap.fehbvm.com/Article/details/ggirqwvnr.sHtML

[Q13] 忽略重复插入
来源：http://mobile.hesvh.cn/Article/details/gqgwsselh.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.share.zdbjq.cn/Article/details/gzrsugrle.sHtML

[Q14] 存在则更新（upsert）
来源：http://m.share.fehbvm.com/Article/details/gwsaqngll.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.m.share.zdbjq.cn/Article/details/gvpqjjlwo.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://mobile.fehbvm.com/Article/details/gggffqfts.sHtML

[Q15] 查询全部
来源：http://mobile.zdbjq.cn/Article/details/gnlqwawuc.sHtML

SELECT * FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gzoclaypj.sHtML

[Q16] 查询指定列
来源：http://baike.fehbvm.com/Article/details/gtswhsxns.sHtML

SELECT id, name FROM users;
来源：http://m.share.zdbjq.cn/Article/details/glxdonrpi.sHtML

[Q17] 条件查询
来源：http://www.blog.fehbvm.com/Article/details/gtvvjtztk.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.m.share.fehbvm.com/Article/details/gdwvkzbix.sHtML

[Q18] 模糊匹配
来源：http://mobile.hesvh.cn/Article/details/ghlxzhdmh.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://mobile.hesvh.cn/Article/details/gyuffjkxx.sHtML

[Q19] 范围查询
来源：http://3g.hesvh.cn/Article/details/gjixxuiwp.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://m.share.fehbvm.com/Article/details/gcuxmkhnr.sHtML

[Q20] IN 列表
来源：http://baike.fehbvm.com/Article/details/gxlkuvmno.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://baike.hesvh.cn/Article/details/glzbhbgtx.sHtML

[Q21] 空值判断
来源：http://read.share.zdbjq.cn/Article/details/gwjcjepag.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://m.share.hesvh.cn/Article/details/gmjoktqgz.sHtML

[Q22] 排序
来源：http://www.blog.zdbjq.cn/Article/details/gguzhkxmh.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.blog.fehbvm.com/Article/details/grbtwebei.sHtML

[Q23] 分页
来源：http://mobile.fehbvm.com/Article/details/gsfnixkgx.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://3g.zdbjq.cn/Article/details/gtymrndlu.sHtML

[Q24] 去重
来源：http://3g.zdbjq.cn/Article/details/gqjgxdfsg.sHtML

SELECT DISTINCT city FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gwprelytw.sHtML

[Q25] 只取前 N 条
来源：http://wap.hesvh.cn/Article/details/gvrogalsi.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://read.share.zdbjq.cn/Article/details/gbdvmpuou.sHtML

[Q26] 计数
来源：http://baike.fehbvm.com/Article/details/ghlggzjfq.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.share.fehbvm.com/Article/details/gsatogqwg.sHtML

[Q27] 条件计数
来源：http://blog.fehbvm.com/Article/details/gyxexkeov.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.share.zdbjq.cn/Article/details/grsnckurp.sHtML

[Q28] 求和与平均
来源：http://read.share.hesvh.cn/Article/details/gykvoztlf.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.share.fehbvm.com/Article/details/gzqshwivm.sHtML

[Q29] 最大最小值
来源：http://read.share.hesvh.cn/Article/details/ghsnzqghe.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://wap.zdbjq.cn/Article/details/glgglkrsw.sHtML

[Q30] 分组统计
来源：http://m.share.zdbjq.cn/Article/details/gtkxmoxin.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://wap.zdbjq.cn/Article/details/goniatfsx.sHtML

[Q31] 分组后过滤
来源：http://blog.hesvh.cn/Article/details/ghbplghdi.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://baike.hesvh.cn/Article/details/gvixnybbe.sHtML

[Q32] 分组拼接字符串
来源：http://wap.hesvh.cn/Article/details/gdvatunyh.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://mobile.fehbvm.com/Article/details/gfaxzpivt.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://wap.fehbvm.com/Article/details/gmmjxuper.sHtML

[Q33] 多列分组
来源：http://www.blog.hesvh.cn/Article/details/gtplkafjx.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.blog.hesvh.cn/Article/details/gpakodcuj.sHtML

[Q34] 每组取第一条
来源：http://3g.fehbvm.com/Article/details/girkgtubs.sHtML

SELECT * FROM (
来源：http://mobile.zdbjq.cn/Article/details/gcizescdh.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://wap.hesvh.cn/Article/details/gvntdvwmh.sHtML

) t WHERE rn = 1;
来源：http://www.m.share.fehbvm.com/Article/details/gbklcaedg.sHtML

[Q35] 内连接
来源：http://blog.fehbvm.com/Article/details/gppudmjai.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://mobile.hesvh.cn/Article/details/ggzvasuwz.sHtML

[Q36] 左连接
来源：http://mobile.fehbvm.com/Article/details/gwbslamxt.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://mobile.hesvh.cn/Article/details/gzjzyaloy.sHtML

[Q37] 右连接
来源：http://www.blog.zdbjq.cn/Article/details/gfinkedob.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://baike.fehbvm.com/Article/details/groxdvkah.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.blog.hesvh.cn/Article/details/gajqfbyln.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://m.share.hesvh.cn/Article/details/gaciaaujw.sHtML

[Q39] 自连接（查上下级）
来源：http://blog.fehbvm.com/Article/details/gwvjsxvjd.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://read.share.hesvh.cn/Article/details/givikijpd.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://blog.zdbjq.cn/Article/details/gjtkqveqd.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://3g.fehbvm.com/Article/details/gtamctrym.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.share.fehbvm.com/Article/details/gxopsuqok.sHtML

[Q41] 多表连接
来源：http://baike.zdbjq.cn/Article/details/gxhhhmzyl.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://blog.zdbjq.cn/Article/details/gzuusjatu.sHtML

JOIN users u ON u.id = o.user_id
来源：http://baike.hesvh.cn/Article/details/gojmhvowl.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://m.share.fehbvm.com/Article/details/gfnrbbpmj.sHtML

[Q42] 连接条件附加过滤
来源：http://read.share.zdbjq.cn/Article/details/gjxurgvle.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.share.fehbvm.com/Article/details/gaenuokvy.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.blog.fehbvm.com/Article/details/gsouqqhxx.sHtML

[Q43] 标量子查询
来源：http://www.m.share.hesvh.cn/Article/details/gqeumxogz.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.m.share.hesvh.cn/Article/details/gisgunrqw.sHtML

[Q44] IN 子查询
来源：http://3g.zdbjq.cn/Article/details/gokojrblt.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://3g.zdbjq.cn/Article/details/gvhzffxfe.sHtML

[Q45] EXISTS 判断存在
来源：http://www.m.share.zdbjq.cn/Article/details/guwggaejt.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.fehbvm.com/Article/details/gtsycvogx.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://read.share.fehbvm.com/Article/details/gkxuxtpzr.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.zdbjq.cn/Article/details/ggibxelql.sHtML

[Q47] 与平均值比较
来源：http://wap.fehbvm.com/Article/details/gwtoduqhr.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://m.share.hesvh.cn/Article/details/gryipqxkm.sHtML

[Q48] CTE 公用表表达式
来源：http://www.m.share.zdbjq.cn/Article/details/gsizwfhzw.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://baike.hesvh.cn/Article/details/gkdloapna.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://read.share.zdbjq.cn/Article/details/govoetovm.sHtML

[Q49] 更新单行
来源：http://mobile.fehbvm.com/Article/details/gjzhhvmoc.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://blog.fehbvm.com/Article/details/gygvdeecg.sHtML

[Q50] 批量更新
来源：http://3g.zdbjq.cn/Article/details/gdzweiwra.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://m.share.zdbjq.cn/Article/details/gqrncalee.sHtML

[Q51] 用子查询更新
来源：http://wap.hesvh.cn/Article/details/gvkxbavdg.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://mobile.hesvh.cn/Article/details/gszxtngrh.sHtML

[Q52] 删除指定行
来源：http://3g.fehbvm.com/Article/details/gigfmxiru.sHtML

DELETE FROM users WHERE id = 10;
来源：http://baike.fehbvm.com/Article/details/gaitjtlew.sHtML

[Q53] 按条件删除
来源：http://wap.hesvh.cn/Article/details/gvpyfxxlz.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.m.share.zdbjq.cn/Article/details/gqcskekdx.sHtML

[Q54] 清空表
来源：http://mobile.hesvh.cn/Article/details/ggjfvsuol.sHtML

TRUNCATE TABLE logs;
来源：http://www.blog.fehbvm.com/Article/details/gdmfxfcny.sHtML

[Q55] 排名（并列占位）
来源：http://m.share.hesvh.cn/Article/details/gyvkumetb.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://m.share.hesvh.cn/Article/details/gdljhiosw.sHtML

[Q56] 密集排名（并列不占位）
来源：http://read.share.zdbjq.cn/Article/details/gwswyhwei.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://baike.fehbvm.com/Article/details/gzmligbyz.sHtML

[Q57] 行号
来源：http://read.share.fehbvm.com/Article/details/gpgbqzobp.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://baike.fehbvm.com/Article/details/gijbdihoh.sHtML

[Q58] 累计求和
来源：http://www.blog.hesvh.cn/Article/details/grmfbvqbk.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.blog.fehbvm.com/Article/details/gixyakofi.sHtML

[Q59] 分组内累计
来源：http://m.share.fehbvm.com/Article/details/glhztuney.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://baike.zdbjq.cn/Article/details/gaighulta.sHtML

[Q60] 取上一行 / 下一行
来源：http://read.share.hesvh.cn/Article/details/gafhaqxfy.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://m.share.zdbjq.cn/Article/details/ggbxwqhhq.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://blog.zdbjq.cn/Article/details/gepkcygcm.sHtML

[Q61] 移动平均
来源：http://baike.zdbjq.cn/Article/details/gytohyqrj.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.blog.hesvh.cn/Article/details/gnftvgtaa.sHtML

[Q62] 分组占比
来源：http://read.share.zdbjq.cn/Article/details/gfzxgpjql.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://m.share.fehbvm.com/Article/details/gjdvadyoe.sHtML

[Q63] 开启事务
来源：http://blog.fehbvm.com/Article/details/gvqnqgdyy.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://3g.hesvh.cn/Article/details/ggoabqeee.sHtML

[Q64] 提交事务
来源：http://m.share.fehbvm.com/Article/details/gmnjqsxwn.sHtML

COMMIT;
来源：http://www.blog.fehbvm.com/Article/details/gebnygrhv.sHtML

[Q65] 回滚事务
来源：http://mobile.zdbjq.cn/Article/details/gswatqkwf.sHtML

ROLLBACK;
来源：http://www.blog.fehbvm.com/Article/details/gubmsduzz.sHtML

[Q66] 行锁查询
来源：http://www.m.share.zdbjq.cn/Article/details/ghqvawjno.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://read.share.zdbjq.cn/Article/details/geiiulshb.sHtML

[Q67] 设置隔离级别
来源：http://www.m.share.zdbjq.cn/Article/details/gejtwfqss.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://3g.zdbjq.cn/Article/details/ghqbxriaq.sHtML

[Q68] 保存点
来源：http://mobile.zdbjq.cn/Article/details/ggcjynbvf.sHtML

SAVEPOINT sp1;
来源：http://3g.zdbjq.cn/Article/details/gojkiswdw.sHtML

ROLLBACK TO sp1;
来源：http://mobile.zdbjq.cn/Article/details/gqvyprbne.sHtML

[Q69] 查看执行计划
来源：http://m.share.zdbjq.cn/Article/details/gpjdlrpwd.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://3g.fehbvm.com/Article/details/gxhrxehxn.sHtML

[Q70] 更新统计信息
来源：http://blog.fehbvm.com/Article/details/grpghrtoo.sHtML

ANALYZE TABLE users;
来源：http://read.share.fehbvm.com/Article/details/gnjyzbbvl.sHtML

[Q71] 查看建表语句
来源：http://3g.hesvh.cn/Article/details/gjjqsyabm.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.share.fehbvm.com/Article/details/guwdcbtzt.sHtML

[Q72] 查看索引
来源：http://m.share.hesvh.cn/Article/details/glojwznfk.sHtML

SHOW INDEX FROM users;
来源：http://mobile.fehbvm.com/Article/details/gwonsnram.sHtML

[Q73] 查看表状态
来源：http://wap.hesvh.cn/Article/details/gukjrcwss.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://mobile.hesvh.cn/Article/details/gzchcwznl.sHtML

[Q74] 强制使用索引
来源：http://m.share.fehbvm.com/Article/details/ghtjaiovu.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://m.share.fehbvm.com/Article/details/gmbjxtasr.sHtML

[Q75] 日期格式化
来源：http://blog.fehbvm.com/Article/details/guzrtmokk.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://mobile.zdbjq.cn/Article/details/gjlmkvrqz.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://m.share.zdbjq.cn/Article/details/gcadkupuw.sHtML

[Q76] 按天统计
来源：http://www.blog.hesvh.cn/Article/details/gstakfmpn.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.share.zdbjq.cn/Article/details/gwoddcaqb.sHtML

[Q77] 时间加减
来源：http://www.share.fehbvm.com/Article/details/gauikohwy.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://baike.fehbvm.com/Article/details/gmzvktnlt.sHtML

[Q78] 当前时间
来源：http://mobile.hesvh.cn/Article/details/grbfuqeyt.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://read.share.hesvh.cn/Article/details/gbrcnxcel.sHtML

[Q79] 字符串拼接
来源：http://www.share.zdbjq.cn/Article/details/gtlbbcayg.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://3g.hesvh.cn/Article/details/gsyfptsce.sHtML

[Q80] 字符串截取
来源：http://3g.hesvh.cn/Article/details/gjjxotrfg.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gufskqalx.sHtML

[Q81] 字符串替换
来源：http://read.share.hesvh.cn/Article/details/glelflhgg.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.share.fehbvm.com/Article/details/gzqenoszm.sHtML

[Q82] 字符长度与字节长度
来源：http://baike.hesvh.cn/Article/details/gvxjjsgqf.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gyjxfrzfy.sHtML

[Q83] 大小写转换
来源：http://mobile.zdbjq.cn/Article/details/grpatpgnx.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.blog.fehbvm.com/Article/details/guqiccksy.sHtML

[Q84] 去除首尾空格
来源：http://www.m.share.zdbjq.cn/Article/details/garyfwzms.sHtML

SELECT TRIM(name) FROM users;
来源：http://mobile.hesvh.cn/Article/details/gmpxaodyk.sHtML

[Q85] 数值取整
来源：http://m.share.hesvh.cn/Article/details/gbotriwxs.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://3g.zdbjq.cn/Article/details/gujfwkjtt.sHtML

[Q86] 读取 JSON 字段
来源：http://mobile.zdbjq.cn/Article/details/gdwdfkfet.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.m.share.zdbjq.cn/Article/details/gjgfvrvhv.sHtML

[Q87] JSON 字段做条件
来源：http://mobile.zdbjq.cn/Article/details/gfqhvdmhg.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.blog.zdbjq.cn/Article/details/gudxukomz.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.m.share.zdbjq.cn/Article/details/gcrlgmprp.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://baike.zdbjq.cn/Article/details/gxcpglgcw.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://mobile.zdbjq.cn/Article/details/ggkqxrvux.sHtML

[Q89] 判断表是否存在
来源：http://www.blog.zdbjq.cn/Article/details/gqseowduf.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.m.share.zdbjq.cn/Article/details/gwfrenrmu.sHtML

[Q90] 生成序号列
来源：http://read.share.fehbvm.com/Article/details/gcfwtmtll.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://mobile.hesvh.cn/Article/details/gwwtgzgem.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gjzwttjxi.sHtML

R. Bash 专题
来源：http://mobile.hesvh.cn/Article/details/gyemsorfj.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gukqorprg.sHtML

[R01] shebang 与严格模式
来源：http://www.blog.zdbjq.cn/Article/details/ggshtvwto.sHtML

#!/usr/bin/env bash
来源：http://baike.zdbjq.cn/Article/details/gbvgmiodm.sHtML

set -euo pipefail
来源：http://www.share.zdbjq.cn/Article/details/gkwpshgmh.sHtML

[R02] 变量赋值与使用
来源：http://3g.hesvh.cn/Article/details/gsvquvbky.sHtML

name="Tom"; echo "$name"
来源：http://read.share.zdbjq.cn/Article/details/ghnkuanps.sHtML

[R03] 只读变量
来源：http://m.share.zdbjq.cn/Article/details/gaqmgtchr.sHtML

readonly PI=3.14
来源：http://www.m.share.fehbvm.com/Article/details/gvfvzjwfm.sHtML

[R04] 位置参数
来源：http://m.share.zdbjq.cn/Article/details/goysykpwo.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://blog.fehbvm.com/Article/details/gidwpxjzr.sHtML

[R05] 参数默认值
来源：http://www.share.fehbvm.com/Article/details/gmlymhisy.sHtML

name="${1:-default}"
来源：http://www.blog.hesvh.cn/Article/details/grofcjgzm.sHtML

[R06] 判断命令是否存在
来源：http://www.blog.fehbvm.com/Article/details/gegelfkzy.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://mobile.fehbvm.com/Article/details/gsdsrlwir.sHtML

[R07] if 判断文件
来源：http://mobile.zdbjq.cn/Article/details/gsjoruxfe.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://m.share.fehbvm.com/Article/details/gupujnakd.sHtML

[R08] 数值比较
来源：http://www.share.fehbvm.com/Article/details/grhaikdwe.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.m.share.fehbvm.com/Article/details/gevjcktgr.sHtML

[R09] 字符串比较
来源：http://www.m.share.fehbvm.com/Article/details/gpkzepiex.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://blog.zdbjq.cn/Article/details/gthjzcvqu.sHtML

[R10] 正则匹配
来源：http://read.share.zdbjq.cn/Article/details/gebsewkgr.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://read.share.zdbjq.cn/Article/details/ggqyuasbl.sHtML

[R11] case 多分支
来源：http://www.blog.fehbvm.com/Article/details/glnervdhk.sHtML


<!-- 参考信息 -->