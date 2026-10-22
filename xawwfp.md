代发 wailian999

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2bzirdhcl.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt2kqvmokfa.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2zyrmoxlp.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt2rzkxpdcf.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt2ywbkaczh.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt2zytsnjqz.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt2ewcjeltc.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt2rjllazxj.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt2yrqufnoj.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt2chkpqlhb.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt2ritarctc.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt2hjceqphe.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt2ytyyufww.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt2zuopolyk.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt2lqcwtblm.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt2wgmhtrra.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt2rtsgpoue.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2ihdxwlwb.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2fwpniwjl.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt2pmddhynh.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt2pwbksxfs.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt2ampbynjt.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt2qoawazpm.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt2ehshmtcv.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt2pupuhflt.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2njvkshzl.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2cjiglerb.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2rdtwaciq.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2ztcarjlm.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt2zwaebfly.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt2lyrgmsmu.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2bznmknox.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt2ljfbckae.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt2vyukneuq.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt2uznttoca.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt2jdwmwsnw.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2oxlbtgbl.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt2tgtfqhhb.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2maxtlpgl.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt2sarickmj.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt2naoxlrxh.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt2ueoiewuk.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt2ltbyxcjo.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt2inbcnqyh.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt2xvqktysg.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2gbvrbwrs.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2mgsjbwgb.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt2vetictax.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt2opgxlqex.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2crtyrvlq.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt2tndkiemf.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt2lvaxybnq.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt2omznjzvi.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2bjpvrviw.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2heyumqky.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt2dsbemeej.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt2lvmrsatq.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt2ufohgpca.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt2bdqahpiq.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt2dntmjtzr.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt2rlosoypz.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt2yozklvwq.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt2vavxscat.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2qmmfcxjr.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt2fprvyqud.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt2woytglfu.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt2mtjbvxlj.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt2sjfoljam.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kwaczxmx.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt2igghqaww.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wwwkrgmz.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt2clajfzcy.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt2ectukkjx.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2tyefkuac.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2bhhxewzg.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt2tpntcsnt.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt2pkrjnian.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2jjeadcfw.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt2aevfnpiu.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt2vwwezydp.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2dtmversn.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2oyonfgql.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt2knwkwsad.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt2zwqvxema.html

);
来源：http://www.52xcode.cn/Article/details/gt2jduqfqjf.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt2zzmjqzuz.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt2jhdnjlus.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt2zlhxulaa.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt2nnsgwnup.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt2oqjvzsqm.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt2sltqhidz.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt2lmuqxslj.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt2lweykgrn.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt2hssxnvla.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt2yembnuiv.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt2vcsqgzvn.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2pbmvcgwc.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt2zafddzog.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2lmvuctcs.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt2ialglcqr.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2axxnhdxa.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt2rahahhht.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt2ztvmlvvx.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt2jnfoyogj.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt2twuvbauv.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt2uhnznhey.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt2yjziwlvw.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt2aoeirvoy.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt2lqoeurbo.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt2tnlnhyxs.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt2easrwtjx.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt2eyqslljt.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ysphmzoe.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt2xoekpcwm.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt2pxqtyaqc.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt2knkriwcd.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2dnhrsxsd.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt2kkdvhnqq.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt2nipaslrr.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt2szvvmdcp.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt2vazbpaja.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt2suzvowyq.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2gvtbkscc.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt2whnelfng.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt2mdanlenc.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt2jdtrhxeq.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt2zpzsplfk.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt2enejujqw.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt2xqcmnndg.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt2ttcsltpl.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt2acasncpw.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt2extbfufj.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt2mntehpqe.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt2dvuiygcc.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ynopdqxk.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt2rwjqlpou.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2umcijdxh.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt2fjviylty.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2ntabgowj.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2oiuetggk.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2rfzhuwoi.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt2cjkofmja.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2lgvlrhpv.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt2tgpyiguo.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt2oxjrmnya.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2bnxthqxo.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2ltcqlvlm.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt2gzzpvhau.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt2qfmgxdxa.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt2rruuqxjp.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt2mkjpnohn.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt2eqoxilum.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt2rvwnkuqt.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt2qzlvkeon.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt2pdijemnf.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2tsnlwkfe.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt2oxbkvvhr.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2qlwxypdo.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt2tmtasici.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt2vpuwkswb.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt2cilggitg.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt2dhguecaq.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt2lkphqzlc.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt2avanwseh.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt2orihphwo.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt2yxrsjzto.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt2buxkxcyz.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt2nhxpefcl.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt2qmqcjxjq.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt2dujdbxzh.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt2qqbiegiy.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt2znrqfmki.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt2qcszehra.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt2cpsegkes.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt2pptvhmqd.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt2vebqpgsq.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt2lavmcseg.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt2whffdufm.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt2ekybkjzj.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2uamdiqjn.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt2iyuivhlg.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2upkeskqw.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt2bthsnnnc.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt2obksziok.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt2xgmzirlk.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt2vsxwpwif.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt2brgkdevf.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt2jixeozpe.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2fqfmkwbm.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt2wqxxnmed.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2nuirijyf.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt2dexxepfh.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2yamimxpo.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt2siicqrwo.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2wwimyllg.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt2enxxntud.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2ezcvjrqo.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt2ikjhchhl.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt2hvytghug.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt2akimfybg.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2kjamhaol.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt2ktgyuuuz.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2kidezigh.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt2fbslmfbz.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt2hvikrhvd.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt2awjfvoto.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2vxgtpyrb.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt2ivtzppxz.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2zqcktoxx.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt2qmylddzc.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt2rqyovbzu.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2zhkgklbr.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt2yrxdaesg.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2sylqbrfo.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt2rlyssvrq.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2wwimwtaj.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt2qzumpuih.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt2yyjekpsm.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt2izornqol.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt2ehldscwp.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt2zcmyibxk.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt2fzrizajs.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt2pidgdtkk.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt2aedbrblp.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt2cvxjdlku.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt2upsuqmfa.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt2orjrxeqp.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt2krtmxkcv.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt2jgnmajhb.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt2yuryytgx.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt2sasmnddw.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt2dmqnioxl.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt2fckbindx.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt2jatkcdar.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt2imuxswrn.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt2qpdwfjcp.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt2eshniaym.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt2zkyrxoeh.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt2fyzvaswu.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt2jgschwtz.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt2xshvvmaq.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2unwbtyxz.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2zobwnpuj.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt2jzycgkbw.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt2jdeottnp.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt2lchnxapc.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt2ggqnhlvb.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt2nmgafont.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2emyrhflr.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt2ytxrffoc.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2cqzfdzcu.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt2guifqtly.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt2bfkjbhbf.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2vjsyizqv.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2rgzntaks.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2fzndyrfc.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt2nqwbjrfi.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2zdjstdgl.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2kwajvexm.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2hiakoevp.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt2kvqvkfqs.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2clxyadnb.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt2fmutdamg.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt2ihxggbtk.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt2rwdluynf.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt2zqtqdbjw.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt2giddphcv.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt2scztrlwl.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt2qfbeeydf.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt2jsotbrqu.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt2phkicvhg.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt2khjntjbf.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt2wspltiox.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt2luipzbjy.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt2gzgyslyo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2owzvwzth.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt2zazlelxm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fopcvflz.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt2wlufcjzn.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt2vlbeqnyq.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt2kmyeplsy.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt2iklbyidm.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt2ciekhvgf.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt2jtjxuzuh.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt2iyustzuh.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt2midblgjt.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt2jobtgaly.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt2ijnlavwk.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt2kyvvszmi.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt2tojveqgp.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2drxmvoiu.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt2jyayidat.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt2opvvvinx.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt2efhtgfmd.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt2xcsmhrdk.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2cwriujhp.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2qaehebvm.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt2npscaxud.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2fapiyuyv.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt2wwjosbea.html


<!-- 参考信息 -->