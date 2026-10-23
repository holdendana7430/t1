代发 wailian999

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3prdskaat.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3cdyyhvme.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3dvwycqmz.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt3hjbvhvjk.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt3isudmhyy.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt3djymqgby.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt3altlqzeq.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt3cobdlwgp.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt3cndwschu.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt3kbgsxbhg.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3olopxmha.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt3elabpeia.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt3lglnoyqo.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt3jvkcfbxf.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt3ohrwnqrn.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt3mylmxlpj.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt3kyffpghm.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3bqtrbixp.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3rqjboqhr.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt3hmksstor.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt3mryrlrzl.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt3cdyiscpj.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt3iexyqsap.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt3vsnxgrhc.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt3ixumfcvm.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3uagnpjle.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3eodjyzib.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3blrrdtdg.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt3vcxaevqh.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt3dammvevc.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt3ohaolenr.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt3gyzfsxol.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt3euzpjcgq.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt3uloxwpmt.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt3frdiczgx.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt3mkffsthl.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3nxnemhvc.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt3qlxpsyvk.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3rqvdqgeb.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt3ibajqeqt.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt3ygimcezt.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt3pvquqrgr.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3ujtugrio.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3mchhtmlv.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt3fofpvtiv.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3fngocyhx.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3iaswwykx.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt3hlgczilf.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt3ikrfapyp.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3temxubbl.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt3amykvlfs.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt3wmblgxdr.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt3jvhprage.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3hsecbrwm.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3iiizreth.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt3uxusseqm.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt3sdjpplvd.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt3bvfwvgac.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt3jhfpyaah.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt3hznzckxb.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt3dokcqknp.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt3jrfysoca.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt3ejxmoxcx.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3cgvdutmq.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt3bgngpdsw.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt3cvnuiwlw.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt3zncczhfh.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt3ckgvvxai.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3yzfwkfoa.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt3qpmgwoqv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lcsksxuc.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt3vrtbbief.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt3mkznwftf.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3uryvbxpx.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3cbwtcedh.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt3rzfmihox.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt3bqzinncz.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3admbskns.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt3zapixxfd.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt3mbvwrgng.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3gjugllio.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3mxbmymlp.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt3wrztohsp.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt3elzzadbn.html

);
来源：http://www.52xcode.cn/Article/details/gt3zujjwutp.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt3vfbwghbg.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt3ejgumbub.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt3fwmaazkv.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3umbyvcxn.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt3glnnadkn.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt3qzjhchjf.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt3ergyivnx.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt3qdoentge.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt3owiyrbak.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt3fnnnzuys.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt3sroondgx.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3aokuebuv.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt3zbdraozu.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3duinbypa.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt3kuxmxmmp.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3zrgleqgd.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt3ifavktlh.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3izoervyh.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt3zaqamlhb.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt3vybpcjtt.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt3sfzwfjmv.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt3bacezkyk.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3tjaviysm.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt3zwkyrnew.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt3frdidcqp.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt3lpzqpegu.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt3uefebqwz.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt3badknyux.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt3wliqocit.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt3aospparm.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt3rpnkkyba.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3bcflzfla.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt3qrebwvsy.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt3ucjcdyqu.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt3ewvajsvo.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt3wiphlcyi.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt3makzteji.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt3xlsjzagk.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt3ywqldrnf.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt3bydzmfym.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt3dihpblmq.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt3erdykbkw.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt3vvjdxtib.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt3aooecelp.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3ivegzubz.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3pbduwhvt.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt3ldavgmoa.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt3qzghzsdo.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt3acpqgnxz.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3psykbpvo.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt3gwsonrjh.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt3zecvdlla.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt3hriawxyk.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3vyhfpeul.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt3rhypcofh.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3tyqoncuk.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt3snfhbhdh.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3hwywewij.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt3hnysezeb.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt3nqpiarqc.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3bkcminiw.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3msukjegg.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt3xrowokzj.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt3fyfltvbn.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt3irayopgh.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt3juximxss.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt3nmjkcmnc.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt3ijimkamo.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3dszzjwkp.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt3dhoapajj.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3mlcxdmmb.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt3mkeartnq.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3vjtrlqgb.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt3mqgfxrst.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt3sklywmgu.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt3owzrgzal.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt3epnwgjwl.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt3clbamtrg.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt3sfsqgxlv.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt3dlmkgcfb.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt3hzxncglv.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt3fnhwklgn.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt3zwhuiwru.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt3yziwwctz.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt3ngtabipz.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt3nygwyjrf.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt3wfenvekn.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt3wscdfbjk.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt3lodmrgbu.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt3obvgkjin.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt3wpgxgawg.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt3ghhekexj.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt3bpqzfutn.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt3sbogybjw.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3lyccpfpn.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt3exzgicon.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3ddwzuoba.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt3ccmvkeox.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt3ydaaqykw.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt3qnrdqjap.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt3ovhjoevj.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt3umnhfzyf.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt3wjzufron.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3kpwaesje.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt3lyyjzgeg.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt3iklmzvgd.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt3dfmvbxty.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt3aeihszxz.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt3fxvpyrzj.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3nrpuqkvw.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt3zkcqwodq.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3ydrtzhxc.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt3uqfjrtjl.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt3kxbmhpaa.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt3soqliaxn.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3qysohmwb.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt3fpzzbnij.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3hgxdiiuv.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt3bngayvhq.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt3dretibgq.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt3ihnsxpxe.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3bvcqhzlp.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt3zjydayes.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3eqbboymf.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt3dmhwxvhi.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt3uiuxpiyr.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3zasrkcst.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt3eqnrtunq.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3ubphtegp.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt3knrbynhh.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3wrrrdcnl.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt3wnrmboby.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt3aizhfvjf.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt3ufzipxwh.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt3ijvcodqg.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt3tabzrbcx.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt3lfktbkxk.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt3aqunecck.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt3rrdsfuzs.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt3qysgobdp.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt3ydkhrgbh.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt3chhsunuv.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3qcntxjxk.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt3pqaccayh.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt3sjitmhys.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt3hutbyaii.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt3nydwpqfu.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt3xitubnns.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt3nycqtvjp.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt3mkukfwyl.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt3mxcbelxk.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3yazokzfl.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt3qiptzsor.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3whbpzuut.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt3ltfnziwh.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt3aonbuvnf.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3kbltzapl.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3rauyxhmy.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt3mgsdxygi.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt3qqjsipkq.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt3klvzklnt.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt3ordliqoc.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt3hjdutfpb.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3ycqtrndu.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt3bubpvpyw.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3egtebozo.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt3pyetsdbk.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt3exfjkidf.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3rwfbpztv.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3zzraueiy.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt3zgtlmsyx.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt3uvbzasaz.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3lwpdoqei.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3uvpgmtxo.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3wukjelad.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt3apbcxyzz.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3mbwfkllm.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt3vndajcvp.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt3sdyxrmop.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt3hxjomnzp.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt3jwpjhlgd.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt3uchleufn.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt3rvrtzivs.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt3hhsnrvss.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt3jkdmesgh.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3iuzvssbn.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3gozmxngl.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3zupbcpxk.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt3uhryasee.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt3yymvqjhu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bjqwjkwf.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt3ejnuotjc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jgbwawye.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt3wlrmclld.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt3idutoauf.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt3gxraksoc.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt3bcuhrxte.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt3mwgcoaub.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt3nwqdopco.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt3alvqvxik.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt3sllxdxzq.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt3jlyelgyc.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt3wpqeiamv.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt3bfelzotr.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt3pnpyfwvc.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3welqiwjg.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt3yomxjvvw.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt3oqkagrwu.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt3vgrjzvos.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt3rlygomaz.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3iecpncjm.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3dblefldf.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt3lyymrozd.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3bbwqexbp.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt3tljprbxq.html


<!-- 参考信息 -->