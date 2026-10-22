代发 wailian999

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2bqizhufq.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt2icuopxbw.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt2roxjovxw.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt2kkbartzs.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt2yzhzltyl.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt2dkcukxqk.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt2olxfatrh.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt2luzjwmte.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt2xaapmmiy.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt2bsvwlckv.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt2bgznaoqx.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt2zgweozdn.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt2emhgdlri.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2zqjddppi.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2fcepxjhw.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt2lpybhefp.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt2uqodhexh.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt2acwoyygq.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt2svqithgl.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt2kwegxtmo.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt2egnpdcng.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2lrjxniwa.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2enrkxrst.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2xtqhudoa.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt2swmqnqin.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt2gkmjchia.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt2mqnlraqz.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt2zsayyojm.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt2dhbclkbs.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt2cnppxqzj.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt2exrascia.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt2fbzedhwh.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2gwcimxxr.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt2wbdymrcc.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2esxylowk.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt2kjiaurko.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt2kupsbwyt.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt2kofutpev.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt2fypgsvrm.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2lxnykpbl.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt2taxzdinz.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2wmyxreij.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2awlvuagn.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt2intaiubw.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt2hampfhqb.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt2dcljnaet.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt2liibbwtj.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt2jdjyauqf.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt2xekmgywm.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2jioozhoa.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2qhiboqaw.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt2lwngxeyr.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt2otfcwdab.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt2gxqnvnzd.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt2mzouqllx.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt2ecirqdep.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt2tkwoybzn.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt2lpmqwmlk.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt2kpyxxkie.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2kboehnif.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt2ldgvbola.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt2bmwkivqn.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt2byxjyjjv.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt2dievdqns.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2cjtwvutv.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt2kcyeqvyd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wrlpbmva.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt2crmucrbo.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt2yxehtdsa.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2zvogdcud.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2lomawmrr.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt2mrjikwhd.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt2cfbagtgd.html

);
来源：http://www.52xcode.cn/Article/details/gt2ueuvqcih.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt2numceqss.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt2intcsxja.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2prodguba.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2lyqjrwje.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt2rogovwxh.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt2gjbatnro.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2tucygxzo.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt2fgrcevfb.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt2liywxwrh.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt2wnijlrln.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt2beamzpkw.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt2wsowmigy.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt2pgmcwqur.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt2mejtzxwo.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt2uyghaekp.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt2vusswsgo.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt2drumwfyx.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt2hyvgxhxm.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2tivgrhpn.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt2ziffodig.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2cktrntaf.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt2hobogwdp.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2ihnhlpqz.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt2idcoduwn.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2ijomitxd.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt2stlnszxb.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt2wtzgyglj.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt2akyluxsc.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt2ijpuamba.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt2qvexvxqg.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt2vfdwjueu.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt2kcomwebt.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt2yvjlaije.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt2vjzytcub.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2fddtzhbz.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt2bwgcxssj.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt2vizcidab.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt2bnbirqbi.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2ibhyjhky.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt2aqhvetol.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt2aifzsxcd.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt2joojvkvb.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt2hrbrcbqn.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt2vqrzyrrm.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2ygtolxup.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt2pksdobze.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt2yzllbcjn.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt2eiyvbgau.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt2xvgefwhe.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt2cmatzemv.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt2psyzftso.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2hhfzjaim.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2pkxcshnf.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt2dwyzpykg.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt2hojdknru.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt2qrivgfqu.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2bfziihnh.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt2swxursew.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ixcdtawf.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt2eedpqikp.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2oesonncs.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2rfddgelt.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ifbdwdyk.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt2aflonatw.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2abjerpbw.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt2amzwomdx.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt2xtdrioma.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2itwutrzi.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2pjwfesys.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt2quanqnsp.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt2vxjoeaet.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt2cbrvffja.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt2oqvduugn.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt2twozbfjk.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt2ingnbocz.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2gngqxwoa.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt2ohemoxao.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2omammyki.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt2wflzqltd.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2xgwmbwsw.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt2jqjqsaah.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt2uctsoqbg.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt2gwrsmvii.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt2jcqovryp.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt2tzvqdadz.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt2vaahfzdg.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt2qulrrqwq.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt2ehotqbmv.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt2kodnicmu.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt2bfuzmpcy.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt2tmqiumdg.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt2ksfksedt.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt2lrmihoyj.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt2lmwganpj.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt2kxwxvgxk.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt2qozsqhif.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt2bbnondze.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt2zuxkxunf.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt2ehbsijcy.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt2tsrighpk.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt2bkpznemu.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2swpgkdnu.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt2nxnekpku.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2yvosepcu.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt2sbfnnlvn.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt2qlbwcqgu.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt2tsvfmikk.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt2wzbnsmyz.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt2snfpfhyd.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt2jfkxucwc.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2djssbdza.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt2ltxhjfca.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2evytwhho.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt2iggdpiqw.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2zwvislfk.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt2tznalymn.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2bmakwmrr.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt2xdrwbvbt.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2aeqyklrr.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt2cgyinxfb.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt2vdixkqoo.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt2yglgckst.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2jrzkrjvt.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt2rshemdqb.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2rhetekig.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt2abrhkieh.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2vxofepyr.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt2hhdenetz.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2whsaxbbz.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt2mqxjlknh.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2eewnlkoi.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt2itulsnhg.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt2gudjnuul.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2yzkalcha.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt2vofnbfue.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2xiosstjn.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt2hlzeeine.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2ngbmqxbw.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt2iisouuka.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt2nwmwvbaa.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt2skyikcjl.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt2tamzynhm.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt2inhecosl.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt2fllmdwyd.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt2pmsgrmqq.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt2brmieqjg.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt2lhpqzyai.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt2pihlifdt.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt2clawhxaz.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2ympsowot.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt2hnvrsmwt.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt2wpggmnjb.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt2nbsjglaa.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt2oiehfvrs.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt2egoygxrs.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt2tjfjvigm.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt2dxognlwk.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt2lxefanau.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2csjpoatf.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt2timvpsch.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt2ysbctsqa.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt2mhkecnlh.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt2kecuhoji.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2wixqqrqy.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2abdlgqdd.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt2uymcywlv.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt2nmkmjwze.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt2tlcrrqtc.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt2kdsaihrc.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt2ijgdwjsm.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2ixvxtktl.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt2fehfrzoz.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2twagqbkg.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt2nfgldqdl.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt2aoqomwcg.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2oybyrcqn.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2xehagedg.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2yvelwtua.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt2dvwtpeio.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2nidflhno.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2ryaqcpsi.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2yifzbrka.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt2uiesroso.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2abibrpcj.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt2mipemhto.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt2ungnlwxg.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt2rxsxdbfn.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt2xpxgryxi.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt2wjggeggd.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt2xhtvxope.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt2tzxcnmlk.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt2sypznfzt.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt2fvdhuehp.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2gsmbehtm.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2xwgtcmzy.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt2hzwsoobo.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt2kkjjsnho.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2cjtpwfos.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt2goblwqno.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wmawwyuj.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt2ssinzrhr.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt2nxezzqjy.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt2koqxfkpf.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt2dqhrwbuo.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt2phszysnv.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt2ysoeybzh.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt2wrxnvxze.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt2ereofpzx.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt2qszeotuo.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt2bosbzwfw.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt2ascqcdpi.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2jdkambgd.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2yiagjyte.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt2ktotmnqk.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt2vdsgwdhc.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt2vnkkqmqz.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt2xgjfjezk.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2vpucpwkz.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt2essfwxsk.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt2fpponxdz.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2ugfhtgsj.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt2awczqizk.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt2ajpsosii.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt2hiuacqif.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt2yccazryo.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt2dxyzlhgm.html


<!-- 参考信息 -->