代发 wailian999

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2kqrvjeuf.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt2gqlmimpf.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2aoadudec.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt2kpsqkjdl.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt2djrubjhb.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt2jurhslcb.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt2ubmkhibn.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt2umorqkbp.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt2xmeaqizb.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt2kmlynrsv.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2gbswtuhk.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt2oeqpaqqx.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt2hjgtjtzb.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt2ahpizzrt.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt2ruexywzz.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt2datwyrcq.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt2yascalhw.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2axuowwxg.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2vcbnntee.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt2tjksjsja.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt2ullnziro.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt2vtertxju.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt2djqqkeik.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt2pjxvcboj.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt2wercshvl.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2ankhndxc.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2sngeexci.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2unkkjfnd.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt2cbehyaml.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt2gybwcswm.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt2qqtmaizm.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2nqciynbr.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt2ohcbcpoz.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt2pnkqaiyk.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt2hnpwxwni.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt2xczcybvz.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2vwqwvoxp.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt2xwsepder.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt2lywzjgdm.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt2rnpmicgb.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt2ckcjrrxt.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt2ixxepmtr.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt2ypdmtirm.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2fshazuzu.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt2upienjzk.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2jkkhlpfr.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2yhppxlzo.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt2snmmngwl.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt2imgcfomc.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt2flshuipo.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt2nncphnir.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt2eofijniq.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt2rjtfxcpu.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2dbavckcj.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2objkukir.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt2zrphmiqa.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt2pytumfzy.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt2nhwfvyll.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt2zbhivrmw.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt2yxzcitfz.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt2zzspmbwi.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt2atswfuan.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt2teztgqwv.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2yaiyrysn.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt2ytazzzuc.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt2jrgfwsuv.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt2eavpgpqy.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt2qvfzprfv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2khtkwndz.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt2wqrysyox.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gfojehhd.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt2daukfoov.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt2fksaptbo.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2fzvmddci.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2wazmenjj.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt2iyidniif.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt2fgtdwrdf.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2cfgbbvph.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt2ziusvejr.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt2pcpjwkng.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2jdktvgcw.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2ykjhtyem.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt2nomzfdjt.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt2fhjshyyf.html

);
来源：http://www.52xcode.cn/Article/details/gt2elpxgaog.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt2dsfqecfs.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt2kiiklove.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt2voahjjpw.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2zvvqcqkn.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt2wlgvokze.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt2obhpwdpa.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt2diqdnpgq.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt2zjafrjej.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt2zobakkvk.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt2idvydgop.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt2khetmipx.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2lgmipwtf.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt2oryutrba.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2vuhgpyfw.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt2ofnvewxl.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt2tslxcjzy.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt2enyxlmmn.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt2osvbfvrm.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt2jxszpzuq.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt2qelvzuox.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt2pjktrtwi.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt2dvygcsrt.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2gwaganbh.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt2nfcprepa.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt2svrtjjfq.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt2gnbfgoub.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt2lmywdbwx.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt2cmufemjc.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt2laxrzqmg.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ddvzewrb.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt2doxfpbot.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt2vxplpmqa.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt2alqqtcfw.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt2gmvbfbae.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt2phkilzjx.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt2ayppcpig.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt2fyolvmun.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2ioegumdq.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt2pvekckni.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2llapbaen.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt2ibuzgpet.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt2ykbykeif.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt2spopnakj.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt2anzhyjqm.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt2mxdsbjvo.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2rgqtzgbz.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt2jujlsady.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt2usnwmvfx.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt2izpvdrll.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2letqmamf.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt2mgtgbdcn.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2dakableh.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt2urxjoudr.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2xfqedbjp.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt2pibnlbyi.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2eymbzhxs.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt2uwhcpyyz.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2ldybtryd.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt2wfzrvzmj.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt2rrfcnzit.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2wlqeaooj.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2fpsxqsqp.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt2hjatdrlk.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt2wbjozsgw.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt2czeykyuw.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt2gugbresy.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt2muxdfazk.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt2rtzpiqoy.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt2sdgczhpz.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt2rrvgekfi.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2tfrpgkjo.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt2zjiqijuy.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2fqkrydwu.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt2jfxrfgpi.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt2ctkwddrf.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt2criqlyqg.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt2dbxzbrvt.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt2euczsook.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt2srktqzfi.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt2tfkkoujr.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt2msvmrdqm.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt2ztbtredo.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt2wvwctlgl.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt2qielolqc.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt2snmyavch.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt2juqrxtga.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt2wuaailke.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt2cnrcsqpn.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt2nawqdiyq.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt2sfazjbaz.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt2kcrkarnf.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt2hjbzzens.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt2wbhhbepq.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt2untlsqnb.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2ecbeyjcz.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt2vvxjrreb.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2jypkxgpg.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt2wpfigowt.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt2nmcojmkc.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt2aqzpvgur.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt2pzpvzlzt.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt2xngumzjt.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt2fczgbllu.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2qvcskelg.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt2tedgkjdk.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2qduznyyx.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt2vnmfrvnz.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2vnrwpwnm.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt2gcuwynre.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2pvwmxfll.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt2vrowkkkw.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2kbcbatys.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt2entsnymp.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt2qgjbxacp.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt2wsspiyxw.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2tcpnrxti.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt2congrcig.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2lrpwnova.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt2duvhalcb.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2bzomcgnu.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt2kucyivfk.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2qyorhwma.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt2rpbvfaun.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2boenieth.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt2piuepiuc.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt2vwfjmern.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2kjpvdbet.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt2pyjvqjlq.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2hdlwgpgg.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt2bvrrmxub.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2uqiopvli.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt2iofeqlyp.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt2epvlsoqr.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt2bssmmeal.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt2upsstatg.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt2klkxbveu.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt2kptebwtf.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt2tfjkrjcr.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt2tpidespo.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt2bdzdtozl.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt2ulyfstdo.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt2bosjbxgj.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2butaczpq.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt2wlhvjnwz.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt2lemnxyem.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt2zoxxscnz.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt2dsajuvfu.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt2sfswngqw.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt2mrmicsqn.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt2jandlcjk.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt2qgtxuigi.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2iroipliz.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt2rwhmhgnb.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2wgkkjlmx.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt2eutjssrd.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt2zsgyvqsd.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2syqqrmlj.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2pgrpttkl.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt2byehxnfs.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt2mwxvyikd.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt2dlsksgml.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt2inuchpjb.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt2pqcwbnvu.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt2metoxhgh.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt2apeszmzv.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2udhtgvjy.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt2ihafwbvv.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt2xtnaxhum.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2pmozilso.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2diqqxjyd.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2kagmvzvp.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt2hxajncxc.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2vobbkczm.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2jepyhxmk.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2hgmcpnrs.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt2quiccmsk.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2czwzfymj.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt2khmeaoef.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt2uqnivksl.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt2seaovmyl.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt2xjcdnlwe.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt2dzjoxatd.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt2tkkyttyg.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt2yyfewdbs.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt2gfcdftll.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2qkqxvipv.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2xcustxdb.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2fjmqxhfh.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt2hfmjabeu.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt2zzyxsdue.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2juimqqwq.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt2xzlypjax.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kymppmcy.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt2hvudbpts.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt2czeyelua.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt2rwlbagwg.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt2zxlrtfew.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt2tdzfnncw.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt2ljkvkjfg.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt2dpxexerf.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt2fclfenlr.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt2snxflrid.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt2qecatykk.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt2lhvohtfi.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt2eltquqzj.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2waumgqbb.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt2ygmbosyy.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt2yufaagyu.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt2setkinyv.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2iimxbflh.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2redveegg.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt2uwpvgwmf.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt2leztlctp.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2uqqlkxsr.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt2njethwik.html


<!-- 参考信息 -->