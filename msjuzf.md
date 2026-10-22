代发 wailian999

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2ydxivqjj.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt2fpztvyom.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt2mdafrilh.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt2vgpokxjy.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt2djerooea.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt2nrjwxiuh.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt2eizbxudh.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt2xqnxtbvb.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt2qtdfjhmh.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt2pxeflvge.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt2bdzxuoct.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt2rjbfqgtk.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt2yolpefaq.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2hguzxfkn.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2hpplrrpl.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt2pijrspzy.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt2igpnmwts.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt2afhsmpmg.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt2jehrinpr.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt2gkfdgexn.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt2bxikgjen.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2eympxjqx.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2igfkzdvz.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2wmkixsjb.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt2vuwythvp.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt2ggyxzeza.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt2lnknkgys.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2nzabuhqv.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt2nkgprolp.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt2hjnijlsn.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt2ocvtieqo.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt2xssfczof.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2cuzxukye.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt2lyvtupid.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt2dlfnqgkl.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt2vtzkbhqo.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt2arnhlzjy.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt2wnwwysmt.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2tallemal.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ajlebhto.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt2nhlvstxw.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt2medmammh.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2rzwfdbmz.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt2qgzzfejj.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt2yzjrmlrf.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2fxfypafz.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt2jpnautdu.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt2gxqzteol.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt2oyydmxqx.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2tzgcgscv.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2uumpjppv.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt2qtyudgzr.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt2pexwghqn.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt2xcmwmjkb.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt2utgawtke.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt2gzxxcphb.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt2uwrdsfwh.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt2orzejxco.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt2ulwjqzor.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2ybkvbcjw.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt2wnjyrlwu.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt2rrmfmqcu.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt2ozoyptxd.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt2zaadlxoq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mmfzasoz.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt2ejgcpzdw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mctvuesz.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt2lauhrhfi.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt2sbsbbubm.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2khlrmrgc.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2xfkaptjm.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt2qbrdgrbu.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt2uxcclxse.html

);
来源：http://www.52xcode.cn/Article/details/gt2wmzdfcxo.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt2llsrvpcb.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt2khyxwtyr.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2kfkpopva.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2bvqqdmqa.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt2edheaasj.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt2osyftdkh.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2iwicbvra.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt2mdkonrax.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt2qqpmdtxk.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt2mcrlrfor.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2uhilxxvw.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt2rsiizyon.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt2ewntpivg.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt2yadbwqmm.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt2kwfyrwvd.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt2vnyxtxce.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt2ylmzmhji.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt2ekolshbq.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2rgxozqea.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt2acsdpktf.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2mmwogwsb.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt2sumtodae.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2utpisxck.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt2gmnobzje.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt2nojyjopw.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt2jjjrablo.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt2tprudety.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt2mktqizuh.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt2mscnpsuk.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt2adjguwla.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt2ngqvpksw.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt2wujvlgyz.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt2rdmqrpyt.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt2rjqvzrtp.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt2uxtmymhn.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt2cznzpunp.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ozlzbaij.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt2jbokewrc.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt2dbvdjwlv.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt2frzzlwqu.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt2lprqbtqj.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt2xiwptnmr.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt2bxmaemlg.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt2dbnmikci.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2yhcjkdfr.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt2xvuavkob.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2mggvuifz.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt2kxddgxdq.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt2vlsjsksx.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt2bnympztt.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt2wruavxhv.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt2abtwousc.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt2hmfazzwf.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt2otvntncu.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt2lwqxeoix.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt2rwsqmyam.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2xhxtazqf.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt2gnbhykaj.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt2abuwxkuf.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt2dpjqqwiv.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2mvigkaee.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt2xwwebnif.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2vbegqhdl.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt2jaywvxhn.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2asfeywxk.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt2xnemohbs.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt2bxmfphus.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2bpmqpife.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2neaomhck.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt2uaxavmxe.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt2hvliowbp.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt2fiuyflkc.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt2cupajyoo.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt2jyfqkqhu.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt2zyvkuejz.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2otipkbsy.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt2hfwurrrk.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2nanqvrcp.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt2dzluiyqq.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2dvlapwgu.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt2rvmobojv.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt2jyroxjgo.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt2nlubrmcx.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt2geddgqcf.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt2oupiiphv.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt2hupbtncc.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt2nqssghaz.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt2lhzyuqdd.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt2imitguda.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt2hjstkpjf.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt2dprnqnsi.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt2gihjyrow.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt2psizxsvd.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt2uyyyfhih.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt2mdjkayac.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt2zshqoybv.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt2izydvmmp.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt2wgnmnoac.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt2riaribvc.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt2wvztjozv.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt2pwmzxndd.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2xcuwgrwv.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt2xhreehjt.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2bsujnsff.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt2rdzdlmmu.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt2nidobgay.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt2cguxsvay.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt2jkkctmlb.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt2momsaceh.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt2pwfmpcit.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2wezdfwgy.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt2xbllboug.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2othdaosh.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt2bzfqxlcr.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt2gdyubluk.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt2mulnhpso.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2emogimvr.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt2xzvoolvs.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2rzpvluag.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt2wljjkzsm.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt2lnhfadsn.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt2hdpmdoyj.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2ynwrzwdm.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt2sqohkbxc.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2pkiusiih.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt2hhflnrdr.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2poaaehyf.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt2opexkkok.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2awspdnhw.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt2kapdszsp.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2cabxhrac.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt2udxjbcdf.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt2ytmrqqyz.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2fnxlunpr.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt2nnnoudri.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2vgobjvpj.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt2girtpcnr.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2djgtyepn.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt2rirodzan.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt2bravhbde.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt2smdcxntw.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt2iyxcqtph.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt2kfvqufmv.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt2tfpenwic.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt2cxtsqksv.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt2wyowixbx.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt2ooqrpkdc.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt2iegwuffl.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt2lhwaqqtf.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2yzvhffrp.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2yjynnjpp.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt2wqmdyqiw.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt2brtcpnlp.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt2ulnswwbv.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt2cwetuian.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt2yodiqnby.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt2oexndkjk.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt2vmzthayr.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2tthdrmsu.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt2whrkhhmj.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt2rjcivzdh.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt2tzykjejh.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt2vggmtfwo.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2gedvlwhe.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2sfteubtk.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt2wberrndj.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt2agjgfuah.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt2jiczupix.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt2ryodsorg.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt2qhfiltuk.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2ueuzcywi.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt2vjlkvken.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2nldwludj.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt2fibmevzq.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt2sygfunlz.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2afjmmcac.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2jlcteuyy.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt2mwgqwpty.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt2wlsynyhq.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2jcnxvvom.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2xphvhcdy.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2kityvkmg.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt2icajflcr.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2cwwaghcz.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt2ersyrrxo.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt2bitzflov.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt2fpiuxlrw.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt2kuoazlcv.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt2qskrncyc.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt2yfgnijlv.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt2lhsqcnlx.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt2xmnkvavb.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt2mejzhfqn.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2cytkppkr.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt2qeqepsae.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt2rgidyccy.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt2hqsuozzb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ahntakpw.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt2wmvjivyj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tiyfawgy.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt2cxwncmer.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt2pufdxvvv.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt2kzufwitu.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt2bcetpnlj.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt2gjrjekpe.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2fjaefehg.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt2kmrwgnoo.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt2zalunrlb.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt2cnuzihcg.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt2qtomekkj.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt2pvsfihup.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2tbpbogto.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2vwvnlyji.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt2bpxzxgbk.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt2qngozcpj.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt2bsocslwa.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt2lrrdwzbo.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2eblsvdwk.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2dqoekyvc.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt2xqmbucig.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2bvutsgeu.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt2dqvyvmym.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt2oilevljy.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt2adxzgytj.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt2sklpglcz.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2sqbykrqd.html


<!-- 参考信息 -->