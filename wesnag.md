代发 wailian999

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt2svwkzani.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt2hkrrqkjo.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt2lodlczeq.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt2ujpaqktr.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt2tztfqygb.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2qskfbazt.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2capcgmaa.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2nfgqpqoh.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2hkhdkouu.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt2karlcmvq.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt2jjybgsnu.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2soidpmus.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt2youfbtca.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt2tshvurfk.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt2mxdialxt.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt2kvmwcsmp.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2gqoorimr.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt2thuukfxq.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2exeziwdy.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt2njtjzqai.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt2yulknqdm.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt2qujwpkai.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2jqrjmdjy.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt2gqqzrqho.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt2klvjowjg.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2pcyiujlg.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2mfftrqrl.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt2pibjqrlo.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt2klgtuzxi.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2meztkwky.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt2tlvrlebf.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt2zsrisqcl.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt2zlzmtzhs.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2veecukxx.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2mimrzndb.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt2pizvlgww.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt2vgaeykox.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt2unlpvpki.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt2jikvzglc.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt2bwdzzrbi.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt2xuydykog.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt2xardvgwi.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt2rymobvgj.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2uzfpnrhh.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt2dftzsscb.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt2hidsshbu.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt2jsddsssc.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt2tnpqisrr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ucenwpbf.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt2acjgoxog.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ejsnuxpk.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt2xircvqce.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt2yoqhggbp.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2ccgrjyoy.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2udtiyvdv.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt2cxbfxcrj.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt2tpfprztd.html

);
来源：http://www.52xcode.cn/Article/details/gt2axbgefmz.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt2tjzsmqeh.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt2yijvidpe.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2npqgynzl.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2ggsafonr.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt2lqznparz.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt2waeeirfx.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2wyjwknhp.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt2nlhdncri.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt2hlsjhaed.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt2rcxceaub.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2hootpitt.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt2gvivcvtv.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt2jdxsqvlf.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt2cbnftdam.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt2tjlblvow.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt2cbaxagdi.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt2qvexenog.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt2jfblvcfn.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2jmbtrtag.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt2nlbfgorv.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2ypzlvlbi.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt2whdjqsle.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2awbskuim.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt2qdwvrcdu.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt2kktmjmmm.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt2aoqafqax.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt2ofdeuxqa.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt2pmmlqtuu.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt2mrmlnvky.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt2qhdnfkxi.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt2rcyxqchr.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt2enuqmimo.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt2blmkhcgf.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt2vanpvjrp.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt2jyvixoka.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt2tcwbeusc.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt2oekqmpzx.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt2mftboojq.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2llahpkgl.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt2jhickckq.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt2rcabtztk.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt2hyarfnfb.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt2dnbfinhz.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt2qhpvlioy.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt2lknfjwjx.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt2rkwldtne.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt2biqyjckn.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt2kkiohvbx.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt2wofiacvo.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt2hbfghrxc.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt2aixciygt.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt2qmgfvgwe.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2xkujfqsz.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt2fdqvvqqn.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt2fisfljdf.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt2hixnffvi.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2liqdcibg.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt2aklksiam.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2shdzhcqf.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt2oamytjsk.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2aeqdczjb.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2akgfyujt.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2knyqswbh.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt2xlvfnovz.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2vlmbrimi.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt2lrmzxzol.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt2dkideyir.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2hgtkpext.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2lzynkniy.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt2xivurddo.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt2mlodabqa.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt2iavtlesi.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt2dzgmngct.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt2wdudslvo.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt2yvrycovb.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2txcrrqoe.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt2katlxmum.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2oifipfgc.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt2zahrwazw.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2cpszuwzx.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt2uepxcykl.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt2nljirhom.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt2kbqjmzer.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt2sglxjfjy.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt2okkexstj.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt2bhvlswxb.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt2fbwxnwug.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt2ddxyggfq.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt2ueiwflje.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt2tjpvafix.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt2kiidehaw.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt2djgjnpeo.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt2pbsdbhaw.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt2igcvwtqh.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt2zdmxydxo.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt2wkjrfflc.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt2pucgxaht.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt2hxxviauc.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt2ilnuslkm.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt2fbktwmyo.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt2phsdnnan.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2hbqyihgh.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt2stjyfofi.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2mrffxqay.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt2gslirjkh.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt2hnhjkvcb.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt2cbwdzlyj.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt2alkooqls.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt2zwskbgpc.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt2lpfkgicd.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2kspgoxgu.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt2lrumfwfe.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt2frxblwzb.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt2ebkflovk.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt2zmuyabig.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt2hqbpbjmr.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2utouizfm.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt2uhjfjxem.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt2ojbqsdcx.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt2zsajswdv.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt2pqgienlc.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt2hqwzsjjw.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2xfwnsleu.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt2leycvxzg.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2kyurjack.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt2wypkdgxl.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt2hcjqtedp.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt2wumwqdbq.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2klsdjxhu.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt2wegvaemw.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2hifhbnra.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt2qhgayalj.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt2egtoqcfb.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2rugngwcd.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt2wrvwqnzu.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2ykalixwr.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt2lgboxslu.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2wjbhyegf.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt2nijfbtip.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt2hjbaazjj.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt2mlamktlu.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt2jvqdzgcq.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt2almipxmh.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt2mivvhjrj.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt2hcmqcfzo.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt2ivkiadzz.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt2jjwbdtyp.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt2ubbwfqws.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt2ynkgebqi.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2okycaoac.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2pmoogkdn.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt2hdjhjczl.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt2nafuioif.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt2rllefbcl.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt2cqikwwmz.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt2ccathqcy.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt2sqauhzoo.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt2qyhdgclf.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt2nernnzct.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt2aehnktwt.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2kizsylty.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt2xaivwpyn.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt2msjrxgbb.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2yqqquorc.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2zefouwrr.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt2iksxyptd.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt2yphjaxlh.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt2newyghvm.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt2ffnmwryi.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt2gvgwttev.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt2tltjsfpg.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt2abeyfxcp.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2ywfoasad.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt2lvhkyxnp.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt2yfkujymm.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2iqmkjncb.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2lijtnjjf.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt2sklhelbi.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt2uwszercq.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2fbmyxxlz.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2znaqplnx.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2hxnajatu.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt2wqteuyuk.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2zdhdkyoq.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt2kjbqatew.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt2lyigdlan.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt2pwikoyah.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt2bkeiahhq.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt2kfcehihf.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt2tnddgwgo.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt2ilospgsj.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt2fqtwbihv.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2fdbyllzo.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2ackequiy.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2xrbbstle.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt2jwvtcdzc.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt2hnhlbigw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dlqsqzmh.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt2cypewyqo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2crqqycix.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt2kuhbdafl.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt2dgdmrxft.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt2uiobikpj.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt2vqsbgupf.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt2kgwwmogi.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt2wfffqyuk.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt2idnywxtk.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt2dvyfkaph.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt2bjqjnaxq.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt2wowyhirl.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt2xzcstrws.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt2irwrdyvw.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2pvnfkdoq.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt2tvpvgqsv.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt2xwjhhvhp.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt2fiodyvwl.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2kxatbwvn.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2navcqjsq.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2abludsef.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt2nagreonx.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2ifmokxnk.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt2cmlptaha.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt2iywzpezz.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2pzbzqyjr.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2iqmbzbve.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt2gowarqpm.html

esac
来源：http://www.52xcode.cn/Article/details/gt2vqelkvzk.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt2ckcjgvdr.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2ppilbufc.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2wldxsfgd.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2ofjwkmfe.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt2lymnvxbr.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2thummbeg.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2rjqmdfxa.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2mftrifkm.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt2dennaoev.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2vytkrefc.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt2yyvqvihe.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt2yiydoyiv.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt2vogiuwbz.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2eqzirauh.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2ygmxgyrf.html


<!-- 参考信息 -->