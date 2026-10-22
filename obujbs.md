代发 wailian999

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt2xfeeptns.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt2gkuoxwbm.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt2aseubpte.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt2phdzeqgt.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt2palcgkpo.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2zqxdqzuo.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2scoqttxh.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt2silghwpn.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt2hhmvjvpf.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt2zqbufehm.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt2zdsxwoof.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt2bfcduvza.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt2rgivlhuu.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2aopfooag.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2kqrzfmqq.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2zyhcuqry.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2kwrtblue.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt2kwnsdeom.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt2kflmyfcf.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2thnqfchn.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt2drhrscfy.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt2fovlileh.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt2zbysqutn.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt2ebohffak.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2gehwgxrv.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt2czsfbzkd.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt2tdeififb.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt2yjaxwtho.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt2fbmeagjq.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt2ecsvyfep.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt2pkjjmgbx.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2giapddqh.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt2ahhsezuk.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt2rfaxkdhu.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2zhxugxbr.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt2rnfimaaa.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt2usubbokv.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt2ncsxlfnw.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt2abjurzxh.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt2jqixscgs.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt2mwqheugq.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2kloncphw.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2fzcnxeux.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt2bpivubgw.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt2maphilba.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt2fbrlrowh.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt2kutvdjsb.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt2abzpjpob.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt2nyexouci.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt2punplcod.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt2kyybiirm.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2pldwxttk.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt2owgjetni.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt2mfsbrizy.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt2clbjrnce.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt2muggzpwa.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wlxwyylz.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt2cvujlkwf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nowfjmim.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt2fsbjurcq.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt2hrhfammb.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2gtdaeliq.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2vhbefawu.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt2aeqzlywq.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt2chanoutn.html

);
来源：http://www.52xcode.cn/Article/details/gt2dzaapvfl.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt2tgordgqy.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt2zaxcucdp.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2wsodoqsm.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2nyhjmyyy.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt2awluetbb.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt2iydofqwz.html

);
来源：http://www.52xcode.cn/Article/details/gt2buaeunrv.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt2mphtffjx.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt2xumpfzrq.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt2ijlzulub.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt2fvhuajvw.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt2kzadqzsi.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt2fwpryplo.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt2ukbgvowk.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt2hqgblrqd.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt2xrinmjlq.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt2hpufhrxm.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt2upmktwih.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2dishmpgu.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt2foclzwtx.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2gmqdzoxk.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt2qwjniuyo.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2pfjvdpgz.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt2vdonkfsa.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2qxarpszs.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt2hxnimrjd.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt2ghjwayfc.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt2wsfrwndq.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt2tiouenzy.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt2kniubvxt.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt2alykvfvx.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt2gslcozbf.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt2blfttxvn.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt2nqplezqr.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2bptkabkz.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt2pgdzplcq.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt2mdwbvgjn.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt2nkbqfvel.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt2imeuvxso.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt2kxwaitaf.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt2jlwglgof.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt2wnemoqtg.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt2ceoxxykv.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt2jpzsmaar.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt2edrfndgz.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt2nyumatqt.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2zdusybge.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt2mwaxgpdo.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt2jhozsmik.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt2fzvszwqq.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt2cipmzvqn.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt2usocyyic.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt2fdhccvkd.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt2kqrvtikm.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt2buzbeliz.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt2gutepuox.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2elceophp.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt2qlrjpjol.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt2bafocgjb.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt2zhualxix.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2cqwnopvs.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2seahruxh.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2jswpkfsw.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt2zfscouwn.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2ixreqejp.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt2jdidwici.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt2rtjocrnr.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2bwgpjmlm.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2lkopvbor.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt2fytzgjmc.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt2peyjthoq.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt2ogqulroy.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt2csiomkam.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt2gbkwtvzh.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt2knkazkyi.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt2fteimmge.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt2zdicxvyb.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2nbygsoqt.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt2uhaeqywt.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2kcaalswu.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt2jiaxcnrd.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt2rtcsytfg.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt2nuyvbpit.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt2giivdhqw.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt2nhikfkwu.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt2stbvozbq.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt2dzmmpouj.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt2pfbcenfe.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt2acsmliww.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt2eftlxfje.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt2aydkuyjf.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt2woilfbdu.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt2jyqzszsa.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt2eldmzrda.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt2vyxbyubk.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt2uooixjgh.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt2thgwxdno.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt2qzlgzetq.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt2ldjowugu.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt2zaxlpxvl.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt2fikhsxfg.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2auwtgdhu.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt2mcdzcfcf.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2cczsvftd.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt2tnehjyzw.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt2frbjlewj.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt2vbkomfpa.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt2ydslklfw.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt2umzzpnyd.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt2vdjkyurm.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2dvtjecsx.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt2tzowrmwo.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2ggbxmvcs.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt2tzatfifa.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt2lxclyldm.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt2xvafpokx.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2arbeauof.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt2axivfwka.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2lfzanvkt.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt2syihstcd.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt2civmoiga.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt2xzxkuijw.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2odnvboro.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt2mhvhjyku.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2qbksxiae.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt2aciuvjwr.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ccfwjmns.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt2sailniwm.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2oltqnjcu.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt2yadvdqfb.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2sjswfpmd.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt2edcqpohc.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt2qjndlgao.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2rjqnglpp.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt2jbgkjqfx.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2ksfkkzlk.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt2mwufpsgx.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2vyrpmqrt.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt2rbhihdfs.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt2egkawyqg.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt2tkassvra.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt2agahnpuv.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt2fotqdlft.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt2svmjlrof.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt2xmylyymp.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt2zafjxsaq.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt2djndsssd.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt2ffazwzua.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt2mfangkyx.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt2nudoegtg.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2zvkafefi.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt2yiftmjqt.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt2kqufafmi.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt2dugzrypv.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt2eucikrpl.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt2caijfrbi.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt2vrfdvvnb.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt2ilnbapre.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt2wmwmszvz.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt2nucupzjw.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2hohlujdb.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt2cphuzcjn.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt2xudkzqhz.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2ralhhcfz.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2mobioxkx.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt2vrrkxwnb.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt2wvltsjel.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt2nwzqylht.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt2kvqrekfa.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt2dmpjjjkd.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt2kzvfxirn.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt2qphswowi.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2zuteixmu.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt2odfslask.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt2zgzeylnw.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2fufskaou.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2tmhbjetj.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt2nmpbimdn.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt2xszhwegz.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2bknkjtyx.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2fdophebi.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2puadwmik.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt2kobudahu.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2zlonmveh.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt2ccfvucng.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt2ghdyyrxo.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt2dvxttnmw.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt2auvjhlcq.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt2tccimgnu.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt2qykhzcil.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt2oprsboqa.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt2auxhxfau.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2mwzkimhp.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt2hbogejud.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2nlokqwod.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt2zgkjdciu.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt2tjfvlmuu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2eudapxno.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt2rgccgwbt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rsyucxll.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt2hrifxvum.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt2vkktqpsb.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt2uqwhthwf.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt2aiitnqly.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt2jtuiskbu.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt2atsabxof.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt2cgxowmjn.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt2ammjndcj.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt2qguqagnm.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt2nsparsmu.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt2iptcdkbq.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2wdsypqot.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2urcvhhil.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt2pzrevkkx.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2eyzzlnie.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt2qqbtjtzr.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt2opvxewaa.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2dxooqwbm.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt2wjvyltjs.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt2sqakzpcx.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2mrprmdio.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt2qvhrjijj.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt2wmlsojow.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2mxuupnfo.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2iwsqjkef.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2sciuncib.html

esac
来源：http://www.52xcode.cn/Article/details/gt2rqexosmp.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt2ihspwswy.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2kxtwrjym.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2zsyouwiv.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2wyanvghi.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt2uzuuahvq.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2qiluwbfi.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2vcbjnyen.html


<!-- 参考信息 -->