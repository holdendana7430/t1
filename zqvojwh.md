代发 wailian999

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://mobile.fehbvm.com/Article/details/geyaaodnp.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://3g.hesvh.cn/Article/details/ggcxjamge.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://m.share.fehbvm.com/Article/details/gfeviocqv.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://m.share.zdbjq.cn/Article/details/gysbbejvi.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.m.share.hesvh.cn/Article/details/gfnadiebx.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://mobile.fehbvm.com/Article/details/gyfrqphwg.sHtML

[P03] 生成短随机字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gyjxrykxe.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.blog.fehbvm.com/Article/details/gfaygmlnu.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.blog.zdbjq.cn/Article/details/ggdhnaxks.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.fehbvm.com/Article/details/gybwblzdn.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.zdbjq.cn/Article/details/glkqxzzjs.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.share.fehbvm.com/Article/details/ggjjcylck.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.m.share.fehbvm.com/Article/details/gjgrznaia.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://3g.hesvh.cn/Article/details/ghiaysjbr.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://read.share.hesvh.cn/Article/details/gmipwjtcu.sHtML

[P04] 求长度
来源：http://blog.fehbvm.com/Article/details/gdhfhzcpc.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://m.share.hesvh.cn/Article/details/gxgofmprq.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.fehbvm.com/Article/details/ghovpnywj.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.hesvh.cn/Article/details/gbnfomboi.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.fehbvm.com/Article/details/gkocxfehr.sHtML

Java: list.size();  map.size();  s.length()
来源：http://3g.hesvh.cn/Article/details/gjvlvdcuz.sHtML

Go:   len(arr);  len(m)
来源：http://www.share.fehbvm.com/Article/details/gojwpsokt.sHtML

Ruby: x.length;  x.size
来源：http://www.share.zdbjq.cn/Article/details/gaevflurc.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://mobile.fehbvm.com/Article/details/gthfvcdip.sHtML

[P05] 判断两个对象内容是否相等
来源：http://m.share.hesvh.cn/Article/details/gbqtbkohk.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://blog.hesvh.cn/Article/details/grsvilbia.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://wap.hesvh.cn/Article/details/gtdnsfgty.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.share.hesvh.cn/Article/details/gdoqygoqt.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://read.share.hesvh.cn/Article/details/gzbjwnhgs.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://blog.fehbvm.com/Article/details/gkmuozbgl.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://read.share.zdbjq.cn/Article/details/gloobyjft.sHtML

Ruby: a == b
来源：http://read.share.fehbvm.com/Article/details/gcwaicvmm.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://read.share.hesvh.cn/Article/details/gzexlvzzt.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.m.share.zdbjq.cn/Article/details/gyqgeuuwq.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://wap.hesvh.cn/Article/details/ghbevrolw.sHtML

PHP:  if (empty($x)) {}
来源：http://www.share.zdbjq.cn/Article/details/gymrtuoay.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.m.share.zdbjq.cn/Article/details/gfbylzmpz.sHtML

TS:   if (x == null) {}
来源：http://www.m.share.fehbvm.com/Article/details/gyvgdrenr.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://m.share.fehbvm.com/Article/details/gvexojuus.sHtML

Go:   if x == nil {}
来源：http://blog.hesvh.cn/Article/details/ginvhrlbh.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://baike.zdbjq.cn/Article/details/gwcxyvsyz.sHtML

C#:   if (x is null) {}
来源：http://mobile.zdbjq.cn/Article/details/gabhkzcle.sHtML

[P07] 防抖与节流
来源：http://www.m.share.zdbjq.cn/Article/details/glpeuwjnx.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.m.share.hesvh.cn/Article/details/gahlhsksx.sHtML

PHP:  // 手写时间戳比较
来源：http://wap.zdbjq.cn/Article/details/gvdvrmvfr.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.zdbjq.cn/Article/details/gagwrqtxf.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.zdbjq.cn/Article/details/gowooqvgg.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://read.share.zdbjq.cn/Article/details/gmiwghatf.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://baike.zdbjq.cn/Article/details/gjvhnlkes.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://read.share.fehbvm.com/Article/details/gvcaktwcv.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://wap.hesvh.cn/Article/details/gaiqdekab.sHtML

[P08] 处理浮点精度问题
来源：http://3g.fehbvm.com/Article/details/gxqmxejak.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://m.share.hesvh.cn/Article/details/gnznvusrj.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://wap.hesvh.cn/Article/details/gsdkfxebm.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://3g.hesvh.cn/Article/details/grmkklqwl.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.m.share.hesvh.cn/Article/details/glnkkywgz.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://m.share.hesvh.cn/Article/details/gmxzyesbj.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://m.share.zdbjq.cn/Article/details/gxvugnfyb.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.blog.hesvh.cn/Article/details/gcuttwtxd.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://m.share.fehbvm.com/Article/details/gmwztnbrg.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gujfretxu.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.share.zdbjq.cn/Article/details/gwnayowav.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gqjahcxfr.sHtML

[Q01] 创建表
来源：http://read.share.fehbvm.com/Article/details/grjzatyps.sHtML

CREATE TABLE users (
来源：http://www.share.fehbvm.com/Article/details/gwgupcvog.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.hesvh.cn/Article/details/ghewqwtnb.sHtML

name VARCHAR(50) NOT NULL,
来源：http://wap.zdbjq.cn/Article/details/gixgvjyhq.sHtML

email VARCHAR(100) UNIQUE,
来源：http://baike.zdbjq.cn/Article/details/gxvcqowte.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://read.share.hesvh.cn/Article/details/gmzvdmnhh.sHtML

);
来源：http://read.share.fehbvm.com/Article/details/gxacnmpmv.sHtML

[Q02] 创建带外键的表
来源：http://mobile.hesvh.cn/Article/details/greqtdggd.sHtML

CREATE TABLE orders (
来源：http://www.m.share.hesvh.cn/Article/details/gpjbhlrlx.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.share.fehbvm.com/Article/details/gxuoyxruy.sHtML

user_id INT NOT NULL,
来源：http://m.share.fehbvm.com/Article/details/gwaesmzpa.sHtML

amount DECIMAL(10, 2),
来源：http://3g.fehbvm.com/Article/details/gedmvmjld.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.share.hesvh.cn/Article/details/gedebmkul.sHtML

);
来源：http://read.share.zdbjq.cn/Article/details/gxkydnpqd.sHtML

[Q03] 增加列
来源：http://3g.fehbvm.com/Article/details/gqhxegqxs.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://read.share.hesvh.cn/Article/details/gqmscwcal.sHtML

[Q04] 修改列类型
来源：http://wap.hesvh.cn/Article/details/gutswngkd.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://blog.hesvh.cn/Article/details/gmirycgtc.sHtML

[Q05] 重命名列
来源：http://blog.zdbjq.cn/Article/details/gwnihszsg.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://baike.hesvh.cn/Article/details/guizmqhfa.sHtML

[Q06] 删除列
来源：http://www.blog.fehbvm.com/Article/details/gjapcmrkg.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://3g.zdbjq.cn/Article/details/gnqvfybsj.sHtML

[Q07] 删除表
来源：http://3g.zdbjq.cn/Article/details/gubnrnhrd.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.share.fehbvm.com/Article/details/ghsotnpin.sHtML

[Q08] 创建普通索引
来源：http://m.share.fehbvm.com/Article/details/gjbnhoqij.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://read.share.zdbjq.cn/Article/details/glqckpuut.sHtML

[Q09] 创建唯一索引
来源：http://3g.fehbvm.com/Article/details/godthwcer.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.share.fehbvm.com/Article/details/gudfokcqc.sHtML

[Q10] 插入单行
来源：http://www.share.zdbjq.cn/Article/details/gbfltcnhu.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://3g.hesvh.cn/Article/details/gpkjfshun.sHtML

[Q11] 一次插入多行
来源：http://read.share.hesvh.cn/Article/details/gofqoconj.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://blog.hesvh.cn/Article/details/gnumanuwn.sHtML

[Q12] 插入后取自增 ID
来源：http://read.share.hesvh.cn/Article/details/gvxtrigoj.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://3g.hesvh.cn/Article/details/gqjqwzurj.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://wap.hesvh.cn/Article/details/gdmvctfqi.sHtML

[Q13] 忽略重复插入
来源：http://www.m.share.hesvh.cn/Article/details/gvswmtlpy.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://wap.zdbjq.cn/Article/details/gpxhbjncw.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.blog.hesvh.cn/Article/details/gguycugev.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://baike.zdbjq.cn/Article/details/gtgwoxiqp.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://blog.fehbvm.com/Article/details/govqeiwwz.sHtML

[Q15] 查询全部
来源：http://read.share.hesvh.cn/Article/details/gtretwbup.sHtML

SELECT * FROM users;
来源：http://baike.hesvh.cn/Article/details/gnspuhzpn.sHtML

[Q16] 查询指定列
来源：http://mobile.hesvh.cn/Article/details/gnhaejhsq.sHtML

SELECT id, name FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gtecqmhdv.sHtML

[Q17] 条件查询
来源：http://www.blog.zdbjq.cn/Article/details/gvcsjevir.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://m.share.fehbvm.com/Article/details/gziivjply.sHtML

[Q18] 模糊匹配
来源：http://m.share.zdbjq.cn/Article/details/gwacvfdcu.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://mobile.fehbvm.com/Article/details/gpwnxlxgq.sHtML

[Q19] 范围查询
来源：http://3g.hesvh.cn/Article/details/gfszxpmzr.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.m.share.fehbvm.com/Article/details/gnpxxzxly.sHtML

[Q20] IN 列表
来源：http://mobile.fehbvm.com/Article/details/gnaakeclo.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://m.share.fehbvm.com/Article/details/gyyosglwo.sHtML

[Q21] 空值判断
来源：http://wap.hesvh.cn/Article/details/gewghgnii.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://m.share.fehbvm.com/Article/details/govplvvrz.sHtML

[Q22] 排序
来源：http://wap.hesvh.cn/Article/details/gyytylbnz.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://wap.hesvh.cn/Article/details/gsjpkcyfx.sHtML

[Q23] 分页
来源：http://wap.zdbjq.cn/Article/details/gsbidmdnf.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.share.zdbjq.cn/Article/details/gfqhycgim.sHtML

[Q24] 去重
来源：http://3g.hesvh.cn/Article/details/gucqxeslt.sHtML

SELECT DISTINCT city FROM users;
来源：http://3g.hesvh.cn/Article/details/gnuzuzswm.sHtML

[Q25] 只取前 N 条
来源：http://read.share.fehbvm.com/Article/details/gqfduzxok.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.share.fehbvm.com/Article/details/gwkjljwyq.sHtML

[Q26] 计数
来源：http://www.m.share.fehbvm.com/Article/details/ggjdlhlch.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gxbnferiq.sHtML

[Q27] 条件计数
来源：http://www.share.hesvh.cn/Article/details/gpogywrqh.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://m.share.hesvh.cn/Article/details/gkwvomhub.sHtML

[Q28] 求和与平均
来源：http://blog.hesvh.cn/Article/details/gyzcxflha.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://wap.hesvh.cn/Article/details/gxcqzgxzh.sHtML

[Q29] 最大最小值
来源：http://mobile.zdbjq.cn/Article/details/gsxfmopwy.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://3g.hesvh.cn/Article/details/gwmbxxfgv.sHtML

[Q30] 分组统计
来源：http://www.blog.fehbvm.com/Article/details/gighesnhc.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://3g.fehbvm.com/Article/details/gkydfmrgz.sHtML

[Q31] 分组后过滤
来源：http://read.share.hesvh.cn/Article/details/gusiwboaf.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://3g.hesvh.cn/Article/details/gokblxjeg.sHtML

[Q32] 分组拼接字符串
来源：http://www.blog.hesvh.cn/Article/details/gnrzzdiof.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.share.zdbjq.cn/Article/details/guffqcybp.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://m.share.hesvh.cn/Article/details/gspecljsa.sHtML

[Q33] 多列分组
来源：http://3g.hesvh.cn/Article/details/gwkwcbjnn.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.m.share.zdbjq.cn/Article/details/gurpodoyy.sHtML

[Q34] 每组取第一条
来源：http://wap.fehbvm.com/Article/details/gofxgseml.sHtML

SELECT * FROM (
来源：http://www.share.zdbjq.cn/Article/details/gswbqyflv.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://read.share.hesvh.cn/Article/details/gpypuvmhz.sHtML

) t WHERE rn = 1;
来源：http://www.share.zdbjq.cn/Article/details/gsedzyvjt.sHtML

[Q35] 内连接
来源：http://m.share.zdbjq.cn/Article/details/gzfbmokxv.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://3g.fehbvm.com/Article/details/gyjimosnz.sHtML

[Q36] 左连接
来源：http://3g.hesvh.cn/Article/details/gepgiifhi.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://3g.fehbvm.com/Article/details/gsatiyyar.sHtML

[Q37] 右连接
来源：http://wap.hesvh.cn/Article/details/gqgcyxjny.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://m.share.fehbvm.com/Article/details/gtxafopko.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://read.share.hesvh.cn/Article/details/glduaihhi.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://3g.hesvh.cn/Article/details/gylsbolhh.sHtML

[Q39] 自连接（查上下级）
来源：http://www.share.zdbjq.cn/Article/details/gmbyqziya.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.blog.fehbvm.com/Article/details/gxauhtxhg.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://baike.fehbvm.com/Article/details/gufxexmmv.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://read.share.hesvh.cn/Article/details/gjuqhprwi.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.share.zdbjq.cn/Article/details/gardqhfgy.sHtML

[Q41] 多表连接
来源：http://blog.zdbjq.cn/Article/details/gqfequsyw.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://mobile.fehbvm.com/Article/details/gslosqoea.sHtML

JOIN users u ON u.id = o.user_id
来源：http://blog.fehbvm.com/Article/details/gaypjayve.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://baike.zdbjq.cn/Article/details/gtovfdxbq.sHtML

[Q42] 连接条件附加过滤
来源：http://blog.fehbvm.com/Article/details/gmdqijayj.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.blog.zdbjq.cn/Article/details/gdwzhurmg.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://baike.hesvh.cn/Article/details/gxckyozkl.sHtML

[Q43] 标量子查询
来源：http://www.m.share.fehbvm.com/Article/details/gqvgyunbx.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://read.share.fehbvm.com/Article/details/gewebuuga.sHtML

[Q44] IN 子查询
来源：http://m.share.fehbvm.com/Article/details/gtxtpxqsr.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.blog.hesvh.cn/Article/details/gkvdpqdoy.sHtML

[Q45] EXISTS 判断存在
来源：http://read.share.zdbjq.cn/Article/details/gftpxzibf.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.hesvh.cn/Article/details/gwqhfggon.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://read.share.hesvh.cn/Article/details/gmfeptqrc.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.fehbvm.com/Article/details/gaahsksrk.sHtML

[Q47] 与平均值比较
来源：http://baike.fehbvm.com/Article/details/gztzxztka.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://baike.zdbjq.cn/Article/details/garzbqjjn.sHtML

[Q48] CTE 公用表表达式
来源：http://read.share.hesvh.cn/Article/details/gbmvfpdpe.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.share.zdbjq.cn/Article/details/gqbgenbob.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://baike.zdbjq.cn/Article/details/ggywxfrgm.sHtML

[Q49] 更新单行
来源：http://www.blog.hesvh.cn/Article/details/gpuueijze.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://baike.zdbjq.cn/Article/details/gaoomxqqs.sHtML

[Q50] 批量更新
来源：http://baike.hesvh.cn/Article/details/ggedzgbvt.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://baike.zdbjq.cn/Article/details/gdcrtqxtl.sHtML

[Q51] 用子查询更新
来源：http://read.share.hesvh.cn/Article/details/gfvqnjkah.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://m.share.zdbjq.cn/Article/details/gpwjkjomf.sHtML

[Q52] 删除指定行
来源：http://read.share.fehbvm.com/Article/details/gjvitclbd.sHtML

DELETE FROM users WHERE id = 10;
来源：http://mobile.hesvh.cn/Article/details/gtjcnnxuz.sHtML

[Q53] 按条件删除
来源：http://3g.zdbjq.cn/Article/details/gmtismqrr.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://mobile.fehbvm.com/Article/details/gojjtkbxn.sHtML

[Q54] 清空表
来源：http://www.blog.zdbjq.cn/Article/details/gafwmvgrk.sHtML

TRUNCATE TABLE logs;
来源：http://mobile.fehbvm.com/Article/details/gyliexurw.sHtML

[Q55] 排名（并列占位）
来源：http://baike.fehbvm.com/Article/details/gxprfbbap.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://blog.fehbvm.com/Article/details/grvmeufat.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.share.fehbvm.com/Article/details/gmishejnf.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://wap.fehbvm.com/Article/details/gpwjxrsbr.sHtML

[Q57] 行号
来源：http://read.share.hesvh.cn/Article/details/gyccomica.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gqscpyzmf.sHtML

[Q58] 累计求和
来源：http://blog.hesvh.cn/Article/details/ggqywfwdw.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://3g.fehbvm.com/Article/details/glplctcxj.sHtML

[Q59] 分组内累计
来源：http://blog.fehbvm.com/Article/details/ghswisesp.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://blog.fehbvm.com/Article/details/gxkamkzla.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.blog.zdbjq.cn/Article/details/gqxulchxd.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://baike.zdbjq.cn/Article/details/ggnqatfbt.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.blog.zdbjq.cn/Article/details/gcrxkxcuy.sHtML

[Q61] 移动平均
来源：http://blog.hesvh.cn/Article/details/goaollwxk.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://m.share.zdbjq.cn/Article/details/gtwxypvoc.sHtML

[Q62] 分组占比
来源：http://baike.hesvh.cn/Article/details/gshucjmgr.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://blog.hesvh.cn/Article/details/gtnqsyyko.sHtML

[Q63] 开启事务
来源：http://www.blog.zdbjq.cn/Article/details/gtcmhzbln.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.blog.hesvh.cn/Article/details/ghzgiktzr.sHtML

[Q64] 提交事务
来源：http://mobile.hesvh.cn/Article/details/gxdsiyyhb.sHtML

COMMIT;
来源：http://3g.fehbvm.com/Article/details/gpjwkhbhm.sHtML

[Q65] 回滚事务
来源：http://3g.fehbvm.com/Article/details/gjfehqqvp.sHtML

ROLLBACK;
来源：http://3g.hesvh.cn/Article/details/gwcdsskvb.sHtML

[Q66] 行锁查询
来源：http://baike.zdbjq.cn/Article/details/gyfgwpsth.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.m.share.hesvh.cn/Article/details/gmwgvfdjx.sHtML

[Q67] 设置隔离级别
来源：http://read.share.hesvh.cn/Article/details/gcpfzsppw.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://mobile.fehbvm.com/Article/details/gyfoovxbn.sHtML

[Q68] 保存点
来源：http://www.share.zdbjq.cn/Article/details/gpgwtdryt.sHtML

SAVEPOINT sp1;
来源：http://www.m.share.fehbvm.com/Article/details/gusvljaav.sHtML

ROLLBACK TO sp1;
来源：http://mobile.fehbvm.com/Article/details/gbquommlf.sHtML

[Q69] 查看执行计划
来源：http://www.share.zdbjq.cn/Article/details/gkhchzxiy.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://wap.zdbjq.cn/Article/details/gmrpvbmle.sHtML

[Q70] 更新统计信息
来源：http://wap.hesvh.cn/Article/details/ggvafwsbj.sHtML

ANALYZE TABLE users;
来源：http://wap.fehbvm.com/Article/details/gwpgefvha.sHtML

[Q71] 查看建表语句
来源：http://wap.zdbjq.cn/Article/details/ghwurvehb.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://wap.hesvh.cn/Article/details/gcpftexkv.sHtML

[Q72] 查看索引
来源：http://read.share.hesvh.cn/Article/details/gkemuevit.sHtML

SHOW INDEX FROM users;
来源：http://wap.fehbvm.com/Article/details/gkjpizype.sHtML

[Q73] 查看表状态
来源：http://www.share.fehbvm.com/Article/details/gjtlamcls.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.share.fehbvm.com/Article/details/gffsxkvjz.sHtML

[Q74] 强制使用索引
来源：http://3g.zdbjq.cn/Article/details/goydcwtrf.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.blog.zdbjq.cn/Article/details/gitjrnkal.sHtML

[Q75] 日期格式化
来源：http://mobile.zdbjq.cn/Article/details/grxpfchkd.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.share.hesvh.cn/Article/details/gedwahbja.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.m.share.fehbvm.com/Article/details/gwcakipfj.sHtML

[Q76] 按天统计
来源：http://www.m.share.fehbvm.com/Article/details/gprrixuqp.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://blog.zdbjq.cn/Article/details/gwakqemni.sHtML

[Q77] 时间加减
来源：http://m.share.hesvh.cn/Article/details/gqmtejfzk.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://baike.zdbjq.cn/Article/details/gotyaggxa.sHtML

[Q78] 当前时间
来源：http://read.share.hesvh.cn/Article/details/gozxuewqs.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://3g.hesvh.cn/Article/details/gbmggsltp.sHtML

[Q79] 字符串拼接
来源：http://read.share.hesvh.cn/Article/details/gzetoevat.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://baike.zdbjq.cn/Article/details/gjuqyspsj.sHtML

[Q80] 字符串截取
来源：http://read.share.zdbjq.cn/Article/details/ggnukhtuz.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://m.share.fehbvm.com/Article/details/gxbbcyray.sHtML

[Q81] 字符串替换
来源：http://www.m.share.zdbjq.cn/Article/details/gtdcpgixb.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://wap.hesvh.cn/Article/details/gkwafdycw.sHtML

[Q82] 字符长度与字节长度
来源：http://www.m.share.fehbvm.com/Article/details/gepqckkhk.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://wap.zdbjq.cn/Article/details/gvfgqnbsv.sHtML

[Q83] 大小写转换
来源：http://3g.fehbvm.com/Article/details/gxknghnoz.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://mobile.hesvh.cn/Article/details/gfwiemwvy.sHtML

[Q84] 去除首尾空格
来源：http://www.m.share.hesvh.cn/Article/details/gicytyuvz.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.share.hesvh.cn/Article/details/gklixavmy.sHtML

[Q85] 数值取整
来源：http://baike.zdbjq.cn/Article/details/gpmekbzca.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://wap.fehbvm.com/Article/details/gbmesodtu.sHtML

[Q86] 读取 JSON 字段
来源：http://m.share.fehbvm.com/Article/details/gtslqjgzv.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://read.share.zdbjq.cn/Article/details/girndsaca.sHtML

[Q87] JSON 字段做条件
来源：http://3g.fehbvm.com/Article/details/glfdomhto.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.blog.zdbjq.cn/Article/details/gxzvtbapr.sHtML

[Q88] 行转列（条件聚合）
来源：http://m.share.fehbvm.com/Article/details/gpnjmgsby.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://m.share.zdbjq.cn/Article/details/gtznkybsr.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://wap.hesvh.cn/Article/details/gqrcolluw.sHtML

[Q89] 判断表是否存在
来源：http://3g.zdbjq.cn/Article/details/glsvigyby.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://blog.hesvh.cn/Article/details/gftogwytb.sHtML

[Q90] 生成序号列
来源：http://blog.hesvh.cn/Article/details/gjfjcvqzj.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://baike.fehbvm.com/Article/details/gwhlehbnb.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/ggdqmwisy.sHtML

R. Bash 专题
来源：http://www.blog.hesvh.cn/Article/details/gwsrtfrkd.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/geosymnmj.sHtML

[R01] shebang 与严格模式
来源：http://wap.zdbjq.cn/Article/details/guvxrfnea.sHtML

#!/usr/bin/env bash
来源：http://baike.fehbvm.com/Article/details/gwnrinfsm.sHtML

set -euo pipefail
来源：http://m.share.hesvh.cn/Article/details/gtjkwzrob.sHtML

[R02] 变量赋值与使用
来源：http://baike.zdbjq.cn/Article/details/gmtkyzucl.sHtML

name="Tom"; echo "$name"
来源：http://www.m.share.zdbjq.cn/Article/details/gxmivvsye.sHtML

[R03] 只读变量
来源：http://read.share.hesvh.cn/Article/details/gkxnugrxb.sHtML

readonly PI=3.14
来源：http://read.share.fehbvm.com/Article/details/gkfpqwpuh.sHtML

[R04] 位置参数
来源：http://www.m.share.hesvh.cn/Article/details/gfoxygnft.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://m.share.fehbvm.com/Article/details/gxhgshccz.sHtML

[R05] 参数默认值
来源：http://wap.hesvh.cn/Article/details/gnzuaydwo.sHtML

name="${1:-default}"
来源：http://3g.hesvh.cn/Article/details/gcuayugke.sHtML

[R06] 判断命令是否存在
来源：http://www.share.fehbvm.com/Article/details/gktrqopfj.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://m.share.fehbvm.com/Article/details/gwpavkkzy.sHtML

[R07] if 判断文件
来源：http://www.m.share.fehbvm.com/Article/details/grvzkizvv.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.share.zdbjq.cn/Article/details/gwdqxsifa.sHtML

[R08] 数值比较
来源：http://blog.zdbjq.cn/Article/details/gfcbbqolu.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.blog.hesvh.cn/Article/details/geuajifct.sHtML

[R09] 字符串比较
来源：http://3g.zdbjq.cn/Article/details/glyzaxjie.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://read.share.hesvh.cn/Article/details/grpbsxgmo.sHtML

[R10] 正则匹配
来源：http://www.m.share.fehbvm.com/Article/details/gmplqrfck.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://read.share.hesvh.cn/Article/details/gtkqfeiqe.sHtML

[R11] case 多分支
来源：http://read.share.fehbvm.com/Article/details/grybhnwav.sHtML

case "$1" in
来源：http://wap.hesvh.cn/Article/details/ggnmztoti.sHtML

start) echo "启动" ;;
来源：http://www.blog.zdbjq.cn/Article/details/gwwyjhwvu.sHtML

stop)  echo "停止" ;;
来源：http://read.share.zdbjq.cn/Article/details/gtnhcdzqq.sHtML

*)     echo "未知命令" ;;
来源：http://blog.hesvh.cn/Article/details/gzciqslvh.sHtML

esac
来源：http://baike.fehbvm.com/Article/details/gdbaofhhs.sHtML

[R12] for 遍历文件
来源：http://read.share.fehbvm.com/Article/details/grehpuqqx.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.share.fehbvm.com/Article/details/gaufwxqsu.sHtML

[R13] for 计数循环
来源：http://www.m.share.zdbjq.cn/Article/details/gupwzowmm.sHtML


<!-- 参考信息 -->