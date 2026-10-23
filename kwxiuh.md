代发 wailian999

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt3jewppblg.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt3igtmgyvq.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt3zbbycmwl.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt3vuvctqeo.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt3ekeupopt.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt3xcttbqlk.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt3wdlbgzxj.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt3snzjrnnz.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt3jaikfvyg.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt3vavsmcuh.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt3nbfhingz.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt3ethxxgvf.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt3hwavexss.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3frzzyosm.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3xrcjxmqb.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt3dotyxjln.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt3ebxqvbie.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt3gtkpcrud.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt3nfuszcqz.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt3hjhptzsj.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt3jnhmvlos.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3zfkvngdo.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3cpcunzrf.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3ciolhjpp.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3hnxiwefm.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt3rdjnapbi.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt3eubzbxfe.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt3urivqnte.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt3cixvosqv.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt3tzmnxzsl.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt3vrbpiwsa.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt3tyqudjlm.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3vvuafkvi.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt3eecessds.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3iniymjrv.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt3akxmabai.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt3upnbrkje.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt3dsuvnrxc.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3lebcahnc.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt3xnukwuap.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt3tqbdzkoy.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt3frryzfoc.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ulrufppe.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt3mtfyhlnp.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt3gokrpafi.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt3djgxlgps.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt3cphwkpel.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt3kpqnlzmc.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt3kkgltusm.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3zupgzayz.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3ahoqsevh.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt3wixkoazq.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt3svjyiyhu.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt3hoogrtqh.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt3yixpodyp.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt3gjfxxrpb.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt3pyqtcgnj.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt3pozogcxx.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt3vjxgifyc.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3cmrlzsbz.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt3montrspm.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt3jadxacho.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt3foazthlr.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt3xmwyrbsi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ojwebfhd.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt3thpfgeug.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vyozttmk.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt3pfkhwxap.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt3dzxmchxi.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3wfvupgfu.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3gytwcogv.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt3uakneqak.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt3mnfalpfd.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3cqxtwfxa.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt3cfgcpxlv.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt3toxmphit.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3brmtxrwx.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3hviqiwdo.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt3hxcsslah.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt3eoiwbpxs.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3ucjzqmsx.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt3rrnixdfj.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt3fslcmzoo.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt3mocsycsx.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3ranmtnxo.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt3dedpktkq.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt3eekkbewz.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt3zwawdieh.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt3nohmwhjd.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt3oxjqitbc.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt3xrfiufnb.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt3wiupmknf.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3mpqhrqky.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt3tyboibvb.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3avhbbrqt.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt3dbblwtcw.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3eaifbnmm.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt3wvxkjavz.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3rrwgdvgq.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt3gowgghrx.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt3ionvtket.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt3wqwwdowr.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt3sifeyykx.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt3owuazhlq.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt3nukynlhk.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt3xptubmyp.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt3zntzserk.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt3fohjggix.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3djjsixzv.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt3muyphigv.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt3tcmhfmhs.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt3smdrzaot.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt3tharryrv.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt3zpwejrdr.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt3ktvfexxl.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt3rgqklmsx.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt3uesvscga.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt3apkhyauo.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3kdtpkhuz.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt3wzohcvaq.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3xokedgcv.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt3wohgfbys.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt3hypcrlgb.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt3kzpoyagi.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt3myhjtmzp.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3oerzenzk.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt3tdhhmjqr.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt3uldxoqds.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt3xpgzcvow.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt3owavmeud.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3zgowiylu.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt3udtyofxr.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ormykqrq.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt3rcjdlenf.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3krehsvtg.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt3yrmxmiwh.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3tessiaqy.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt3ogkaluwt.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3dgjwrhnz.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt3ndfctzlh.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt3uhnzsppw.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3xfmwifpa.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3nohcvsbc.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt3mxgzosjf.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt3qgitywgp.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt3esmuxuwd.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt3mgfecshr.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt3znyskgxm.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt3dctgifqn.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3gfymahoy.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt3jorgthox.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3hfihpmer.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt3onbolraa.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3ysrutsie.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt3hssivmyb.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt3ucrorsyo.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt3uvtxocal.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt3xzlxmcrm.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt3kghhdgkt.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt3ygjyxjok.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt3iohpgyyw.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt3yxwyfjwo.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt3fqyafvqn.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt3npbkfjqv.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt3ojcnxzpq.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt3cgjqrmly.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt3rzjkawtc.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt3vqgawruj.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt3ldpoalwa.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt3cscfzlql.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt3fsdyvmme.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt3tpfvrxpg.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt3sqqgvpxa.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt3dcnrkhch.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt3qnhjrger.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3rtyadeft.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt3puocqdvm.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3xwoqqwen.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt3ytkclsfk.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt3ehuhaita.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt3dskpjjmx.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt3eupmmdba.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt3ngkigpdy.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt3ptyqetuq.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3qmyxqzwj.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt3dlbsuyux.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3xqaaqdvr.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt3lqsoloue.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3ttzrfudx.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt3gjuzllie.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3mqrmoxts.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt3mptcvvvj.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3azdofzhm.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt3dltxeafp.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt3fhbbhady.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt3gnpuxsgu.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3qqanohrd.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt3hgsybiaf.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3gqfkukhz.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt3vmxcqykt.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt3eonilorx.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt3yyrxhjou.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3pwzrjyul.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt3tilwknvd.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3vgtpwzdp.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt3kzcgabqp.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt3fwwkfokd.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3oiwxfhuw.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt3nijpznic.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3aqmfyiad.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt3zyvmngmi.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3caxrjwxe.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt3dwoysicm.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt3llhittds.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt3yyjzxthp.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt3qgofrkzn.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt3wzrdimit.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt3txqcwlnd.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt3vyzprzuq.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt3eigsmxxp.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt3iagdulfu.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt3leuhzxvx.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt3cfwktdfv.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3qdanncgp.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3yxrisbnz.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt3xcskfzpe.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt3xyshfsfx.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt3kfvmhflg.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt3zapazbcm.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt3nlggmtbw.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt3zqdkzyos.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt3zjiwdrac.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt3bushrcat.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt3ojzzhaxi.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3swqwfxuj.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt3ccakrpqr.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt3flqygnlh.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3isszjgrk.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3sgonzbpk.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt3iopwsaof.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt3txnzepzy.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt3pegdykrw.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt3jgsoyvnz.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt3knuvmlrw.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt3zzyggomq.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt3doitleig.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3qrekfrxq.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt3azmzllur.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt3dpftswvz.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3hqmwscue.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3ugdkomrt.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3mqdopkax.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt3wbqhiotb.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3bqdgjxah.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3sezoadyk.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3kqicvrzh.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt3aflnvjcx.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3miymovic.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt3tyzjwgog.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt3vgmdmrmg.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt3fdfeftsf.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt3litfzprz.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt3wvytznul.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt3yhxsgkwl.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt3sqencmqp.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt3icuwqilw.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ifkgkijn.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3npcfnuey.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3kawpjkmu.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt3dzpwlboi.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt3psvaeanz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wmiodnlo.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt3hiqtsirs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3chklqmzq.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt3aizhybdu.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt3dxnvgwwu.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt3svmqjqwp.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt3srhjvmgz.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt3udchcsyr.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt3tspobinp.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt3yyxuwytc.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt3augrfekc.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt3hykdjqop.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt3ncfqroiv.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt3bysoudfg.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt3sounetht.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3dvzheugc.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt3ambbbuel.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3syzyzqmn.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt3eynqotdr.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3pdsduupf.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3oxpnzyxr.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt3mhutfmeb.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt3xdvwiqpw.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3wjegmvhk.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt3jvayrbze.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt3hkskhyea.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt3jxqusari.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt3mwpgzvqi.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt3wmlprzdo.html


<!-- 参考信息 -->