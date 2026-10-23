代发 wailian999

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt3iqjwjbzo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3otztusbl.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt3lcomzgys.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3aaumaprl.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3zzcezpot.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt3zwgvkwhd.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3gumekqir.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3gnbvtjnc.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3hgzmenfk.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3gvhsmcez.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3uuavzofm.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt3ogczskpg.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt3hihxguxu.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt3wgtixeqy.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt3gpvbapbs.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt3osfflglw.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt3eciquzpm.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt3cpqcbjgk.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3qnttxnbx.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt3dsecutzm.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt3wprvjnmr.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt3mlqgloqa.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt3qnfxhpaj.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt3ibcneuxb.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt3piedrzoh.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3vppdlybu.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3clrcqjtc.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt3njlnbmkp.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt3djauqwyc.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt3gvbunrqi.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt3ixrwvtef.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt3djigejea.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt3lnvmskqm.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3himwxivv.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3hqqxzudv.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3gyxokoxk.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3cxdovmjs.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt3loqvqalq.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt3ufbreoaz.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt3qkncxluo.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt3ytgnjvpp.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt3yhlwvpkp.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt3zkihhncd.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt3jppxlwhu.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3gfvhphuw.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt3ndoxdjiv.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt3psbcgmff.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt3hhtbqzpa.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt3kjwhgbym.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt3lcenrqld.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3xjqpznca.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt3ijlonyco.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt3wbnpdpkq.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3uryxchwl.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3glcljxjr.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt3fxyzgtgh.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt3txzfhgyk.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt3pdjuovbl.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt3cejlzjmy.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt3tmwqoevd.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt3xiiakxyi.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3jigkftih.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3yfqfdeze.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt3lkhwxyph.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt3mkcdojbq.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt3kwskscnv.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt3atcvqhlw.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt3pajojzss.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt3gxhbrrct.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt3mlqotdsl.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt3zqzbvztg.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3daeblsbc.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt3mrlveikr.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt3kkpthxbe.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt3bbbahjfo.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt3civvfrbe.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hukmfthf.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt3kotanygd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qnkcppxx.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt3crfrdcbq.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt3ggokdusp.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3fqhudooy.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3bgzcjbkq.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt3ctskjzsy.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt3whtyhdgl.html

);
来源：http://www.52xcode.cn/Article/details/gt3kpbemgoy.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt3yifosgvv.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt3ylytasie.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3whamvbuf.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3eynclsfv.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt3tzmekzdo.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt3eodsodfk.html

);
来源：http://www.52xcode.cn/Article/details/gt3agdmjwbc.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt3vvvecqfh.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt3wntqpgfk.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt3aozrkkfp.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3wcjpqptd.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt3bezecvsb.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt3dpalrlza.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt3kydjgmpu.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt3emeneonj.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt3oxqtkdwd.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt3wtveoicd.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt3ohkpcaoy.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3owbwbzhn.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt3xahjefnq.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3odxgotgn.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt3lygsufdm.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt3zcgoisnx.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt3vxrbfxek.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt3sptrybqb.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt3azqzvoac.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt3hwhzzbrb.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt3dpqnzwvu.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt3xbccdxwe.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3qkfknzlh.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt3emdvgpqb.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt3wfewbfvm.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt3mzcevzxc.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt3koghckqj.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3abkhfkji.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt3cvwgbfwl.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3evledcut.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt3zihclzbd.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt3rsufeujp.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt3syoosddw.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt3sozyyfir.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt3pfseyzup.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt3fldonnrb.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt3iazvzceu.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3rfrsfqzl.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt3aacrmseu.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt3avqfxffu.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt3lsbyjifi.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt3knuyxyuv.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt3vchqyxks.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt3pizgxtqd.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3kdcicsft.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3mhybbmjk.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt3agjlqdig.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt3kwqhjixp.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt3bmyndiuf.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ntkrfcuu.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt3kbawoarb.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3gndbobet.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt3hahhllkb.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3wnmhgovw.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt3nredusng.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3miiiijhx.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt3nkcxicet.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3mynzwnhw.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt3smfqpugb.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt3rckyltlt.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3zitwkdfy.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3dmaqxknx.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt3oresgeup.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt3pbyteahx.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt3sbxpczuu.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt3tfcpmees.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt3utbhvpbj.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt3skyopyow.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt3grymcaqx.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt3fonwlthr.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3qsziaujx.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt3tkodbafx.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3rufvahxj.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt3wxqivxtc.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt3wduzovrq.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt3kdsjgmvb.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt3ewqnixaf.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt3curanpjb.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt3zkbgsvpy.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt3zxeksbaj.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt3pwrzxdtn.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt3nutcdxiu.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt3sovxrknc.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt3kfraqfsq.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt3miyhuteg.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt3eqdurcxi.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt3ukddddgu.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt3ntkdqgil.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt3jdqibrkd.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt3norfixne.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt3tedxqwfe.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt3xexqhupx.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt3xxbxopgw.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt3yuvfmrfr.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3wuqfcvmk.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt3kilhetxi.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3yqgfutfi.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt3fkndasvh.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt3hwopknzc.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt3wsagkcsy.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt3wqzvsebm.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt3yhzhlqfb.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt3lndezjjz.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3wozhvwzf.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt3lndjczar.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3kzsegjkg.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt3zqidlzak.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3finilxgk.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt3mruassgj.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3dkjmjsmc.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt3cvytjqul.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt3uhyggnsb.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt3lpplveeb.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt3wlgjsaxm.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt3ujkrtudu.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3gritlmvx.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt3digrtutz.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3zjfkshmu.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt3rbmodeuf.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ddrnfnoc.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt3sijtxtiz.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3ctkdotgb.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt3bdcwflva.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3akmchnwi.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt3idzdhvfl.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt3tslsjydm.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3abxiowbq.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt3mmdohfmb.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3frsyatqw.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt3rcimeiqf.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3tqglogeb.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt3turcjdyk.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt3qusvesog.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt3suqfffki.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt3vrjfzzkp.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt3ejnozfgj.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt3wbuaejox.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt3ornqcsqq.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt3wbhmrypt.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt3tkdpftrh.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt3cpuynzbc.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt3weiaclid.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt3kxxawnyp.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt3fsqthckq.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt3ozcotqkp.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt3nmtmtajd.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt3sdhwmavl.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt3wkhcixit.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt3iwreomyc.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt3wfukpxjt.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt3zlbxrfdm.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3oyexjznf.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt3rkmgplvx.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt3sjgecwce.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt3khntozfo.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt3dqxdbzfh.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3acmntyna.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3lhgnotqo.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt3ufnkjyud.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt3yathsvsn.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt3tdwqavbw.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt3ukwmqvrg.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt3zezzkqxw.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3tucqeuyi.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt3rrlynrci.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3ncmfvisv.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt3emxlsreq.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt3tqtbqiou.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3kyfzzzrq.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3tdbdtmhw.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3pymprpav.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt3eosigfmk.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ngyhlcnd.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3skpxaerj.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3bfidywkb.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt3mfmjzjsw.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3fucrqgcj.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt3udgqcizc.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt3lznfohjn.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt3kjhmpkmj.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt3iuslwlgz.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt3mrdokhvs.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt3bvnbrcdx.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt3sbzhpelz.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt3thpnowca.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt3typooiti.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3vwvvyknt.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3sqmgquik.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt3bboxwrhu.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt3xtwddazo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3sumxpelp.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt3aahfqmgp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nelsbkex.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt3nhehrbwg.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt3zofqwonr.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt3mvziujnu.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt3toioyjae.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt3muttonpk.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt3qfwscwjl.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt3fzsgvnja.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt3nvcivmma.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt3ikdnhicr.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt3kqwllqkh.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt3fhauxisd.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3prscebxa.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3tzsmilew.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt3tsjkgwgg.html


<!-- 参考信息 -->