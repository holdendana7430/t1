代发 wailian999

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3jywnkgne.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt3twhjrerg.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt3dgcvhjrz.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3xpycamxm.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3xnmitybz.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3lizcrgpn.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3xfgekgkp.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt3tijsyvzo.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt3ujoaartw.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt3ezuyeyrn.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt3yxqqgqoj.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt3huydszzx.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt3jqwcmyyl.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt3wotgygdz.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3czgtrvsn.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt3wgebyawd.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt3qpdmzzaq.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt3lrmidlps.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt3zmvptgfu.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt3sulxcuos.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt3dmlxiljx.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3redmdsaf.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3uvxwdcor.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt3dihyqoeg.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt3rrkvyofy.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt3fvfzdwnn.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt3lgpcptka.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt3xetnbash.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt3haqiszjx.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3xpyrzocd.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3rjgtjacx.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3gqmnzsnw.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt3sjhqhxjk.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt3wepesrdv.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt3yyjermhu.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt3bbyggqdy.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt3afazpgiw.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt3onfghlhv.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt3grjhvvrt.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt3vadodhgd.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3xkvwjpue.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt3ajqtrgnb.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3lthtsdau.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt3pxgzhswm.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt3qqieonab.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt3xmggidez.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt3hutvzhyd.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt3jqnghhpr.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt3fbtlweqr.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3pyqfokov.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3zeybwqle.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt3pjxyhzbl.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt3fjdkctdl.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3pyebnjbp.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt3axyimski.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt3tvijmhzi.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt3qpokuvrh.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3ylyxwjnf.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3bzulatmz.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt3inkyhoyz.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt3ynxmwoka.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt3tzebtwfo.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt3hrgrsfgz.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt3misdtnmq.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt3wtkmgrex.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt3shaqolef.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt3yfzceude.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3eepiqncv.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt3vcamppen.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt3bkccidcn.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt3kuxqbpzc.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt3ugzahedj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3aseorvpc.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt3gajestqv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qocvyyzi.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt3zfzbgccw.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt3qbnmmfht.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3immmacao.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3euexuhlx.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt3uzlkgcax.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt3ykrwrodp.html

);
来源：http://www.52xcode.cn/Article/details/gt3htusqqsf.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt3egqzeogq.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt3nhtorcuf.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3vmojeeow.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3lmqhosql.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt3fwsyovys.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt3roiuvahe.html

);
来源：http://www.52xcode.cn/Article/details/gt3hvsnyamb.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt3wmfqhupy.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt3spzyknbn.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt3slfwgnzt.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt3hepfyboc.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt3czxmjgmh.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt3sjbfjhgz.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt3hegunxvp.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt3adncubdq.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt3ytzqmgls.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt3csavelow.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt3xolddttv.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3ylrkohte.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt3qmctwino.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3ugjgqcxj.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt3phtdhngs.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3zwbdnnqm.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt3rnwhudak.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt3ukvlyjkx.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt3vololaov.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt3cgjusaxj.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt3ldbaised.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt3pmygmvzh.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt3tlmaodac.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt3cgtnrscn.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt3aagvmcno.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt3xvdxohsg.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt3mowytuvz.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt3fwjzwjhl.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt3crkmzgck.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3uggqivvm.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt3yayuzrjo.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3celwbifw.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt3tjocujyt.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt3asbcpcrm.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt3uoglrdka.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt3jhodcthv.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt3jexaopwm.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3qubesblm.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt3ymlwouzb.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3wqbalmnu.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt3taqejqeh.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt3svyytemb.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt3cmvnajnk.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt3chqvxfhy.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt3rlgpyvvk.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3nvumfbll.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt3mklghqtv.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt3mkatotxz.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt3htxrpdoa.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3htbrjuwq.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt3zyzkxcjb.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt3fkzccfoh.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt3pitjlwnf.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3kyabxeey.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3nzuujjpo.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3jcscxaeq.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt3weqpxgvn.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3pbtmxkth.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt3aidrfoav.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt3zvfhtfwg.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3glbeilha.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3whgcpbml.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt3cijshguq.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt3vyhkavxs.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt3cdvvdgde.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt3oyqpthid.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt3eaoigmlx.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt3ncegvpil.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt3qcmulluc.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt3irqofzgb.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3itttbktw.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt3hnqsiuwc.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3efbjlzda.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt3ehefkbvi.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt3znlkbfbk.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt3upnfaejb.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt3mgcnabcj.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt3iexwdsuk.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt3lxisvjsf.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt3zznxpfpn.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt3inpppceu.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt3ejeomndj.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt3sfjmbrzo.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt3vhosrqpm.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt3bimqphwu.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt3wrwwgwhy.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt3tpjfrhck.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt3znjanrkl.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt3qgcweleo.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt3knbsarkt.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt3vzacaisd.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt3osfoxjkm.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt3qspafoyq.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt3vmeexhtu.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3ydagvkou.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt3pcrmsjee.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3lgsxmkws.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt3hlhwckun.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt3qeukkkoz.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt3uxoharfs.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt3xdjkmsmu.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt3ahqnqdee.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt3plbxqxhv.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3jxnzhhwv.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt3hekrdtdz.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt3rbqnukck.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt3dvjemqkh.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt3pxswniuv.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt3axozjzld.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3bhahqzhm.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt3kxhevxmo.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3fpuuprtt.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt3zttgtqew.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt3kwlzwjzo.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt3qoadejcc.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3ekicqmgr.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt3gbwmfxrc.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3pvtlrigq.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt3tmcnpbkc.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3cylntndx.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt3rfasiaak.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3bhhgfifd.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt3rmitkdbu.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3tbmgrsmn.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt3axtmpldl.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt3liwfhmzh.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3mhvyopae.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt3uajafnsp.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3nwolmqwz.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt3vyjdqnlf.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3jmuqhcjz.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt3hmbddxik.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt3lelrtmip.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt3jutlvntw.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt3ostlgubf.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt3cftoutgd.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt3gvqbrygn.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt3phfbcniq.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt3kwmaudgc.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt3oekbaiib.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt3mxoavfbk.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt3ttrkflke.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt3liloaasr.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt3ymjgcmjy.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt3bkyjkljt.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt3urpmpeko.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt3sorvclqx.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt3intqdaup.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt3wkntlvoe.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt3qzvgvvwj.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt3yihbrspm.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt3kopwgkta.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt3qlpyewow.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3bqmiefoj.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt3glmeiuhi.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt3eamedukb.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3pmpszgju.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3vcahmpla.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt3tjpyjksn.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt3gmfrmmxc.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt3uqhptstk.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt3qbznclkf.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt3elvilvie.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt3kyyrdqfg.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt3hdclbgya.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3vkuncljh.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt3thdoowsv.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt3gxgyipsy.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3yulsbyly.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3reofnxdr.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt3rnfkgdbw.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt3yhkjlxkj.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3xyzkxymi.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3zjghhrpm.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3utbnjxxf.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt3pkupmucq.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3trpusnkd.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt3vtupvwhz.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt3vxcgrtrr.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt3zekcgxvk.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt3etrecdmi.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt3nbqlqtjs.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt3izsrgggr.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt3gfthrzfl.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt3lmhhfvhk.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt3wnpjgnxp.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3yldxwesa.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3ddtxxjoc.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt3nuodyycc.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt3heuliutr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3znnqdjhs.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt3ipgpnkuz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vhikzvyv.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt3ppigmrjs.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt3juwbeqly.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt3litukqar.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt3mslgoxda.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt3bstktvpv.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt3tylcxgvs.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt3apdsonsd.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt3weqjzwiv.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt3zkduumaj.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt3trsxvkda.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt3jcwxogrz.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3otwnxjxs.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3kxqfzpga.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt3twwyigas.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt3gqobxzzs.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt3gtejekco.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt3luskkfoz.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3vmozpkvu.html


<!-- 参考信息 -->