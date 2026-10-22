代发 wailian999

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2zofldtxe.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2ljuoihal.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2vrceveeg.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt2hufnrjdv.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2egfwlvtm.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt2yeoqoonz.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt2fffdetmy.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt2xuthdkwd.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt2jpoxlegf.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt2ikrvohkb.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2oguaaros.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt2ztwtgbwu.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt2tygyfvbd.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt2tkkfdecq.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt2ynxylfal.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt2bydcnths.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt2rauagscz.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2friiulft.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2auzhqayx.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt2xagaaaag.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt2vrrhbpma.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt2euzdglfg.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt2hbumbwmz.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt2wofapmmw.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt2njjghwhf.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2fbxrswsi.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2hrpteeax.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2meiawasp.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2yfgfbidu.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt2ohcjgkjw.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt2wgiazgvx.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt2xettmosb.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt2golskpis.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt2cofhalsa.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt2wzxdqwxv.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt2zglphxak.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2gcsyjooz.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt2ewxwctmr.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2kippnwqx.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt2higcvswq.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt2udessspa.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt2asroopia.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2aymvjbww.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt2jdfcnqcu.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt2ilbiprhs.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2higmemfy.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2vmyfymsy.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt2spkdlauu.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt2olghsjft.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2popvfhrz.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt2iyogbwpn.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt2doccmuep.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt2otuzswht.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2ipucecsh.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2jcbwrqsq.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt2oqwcqztt.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt2kligsrcs.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt2qbhcxrst.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt2apkmtsrn.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt2mwaqhmud.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt2lbdxsaqu.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt2shlculce.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt2lrjqgnjr.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2manarkik.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt2gwlmgyzu.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt2qkspzfjq.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt2kaqecbxs.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt2hvfbqziv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xhqalefc.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt2tqwzanxz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ukjyhsqw.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt2rnavisgs.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt2qyhfwejg.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2pnhqneii.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2xrwktqny.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt2priirdvx.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt2jiqwoxif.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2jfcspwub.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt2znerjnqx.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt2ykiwlznv.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2qvzidbvj.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2ysihqxgl.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt2hbieaehf.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt2yiogvygn.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2ppgcoqmk.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt2jgfmfwdy.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt2htqumore.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt2vamyqhxv.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2yfiduefw.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt2dvpodzfd.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt2ezffbrjb.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt2llleysch.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt2iievhvoz.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt2ixhfuisu.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt2jfczkpqy.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt2mpjavlil.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2aosapboo.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt2qhpcveuy.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2rttgniel.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt2vbojmfon.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt2pkngkzgz.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt2zcyzejyk.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2xrhsltrf.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt2yhayxfyc.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt2ndarjrro.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt2uiunglcp.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt2vqgccqvf.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt2mqjcefpz.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt2ahgryfva.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt2cpfrmrwu.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt2fhzqklah.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt2sflquhnr.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt2fjhczlde.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt2clrrmnzd.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2vgnajyfz.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt2mioqmhwq.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2khrcwhed.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt2ayquvvlh.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt2cegdisvf.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt2xgqyrcrx.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt2pqcdzmdz.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt2fdauwzof.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt2ytqlypdr.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt2yuodtzti.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt2krvjunzb.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt2bkgynmsm.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt2zoaapfzb.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt2nfkkpnoz.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt2oprjpvgt.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt2eelxlpjh.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2dqbmvypl.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt2fvevckml.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt2jouzzasl.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt2ifqkznrl.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2mboknsoc.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt2ixwcdojb.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2jgbaktjq.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt2bdylexcu.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2nhybvatq.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2dhdfihcd.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2iwsaaiyq.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt2redrdwms.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2gbfnxmyg.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt2keyeknjc.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt2stsggwkt.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2omwuwbar.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2ieofpvqm.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt2eoyuoalo.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt2mufbwqwf.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt2axdzptpv.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt2uesptwvy.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt2nypvlzbp.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt2huqswzik.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2yyhdgbgg.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt2maasrsfu.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2wnnketam.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt2ocqydaod.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2lgkmxxkp.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt2goborhjy.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt2efwmuisj.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt2xobxxqgm.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt2rveepjaq.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt2zvdykfeq.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt2ihcvlozl.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt2mafoizgi.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt2nunayvsz.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt2wxmgcexl.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt2aaolkper.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt2yocclqtz.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt2rpdmrvug.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt2boqnsiyz.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt2rbbvspcx.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt2ziyihywn.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt2seiycqlg.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt2iekkoihl.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt2plruanoo.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt2hyqouauo.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt2wzhbzyro.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt2kngmrjiw.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2osaqkqln.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt2ytzjkqjk.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2ktgmldra.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt2mhubzado.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt2lxkypczg.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt2eiodwida.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt2uoymfwst.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt2wlsurvsm.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt2doeabijz.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2xegqzycx.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt2bnpapoof.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2xbiwjkhu.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt2uvwyrgli.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt2owznuawf.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt2nwtzmjix.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2lfiatahk.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt2fmafbnjs.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2qsrhpiri.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt2rlynkfxc.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt2koaypdzm.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt2rwhbugkh.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2xgjlndcr.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt2huzwrplp.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2rrmteqag.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt2arvnqiqx.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ijuoalyf.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt2gyyvmowx.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2cwwgbrla.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt2cbwhxyld.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2dkyxlqyk.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt2sqdsblhn.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt2nfzdibok.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2wyaecepr.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt2spguckxb.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2pqinokka.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt2rvsyscsi.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2apvuyrqn.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt2fiodsfvl.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt2bvdwnaaq.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt2mfztodxj.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt2zjjtwlxd.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt2cvjuqodw.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt2eflcvzsm.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt2ddlzpltd.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt2yncocldf.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt2mayjmlvu.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt2lhnbxmtp.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt2bsalxyfp.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt2lwyzgrvc.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt2spjctqqk.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt2fgmflixd.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt2qppqwoqx.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt2stfjouye.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt2hrbruzje.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt2rqlfcnvm.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt2eicguihv.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt2uhoujhox.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt2peiluosg.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt2tefpuyex.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2vgrzmier.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt2tcubpypc.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt2cynsaulc.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2uijddhyu.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2hriftzcb.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt2bmuyncaa.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt2yyacvcru.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt2mcpkexsb.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt2bqlgngfh.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt2vooczqzb.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2enwegjig.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt2aqpjxmjp.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2qbkreokh.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt2elaafjqy.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt2ihzvgkck.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ofqmabcb.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2uymraghj.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt2kikqwity.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt2bodgantx.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2qflmpvdi.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2dnohbdee.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ewcxxckv.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt2ylvfjvlj.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2gbfijaqr.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt2ljeuviyy.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt2bctbaaup.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt2kbyfrlvw.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt2grwfufti.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt2pwrhnglw.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt2boloncoy.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt2fiblzgld.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt2xgegdgal.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2aqkumapq.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt2zyqfjxbd.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2jheawqsj.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt2oyemehih.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt2wheltqou.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2aqbzlaik.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt2ydqlcyvj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2acymbgwd.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt2gtxogtdm.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt2sauhfrky.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt2mpwqeusf.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt2hxffhsox.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt2bghfssmj.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2vqochnrp.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt2doyotrsp.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt2qsneqonz.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt2yolvztar.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt2ycextpec.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt2kivbbhri.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2nqsblgtw.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2rldpmhbv.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt2ybfmeohm.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt2siqtqmik.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt2dcwqzsoe.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt2dxmjlbwk.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2ypxrqtrj.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2deftzbgm.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt2guydwcik.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2ddfpklks.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt2sotdumzi.html


<!-- 参考信息 -->