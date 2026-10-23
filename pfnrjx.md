代发 wailian999

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt3ooeztcge.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt3nusvujho.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt3avgtrlqi.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt3gaafscyq.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt3nlckxkup.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt3zimdfjhd.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt3yokwfdww.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt3pjgbcmal.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt3axuhzfer.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3sotwhcdf.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3oihlqpiv.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt3tbtccxux.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt3uvhspwdo.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt3prglfskz.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt3jpuznwvk.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt3oastanbv.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt3nkvfsytw.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3xcqrcmgw.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3xaisvjzd.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3ncamkpdy.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt3fltowfef.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt3ukdueajc.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt3vhlanubc.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3uvsmaebj.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt3ajltbpiy.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt3wgxeflca.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt3jzchjbil.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt3wjnyswac.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3ohynpism.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt3bntpoxzy.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt3yyfioico.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt3ijdzzadm.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt3dlplvfvn.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt3hemwttwp.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3mcgrodhg.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt3jraeunpy.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt3radbxpiq.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt3nzewnsok.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3aqfmfonn.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt3unlltutk.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt3tkwsgoos.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt3anomuyio.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt3xsgphuqg.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt3atmgrdgi.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt3jsishowg.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3tdhkcjbx.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3xwaglibq.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt3aovbtrik.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt3mftqfycf.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt3lhwxvyls.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt3egynlpkt.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt3simrxmod.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt3dkmwrzmd.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt3tsuovacj.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt3imswdhia.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3evslxenm.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt3nqkaaclc.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt3crreosuv.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt3wkvlupiz.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt3jogwmcir.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kwyzzvyx.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt3jyhmzeov.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3onpsiaau.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt3rdmxcnlc.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt3maulefik.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3xmweujfl.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3ulexjcab.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt3wkifjsti.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt3sgkzxolt.html

);
来源：http://www.52xcode.cn/Article/details/gt3lmrpdlyx.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt3uuoswqtg.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt3ukyrjmap.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3kaqmvlpq.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3mosstxum.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt3pdrkahpc.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt3qjnvdqzk.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3umrnszmb.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt3mkhpsprr.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt3atfktiuj.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt3paxnqsbd.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt3tkefddsf.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt3capkdzcf.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt3wehbkvgv.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt3shiblujj.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt3kqcqxant.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt3jwmntxcx.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt3dtutoujq.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt3whftzkbx.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3nftluutg.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt3cuxpibez.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3gsnnachw.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt3xzgtujff.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3xrjrtrdh.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt3fzhulhfp.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3lgpjcwir.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt3unacvhxo.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt3zrogskcc.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt3enlmcxkw.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt3keqjekks.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt3hzwdxlty.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt3upriznvi.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt3nvcdasxm.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt3omkrhepy.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt3jlyjolmv.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt3jivurijh.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt3qtmdxdqq.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3hflumyya.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt3exojcnqo.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3jgqqozhu.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt3lulcpopi.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt3ewjpeifb.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt3elngyoyd.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt3nyvipsbe.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt3eralylrl.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt3zgtmtids.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt3axmmxtby.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt3nndwevil.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt3nksnynvw.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt3vnseneih.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt3qzutoxzm.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt3vwpvawje.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3wiaesvbd.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ldmfowrr.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt3himvahda.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt3ykgoryja.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt3lynayani.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3myvinqgp.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt3uitruwdd.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3clytwejr.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt3hzhjrzmc.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3ubedydtn.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3mhnhtgqq.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3fcqcjvfm.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt3bhfzyjfi.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3fnmqaapr.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt3lcrjhoub.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt3arjwuurt.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3gasqvaxt.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3uwudsafr.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt3qfiojcts.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt3bbcbfvmd.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt3tlzwbblb.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt3flxlidvn.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt3mroezhxw.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt3efajetbm.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt3ehejbugm.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt3wglaktto.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3bqzcpytm.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt3jzwdnbdr.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3xvnqrpgi.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt3ruhovnpx.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt3bzwumkmq.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt3jbjavfub.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt3tulqbzfs.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt3ssvzzpne.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt3curgcigy.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt3qeovfnbi.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt3zqhjfyjf.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt3qhzpgdye.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt3ywxnycof.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt3dywzgdhk.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt3qznnfjtp.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt3oxkntwvw.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt3vwpcbuel.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt3qmozlwaq.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt3ujfqnniy.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt3ufinvdks.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt3bgfyckxp.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt3qhbbwoyl.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt3idoyiivy.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt3rhxkmtro.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3mwrvjjfg.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt3uudxgpiu.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3nwjjyxha.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt3dfnncrhi.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt3pqxcihab.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt3vbbslook.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt3pprccdgz.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt3pmdsqrft.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt3abthedus.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3rvkjsncm.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt3swgdqxey.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3onkwduzk.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt3jxuvjzep.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3btalxejl.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt3hvylzawt.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3dixfmhmf.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt3thxwbrpe.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt3aqplxfrl.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt3edrmmtvw.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt3efkmhqrg.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt3uzqlgaiu.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3oncundts.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt3bqsmvwae.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3kzrelsom.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt3tjsooukz.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3yuvoztqv.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt3eccsiyor.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3zrelgsth.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt3gagbbihp.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3gngfvsfo.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt3fnubpcyx.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt3oizzkmup.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3bwoijvgc.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt3jexdnrrr.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3ahllvcha.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt3allzhzox.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3hsqoiyfl.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt3ousrejdw.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt3olclpfcy.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt3zrtbnedc.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt3audobhty.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt3zmtfkcjk.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt3vohxtffy.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt3lyizwvrv.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt3sdjbideq.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt3taqleevc.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt3ixtircrx.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt3sjabqhfd.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt3sospyafy.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3yrhwqais.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt3ezudxhsw.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt3fvxefwke.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt3qomapsce.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt3oclhdjnc.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt3tgkqaivp.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt3bdttokqg.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt3qsoxbxqs.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3bdtiutav.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt3xyxakshq.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3uuzipykg.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt3axeuynvg.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt3pnbeoerb.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3bqfmijzb.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3qaiqspnd.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt3juzyiczp.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt3ulhenuea.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt3uavswbtm.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt3tgichlvz.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt3hmhnfprl.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3ngnvkyqz.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt3woyjqjmx.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3jhbeyfme.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt3hmwmbriq.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt3bcodahze.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3zzxouofv.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3gojnphuv.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt3hcgkqofa.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt3euytuzmv.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3pdznyreu.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3jwfjayun.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3tcsciygd.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt3uxpxfbpe.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3gtmgycha.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt3ebchudve.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt3ggcmhdod.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt3xxnlqpan.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt3ailjpxcp.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt3huhbhhef.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt3rcncbjti.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt3tialnpdp.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt3lnpnoxqw.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3qhlqvnab.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3spkkuaao.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt3voecsdcd.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt3fbopqllf.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt3mgyepgab.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3tzecfife.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt3pyxlswmp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xnlzetet.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt3qmnyrjqf.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt3xhwzifss.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt3ktyxkeed.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt3sgsjrfxk.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt3xikdpsmg.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt3kuvmvyrs.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt3onjpmgwb.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt3orlmlsma.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt3lbggnwqa.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt3pbirsmsy.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt3chfjpwxj.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt3glpuyrik.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3odxgpxrv.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt3vwvzxnxv.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt3ocalnhwq.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt3livgllxu.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3fxqwcooq.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3cwfvpizv.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt3orvcaios.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt3yufzbjqi.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3fubglqoy.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt3qvjkvjkf.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt3lvwsnjbm.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt3tmarjerb.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt3zvwwzdsu.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt3anhruwpv.html

esac
来源：http://www.52xcode.cn/Article/details/gt3fsnglihu.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt3mosrcvlv.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt3shcpeczw.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3lnsxroop.html


<!-- 参考信息 -->