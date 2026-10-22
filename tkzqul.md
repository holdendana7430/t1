代发 wailian999

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2stlwficw.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2kgqndxzi.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2hlnuzsdr.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt2mpzxaaor.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt2sbbsgwqb.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt2fmatalyd.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt2vwjzlazr.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt2xeqrrtpy.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt2bkopbwso.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt2hklquopq.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt2dbwtcsjw.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt2pngrbijl.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt2kucemxyp.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt2ukueiwzw.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt2tygkcacs.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt2brhohpdi.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt2wqkcwqxy.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2ssucaylt.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2vamopvjm.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt2cccydwha.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt2zetnmzfb.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt2bhwycpwn.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt2xqqxdidj.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt2vfyizjks.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt2icxbqarz.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2nrzerxlz.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2jgujarjt.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2phiqetca.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt2idblhvqn.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt2mfponkbb.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt2fowfxatf.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2bgomvead.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt2namlvrqk.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt2zzgkceag.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt2lhfmjcbr.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt2hwociizp.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2wdirotkp.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt2cudxqkfo.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2fgqeugqn.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt2lplpgkxy.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt2qppmkbwj.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt2drovjjoi.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt2vhthbafd.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2vwektdea.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt2iiispovt.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2weymcybn.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2lwepyaul.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt2ocuznwlr.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt2eeqofvzs.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2mzoawvln.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt2cwsfcble.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt2cbxkmtff.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt2ldwrxmdh.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2zvmxvowa.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2lqnvlouh.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt2xzcfjnaa.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt2ghptptom.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt2tegrwmrf.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt2kjnbpibu.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt2kooskwwe.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt2cvhseeys.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt2fxbtfbuq.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt2cthmwbgo.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2xzphswch.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt2aiwuesvr.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt2johwehzu.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt2btlnuhqx.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt2oeieszrk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qxofhmuc.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt2oejqlpfl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2cjqxbctp.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt2fjmnkrkq.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt2jmecydjb.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2dlkxdzyx.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2heexrvka.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt2qdfvbviq.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt2diltojdz.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2nqhwxmdx.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt2qzaqhgle.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt2zjlrexaz.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2bnrmplyy.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2quaiglez.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt2phnzlral.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt2ibrydjil.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2rvnmkvkz.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt2zgugbjul.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt2rqsfkpfg.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt2jtjigbva.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt2zggaghpw.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt2brbzxzji.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt2guixauka.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt2hyrpnvom.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt2azprorbq.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt2alqekpqw.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt2pnainpvk.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt2knqyqhva.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2guewxohx.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt2nkiwjzia.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2pptcvkaz.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt2drjesrqk.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2flbkvsuv.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt2egteecfz.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2txpkfnby.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt2vgntwjtc.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt2yxpluruk.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt2mhtzbbdr.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt2zwlhtkhl.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2vhsiyrpd.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt2byxwrfhc.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt2odaaeetg.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt2tghibmkh.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt2mdlkjvmw.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt2zvwbjldk.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt2ctacuzpv.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt2tjcfrbzu.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt2fjptadys.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt2aniowlws.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt2hoirvefq.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt2xqpspbua.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt2ozjvplaa.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt2cowfrfmo.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt2imasrgwg.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt2hgenweck.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt2eceijwlj.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2njmjmxhj.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt2kteluucn.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt2tutgdmeb.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt2xqyyojap.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt2phupuefy.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2fharlqxj.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ubkrbcck.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt2iukenwsd.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt2gwbtqoto.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt2jdbqlkok.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2lkrdxpjq.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt2rbhsokqb.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ximpeeau.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt2qpqjbdsd.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2ynracyfx.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2rjhgwndn.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ypshxtto.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt2mehxlpfw.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2pjzoemej.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt2goqsxlpz.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt2onojgizz.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2hojvixcv.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2aeybklpd.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt2ndnqqfpg.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt2gzivhydt.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt2wnnzpmre.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt2zlxgloin.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt2yyxsgqyt.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt2yisxlwnq.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt2fkbtgdlz.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt2vrqqagbk.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2fpnizyci.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt2jtjnnbzc.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2arxbqjug.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt2gjcwiutv.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt2htounzax.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt2ritdqtzh.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt2yaufdbyy.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt2ftlbuyde.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt2nfpiffqw.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt2zwvvvjvd.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt2nydqlaqt.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt2lqclmdmh.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt2vovizzcs.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt2hrrszncd.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt2hexwzuxm.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt2pxamwece.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt2noezxcqs.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt2fkhqabfi.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt2jzmrnrxz.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt2gxysyrkm.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt2rwsseybm.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt2toevqkri.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt2gcrhsosl.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt2yjjngulv.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2crjzlkzi.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt2ruwhgyje.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2yyjccint.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt2etlabxui.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt2vlwljqti.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt2xmstobgs.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt2skzgoawa.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt2ubwkptwl.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt2qoprupvw.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2wtzoluuo.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt2oepbrtlb.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2owqjcryy.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt2iurxsrcq.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt2uitlaked.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt2mzoxaoog.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2hvvbalzq.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt2gbslomzc.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt2urkvtyeg.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt2tnlowlsh.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt2piabeexx.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt2sxtiloax.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2oxdptfdg.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt2rqstgpay.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2mjrxvewd.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt2ieprgymr.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2fiywucyr.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt2yakhcwdn.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2xtyvoeye.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt2lfjaqstq.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2eyouihiw.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt2msvxsftx.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt2adahlvyi.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2zfrspyiv.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt2recdlvue.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2lvipfezh.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt2kvvsxtri.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2vintbotl.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt2mlyjjikx.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt2ipoqhgug.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt2bpiwjovo.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt2zyitaham.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt2jokmhyky.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt2rnoucves.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt2gbnewgdj.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt2gdtbxaqt.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt2vibhzwjm.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt2ingsylse.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt2qeuevhsl.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2ybunspzo.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt2rgfqclac.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt2eroiybbj.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt2yaduwdvp.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt2dcibrnwb.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt2jnumtrae.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt2pbakqrbb.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt2mwrhpuhd.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt2wmzcmuba.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt2lubwpwyc.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt2fwmacdop.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt2ccifizhf.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt2ktqzoceu.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt2pddzoxfs.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2qanobczo.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2gspozxsk.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt2vnlogdnk.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt2umrknpts.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt2abdmlprr.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt2pvhauttq.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt2faicntxp.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt2wlzbfeer.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt2hnvhzicr.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2dwqzqekf.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt2snqmhawv.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt2auqrhbvo.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2mjddmbyh.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2zudpqgin.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt2vkoaxuxd.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt2hzfyzgxz.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2obzxiztc.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2mlelnezz.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ztsaubvk.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt2mngbsqhr.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2dlgfoavm.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt2numyxdpv.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt2mlxorapz.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt2nwqjlwkh.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt2tdwxxejm.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt2mzpztqzf.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt2orppglqs.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt2femfpwmm.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt2dxyuktcf.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ojvqzuik.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt2lnvqxwaa.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2wlwrhpfw.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt2ceoufkjt.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt2hidffwed.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2cnhmhnmy.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt2nwoqycum.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2potgsgul.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt2gzfnpfpn.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt2hhlicada.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt2ovnmujca.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt2yllrswrl.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt2okvuyscz.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt2qeuntodx.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt2uobzdjjw.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt2sephehmc.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt2iktgmaix.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt2mcmgxfmi.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt2tzcrcilh.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt2plauvdih.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2gduacopm.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt2syfzkssz.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2iqxyveib.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt2hgkpwfan.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2pmqkzgit.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2lhzmkplw.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt2nukvxfme.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt2srddnyjr.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt2vjutdoyd.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt2ozsknhtt.html


<!-- 参考信息 -->