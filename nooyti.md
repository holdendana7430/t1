代发 wailian999

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3rctznwlj.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt3fupnadem.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt3thrumduc.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt3grlruuhs.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt3kcozcilm.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt3hazomsoh.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3cqcdfmrc.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt3nnniqooj.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt3wsnyssmt.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt3wiqaqpww.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt3lxnnzebx.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt3yfaanjny.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt3lmhhpjux.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3xtblphcw.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3svkmyfjq.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt3ctfbzdqa.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt3iesrudfk.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt3vsivenfr.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt3mgwdmmdr.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt3rhbjvwep.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt3tnhunejr.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3ureojuiq.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3kjpfknqt.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3bpdxkghn.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3svtvpjut.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt3effamxeo.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt3ojtlbamq.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3gghefsah.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt3dspcfdpm.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt3ausauvun.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt3qyehenxi.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt3sdmfptgb.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3rekyesko.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt3kxwuysif.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3bfsdekim.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt3szweyfbx.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt3pddcevcc.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt3bjwalwia.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3yhajkupc.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt3kbpogaqh.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt3koxvpglr.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt3qmltpkde.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3ddjscvqz.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt3kydkpzps.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt3vpapqgmj.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3svmtifnd.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt3uhknxlux.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt3nqkyffhj.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt3repupltk.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3exqddkyk.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3totpqnzh.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt3cwkalbtl.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt3kkwpfnou.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt3bmjqlubn.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt3vdtggqxy.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt3iirozbsy.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt3cmhxeckb.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt3uaztmajq.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt3tdshtydu.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3kkmecuxe.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt3mgeejtvq.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt3bhsqyrnv.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt3hohvacsv.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt3wqoeoked.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3uvveogxn.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt3rmuoarbi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vfjvjeav.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt3bvkvhdbf.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt3vbrwxxte.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3ifqxmajj.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3vttmduem.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt3eywzvrfk.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt3tirxtwyq.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3cvjtgejx.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt3blmfwvll.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt3yxdytsef.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3zbwpjbqx.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3azhgpavm.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt3cfbtkkxs.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt3zzemjwcg.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3bnpmcyjx.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt3vfpumkjn.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt3zhqgckpn.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt3zqdwazue.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt3exoucukx.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt3rducodhb.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt3chwbjtny.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt3aqclioqq.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt3rsybiqdt.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt3dklcnico.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt3ilgzedhm.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt3bacpmzir.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3ehqzsxwm.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt3raxwuplp.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3okmxoywn.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt3jjdctrdb.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt3tntxyhrf.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt3bakxcecw.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt3myxotvzx.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt3tuktlpqz.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt3xfrfnzix.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt3rytfuhea.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt3vudosmus.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3mjjqxsov.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt3ofegaqha.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt3tzgquvml.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt3fjfsphdi.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt3ffhvtsfx.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt3tabyrynz.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt3vwrsjgzo.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3utkbtipj.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt3gkmucilq.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt3gioxhkot.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt3ehiqjwpb.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt3hpkmuahm.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt3qhtzomlx.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt3kvxasyzs.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt3gwkefchm.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt3htwpzear.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt3cuufdywg.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt3ugxldajr.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt3qablktmz.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt3qkzzxjoj.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt3lcxylcvq.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt3ybwjfloe.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt3sxftkzyo.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt3sreporuf.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt3krfhhkpz.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt3ryamizaf.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt3hfrsgzto.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3jgtsansi.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt3ubacrrec.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3lhpujppr.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt3ohxftvhv.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3oogihdoj.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt3uqdktudh.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3zcmoiohb.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt3pcqjspkx.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3qiriqynj.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt3ohussgtf.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt3nprvypwt.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3twvbropt.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3vqgjyjmu.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt3xzacsbeb.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt3kwxfqgqi.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt3zpstinzr.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt3xmukdcwc.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt3atqosivu.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt3gklxeoxi.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3auuaaikg.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt3xbkfuafx.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3vbahebmn.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt3pmfattqk.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3kaoekrji.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt3ybaisocz.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt3vjqiefis.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt3mvlydzae.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt3lsmtornd.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt3utsykblc.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt3plyoecej.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt3driumjyy.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt3swhdkorh.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt3bbnnrlvg.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt3qsjxysor.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt3uthryubg.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt3mnbghnaz.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt3hjblmhty.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt3yzzvcnzf.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt3knlvgbzi.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt3bmcvzwve.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt3ooyrsvls.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt3efvtmxjd.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt3dcracphw.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt3ddhejcly.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt3ftcitpuu.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3tdhxdvds.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt3dxzrfedx.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3hgkbebxd.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt3sqsoijml.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt3fagrsrpg.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt3cjphgjuy.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt3wnbivvgh.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt3gujhtsbl.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt3qhwesxnj.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3lfaocxjd.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt3dmzmizxz.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3zwitdqbh.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt3gjpeiglc.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt3bbsiclzs.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt3kzchqlmd.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3pdleipob.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt3zxryawch.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3ygdgbspc.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt3cqtcuchn.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt3faphqwat.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt3banjbxkf.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3znfgqmzt.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt3pxnoblxv.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3ghkkejhq.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt3usmiilgq.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3lkanwfuq.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt3bnuiwvnq.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3ljadwynm.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt3yauprngq.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3tupduxgp.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt3fvatjjxt.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt3aduonold.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3rgyfovne.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt3gdunazwx.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3zxnaxhcv.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt3hsizprhx.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3mlavovus.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt3ovdqokwq.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt3mmkjygxv.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt3flpimnod.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt3hpglkich.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt3rbtxaxqt.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt3fzrqtmhu.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt3ciszpibd.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt3ombxyrud.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt3mijnijxp.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt3liayshwh.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt3akkxunku.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt3jclfmtea.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3iydpvigy.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt3wgqzxfkz.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt3zstsvosk.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt3cuhmpcld.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt3utgeqrsv.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt3vbpaxots.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt3aqqeltxp.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt3sjonoaol.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3mxepjfbt.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt3qhtbvzxt.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3jqqrxqra.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt3euxgazji.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt3elwqhnli.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3bbmirhmk.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3vlmngieh.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt3fyluhyxg.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt3tplwrywe.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt3njhisolr.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt3lqgatcxl.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt3nvkvyoms.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3dnrnhmdt.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt3yckjrxlo.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3qnztcdtn.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt3soexlntd.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt3gcmtkeqn.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3izbbhwnx.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3cndfbhzq.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt3oamjhjop.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt3mvvacdef.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3dqujzfpe.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3rpvyoubs.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3mxcslkps.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt3dxwmmyiy.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3rkdxvbit.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt3lwyaqzeb.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt3cqvkmtvr.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt3mesivrux.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt3ghhkmvay.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt3hrcrptow.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt3mwiftxwb.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt3jpiwovsk.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt3krpxaxul.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt3dvxxsnej.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3wlmrlvmx.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3jrudbayq.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt3tdcjlzcz.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt3qltpsjcd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wxxkqiiz.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt3nbbhdsld.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3aslqcwef.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt3silbsxci.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt3vhnipmbu.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt3cpmkzccp.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt3vgbjovmy.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt3dhnpbdlf.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt3xmenuasc.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt3qzqhzwin.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt3vknpyoyk.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt3asrvropc.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt3caxjzmve.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt3thadctrx.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt3mquqvean.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3lmnzqfeb.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt3wjlnyfbl.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt3clvjtqyi.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt3mfqwgean.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3nsfqyhxl.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3vovoqley.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3ceoetltk.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt3trtmwxkc.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3lqxmimfu.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt3fwxzlvzb.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt3mdrjknrr.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3psrpgvoc.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3jjagannr.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt3wiivyfoa.html


<!-- 参考信息 -->