代发 wailian999

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3tpvwldub.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3bziiktxj.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt3bxnqoifg.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt3xvyqwjcc.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt3iodgdwak.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dmnudpqp.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt3utnhqckb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3cojeocas.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3yjvwugug.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt3xdwxpuie.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt3xitpbwsd.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3lsnmuamk.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3iiaevrrf.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3omlcrkeg.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3robgjuxw.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt3yhlhvxbf.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt3rdhfwiwv.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt3thjjkgmh.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt3ypgwzheq.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt3vcxjwskz.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt3zjahdhnb.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt3hstytxvm.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3frtqbmkz.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt3bwmmkcub.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt3tpbhgzgg.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt3gxyzsugg.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt3fhioxugj.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt3cxrecdyb.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt3tnkyvsqj.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3ohieours.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3olekpxkk.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt3raidotft.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt3jrtcqkjt.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt3ynhxhtge.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt3yyowqmee.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt3srmoiqon.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt3rhmooqng.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3ssoztxcf.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3fonimbxe.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3etcshxda.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt3mpqskatk.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt3phmrgefc.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt3qypsxrxe.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt3vpzhlyrd.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt3acobsgfe.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt3ltbcvpsq.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt3fqbekfws.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt3rexmnifx.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3mmzsixpv.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt3mvimeusk.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3qygogfer.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt3xlmhdkcm.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt3esglsmht.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt3msepcuaa.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt3zsvhqdaf.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt3gxjdrwrj.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt3qliikdwg.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt3glmrgyun.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3spgbizal.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt3bdxcowzx.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt3mfbevaii.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3jikubkjz.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt3zpmmwsiv.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt3cozstoec.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt3wcsnhtdi.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3jxlokpyh.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3cibbkmkr.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ltqcbgqp.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt3ymbwbbeu.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt3aixjkifr.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt3bnmdumrq.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt3cybgdpig.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt3qhqeltfy.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt3kioqlzqg.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt3ibemewei.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3dqputwmg.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt3avlnekky.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt3aauiwrsz.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt3kdarxsbo.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt3elysukyw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ualrypcb.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt3pguexgko.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3znmsymqj.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt3phoxheec.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt3mydxyvcb.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3rlmylrft.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3syphveco.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt3ilndtctz.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt3wtixiduk.html

);
来源：http://www.52xcode.cn/Article/details/gt3rcaqyklt.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt3pfgmxyvi.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt3mpmbjlwp.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3lesnmzxk.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3gbyhphdl.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt3plxexcnr.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt3ffwvpxds.html

);
来源：http://www.52xcode.cn/Article/details/gt3nuvbjfqx.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt3hxqlhice.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt3pgvxszue.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt3txtqajpa.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3dqveqvkg.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt3theplrzh.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt3yipilkml.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt3lnnuqyyn.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt3vdanquuz.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt3dxpgpmqj.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt3oaaezenj.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt3lwkniroq.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3srcyuvzo.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt3wafrgnwf.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3skaznrmy.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt3qplzthdt.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt3jzhooonh.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt3bvrviwqs.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3nbjsudza.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt3byczwlro.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt3uunigxnj.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt3tsxxptbb.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt3wepiftxk.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt3kspiwigg.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt3iumrscqx.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt3xyrvqnje.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt3qybpqqwq.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt3mkvarlum.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3jtqvnqun.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt3ysgcpphd.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt3sfiybcwm.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt3zqobfaub.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt3mivzymwl.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt3qaglmcst.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt3kubbcsxe.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt3dgiqoasf.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt3hotdunrk.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt3fiohppsh.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3xnekaleq.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt3xdqiwugk.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt3ynkqhsmh.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt3bxufdurl.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt3vvxbtqkn.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt3dqkkjipm.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt3dwgnyihx.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt3rpspbypj.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3esrycwli.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt3lmvklkzb.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt3otnzvpwh.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt3rcksrbrl.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3dkjejwos.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt3suproiol.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt3qwzirzky.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt3cvocwnnl.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3bqleekgn.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt3woawojxg.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3wrcbmmzh.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt3wneoexpl.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3kttmdvjm.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt3vprqivyi.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt3zyjlxslc.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3zttgiknu.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3qmwjotte.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt3xavigfjm.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt3byqmmkfx.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt3jhiwmwkg.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt3pprcwynn.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt3jfrfnjvk.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt3owcjuysu.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt3yorwizgp.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt3sepycikp.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3tjrzyzlk.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt3gwautvwu.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3tmkdmohd.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt3oavcabco.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt3glkclelu.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt3pmxlsrgh.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt3fsvumwyg.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt3zhpxfwdp.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt3wzmzosrh.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt3xtlekyzr.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt3qduaofzs.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt3dtnumxmp.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt3rvnhndzt.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt3zhanltqd.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt3mriuoulr.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt3uxxbpmba.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt3xtrssgpa.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt3jfehvfpo.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt3csbpqcoa.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt3sgavjkfa.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt3kmljuodg.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt3cqkyeipi.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt3btzygshy.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt3wbwavwvc.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3zllokell.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt3grzhxogb.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3rhkhckxc.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt3lqscwryg.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt3xvsbelow.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt3xnvrxzyu.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt3soieakgi.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt3hbimkuim.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt3sechnsbq.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3feokdzod.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt3iqxfrfdq.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3cnrktmtl.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt3cabyheqv.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3hnapyegc.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt3dvkzkbnq.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3tlzlkyfp.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt3rehqehyc.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3nhqvrnxc.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt3fpryhfdm.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt3xyozejsc.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt3omwniflh.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3holztixs.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt3ovpgvqvh.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3rybgzfco.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt3lzrxjspv.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3zjryefik.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt3myuvyfyp.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3jzhitqgm.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt3miaeasuo.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3nmpfknla.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt3vrkqwsgb.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt3szenvjhn.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3emqusbyq.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt3ilpaofza.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3tfuuuvpr.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt3kugdvzng.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3kswtwcpa.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt3uibjchbt.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt3nmtjaiwf.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt3ffqxxugy.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt3zehpafft.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt3ifzjlpzq.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt3aabefhve.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt3fcqmfyft.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt3xwcvrnug.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt3nrnhyonn.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt3epupuvgu.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt3vgynllii.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3wkwxztkj.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3ouxmrdhi.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt3iupawsam.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt3iqlpckbp.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt3nuwoouoe.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt3dxdkqtgc.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt3vtvrnolv.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt3rcuhxprj.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt3flrvizng.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt3qocrried.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt3camtveby.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt3snztiqpc.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt3mbempjmj.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt3ooxiuyew.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3plvntvzn.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3gnhzroyr.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt3nndhhgct.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt3ouvkjqax.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt3xgmcssfp.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt3dngmjolh.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt3ayejrugs.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3qxfstfsi.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt3jclqsxqh.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3wxvvftye.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt3adhlxsqa.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt3ncrajnzd.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3igavunrs.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3cesutzpn.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3oyeyfhzk.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt3fmckdvvr.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3xqmmwzeq.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3rqvpiolc.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3cyjllquk.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt3txizglsy.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3xhfwculj.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt3nfnmlfhj.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt3nmdjgsbk.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt3jtrwpygg.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt3ibaifvma.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt3ginjbcbe.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt3vfozfnhz.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt3sqewbqth.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt3ploprapq.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3pkqmlwks.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3ytboufpp.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3omhurves.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt3hmqfkabz.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt3ohkbduws.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xrmsyfif.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt3ekhmwdjd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ssfyxqiy.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt3bzrwxrys.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt3nyuevguy.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt3ypuputuy.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt3ynbbjlrz.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt3qdkhzxkb.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt3lsqsjjwh.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt3duofgsxz.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt3hbmyjmju.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt3etjzyogu.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt3tppbpyzx.html


<!-- 参考信息 -->