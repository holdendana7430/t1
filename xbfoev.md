代发 wailian999

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt2ajbujave.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt2rgxrcoam.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt2gehywbou.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt2qboxuiwu.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt2fgtsenvh.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt2gxmmjlrk.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt2xqpilygy.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt2yqktahfs.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt2cecccgtm.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2thvdpmly.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2phbibymz.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt2ptzscgmw.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt2bgwbvrqj.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt2cgkvlbwd.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt2krnyrhgo.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt2xkkjsgoj.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt2ythfcyly.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2rpijejvv.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2sqjvabip.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2suzkzacn.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2vawuhlck.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt2gcwskupi.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt2dxvudyqx.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt2bnijkukm.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt2wfrhcbew.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt2taodqccg.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt2rpxehutu.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt2vrzlxhgq.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2bzpbprpt.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt2cyvcfuty.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt2lyplzszw.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt2cnuryvjh.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt2aormvrfi.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt2hrrvcsuf.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2zwyxbwou.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2oayzcdsd.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt2fjramlwb.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2sdvmoehr.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2xesszjkw.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt2ztgxkkqt.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt2fsrliiif.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt2kojdkxqx.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt2wrzlslqa.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt2bwasnarr.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt2dzwelwhv.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2qgacicub.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2wpmdxwnk.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt2wkyzrldk.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt2ewcdjnbe.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt2kpgfrvje.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt2nvbbjtda.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt2vqiwsxki.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt2pkoeiooi.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt2zguxmdnk.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt2zhmevvoa.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2wpppdomp.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt2cpkbomlw.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt2rbarvlcr.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt2eniwfdos.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt2jzzlrryp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gyegfhye.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt2mhpuummt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jrlzwzuu.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt2xutzqumi.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt2rpztnsor.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2dhmmnvbo.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2yydpoaez.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt2lyeazjfw.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt2znrjzjod.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2thzurcbl.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt2adqzhdcr.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt2airgtkao.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2dsigsoya.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2ebtofjyc.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt2zxscjisb.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt2gbrssyuv.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2qjgcfmtw.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt2ukbbksjf.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt2qwlcitae.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt2cmsmiesm.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2msbxkwel.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt2xdtzmbuc.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt2huokawcs.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt2jmakzyse.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt2oozdamml.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt2uwsdckjk.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt2dlvqbqmb.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt2urzbqjpw.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2sujntrxu.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt2niqqzqth.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2efyameal.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt2dvfzvzkg.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt2vestdaxm.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt2nmjtyznk.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt2yophnzvd.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt2fnrglaxm.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt2wcdxypqp.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt2xatpwihh.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt2dgrwhndb.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2tflzvjvl.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt2ttqohlfm.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt2uxwhqpem.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt2nixdrzdc.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt2fasrbmog.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt2adkimpfm.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt2fbpshxhp.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ukzzohtt.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt2achgxley.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt2ntbvxjor.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt2mloovogy.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt2owcxvjqi.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt2peyamyyi.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt2arsxegwa.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt2qpwrayho.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt2djluebvi.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt2rokwwljx.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt2ihezuurl.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt2aauslpbf.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt2ixrptwgl.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt2ulxfxjlb.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt2vlialgzy.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt2alhfchug.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt2zbnmivya.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt2gjpzzjyr.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt2nudassrd.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt2bizjrqcg.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2vlihujxy.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt2nvprxman.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2snwtenqs.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt2dyrioenx.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2kfnpxpex.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt2qyiaxxsf.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2hbdflyec.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt2rcrrjnnp.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2kvkmtxxk.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt2zwfvnwnw.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt2ikvezssp.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2gatcwhbd.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2ikovzaxh.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt2bhbrynrw.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt2apsemmhm.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt2esgsglvl.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt2fqcctacg.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt2cpvyycey.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt2dximnwsp.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt2pgsmljxu.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt2anvvyuki.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2mnkknlly.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt2utioijch.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2jjdeppuj.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt2ilxitvow.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt2endiptag.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt2tutetsud.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt2kqhmfccj.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt2jaklenoi.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt2mschgbht.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt2aummqlmk.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt2tgctgjqk.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt2djcyuzei.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt2fpjltmri.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt2chhmtruu.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt2vgutfzkq.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt2vuobkzzn.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt2uieluniu.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt2cozzgjpt.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt2rckvyujt.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt2rxacqmrf.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt2urvqlski.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt2ugvixvkz.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt2nadzvpvk.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt2dcipkpzh.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2evpjosnk.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt2xnloduhy.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2rfomywfa.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt2yxyrtumf.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt2wtekvuzv.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt2qhxhydnz.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt2wqomkjha.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt2tnhweqlj.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt2awlqxjvb.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2dfdawerj.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt2kbqfmfwb.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt2bqcjodoj.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt2lprfeblb.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt2xwfyyqkz.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt2bmdsnbyw.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2yrekrhbd.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt2vtakilvn.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt2fzhfklhw.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt2vrzncnpi.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt2baxdlmti.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt2gsoegjdm.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2jpzhssxw.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt2xleumkja.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2srrnrrkz.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt2qcdajtgj.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt2jalzicdm.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt2lqtjrpji.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2yertdaaf.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt2wbepipxa.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2hsbpoxpt.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt2vnifhvmq.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt2ulnhcfnk.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2lpxdkhoa.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt2rmxdswql.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2gjcmhbup.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt2rxxanjvx.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2xrxvkhig.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt2vurcmgcf.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt2fxexktzp.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt2slnikslh.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt2okvbkuvr.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt2hvbucsmh.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt2bcgbbxjm.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt2blpzyfqt.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt2itxriykl.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt2xewutifw.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt2qabclrbn.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt2pomyddoy.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2omwwdgdd.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt2yenclfvu.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt2xejqgzcz.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt2uhnrleyv.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt2iapgpikn.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt2evxhmuqn.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt2cwhkpwfs.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt2ujqzcmjv.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt2fwgkcyvo.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt2eqckkvzl.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt2faymgyny.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2wheuwgei.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt2igjyckki.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt2yrghmntb.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2ltsnqoys.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2tlkequst.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt2ablgkphy.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt2djgnwnys.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt2ebtstdpi.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt2nwmmezom.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt2rbtbjmoc.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2coitrslu.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt2iffpivhp.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2bxpkpytg.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt2gshncopm.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt2fxuduoay.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2pjuiwpec.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2affveawr.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2lobkljfp.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt2ebzkbbea.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2fjlsdbkk.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2oynukqyj.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ndsfjqml.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt2ksabpnau.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ijfizpxo.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt2ysatxobl.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt2ydpbsiwy.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt2kvgzvdcw.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt2ebnjcywf.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt2rjunmnif.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt2sofxcxoq.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt2wijoycdv.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt2yjxphivz.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt2pxocauhs.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt2gtrumjfu.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt2abptqlgq.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt2ymmolqde.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt2rwuqtzfo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ieggspmg.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt2yxmzksaf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2cpsnbbrd.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt2wybsyoyv.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt2czwitzwq.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt2ekhfqkym.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt2ohfgbnfw.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt2rrhgafwg.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2leyzjtuz.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt2mdzkwbpi.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt2ioeqhwwq.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt2tdhlmgij.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt2gsigvcze.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt2qlmkgvtr.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2ckbzlupg.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2qktrpcpl.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt2avdhhucm.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2lpwhkmkf.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt2vbbsimay.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2smgecjkh.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2vyrvpatu.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt2nwuvhgcb.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt2vqqfiekq.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt2nnhzzzlc.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt2fafgeowg.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt2pruadysq.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt2fwecrczk.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2ilnpgpsg.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt2tggbvbfq.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt2jtejognw.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt2juncxuuu.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2rqhjumjq.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2labswqpx.html


<!-- 参考信息 -->