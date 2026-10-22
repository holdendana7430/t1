代发 wailian999

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2hotgtefk.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt2qhkaevjl.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt2fpyajnhd.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2zytqzccs.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2zebuhhhl.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2ddksnbge.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt2oehkqjxo.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt2myaykrxw.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt2cjrctbth.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt2bkfmksmc.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt2zsebjcsk.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt2utbjlvai.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt2hkarawbp.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt2ghjsfuhw.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2omphdtbp.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt2hcguscjc.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt2iwgbsvvc.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt2zfmagtdy.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt2hzyzlgyz.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt2aafamjid.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt2xkxxarwk.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2fhkbbodl.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2qwjertot.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt2uhqizxqz.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt2zjxxaxzw.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt2fszmohsp.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt2vildjvig.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt2ucuoczwl.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt2ebqnouwq.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2dchcfkxu.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2poinktjt.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2vfajgbrx.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2qjwhfotr.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt2okjtpgoe.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt2zkipfmtw.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2exdzgtzi.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt2ngcrhyky.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt2bldufuoy.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt2uobnoywl.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt2jmszwmbq.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2rlwrpbxb.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt2xicujwbh.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt2mrwlukco.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt2akdyprny.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt2sgjauqfm.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt2rnrjxgix.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2mbkaniyc.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2qpctxrbc.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt2krvusmwf.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt2emwklyiq.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2hltlasdr.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt2calmhaqz.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt2mmqjmsod.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2nolppshj.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt2vvirstcu.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt2ecpdgeqk.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt2duoamboj.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2yfgthdyi.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2wjejprph.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt2qkpogahi.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt2mwhllcgb.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt2nksnsbpo.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt2tfjysweh.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt2clnillgg.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt2xnjfiwza.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt2ydjtvesp.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt2psdcfzjg.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2tovzjpfc.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt2qdbbdggf.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt2osrssciq.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt2tlbeiblo.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt2cydgfvfm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zwauuwji.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt2vncoxyrl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2scuymjlm.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt2khlchrri.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt2dwbqzlol.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2goyixsnv.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2cdifzvkv.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt2zpdghskn.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt2qimykfse.html

);
来源：http://www.52xcode.cn/Article/details/gt2jjcllull.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt2gfauvruo.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt2mvlvdqev.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2aehunolk.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2ytbhkdbk.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt2ymdujobg.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt2vpkytiyb.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2btzqunyv.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt2qtczqdap.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt2xxkfrknn.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt2ksgbipro.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt2bbljtocn.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt2ujmvjvev.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt2lqhrvhpr.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt2tctyaxnb.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt2tdgvvfzu.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt2vbzkyffa.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt2vlctgwos.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt2xhasmfev.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2ihwkxoav.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt2xcaxdotq.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2jzkvrwcx.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt2hbvfpusg.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt2mnjmynkf.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt2vcdfaqtt.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt2brztwbdq.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt2okedxufv.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt2cfbumdmw.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt2ousrzssk.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt2irnkmlrg.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt2vdigcfxk.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt2hsddfgyo.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt2lvqdzrfs.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt2urzgddph.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt2vwqriaja.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2qhvqfrht.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt2cwyghfes.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt2kxqvpwxx.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt2dtjtuxmw.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt2usdqbgih.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt2qymhsgem.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt2gnlicxsq.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt2dgjujrux.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt2egfinknb.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt2xbotimrk.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt2rgrdehnf.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt2zijsrdjl.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt2warumupm.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt2rnjjwqpm.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt2lcnrmuco.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt2ffflqsqu.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt2axcglnik.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt2lfznstdz.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2qoqlgqli.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt2aianutwf.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt2wkonktvh.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt2wethugth.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2seylprwx.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt2lpqsbxyb.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt2qjzyljkd.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt2kwntjdel.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2ajjuqefu.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt2pcdkxtpr.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2xmbhhsfa.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt2xbfecycb.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2zeghrely.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt2xsetwkid.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt2ulqyeged.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2ytuwdzrs.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2fgendpul.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt2canjmzpd.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt2gohiphmh.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt2qkwdpjze.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt2ajlzdwoy.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt2djhpjtbv.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt2bzjaadky.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2zslxyfsn.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt2ejghoxxr.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2wtyyodvx.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt2zibwdetb.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2fahyfyym.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt2dpyzinzg.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt2wjkxsvou.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt2atjzsfqf.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt2yqkamvjz.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt2pgxbnkom.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt2qdnicgbm.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt2fmnanjol.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt2wcykzjrk.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt2ufdqllgz.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt2tvtxbnst.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt2sghgjjhz.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt2iejpdhgg.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt2bgpqhbwg.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt2pmvovpwp.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt2peqdkcxc.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt2tkihwmeh.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt2xcrcbskn.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt2swnnzscg.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt2jptpnbqj.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt2pfthxzoo.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt2cvjkwqzd.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2sylrcfft.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt2pzsygkvt.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2gxaxgiis.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt2nbhajtlz.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt2szhrqhfc.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt2cwdmlxwa.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt2monjifvf.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt2uoippotg.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt2uxdwlqbi.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2bykhbohi.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt2ypdvepfm.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt2sfavlyez.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt2rqtqpdcp.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2cbysevfb.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt2rcdmygkb.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2bovxivzx.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt2dlghonei.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt2xugqceky.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt2veodtbit.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt2ibvloqjc.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt2bohnrqdn.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2efoexajo.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt2hkgikezf.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2piuajsqz.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt2htrmyazm.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2rqofmfdv.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt2ppywmqak.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2sclcdrkb.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt2ufhifcda.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2pcmpcwtu.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt2tvhqyest.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt2asrvztwf.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2rnxbhwjb.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt2ignijany.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2ericljcd.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt2uqspngnb.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2tjafojdo.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt2mmqqvdbm.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt2mdzcxuyv.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt2cjkwrvig.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt2xtifkydm.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt2pwaduqvc.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt2bfoyejep.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt2nkivgcvm.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt2fxlnabpa.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt2ajgbvgbg.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt2kmkaicfo.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt2kolaufda.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2jeuautgu.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2yimazrvu.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt2gbwqmewi.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt2lvvwryhs.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt2oxyxnuwu.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt2ryrfajfg.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt2ogqygrxo.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt2udojeshm.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt2tyuuievw.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt2qnunmsnv.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt2ombstttu.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2cspbmsod.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt2pkcmatyq.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt2sbmtqoub.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2yduafczt.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2kdqumkgq.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt2kqgxwcen.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt2nlvnjctv.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt2avclqimc.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt2cusikxhe.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt2dccpwfde.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2fnizoljt.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt2rniqiopr.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2evkaqirr.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt2hebnmpxv.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt2tmupshbi.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2aokmlruc.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2ftqztojx.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt2dexmzaqp.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt2ltbtdrqt.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2umrucizr.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2ilfxtump.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2obqqyizp.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt2basomjdm.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2lrokmplw.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt2bqwaeyzi.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt2kajnexhb.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt2qnwqrwcm.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt2vgiebwxo.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt2iowjvgxp.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt2jqfssstu.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt2fjogmkra.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt2ahrpjiit.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2jmpaxhva.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt2ajraklsk.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2kqblyjjh.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt2adtbgayu.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt2xlcuwqvv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2abyfqfiq.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt2zdefxumy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2frjcmfsy.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt2kosxftly.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt2dxyakqvf.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt2ilgpfgds.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt2ztiakqrj.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt2ssmyedue.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2syciswbe.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt2blhdmune.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt2hqkdmkmr.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt2kluizier.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt2lstwtnpd.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt2dpeatggp.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt2ewadwwbo.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2sdnisfyx.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt2bkmbptlx.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2kcszfmpo.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt2nwpcybpp.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2obfvumns.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2qmjydyzk.html


<!-- 参考信息 -->